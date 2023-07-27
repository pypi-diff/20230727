# Comparing `tmp/pglive-0.6.6.tar.gz` & `tmp/pglive-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pglive-0.6.6.tar", max compression
+gzip compressed data, was "pglive-0.6.7.tar", max compression
```

## Comparing `pglive-0.6.6.tar` & `pglive-0.6.7.tar`

### file list

```diff
@@ -1,96 +1,78 @@
--rwxr-xr-x   0        0        0     1067 2022-07-09 17:29:11.350000 pglive-0.6.6/LICENSE
--rw-r--r--   0        0        0     4832 2023-07-24 05:42:21.879592 pglive-0.6.6/README.md
--rw-r--r--   0        0        0        0 2023-07-24 05:42:21.879592 pglive-0.6.6/pglive/__init__.py
--rw-r--r--   0        0        0     4657 2023-07-24 05:42:21.879592 pglive-0.6.6/pglive/examples_pyqt5/__init__.py
--rw-r--r--   0        0        0     1093 2023-07-24 05:42:21.879592 pglive-0.6.6/pglive/examples_pyqt5/all_plot_types.py
--rw-r--r--   0        0        0     1992 2023-07-24 05:42:21.879592 pglive-0.6.6/pglive/examples_pyqt5/axis.py
--rw-r--r--   0        0        0      685 2023-07-24 05:42:21.879592 pglive-0.6.6/pglive/examples_pyqt5/candlestick_plot.py
--rw-r--r--   0        0        0     1416 2023-07-24 05:42:21.879592 pglive-0.6.6/pglive/examples_pyqt5/categorized_bar_plot.py
--rw-r--r--   0        0        0     2957 2023-07-24 05:42:21.879592 pglive-0.6.6/pglive/examples_pyqt5/crop_offset_to_data.py
--rw-r--r--   0        0        0     2650 2023-07-24 05:42:21.879592 pglive-0.6.6/pglive/examples_pyqt5/crosshair.py
--rw-r--r--   0        0        0        0 2023-07-24 05:42:21.879592 pglive-0.6.6/pglive/examples_pyqt5/designer_example/__init__.py
--rw-r--r--   0        0        0      813 2023-07-24 05:42:21.879592 pglive-0.6.6/pglive/examples_pyqt5/designer_example/main_example.py
--rw-r--r--   0        0        0     2203 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt5/designer_example/win_template.py
--rw-r--r--   0        0        0     1489 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt5/designer_example/win_template.ui
--rw-r--r--   0        0        0      610 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt5/horizontal_bar_plot.py
--rw-r--r--   0        0        0     2498 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt5/leading_line.py
--rw-r--r--   0        0        0      630 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt5/line_plot.py
--rw-r--r--   0        0        0     6533 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt5/live_plot_range.py
--rw-r--r--   0        0        0     2061 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt5/one_plot_multiple_plot_rates.py
--rw-r--r--   0        0        0     1767 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt5/pause_resume.py
--rw-r--r--   0        0        0      999 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt5/plot_rate.py
--rw-r--r--   0        0        0      642 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt5/scatter_plot.py
--rw-r--r--   0        0        0     1248 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt5/update_rate.py
--rw-r--r--   0        0        0      683 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt5/vertical_bar_plot.py
--rw-r--r--   0        0        0     1143 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt5/vertical_bar_plot_color.py
--rw-r--r--   0        0        0     4657 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/__init__.py
--rw-r--r--   0        0        0     1091 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/all_plot_types.py
--rw-r--r--   0        0        0     1992 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/axis.py
--rw-r--r--   0        0        0      685 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/candlestick_plot.py
--rw-r--r--   0        0        0     1416 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/categorized_bar_plot.py
--rw-r--r--   0        0        0     2955 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/crop_offset_to_data.py
--rw-r--r--   0        0        0     2650 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/crosshair.py
--rw-r--r--   0        0        0        0 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/designer_example/__init__.py
--rw-r--r--   0        0        0      813 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/designer_example/main_example.py
--rw-r--r--   0        0        0     2191 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/designer_example/win_template.py
--rw-r--r--   0        0        0     1489 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/designer_example/win_template.ui
--rw-r--r--   0        0        0      610 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/horizontal_bar_plot.py
--rw-r--r--   0        0        0     2498 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/leading_line.py
--rw-r--r--   0        0        0      630 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/line_plot.py
--rw-r--r--   0        0        0     6546 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/live_plot_range.py
--rw-r--r--   0        0        0     2061 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/one_plot_multiple_plot_rates.py
--rw-r--r--   0        0        0     1767 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/pause_resume.py
--rw-r--r--   0        0        0     1002 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/plot_rate.py
--rw-r--r--   0        0        0      642 2023-07-24 05:42:21.883592 pglive-0.6.6/pglive/examples_pyqt6/scatter_plot.py
--rw-r--r--   0        0        0     1249 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyqt6/update_rate.py
--rw-r--r--   0        0        0      683 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyqt6/vertical_bar_plot.py
--rw-r--r--   0        0        0     1143 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyqt6/vertical_bar_plot_color.py
--rw-r--r--   0        0        0     4661 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/__init__.py
--rw-r--r--   0        0        0     1090 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/all_plot_types.py
--rw-r--r--   0        0        0     1995 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/axis.py
--rw-r--r--   0        0        0      688 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/candlestick_plot.py
--rw-r--r--   0        0        0     1419 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/categorized_bar_plot.py
--rw-r--r--   0        0        0     2959 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/crop_offset_to_data.py
--rw-r--r--   0        0        0     2657 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/crosshair.py
--rw-r--r--   0        0        0      613 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/horizontal_bar_plot.py
--rw-r--r--   0        0        0     2501 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/leading_line.py
--rw-r--r--   0        0        0      633 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/line_plot.py
--rw-r--r--   0        0        0     6615 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/live_plot_range.py
--rw-r--r--   0        0        0     2064 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/one_plot_multiple_plot_rates.py
--rw-r--r--   0        0        0     1772 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/pause_resume.py
--rw-r--r--   0        0        0     1043 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/plot_rate.py
--rw-r--r--   0        0        0      645 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/scatter_plot.py
--rw-r--r--   0        0        0     1251 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/update_rate.py
--rw-r--r--   0        0        0      686 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/vertical_bar_plot.py
--rw-r--r--   0        0        0     1146 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside2/vertical_bar_plot_color.py
--rw-r--r--   0        0        0     4661 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside6/__init__.py
--rw-r--r--   0        0        0     1089 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside6/all_plot_types.py
--rw-r--r--   0        0        0     1994 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside6/axis.py
--rw-r--r--   0        0        0      687 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside6/candlestick_plot.py
--rw-r--r--   0        0        0     1418 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside6/categorized_bar_plot.py
--rw-r--r--   0        0        0     2958 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside6/crop_offset_to_data.py
--rw-r--r--   0        0        0     2656 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside6/crosshair.py
--rw-r--r--   0        0        0      612 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside6/horizontal_bar_plot.py
--rw-r--r--   0        0        0     2500 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside6/leading_line.py
--rw-r--r--   0        0        0      632 2023-07-24 05:42:21.887592 pglive-0.6.6/pglive/examples_pyside6/line_plot.py
--rw-r--r--   0        0        0     6614 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/examples_pyside6/live_plot_range.py
--rw-r--r--   0        0        0     2063 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/examples_pyside6/one_plot_multiple_plot_rates.py
--rw-r--r--   0        0        0     1771 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/examples_pyside6/pause_resume.py
--rw-r--r--   0        0        0      999 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/examples_pyside6/plot_rate.py
--rw-r--r--   0        0        0      644 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/examples_pyside6/scatter_plot.py
--rw-r--r--   0        0        0     1250 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/examples_pyside6/update_rate.py
--rw-r--r--   0        0        0      685 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/examples_pyside6/vertical_bar_plot.py
--rw-r--r--   0        0        0     1145 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/examples_pyside6/vertical_bar_plot_color.py
--rw-r--r--   0        0        0      967 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/kwargs.py
--rw-r--r--   0        0        0        0 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/sources/__init__.py
--rw-r--r--   0        0        0     8324 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/sources/data_connector.py
--rw-r--r--   0        0        0     4694 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/sources/live_axis.py
--rw-r--r--   0        0        0     8419 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/sources/live_axis_range.py
--rw-r--r--   0        0        0     3256 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/sources/live_candleStickPlot.py
--rw-r--r--   0        0        0     4510 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/sources/live_categorized_bar_plot.py
--rw-r--r--   0        0        0     5883 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/sources/live_mixins.py
--rw-r--r--   0        0        0     5274 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/sources/live_plot.py
--rw-r--r--   0        0        0    11010 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/sources/live_plot_widget.py
--rw-r--r--   0        0        0     1599 2023-07-24 05:42:21.891592 pglive-0.6.6/pglive/sources/utils.py
--rw-r--r--   0        0        0      951 2023-07-24 05:43:21.561629 pglive-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     5811 1970-01-01 00:00:00.000000 pglive-0.6.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1067 2022-07-09 17:29:11.350000 pglive-0.6.7/LICENSE
+-rw-r--r--   0        0        0     5091 2023-07-27 07:04:40.933372 pglive-0.6.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 05:42:21.879592 pglive-0.6.7/pglive/__init__.py
+-rw-r--r--   0        0        0     4657 2023-07-24 05:42:21.879592 pglive-0.6.7/pglive/examples_pyqt5/__init__.py
+-rw-r--r--   0        0        0     1093 2023-07-24 05:42:21.879592 pglive-0.6.7/pglive/examples_pyqt5/all_plot_types.py
+-rw-r--r--   0        0        0     1992 2023-07-24 05:42:21.879592 pglive-0.6.7/pglive/examples_pyqt5/axis.py
+-rw-r--r--   0        0        0      685 2023-07-24 05:42:21.879592 pglive-0.6.7/pglive/examples_pyqt5/candlestick_plot.py
+-rw-r--r--   0        0        0     1416 2023-07-24 05:42:21.879592 pglive-0.6.7/pglive/examples_pyqt5/categorized_bar_plot.py
+-rw-r--r--   0        0        0     2957 2023-07-24 05:42:21.879592 pglive-0.6.7/pglive/examples_pyqt5/crop_offset_to_data.py
+-rw-r--r--   0        0        0     2650 2023-07-24 05:42:21.879592 pglive-0.6.7/pglive/examples_pyqt5/crosshair.py
+-rw-r--r--   0        0        0        0 2023-07-24 05:42:21.879592 pglive-0.6.7/pglive/examples_pyqt5/designer_example/__init__.py
+-rw-r--r--   0        0        0      813 2023-07-24 05:42:21.879592 pglive-0.6.7/pglive/examples_pyqt5/designer_example/main_example.py
+-rw-r--r--   0        0        0     2203 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt5/designer_example/win_template.py
+-rw-r--r--   0        0        0     1489 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt5/designer_example/win_template.ui
+-rw-r--r--   0        0        0      610 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt5/horizontal_bar_plot.py
+-rw-r--r--   0        0        0     2498 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt5/leading_line.py
+-rw-r--r--   0        0        0      630 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt5/line_plot.py
+-rw-r--r--   0        0        0     6533 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt5/live_plot_range.py
+-rw-r--r--   0        0        0     2061 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt5/one_plot_multiple_plot_rates.py
+-rw-r--r--   0        0        0     1767 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt5/pause_resume.py
+-rw-r--r--   0        0        0      999 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt5/plot_rate.py
+-rw-r--r--   0        0        0      642 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt5/scatter_plot.py
+-rw-r--r--   0        0        0     1248 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt5/update_rate.py
+-rw-r--r--   0        0        0      683 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt5/vertical_bar_plot.py
+-rw-r--r--   0        0        0     1143 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt5/vertical_bar_plot_color.py
+-rw-r--r--   0        0        0     4657 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/__init__.py
+-rw-r--r--   0        0        0     1091 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/all_plot_types.py
+-rw-r--r--   0        0        0     1992 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/axis.py
+-rw-r--r--   0        0        0      685 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/candlestick_plot.py
+-rw-r--r--   0        0        0     1416 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/categorized_bar_plot.py
+-rw-r--r--   0        0        0     2955 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/crop_offset_to_data.py
+-rw-r--r--   0        0        0     2650 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/crosshair.py
+-rw-r--r--   0        0        0        0 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/designer_example/__init__.py
+-rw-r--r--   0        0        0      813 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/designer_example/main_example.py
+-rw-r--r--   0        0        0     2191 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/designer_example/win_template.py
+-rw-r--r--   0        0        0     1489 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/designer_example/win_template.ui
+-rw-r--r--   0        0        0      610 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/horizontal_bar_plot.py
+-rw-r--r--   0        0        0     2498 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/leading_line.py
+-rw-r--r--   0        0        0      630 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/line_plot.py
+-rw-r--r--   0        0        0     6546 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/live_plot_range.py
+-rw-r--r--   0        0        0     2061 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/one_plot_multiple_plot_rates.py
+-rw-r--r--   0        0        0     1767 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/pause_resume.py
+-rw-r--r--   0        0        0     1002 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/plot_rate.py
+-rw-r--r--   0        0        0      642 2023-07-24 05:42:21.883592 pglive-0.6.7/pglive/examples_pyqt6/scatter_plot.py
+-rw-r--r--   0        0        0     1249 2023-07-24 05:42:21.887592 pglive-0.6.7/pglive/examples_pyqt6/update_rate.py
+-rw-r--r--   0        0        0      683 2023-07-24 05:42:21.887592 pglive-0.6.7/pglive/examples_pyqt6/vertical_bar_plot.py
+-rw-r--r--   0        0        0     1143 2023-07-24 05:42:21.887592 pglive-0.6.7/pglive/examples_pyqt6/vertical_bar_plot_color.py
+-rw-r--r--   0        0        0     4661 2023-07-27 06:26:42.860036 pglive-0.6.7/pglive/examples_pyside6/__init__.py
+-rw-r--r--   0        0        0     1089 2023-07-24 05:42:21.887592 pglive-0.6.7/pglive/examples_pyside6/all_plot_types.py
+-rw-r--r--   0        0        0     1994 2023-07-24 05:42:21.887592 pglive-0.6.7/pglive/examples_pyside6/axis.py
+-rw-r--r--   0        0        0      687 2023-07-24 05:42:21.887592 pglive-0.6.7/pglive/examples_pyside6/candlestick_plot.py
+-rw-r--r--   0        0        0     1418 2023-07-24 05:42:21.887592 pglive-0.6.7/pglive/examples_pyside6/categorized_bar_plot.py
+-rw-r--r--   0        0        0     2958 2023-07-24 05:42:21.887592 pglive-0.6.7/pglive/examples_pyside6/crop_offset_to_data.py
+-rw-r--r--   0        0        0     2656 2023-07-24 05:42:21.887592 pglive-0.6.7/pglive/examples_pyside6/crosshair.py
+-rw-r--r--   0        0        0      612 2023-07-24 05:42:21.887592 pglive-0.6.7/pglive/examples_pyside6/horizontal_bar_plot.py
+-rw-r--r--   0        0        0     2500 2023-07-24 05:42:21.887592 pglive-0.6.7/pglive/examples_pyside6/leading_line.py
+-rw-r--r--   0        0        0      632 2023-07-24 13:59:38.958200 pglive-0.6.7/pglive/examples_pyside6/line_plot.py
+-rw-r--r--   0        0        0     6614 2023-07-24 05:42:21.891592 pglive-0.6.7/pglive/examples_pyside6/live_plot_range.py
+-rw-r--r--   0        0        0     2063 2023-07-24 05:42:21.891592 pglive-0.6.7/pglive/examples_pyside6/one_plot_multiple_plot_rates.py
+-rw-r--r--   0        0        0     1771 2023-07-24 05:42:21.891592 pglive-0.6.7/pglive/examples_pyside6/pause_resume.py
+-rw-r--r--   0        0        0      999 2023-07-24 05:42:21.891592 pglive-0.6.7/pglive/examples_pyside6/plot_rate.py
+-rw-r--r--   0        0        0      644 2023-07-24 05:42:21.891592 pglive-0.6.7/pglive/examples_pyside6/scatter_plot.py
+-rw-r--r--   0        0        0     1250 2023-07-24 05:42:21.891592 pglive-0.6.7/pglive/examples_pyside6/update_rate.py
+-rw-r--r--   0        0        0      685 2023-07-24 05:42:21.891592 pglive-0.6.7/pglive/examples_pyside6/vertical_bar_plot.py
+-rw-r--r--   0        0        0     1145 2023-07-27 06:26:22.811949 pglive-0.6.7/pglive/examples_pyside6/vertical_bar_plot_color.py
+-rw-r--r--   0        0        0      967 2023-07-24 05:42:21.891592 pglive-0.6.7/pglive/kwargs.py
+-rw-r--r--   0        0        0        0 2023-07-24 05:42:21.891592 pglive-0.6.7/pglive/sources/__init__.py
+-rw-r--r--   0        0        0     8734 2023-07-27 06:15:51.836352 pglive-0.6.7/pglive/sources/data_connector.py
+-rw-r--r--   0        0        0     4694 2023-07-24 05:42:21.891592 pglive-0.6.7/pglive/sources/live_axis.py
+-rw-r--r--   0        0        0     8512 2023-07-27 06:20:13.774097 pglive-0.6.7/pglive/sources/live_axis_range.py
+-rw-r--r--   0        0        0     3633 2023-07-25 14:22:14.224701 pglive-0.6.7/pglive/sources/live_candleStickPlot.py
+-rw-r--r--   0        0        0     4866 2023-07-25 14:20:04.596089 pglive-0.6.7/pglive/sources/live_categorized_bar_plot.py
+-rw-r--r--   0        0        0     6117 2023-07-27 05:51:40.248829 pglive-0.6.7/pglive/sources/live_mixins.py
+-rw-r--r--   0        0        0     6351 2023-07-27 05:53:15.673148 pglive-0.6.7/pglive/sources/live_plot.py
+-rw-r--r--   0        0        0    11010 2023-07-27 06:15:51.852352 pglive-0.6.7/pglive/sources/live_plot_widget.py
+-rw-r--r--   0        0        0     1599 2023-07-24 05:42:21.891592 pglive-0.6.7/pglive/sources/utils.py
+-rw-r--r--   0        0        0      940 2023-07-24 14:15:43.792538 pglive-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     6062 1970-01-01 00:00:00.000000 pglive-0.6.7/PKG-INFO
```

### Comparing `pglive-0.6.6/LICENSE` & `pglive-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/README.md` & `pglive-0.6.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # Live pyqtgraph plot
 
 Pglive package adds support for thread-safe live plotting to pyqtgraph.  
-It supports PyQt5, PyQt6, PySide2 and PySide6.
+It supports PyQt5, PyQt6 and PySide6.
 
 # Description #
 
-By default, pyqtgraph doesn't support live plotting. Aim of this package is to provide easy implementation of Line,
-Scatter and Bar Live plot. Every plot is connected with it's DataConnector, which sole purpose is to consume data points
-and manage data re-plotting. DataConnector interface provides Pause and Resume method, update rate and maximum number of
-plotted points. Each time data point is collected, call `DataConnector.cb_set_data`
-or `DataConnector.cb_append_data_point` callback. That's all You need to update plot with new data. Callbacks are Thread
-safe, so it works nicely in applications with multiple data collection Threads.
+By default, pyqtgraph doesn't support real-time plotting. Aim of this package is to provide easy way to implement various Live plots.
+Every plot is connected with DataConnector, which sole purpose is to consume data points
+and manage data re-plotting / clearing. DataConnector interface provides Pause and Resume method, update rate and maximum number of
+plotted points. Each time data point is collected, call `DataConnector.cb_set_data`, `DataConnector.cb_append_data_array`
+or `DataConnector.cb_append_data_point` callback. Calling `DataConnector.clear` will clear the plot.
+That's all you need to update plot with new data. Callbacks are Thread  safe, so it works nicely in multithreaded applications.
 
 **Focus on data collection and leave plotting to pglive.**
 
-To make firsts steps easy, package comes with many examples implemented in PyQt5 or PyQt6.
-Support for PySide2 and PySide6 was added in version 0.3.0.
+To make firsts steps easy, package comes with many examples implemented in PyQt5, PyQt6 and PySide6.
+
+# News #
+
+- Added `clear` method to `DataConnector` which can be used to clear plot data.
+- PySide2 support was removed in **v0.6.6** due to the fact, that is no longer supported by devs. Removing PySide2 allowed me to support current Python versions.  
 
 # Code examples #
 
 ```python
 import sys
 from math import sin
 from threading import Thread
```

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/__init__.py` & `pglive-0.6.7/pglive/examples_pyqt5/__init__.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/all_plot_types.py` & `pglive-0.6.7/pglive/examples_pyqt5/all_plot_types.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/axis.py` & `pglive-0.6.7/pglive/examples_pyqt5/axis.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/candlestick_plot.py` & `pglive-0.6.7/pglive/examples_pyqt5/candlestick_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/categorized_bar_plot.py` & `pglive-0.6.7/pglive/examples_pyqt5/categorized_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/crop_offset_to_data.py` & `pglive-0.6.7/pglive/examples_pyqt5/crop_offset_to_data.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/crosshair.py` & `pglive-0.6.7/pglive/examples_pyqt5/crosshair.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/designer_example/main_example.py` & `pglive-0.6.7/pglive/examples_pyqt5/designer_example/main_example.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/designer_example/win_template.py` & `pglive-0.6.7/pglive/examples_pyqt5/designer_example/win_template.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/designer_example/win_template.ui` & `pglive-0.6.7/pglive/examples_pyqt5/designer_example/win_template.ui`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/horizontal_bar_plot.py` & `pglive-0.6.7/pglive/examples_pyqt5/horizontal_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/leading_line.py` & `pglive-0.6.7/pglive/examples_pyqt5/leading_line.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/line_plot.py` & `pglive-0.6.7/pglive/examples_pyqt5/line_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/live_plot_range.py` & `pglive-0.6.7/pglive/examples_pyqt5/live_plot_range.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/one_plot_multiple_plot_rates.py` & `pglive-0.6.7/pglive/examples_pyqt5/one_plot_multiple_plot_rates.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/pause_resume.py` & `pglive-0.6.7/pglive/examples_pyqt5/pause_resume.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/plot_rate.py` & `pglive-0.6.7/pglive/examples_pyqt5/plot_rate.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/scatter_plot.py` & `pglive-0.6.7/pglive/examples_pyqt5/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/update_rate.py` & `pglive-0.6.7/pglive/examples_pyqt5/update_rate.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/vertical_bar_plot.py` & `pglive-0.6.7/pglive/examples_pyqt5/vertical_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt5/vertical_bar_plot_color.py` & `pglive-0.6.7/pglive/examples_pyqt5/vertical_bar_plot_color.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/__init__.py` & `pglive-0.6.7/pglive/examples_pyqt6/__init__.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/all_plot_types.py` & `pglive-0.6.7/pglive/examples_pyqt6/all_plot_types.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/axis.py` & `pglive-0.6.7/pglive/examples_pyqt6/axis.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/candlestick_plot.py` & `pglive-0.6.7/pglive/examples_pyqt6/candlestick_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/categorized_bar_plot.py` & `pglive-0.6.7/pglive/examples_pyqt6/categorized_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/crop_offset_to_data.py` & `pglive-0.6.7/pglive/examples_pyqt6/crop_offset_to_data.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/crosshair.py` & `pglive-0.6.7/pglive/examples_pyqt6/crosshair.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/designer_example/main_example.py` & `pglive-0.6.7/pglive/examples_pyqt6/designer_example/main_example.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/designer_example/win_template.py` & `pglive-0.6.7/pglive/examples_pyqt6/designer_example/win_template.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/designer_example/win_template.ui` & `pglive-0.6.7/pglive/examples_pyqt6/designer_example/win_template.ui`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/horizontal_bar_plot.py` & `pglive-0.6.7/pglive/examples_pyqt6/horizontal_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/leading_line.py` & `pglive-0.6.7/pglive/examples_pyqt6/leading_line.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/line_plot.py` & `pglive-0.6.7/pglive/examples_pyqt6/line_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/live_plot_range.py` & `pglive-0.6.7/pglive/examples_pyqt6/live_plot_range.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/one_plot_multiple_plot_rates.py` & `pglive-0.6.7/pglive/examples_pyqt6/one_plot_multiple_plot_rates.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/pause_resume.py` & `pglive-0.6.7/pglive/examples_pyqt6/pause_resume.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/plot_rate.py` & `pglive-0.6.7/pglive/examples_pyqt6/plot_rate.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/scatter_plot.py` & `pglive-0.6.7/pglive/examples_pyqt6/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/update_rate.py` & `pglive-0.6.7/pglive/examples_pyqt6/update_rate.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/vertical_bar_plot.py` & `pglive-0.6.7/pglive/examples_pyqt6/vertical_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyqt6/vertical_bar_plot_color.py` & `pglive-0.6.7/pglive/examples_pyqt6/vertical_bar_plot_color.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/examples_pyside2/__init__.py` & `pglive-0.6.7/pglive/examples_pyside6/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import random
 import signal
 import sys
 from math import sin, cos
 from time import sleep
 from typing import List
 
-from PySide2.QtGui import QColor
-from PySide2.QtWidgets import QApplication
+from PySide6.QtGui import QColor
+from PySide6.QtWidgets import QApplication
 
 running = True
 app = QApplication(sys.argv)
 
 
 def stop():
     """Stop current QApplication"""
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/all_plot_types.py` & `pglive-0.6.7/pglive/examples_pyside6/all_plot_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Tuple
 
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot, LiveVBarPlot, LiveLinePlot, LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
@@ -27,9 +27,9 @@
     widget.addItem(plot)
     layout.addWidget(widget)
     args.append(DataConnector(plot, max_points=300, update_rate=50))
 
 layout.show()
 
 Thread(target=examples.sin_wave_generator, args=args).start()
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/axis.py` & `pglive-0.6.7/pglive/examples_pyside6/axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 import signal
 import time
 from math import sin
 from threading import Thread
 from time import sleep
 
 import pyqtgraph as pg  # type: ignore
@@ -51,9 +51,9 @@
         for data_connector in data_connectors:
             data_connector.cb_append_data_point(sin(x * 0.01), time.time())
         sleep(0.01)
 
 
 Thread(target=sin_wave_generator, args=connectors).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/candlestick_plot.py` & `pglive-0.6.7/pglive/examples_pyside6/candlestick_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import signal
 from threading import Thread
 
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_candleStickPlot import LiveCandleStickPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
 Candlestick Bar plot is displayed in this example.
 """
@@ -15,9 +15,9 @@
 
 data_connector = DataConnector(plot, max_points=50, update_rate=10)
 
 win.show()
 
 Thread(target=examples.candle_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/categorized_bar_plot.py` & `pglive-0.6.7/pglive/examples_pyside6/categorized_bar_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import signal
 from threading import Thread
 
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 from pglive.kwargs import Axis
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_categorized_bar_plot import LiveCategorizedBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
@@ -21,9 +21,9 @@
 win = LivePlotWidget(title="Categorized Bar Plot @ 5Hz", axisItems={'bottom': bottom_axis, 'left': left_axis})
 win.addItem(plot)
 data_connector = DataConnector(plot, max_points=50, update_rate=5)
 win.show()
 
 Thread(target=examples.category_generator, args=(data_connector,), kwargs={"categories": categories}).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/crop_offset_to_data.py` & `pglive-0.6.7/pglive/examples_pyside6/crop_offset_to_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import signal
 from threading import Thread
 
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 import pyqtgraph as pg  # type: ignore
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
@@ -65,9 +65,9 @@
 
 layout.show()
 
 Thread(target=examples.sin_wave_generator, args=(data_connector, data_connector2)).start()
 Thread(target=examples.sin_wave_generator, args=(data_connector3, data_connector4), kwargs={"flip": True}).start()
 
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/crosshair.py` & `pglive-0.6.7/pglive/examples_pyside6/crosshair.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 import signal
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
-from PySide2.QtCore import QPointF
-from PySide2.QtWidgets import QWidget, QGridLayout, QLabel
+from PySide6.QtCore import QPointF
+from PySide6.QtWidgets import QWidget, QGridLayout, QLabel
 
 from pglive.kwargs import Crosshair
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
@@ -73,9 +73,9 @@
 widget.sig_crosshair_out.connect(crosshair_out)
 widget.sig_crosshair_in.connect(crosshair_in)
 
 parent_widget.show()
 
 Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/horizontal_bar_plot.py` & `pglive-0.6.7/pglive/examples_pyside6/vertical_bar_plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
+import signal
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
-from pglive.sources.live_plot import LiveHBarPlot
+from pglive.sources.live_plot import LiveVBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-Horizontal Bar plot is displayed in this example.
+Vertical Bar plot is displayed in this example.
 """
-win = LivePlotWidget(title="Horizontal Bar Plot @ 100Hz")
-plot = LiveHBarPlot(bar_height=1, brush="green", pen="green")
+win = LivePlotWidget(title="Vertical Bar Plot @ 100Hz")
+plot = LiveVBarPlot(bar_width=1, brush="blue", pen="blue")
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
+
 win.show()
 
 Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
-examples.app.exec_()
+signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/leading_line.py` & `pglive-0.6.7/pglive/examples_pyside6/leading_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 from pyqtgraph import mkPen  # type: ignore
 
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 
 from pglive.kwargs import LeadingLine
@@ -50,9 +50,9 @@
 data_connector4 = DataConnector(plot, max_points=300, update_rate=50)
 layout.addWidget(plot_widget_4)
 
 layout.show()
 
 Thread(target=examples.sin_wave_generator, args=(data_connector, data_connector3, data_connector4)).start()
 Thread(target=examples.sin_wave_generator, args=(data_connector2, ), kwargs={"flip": True}).start()
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/line_plot.py` & `pglive-0.6.7/pglive/examples_pyside6/line_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 import signal
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
@@ -15,9 +15,9 @@
 
 data_connector = DataConnector(plot, max_points=600)
 
 win.show()
 
 Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/live_plot_range.py` & `pglive-0.6.7/pglive/examples_pyside6/live_plot_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 import signal
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 from pglive.kwargs import Axis
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
@@ -148,9 +148,9 @@
 # ---
 
 layout.show()
 Thread(target=examples.sin_wave_generator, args=args).start()
 Thread(target=examples.sin_wave_generator, args=args2, kwargs={"flip": True}).start()
 
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/one_plot_multiple_plot_rates.py` & `pglive-0.6.7/pglive/examples_pyside6/one_plot_multiple_plot_rates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import signal
 from threading import Thread
 
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 import pyqtgraph as pg  # type: ignore
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
@@ -37,9 +37,9 @@
 data_connector = DataConnector(plot, max_points=6000, plot_rate=100)
 data_connector2 = DataConnector(plot2, max_points=6000, plot_rate=1, ignore_auto_range=True)
 layout.show()
 
 Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
 Thread(target=examples.cos_wave_generator, args=(data_connector2,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/pause_resume.py` & `pglive-0.6.7/pglive/examples_pyside6/pause_resume.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 import signal
 from threading import Thread
 
-from PySide2.QtWidgets import QWidget, QGridLayout, QPushButton, QLabel
+from PySide6.QtWidgets import QWidget, QGridLayout, QPushButton, QLabel
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
 Pause and Resume functionality of DataConnector is demonstrated in this example.
@@ -45,9 +45,9 @@
 data_connector.sig_paused.connect(lambda: status_label.setText("Paused"))
 data_connector.sig_resumed.connect(lambda: status_label.setText("Live"))
 
 parent_widget.show()
 
 Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/plot_rate.py` & `pglive-0.6.7/pglive/examples_pyside6/plot_rate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
@@ -21,15 +21,14 @@
 bar_height = 1
 for index in range(4):
     widget = LivePlotWidget(title=f"Horizontal Bar Plot @ {plot_rate}Hz")
     plot = LiveHBarPlot(bar_height=bar_height, brush="green", pen="green")
     widget.addItem(plot)
     layout.addWidget(widget)
     args.append(DataConnector(plot, max_points=max_len, plot_rate=plot_rate))
-    # divide all important parameters by 4
     plot_rate /= 4.
 
 layout.show()
 
 Thread(target=examples.sin_wave_generator, args=args).start()
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/scatter_plot.py` & `pglive-0.6.7/pglive/examples_pyside6/scatter_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 import signal
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
@@ -15,9 +15,9 @@
 
 data_connector = DataConnector(plot, max_points=600)
 
 win.show()
 
 Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/update_rate.py` & `pglive-0.6.7/pglive/examples_pyside6/update_rate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 from math import ceil
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot
@@ -32,9 +32,9 @@
     # bar height depends on Y distance, that's why we should multiply it by 4
     # if we leave it at 1, we get smaller bars
     bar_height *= 4
 
 layout.show()
 
 Thread(target=examples.sin_wave_generator, args=args).start()
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/vertical_bar_plot.py` & `pglive-0.6.7/pglive/examples_pyside6/horizontal_bar_plot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-import pglive.examples_pyside2 as examples
-import signal
+import pglive.examples_pyside6 as examples
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
-from pglive.sources.live_plot import LiveVBarPlot
+from pglive.sources.live_plot import LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-Vertical Bar plot is displayed in this example.
+Horizontal Bar plot is displayed in this example.
 """
-win = LivePlotWidget(title="Vertical Bar Plot @ 100Hz")
-plot = LiveVBarPlot(bar_width=1, brush="blue", pen="blue")
+win = LivePlotWidget(title="Horizontal Bar Plot @ 100Hz")
+plot = LiveHBarPlot(bar_height=1, brush="green", pen="green")
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
-
 win.show()
 
 Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
-signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/examples_pyside2/vertical_bar_plot_color.py` & `pglive-0.6.7/pglive/examples_pyside6/vertical_bar_plot_color.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 import signal
 from math import sin
 from threading import Thread
 from time import sleep
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveVBarPlot
@@ -30,9 +30,9 @@
         sleep(0.01)
 
 
 win.show()
 
 Thread(target=sin_wave_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.6/pglive/kwargs.py` & `pglive-0.6.7/pglive/kwargs.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/sources/data_connector.py` & `pglive-0.6.7/pglive/sources/data_connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import time
 import warnings
 from collections import deque
 from math import inf
 from threading import Lock
 from typing import List, Union, Deque, Optional
 
@@ -17,14 +18,15 @@
 
 class DataConnector(QtCore.QObject):
     sig_new_data = QtCore.Signal(object, object, dict)
     sig_data_roll_tick = QtCore.Signal(object, int)
     sig_data_toggle = QtCore.Signal(object, bool)
     sig_paused = QtCore.Signal()
     sig_resumed = QtCore.Signal()
+    sig_clear = QtCore.Signal()
     paused: bool = False
     # Last update time, using perf_counter for most precise counter
     last_update: float = 0.
     last_plot: float = 0.
 
     def __init__(self, plot: Union[MixinLivePlot, MixinLiveBarPlot], max_points: float = inf, update_rate: float = inf,
                  plot_rate: float = inf, ignore_auto_range: bool = False) -> None:
@@ -57,14 +59,15 @@
         self.plot_timeout = 1 / plot_rate
         self.tick_position_indexes = None
         self.plot = plot
         # Set plot and connect sig_new_data with plot.slot_new_data
         self.sig_new_data.connect(self.plot.slot_new_data)
         self.sig_data_toggle.connect(self.plot.slot_connector_toggle)
         self.sig_data_roll_tick.connect(self.plot.slot_roll_tick)
+        self.sig_clear.connect(self.plot.clear)
         self.x: Union[NUM_LIST, Deque[NUM], List]
         self.y: Union[NUM_LIST, Deque[NUM], List]
         if self.max_points == inf:
             # Use simple list if there is no point limits
             self.x = []
             self.y = []
         else:
@@ -95,29 +98,39 @@
         self.sig_paused.emit()
 
     def resume(self) -> None:
         """Resume data plotting"""
         self.paused = False
         self.sig_resumed.emit()
 
+    def clear(self) -> None:
+        """Clear all data"""
+        with self.data_lock:
+            self.x.clear()
+            self.y.clear()
+            self.rolling_index = 0
+            self.tick_position_indexes = None
+            self.sig_clear.emit()
+            self.sig_data_roll_tick.emit(self, 0)
+
     def _skip_update(self) -> bool:
         """Skip data update"""
         return self.paused or (time.perf_counter() - self.last_update) < self.update_timeout or self.data_lock.locked()
 
     def _skip_plot(self) -> bool:
         """Skip data plot"""
         return self.paused or (time.perf_counter() - self.last_plot) < self.plot_timeout
 
     def _update_data(self, **kwargs):
         """Update data and last update time"""
         # Notify all connected plots
         try:
             self.sig_new_data.emit(np.asarray(self.y), np.asarray(self.x), kwargs)
         except ValueError:
-            self.sig_new_data.emit(self.y, np.asarray(self.x), kwargs)
+            self.sig_new_data.emit(copy.copy(self.y), np.asarray(self.x), kwargs)
         self.last_plot = time.perf_counter()
 
     def cb_set_data(self, y: List[Union[int, float]], x: Optional[NUM_LIST] = None, **kwargs) -> None:
         """Replace current data"""
         if self._skip_update():
             return
```

### Comparing `pglive-0.6.6/pglive/sources/live_axis.py` & `pglive-0.6.7/pglive/sources/live_axis.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/sources/live_axis_range.py` & `pglive-0.6.7/pglive/sources/live_axis_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         self.final_x_range = [0., 0.]
         self.final_y_range = [0., 0.]
         self.ignored_data_connectors: List[str] = []
 
     def get_x_range(self, data_connector, tick: int) -> List[float]:
         axis_range = data_connector.plot.data_bounds(ax=0, offset=self.roll_on_tick if self.roll_on_tick > 1 else 0)
         x, _ = data_connector.plot.getData()
+        if x is None:
+            return [0.]
 
         final_range = self._get_range(axis_range, tick, (self.offset_left, self.offset_right))
         if final_range is None:
             return self.final_x_range
         offset_x = data_connector.plot.pos().x()
         final_range[0] += offset_x
         final_range[1] += offset_x
@@ -76,14 +78,17 @@
         if self.final_x_range != final_range:
             self.final_x_range = final_range
         return self.final_x_range
 
     def get_y_range(self, data_connector, tick: int) -> List[float]:
         axis_range = data_connector.plot.data_bounds(ax=1, offset=self.roll_on_tick if self.roll_on_tick > 1 else 0)
         _, y = data_connector.plot.getData()
+        if y is None:
+            return [0.]
+
         final_range = self._get_range(axis_range, tick, (self.offset_bottom, self.offset_top))
         if final_range is None:
             return self.final_y_range
         offset_y = data_connector.plot.pos().y()
         final_range[0] += offset_y
         final_range[1] += offset_y
         # Check left and right offset and crop to data if flag is set
```

### Comparing `pglive-0.6.6/pglive/sources/live_candleStickPlot.py` & `pglive-0.6.7/pglive/sources/live_candleStickPlot.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,24 @@
 
     def paint(self, p: QtGui.QPainter, *args: Any) -> None:
         p.drawPicture(0, 0, self.picture)
 
     def boundingRect(self) -> QtCore.QRect:
         return QtCore.QRectF(self.picture.boundingRect())
 
+    def clear(self):
+        self.x_data = []
+        self.y_data = []
+        self.output_y_data = []
+        self.picture = QtGui.QPicture()
+        self.prepareGeometryChange()
+        self.informViewBoundsChanged()
+        self.bounds = [None, None]
+        self.sigPlotChanged.emit(self)
+
     def setData(self, x_data: List[float], y_data: List[Tuple[float, ...]], **kwargs: Dict) -> None:
         """y_data must be in format [[open, close, min, max], ...]"""
         self.x_data = x_data
         self.y_data = y_data
         self.output_y_data = []
         if len(x_data) != len(y_data):
             raise Exception("Len of x_data must be the same as y_data")
@@ -73,12 +83,14 @@
         y_text = str([round(x, 4) for x in self.y_data[-1]])
         self.update_leading_text(last_x_point, last_y_point, y_text=y_text)
 
     def getData(self) -> Tuple[List[float], List[Tuple[float, ...]]]:
         return self.x_data, self.y_data
 
     def data_bounds(self, ax: int = 0, offset: int = 0) -> Tuple[ndarray, ndarray]:
+        if self.x_data == [] and self.output_y_data == []:
+            return 0, 0
         if ax == 0:
             sub_range = self.x_data[-offset:]
         else:
             sub_range = self.output_y_data[-offset * 2:]
         return np.nanmin(sub_range), np.nanmax(sub_range)
```

### Comparing `pglive-0.6.6/pglive/sources/live_categorized_bar_plot.py` & `pglive-0.6.7/pglive/sources/live_categorized_bar_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,24 @@
 
     def paint(self, p: QtGui.QPainter, *args: Any) -> None:
         p.drawPicture(0, 0, self.picture)
 
     def boundingRect(self) -> QtCore.QRect:
         return QtCore.QRectF(self.picture.boundingRect())
 
+    def clear(self):
+        self.x_data = []
+        self.y_data = []
+        self.output_y_data = []
+        self.picture = QtGui.QPicture()
+        self.prepareGeometryChange()
+        self.informViewBoundsChanged()
+        self.bounds = [None, None]
+        self.sigPlotChanged.emit(self)
+
     def setData(self, x_data: List[float], y_data: List[Tuple[str]], **kwargs: Dict) -> None:
         """y_data must be in format [[category1, category2, ...], ...]"""
         self.x_data = x_data
         self.y_data = y_data
         if len(x_data) != len(y_data):
             raise Exception("Len of x_data must be the same as y_data")
 
@@ -99,12 +109,14 @@
         self.update_leading_text(last_x_point, last_y_point, y_text=y_text)
 
     def getData(self):
         return self.x_data, self.y_data
 
     def data_bounds(self, ax: int = 0, offset: int = 0) -> Tuple:
         if ax == 0:
+            if self.x_data == []:
+                return 0, 0
             sub_range = self.x_data[-offset:]
             return np.nanmin(sub_range), np.nanmax(sub_range)
         else:
             h = self.bar_height / 2
             return 0 - h, len(self.categories) - (1 - h)
```

### Comparing `pglive-0.6.6/pglive/sources/live_mixins.py` & `pglive-0.6.7/pglive/sources/live_mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Union, Optional, Protocol, Dict, Any, TYPE_CHECKING, List, Tuple
+from typing import Union, Optional, Protocol, Dict, Any, TYPE_CHECKING
 
 import pyqtgraph as pg  # type: ignore
 from pyqtgraph.Qt import QtGui, QtCore  # type: ignore
 
 from pglive.kwargs import LeadingLine
 from pglive.sources.live_plot_widget import LivePlotWidget
 from pglive.sources.utils import NUM_LIST
@@ -133,7 +133,14 @@
         if self._hl_kwargs is not None:
             text_axis = x_text if self._hl_kwargs["text_axis"] == LeadingLine.AXIS_X else y_text
             self._hl_kwargs["text"].setText(text_axis)
             pixel_pos = vb.mapViewToScene(QtCore.QPointF(x, y))
             x_pos = width - self._hl_kwargs["text"].boundingRect().width() + 21
             new_pos = vb.mapSceneToView(QtCore.QPointF(x_pos, pixel_pos.y()))
             self._hl_kwargs["text"].setPos(new_pos.x(), new_pos.y())
+
+    def clear_leading_lines(self):
+        if self._vl_kwargs is not None:
+            self._vl_kwargs["line"].setPos(0)
+        if self._hl_kwargs is not None:
+            self._hl_kwargs["line"].setPos(0)
+        self.update_leading_text(0, 0)
```

### Comparing `pglive-0.6.6/pglive/sources/live_plot.py` & `pglive-0.6.7/pglive/sources/live_plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,37 +13,57 @@
         if self._vl_kwargs is not None:
             self._vl_kwargs["line"].setPos(self.xData[-1])
 
         if self._hl_kwargs is not None:
             self._hl_kwargs["line"].setPos(self.yData[-1])
         self.update_leading_text(self.xData[-1], self.yData[-1])
 
+    def clear(self):
+        try:
+            self.clear_leading_lines()
+        except:
+            pass
+
+        super().clear()
+
     def data_bounds(self, ax: int = 0, offset: int = 0) -> Tuple:
         x, y = self.getData()
+        if x is None and y is None:
+            return 0, 0
         if ax == 0:
             sub_range = x[-offset:]
         else:
             sub_range = y[-offset:]
         return np.nanmin(sub_range), np.nanmax(sub_range)
 
 
 class LiveScatterPlot(pg.ScatterPlotItem, MixinLivePlot, MixinLeadingLine):
     """Scatter plot"""
 
+    def clear(self):
+        try:
+            self.clear_leading_lines()
+        except AttributeError:
+            pass
+
+        super().clear()
+
     def update_leading_line(self) -> None:
         last_point = self.data[-1]
         if self._vl_kwargs is not None:
             self._vl_kwargs["line"].setPos(last_point[0])
         if self._hl_kwargs is not None:
             self._hl_kwargs["line"].setPos(last_point[1])
 
         self.update_leading_text(last_point[0], last_point[1])
 
     def data_bounds(self, ax: int = 0, offset: int = 0) -> Tuple[np.ndarray, np.ndarray]:
         x, y = self.getData()
+        if x.size == 0 and y.size == 0:
+            return 0, 0
         if ax == 0:
             sub_range = x[-offset:]
         else:
             sub_range = y[-offset:]
         return np.nanmin(sub_range), np.nanmax(sub_range)
 
 
@@ -55,26 +75,36 @@
         self.x0 = x0
         super().__init__(x0=x0, y=[0], width=0, height=0, **kwargs)
 
     def setData(self, x_data: float, y_data: float, **kwargs: Dict) -> None:
         self.setOpts(x0=self.x0, y=x_data, height=self.bar_height, width=y_data, **kwargs)
         self.sigPlotChanged.emit()
 
+    def clear(self):
+        self.setOpts(x0=self.x0, y=[], height=self.bar_height, width=[])
+        self.sigPlotChanged.emit()
+
     def getData(self) -> Tuple[List[float], List[float]]:
         return self.opts["width"], self.opts["y"]
 
     def update_leading_line(self) -> None:
+        if self.opts["width"] == [] and self.opts["y"] == []:
+            self.clear_leading_lines()
+            return
+
         if self._vl_kwargs is not None:
             self._vl_kwargs["line"].setPos(self.opts["width"][-1])
         if self._hl_kwargs is not None:
             self._hl_kwargs["line"].setPos(self.opts["y"][-1])
         self.update_leading_text(self.opts["width"][-1], self.opts["y"][-1])
 
     def data_bounds(self, ax: int = 0, offset: int = 0) -> Tuple[np.ndarray, np.ndarray]:
         x, y = self.getData()
+        if x == [] and y == []:
+            return 0, 0
         if ax == 0:
             sub_range = x[-offset:]
         else:
             sub_range = y[-offset:]
         return np.nanmin(sub_range), np.nanmax(sub_range)
 
 
@@ -86,23 +116,33 @@
         self.y0 = y0
         super().__init__(y0=y0, x=[0], width=0, height=0, **kwargs)
 
     def setData(self, x_data: float, y_data: float, **kwargs: Dict) -> None:
         self.setOpts(y0=self.y0, x=x_data, height=y_data, width=self.bar_width, **kwargs)
         self.sigPlotChanged.emit()
 
+    def clear(self):
+        self.setOpts(y0=self.y0, x=[], height=[], width=self.bar_width)
+        self.sigPlotChanged.emit()
+
     def update_leading_line(self) -> None:
+        if self.opts["x"] == [] and self.opts["height"] == []:
+            self.clear_leading_lines()
+            return
+
         if self._vl_kwargs is not None:
             self._vl_kwargs["line"].setPos(self.opts["x"][-1])
         if self._hl_kwargs is not None:
             self._hl_kwargs["line"].setPos(self.opts["height"][-1])
         self.update_leading_text(self.opts["x"][-1], self.opts["height"][-1])
 
     def data_bounds(self, ax: int = 0, offset: int = 0) -> Tuple[np.ndarray, np.ndarray]:
         x, y = self.getData()
+        if x == [] and y == []:
+            return 0, 0
         if ax == 0:
             sub_range = x[-offset:]
         else:
             sub_range = y[-offset:]
         return np.nanmin(sub_range), np.nanmax(sub_range)
 
 
@@ -117,14 +157,16 @@
     elif isinstance(plot, pg.PlotCurveItem):
         plot.slot_new_data = lambda y, x, kwargs: plot.setData(np.array(x), np.array(y), **kwargs)
     else:
         plot.slot_new_data = lambda y, x, kwargs: plot.setData(x, y, **kwargs)
 
     def data_bounds(ax: int = 0, offset: int = 0) -> Tuple[np.ndarray, np.ndarray]:
         x, y = plot.getData()
+        if x is None and y is None:
+            return 0, 0
         if ax == 0:
             sub_range = x[-offset:]
         else:
             sub_range = y[-offset:]
         return np.nanmin(sub_range), np.nanmax(sub_range)
 
     plot.data_bounds = data_bounds
```

### Comparing `pglive-0.6.6/pglive/sources/live_plot_widget.py` & `pglive-0.6.7/pglive/sources/live_plot_widget.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pglive/sources/utils.py` & `pglive-0.6.7/pglive/sources/utils.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.6/pyproject.toml` & `pglive-0.6.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "pglive"
-version = "0.6.6"
+version = "0.6.7"
 description = "Pyqtgraph live plot"
 authors = ["Martin Domaracky <domarm@comat.sk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/domarm-comat/pglive"
 repository = "https://github.com/domarm-comat/pglive"
-keywords = ["pyqtgraph", "realtime", "live", "plotting", "pyqt5", "pyqt6", "pyside2", "pyside6"]
+keywords = ["pyqtgraph", "realtime", "live", "plotting", "pyqt5", "pyqt6", "pyside6"]
 classifiers = [
 "Programming Language :: Python :: 3",
 "Operating System :: OS Independent",
 "Topic :: Software Development :: Libraries",
 "License :: OSI Approved :: MIT License",
 "Natural Language :: English",
 "Intended Audience :: Science/Research",
```

### Comparing `pglive-0.6.6/PKG-INFO` & `pglive-0.6.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pglive
-Version: 0.6.6
+Version: 0.6.7
 Summary: Pyqtgraph live plot
 Home-page: https://github.com/domarm-comat/pglive
 License: MIT
-Keywords: pyqtgraph,realtime,live,plotting,pyqt5,pyqt6,pyside2,pyside6
+Keywords: pyqtgraph,realtime,live,plotting,pyqt5,pyqt6,pyside6
 Author: Martin Domaracky
 Author-email: domarm@comat.sk
 Requires-Python: >=3.8,<3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -22,29 +22,33 @@
 Requires-Dist: pyqtgraph (>=0.13.3,<0.14.0)
 Project-URL: Repository, https://github.com/domarm-comat/pglive
 Description-Content-Type: text/markdown
 
 # Live pyqtgraph plot
 
 Pglive package adds support for thread-safe live plotting to pyqtgraph.  
-It supports PyQt5, PyQt6, PySide2 and PySide6.
+It supports PyQt5, PyQt6 and PySide6.
 
 # Description #
 
-By default, pyqtgraph doesn't support live plotting. Aim of this package is to provide easy implementation of Line,
-Scatter and Bar Live plot. Every plot is connected with it's DataConnector, which sole purpose is to consume data points
-and manage data re-plotting. DataConnector interface provides Pause and Resume method, update rate and maximum number of
-plotted points. Each time data point is collected, call `DataConnector.cb_set_data`
-or `DataConnector.cb_append_data_point` callback. That's all You need to update plot with new data. Callbacks are Thread
-safe, so it works nicely in applications with multiple data collection Threads.
+By default, pyqtgraph doesn't support real-time plotting. Aim of this package is to provide easy way to implement various Live plots.
+Every plot is connected with DataConnector, which sole purpose is to consume data points
+and manage data re-plotting / clearing. DataConnector interface provides Pause and Resume method, update rate and maximum number of
+plotted points. Each time data point is collected, call `DataConnector.cb_set_data`, `DataConnector.cb_append_data_array`
+or `DataConnector.cb_append_data_point` callback. Calling `DataConnector.clear` will clear the plot.
+That's all you need to update plot with new data. Callbacks are Thread  safe, so it works nicely in multithreaded applications.
 
 **Focus on data collection and leave plotting to pglive.**
 
-To make firsts steps easy, package comes with many examples implemented in PyQt5 or PyQt6.
-Support for PySide2 and PySide6 was added in version 0.3.0.
+To make firsts steps easy, package comes with many examples implemented in PyQt5, PyQt6 and PySide6.
+
+# News #
+
+- Added `clear` method to `DataConnector` which can be used to clear plot data.
+- PySide2 support was removed in **v0.6.6** due to the fact, that is no longer supported by devs. Removing PySide2 allowed me to support current Python versions.  
 
 # Code examples #
 
 ```python
 import sys
 from math import sin
 from threading import Thread
```

