# Comparing `tmp/eaiautomatontools-1.1.8.tar.gz` & `tmp/eaiautomatontools-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\eaiautomatontools-1.1.8.tar", last modified: Thu Nov 17 21:06:04 2022, max compression
+gzip compressed data, was "dist\eaiautomatontools-1.1.9.tar", last modified: Thu Jul 27 19:53:32 2023, max compression
```

## Comparing `eaiautomatontools-1.1.8.tar` & `eaiautomatontools-1.1.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2022-11-17 21:06:04.584319 eaiautomatontools-1.1.8/
--rw-rw-rw-   0        0        0    35176 2021-03-08 20:02:21.000000 eaiautomatontools-1.1.8/LICENSE
--rw-rw-rw-   0        0        0      159 2021-03-09 21:03:49.000000 eaiautomatontools-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0    11083 2022-11-17 21:06:04.584319 eaiautomatontools-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     8938 2022-11-17 21:05:53.000000 eaiautomatontools-1.1.8/README.md
--rw-rw-rw-   0        0        0     6344 2021-03-08 20:02:21.000000 eaiautomatontools-1.1.8/README.rst
-drwxrwxrwx   0        0        0        0 2022-11-17 21:06:04.446721 eaiautomatontools-1.1.8/eaiautomatontools/
--rw-rw-rw-   0        0        0       23 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.8/eaiautomatontools/__init__.py
--rw-rw-rw-   0        0        0    13100 2022-06-25 13:10:26.000000 eaiautomatontools-1.1.8/eaiautomatontools/actions.py
--rw-rw-rw-   0        0        0     4293 2021-07-24 13:29:58.000000 eaiautomatontools-1.1.8/eaiautomatontools/alerts.py
--rw-rw-rw-   0        0        0    25379 2022-11-17 21:04:16.000000 eaiautomatontools-1.1.8/eaiautomatontools/browserServer.py
--rw-rw-rw-   0        0        0     5987 2021-05-03 18:39:21.000000 eaiautomatontools-1.1.8/eaiautomatontools/drivers_tools.py
--rw-rw-rw-   0        0        0     7410 2022-02-27 08:39:01.000000 eaiautomatontools-1.1.8/eaiautomatontools/finders.py
--rw-rw-rw-   0        0        0    13615 2022-11-17 21:04:16.000000 eaiautomatontools-1.1.8/eaiautomatontools/information.py
--rw-rw-rw-   0        0        0     2855 2021-05-14 20:33:31.000000 eaiautomatontools-1.1.8/eaiautomatontools/navigators.py
-drwxrwxrwx   0        0        0        0 2022-11-17 21:06:04.514958 eaiautomatontools-1.1.8/eaiautomatontools/resources/
--rw-rw-rw-   0        0        0       23 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/__init__.py
--rw-rw-rw-   0        0        0     1773 2021-04-30 20:20:31.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/app.py
--rw-rw-rw-   0        0        0      185 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/default_popup.html
--rw-rw-rw-   0        0        0      224 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/first_popup.html
--rw-rw-rw-   0        0        0      208 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/forms-css.css
--rw-rw-rw-   0        0        0     1347 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/forms.html
--rw-rw-rw-   0        0        0      157 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/iframe.html
--rw-rw-rw-   0        0        0     1824 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/index.html
--rw-rw-rw-   0        0        0      504 2021-03-08 21:12:05.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/myjs.js
--rw-rw-rw-   0        0        0      728 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/popups.html
--rw-rw-rw-   0        0        0      561 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/screenshot.html
--rw-rw-rw-   0        0        0      775 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/second.html
--rw-rw-rw-   0        0        0     1637 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/select.html
--rw-rw-rw-   0        0        0     3564 2021-04-30 16:52:40.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/server.py
--rw-rw-rw-   0        0        0     2381 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.8/eaiautomatontools/resources/tables.html
-drwxrwxrwx   0        0        0        0 2022-11-17 21:06:04.478625 eaiautomatontools-1.1.8/eaiautomatontools.egg-info/
--rw-rw-rw-   0        0        0    11083 2022-11-17 21:06:03.000000 eaiautomatontools-1.1.8/eaiautomatontools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2132 2022-11-17 21:06:04.000000 eaiautomatontools-1.1.8/eaiautomatontools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-17 21:06:03.000000 eaiautomatontools-1.1.8/eaiautomatontools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2022-11-17 21:06:03.000000 eaiautomatontools-1.1.8/eaiautomatontools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-11-17 21:06:03.000000 eaiautomatontools-1.1.8/eaiautomatontools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      314 2022-11-17 21:06:04.588630 eaiautomatontools-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1512 2022-11-17 21:05:02.000000 eaiautomatontools-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-17 21:06:04.582320 eaiautomatontools-1.1.8/test/
--rw-rw-rw-   0        0        0     8938 2022-11-17 21:05:02.000000 eaiautomatontools-1.1.8/test/README.md
--rw-rw-rw-   0        0        0     2578 2022-06-25 13:53:25.000000 eaiautomatontools-1.1.8/test/test_01_01_browserServer.md
--rw-rw-rw-   0        0        0     4053 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_01_02_take_a_screenshot.md
--rw-rw-rw-   0        0        0     6849 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_02_01_finders_element.md
--rw-rw-rw-   0        0        0     5888 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_02_02_finders_elements.md
--rw-rw-rw-   0        0        0     3740 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_02_03_finders_from_elements.md
--rw-rw-rw-   0        0        0        0 2021-03-10 20:56:57.000000 eaiautomatontools-1.1.8/test/test_02_04_finders_sub_element_from_element.md
--rw-rw-rw-   0        0        0      844 2021-03-11 20:17:13.000000 eaiautomatontools-1.1.8/test/test_03_01_navigators_driver_assertion.md
--rw-rw-rw-   0        0        0     4237 2022-06-25 13:53:25.000000 eaiautomatontools-1.1.8/test/test_03_02_navigators_go_to_window.md
--rw-rw-rw-   0        0        0     3436 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_04_01_actions_fill_element.md
--rw-rw-rw-   0        0        0     2981 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_04_02_actions_fill_elements.md
--rw-rw-rw-   0        0        0     3049 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_04_03_actions_set_checkbox.md
--rw-rw-rw-   0        0        0     3627 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_04_04_actions_select_in_dropdown.md
--rw-rw-rw-   0        0        0     2504 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_04_05_actions_click_element.md
--rw-rw-rw-   0        0        0     2558 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_04_06_actions_mouse_click_element.md
--rw-rw-rw-   0        0        0     8206 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_05_01_alerts_intercept_alert.md
--rw-rw-rw-   0        0        0     3093 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_05_02_alerts_alert_message.md
--rw-rw-rw-   0        0        0     2038 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_06_01_informations_is_field_exist.md
--rw-rw-rw-   0        0        0     2713 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_06_02_informations_is_field_contains_text.md
--rw-rw-rw-   0        0        0     1818 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_06_03_informations_is_alert_present.md
--rw-rw-rw-   0        0        0     2512 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_06_04_informations_element_text.md
--rw-rw-rw-   0        0        0     1524 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_06_05_informations_how_many_windows.md
--rw-rw-rw-   0        0        0     2403 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_06_06_informations_retrieve_tabular.md
--rw-rw-rw-   0        0        0     1497 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.8/test/test_06_07_informations_where_am_i.md
+drwxrwxrwx   0        0        0        0 2023-07-27 19:53:32.096315 eaiautomatontools-1.1.9/
+-rw-rw-rw-   0        0        0    35176 2021-03-08 20:02:21.000000 eaiautomatontools-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0      159 2021-03-09 21:03:49.000000 eaiautomatontools-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    11182 2023-07-27 19:53:32.096315 eaiautomatontools-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9021 2023-07-27 19:33:25.000000 eaiautomatontools-1.1.9/README.md
+-rw-rw-rw-   0        0        0     6344 2021-03-08 20:02:21.000000 eaiautomatontools-1.1.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-27 19:53:31.930427 eaiautomatontools-1.1.9/eaiautomatontools/
+-rw-rw-rw-   0        0        0       23 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.9/eaiautomatontools/__init__.py
+-rw-rw-rw-   0        0        0    13100 2022-06-25 13:10:26.000000 eaiautomatontools-1.1.9/eaiautomatontools/actions.py
+-rw-rw-rw-   0        0        0     4293 2021-07-24 13:29:58.000000 eaiautomatontools-1.1.9/eaiautomatontools/alerts.py
+-rw-rw-rw-   0        0        0    25384 2023-07-27 19:33:25.000000 eaiautomatontools-1.1.9/eaiautomatontools/browserServer.py
+-rw-rw-rw-   0        0        0     5987 2021-05-03 18:39:21.000000 eaiautomatontools-1.1.9/eaiautomatontools/drivers_tools.py
+-rw-rw-rw-   0        0        0     7410 2022-02-27 08:39:01.000000 eaiautomatontools-1.1.9/eaiautomatontools/finders.py
+-rw-rw-rw-   0        0        0    13615 2022-11-17 21:04:16.000000 eaiautomatontools-1.1.9/eaiautomatontools/information.py
+-rw-rw-rw-   0        0        0     2855 2021-05-14 20:33:31.000000 eaiautomatontools-1.1.9/eaiautomatontools/navigators.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:53:32.031247 eaiautomatontools-1.1.9/eaiautomatontools/resources/
+-rw-rw-rw-   0        0        0       23 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/__init__.py
+-rw-rw-rw-   0        0        0     1773 2021-04-30 20:20:31.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/app.py
+-rw-rw-rw-   0        0        0      185 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/default_popup.html
+-rw-rw-rw-   0        0        0      224 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/first_popup.html
+-rw-rw-rw-   0        0        0      208 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/forms-css.css
+-rw-rw-rw-   0        0        0     1347 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/forms.html
+-rw-rw-rw-   0        0        0      157 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/iframe.html
+-rw-rw-rw-   0        0        0     1824 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/index.html
+-rw-rw-rw-   0        0        0      504 2021-03-08 21:12:05.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/myjs.js
+-rw-rw-rw-   0        0        0      728 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/popups.html
+-rw-rw-rw-   0        0        0      561 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/screenshot.html
+-rw-rw-rw-   0        0        0      775 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/second.html
+-rw-rw-rw-   0        0        0     1637 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/select.html
+-rw-rw-rw-   0        0        0     3564 2021-04-30 16:52:40.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/server.py
+-rw-rw-rw-   0        0        0     2381 2021-01-30 18:18:15.000000 eaiautomatontools-1.1.9/eaiautomatontools/resources/tables.html
+drwxrwxrwx   0        0        0        0 2023-07-27 19:53:31.983836 eaiautomatontools-1.1.9/eaiautomatontools.egg-info/
+-rw-rw-rw-   0        0        0    11182 2023-07-27 19:53:31.000000 eaiautomatontools-1.1.9/eaiautomatontools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2132 2023-07-27 19:53:31.000000 eaiautomatontools-1.1.9/eaiautomatontools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 19:53:31.000000 eaiautomatontools-1.1.9/eaiautomatontools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-07-27 19:53:31.000000 eaiautomatontools-1.1.9/eaiautomatontools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-27 19:53:31.000000 eaiautomatontools-1.1.9/eaiautomatontools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      314 2023-07-27 19:53:32.111527 eaiautomatontools-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1512 2023-07-27 19:33:25.000000 eaiautomatontools-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:53:32.096315 eaiautomatontools-1.1.9/test/
+-rw-rw-rw-   0        0        0     8938 2022-11-17 21:07:16.000000 eaiautomatontools-1.1.9/test/README.md
+-rw-rw-rw-   0        0        0     2578 2022-06-25 13:53:25.000000 eaiautomatontools-1.1.9/test/test_01_01_browserServer.md
+-rw-rw-rw-   0        0        0     4053 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_01_02_take_a_screenshot.md
+-rw-rw-rw-   0        0        0     6849 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_02_01_finders_element.md
+-rw-rw-rw-   0        0        0     5888 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_02_02_finders_elements.md
+-rw-rw-rw-   0        0        0     3740 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_02_03_finders_from_elements.md
+-rw-rw-rw-   0        0        0        0 2021-03-10 20:56:57.000000 eaiautomatontools-1.1.9/test/test_02_04_finders_sub_element_from_element.md
+-rw-rw-rw-   0        0        0      844 2021-03-11 20:17:13.000000 eaiautomatontools-1.1.9/test/test_03_01_navigators_driver_assertion.md
+-rw-rw-rw-   0        0        0     4237 2022-06-25 13:53:25.000000 eaiautomatontools-1.1.9/test/test_03_02_navigators_go_to_window.md
+-rw-rw-rw-   0        0        0     3436 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_04_01_actions_fill_element.md
+-rw-rw-rw-   0        0        0     2981 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_04_02_actions_fill_elements.md
+-rw-rw-rw-   0        0        0     3049 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_04_03_actions_set_checkbox.md
+-rw-rw-rw-   0        0        0     3627 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_04_04_actions_select_in_dropdown.md
+-rw-rw-rw-   0        0        0     2504 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_04_05_actions_click_element.md
+-rw-rw-rw-   0        0        0     2558 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_04_06_actions_mouse_click_element.md
+-rw-rw-rw-   0        0        0     8206 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_05_01_alerts_intercept_alert.md
+-rw-rw-rw-   0        0        0     3093 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_05_02_alerts_alert_message.md
+-rw-rw-rw-   0        0        0     2038 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_06_01_informations_is_field_exist.md
+-rw-rw-rw-   0        0        0     2713 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_06_02_informations_is_field_contains_text.md
+-rw-rw-rw-   0        0        0     1818 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_06_03_informations_is_alert_present.md
+-rw-rw-rw-   0        0        0     2512 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_06_04_informations_element_text.md
+-rw-rw-rw-   0        0        0     1524 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_06_05_informations_how_many_windows.md
+-rw-rw-rw-   0        0        0     2403 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_06_06_informations_retrieve_tabular.md
+-rw-rw-rw-   0        0        0     1497 2022-06-25 13:35:31.000000 eaiautomatontools-1.1.9/test/test_06_07_informations_where_am_i.md
```

### Comparing `eaiautomatontools-1.1.8/LICENSE` & `eaiautomatontools-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/PKG-INFO` & `eaiautomatontools-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eaiautomatontools
-Version: 1.1.8
+Version: 1.1.9
 Summary: UI utilities in order to abstract selenium commands
 Home-page: https://eaiwebautomationtools.readthedocs.io/
 Author: Eric Aïvayan
 Author-email: eric.aivayan@free.fr
 License: UNKNOWN
 Description: Automaton Tools module
         ======================
@@ -136,14 +136,16 @@
         
         -   Add a multi-selection for dropdown
         -   Add a drag & drop functionality
         -   Add a get handles functionality
         
         Release Notes
         =============
+        - version 1.1.9:
+          - update path to find ChromeType in webdriver-manager package
         - version 1.1.8:
           - add information method to check if an element is in the viewport
             - browserServer.is\_element\_in\_viewport(field, [webElement])
             - information.is\_field\_in\_viewport(driver, field, [webElement])
         - version 1.1.7:
           - Rewrite __serve_chrome method to lower complexity
         - version 1.1.6:
```

### Comparing `eaiautomatontools-1.1.8/README.md` & `eaiautomatontools-1.1.9/test/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 This module space is about filling, selecting and clicking on web element.
 
 - fill\_element(field,value): return 0 if successful, fill the field with the value
 - fill\_elements(fields, data): return 0 if successful, fill each field in the fields dictionary with the value hold in the data dictionary. You can have a larger fields dictionary than the data but each data entry must be found in the fields dictionary. 
 - select\_in\_dropdown(field,visible\_text,value): return 0 if successful, select in the field dropdown the element either described by its visible text or its hidden value. 
 - click\_element(field): return 0 if successful, perform a left click on the field.
 - mouse\_click(field): return 0 if successful, perform a chain action moving the mouse on the element and mouse click element.
-- set\_checked(field,is\_checked): return 0 if successful, set the checkbox field so that the is\_checked value is always true i.e. checked if is\_checked set to true and not checked if is\_checked set to false.
+- set\_checked(field,is\_checked): return 0 if successful, set the check box field so that the is\_checked value is always true i.e. checked if is\_checked set to true and not checked if is\_checked set to false.
 
 Other documentation
 ===================
 
 Please find in the test folder doctest files which describe almost all methods here.
 
 Moreover don't hesitate to use the python help(method/class) directly from the python console in order to access the docstring.
@@ -154,15 +154,15 @@
   - add browser_version attribute. It allows to specify a browser version so that the webdriver manager will use this specific version.
 - version 1.1.0:
   - add selenium 4 support. Relative locator are not included in the current "field" model
 - version 1.0.14:
   - fix missing `web_element` variable in `BrowserServer.set_checkbox` method
   - add `mouse_click` method in the actions
 - version 1.0.13:
-  - fix missing `avoid_move_to` passing value to find_from_elements when using find_element in conjunction with `text` parameter. 
+  - fix missing `avoid_move_to` passing value to find_from_elements when using find_element in conjunction with `text` parameter.
 - version 1.0.12:
     - lower log level for finder(s) actions
     - add wait_for_another_window in information
     - add typing annotations and minimal docstring on BrowserServer
     - fix test_01_01
     - fix case browser_name is None
 - version 1.0.11:
```

### Comparing `eaiautomatontools-1.1.8/README.rst` & `eaiautomatontools-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/actions.py` & `eaiautomatontools-1.1.9/eaiautomatontools/actions.py`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/alerts.py` & `eaiautomatontools-1.1.9/eaiautomatontools/alerts.py`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/browserServer.py` & `eaiautomatontools-1.1.9/eaiautomatontools/browserServer.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from selenium.webdriver.firefox.service import Service as FfService
 from selenium.webdriver.edge.service import Service as EdgService
 # Driver Manager
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.firefox import GeckoDriverManager
 from webdriver_manager.microsoft import EdgeChromiumDriverManager
 from webdriver_manager.opera import OperaDriverManager
-from webdriver_manager.core.utils import ChromeType
+from webdriver_manager.core.os_manager import ChromeType
 # Self 
 from .navigators import (go_to_url, enter_frame, go_to_window)
 from .finders import (find_element, find_elements, find_from_elements,
                       find_sub_element_from_element)
 from .actions import (fill_element, fill_elements, mouse_click, select_in_dropdown, set_checkbox,
                       click_element, select_in_angular_dropdown, hover_element, select_in_elements)
 from .alerts import (alert_message, intercept_alert)
```

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/drivers_tools.py` & `eaiautomatontools-1.1.9/eaiautomatontools/drivers_tools.py`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/finders.py` & `eaiautomatontools-1.1.9/eaiautomatontools/finders.py`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/information.py` & `eaiautomatontools-1.1.9/eaiautomatontools/information.py`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/navigators.py` & `eaiautomatontools-1.1.9/eaiautomatontools/navigators.py`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/resources/app.py` & `eaiautomatontools-1.1.9/eaiautomatontools/resources/app.py`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/resources/forms.html` & `eaiautomatontools-1.1.9/eaiautomatontools/resources/forms.html`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/resources/index.html` & `eaiautomatontools-1.1.9/eaiautomatontools/resources/index.html`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/resources/popups.html` & `eaiautomatontools-1.1.9/eaiautomatontools/resources/popups.html`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/resources/screenshot.html` & `eaiautomatontools-1.1.9/eaiautomatontools/resources/screenshot.html`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/resources/second.html` & `eaiautomatontools-1.1.9/eaiautomatontools/resources/second.html`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/resources/select.html` & `eaiautomatontools-1.1.9/eaiautomatontools/resources/select.html`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/resources/server.py` & `eaiautomatontools-1.1.9/eaiautomatontools/resources/server.py`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools/resources/tables.html` & `eaiautomatontools-1.1.9/eaiautomatontools/resources/tables.html`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools.egg-info/PKG-INFO` & `eaiautomatontools-1.1.9/eaiautomatontools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eaiautomatontools
-Version: 1.1.8
+Version: 1.1.9
 Summary: UI utilities in order to abstract selenium commands
 Home-page: https://eaiwebautomationtools.readthedocs.io/
 Author: Eric Aïvayan
 Author-email: eric.aivayan@free.fr
 License: UNKNOWN
 Description: Automaton Tools module
         ======================
@@ -136,14 +136,16 @@
         
         -   Add a multi-selection for dropdown
         -   Add a drag & drop functionality
         -   Add a get handles functionality
         
         Release Notes
         =============
+        - version 1.1.9:
+          - update path to find ChromeType in webdriver-manager package
         - version 1.1.8:
           - add information method to check if an element is in the viewport
             - browserServer.is\_element\_in\_viewport(field, [webElement])
             - information.is\_field\_in\_viewport(driver, field, [webElement])
         - version 1.1.7:
           - Rewrite __serve_chrome method to lower complexity
         - version 1.1.6:
```

### Comparing `eaiautomatontools-1.1.8/eaiautomatontools.egg-info/SOURCES.txt` & `eaiautomatontools-1.1.9/eaiautomatontools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/setup.py` & `eaiautomatontools-1.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="eaiautomatontools",
-    version="1.1.8",
+    version="1.1.9",
     description="UI utilities in order to abstract selenium commands",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://eaiwebautomationtools.readthedocs.io/",
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
```

### Comparing `eaiautomatontools-1.1.8/test/README.md` & `eaiautomatontools-1.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 This module space is about filling, selecting and clicking on web element.
 
 - fill\_element(field,value): return 0 if successful, fill the field with the value
 - fill\_elements(fields, data): return 0 if successful, fill each field in the fields dictionary with the value hold in the data dictionary. You can have a larger fields dictionary than the data but each data entry must be found in the fields dictionary. 
 - select\_in\_dropdown(field,visible\_text,value): return 0 if successful, select in the field dropdown the element either described by its visible text or its hidden value. 
 - click\_element(field): return 0 if successful, perform a left click on the field.
 - mouse\_click(field): return 0 if successful, perform a chain action moving the mouse on the element and mouse click element.
-- set\_checked(field,is\_checked): return 0 if successful, set the check box field so that the is\_checked value is always true i.e. checked if is\_checked set to true and not checked if is\_checked set to false.
+- set\_checked(field,is\_checked): return 0 if successful, set the checkbox field so that the is\_checked value is always true i.e. checked if is\_checked set to true and not checked if is\_checked set to false.
 
 Other documentation
 ===================
 
 Please find in the test folder doctest files which describe almost all methods here.
 
 Moreover don't hesitate to use the python help(method/class) directly from the python console in order to access the docstring.
@@ -128,14 +128,16 @@
 
 -   Add a multi-selection for dropdown
 -   Add a drag & drop functionality
 -   Add a get handles functionality
 
 Release Notes
 =============
+- version 1.1.9:
+  - update path to find ChromeType in webdriver-manager package
 - version 1.1.8:
   - add information method to check if an element is in the viewport
     - browserServer.is\_element\_in\_viewport(field, [webElement])
     - information.is\_field\_in\_viewport(driver, field, [webElement])
 - version 1.1.7:
   - Rewrite __serve_chrome method to lower complexity
 - version 1.1.6:
@@ -154,15 +156,15 @@
   - add browser_version attribute. It allows to specify a browser version so that the webdriver manager will use this specific version.
 - version 1.1.0:
   - add selenium 4 support. Relative locator are not included in the current "field" model
 - version 1.0.14:
   - fix missing `web_element` variable in `BrowserServer.set_checkbox` method
   - add `mouse_click` method in the actions
 - version 1.0.13:
-  - fix missing `avoid_move_to` passing value to find_from_elements when using find_element in conjunction with `text` parameter.
+  - fix missing `avoid_move_to` passing value to find_from_elements when using find_element in conjunction with `text` parameter. 
 - version 1.0.12:
     - lower log level for finder(s) actions
     - add wait_for_another_window in information
     - add typing annotations and minimal docstring on BrowserServer
     - fix test_01_01
     - fix case browser_name is None
 - version 1.0.11:
```

### Comparing `eaiautomatontools-1.1.8/test/test_01_01_browserServer.md` & `eaiautomatontools-1.1.9/test/test_01_01_browserServer.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_01_02_take_a_screenshot.md` & `eaiautomatontools-1.1.9/test/test_01_02_take_a_screenshot.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_02_01_finders_element.md` & `eaiautomatontools-1.1.9/test/test_02_01_finders_element.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_02_02_finders_elements.md` & `eaiautomatontools-1.1.9/test/test_02_02_finders_elements.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_02_03_finders_from_elements.md` & `eaiautomatontools-1.1.9/test/test_02_03_finders_from_elements.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_03_01_navigators_driver_assertion.md` & `eaiautomatontools-1.1.9/test/test_03_01_navigators_driver_assertion.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_03_02_navigators_go_to_window.md` & `eaiautomatontools-1.1.9/test/test_03_02_navigators_go_to_window.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_04_01_actions_fill_element.md` & `eaiautomatontools-1.1.9/test/test_04_01_actions_fill_element.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_04_02_actions_fill_elements.md` & `eaiautomatontools-1.1.9/test/test_04_02_actions_fill_elements.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_04_03_actions_set_checkbox.md` & `eaiautomatontools-1.1.9/test/test_04_03_actions_set_checkbox.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_04_04_actions_select_in_dropdown.md` & `eaiautomatontools-1.1.9/test/test_04_04_actions_select_in_dropdown.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_04_05_actions_click_element.md` & `eaiautomatontools-1.1.9/test/test_04_05_actions_click_element.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_04_06_actions_mouse_click_element.md` & `eaiautomatontools-1.1.9/test/test_04_06_actions_mouse_click_element.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_05_01_alerts_intercept_alert.md` & `eaiautomatontools-1.1.9/test/test_05_01_alerts_intercept_alert.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_05_02_alerts_alert_message.md` & `eaiautomatontools-1.1.9/test/test_05_02_alerts_alert_message.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_06_01_informations_is_field_exist.md` & `eaiautomatontools-1.1.9/test/test_06_01_informations_is_field_exist.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_06_02_informations_is_field_contains_text.md` & `eaiautomatontools-1.1.9/test/test_06_02_informations_is_field_contains_text.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_06_03_informations_is_alert_present.md` & `eaiautomatontools-1.1.9/test/test_06_03_informations_is_alert_present.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_06_04_informations_element_text.md` & `eaiautomatontools-1.1.9/test/test_06_04_informations_element_text.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_06_05_informations_how_many_windows.md` & `eaiautomatontools-1.1.9/test/test_06_05_informations_how_many_windows.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_06_06_informations_retrieve_tabular.md` & `eaiautomatontools-1.1.9/test/test_06_06_informations_retrieve_tabular.md`

 * *Files identical despite different names*

### Comparing `eaiautomatontools-1.1.8/test/test_06_07_informations_where_am_i.md` & `eaiautomatontools-1.1.9/test/test_06_07_informations_where_am_i.md`

 * *Files identical despite different names*

