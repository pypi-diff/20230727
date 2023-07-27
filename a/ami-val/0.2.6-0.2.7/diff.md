# Comparing `tmp/ami-val-0.2.6.tar.gz` & `tmp/ami-val-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ami-val-0.2.6.tar", last modified: Wed Apr 26 10:08:55 2023, max compression
+gzip compressed data, was "dist/ami-val-0.2.7.tar", last modified: Thu Jul 27 03:18:00 2023, max compression
```

## Comparing `ami-val-0.2.6.tar` & `ami-val-0.2.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:08:55.000000 ami-val-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-26 10:08:55.000000 ami-val-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-26 10:08:50.000000 ami-val-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:08:55.000000 ami-val-0.2.6/ami_val/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10962 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/ami_val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:08:55.000000 ami-val-0.2.6/ami_val/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/cfg/ami-val.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:08:55.000000 ami-val-0.2.6/ami_val/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/libs/aws_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/libs/resource_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    39009 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/libs/utils_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:08:55.000000 ami-val-0.2.6/ami_val/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/scripts/rhel-ha-aws-check.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:08:55.000000 ami-val-0.2.6/ami_val/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/templates/sum.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:08:55.000000 ami-val-0.2.6/ami_val/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/tests/test_stage0.py
--rw-r--r--   0 runner    (1001) docker     (123)    44375 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/tests/test_stage1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/tests/test_stage2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-04-26 10:08:50.000000 ami-val-0.2.6/ami_val/tests/test_stage3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:08:55.000000 ami-val-0.2.6/ami_val.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-26 10:08:55.000000 ami-val-0.2.6/ami_val.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-26 10:08:55.000000 ami-val-0.2.6/ami_val.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:08:55.000000 ami-val-0.2.6/ami_val.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 10:08:55.000000 ami-val-0.2.6/ami_val.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 10:08:55.000000 ami-val-0.2.6/ami_val.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 10:08:55.000000 ami-val-0.2.6/ami_val.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:08:55.000000 ami-val-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-26 10:08:50.000000 ami-val-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:18:00.000000 ami-val-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-27 03:18:00.000000 ami-val-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-27 03:17:52.000000 ami-val-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:18:00.000000 ami-val-0.2.7/ami_val/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10962 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/ami_val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:18:00.000000 ami-val-0.2.7/ami_val/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/cfg/ami-val.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:18:00.000000 ami-val-0.2.7/ami_val/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/libs/aws_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/libs/resource_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39009 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/libs/utils_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:18:00.000000 ami-val-0.2.7/ami_val/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/scripts/rhel-ha-aws-check.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:18:00.000000 ami-val-0.2.7/ami_val/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/templates/sum.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:18:00.000000 ami-val-0.2.7/ami_val/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/tests/test_stage0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44513 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/tests/test_stage1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/tests/test_stage2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-27 03:17:52.000000 ami-val-0.2.7/ami_val/tests/test_stage3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:18:00.000000 ami-val-0.2.7/ami_val.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-27 03:18:00.000000 ami-val-0.2.7/ami_val.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-27 03:18:00.000000 ami-val-0.2.7/ami_val.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:18:00.000000 ami-val-0.2.7/ami_val.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 03:18:00.000000 ami-val-0.2.7/ami_val.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 03:18:00.000000 ami-val-0.2.7/ami_val.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 03:18:00.000000 ami-val-0.2.7/ami_val.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 03:18:00.000000 ami-val-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-27 03:17:52.000000 ami-val-0.2.7/setup.py
```

### Comparing `ami-val-0.2.6/PKG-INFO` & `ami-val-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ami-val
-Version: 0.2.6
+Version: 0.2.7
 Summary: AMI validation tool
 Home-page: https://github.com/liangxiao1/ami-val
 Author: Xiao Liang
 Author-email: xiliang@redhat.com
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ami-val-0.2.6/README.md` & `ami-val-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.6/ami_val/ami_val.py` & `ami-val-0.2.7/ami_val/ami_val.py`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.6/ami_val/cfg/ami-val.yaml` & `ami-val-0.2.7/ami_val/cfg/ami-val.yaml`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.6/ami_val/libs/aws_lib.py` & `ami-val-0.2.7/ami_val/libs/aws_lib.py`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.6/ami_val/libs/resource_class.py` & `ami-val-0.2.7/ami_val/libs/resource_class.py`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.6/ami_val/libs/utils_lib.py` & `ami-val-0.2.7/ami_val/libs/utils_lib.py`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.6/ami_val/scripts/rhel-ha-aws-check.sh` & `ami-val-0.2.7/ami_val/scripts/rhel-ha-aws-check.sh`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.6/ami_val/templates/sum.html` & `ami-val-0.2.7/ami_val/templates/sum.html`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.6/ami_val/tests/test_stage0.py` & `ami-val-0.2.7/ami_val/tests/test_stage0.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,26 @@
             test_instance.log.info('ena_support is enabled as expected in push task after RHEL-7.4, acutal: {}'.format(test_instance.info['ena_support']))
 
 def test_stage0_check_ena_set_in_cloud(test_instance):
     '''
     check if ena is actually enabled in cloud
     '''
     image = resource_class.EC2Image(test_instance)
-    if not image.is_ena_enabled():
-        test_instance.fail('ena not enabled')
+    test_instance.log.info("Details:{}".format(json.dumps(test_instance.info, indent=4)))
+    aminame = test_instance.info['name']
+    if aminame.startswith(('RHEL-6','RHEL-7.0','RHEL-7.1','RHEL-7.2','RHEL-7.3')):
+        if image.is_ena_enabled():
+            test_instance.fail('ena should not be enabled earlier than RHEL-7.4')
+        else:
+            test_instance.log.info('ena is not enabled earlier than RHEL-7.4')
+    else:
+        if not image.is_ena_enabled():
+            test_instance.fail('ena should be enabled after RHEL-7.3')
+        else:
+            test_instance.log.info('ena is enabled as expected after RHEL7.3')
 
 def test_stage0_launch_instance(test_instance):
     '''
     launch instances from AMIs in all supported regions
     '''
     aws_lib.aws_check_region(region=test_instance.info['region'], profile=test_instance.profile_name, resource_file=test_instance.resource_file, log=test_instance.log, tag=test_instance.tag)
     vm = resource_class.EC2VM(test_instance)
```

### Comparing `ami-val-0.2.6/ami_val/tests/test_stage1.py` & `ami-val-0.2.7/ami_val/tests/test_stage1.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 def test_stage1_check_bootime_launch(test_instance):
     '''
     check first launch boot time.
     can change pass criteria in cfg ami-val.yaml, default is 50s.
     rhbz: 1862930
     '''
 
+    aminame = test_instance.info['name']
+    if aminame.startswith('RHEL-6'):
+        test_instance.skipTest('no systemd-analyze in el6')
     test_instance.tmp_data['BootTime'] = {''}
     boottime = getboottime(test_instance)
     test_instance.tmp_data['BootTime'] = {'FirstLaunchTIme':boottime}
     test_instance.tmp_data['BootTime']['ImageID'] = test_instance.vm.ami_id
     test_instance.tmp_data['BootTime']['ImageName'] = test_instance.info['name']
     test_instance.tmp_data['BootTime']['Release'] = test_instance.info['release'].get('version')
     out = run_cmd(test_instance, 'uname -r', expect_ret=0, msg='get kernel version')
```

### Comparing `ami-val-0.2.6/ami_val/tests/test_stage2.py` & `ami-val-0.2.7/ami_val/tests/test_stage2.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,17 @@
 def test_stage2_test_rebootime(test_instance):
     '''
     rhbz: 1776710, 1446698, 1446688
     check reboot time after 1st init.
     can change pass criteria in cfg ami-val.yaml, default is 30s.
     '''
 
+    aminame = test_instance.info['name']
+    if aminame.startswith('RHEL-6'):
+        test_instance.skipTest('no systemd-analyze in el6')
     test_instance.ssh_client.close()
     test_instance.vm.reboot()
     test_instance.ssh_client = test_instance.vm.new_ssh_client()
     boottime = getboottime(test_instance)
     test_instance.tmp_data['BootTime']['RebootTime'] = boottime
     if float(boottime) > float(test_instance.params['max_reboot_time']):
         test_instance.fail('boot time {} over expected {}'.format(boottime, test_instance.params['max_reboot_time']))
@@ -153,14 +156,17 @@
 
 def test_stage2_test_stop_start_bootime(test_instance):
     '''
     check reboot time after stop
     can change pass criteria in cfg ami-val.yaml, default is 30s.
     '''
 
+    aminame = test_instance.info['name']
+    if aminame.startswith('RHEL-6'):
+        test_instance.skipTest('no systemd-analyze in el6')
     test_instance.ssh_client.close()
     test_instance.vm.stop()
     test_instance.vm.start()
     test_instance.ssh_client = test_instance.vm.new_ssh_client()
     boottime = getboottime(test_instance)
     test_instance.tmp_data['BootTime']['Stop-StartTime'] = boottime
     test_instance.log.info(test_instance.tmp_data)
```

### Comparing `ami-val-0.2.6/ami_val/tests/test_stage3.py` & `ami-val-0.2.7/ami_val/tests/test_stage3.py`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.6/ami_val.egg-info/PKG-INFO` & `ami-val-0.2.7/ami_val.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ami-val
-Version: 0.2.6
+Version: 0.2.7
 Summary: AMI validation tool
 Home-page: https://github.com/liangxiao1/ami-val
 Author: Xiao Liang
 Author-email: xiliang@redhat.com
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ami-val-0.2.6/ami_val.egg-info/SOURCES.txt` & `ami-val-0.2.7/ami_val.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.6/setup.py` & `ami-val-0.2.7/setup.py`

 * *Files identical despite different names*

