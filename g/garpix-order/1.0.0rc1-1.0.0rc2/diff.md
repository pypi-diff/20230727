# Comparing `tmp/garpix_order-1.0.0rc1.tar.gz` & `tmp/garpix_order-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_order-1.0.0rc1.tar", last modified: Thu Jul 27 14:05:25 2023, max compression
+gzip compressed data, was "garpix_order-1.0.0rc2.tar", last modified: Thu Jul 27 14:10:13 2023, max compression
```

## Comparing `garpix_order-1.0.0rc1.tar` & `garpix_order-1.0.0rc2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.070755 garpix_order-1.0.0rc1/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       64 2023-07-27 14:05:24.000000 garpix_order-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1531 2023-07-27 14:05:25.070594 garpix_order-1.0.0rc1/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.062859 garpix_order-1.0.0rc1/garpix_order/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       64 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc1/garpix_order/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      963 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      462 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc1/garpix_order/README.rst
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       59 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.064172 garpix_order-1.0.0rc1/garpix_order/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      225 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      499 2023-07-04 08:03:22.000000 garpix_order-1.0.0rc1/garpix_order/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      658 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      452 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/__pycache__/utils.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.064529 garpix_order-1.0.0rc1/garpix_order/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc1/garpix_order/admin/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.064659 garpix_order-1.0.0rc1/garpix_order/admin/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      173 2023-07-03 13:24:04.000000 garpix_order-1.0.0rc1/garpix_order/admin/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc1/garpix_order/admin/home_page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      207 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/admin/recurring.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      184 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc1/garpix_order/apps.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.065341 garpix_order-1.0.0rc1/garpix_order/migrations/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6932 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/migrations/0001_initial.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2607 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/migrations/0002_auto_20230703_1624.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      803 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/migrations/0003_robokassainvoice.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc1/garpix_order/migrations/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.065816 garpix_order-1.0.0rc1/garpix_order/migrations/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3139 2023-07-03 13:24:04.000000 garpix_order-1.0.0rc1/garpix_order/migrations/__pycache__/0001_squashed_0008_auto_20211105_1533.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2000 2023-07-03 13:30:54.000000 garpix_order-1.0.0rc1/garpix_order/migrations/__pycache__/0002_auto_20230703_1624.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      939 2023-07-03 13:31:02.000000 garpix_order-1.0.0rc1/garpix_order/migrations/__pycache__/0003_robokassainvoice.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      178 2023-07-03 13:24:04.000000 garpix_order-1.0.0rc1/garpix_order/migrations/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.066341 garpix_order-1.0.0rc1/garpix_order/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      209 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/models/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.066976 garpix_order-1.0.0rc1/garpix_order/models/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      435 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      856 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/models/__pycache__/config.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4227 2023-07-03 13:23:09.000000 garpix_order-1.0.0rc1/garpix_order/models/__pycache__/invoice.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4433 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/models/__pycache__/order.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1438 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/models/__pycache__/order_item.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5559 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/models/__pycache__/payment.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      468 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/models/config.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4210 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/models/order.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      789 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/models/order_item.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5279 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/models/payment.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.067611 garpix_order-1.0.0rc1/garpix_order/models/payments/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      149 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/models/payments/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.068257 garpix_order-1.0.0rc1/garpix_order/models/payments/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      372 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/models/payments/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      685 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/models/payments/__pycache__/bank_card.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      642 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/models/payments/__pycache__/cash.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1581 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/models/payments/__pycache__/cloudpayments.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2297 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/models/payments/__pycache__/recurring.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2024 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/models/payments/__pycache__/robokassa.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      241 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/models/payments/bank_card.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      207 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/models/payments/cash.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1338 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/models/payments/cloudpayments.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1874 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/models/payments/recurring.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1589 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/models/payments/robokassa.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      100 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc1/garpix_order/pyproject.toml
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.068474 garpix_order-1.0.0rc1/garpix_order/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/serializers/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.068693 garpix_order-1.0.0rc1/garpix_order/serializers/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      275 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/serializers/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      952 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/serializers/__pycache__/robokassa.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      419 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/serializers/robokassa.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.068876 garpix_order-1.0.0rc1/garpix_order/services/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/services/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.069094 garpix_order-1.0.0rc1/garpix_order/services/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/services/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3743 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/services/__pycache__/robokassa.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3577 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/services/robokassa.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1121 2023-07-27 14:05:23.000000 garpix_order-1.0.0rc1/garpix_order/setup.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     7708 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/tests.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      515 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/urls.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/utils.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.069198 garpix_order-1.0.0rc1/garpix_order/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       37 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/views/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.069301 garpix_order-1.0.0rc1/garpix_order/views/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      220 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/views/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.069838 garpix_order-1.0.0rc1/garpix_order/views/cloudpayments/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5754 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/views/cloudpayments/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.069955 garpix_order-1.0.0rc1/garpix_order/views/cloudpayments/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5051 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/views/cloudpayments/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1239 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/views/cloudpayments/default_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       98 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc1/garpix_order/views/cloudpayments/fail.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       97 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc1/garpix_order/views/cloudpayments/pay.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/views/cloudpayments/payment_data.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.070177 garpix_order-1.0.0rc1/garpix_order/views/robokassa/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/views/robokassa/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.070407 garpix_order-1.0.0rc1/garpix_order/views/robokassa/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      228 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/views/robokassa/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2053 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc1/garpix_order/views/robokassa/__pycache__/payment.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1553 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc1/garpix_order/views/robokassa/payment.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:05:25.063639 garpix_order-1.0.0rc1/garpix_order.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1531 2023-07-27 14:05:25.000000 garpix_order-1.0.0rc1/garpix_order.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3379 2023-07-27 14:05:25.000000 garpix_order-1.0.0rc1/garpix_order.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-07-27 14:05:25.000000 garpix_order-1.0.0rc1/garpix_order.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-07-27 14:05:25.000000 garpix_order-1.0.0rc1/garpix_order.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-07-27 14:05:25.000000 garpix_order-1.0.0rc1/garpix_order.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       13 2023-07-27 14:05:25.000000 garpix_order-1.0.0rc1/garpix_order.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-07-27 14:05:25.070797 garpix_order-1.0.0rc1/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1121 2023-07-27 14:05:24.000000 garpix_order-1.0.0rc1/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.506937 garpix_order-1.0.0rc2/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       64 2023-07-27 14:10:13.000000 garpix_order-1.0.0rc2/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1531 2023-07-27 14:10:13.506774 garpix_order-1.0.0rc2/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.470003 garpix_order-1.0.0rc2/garpix_order/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       64 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc2/garpix_order/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      963 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      462 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc2/garpix_order/README.rst
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       59 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.471140 garpix_order-1.0.0rc2/garpix_order/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      225 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      499 2023-07-04 08:03:22.000000 garpix_order-1.0.0rc2/garpix_order/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      658 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      452 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/__pycache__/utils.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.471453 garpix_order-1.0.0rc2/garpix_order/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc2/garpix_order/admin/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.471575 garpix_order-1.0.0rc2/garpix_order/admin/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      173 2023-07-03 13:24:04.000000 garpix_order-1.0.0rc2/garpix_order/admin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc2/garpix_order/admin/home_page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      207 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/admin/recurring.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      184 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc2/garpix_order/apps.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.472036 garpix_order-1.0.0rc2/garpix_order/migrations/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6932 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/migrations/0001_initial.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2607 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/migrations/0002_auto_20230703_1624.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      803 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/migrations/0003_robokassainvoice.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc2/garpix_order/migrations/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.472500 garpix_order-1.0.0rc2/garpix_order/migrations/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3139 2023-07-03 13:24:04.000000 garpix_order-1.0.0rc2/garpix_order/migrations/__pycache__/0001_squashed_0008_auto_20211105_1533.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2000 2023-07-03 13:30:54.000000 garpix_order-1.0.0rc2/garpix_order/migrations/__pycache__/0002_auto_20230703_1624.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      939 2023-07-03 13:31:02.000000 garpix_order-1.0.0rc2/garpix_order/migrations/__pycache__/0003_robokassainvoice.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      178 2023-07-03 13:24:04.000000 garpix_order-1.0.0rc2/garpix_order/migrations/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.473160 garpix_order-1.0.0rc2/garpix_order/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      209 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.479433 garpix_order-1.0.0rc2/garpix_order/models/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      435 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      856 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/models/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4227 2023-07-03 13:23:09.000000 garpix_order-1.0.0rc2/garpix_order/models/__pycache__/invoice.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4433 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/models/__pycache__/order.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1438 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/models/__pycache__/order_item.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5559 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/models/__pycache__/payment.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      468 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/models/config.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4210 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/models/order.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      789 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/models/order_item.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5279 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/models/payment.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.480254 garpix_order-1.0.0rc2/garpix_order/models/payments/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      149 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/models/payments/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.481876 garpix_order-1.0.0rc2/garpix_order/models/payments/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      372 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/models/payments/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      685 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/models/payments/__pycache__/bank_card.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      642 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/models/payments/__pycache__/cash.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1581 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/models/payments/__pycache__/cloudpayments.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2297 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/models/payments/__pycache__/recurring.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2024 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/models/payments/__pycache__/robokassa.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      241 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/models/payments/bank_card.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      207 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/models/payments/cash.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1338 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/models/payments/cloudpayments.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1874 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/models/payments/recurring.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1589 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/models/payments/robokassa.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      100 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc2/garpix_order/pyproject.toml
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.483375 garpix_order-1.0.0rc2/garpix_order/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/serializers/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.485838 garpix_order-1.0.0rc2/garpix_order/serializers/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      275 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/serializers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      952 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/serializers/__pycache__/robokassa.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      419 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/serializers/robokassa.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.487813 garpix_order-1.0.0rc2/garpix_order/services/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/services/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.491360 garpix_order-1.0.0rc2/garpix_order/services/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/services/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3743 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/services/__pycache__/robokassa.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3577 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/services/robokassa.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1151 2023-07-27 14:10:11.000000 garpix_order-1.0.0rc2/garpix_order/setup.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     7708 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/tests.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      515 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/urls.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/utils.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.496525 garpix_order-1.0.0rc2/garpix_order/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       37 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/views/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.496678 garpix_order-1.0.0rc2/garpix_order/views/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      220 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/views/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.497585 garpix_order-1.0.0rc2/garpix_order/views/cloudpayments/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5754 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/views/cloudpayments/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.498467 garpix_order-1.0.0rc2/garpix_order/views/cloudpayments/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5051 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/views/cloudpayments/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1239 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/views/cloudpayments/default_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       98 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc2/garpix_order/views/cloudpayments/fail.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       97 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc2/garpix_order/views/cloudpayments/pay.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/views/cloudpayments/payment_data.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.500285 garpix_order-1.0.0rc2/garpix_order/views/robokassa/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/views/robokassa/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.506566 garpix_order-1.0.0rc2/garpix_order/views/robokassa/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      228 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/views/robokassa/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2053 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc2/garpix_order/views/robokassa/__pycache__/payment.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1553 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc2/garpix_order/views/robokassa/payment.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:10:13.470686 garpix_order-1.0.0rc2/garpix_order.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1531 2023-07-27 14:10:13.000000 garpix_order-1.0.0rc2/garpix_order.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3379 2023-07-27 14:10:13.000000 garpix_order-1.0.0rc2/garpix_order.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-07-27 14:10:13.000000 garpix_order-1.0.0rc2/garpix_order.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-07-27 14:10:13.000000 garpix_order-1.0.0rc2/garpix_order.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       56 2023-07-27 14:10:13.000000 garpix_order-1.0.0rc2/garpix_order.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       13 2023-07-27 14:10:13.000000 garpix_order-1.0.0rc2/garpix_order.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-07-27 14:10:13.506981 garpix_order-1.0.0rc2/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1151 2023-07-27 14:10:13.000000 garpix_order-1.0.0rc2/setup.py
```

### Comparing `garpix_order-1.0.0rc1/PKG-INFO` & `garpix_order-1.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_order
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Home-page: https://github.com/garpixcms/garpix_order
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_order-1.0.0rc1/garpix_order/README.md` & `garpix_order-1.0.0rc2/garpix_order/README.md`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/__pycache__/urls.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/migrations/0001_initial.py` & `garpix_order-1.0.0rc2/garpix_order/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/migrations/0002_auto_20230703_1624.py` & `garpix_order-1.0.0rc2/garpix_order/migrations/0002_auto_20230703_1624.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/migrations/0003_robokassainvoice.py` & `garpix_order-1.0.0rc2/garpix_order/migrations/0003_robokassainvoice.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/migrations/__pycache__/0001_squashed_0008_auto_20211105_1533.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/migrations/__pycache__/0001_squashed_0008_auto_20211105_1533.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/migrations/__pycache__/0002_auto_20230703_1624.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/migrations/__pycache__/0002_auto_20230703_1624.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/migrations/__pycache__/0003_robokassainvoice.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/migrations/__pycache__/0003_robokassainvoice.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/__pycache__/config.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/models/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/__pycache__/invoice.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/models/__pycache__/invoice.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/__pycache__/order.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/models/__pycache__/order.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/__pycache__/order_item.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/models/__pycache__/order_item.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/__pycache__/payment.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/models/__pycache__/payment.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/order.py` & `garpix_order-1.0.0rc2/garpix_order/models/order.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/order_item.py` & `garpix_order-1.0.0rc2/garpix_order/models/order_item.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/payment.py` & `garpix_order-1.0.0rc2/garpix_order/models/payment.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/payments/__pycache__/bank_card.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/models/payments/__pycache__/bank_card.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/payments/__pycache__/cash.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/models/payments/__pycache__/cash.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/payments/__pycache__/cloudpayments.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/models/payments/__pycache__/cloudpayments.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/payments/__pycache__/recurring.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/models/payments/__pycache__/recurring.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/payments/__pycache__/robokassa.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/models/payments/__pycache__/robokassa.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/payments/cloudpayments.py` & `garpix_order-1.0.0rc2/garpix_order/models/payments/cloudpayments.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/payments/recurring.py` & `garpix_order-1.0.0rc2/garpix_order/models/payments/recurring.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/models/payments/robokassa.py` & `garpix_order-1.0.0rc2/garpix_order/models/payments/robokassa.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/serializers/__pycache__/robokassa.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/serializers/__pycache__/robokassa.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/services/__pycache__/robokassa.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/services/__pycache__/robokassa.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/services/robokassa.py` & `garpix_order-1.0.0rc2/garpix_order/services/robokassa.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/setup.py` & `garpix_order-1.0.0rc2/garpix_order/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_order')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_order',
-    version='1.0.0-rc1',
+    version='1.0.0-rc2',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_order',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -29,9 +29,10 @@
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 1.11',
         'djangorestframework >= 3.8',
+        'django-fsm >= 2.8.1'
     ],
 )
```

### Comparing `garpix_order-1.0.0rc1/garpix_order/tests.py` & `garpix_order-1.0.0rc2/garpix_order/tests.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/urls.py` & `garpix_order-1.0.0rc2/garpix_order/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/views/cloudpayments/__init__.py` & `garpix_order-1.0.0rc2/garpix_order/views/cloudpayments/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/views/cloudpayments/__pycache__/__init__.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/views/cloudpayments/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/views/cloudpayments/default_view.py` & `garpix_order-1.0.0rc2/garpix_order/views/cloudpayments/default_view.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/views/cloudpayments/payment_data.py` & `garpix_order-1.0.0rc2/garpix_order/views/cloudpayments/payment_data.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/views/robokassa/__pycache__/payment.cpython-38.pyc` & `garpix_order-1.0.0rc2/garpix_order/views/robokassa/__pycache__/payment.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order/views/robokassa/payment.py` & `garpix_order-1.0.0rc2/garpix_order/views/robokassa/payment.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/garpix_order.egg-info/PKG-INFO` & `garpix_order-1.0.0rc2/garpix_order.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-order
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Home-page: https://github.com/garpixcms/garpix_order
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_order-1.0.0rc1/garpix_order.egg-info/SOURCES.txt` & `garpix_order-1.0.0rc2/garpix_order.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc1/setup.py` & `garpix_order-1.0.0rc2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_order')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_order',
-    version='1.0.0-rc1',
+    version='1.0.0-rc2',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_order',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -29,9 +29,10 @@
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 1.11',
         'djangorestframework >= 3.8',
+        'django-fsm >= 2.8.1'
     ],
 )
```

