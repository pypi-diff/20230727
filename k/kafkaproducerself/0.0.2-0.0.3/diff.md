# Comparing `tmp/kafkaproducerself-0.0.2.tar.gz` & `tmp/kafkaproducerself-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafkaproducerself-0.0.2.tar", last modified: Thu Jul 27 07:11:31 2023, max compression
+gzip compressed data, was "kafkaproducerself-0.0.3.tar", last modified: Thu Jul 27 07:13:51 2023, max compression
```

## Comparing `kafkaproducerself-0.0.2.tar` & `kafkaproducerself-0.0.3.tar`

### file list

```diff
@@ -1,972 +1,973 @@
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.864097 kafkaproducerself-0.0.2/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       77 2023-07-27 05:31:37.000000 kafkaproducerself-0.0.2/CHANGELOG.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1062 2023-07-27 05:34:59.000000 kafkaproducerself-0.0.2/LICENSE.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       25 2023-07-27 05:32:21.000000 kafkaproducerself-0.0.2/MANIFEST.in
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1062 2023-07-27 07:11:31.864097 kafkaproducerself-0.0.2/PKG-INFO
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      728 2023-07-27 07:10:46.000000 kafkaproducerself-0.0.2/README.txt
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.800091 kafkaproducerself-0.0.2/kafkaproducerself/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       23 2023-07-26 06:35:22.000000 kafkaproducerself-0.0.2/kafkaproducerself/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1065 2023-07-27 04:45:01.000000 kafkaproducerself-0.0.2/kafkaproducerself/producer.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.800091 kafkaproducerself-0.0.2/kafkaproducerself.egg-info/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1062 2023-07-27 07:11:31.000000 kafkaproducerself-0.0.2/kafkaproducerself.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    58012 2023-07-27 07:11:31.000000 kafkaproducerself-0.0.2/kafkaproducerself.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        1 2023-07-27 07:11:31.000000 kafkaproducerself-0.0.2/kafkaproducerself.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       18 2023-07-27 07:11:31.000000 kafkaproducerself-0.0.2/kafkaproducerself.egg-info/top_level.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       38 2023-07-27 07:11:31.864097 kafkaproducerself-0.0.2/setup.cfg
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      408 2023-07-27 07:09:29.000000 kafkaproducerself-0.0.2/setup.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.784089 kafkaproducerself-0.0.2/venv/
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.800091 kafkaproducerself-0.0.2/venv/bin/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1176 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/bin/activate_this.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.784089 kafkaproducerself-0.0.2/venv/lib/
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.784089 kafkaproducerself-0.0.2/venv/lib/python3.10/
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.800091 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.800091 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/_distutils_hack/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6299 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/_distutils_hack/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       44 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/_distutils_hack/override.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5640 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/_virtualenv.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.800091 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1077 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.804092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/admin/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      720 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/admin/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8265 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/admin/acl_resource.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    63518 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/admin/client.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1039 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/admin/config_resource.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      757 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/admin/new_partitions.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1306 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/admin/new_topic.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    45265 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/client_async.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14822 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/cluster.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9548 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/codec.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    68402 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/conn.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.804092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/consumer/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      122 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/consumer/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    47679 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/consumer/fetcher.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    58768 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/consumer/group.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    21665 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/consumer/subscription_state.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.804092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.804092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1507 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/abstract.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2912 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/range.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3776 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/roundrobin.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.804092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6476 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/partition_movements.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1904 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/sorted_set.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    34114 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/sticky_assignor.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    46140 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/base.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    38920 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/consumer.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2304 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/heartbeat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1041 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/protocol.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16324 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/errors.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2474 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/future.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.804092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      574 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      776 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/compound_stat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2567 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/dict_reporter.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      933 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/kafka_metric.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      770 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/measurable.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      503 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/measurable_stat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1154 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/metric_config.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3419 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/metric_name.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10314 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/metrics.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1398 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/metrics_reporter.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1128 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/quota.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      628 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stat.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.804092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      629 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      678 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/avg.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      487 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/count.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2874 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/histogram.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      546 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/max_stat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      568 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/min_stat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      342 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/percentile.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2901 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/percentiles.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4533 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/rate.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3458 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/sampled_stat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5129 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/sensor.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      418 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/total.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.804092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/oauth/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       95 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/oauth/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1296 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/oauth/abstract.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.804092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/partitioner/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      158 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/partitioner/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2879 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/partitioner/default.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.804092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/producer/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      122 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/producer/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4370 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/producer/buffer.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3039 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/producer/future.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    37649 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/producer/kafka.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    24994 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/producer/record_accumulator.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22968 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/producer/sender.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.808092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1075 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      385 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/abstract.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    25122 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/admin.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2493 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/api.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6888 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/commit.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11014 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/fetch.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      734 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/frame.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5599 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/group.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7657 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/message.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6116 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/metadata.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4707 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/offset.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6963 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/parser.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      920 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/pickle.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6460 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/produce.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2380 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/struct.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5427 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/types.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.808092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      129 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5753 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/_crc32c.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3465 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/abc.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    21023 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/default_records.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17820 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/legacy_records.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6344 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/memory_records.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3556 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/util.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3034 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/scram.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.808092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/serializer/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      103 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/serializer/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      486 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/serializer/abstract.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2927 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/structs.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1856 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/util.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.812092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/vendor/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/vendor/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    31204 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/vendor/enum34.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20502 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/vendor/selectors34.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    31133 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/vendor/six.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2127 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/vendor/socketpair.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       22 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/version.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.812092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka_python-2.0.2.dist-info/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        6 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka_python-2.0.2.dist-info/top_level.txt
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.812092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      357 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1198 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/__main__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1444 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/__pip-runner__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.812092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      573 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10243 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/build_env.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9661 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cache.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.812092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      132 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6676 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8176 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30030 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      774 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2816 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/main.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4338 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10817 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1968 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18328 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5118 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      116 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/status_codes.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.816093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3882 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7581 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1684 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/check.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4129 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9815 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6591 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5182 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/download.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2951 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1703 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1132 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/help.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4793 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/index.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3188 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    28722 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/install.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12343 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/list.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5697 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/search.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6419 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/show.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3886 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6324 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13529 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/configuration.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.816093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      858 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1221 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      729 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6494 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1164 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    23741 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/exceptions.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.816093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       30 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16504 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/collector.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    37873 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6556 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/sources.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.816093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15365 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6100 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7680 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2556 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/base.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      340 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/main.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.816093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4280 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2595 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    25277 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.816093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      107 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1882 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8181 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7457 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9773 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.816093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       63 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      990 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6931 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2520 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1030 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/index.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2619 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18817 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/link.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      738 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4643 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1907 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3858 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3600 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.816093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       50 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20435 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/auth.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2145 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/cache.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6096 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/download.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7638 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18442 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/session.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4073 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/utils.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1791 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.816093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.820093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4133 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1422 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1474 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2198 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1075 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1417 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3064 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5122 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/check.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9816 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.820093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       51 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1282 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    27475 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    27696 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7161 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/pyproject.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.820093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2738 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16610 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17872 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    32782 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2858 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    24678 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.820093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      583 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.820093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    24128 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.820093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5220 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18864 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    27845 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5705 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9824 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3094 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5454 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11538 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8167 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.820093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3351 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1015 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1665 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1884 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5377 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      242 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/datetime.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3627 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3206 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2118 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1169 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3064 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5122 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      716 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3110 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5118 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      795 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11632 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22216 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1193 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/models.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2108 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4435 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9200 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7702 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8821 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1759 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3456 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4549 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.820093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      596 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3519 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18116 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5238 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11729 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22811 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11842 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.824093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4966 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.824093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      465 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1379 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5033 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1535 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.824093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      242 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5271 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1033 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      778 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16416 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3946 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4154 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7105 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      774 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.824093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       94 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/certifi/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      255 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/certifi/__main__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4279 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.824093 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4797 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    31274 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1763 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10032 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3915 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5420 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.828094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3242 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3732 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      542 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1860 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1683 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4006 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12176 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3934 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13566 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1753 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    36913 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1753 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20735 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1759 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14537 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    25796 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    42498 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1752 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    27055 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   104562 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    98484 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    98196 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   101363 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   128035 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   102774 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    95372 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5380 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6077 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3715 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2131 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30391 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.828094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13560 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      402 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/resultdict.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6400 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4137 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4007 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14848 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8505 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2812 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      244 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/version.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.828094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      266 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2522 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11128 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3325 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.828094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       75 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2839 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10678 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6741 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1866 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1079 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3709 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6181 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7134 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.828094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      581 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    41259 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    51697 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20834 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    51991 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14811 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5058 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39801 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10820 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18102 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    66262 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    23513 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    43898 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.828094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distro/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      981 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       64 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distro/__main__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    49330 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.828094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      849 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3374 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      321 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12950 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    44375 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1881 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       21 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/package_data.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   206539 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.828094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1132 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1081 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6079 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    34544 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.828094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      661 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      497 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11488 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4378 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1431 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8487 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4676 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30110 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15699 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4200 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14665 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.828094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   109388 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.832094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18003 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1198 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4303 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5706 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2800 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7448 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      160 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/version.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7098 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.832094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2999 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      353 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/__main__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    23685 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1697 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1938 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.832094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    40386 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2917 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.832094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4800 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4104 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3314 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5086 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    35601 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    21938 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4981 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19351 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5073 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2212 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5014 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7335 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4674 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11753 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    32064 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.832094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11164 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    71556 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    53572 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      986 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2591 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3072 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3092 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6882 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6257 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.832094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3419 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6184 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    63187 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9110 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.832094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9171 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6426 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12936 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   213344 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.832094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    23685 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9023 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39129 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    25341 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13402 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10787 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6805 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.832094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      491 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      138 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11920 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_impl.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.832094 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      546 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10927 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.836095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5178 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      435 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/__version__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1397 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    21443 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6377 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10187 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      575 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1286 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18560 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3823 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3879 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      733 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    35288 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      695 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30180 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4235 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2912 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    33240 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.836095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      537 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.836095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      156 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5871 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1601 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20511 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4963 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.840095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6090 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8478 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10096 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   140235 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1064 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2100 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      265 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_extension.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      799 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_fileno.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9695 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3225 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1236 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1387 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_null_file.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7063 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      423 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_pick.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5472 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19919 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      351 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_stack.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      417 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_timer.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22820 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1926 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2783 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1840 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      890 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10368 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6906 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3264 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9842 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4509 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18224 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1054 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7131 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    99195 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1288 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5497 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6630 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8082 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      972 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2501 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      642 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1683 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2508 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9584 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5032 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3252 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14007 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14273 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3667 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11903 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8198 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5305 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4970 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      828 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3396 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10574 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    35852 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    59706 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8165 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11303 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1391 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      166 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/region.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4431 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4602 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2843 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1591 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    24247 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4339 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4425 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    27073 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1258 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    35153 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39684 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3370 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    45525 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3777 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      102 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/themes.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    29604 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9169 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    34549 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/six.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.840095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20493 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3551 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2179 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1682 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1562 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2372 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1383 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8746 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3086 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2142 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8024 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.840095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      396 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22633 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2943 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      254 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_types.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    84101 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.840095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3333 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10811 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       64 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_version.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20300 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39128 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.840095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      957 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.840095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17632 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13922 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11036 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4528 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17081 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    34448 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7097 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8217 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8579 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2440 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.844095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.844095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1417 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    34665 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19786 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5985 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30641 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.844095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1155 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4901 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1605 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      498 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3997 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3510 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22003 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17177 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5758 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6895 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10168 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14296 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5403 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      476 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/vendor.txt
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.844095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10579 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8979 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1305 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6563 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4307 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.812092 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9953 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1093 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/LICENSE.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      125 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        4 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/top_level.txt
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.844095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   109427 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.844095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.844095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      506 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4504 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5457 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2925 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      884 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3481 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5140 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3581 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2576 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.844095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7460 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15056 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/functools.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.844095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15526 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.844095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      148 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   134976 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    25416 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.844095 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      501 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3266 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_elffile.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8926 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2524 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10194 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_parser.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1431 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5292 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8208 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16397 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/metadata.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3287 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39206 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18106 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4355 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16326 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.848096 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12806 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1164 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4068 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/android.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4910 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/api.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2655 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/macos.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6911 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/unix.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      160 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/version.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6596 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/windows.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    80078 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/typing_extensions.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8425 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/zipp.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.848096 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/extern/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2442 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.848096 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9257 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.852096 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      359 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5300 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/_collections.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      411 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/_functools.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       43 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/_log.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      239 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/_macos_compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19616 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8572 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14721 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    48643 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17861 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.852096 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      430 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1614 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5408 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4665 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22013 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5584 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7684 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    31503 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16537 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5604 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4872 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2594 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13077 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30153 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2762 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2788 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1180 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8409 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1932 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      672 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11817 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19232 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7491 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4911 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/config.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9397 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/core.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11924 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      139 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/debug.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3414 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8072 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    50174 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/dist.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3589 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/errors.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10270 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/extension.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17899 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8212 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13715 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1201 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/log.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30188 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    23577 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      217 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/py38compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      639 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/py39compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3495 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18928 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12085 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15601 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18099 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/util.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12951 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/version.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5205 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2282 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_entry_points.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2395 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_imp.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1466 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_importlib.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      675 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_itertools.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3706 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_normalization.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1056 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_path.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      882 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_reqs.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.852096 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.856097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    26498 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2454 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      743 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1859 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2895 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2068 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1165 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1098 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2166 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_text.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.856097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      506 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4504 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5457 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2925 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      884 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3481 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5140 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3581 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2576 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/simple.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.856097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7460 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/context.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15053 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/functools.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.856097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/text/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15517 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/text/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.856097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       82 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   117959 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16256 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15130 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.856097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      501 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3266 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_elffile.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8926 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2524 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10194 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_parser.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1431 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5292 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_tokenizer.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8208 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16397 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/metadata.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3287 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39206 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18106 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4355 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16326 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.856097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      396 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22633 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2943 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_re.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      254 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_types.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    87149 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/typing_extensions.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8425 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/zipp.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7346 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/archive_util.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19778 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/build_meta.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.860097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      396 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2381 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/alias.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16596 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1353 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6784 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4423 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build_clib.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15821 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build_ext.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15012 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build_py.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6744 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/develop.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4195 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/dist_info.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    86117 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/easy_install.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    31965 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/editable_wheel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    27278 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/egg_info.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5598 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2123 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3875 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install_lib.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2714 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install_scripts.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      468 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/register.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2128 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/rotate.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      658 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/saveopts.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7007 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/sdist.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5086 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/setopt.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8102 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/test.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      462 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/upload.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7690 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/upload_docs.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.860097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1498 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13755 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_apply_pyprojecttoml.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.860097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1038 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11266 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1153 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1612 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   274907 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9161 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16353 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/expand.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17396 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/pyprojecttoml.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    26184 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/setupcfg.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      949 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/dep_util.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5499 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/depends.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    21087 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/discovery.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    46807 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/dist.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2464 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/errors.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5591 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/extension.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.860097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/extern/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2527 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/extern/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4873 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/glob.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4926 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/installer.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      812 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/launch.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1232 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/logging.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4697 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/monkey.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    47345 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/msvc.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3093 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/namespaces.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    38349 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/package_index.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      330 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/py312compat.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14349 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/sandbox.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      941 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/unicode_utils.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      161 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/version.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3664 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/warnings.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8608 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/wheel.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      718 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/windows_support.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.848096 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools-68.0.0.dist-info/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2676 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools-68.0.0.dist-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       41 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools-68.0.0.dist-info/top_level.txt
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.860097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       59 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      455 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/__main__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      746 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/_setuptools_logging.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19868 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/bdist_wheel.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.860097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3932 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9427 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/convert.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4338 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/pack.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5124 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/tags.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1021 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/unpack.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16143 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/macosx_libfile.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5889 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/metadata.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      621 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/util.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.860097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/__init__.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.864097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3266 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_elffile.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8813 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_manylinux.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2524 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_musllinux.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9399 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_parser.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1431 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_structures.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5148 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_tokenizer.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8161 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/markers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3264 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/requirements.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39047 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/specifiers.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18065 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/tags.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4355 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/utils.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16295 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/version.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       16 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/vendor.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7674 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/wheelfile.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:11:31.860097 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel-0.40.0.dist-info/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1107 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel-0.40.0.dist-info/LICENSE.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      104 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel-0.40.0.dist-info/entry_points.txt
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.352167 kafkaproducerself-0.0.3/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       77 2023-07-27 05:31:37.000000 kafkaproducerself-0.0.3/CHANGELOG.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1062 2023-07-27 05:34:59.000000 kafkaproducerself-0.0.3/LICENSE.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       25 2023-07-27 05:32:21.000000 kafkaproducerself-0.0.3/MANIFEST.in
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1014 2023-07-27 07:13:51.352167 kafkaproducerself-0.0.3/PKG-INFO
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      680 2023-07-27 07:13:33.000000 kafkaproducerself-0.0.3/README.txt
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.228158 kafkaproducerself-0.0.3/kafkaproducerself/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       23 2023-07-26 06:35:22.000000 kafkaproducerself-0.0.3/kafkaproducerself/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1065 2023-07-27 04:45:01.000000 kafkaproducerself-0.0.3/kafkaproducerself/producer.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.228158 kafkaproducerself-0.0.3/kafkaproducerself.egg-info/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1014 2023-07-27 07:13:51.000000 kafkaproducerself-0.0.3/kafkaproducerself.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    58052 2023-07-27 07:13:51.000000 kafkaproducerself-0.0.3/kafkaproducerself.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        1 2023-07-27 07:13:51.000000 kafkaproducerself-0.0.3/kafkaproducerself.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       13 2023-07-27 07:13:51.000000 kafkaproducerself-0.0.3/kafkaproducerself.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       18 2023-07-27 07:13:51.000000 kafkaproducerself-0.0.3/kafkaproducerself.egg-info/top_level.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       38 2023-07-27 07:13:51.352167 kafkaproducerself-0.0.3/setup.cfg
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      420 2023-07-27 07:12:56.000000 kafkaproducerself-0.0.3/setup.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.216157 kafkaproducerself-0.0.3/venv/
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.228158 kafkaproducerself-0.0.3/venv/bin/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1176 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/bin/activate_this.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.216157 kafkaproducerself-0.0.3/venv/lib/
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.216157 kafkaproducerself-0.0.3/venv/lib/python3.10/
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.228158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.228158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/_distutils_hack/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6299 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/_distutils_hack/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       44 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/_distutils_hack/override.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5640 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/_virtualenv.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.228158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1077 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.228158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/admin/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      720 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/admin/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8265 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/admin/acl_resource.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    63518 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/admin/client.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1039 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/admin/config_resource.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      757 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/admin/new_partitions.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1306 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/admin/new_topic.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    45265 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/client_async.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14822 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/cluster.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9548 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/codec.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    68402 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/conn.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.228158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/consumer/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      122 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/consumer/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    47679 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/consumer/fetcher.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    58768 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/consumer/group.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    21665 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/consumer/subscription_state.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.228158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.232158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1507 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/abstract.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2912 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/range.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3776 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/roundrobin.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.232158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6476 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/partition_movements.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1904 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/sorted_set.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    34114 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/sticky_assignor.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    46140 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/base.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    38920 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/consumer.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2304 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/heartbeat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1041 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/protocol.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16324 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/errors.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2474 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/future.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.232158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      574 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      776 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/compound_stat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2567 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/dict_reporter.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      933 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/kafka_metric.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      770 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/measurable.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      503 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/measurable_stat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1154 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/metric_config.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3419 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/metric_name.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10314 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/metrics.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1398 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/metrics_reporter.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1128 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/quota.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      628 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stat.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.232158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      629 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      678 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/avg.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      487 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/count.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2874 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/histogram.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      546 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/max_stat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      568 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/min_stat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      342 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/percentile.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2901 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/percentiles.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4533 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/rate.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3458 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/sampled_stat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5129 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/sensor.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      418 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/total.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.232158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/oauth/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       95 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/oauth/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1296 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/oauth/abstract.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.232158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/partitioner/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      158 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/partitioner/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2879 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/partitioner/default.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.232158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/producer/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      122 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/producer/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4370 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/producer/buffer.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3039 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/producer/future.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    37649 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/producer/kafka.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    24994 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/producer/record_accumulator.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22968 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/producer/sender.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.232158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1075 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      385 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/abstract.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    25122 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/admin.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2493 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/api.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6888 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/commit.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11014 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/fetch.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      734 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/frame.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5599 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/group.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7657 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/message.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6116 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/metadata.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4707 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/offset.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6963 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/parser.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      920 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/pickle.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6460 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/produce.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2380 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/struct.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5427 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/types.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.232158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      129 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5753 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/_crc32c.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3465 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/abc.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    21023 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/default_records.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17820 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/legacy_records.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6344 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/memory_records.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3556 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/util.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3034 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/scram.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.236158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/serializer/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      103 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/serializer/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      486 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/serializer/abstract.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2927 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/structs.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1856 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/util.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.236158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/vendor/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/vendor/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    31204 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/vendor/enum34.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20502 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/vendor/selectors34.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    31133 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/vendor/six.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2127 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/vendor/socketpair.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       22 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/version.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.236158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka_python-2.0.2.dist-info/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        6 2023-07-26 06:09:17.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka_python-2.0.2.dist-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.236158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      357 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1198 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/__main__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1444 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/__pip-runner__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.236158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      573 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10243 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/build_env.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9661 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cache.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.236158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      132 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6676 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8176 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30030 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      774 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2816 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/main.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4338 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10817 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1968 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18328 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5118 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      116 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/status_codes.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.236158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3882 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7581 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1684 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/check.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4129 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9815 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6591 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5182 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/download.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2951 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1703 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1132 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/help.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4793 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/index.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3188 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    28722 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/install.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12343 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/list.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5697 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/search.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6419 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/show.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3886 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6324 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13529 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/configuration.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.240159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/distributions/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      858 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1221 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      729 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6494 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1164 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    23741 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/exceptions.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.240159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/index/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       30 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/index/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16504 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/index/collector.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    37873 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6556 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/index/sources.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.240159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/locations/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15365 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6100 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7680 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2556 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/locations/base.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      340 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/main.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.240159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4280 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2595 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    25277 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.240159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      107 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1882 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8181 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7457 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9773 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.240159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       63 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      990 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6931 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2520 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1030 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/index.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2619 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18817 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/link.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      738 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4643 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1907 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3858 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3600 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.240159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       50 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20435 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/auth.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2145 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/cache.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6096 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/download.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7638 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18442 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/session.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4073 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/utils.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1791 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.240159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.244159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4133 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1422 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1474 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2198 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1075 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1417 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3064 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5122 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/check.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9816 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.244159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/install/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       51 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/install/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1282 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    27475 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    27696 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7161 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/pyproject.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.244159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/req/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2738 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16610 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17872 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    32782 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2858 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    24678 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.244159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      583 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.244159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    24128 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.244159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5220 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18864 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    27845 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5705 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9824 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3094 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5454 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11538 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8167 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.244159 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3351 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1015 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1665 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1884 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5377 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      242 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/datetime.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3627 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3206 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2118 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1169 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3064 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5122 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      716 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3110 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5118 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      795 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11632 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22216 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1193 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/models.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2108 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4435 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9200 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7702 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8821 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1759 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3456 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4549 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.248160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/vcs/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      596 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3519 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18116 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5238 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11729 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22811 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11842 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.248160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4966 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.248160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      465 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1379 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5033 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1535 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.248160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      242 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5271 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1033 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      778 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16416 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3946 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4154 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7105 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      774 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.248160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       94 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      255 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4279 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.252160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4797 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    31274 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1763 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10032 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3915 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5420 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.252160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3242 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3732 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      542 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1860 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1683 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4006 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12176 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3934 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13566 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1753 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    36913 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1753 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20735 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1759 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14537 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    25796 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    42498 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1752 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    27055 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   104562 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    98484 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    98196 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   101363 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   128035 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   102774 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    95372 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5380 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6077 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3715 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2131 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30391 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.252160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13560 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      402 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6400 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4137 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4007 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14848 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8505 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2812 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      244 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/version.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.252160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      266 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2522 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11128 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3325 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.252160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       75 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2839 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10678 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6741 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1866 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1079 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3709 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6181 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7134 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.256160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      581 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    41259 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    51697 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20834 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    51991 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14811 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5058 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39801 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10820 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18102 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    66262 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    23513 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    43898 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.256160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distro/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      981 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       64 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distro/__main__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    49330 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.256160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      849 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3374 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      321 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12950 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    44375 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1881 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       21 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   206539 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.256160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1132 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1081 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6079 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    34544 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.256160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      661 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      497 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11488 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4378 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1431 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8487 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4676 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30110 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15699 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4200 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14665 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.256160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   109388 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.256160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18003 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1198 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4303 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5706 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2800 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7448 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      160 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/version.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7098 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.256160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2999 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      353 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/__main__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    23685 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1697 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1938 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.256160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    40386 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2917 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.260160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4800 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4104 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3314 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5086 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    35601 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    21938 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4981 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19351 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5073 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2212 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5014 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7335 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4674 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11753 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    32064 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.260160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11164 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    71556 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    53572 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      986 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2591 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3072 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3092 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6882 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6257 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.260160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3419 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6184 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    63187 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9110 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.260160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9171 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6426 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12936 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   213344 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.260160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    23685 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9023 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39129 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    25341 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13402 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10787 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6805 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.260160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      491 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      138 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11920 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.260160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      546 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10927 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.260160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5178 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      435 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1397 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    21443 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6377 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10187 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      575 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1286 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18560 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3823 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3879 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      733 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    35288 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      695 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30180 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4235 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2912 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    33240 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.260160 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      537 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.264161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      156 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5871 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1601 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20511 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4963 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.268161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6090 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8478 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10096 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   140235 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1064 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2100 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      265 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_extension.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      799 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_fileno.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9695 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3225 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1236 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1387 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_null_file.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7063 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      423 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_pick.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5472 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19919 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      351 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_stack.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      417 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_timer.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22820 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1926 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2783 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1840 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      890 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10368 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6906 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3264 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9842 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4509 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18224 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1054 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7131 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    99195 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1288 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5497 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6630 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8082 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      972 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2501 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      642 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1683 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2508 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9584 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5032 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3252 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14007 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14273 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3667 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11903 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8198 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5305 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4970 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      828 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3396 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10574 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    35852 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    59706 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8165 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11303 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1391 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      166 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/region.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4431 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4602 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2843 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1591 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    24247 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4339 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4425 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    27073 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1258 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    35153 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39684 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3370 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    45525 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3777 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      102 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/themes.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    29604 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9169 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    34549 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/six.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.268161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20493 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3551 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2179 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1682 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1562 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2372 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1383 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8746 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3086 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2142 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8024 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.268161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tomli/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      396 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tomli/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22633 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2943 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      254 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_types.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    84101 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.272161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3333 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10811 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       64 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_version.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    20300 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39128 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.272161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      957 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.272161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17632 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13922 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11036 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4528 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17081 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    34448 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7097 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8217 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8579 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2440 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.272161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.272161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1417 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    34665 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19786 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5985 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30641 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.272161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1155 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4901 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1605 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      498 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3997 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3510 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22003 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17177 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5758 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6895 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10168 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14296 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5403 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      476 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/vendor.txt
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.272161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10579 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8979 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1305 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6563 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4307 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.236158 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9953 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1093 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      125 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        4 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.272161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   109427 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.272161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.272161 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      506 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4504 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5457 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2925 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      884 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3481 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5140 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3581 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2576 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.276162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7460 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15056 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/functools.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.276162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15526 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.276162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      148 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   134976 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    25416 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.276162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      501 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3266 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_elffile.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8926 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2524 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10194 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_parser.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1431 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5292 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8208 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16397 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/metadata.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3287 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39206 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18106 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4355 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16326 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.276162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12806 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1164 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4068 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/android.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4910 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/api.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2655 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/macos.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6911 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/unix.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      160 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/version.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6596 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/windows.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    80078 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/typing_extensions.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8425 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/zipp.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.276162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/extern/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2442 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.280162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9257 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.280162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      359 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5300 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/_collections.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      411 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/_functools.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       43 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/_log.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      239 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19616 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8572 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14721 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    48643 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17861 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.280162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      430 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1614 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5408 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4665 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22013 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5584 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7684 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    31503 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16537 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5604 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4872 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2594 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13077 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30153 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2762 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2788 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1180 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8409 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1932 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      672 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11817 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19232 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7491 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4911 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/config.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9397 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/core.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11924 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      139 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/debug.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3414 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8072 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    50174 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/dist.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3589 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/errors.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10270 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/extension.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17899 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8212 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13715 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1201 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/log.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    30188 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    23577 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      217 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/py38compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      639 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/py39compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3495 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18928 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12085 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15601 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18099 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/util.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    12951 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/version.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5205 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2282 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_entry_points.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2395 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_imp.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1466 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_importlib.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      675 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_itertools.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3706 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_normalization.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1056 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_path.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      882 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_reqs.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.280162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.284162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    26498 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2454 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      743 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1859 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2895 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2068 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1165 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1098 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2166 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.284162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      506 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4504 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5457 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2925 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      884 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3481 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5140 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3581 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2576 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/simple.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.284162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7460 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15053 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/functools.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.284162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/text/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15517 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.284162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       82 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   117959 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16256 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15130 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.284162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      501 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3266 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_elffile.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8926 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2524 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    10194 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_parser.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1431 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5292 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_tokenizer.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8208 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16397 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/metadata.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3287 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39206 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18106 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4355 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16326 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.284162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      396 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    22633 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2943 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      254 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    87149 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8425 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/zipp.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7346 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/archive_util.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19778 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/build_meta.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.348167 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      396 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2381 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/alias.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16596 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1353 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6784 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/build.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4423 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/build_clib.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15821 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/build_ext.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    15012 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/build_py.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     6744 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/develop.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4195 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/dist_info.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    86117 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/easy_install.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    31965 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/editable_wheel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    27278 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/egg_info.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5598 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/install.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2123 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3875 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/install_lib.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2714 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/install_scripts.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      468 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/register.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2128 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/rotate.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      658 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/saveopts.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7007 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/sdist.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5086 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/setopt.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8102 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/test.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      462 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/upload.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7690 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/upload_docs.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.348167 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1498 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    13755 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_apply_pyprojecttoml.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.348167 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1038 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    11266 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1153 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1612 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)   274907 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9161 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16353 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/expand.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    17396 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/pyprojecttoml.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    26184 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/setupcfg.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      949 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/dep_util.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5499 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/depends.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    21087 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/discovery.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    46807 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/dist.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2464 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/errors.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5591 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/extension.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.348167 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/extern/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2527 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/extern/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4873 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/glob.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4926 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/installer.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      812 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/launch.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1232 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/logging.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4697 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/monkey.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    47345 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/msvc.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3093 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/namespaces.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    38349 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/package_index.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      330 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/py312compat.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    14349 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/sandbox.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      941 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/unicode_utils.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      161 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/version.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3664 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/warnings.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8608 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/wheel.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      718 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/windows_support.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.280162 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools-68.0.0.dist-info/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2676 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools-68.0.0.dist-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       41 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools-68.0.0.dist-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.348167 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       59 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      455 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/__main__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      746 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/_setuptools_logging.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    19868 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/bdist_wheel.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.352167 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/cli/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3932 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9427 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/cli/convert.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4338 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/cli/pack.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5124 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/cli/tags.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1021 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/cli/unpack.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16143 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/macosx_libfile.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5889 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/metadata.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      621 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/util.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.352167 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/__init__.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.352167 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        0 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3266 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_elffile.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8813 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_manylinux.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     2524 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_musllinux.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     9399 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_parser.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1431 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_structures.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     5148 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_tokenizer.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     8161 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/markers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     3264 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/requirements.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    39047 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/specifiers.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    18065 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/tags.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     4355 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/utils.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)    16295 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/version.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       16 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/vendor.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     7674 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/wheelfile.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2023-07-27 07:13:51.348167 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel-0.40.0.dist-info/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)     1107 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel-0.40.0.dist-info/LICENSE.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      104 2023-07-26 06:08:56.000000 kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel-0.40.0.dist-info/entry_points.txt
```

### Comparing `kafkaproducerself-0.0.2/LICENSE.txt` & `kafkaproducerself-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/PKG-INFO` & `kafkaproducerself-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: kafkaproducerself
-Version: 0.0.2
+Version: 0.0.3
 Summary: produce events to kafka
 Home-page: UNKNOWN
 Author: Abhishek Borana
 Author-email: tracer.domanik@fixedfor.com
 License: MIT
 Keywords: kafka
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 It provides general functions to get kafka producer and publish events using it, additonally a health check also there to make sure connections is live.
 
 It provides three functions :
 
 -- health_check  
-    accepts url as parameter
-    returns tuple
-    True/False : Depending if connection is on or not
-    String : Success or failure message
+accepts url as parameter
+returns tuple
+True/False : Depending if connection is on or not
+String : Success or failure message
 
 
 -- connect_to_kafka_producer 
-    accepts url as parameter
-    returns tuple
-    True/False : Depending on producer status
-    Obj/String : producer object if connected else error message
+accepts url as parameter
+returns tuple
+True/False : Depending on producer status
+Obj/String : producer object if connected else error message
 
 
 -- push_event_to_kafka
-    accepts eventData, topicName, producer as parameters
-    returns tuple
-    True/False : Depending if message published or not
-    String : Success or failure message
+accepts eventData, topicName, producer as parameters
+returns tuple
+True/False : Depending if message published or not
+String : Success or failure message
 
 Change log
 ==========
 
 
 0.0.1 (27/07/2023)
 ------------------
```

### Comparing `kafkaproducerself-0.0.2/README.txt` & `kafkaproducerself-0.0.3/README.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 It provides general functions to get kafka producer and publish events using it, additonally a health check also there to make sure connections is live.
 
 It provides three functions :
 
 -- health_check  
-    accepts url as parameter
-    returns tuple
-    True/False : Depending if connection is on or not
-    String : Success or failure message
+accepts url as parameter
+returns tuple
+True/False : Depending if connection is on or not
+String : Success or failure message
 
 
 -- connect_to_kafka_producer 
-    accepts url as parameter
-    returns tuple
-    True/False : Depending on producer status
-    Obj/String : producer object if connected else error message
+accepts url as parameter
+returns tuple
+True/False : Depending on producer status
+Obj/String : producer object if connected else error message
 
 
 -- push_event_to_kafka
-    accepts eventData, topicName, producer as parameters
-    returns tuple
-    True/False : Depending if message published or not
-    String : Success or failure message
+accepts eventData, topicName, producer as parameters
+returns tuple
+True/False : Depending if message published or not
+String : Success or failure message
```

### Comparing `kafkaproducerself-0.0.2/kafkaproducerself/producer.py` & `kafkaproducerself-0.0.3/kafkaproducerself/producer.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/kafkaproducerself.egg-info/PKG-INFO` & `kafkaproducerself-0.0.3/kafkaproducerself.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: kafkaproducerself
-Version: 0.0.2
+Version: 0.0.3
 Summary: produce events to kafka
 Home-page: UNKNOWN
 Author: Abhishek Borana
 Author-email: tracer.domanik@fixedfor.com
 License: MIT
 Keywords: kafka
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 It provides general functions to get kafka producer and publish events using it, additonally a health check also there to make sure connections is live.
 
 It provides three functions :
 
 -- health_check  
-    accepts url as parameter
-    returns tuple
-    True/False : Depending if connection is on or not
-    String : Success or failure message
+accepts url as parameter
+returns tuple
+True/False : Depending if connection is on or not
+String : Success or failure message
 
 
 -- connect_to_kafka_producer 
-    accepts url as parameter
-    returns tuple
-    True/False : Depending on producer status
-    Obj/String : producer object if connected else error message
+accepts url as parameter
+returns tuple
+True/False : Depending on producer status
+Obj/String : producer object if connected else error message
 
 
 -- push_event_to_kafka
-    accepts eventData, topicName, producer as parameters
-    returns tuple
-    True/False : Depending if message published or not
-    String : Success or failure message
+accepts eventData, topicName, producer as parameters
+returns tuple
+True/False : Depending if message published or not
+String : Success or failure message
 
 Change log
 ==========
 
 
 0.0.1 (27/07/2023)
 ------------------
```

### Comparing `kafkaproducerself-0.0.2/kafkaproducerself.egg-info/SOURCES.txt` & `kafkaproducerself-0.0.3/kafkaproducerself.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.txt
 setup.py
 kafkaproducerself/__init__.py
 kafkaproducerself/producer.py
 kafkaproducerself.egg-info/PKG-INFO
 kafkaproducerself.egg-info/SOURCES.txt
 kafkaproducerself.egg-info/dependency_links.txt
+kafkaproducerself.egg-info/requires.txt
 kafkaproducerself.egg-info/top_level.txt
 venv/bin/activate_this.py
 venv/lib/python3.10/site-packages/_virtualenv.py
 venv/lib/python3.10/site-packages/_distutils_hack/__init__.py
 venv/lib/python3.10/site-packages/_distutils_hack/override.py
 venv/lib/python3.10/site-packages/kafka/__init__.py
 venv/lib/python3.10/site-packages/kafka/client_async.py
```

### Comparing `kafkaproducerself-0.0.2/venv/bin/activate_this.py` & `kafkaproducerself-0.0.3/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/_distutils_hack/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/_virtualenv.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/admin/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/admin/acl_resource.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/admin/acl_resource.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/admin/client.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/admin/client.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/admin/config_resource.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/admin/config_resource.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/admin/new_partitions.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/admin/new_partitions.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/admin/new_topic.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/admin/new_topic.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/client_async.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/client_async.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/cluster.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/cluster.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/codec.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/codec.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/conn.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/conn.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/consumer/fetcher.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/consumer/fetcher.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/consumer/group.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/consumer/group.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/consumer/subscription_state.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/consumer/subscription_state.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/abstract.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/abstract.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/range.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/range.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/roundrobin.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/roundrobin.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/partition_movements.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/partition_movements.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/sorted_set.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/sorted_set.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/sticky_assignor.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/assignors/sticky/sticky_assignor.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/base.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/base.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/consumer.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/consumer.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/heartbeat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/heartbeat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/coordinator/protocol.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/coordinator/protocol.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/errors.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/errors.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/future.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/future.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/compound_stat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/compound_stat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/dict_reporter.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/dict_reporter.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/kafka_metric.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/kafka_metric.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/measurable.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/measurable.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/metric_config.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/metric_config.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/metric_name.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/metric_name.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/metrics.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/metrics_reporter.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/metrics_reporter.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/quota.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/quota.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/avg.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/avg.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/histogram.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/histogram.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/max_stat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/max_stat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/min_stat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/min_stat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/percentiles.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/percentiles.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/rate.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/rate.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/sampled_stat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/sampled_stat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/metrics/stats/sensor.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/metrics/stats/sensor.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/oauth/abstract.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/oauth/abstract.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/partitioner/default.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/partitioner/default.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/producer/buffer.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/producer/buffer.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/producer/future.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/producer/future.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/producer/kafka.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/producer/kafka.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/producer/record_accumulator.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/producer/record_accumulator.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/producer/sender.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/producer/sender.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/admin.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/admin.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/api.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/api.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/commit.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/commit.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/fetch.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/fetch.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/frame.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/frame.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/group.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/group.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/message.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/message.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/metadata.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/metadata.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/offset.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/offset.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/parser.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/pickle.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/pickle.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/produce.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/produce.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/struct.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/struct.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/protocol/types.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/protocol/types.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/_crc32c.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/_crc32c.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/abc.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/abc.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/default_records.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/default_records.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/legacy_records.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/legacy_records.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/memory_records.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/memory_records.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/record/util.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/record/util.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/scram.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/scram.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/structs.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/structs.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/util.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/util.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/vendor/enum34.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/vendor/enum34.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/vendor/selectors34.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/vendor/selectors34.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/vendor/six.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/vendor/six.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/kafka/vendor/socketpair.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/kafka/vendor/socketpair.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/__main__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/__pip-runner__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/build_env.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cache.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/main.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/check.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/download.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/help.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/index.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/install.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/list.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/search.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/show.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/configuration.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/exceptions.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/collector.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/sources.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/base.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/index.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/link.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/auth.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/cache.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/download.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/session.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/utils.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/check.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/pyproject.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/_jaraco_text.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/models.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/macromanprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/utils.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_fileno.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_null_file.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/six.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/AUTHORS.txt` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/LICENSE.txt` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/context.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_elffile.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_parser.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/metadata.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__main__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/android.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/api.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/macos.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/unix.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/windows.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/typing_extensions.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/zipp.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/_collections.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/_framework_compat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/config.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/core.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/dist.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/errors.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/extension.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/log.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/py39compat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/util.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/version.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_entry_points.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_imp.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_importlib.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_itertools.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_normalization.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_normalization.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_path.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_reqs.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_reqs.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/context.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/functools.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_elffile.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_parser.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_tokenizer.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/metadata.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_parser.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_re.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/typing_extensions.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/zipp.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/archive_util.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/build_meta.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/alias.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build_clib.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build_ext.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build_py.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/develop.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/dist_info.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/easy_install.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/editable_wheel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/egg_info.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install_lib.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install_scripts.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/rotate.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/saveopts.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/sdist.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/setopt.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/test.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/upload_docs.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/formats.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/expand.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/pyprojecttoml.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/config/setupcfg.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/dep_util.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/depends.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/discovery.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/dist.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/errors.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/extension.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/extern/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/glob.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/installer.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/launch.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/logging.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/monkey.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/msvc.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/namespaces.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/package_index.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/sandbox.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/unicode_utils.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/warnings.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/warnings.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/wheel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools/windows_support.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/setuptools-68.0.0.dist-info/entry_points.txt` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/setuptools-68.0.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/_setuptools_logging.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/_setuptools_logging.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/bdist_wheel.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/__init__.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/convert.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/pack.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/tags.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/cli/tags.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/unpack.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/macosx_libfile.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/macosx_libfile.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/metadata.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/metadata.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/util.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/util.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_elffile.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_manylinux.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_musllinux.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_parser.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_structures.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_tokenizer.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/markers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/requirements.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/specifiers.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/tags.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/utils.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/version.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/vendored/packaging/version.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel/wheelfile.py` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `kafkaproducerself-0.0.2/venv/lib/python3.10/site-packages/wheel-0.40.0.dist-info/LICENSE.txt` & `kafkaproducerself-0.0.3/venv/lib/python3.10/site-packages/wheel-0.40.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

