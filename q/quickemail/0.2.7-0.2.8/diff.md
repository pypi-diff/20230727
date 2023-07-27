# Comparing `tmp/quickemail-0.2.7-py3-none-any.whl.zip` & `tmp/quickemail-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 8624 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    28591 b- defN 23-Jul-26 02:53 quickemail.py
--rw-rw-rw-  2.0 fat     3025 b- defN 23-Jul-26 02:56 quickemail-0.2.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-26 02:56 quickemail-0.2.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-26 02:56 quickemail-0.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      381 b- defN 23-Jul-26 02:56 quickemail-0.2.7.dist-info/RECORD
-5 files, 32100 bytes uncompressed, 7916 bytes compressed:  75.3%
+Zip file size: 8766 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    29106 b- defN 23-Jul-27 06:15 quickemail.py
+-rw-rw-rw-  2.0 fat     3139 b- defN 23-Jul-27 06:48 quickemail-0.2.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 06:48 quickemail-0.2.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-27 06:48 quickemail-0.2.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      381 b- defN 23-Jul-27 06:48 quickemail-0.2.8.dist-info/RECORD
+5 files, 32729 bytes uncompressed, 8058 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: quickemail.py
 Comment: 
 
-Filename: quickemail-0.2.7.dist-info/METADATA
+Filename: quickemail-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: quickemail-0.2.7.dist-info/WHEEL
+Filename: quickemail-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: quickemail-0.2.7.dist-info/top_level.txt
+Filename: quickemail-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: quickemail-0.2.7.dist-info/RECORD
+Filename: quickemail-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quickemail.py

```diff
@@ -402,14 +402,16 @@
         'sisx': 'application/vnd.symbian.install',
         'ipa': 'application/vnd.iphone',
         'xap': 'application/x-silverlight-app',
     }
 
     def __init__(self, host, port=25):
 
+        self._tls = False
+        self._ssl = False
         self.debug = False
         self._host = host
         self._port = port
         self._debuglevel = 0
         self._auth_user = None
         self._user_pass = None
         self._mail_from = ''
@@ -439,33 +441,33 @@
     def set_auth_user(self, s):
         self._auth_user = s
 
     def set_user_pass(self, s):
         self._user_pass = s
 
     def set_mail_from(self, s):
-        self._mail_from = s if s is not None else ''
+        self._mail_from = s
 
     def set_mail_to(self, s):
-        self._mail_to = s if s is not None else ''
+        self._mail_to = s
 
     def set_mail_cc(self, s):
-        self._mail_cc = s if s is not None else ''
+        self._mail_cc = s
 
     def set_mail_bcc(self, s):
-        self._mail_bcc = s if s is not None else ''
+        self._mail_bcc = s
 
     def set_content_from(self, s):
-        self._content_from = s if s is not None else ''
+        self._content_from = s
 
     def set_content_to(self, s):
-        self._content_to = s if s is not None else ''
+        self._content_to = s
 
     def set_content_cc(self, s):
-        self._content_cc = s if s is not None else ''
+        self._content_cc = s
 
     def set_mail_subject(self, s):
         self._mail_subject = s
 
     def set_mail_content(self, s):
         self._mail_content = s
 
@@ -474,14 +476,20 @@
 
     def set_is_html(self, b):
         self._is_html = b
 
     def set_time_out(self, t):
         self._time_out = t
 
+    def set_tls(self, b):
+        self._tls = b
+
+    def set_ssl(self, b):
+        self._ssl = b
+
     @property
     def helo(self):
         return self._helo
 
     @helo.setter
     def helo(self, h):
         self._helo = h
@@ -603,14 +611,30 @@
         return self._is_html
 
     @is_html.setter
     def is_html(self, b):
         self._is_html = b
 
     @property
+    def tls(self):
+        return self._tls
+
+    @tls.setter
+    def tls(self, b):
+        self._tls = b
+
+    @property
+    def ssl(self):
+        return self._ssl
+
+    @ssl.setter
+    def ssl(self, b):
+        self._ssl = b
+
+    @property
     def time_out(self):
         return self._time_out
 
     @time_out.setter
     def time_out(self, t):
         self._time_out = t
 
@@ -737,28 +761,32 @@
         else:
             smtpto = self.mail_to
 
         if self.mail_bcc:
             smtpto = smtpto + "," + self.mail_bcc
 
         if not smtpto:
-            return """Must set_mail_to()"""
+            raise ConnectionError("Recv addr empty!")
 
-        if self.port == 465:
-            return "Anonymous send must use port 25"
+        # if self.port == 465:
+        #     return "Anonymous send must use port 25"
 
         send_err = ''
         try:
-            smtphandle = smtplib.SMTP(host=self.host, port=self.port, timeout=self.time_out)
-            # smtphandle.connect(self.host, self.port)
-            smtphandle.set_debuglevel = self._debuglevel
-            smtphandle.helo(self._helo)
-            smtphandle.sendmail(smtpfrom, smtpto.split(','), msgdata)
-            smtphandle.quit()
-            smtphandle.close()
+            smtp_handle = smtplib.SMTP(host=self.host, port=self.port, timeout=self.time_out)
+            # smtp_handle.connect(self.host, self.port)
+            smtp_handle.set_debuglevel = self._debuglevel
+            if self.tls:
+                smtp_handle.ehlo(self._helo)
+                smtp_handle.starttls()
+            else:
+                smtp_handle.helo(self._helo)
+            smtp_handle.sendmail(smtpfrom, smtpto.split(','), msgdata)
+            smtp_handle.quit()
+            smtp_handle.close()
         except Exception as e:
             if hasattr(e, 'args'):
                 for i in e.args:
                     if not i:
                         continue
                     if isinstance(i, int):
                         send_err += str(i) + ' '
@@ -777,42 +805,44 @@
 
     def authsend(self, msgdata=None):
         """
         # from must be a string
         # rcptto must be list
         """
         if not self.auth_user or not self.user_pass:
-            return """Must set mailuser and password : 
+            raise ConnectionError("""Must set mailuser and password : 
                 auth_user('username')
-                user_pass('password')"""
+                user_pass('password')""")
         if msgdata is None:
             self.creatmsg()
             msgdata = self._msg
         smtpfrom = self.mail_from
 
         if self.mail_cc:
             smtpto = self.mail_to + "," + self.mail_cc
         else:
             smtpto = self._mail_to
 
         if self.mail_bcc:
             smtpto = smtpto + "," + self.mail_bcc
 
         if not smtpto:
-            return """Must mail_to()"""
+            raise ConnectionError("Recv addr empty!")
 
         send_err = ''
         try:
-            if self.port == 465:
+            if self.ssl:
                 smtp_handle = smtplib.SMTP_SSL(host=self.host, port=self.port, timeout=self.time_out)
             else:
                 smtp_handle = smtplib.SMTP(host=self.host, port=self.port, timeout=self.time_out)
             # smtp_handle.connect(self.host, self.port)
             smtp_handle.set_debuglevel = self._debuglevel
             smtp_handle.ehlo(self._helo)
+            if self.tls:
+                smtp_handle.starttls()
             smtp_handle.login(self.auth_user, self.user_pass)
             smtp_handle.sendmail(smtpfrom, smtpto.split(','), msgdata)
             smtp_handle.quit()
             smtp_handle.close()
         except Exception as e:
             if hasattr(e, 'args'):
                 for i in e.args:
@@ -832,27 +862,28 @@
                 raise ConnectionError(send_err)
             return False
         return True
 
 
 if __name__ == '__main__':
 
-    quicksend = QuickEmail('127.0.0.1', 25)
+    quicksend = QuickEmail('127.0.0.1', 587)
     quicksend.debug = True
+    quicksend.tls = True
     quicksend.auth_user = 'abc'
     quicksend.user_pass = 'test'
     quicksend.mail_from = '<a@test.com>'
     quicksend.mail_to = '一二三 <123@test.com>,abc@test.com,<a@test.com>'
-    quicksend.mail_bcc = '张三<b@test.com>'
+    quicksend.mail_cc = '张三<b@test.com>'
     quicksend.mail_subject = 'mY subject还有中文!'
     quicksend.mail_content = '<font color=red>red content一段中文</font>'
     quicksend.mail_attach = ['C:\\Users\\Administrator\\Pictures\\163.com.png']
     quicksend.is_html = True
     quicksend.content_from = '假发件人<a@a.com>'
-    quicksend.content_cc = ''
+    quicksend.content_cc = 'e@test.com'
 
     # msg = quicksend.creatmsg()
     # print(msg)
     print(quicksend.auth_user, quicksend.user_pass)
-    do_send = quicksend.authsend()
+    do_send = quicksend.send()
     if not do_send:
         print(do_send)
```

## Comparing `quickemail-0.2.7.dist-info/METADATA` & `quickemail-0.2.8.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickemail
-Version: 0.2.7
+Version: 0.2.8
 Summary: Quick send email use python3.
 Home-page: http://clayboy.cn
 Author: Clayboy
 Author-email: clayboy@foxmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -26,16 +26,16 @@
 
 1. 发信前先定义发信要素：
    
         指定主机和端口，必须参数：
         quicksend = QuickEmail('mail.test.com', 25)    # SMTP发信端口，默认是25 SSL链接使用465
         quicksend.debug = True                         # 打开调试
         定义HELO主机名，参数可省略：
-        quicksend.helo = 'QuickEmail'                 # HELO主机名不能使用有空格的字符串
-    
+        quicksend.helo = 'QuickEmail'                 # HELO主机名不能使用有空格的字符串，可以省略
+        quicksend.tls = True / quicksend.ssl = True   # 开启startTLS或者SSL，SSL端口一般为465
         认证用户名和密码，authsend()必须的参数：
         quicksend.mail_user = 'a'                     # 认证用户名
         quicksend.user_pass = 'test'                  # 认证用户的密码
     
         发信人、收信人为必须参数：
         quicksend.mail_from = 'AA高丽A<a@test.com>'    # 发信人地址，格式为:   FullName<email address>
         quicksend.mail_to = '一二三<123@test.com>,ABC<abc@test.com>'    # 格式同上，多地址使用逗号","分隔
```

