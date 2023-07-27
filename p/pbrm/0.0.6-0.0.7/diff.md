# Comparing `tmp/pbrm-0.0.6-py3-none-any.whl.zip` & `tmp/pbrm-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 13288 bytes, number of entries: 22
+Zip file size: 13298 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat       22 b- defN 23-Mar-30 13:58 pbrm/__init__.py
 -rw-rw-rw-  2.0 fat      165 b- defN 23-Mar-30 13:06 pbrm/change_repository.py
 -rw-rw-rw-  2.0 fat     2906 b- defN 23-Mar-31 11:14 pbrm/command_process.py
 -rw-rw-rw-  2.0 fat     1567 b- defN 23-Mar-30 14:17 pbrm/config.py
 -rw-rw-rw-  2.0 fat      364 b- defN 23-Mar-30 14:07 pbrm/delete.py
 -rw-rw-rw-  2.0 fat      930 b- defN 23-Mar-30 12:40 pbrm/error.py
 -rw-rw-rw-  2.0 fat     1584 b- defN 23-Mar-31 13:32 pbrm/gif.py
 -rw-rw-rw-  2.0 fat     2197 b- defN 23-Mar-30 14:07 pbrm/main.py
 -rw-rw-rw-  2.0 fat     1556 b- defN 23-Jul-27 06:08 pbrm/pbrm_statistics.py
 -rw-rw-rw-  2.0 fat     3315 b- defN 23-Mar-31 10:55 pbrm/save_illust.py
--rw-rw-rw-  2.0 fat     3161 b- defN 23-Jul-27 06:34 pbrm/update.py
+-rw-rw-rw-  2.0 fat     3193 b- defN 23-Jul-27 06:47 pbrm/update.py
 -rw-rw-rw-  2.0 fat      440 b- defN 23-Mar-30 05:25 pbrm/utils.py
 -rw-rw-rw-  2.0 fat      213 b- defN 23-Mar-30 05:45 pbrm/spider/__init__.py
 -rw-rw-rw-  2.0 fat     1357 b- defN 23-Mar-30 14:19 pbrm/spider/cookie_verify.py
 -rw-rw-rw-  2.0 fat     1763 b- defN 23-Mar-30 14:31 pbrm/spider/get_bookmarks.py
 -rw-rw-rw-  2.0 fat     1922 b- defN 23-Mar-30 05:41 pbrm/spider/get_meta.py
 -rw-rw-rw-  2.0 fat     1099 b- defN 23-Mar-29 14:46 pbrm/spider/illust_download.py
--rw-rw-rw-  2.0 fat      323 b- defN 23-Jul-27 06:36 pbrm-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 06:36 pbrm-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       41 b- defN 23-Jul-27 06:36 pbrm-0.0.6.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-27 06:36 pbrm-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1667 b- defN 23-Jul-27 06:36 pbrm-0.0.6.dist-info/RECORD
-22 files, 26689 bytes uncompressed, 10630 bytes compressed:  60.2%
+-rw-rw-rw-  2.0 fat      323 b- defN 23-Jul-27 06:47 pbrm-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 06:47 pbrm-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       41 b- defN 23-Jul-27 06:47 pbrm-0.0.7.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-27 06:47 pbrm-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1667 b- defN 23-Jul-27 06:47 pbrm-0.0.7.dist-info/RECORD
+22 files, 26721 bytes uncompressed, 10640 bytes compressed:  60.2%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: pbrm/spider/get_meta.py
 Comment: 
 
 Filename: pbrm/spider/illust_download.py
 Comment: 
 
-Filename: pbrm-0.0.6.dist-info/METADATA
+Filename: pbrm-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: pbrm-0.0.6.dist-info/WHEEL
+Filename: pbrm-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: pbrm-0.0.6.dist-info/entry_points.txt
+Filename: pbrm-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: pbrm-0.0.6.dist-info/top_level.txt
+Filename: pbrm-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pbrm-0.0.6.dist-info/RECORD
+Filename: pbrm-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pbrm/update.py

```diff
@@ -36,15 +36,15 @@
     i = 0
     all_illust = []
     for illust in bookmarks["illust"]:
         i = i + 1
         all_illust.append(str(illust["id"]))
         print("update: " + str(illust["id"]) + " process: {}/{}".format(str(i), bookmarks["total"]))
         if not force_update:
-            if work_exists(str(illust["id"]), path, illust["userId"] == 0, save_gif, illust["pageCount"]):
+            if work_exists(str(illust["id"]), path, illust["userId"] == 0, save_gif and (illust["illustType"] == 2), illust["pageCount"]):
                 if force_update_meta != force_update_illust and illust["userId"] != 0:
                     # 将force当skip用
                     log["updated"] += 1
                     save_illust.save_illust(illust["id"], path + "/" + illust["id"], cookie, save_gif
                                             , not force_update_illust, not force_update_meta)
                 continue
```

## Comparing `pbrm-0.0.6.dist-info/RECORD` & `pbrm-0.0.7.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 pbrm/config.py,sha256=BrnDKysM-itHf4n4uveyOySNhwfqtic9RTXOZff_y-Q,1567
 pbrm/delete.py,sha256=HthbsukXltSwXGKhTpUFV7QWV5RYJlJmNeqMs23rwg4,364
 pbrm/error.py,sha256=3_QG_jc5M3MUCIlbNHYzKASXxu6-6A073KWWEUfHKZk,930
 pbrm/gif.py,sha256=3AkybgN_7ny3dRORamg34IvobrDaK94Z0BRhYzcBiI0,1584
 pbrm/main.py,sha256=fept3TvFFXm3UtouUwXp6Li9xDAOx20EsbV2zRdd16Y,2197
 pbrm/pbrm_statistics.py,sha256=D_MKx6h9jpLrADqMT69_62rN0KWWydtzRIp03mW_LbQ,1556
 pbrm/save_illust.py,sha256=mkwkL8CRUyOhY_Nyx7-LLV8bJgMgtqUcM9ooqaC2P-g,3315
-pbrm/update.py,sha256=zvQ1-8fB8Hz0-Nn1TsomiS9C54j0tCad4gE6aczpTLw,3161
+pbrm/update.py,sha256=Cxepgb3aFxBEkLuyhvLKmWFzRSRENZj8mjFU24Hc4Rs,3193
 pbrm/utils.py,sha256=zxUWrG2sgtYY5IBybIMxuS09-r9P6t-YmLk4d396qog,440
 pbrm/spider/__init__.py,sha256=_rKqeAfc1TQn0b0aOwpY_-fEo9baJAeDFsc-Eldw3gA,213
 pbrm/spider/cookie_verify.py,sha256=ovbuKTRqE1WBO0UAm2vJF8NBqEgG1xWj72hOWaCsPhg,1357
 pbrm/spider/get_bookmarks.py,sha256=EfWZg7wpC7uW7aKImfdAbSNtAcUkrw2HEIu-ny0BOhk,1763
 pbrm/spider/get_meta.py,sha256=Xe4fbjGv7kW62-8GS8mMf48vWv0lptAZBE0V438U2YM,1922
 pbrm/spider/illust_download.py,sha256=QGwG74_CYMtDRUAIXn4ESP6tPjUe_slge6JAnkYW3lE,1099
-pbrm-0.0.6.dist-info/METADATA,sha256=msCsdF9BYTu6910ntBbCSMh7_P9crrFQevd5Hlfq6Jc,323
-pbrm-0.0.6.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-pbrm-0.0.6.dist-info/entry_points.txt,sha256=eY6nveOpcWgPIHq0P7RQH3IomveLzluu7F-J23DJlgY,41
-pbrm-0.0.6.dist-info/top_level.txt,sha256=d05lGeEdLKRqSqZ6e_PWuRaKhCsr-04jpHn720xlGJI,5
-pbrm-0.0.6.dist-info/RECORD,,
+pbrm-0.0.7.dist-info/METADATA,sha256=Z-zRco5MqoDlvGEE3sU1nJ6Rs536CX7pTvoo3_-T_oA,323
+pbrm-0.0.7.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+pbrm-0.0.7.dist-info/entry_points.txt,sha256=eY6nveOpcWgPIHq0P7RQH3IomveLzluu7F-J23DJlgY,41
+pbrm-0.0.7.dist-info/top_level.txt,sha256=d05lGeEdLKRqSqZ6e_PWuRaKhCsr-04jpHn720xlGJI,5
+pbrm-0.0.7.dist-info/RECORD,,
```

