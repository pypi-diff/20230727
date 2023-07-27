# Comparing `tmp/gardener-cicd-libs-1.2116.0.tar.gz` & `tmp/gardener-cicd-libs-1.2117.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-libs-1.2116.0.tar", last modified: Mon Jul 24 11:00:34 2023, max compression
+gzip compressed data, was "gardener-cicd-libs-1.2117.0.tar", last modified: Thu Jul 27 06:35:42 2023, max compression
```

## Comparing `gardener-cicd-libs-1.2116.0.tar` & `gardener-cicd-libs-1.2117.0.tar`

### file list

```diff
@@ -1,268 +1,258 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.927936 gardener-cicd-libs-1.2116.0/
--rw-r--r--   0 root         (0) root         (0)    16830 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-24 11:00:34.927936 gardener-cicd-libs-1.2116.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.899936 gardener-cicd-libs-1.2116.0/ccc/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      631 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/alicloud.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/aws.py
--rw-r--r--   0 root         (0) root         (0)      127 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/cfg.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/clamav.py
--rw-r--r--   0 root         (0) root         (0)     4131 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/concourse.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/delivery.py
--rw-r--r--   0 root         (0) root         (0)     6490 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/elasticsearch.py
--rw-r--r--   0 root         (0) root         (0)     8491 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/gcp.py
--rw-r--r--   0 root         (0) root         (0)    10733 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/github.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/grafeas_model.py
--rw-r--r--   0 root         (0) root         (0)     4925 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/oci.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/protecode.py
--rw-r--r--   0 root         (0) root         (0)     7274 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/secrets_server.py
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ccc/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.903936 gardener-cicd-libs-1.2116.0/cfg_mgmt/
--rw-r--r--   0 root         (0) root         (0)      244 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/alicloud.py
--rw-r--r--   0 root         (0) root         (0)     3198 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/aws.py
--rw-r--r--   0 root         (0) root         (0)     6025 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/azure.py
--rw-r--r--   0 root         (0) root         (0)     8833 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/btp_application_certificate.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/btp_service_binding.py
--rw-r--r--   0 root         (0) root         (0)     3433 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/gcp.py
--rw-r--r--   0 root         (0) root         (0)     6378 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/github.py
--rw-r--r--   0 root         (0) root         (0)     7825 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     3635 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/metrics.py
--rw-r--r--   0 root         (0) root         (0)    10471 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/model.py
--rw-r--r--   0 root         (0) root         (0)    14273 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/reporting.py
--rw-r--r--   0 root         (0) root         (0)     6143 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/rotate.py
--rw-r--r--   0 root         (0) root         (0)    11110 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cfg_mgmt/util.py
--rwxr-xr-x   0 root         (0) root         (0)     9186 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.903936 gardener-cicd-libs-1.2116.0/cnudie/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cnudie/__init__.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cnudie/access.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cnudie/iter.py
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cnudie/migrate.py
--rw-r--r--   0 root         (0) root         (0)     5996 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cnudie/purge.py
--rw-r--r--   0 root         (0) root         (0)     3492 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cnudie/replicate.py
--rw-r--r--   0 root         (0) root         (0)    20986 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cnudie/retrieve.py
--rw-r--r--   0 root         (0) root         (0)    17536 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cnudie/util.py
--rw-r--r--   0 root         (0) root         (0)     2662 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cnudie/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.903936 gardener-cicd-libs-1.2116.0/concourse/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.907935 gardener-cicd-libs-1.2116.0/concourse/client/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14969 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/client/api.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/client/model.py
--rw-r--r--   0 root         (0) root         (0)     6557 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/client/routes.py
--rw-r--r--   0 root         (0) root         (0)    12621 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/client/util.py
--rw-r--r--   0 root         (0) root         (0)    20369 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/enumerator.py
--rw-r--r--   0 root         (0) root         (0)    10077 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.907935 gardener-cicd-libs-1.2116.0/concourse/model/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7643 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/base.py
--rw-r--r--   0 root         (0) root         (0)    10402 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/job.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    12384 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/resources.py
--rw-r--r--   0 root         (0) root         (0)    17522 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.911936 gardener-cicd-libs-1.2116.0/concourse/model/traits/
--rw-r--r--   0 root         (0) root         (0)     2587 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14494 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/component_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     5217 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/cronjob.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/draft_release.py
--rw-r--r--   0 root         (0) root         (0)     4548 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/filter.py
--rw-r--r--   0 root         (0) root         (0)    19291 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/image_scan.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/images.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/meta.py
--rw-r--r--   0 root         (0) root         (0)     6530 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/notifications.py
--rw-r--r--   0 root         (0) root         (0)     1948 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/options.py
--rw-r--r--   0 root         (0) root         (0)    17352 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/publish.py
--rw-r--r--   0 root         (0) root         (0)     4400 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/pullrequest.py
--rw-r--r--   0 root         (0) root         (0)    11846 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/release.py
--rw-r--r--   0 root         (0) root         (0)     8268 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/scan_sources.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2705 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/slack.py
--rw-r--r--   0 root         (0) root         (0)    10333 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/update_component_deps.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/model/traits/version.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/paths.py
--rw-r--r--   0 root         (0) root         (0)    27119 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/replicator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.911936 gardener-cicd-libs-1.2116.0/concourse/resources/
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-24 11:00:28.000000 gardener-cicd-libs-1.2116.0/concourse/resources/LAST_RELEASED_TAG
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/resources/defaults.mako
--rw-r--r--   0 root         (0) root         (0)     1039 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/resources/email.mako
--rw-r--r--   0 root         (0) root         (0)     4192 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/resources/github.mako
--rw-r--r--   0 root         (0) root         (0)      463 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/resources/image.mako
--rw-r--r--   0 root         (0) root         (0)      639 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/resources/resource_types.mako
--rw-r--r--   0 root         (0) root         (0)      389 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/resources/time.mako
--rw-r--r--   0 root         (0) root         (0)     1301 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/resources/variants.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.915936 gardener-cicd-libs-1.2116.0/concourse/steps/
--rw-r--r--   0 root         (0) root         (0)     1418 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/alter_container_images.py
--rw-r--r--   0 root         (0) root         (0)     9157 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/build_oci_image.mako
--rw-r--r--   0 root         (0) root         (0)     3137 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/build_oci_image.py
--rw-r--r--   0 root         (0) root         (0)     3016 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/cfg_reporting.mako
--rw-r--r--   0 root         (0) root         (0)     4097 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/cfg_reporting.py
--rw-r--r--   0 root         (0) root         (0)    10914 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/component_descriptor.mako
--rw-r--r--   0 root         (0) root         (0)     5609 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/component_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     2260 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/component_descriptor_util.py
--rw-r--r--   0 root         (0) root         (0)     4090 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/draft_release.mako
--rw-r--r--   0 root         (0) root         (0)     1497 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/images.py
--rw-r--r--   0 root         (0) root         (0)     9120 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/malware_scan.mako
--rw-r--r--   0 root         (0) root         (0)      676 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/meta.mako
--rw-r--r--   0 root         (0) root         (0)      977 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/meta.py
--rw-r--r--   0 root         (0) root         (0)     8822 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/notification.mako
--rw-r--r--   0 root         (0) root         (0)     4621 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/notification.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/os_id.mako
--rw-r--r--   0 root         (0) root         (0)     5271 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/os_id.py
--rw-r--r--   0 root         (0) root         (0)     1743 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/prepare.mako
--rw-r--r--   0 root         (0) root         (0)     3703 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/publish.mako
--rw-r--r--   0 root         (0) root         (0)     4213 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/release.mako
--rw-r--r--   0 root         (0) root         (0)    38055 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/release.py
--rw-r--r--   0 root         (0) root         (0)     1145 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/replicate_pipelines.mako
--rw-r--r--   0 root         (0) root         (0)     1002 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/replicate_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/replicate_secrets.mako
--rw-r--r--   0 root         (0) root         (0)     6520 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/replicate_secrets.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/rm_pr_label.mako
--rw-r--r--   0 root         (0) root         (0)     7028 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/scan_container_images.mako
--rw-r--r--   0 root         (0) root         (0)     6837 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/scan_container_images.py
--rw-r--r--   0 root         (0) root         (0)     4703 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/scan_sources.mako
--rw-r--r--   0 root         (0) root         (0)     2107 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/scan_sources.py
--rw-r--r--   0 root         (0) root         (0)     6828 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/update_component_deps.mako
--rw-r--r--   0 root         (0) root         (0)    20611 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/update_component_deps.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/version.mako
--rw-r--r--   0 root         (0) root         (0)     1165 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/steps/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.915936 gardener-cicd-libs-1.2116.0/concourse/templates/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23495 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/templates/default.mako
--rw-r--r--   0 root         (0) root         (0)     5362 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/util.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/concourse/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.915936 gardener-cicd-libs-1.2116.0/container/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/container/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11787 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/container/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.915936 gardener-cicd-libs-1.2116.0/cosign/
--rw-r--r--   0 root         (0) root         (0)      735 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cosign/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/cosign/payload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.919936 gardener-cicd-libs-1.2116.0/ctt/
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/cosign.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/filters.py
--rw-r--r--   0 root         (0) root         (0)     2769 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/platform.py
--rwxr-xr-x   0 root         (0) root         (0)    27481 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/process_dependencies.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/processing_model.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/processors.py
--rw-r--r--   0 root         (0) root         (0)     6811 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/rbsc_bom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.919936 gardener-cicd-libs-1.2116.0/ctt/test/
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1683 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/test/filters_test.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/test/platform_test.py
--rw-r--r--   0 root         (0) root         (0)     1272 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/test/process_deps_test.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/test/processors_test.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/test/uploaders_test.py
--rw-r--r--   0 root         (0) root         (0)     7562 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/uploaders.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ctt/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.919936 gardener-cicd-libs-1.2116.0/delivery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/delivery/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10892 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/delivery/client.py
--rw-r--r--   0 root         (0) root         (0)     2921 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/delivery/model.py
--rw-r--r--   0 root         (0) root         (0)     1724 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/delivery/util.py
--rw-r--r--   0 root         (0) root         (0)     2025 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/dockerutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.919936 gardener-cicd-libs-1.2116.0/dso/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/dso/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9639 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/dso/cvss.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/dso/labels.py
--rw-r--r--   0 root         (0) root         (0)     5434 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/dso/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.919936 gardener-cicd-libs-1.2116.0/gardener_cicd_libs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-24 11:00:34.000000 gardener-cicd-libs-1.2116.0/gardener_cicd_libs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6074 2023-07-24 11:00:34.000000 gardener-cicd-libs-1.2116.0/gardener_cicd_libs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 11:00:34.000000 gardener-cicd-libs-1.2116.0/gardener_cicd_libs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      898 2023-07-24 11:00:34.000000 gardener-cicd-libs-1.2116.0/gardener_cicd_libs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      224 2023-07-24 11:00:34.000000 gardener-cicd-libs-1.2116.0/gardener_cicd_libs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.919936 gardener-cicd-libs-1.2116.0/github/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8440 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/codeowners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.919936 gardener-cicd-libs-1.2116.0/github/compliance/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/compliance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11309 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/compliance/issue.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/compliance/milestone.py
--rw-r--r--   0 root         (0) root         (0)     9059 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/compliance/model.py
--rw-r--r--   0 root         (0) root         (0)    34537 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/compliance/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.923936 gardener-cicd-libs-1.2116.0/github/release_notes/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4159 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/release_notes/model.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/release_notes/renderer.py
--rw-r--r--   0 root         (0) root         (0)    19222 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/release_notes/util.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/retry.py
--rw-r--r--   0 root         (0) root         (0)     1360 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/user.py
--rw-r--r--   0 root         (0) root         (0)    34243 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/util.py
--rw-r--r--   0 root         (0) root         (0)     2170 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/github/webhook.py
--rw-r--r--   0 root         (0) root         (0)    15259 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/gitutil.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/gziputil.py
--rw-r--r--   0 root         (0) root         (0)     6926 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/http_requests.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/ioutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.923936 gardener-cicd-libs-1.2116.0/mail/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/mail/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1981 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/mail/template_mailer.py
--rw-r--r--   0 root         (0) root         (0)     9573 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/mailutil.py
--rw-r--r--   0 root         (0) root         (0)      286 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/makoutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.923936 gardener-cicd-libs-1.2116.0/product/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/product/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1373 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/product/util.py
--rw-r--r--   0 root         (0) root         (0)    22350 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/product/v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.923936 gardener-cicd-libs-1.2116.0/release_notes/
--rw-r--r--   0 root         (0) root         (0)      913 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13285 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/release_notes/fetch.py
--rw-r--r--   0 root         (0) root         (0)     5613 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/release_notes/markdown.py
--rw-r--r--   0 root         (0) root         (0)    11411 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/release_notes/model.py
--rw-r--r--   0 root         (0) root         (0)     7739 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/release_notes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/reutil.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-07-24 11:00:34.927936 gardener-cicd-libs-1.2116.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2096 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.923936 gardener-cicd-libs-1.2116.0/slackclient/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/slackclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3454 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/slackclient/util.py
--rw-r--r--   0 root         (0) root         (0)     6591 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/tarutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.923936 gardener-cicd-libs-1.2116.0/test/
--rw-r--r--   0 root         (0) root         (0)     1241 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/_test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.923936 gardener-cicd-libs-1.2116.0/test/concourse/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/client_test.py
--rw-r--r--   0 root         (0) root         (0)     4760 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/factory_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.923936 gardener-cicd-libs-1.2116.0/test/concourse/model/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6657 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/model/job_test.py
--rw-r--r--   0 root         (0) root         (0)     3272 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/model/resources_test.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/model/step_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.927936 gardener-cicd-libs-1.2116.0/test/concourse/model/traits/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/model/traits/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/model/traits/component_descriptor_test.py
--rw-r--r--   0 root         (0) root         (0)     7482 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/model/traits/filter_test.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/model/traits/slack_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.927936 gardener-cicd-libs-1.2116.0/test/concourse/resources/
--rw-r--r--   0 root         (0) root         (0)     1458 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6308 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/resources/github_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.927936 gardener-cicd-libs-1.2116.0/test/concourse/steps/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/steps/component_descriptor_test.py
--rw-r--r--   0 root         (0) root         (0)     6544 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/steps/notification_test.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/steps/release_test.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/steps/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     6498 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/steps/update_component_deps_test.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/steps/version_test.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/concourse/util_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.927936 gardener-cicd-libs-1.2116.0/test/container/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/container/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.927936 gardener-cicd-libs-1.2116.0/test/github/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6142 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/github/github_util_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.927936 gardener-cicd-libs-1.2116.0/test/github/release_notes/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/github/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5803 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/github/release_notes/default_util.py
--rw-r--r--   0 root         (0) root         (0)    18172 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/github/release_notes/renderer_test.py
--rw-r--r--   0 root         (0) root         (0)    21822 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/github/release_notes/util_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.927936 gardener-cicd-libs-1.2116.0/test/product_/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/product_/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/reutil_test.py
--rw-r--r--   0 root         (0) root         (0)     5754 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/test/version_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:00:34.927936 gardener-cicd-libs-1.2116.0/unixutil/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/unixutil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/unixutil/model.py
--rw-r--r--   0 root         (0) root         (0)     3717 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/unixutil/scan.py
--rw-r--r--   0 root         (0) root         (0)    15220 2023-07-24 10:59:46.000000 gardener-cicd-libs-1.2116.0/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.427205 gardener-cicd-libs-1.2117.0/
+-rw-r--r--   0 root         (0) root         (0)    16830 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-27 06:35:42.427205 gardener-cicd-libs-1.2117.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.399205 gardener-cicd-libs-1.2117.0/ccc/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      631 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/aws.py
+-rw-r--r--   0 root         (0) root         (0)      127 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/cfg.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/clamav.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/concourse.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/delivery.py
+-rw-r--r--   0 root         (0) root         (0)     6490 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/elasticsearch.py
+-rw-r--r--   0 root         (0) root         (0)     8491 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/gcp.py
+-rw-r--r--   0 root         (0) root         (0)    10733 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/github.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/grafeas_model.py
+-rw-r--r--   0 root         (0) root         (0)     4925 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/oci.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/protecode.py
+-rw-r--r--   0 root         (0) root         (0)     7274 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/secrets_server.py
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ccc/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.399205 gardener-cicd-libs-1.2117.0/cfg_mgmt/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/aws.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/azure.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/btp_application_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/btp_service_binding.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/gcp.py
+-rw-r--r--   0 root         (0) root         (0)     6378 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/github.py
+-rw-r--r--   0 root         (0) root         (0)     7825 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     3635 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    10471 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/model.py
+-rw-r--r--   0 root         (0) root         (0)    14273 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/reporting.py
+-rw-r--r--   0 root         (0) root         (0)     6143 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/rotate.py
+-rw-r--r--   0 root         (0) root         (0)    11110 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cfg_mgmt/util.py
+-rwxr-xr-x   0 root         (0) root         (0)     9187 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.403205 gardener-cicd-libs-1.2117.0/cnudie/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cnudie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cnudie/access.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cnudie/iter.py
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cnudie/migrate.py
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cnudie/purge.py
+-rw-r--r--   0 root         (0) root         (0)     3492 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cnudie/replicate.py
+-rw-r--r--   0 root         (0) root         (0)    20986 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cnudie/retrieve.py
+-rw-r--r--   0 root         (0) root         (0)    17536 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cnudie/util.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cnudie/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.403205 gardener-cicd-libs-1.2117.0/concourse/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.403205 gardener-cicd-libs-1.2117.0/concourse/client/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14969 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/client/api.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/client/model.py
+-rw-r--r--   0 root         (0) root         (0)     6557 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/client/routes.py
+-rw-r--r--   0 root         (0) root         (0)    12621 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/client/util.py
+-rw-r--r--   0 root         (0) root         (0)    20369 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/enumerator.py
+-rw-r--r--   0 root         (0) root         (0)    10077 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.407204 gardener-cicd-libs-1.2117.0/concourse/model/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7643 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/base.py
+-rw-r--r--   0 root         (0) root         (0)    10402 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/job.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    12384 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/resources.py
+-rw-r--r--   0 root         (0) root         (0)    17522 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.407204 gardener-cicd-libs-1.2117.0/concourse/model/traits/
+-rw-r--r--   0 root         (0) root         (0)     2587 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14494 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/component_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     5217 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/cronjob.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/draft_release.py
+-rw-r--r--   0 root         (0) root         (0)     4548 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/filter.py
+-rw-r--r--   0 root         (0) root         (0)    19291 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/image_scan.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/images.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/meta.py
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/notifications.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/options.py
+-rw-r--r--   0 root         (0) root         (0)    17352 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/publish.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/pullrequest.py
+-rw-r--r--   0 root         (0) root         (0)    10761 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/release.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/scan_sources.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/slack.py
+-rw-r--r--   0 root         (0) root         (0)     9850 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/update_component_deps.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/model/traits/version.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/paths.py
+-rw-r--r--   0 root         (0) root         (0)    27119 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/replicator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.407204 gardener-cicd-libs-1.2117.0/concourse/resources/
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-27 06:35:36.000000 gardener-cicd-libs-1.2117.0/concourse/resources/LAST_RELEASED_TAG
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/resources/defaults.mako
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/resources/email.mako
+-rw-r--r--   0 root         (0) root         (0)     4192 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/resources/github.mako
+-rw-r--r--   0 root         (0) root         (0)      463 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/resources/image.mako
+-rw-r--r--   0 root         (0) root         (0)      639 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/resources/resource_types.mako
+-rw-r--r--   0 root         (0) root         (0)      389 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/resources/time.mako
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/resources/variants.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.415205 gardener-cicd-libs-1.2117.0/concourse/steps/
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/alter_container_images.py
+-rw-r--r--   0 root         (0) root         (0)     9157 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/build_oci_image.mako
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/build_oci_image.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/cfg_reporting.mako
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/cfg_reporting.py
+-rw-r--r--   0 root         (0) root         (0)    10914 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/component_descriptor.mako
+-rw-r--r--   0 root         (0) root         (0)     5609 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/component_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/component_descriptor_util.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/draft_release.mako
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/images.py
+-rw-r--r--   0 root         (0) root         (0)     9120 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/malware_scan.mako
+-rw-r--r--   0 root         (0) root         (0)      676 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/meta.mako
+-rw-r--r--   0 root         (0) root         (0)      977 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/meta.py
+-rw-r--r--   0 root         (0) root         (0)     8822 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/notification.mako
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/notification.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/os_id.mako
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/os_id.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/prepare.mako
+-rw-r--r--   0 root         (0) root         (0)     3703 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/publish.mako
+-rw-r--r--   0 root         (0) root         (0)     4137 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/release.mako
+-rw-r--r--   0 root         (0) root         (0)    34761 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/release.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/replicate_pipelines.mako
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/replicate_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/replicate_secrets.mako
+-rw-r--r--   0 root         (0) root         (0)     6520 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/replicate_secrets.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/rm_pr_label.mako
+-rw-r--r--   0 root         (0) root         (0)     7028 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/scan_container_images.mako
+-rw-r--r--   0 root         (0) root         (0)     6837 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/scan_container_images.py
+-rw-r--r--   0 root         (0) root         (0)     4703 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/scan_sources.mako
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/scan_sources.py
+-rw-r--r--   0 root         (0) root         (0)     6579 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/update_component_deps.mako
+-rw-r--r--   0 root         (0) root         (0)    19187 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/update_component_deps.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/version.mako
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/steps/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.415205 gardener-cicd-libs-1.2117.0/concourse/templates/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23495 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/templates/default.mako
+-rw-r--r--   0 root         (0) root         (0)     5362 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/util.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/concourse/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.415205 gardener-cicd-libs-1.2117.0/container/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/container/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11787 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/container/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.415205 gardener-cicd-libs-1.2117.0/cosign/
+-rw-r--r--   0 root         (0) root         (0)      735 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cosign/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/cosign/payload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.415205 gardener-cicd-libs-1.2117.0/ctt/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/cosign.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/filters.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/platform.py
+-rwxr-xr-x   0 root         (0) root         (0)    27481 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/process_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/processing_model.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/processors.py
+-rw-r--r--   0 root         (0) root         (0)     6811 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/rbsc_bom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.415205 gardener-cicd-libs-1.2117.0/ctt/test/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/test/filters_test.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/test/platform_test.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/test/process_deps_test.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/test/processors_test.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/test/uploaders_test.py
+-rw-r--r--   0 root         (0) root         (0)     7562 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/uploaders.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ctt/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.419205 gardener-cicd-libs-1.2117.0/delivery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/delivery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10892 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/delivery/client.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/delivery/model.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/delivery/util.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/dockerutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.419205 gardener-cicd-libs-1.2117.0/dso/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/dso/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9639 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/dso/cvss.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/dso/labels.py
+-rw-r--r--   0 root         (0) root         (0)     5434 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/dso/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.419205 gardener-cicd-libs-1.2117.0/gardener_cicd_libs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-27 06:35:42.000000 gardener-cicd-libs-1.2117.0/gardener_cicd_libs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5787 2023-07-27 06:35:42.000000 gardener-cicd-libs-1.2117.0/gardener_cicd_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 06:35:42.000000 gardener-cicd-libs-1.2117.0/gardener_cicd_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      898 2023-07-27 06:35:42.000000 gardener-cicd-libs-1.2117.0/gardener_cicd_libs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      224 2023-07-27 06:35:42.000000 gardener-cicd-libs-1.2117.0/gardener_cicd_libs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.419205 gardener-cicd-libs-1.2117.0/github/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8440 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/github/codeowners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.419205 gardener-cicd-libs-1.2117.0/github/compliance/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/github/compliance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11309 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/github/compliance/issue.py
+-rw-r--r--   0 root         (0) root         (0)      823 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/github/compliance/milestone.py
+-rw-r--r--   0 root         (0) root         (0)     9059 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/github/compliance/model.py
+-rw-r--r--   0 root         (0) root         (0)    34537 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/github/compliance/report.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/github/retry.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/github/user.py
+-rw-r--r--   0 root         (0) root         (0)    34178 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/github/util.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/github/webhook.py
+-rw-r--r--   0 root         (0) root         (0)    15259 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/gitutil.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/gziputil.py
+-rw-r--r--   0 root         (0) root         (0)     6926 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/http_requests.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/ioutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.419205 gardener-cicd-libs-1.2117.0/mail/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/mail/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/mail/template_mailer.py
+-rw-r--r--   0 root         (0) root         (0)     9573 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/mailutil.py
+-rw-r--r--   0 root         (0) root         (0)      286 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/makoutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.419205 gardener-cicd-libs-1.2117.0/product/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/product/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/product/util.py
+-rw-r--r--   0 root         (0) root         (0)    22350 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/product/v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.423205 gardener-cicd-libs-1.2117.0/release_notes/
+-rw-r--r--   0 root         (0) root         (0)      913 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13285 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/release_notes/fetch.py
+-rw-r--r--   0 root         (0) root         (0)     5613 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/release_notes/markdown.py
+-rw-r--r--   0 root         (0) root         (0)    11411 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/release_notes/model.py
+-rw-r--r--   0 root         (0) root         (0)     7739 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/release_notes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/reutil.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-07-27 06:35:42.427205 gardener-cicd-libs-1.2117.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.423205 gardener-cicd-libs-1.2117.0/slackclient/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/slackclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/slackclient/util.py
+-rw-r--r--   0 root         (0) root         (0)     6591 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/tarutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.423205 gardener-cicd-libs-1.2117.0/test/
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.423205 gardener-cicd-libs-1.2117.0/test/concourse/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/client_test.py
+-rw-r--r--   0 root         (0) root         (0)     4760 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/factory_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.423205 gardener-cicd-libs-1.2117.0/test/concourse/model/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6657 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/model/job_test.py
+-rw-r--r--   0 root         (0) root         (0)     3272 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/model/resources_test.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/model/step_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.423205 gardener-cicd-libs-1.2117.0/test/concourse/model/traits/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/model/traits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/model/traits/component_descriptor_test.py
+-rw-r--r--   0 root         (0) root         (0)     7482 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/model/traits/filter_test.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/model/traits/slack_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.423205 gardener-cicd-libs-1.2117.0/test/concourse/resources/
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/resources/github_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.427205 gardener-cicd-libs-1.2117.0/test/concourse/steps/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/steps/component_descriptor_test.py
+-rw-r--r--   0 root         (0) root         (0)     6544 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/steps/notification_test.py
+-rw-r--r--   0 root         (0) root         (0)     8060 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/steps/release_test.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/steps/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/steps/update_component_deps_test.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/steps/version_test.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/concourse/util_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.427205 gardener-cicd-libs-1.2117.0/test/container/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/container/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.427205 gardener-cicd-libs-1.2117.0/test/github/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6142 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/github/github_util_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.427205 gardener-cicd-libs-1.2117.0/test/product_/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/product_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/reutil_test.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/test/version_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:35:42.427205 gardener-cicd-libs-1.2117.0/unixutil/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/unixutil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/unixutil/model.py
+-rw-r--r--   0 root         (0) root         (0)     3717 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/unixutil/scan.py
+-rw-r--r--   0 root         (0) root         (0)    15220 2023-07-27 06:32:58.000000 gardener-cicd-libs-1.2117.0/version.py
```

### Comparing `gardener-cicd-libs-1.2116.0/LICENSE.md` & `gardener-cicd-libs-1.2117.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/README.md` & `gardener-cicd-libs-1.2117.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ccc/__init__.py` & `gardener-cicd-libs-1.2117.0/ccc/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ccc/alicloud.py` & `gardener-cicd-libs-1.2117.0/ccc/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ccc/aws.py` & `gardener-cicd-libs-1.2117.0/ccc/aws.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ccc/clamav.py` & `gardener-cicd-libs-1.2117.0/ccc/clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ccc/concourse.py` & `gardener-cicd-libs-1.2117.0/ccc/concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ccc/delivery.py` & `gardener-cicd-libs-1.2117.0/ccc/delivery.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ccc/elasticsearch.py` & `gardener-cicd-libs-1.2117.0/ccc/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ccc/gcp.py` & `gardener-cicd-libs-1.2117.0/ccc/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ccc/github.py` & `gardener-cicd-libs-1.2117.0/ccc/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ccc/grafeas_model.py` & `gardener-cicd-libs-1.2117.0/ccc/grafeas_model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ccc/oci.py` & `gardener-cicd-libs-1.2117.0/ccc/oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ccc/protecode.py` & `gardener-cicd-libs-1.2117.0/ccc/protecode.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ccc/secrets_server.py` & `gardener-cicd-libs-1.2117.0/ccc/secrets_server.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cfg_mgmt/alicloud.py` & `gardener-cicd-libs-1.2117.0/cfg_mgmt/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cfg_mgmt/aws.py` & `gardener-cicd-libs-1.2117.0/cfg_mgmt/aws.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cfg_mgmt/azure.py` & `gardener-cicd-libs-1.2117.0/cfg_mgmt/azure.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cfg_mgmt/btp_application_certificate.py` & `gardener-cicd-libs-1.2117.0/cfg_mgmt/btp_application_certificate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cfg_mgmt/btp_service_binding.py` & `gardener-cicd-libs-1.2117.0/cfg_mgmt/btp_service_binding.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cfg_mgmt/gcp.py` & `gardener-cicd-libs-1.2117.0/cfg_mgmt/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cfg_mgmt/github.py` & `gardener-cicd-libs-1.2117.0/cfg_mgmt/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cfg_mgmt/kubernetes.py` & `gardener-cicd-libs-1.2117.0/cfg_mgmt/kubernetes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cfg_mgmt/metrics.py` & `gardener-cicd-libs-1.2117.0/cfg_mgmt/metrics.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cfg_mgmt/model.py` & `gardener-cicd-libs-1.2117.0/cfg_mgmt/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cfg_mgmt/reporting.py` & `gardener-cicd-libs-1.2117.0/cfg_mgmt/reporting.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cfg_mgmt/rotate.py` & `gardener-cicd-libs-1.2117.0/cfg_mgmt/rotate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cfg_mgmt/util.py` & `gardener-cicd-libs-1.2117.0/cfg_mgmt/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cli.py` & `gardener-cicd-libs-1.2117.0/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,31 +20,32 @@
 import functools
 import inspect
 import itertools
 import os
 import pkgutil
 import sys
 
-import ci.log
-# to overwrite cli.py log level, call
-# "configure_default_logging(force=True, stdout_level=logging.DEBUG)" in specific module cli
-ci.log.configure_default_logging(force=True)
-
 try:
     import ci.util
 except ModuleNotFoundError:
     repo_dir = os.path.abspath(
         os.path.join(
             os.path.dirname(__name__),
             os.pardir,
             os.pardir,
         )
     )
     sys.path.insert(1, repo_dir)
     import ci.util
+
+import ci.log
+# to overwrite cli.py log level, call
+# "configure_default_logging(force=True, stdout_level=logging.DEBUG)" in specific module cli
+ci.log.configure_default_logging(force=True)
+
 import ctx  # noqa: E402
 
 import_errs = []
 
 
 def print_import_errs():
     for ie in import_errs:
```

### Comparing `gardener-cicd-libs-1.2116.0/cnudie/access.py` & `gardener-cicd-libs-1.2117.0/cnudie/access.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cnudie/iter.py` & `gardener-cicd-libs-1.2117.0/cnudie/iter.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cnudie/purge.py` & `gardener-cicd-libs-1.2117.0/cnudie/purge.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cnudie/replicate.py` & `gardener-cicd-libs-1.2117.0/cnudie/replicate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cnudie/retrieve.py` & `gardener-cicd-libs-1.2117.0/cnudie/retrieve.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cnudie/util.py` & `gardener-cicd-libs-1.2117.0/cnudie/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cnudie/validate.py` & `gardener-cicd-libs-1.2117.0/cnudie/validate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/__init__.py` & `gardener-cicd-libs-1.2117.0/concourse/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/client/__init__.py` & `gardener-cicd-libs-1.2117.0/concourse/client/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/client/api.py` & `gardener-cicd-libs-1.2117.0/concourse/client/api.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/client/model.py` & `gardener-cicd-libs-1.2117.0/concourse/client/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/client/routes.py` & `gardener-cicd-libs-1.2117.0/concourse/client/routes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/client/util.py` & `gardener-cicd-libs-1.2117.0/concourse/client/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/enumerator.py` & `gardener-cicd-libs-1.2117.0/concourse/enumerator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/factory.py` & `gardener-cicd-libs-1.2117.0/concourse/factory.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/__init__.py` & `gardener-cicd-libs-1.2117.0/concourse/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/base.py` & `gardener-cicd-libs-1.2117.0/concourse/model/base.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/job.py` & `gardener-cicd-libs-1.2117.0/concourse/model/job.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/pipeline.py` & `gardener-cicd-libs-1.2117.0/concourse/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/resources.py` & `gardener-cicd-libs-1.2117.0/concourse/model/resources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/step.py` & `gardener-cicd-libs-1.2117.0/concourse/model/step.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/__init__.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/component_descriptor.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/component_descriptor.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/cronjob.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/cronjob.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/draft_release.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/draft_release.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,32 +23,21 @@
   ScriptType,
   Trait,
   TraitTransformer,
 )
 from concourse.model.job import (
   JobVariant,
 )
-from concourse.model.traits.release import (
-    ReleaseNotesHandling,
-)
 
 ATTRIBUTES = (
     AttributeSpec.optional(
         name='preprocess',
         default='finalize',
         doc='version processing operation to set effective version',
     ),
-    AttributeSpec.optional(
-        name='release_notes_handling',
-        default=ReleaseNotesHandling.PREVIEW.value,
-        doc='''
-        configures which iteration of the code to use when generating release notes.
-        ''',
-        type=ReleaseNotesHandling,
-    ),
 )
 
 
 class DraftReleaseTrait(Trait):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -58,17 +47,14 @@
     @classmethod
     def _attribute_specs(cls):
         return ATTRIBUTES
 
     def _preprocess(self):
         return self.raw['preprocess']
 
-    def release_notes_handling(self) -> ReleaseNotesHandling:
-        return ReleaseNotesHandling(self.raw['release_notes_handling'])
-
     def validate(self):
         super().validate()
         if self._preprocess() != 'finalize':
             raise ModelValidationError(
                 "Only 'finalize' is supported as value for 'preprocess' in draft_release trait"
             )
```

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/filter.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/filter.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/image_scan.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/image_scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/images.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/meta.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/meta.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/notifications.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/notifications.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/options.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/options.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/publish.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/publish.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/pullrequest.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/pullrequest.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/release.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/release.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,35 +82,14 @@
 
     TAG_ONLY = EnumValueWithDocumentation(
         value='tag_only',
         doc='publish release tag to dead-end',
     )
 
 
-class ReleaseNotesHandling(EnumWithDocumentation):
-    DEFAULT = EnumValueWithDocumentation(
-        value='default',
-        doc='''
-        Use default version of release note creation code. Use this if you are interested in
-        stability rather than the latest features.
-        ''',
-    )
-    PREVIEW = EnumValueWithDocumentation(
-        value='preview',
-        doc='''
-            Use preview version of release note creation code. Use this to join new features and
-            feature-rollouts.
-
-            .. note::
-                if no features are being tested/rolled-out, using this value is the same as using
-                `default`.
-        '''
-    )
-
-
 ATTRIBUTES = (
     AttributeSpec.optional(
         name='nextversion',
         default=NextVersion.BUMP_MINOR.value,
         doc='specifies how the next development version is to be calculated',
         type=NextVersion,
     ),
@@ -203,22 +182,14 @@
         default=True,
         doc='''
         if true, a github release is published.
         ''',
         type=bool
     ),
     AttributeSpec.optional(
-        name='release_notes_handling',
-        default=ReleaseNotesHandling.PREVIEW.value,
-        doc='''
-        configures which iteration of the code to use when generating release notes.
-        ''',
-        type=ReleaseNotesHandling,
-    ),
-    AttributeSpec.optional(
         name='increment_version_on_tag_collision',
         default=False,
         doc='''
         If `True`, the pipeline will automatically increment the version _once_ if the tag
         corresponding to the desired version already exists.
         This incrementation follows the semantics set by the `nextversion` attribute.
         ''',
@@ -278,17 +249,14 @@
         if tags := self.raw.get('git_tags'):
             return tags[0]
         return None
 
     def release_on_github(self) -> bool:
         return self.raw['release_on_github']
 
-    def release_notes_handling(self) -> ReleaseNotesHandling:
-        return ReleaseNotesHandling(self.raw['release_notes_handling'])
-
     def validate(self):
         super().validate()
         if self.nextversion() == version.NOOP and self.next_version_callback_path():
             raise ModelValidationError(
                 f'not possible to configure "next_version_callback" if version is "{version.NOOP}"'
             )
         if not self.github_release_tag():
```

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/scan_sources.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/scan_sources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/scheduling.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/scheduling.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/slack.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/slack.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/update_component_deps.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/update_component_deps.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,14 @@
     ScriptType,
     Trait,
     TraitTransformer,
 )
 from concourse.model.job import (
     JobVariant,
 )
-from concourse.model.traits.release import (
-    ReleaseNotesHandling,
-)
 from model.base import ModelValidationError
 
 import concourse.model.traits.component_descriptor
 import concourse.model.traits.images
 
 OciImageCfg = concourse.model.traits.images.OciImageCfg
 
@@ -164,22 +161,14 @@
     ),
     AttributeSpec.optional(
         name='vars',
         default={},
         doc='env vars to pass to after_merge_callback (similar to step\'s vars)',
         type=dict,
     ),
-    AttributeSpec.optional(
-        name='release_notes_handling',
-        default=ReleaseNotesHandling.PREVIEW.value,
-        doc='''
-        configures which iteration of the code to use when generating release notes.
-        ''',
-        type=ReleaseNotesHandling,
-    ),
 )
 
 
 class UpdateComponentDependenciesTrait(Trait):
     @classmethod
     def _attribute_specs(cls):
         return ATTRIBUTES
@@ -230,17 +219,14 @@
 
     def after_merge_callback(self):
         return self.raw.get('after_merge_callback')
 
     def ignore_prerelease_versions(self):
         return self.raw.get('ignore_prerelease_versions')
 
-    def release_notes_handling(self) -> ReleaseNotesHandling:
-        return ReleaseNotesHandling(self.raw['release_notes_handling'])
-
     def vars(self):
         return self.raw['vars']
 
     def transformer(self):
         return UpdateComponentDependenciesTraitTransformer(trait=self)
 
     def validate(self):
```

### Comparing `gardener-cicd-libs-1.2116.0/concourse/model/traits/version.py` & `gardener-cicd-libs-1.2117.0/concourse/model/traits/version.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/replicator.py` & `gardener-cicd-libs-1.2117.0/concourse/replicator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/resources/defaults.mako` & `gardener-cicd-libs-1.2117.0/concourse/resources/defaults.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/resources/email.mako` & `gardener-cicd-libs-1.2117.0/concourse/resources/email.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/resources/github.mako` & `gardener-cicd-libs-1.2117.0/concourse/resources/github.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/resources/resource_types.mako` & `gardener-cicd-libs-1.2117.0/concourse/resources/resource_types.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/resources/variants.mako` & `gardener-cicd-libs-1.2117.0/concourse/resources/variants.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/__init__.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/alter_container_images.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/alter_container_images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/build_oci_image.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/build_oci_image.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/build_oci_image.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/build_oci_image.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/cfg_reporting.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/cfg_reporting.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/cfg_reporting.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/cfg_reporting.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/component_descriptor.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/component_descriptor.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/component_descriptor.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/component_descriptor.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/component_descriptor_util.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/component_descriptor_util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/draft_release.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/draft_release.mako`

 * *Files 22% similar despite different names*

```diff
@@ -14,32 +14,28 @@
 component_descriptor_trait = job_variant.trait('component_descriptor')
 component_name = component_descriptor_trait.component_name()
 version_operation = draft_release_trait._preprocess()
 component_descriptor_path = os.path.join(
     job_step.input('component_descriptor_dir'),
     cdu.component_descriptor_fname(gci.componentmodel.SchemaVersion.V2),
 )
-release_notes_handling=draft_release_trait.release_notes_handling().value
 %>
 import version
 import os
 
 import ccc.github
 import ci.util
 import cnudie.util
 import gci.componentmodel as cm
 import release_notes.fetch
 import release_notes.markdown
 
-from concourse.model.traits.release import ReleaseNotesHandling
 from gitutil import GitHelper
 from github.release_notes.util import (
     draft_release_name_for_version,
-    ReleaseNotes,
-    github_repo_path,
 )
 from github.util import (
     GitHubRepositoryHelper,
     GitHubRepoBranch,
 )
 
 if '${version_operation}' != 'finalize':
@@ -83,37 +79,21 @@
     repo_name='${repo.repo_name()}',
     branch='${repo.branch()}',
 )
 
 github_helper = GitHubRepositoryHelper.from_githubrepobranch(
     githubrepobranch=githubrepobranch,
 )
-
-release_notes_handling = ReleaseNotesHandling(
-    '${release_notes_handling}'
-)
-
-if release_notes_handling is ReleaseNotesHandling.DEFAULT:
-    release_notes = ReleaseNotes(
-        component=component,
-        repo_dir=repo_dir,
-    )
-    release_notes.create(
-        start_ref='${repo.branch()}'
-    )
-    release_notes_md = release_notes.to_markdown()
-
-elif release_notes_handling is ReleaseNotesHandling.PREVIEW:
-    release_note_blocks = release_notes.fetch.fetch_release_notes(
-        repo_path=repo_dir,
-        component=component,
-    )
-    release_notes_md = '\n'.join(
-        str(i) for i in release_notes.markdown.render(release_note_blocks)
-    ) or 'no release notes available'
+release_note_blocks = release_notes.fetch.fetch_release_notes(
+    repo_path=repo_dir,
+    component=component,
+)
+release_notes_md = '\n'.join(
+    str(i) for i in release_notes.markdown.render(release_note_blocks)
+) or 'no release notes available'
 
 draft_name = draft_release_name_for_version(processed_version)
 draft_release = github_helper.draft_release_with_name(draft_name)
 if not draft_release:
     github_helper.create_draft_release(
         name=draft_name,
         body=release_notes_md,
```

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/images.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/malware_scan.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/malware_scan.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/meta.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/meta.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/meta.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/meta.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/notification.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/notification.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/notification.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/notification.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/os_id.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/os_id.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/os_id.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/os_id.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/prepare.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/prepare.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/publish.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/publish.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/release.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/release.mako`

 * *Files 5% similar despite different names*

```diff
@@ -110,10 +110,9 @@
   release_commit_message_prefix='${release_commit_message_prefix}',
   % endif
   % if next_cycle_commit_message_prefix:
   next_cycle_commit_message_prefix='${next_cycle_commit_message_prefix}',
   % endif
   github_release_tag=${github_release_tag},
   git_tags=${git_tags},
-  release_notes_handling='${release_trait.release_notes_handling().value}',
 )
 </%def>
```

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/release.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,18 @@
 from gitutil import GitHelper
 from github.util import (
     GitHubRepositoryHelper,
     GitHubRepoBranch,
 )
 import product.v2
 from github.release_notes.util import (
-    fetch_release_notes,
     post_to_slack,
 )
 from concourse.model.traits.release import (
     ReleaseCommitPublishingPolicy,
-    ReleaseNotesHandling,
     ReleaseNotesPolicy,
 )
 import model.container_registry as cr
 import oci.model
 
 logger = logging.getLogger('step.release')
 
@@ -632,56 +630,14 @@
             except ConnectionError:
                 logger.warning('Unable to attach component-descriptors to release as release-asset.')
 
         if self.release_on_github:
             upload_component_descriptor_as_release_asset()
 
 
-class PublishReleaseNotesStep(TransactionalStep):
-    def name(self):
-        return "Publish Release Notes"
-
-    def __init__(
-        self,
-        githubrepobranch: GitHubRepoBranch,
-        github_helper: GitHubRepositoryHelper,
-        component: cm.Component,
-        release_version: str,
-        repo_dir: str,
-    ):
-        self.githubrepobranch = not_none(githubrepobranch)
-        self.github_helper = not_none(github_helper)
-        self.component = component
-        self.release_version = release_version
-        self.repo_dir = os.path.abspath(not_empty(repo_dir))
-
-    def validate(self):
-        pass
-
-    def apply(self):
-        create_release_step_output = self.context().step_output('Create Release')
-        release_tag = create_release_step_output['release_tag_name']
-
-        release_notes = fetch_release_notes(
-            self.component,
-            repo_dir=self.repo_dir,
-            repository_branch=self.githubrepobranch.branch(),
-        )
-        release_notes_md = release_notes.to_markdown(force_link_generation=True)
-        self.github_helper.update_release_notes(
-            tag_name=release_tag,
-            body=release_notes_md,
-            component_name=self.component.name,
-        )
-        return {
-            'release notes': release_notes,
-            'release notes markdown': release_notes_md,
-        }
-
-
 class TryCleanupDraftReleasesStep(TransactionalStep):
     def name(self):
         return "Try to Cleanup Draft Releases"
 
     def __init__(
         self,
         github_helper: GitHubRepositoryHelper,
@@ -870,15 +826,14 @@
     release_notes_policy: str,
     release_version: str,
     repo_dir: str,
     repository_version_file_path: str,
     git_tags: list,
     github_release_tag: dict,
     release_commit_callback_image_reference: str,
-    release_notes_handling: str,
     component_descriptor_path: str=None,
     next_cycle_commit_message_prefix: str=None,
     next_version_callback: str=None,
     increment_on_tag_collision: bool=False,
     prerelease_suffix: str="dev",
     rebase_before_release: bool=False,
     release_on_github: bool=True,
@@ -909,15 +864,14 @@
 
     transaction_ctx = TransactionContext() # shared between all steps/trxs
 
     release_notes_policy = ReleaseNotesPolicy(release_notes_policy)
     release_commit_publishing_policy = ReleaseCommitPublishingPolicy(
         release_commit_publishing_policy
     )
-    release_notes_handling = ReleaseNotesHandling(release_notes_handling)
     github_helper = GitHubRepositoryHelper.from_githubrepobranch(githubrepobranch)
     git_helper = GitHelper.from_githubrepobranch(
         githubrepobranch=githubrepobranch,
         repo_path=repo_dir,
     )
 
     # make sure that desired tag(s) do not already exist. If configured to do so, increment
@@ -1033,67 +987,32 @@
         return logger.info('release notes were disabled - skipping')
     elif release_notes_policy == ReleaseNotesPolicy.DEFAULT:
         pass
     else:
         raise NotImplementedError(release_notes_policy)
 
     if release_on_github:
-        if release_notes_handling is ReleaseNotesHandling.DEFAULT:
-            publish_release_notes_step = PublishReleaseNotesStep(
-                githubrepobranch=githubrepobranch,
-                github_helper=github_helper,
-                component=component,
-                release_version=release_version,
-                repo_dir=repo_dir,
-            )
-            release_notes_transaction = Transaction(
-                ctx=transaction_ctx,
-                steps=(publish_release_notes_step,),
-            )
-            release_notes_transaction.validate()
-            if not release_notes_transaction.execute():
-                raise RuntimeError('An error occurred while publishing the release notes.')
-        elif release_notes_handling is ReleaseNotesHandling.PREVIEW:
-            release_note_blocks = release_notes.fetch.fetch_release_notes(
-                repo_path=repo_dir,
-                component=component,
-                current_version=version.parse_to_semver(release_version),
-            )
-            release_notes_markdown = '\n'.join(
-                str(i) for i in release_notes.markdown.render(release_note_blocks)
-            ) or 'no release notes available'
-            github_helper.update_release_notes(
-                tag_name=release_version,
-                body=release_notes_markdown,
-                component_name=component.name,
-            )
-        else:
-            raise NotImplementedError(release_notes_handling)
+        release_note_blocks = release_notes.fetch.fetch_release_notes(
+            repo_path=repo_dir,
+            component=component,
+            current_version=version.parse_to_semver(release_version),
+        )
+        release_notes_markdown = '\n'.join(
+            str(i) for i in release_notes.markdown.render(release_note_blocks)
+        ) or 'no release notes available'
+        github_helper.update_release_notes(
+            tag_name=release_version,
+            body=release_notes_markdown,
+            component_name=component.name,
+        )
 
     if slack_channel_configs:
         if not release_on_github:
             raise RuntimeError('Cannot post to slack without a github release')
 
-        if release_notes_handling is ReleaseNotesHandling.DEFAULT:
-            release_notes_raw = transaction_ctx.step_output(
-                publish_release_notes_step.name()
-            ).get('release notes')
-            # slack can't auto link pull requests, commits or users
-            # hence we force the link generation when building the markdown string
-            logger.info('Creating release-note markdown before posting to Slack')
-            release_notes_markdown = release_notes_raw.to_markdown(
-                force_link_generation=True
-            )
-        elif release_notes_handling is ReleaseNotesHandling.PREVIEW:
-            # release_notes_markdown already prepared earlier albeit without special link
-            # preparation for Slack.
-            pass
-        else:
-            raise NotImplementedError(release_notes_handling)
-
         all_slack_releases_successful = True
         for slack_cfg in slack_channel_configs:
             slack_cfg_name = slack_cfg['slack_cfg_name']
             slack_channel = slack_cfg['channel_name']
             post_to_slack_step = PostSlackReleaseStep(
                 slack_cfg_name=slack_cfg_name,
                 slack_channel=slack_channel,
```

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/replicate_pipelines.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/replicate_pipelines.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/replicate_pipelines.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/replicate_pipelines.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/replicate_secrets.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/replicate_secrets.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/replicate_secrets.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/replicate_secrets.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/rm_pr_label.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/rm_pr_label.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/scan_container_images.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/scan_container_images.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/scan_container_images.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/scan_container_images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/scan_sources.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/scan_sources.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/scan_sources.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/scan_sources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/update_component_deps.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/update_component_deps.mako`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 repo_branch = main_repo.branch()
 
 update_component_deps_trait = job_variant.trait('update_component_deps')
 set_dependency_version_script_path = update_component_deps_trait.set_dependency_version_script_path()
 after_merge_callback = update_component_deps_trait.after_merge_callback()
 upstream_update_policy = update_component_deps_trait.upstream_update_policy()
 ignore_prerelease_versions=update_component_deps_trait.ignore_prerelease_versions()
-release_notes_handling=update_component_deps_trait.release_notes_handling()
 component_descriptor_trait = job_variant.trait('component_descriptor')
 ctx_repo = component_descriptor_trait.ctx_repository()
 
 set_version_script_image_cfg = \
     update_component_deps_trait.set_dependency_version_script_container_image()
 if set_version_script_image_cfg:
     set_version_script_image = set_version_script_image_cfg.image_reference()
@@ -93,17 +92,14 @@
 ]
 merge_policy_and_filters = {
     p: component_ref_component_name_filter(
         include_regexes=p.component_names(),
         exclude_regexes=(),
     ) for p in merge_policy_configs
 }
-release_notes_handling = concourse.model.traits.release.ReleaseNotesHandling(
-    '${release_notes_handling.value}'
-)
 # indicates whether or not an upstream component was defined as a reference
 upstream_component_name = os.environ.get('UPSTREAM_COMPONENT_NAME', None)
 UPGRADE_TO_UPSTREAM = bool(upstream_component_name)
 
 logger.info(f'{UPGRADE_TO_UPSTREAM=}')
 
 pull_request_util = github.util.PullRequestUtil(
@@ -197,15 +193,14 @@
         after_merge_callback='${after_merge_callback}',
 % endif
 % if set_version_script_image:
         container_image='${set_version_script_image}',
 % else:
         container_image = None,
 % endif
-        release_notes_handling=release_notes_handling,
     )
     # add pr to the list of known upgrade pull requests, so next iteration
     # on the generator returned by determine_upgrade_prs takes it into
     # consideration
     upgrade_pull_requests.append(pull_request)
 
 for upgrade_pull_request in github.util.iter_obsolete_upgrade_pull_requests(
```

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/update_component_deps.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/update_component_deps.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,25 +20,21 @@
 import dockerutil
 import github.util
 import gitutil
 import model.container_registry as cr
 import product.v2
 import release_notes.fetch as release_notes_fetch
 import version
-from concourse.model.traits.release import (
-    ReleaseNotesHandling,
-)
 from concourse.model.traits.update_component_deps import (
     MergePolicy,
     MergeMethod,
 )
 from github.util import (
     GitHubRepoBranch,
 )
-from github.release_notes.util import ReleaseNotes
 
 logger = logging.getLogger('step.update_component_deps')
 
 
 UpstreamUpdatePolicy = concourse.model.traits.update_component_deps.UpstreamUpdatePolicy
 
 
@@ -263,15 +259,14 @@
                 yield(greatest_component_reference, candidate_version)
 
 
 def _import_release_notes(
     component: gci.componentmodel.Component,
     to_version: str,
     pull_request_util,
-    release_notes_handling: ReleaseNotesHandling = ReleaseNotesHandling.DEFAULT,
 ):
     if not component.sources:
         logger.warning(
             f'''
             {component.name=}:{component.version=} has no sources; skipping release-notes-import
             '''
         )
@@ -284,15 +279,14 @@
 
     release_notes = create_release_notes(
         from_component=component,
         from_github_cfg=github_cfg,
         from_repo_owner=org_name,
         from_repo_name=repository_name,
         to_version=to_version,
-        release_notes_handling=release_notes_handling,
     )
 
     if not release_notes:
         release_notes = pull_request_util.retrieve_pr_template_text()
 
     return release_notes
 
@@ -309,15 +303,14 @@
     repo_dir,
     github_cfg_name,
     ctx_repo: gci.componentmodel.OciRepositoryContext,
     merge_policy: MergePolicy,
     merge_method: MergeMethod,
     after_merge_callback=None,
     container_image:str=None,
-    release_notes_handling: ReleaseNotesHandling=ReleaseNotesHandling.DEFAULT,
 ) -> github.util.UpgradePullRequest:
     if container_image:
         dockerutil.launch_dockerd_if_not_running()
 
     ls_repo = pull_request_util.repository
 
     from_component_descriptor = component_descriptor_lookup()(
@@ -402,15 +395,14 @@
     )
     # branch was created. Cleanup if something fails
     try:
         release_notes = _import_release_notes(
             component=from_component,
             to_version=to_version,
             pull_request_util=pull_request_util,
-            release_notes_handling=release_notes_handling,
         )
     except Exception:
         logger.warning('failed to retrieve release-notes')
         traceback.print_exc()
         release_notes = 'failed to retrieve release-notes'
 
     if release_notes:
@@ -515,52 +507,30 @@
 
 def create_release_notes(
     from_component: gci.componentmodel.Component,
     from_github_cfg,
     from_repo_owner: str,
     from_repo_name: str,
     to_version: str,
-    release_notes_handling: ReleaseNotesHandling = ReleaseNotesHandling.DEFAULT,
 ):
     from_version = from_component.version
     try:
         with tempfile.TemporaryDirectory() as temp_dir:
             gitutil.GitHelper.clone_into(
                 target_directory=temp_dir,
                 github_cfg=from_github_cfg,
                 github_repo_path=f'{from_repo_owner}/{from_repo_name}'
             )
-            if release_notes_handling is ReleaseNotesHandling.DEFAULT:
-                commit_range = '{from_version}..{to_version}'.format(
-                    from_version=from_version,
-                    to_version=to_version,
-                )
-                release_notes = ReleaseNotes(
-                    component=from_component,
-                    repo_dir=temp_dir,
-                )
-                release_notes.create(
-                    start_ref=None, # the repo's default branch
-                    commit_range=commit_range
-                )
-                release_note_blocks = release_notes.release_note_blocks()
-                if release_note_blocks:
-                    return f'**Release Notes**:\n{release_note_blocks}'
-
-            elif release_notes_handling is ReleaseNotesHandling.PREVIEW:
-                release_note_blocks = release_notes_fetch.fetch_release_notes(
-                    repo_path=temp_dir,
-                    component=from_component,
-                    current_version=version.parse_to_semver(to_version),
-                    previous_version=version.parse_to_semver(from_version),
-                )
-                if release_note_blocks:
-                    n = '\n'
-                    return f'**Release Notes**:\n{n.join(r.block_str for r in release_note_blocks)}'
-
-            else:
-                raise NotImplementedError(release_notes_handling)
+            release_note_blocks = release_notes_fetch.fetch_release_notes(
+                repo_path=temp_dir,
+                component=from_component,
+                current_version=version.parse_to_semver(to_version),
+                previous_version=version.parse_to_semver(from_version),
+            )
+            if release_note_blocks:
+                n = '\n'
+                return f'**Release Notes**:\n{n.join(r.block_str for r in release_note_blocks)}'
 
     except:
         logger.warning('an error occurred during release notes processing (ignoring)')
         import traceback
         logger.warning(traceback.format_exc())
```

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/version.mako` & `gardener-cicd-libs-1.2117.0/concourse/steps/version.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/steps/version.py` & `gardener-cicd-libs-1.2117.0/concourse/steps/version.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/templates/__init__.py` & `gardener-cicd-libs-1.2117.0/concourse/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/templates/default.mako` & `gardener-cicd-libs-1.2117.0/concourse/templates/default.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/util.py` & `gardener-cicd-libs-1.2117.0/concourse/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/concourse/validator.py` & `gardener-cicd-libs-1.2117.0/concourse/validator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/container/__init__.py` & `gardener-cicd-libs-1.2117.0/container/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/container/util.py` & `gardener-cicd-libs-1.2117.0/container/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cosign/__init__.py` & `gardener-cicd-libs-1.2117.0/cosign/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/cosign/payload.py` & `gardener-cicd-libs-1.2117.0/cosign/payload.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/cosign.py` & `gardener-cicd-libs-1.2117.0/ctt/cosign.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/filters.py` & `gardener-cicd-libs-1.2117.0/ctt/filters.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/platform.py` & `gardener-cicd-libs-1.2117.0/ctt/platform.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/process_dependencies.py` & `gardener-cicd-libs-1.2117.0/ctt/process_dependencies.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/processing_model.py` & `gardener-cicd-libs-1.2117.0/ctt/processing_model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/processors.py` & `gardener-cicd-libs-1.2117.0/ctt/processors.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/rbsc_bom.py` & `gardener-cicd-libs-1.2117.0/ctt/rbsc_bom.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/test/filters_test.py` & `gardener-cicd-libs-1.2117.0/ctt/test/filters_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/test/platform_test.py` & `gardener-cicd-libs-1.2117.0/ctt/test/platform_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/test/process_deps_test.py` & `gardener-cicd-libs-1.2117.0/ctt/test/process_deps_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/test/processors_test.py` & `gardener-cicd-libs-1.2117.0/ctt/test/processors_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/test/uploaders_test.py` & `gardener-cicd-libs-1.2117.0/ctt/test/uploaders_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/uploaders.py` & `gardener-cicd-libs-1.2117.0/ctt/uploaders.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/ctt/util.py` & `gardener-cicd-libs-1.2117.0/ctt/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/delivery/client.py` & `gardener-cicd-libs-1.2117.0/delivery/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/delivery/model.py` & `gardener-cicd-libs-1.2117.0/delivery/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/delivery/util.py` & `gardener-cicd-libs-1.2117.0/delivery/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/dockerutil.py` & `gardener-cicd-libs-1.2117.0/dockerutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/dso/cvss.py` & `gardener-cicd-libs-1.2117.0/dso/cvss.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/dso/labels.py` & `gardener-cicd-libs-1.2117.0/dso/labels.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/dso/model.py` & `gardener-cicd-libs-1.2117.0/dso/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/gardener_cicd_libs.egg-info/SOURCES.txt` & `gardener-cicd-libs-1.2117.0/gardener_cicd_libs.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -173,18 +173,14 @@
 github/util.py
 github/webhook.py
 github/compliance/__init__.py
 github/compliance/issue.py
 github/compliance/milestone.py
 github/compliance/model.py
 github/compliance/report.py
-github/release_notes/__init__.py
-github/release_notes/model.py
-github/release_notes/renderer.py
-github/release_notes/util.py
 mail/__init__.py
 mail/template_mailer.py
 product/__init__.py
 product/util.py
 product/v2.py
 release_notes/__init__.py
 release_notes/fetch.py
@@ -217,15 +213,11 @@
 test/concourse/steps/release_test.py
 test/concourse/steps/test_utils.py
 test/concourse/steps/update_component_deps_test.py
 test/concourse/steps/version_test.py
 test/container/__init__.py
 test/github/__init__.py
 test/github/github_util_test.py
-test/github/release_notes/__init__.py
-test/github/release_notes/default_util.py
-test/github/release_notes/renderer_test.py
-test/github/release_notes/util_test.py
 test/product_/__init__.py
 unixutil/__init__.py
 unixutil/model.py
 unixutil/scan.py
```

### Comparing `gardener-cicd-libs-1.2116.0/gardener_cicd_libs.egg-info/requires.txt` & `gardener-cicd-libs-1.2117.0/gardener_cicd_libs.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-gardener-cicd-base>=1.2116.0
-gardener-oci>=1.2116.0
+gardener-cicd-base>=1.2117.0
+gardener-oci>=1.2117.0
 GitPython
 Mako<2.0.0
 Sphinx
 aliyun-python-sdk-core==2.13.36
 aliyun-python-sdk-ecs==4.24.64
 aliyun-python-sdk-ram==3.3.0
 awesomeversion
@@ -27,15 +27,15 @@
 google-auth<3
 google-cloud-storage<3
 google-crc32c>1.1.4
 html2text
 kubernetes>=26.0.0
 msal<2
 openstacksdk
-oss2==2.18.0
+oss2==2.18.1
 passlib<2.0.0
 pycryptodome
 pydash<8.0.0
 pylama
 pylint
 pytest
 python-dateutil
```

### Comparing `gardener-cicd-libs-1.2116.0/github/__init__.py` & `gardener-cicd-libs-1.2117.0/github/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/github/codeowners.py` & `gardener-cicd-libs-1.2117.0/github/codeowners.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/github/compliance/issue.py` & `gardener-cicd-libs-1.2117.0/github/compliance/issue.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/github/compliance/milestone.py` & `gardener-cicd-libs-1.2117.0/github/compliance/milestone.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/github/compliance/model.py` & `gardener-cicd-libs-1.2117.0/github/compliance/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/github/compliance/report.py` & `gardener-cicd-libs-1.2117.0/github/compliance/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/github/release_notes/__init__.py` & `gardener-cicd-libs-1.2117.0/mail/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/github/retry.py` & `gardener-cicd-libs-1.2117.0/github/retry.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/github/user.py` & `gardener-cicd-libs-1.2117.0/github/user.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/github/util.py` & `gardener-cicd-libs-1.2117.0/github/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 import enum
 import io
 import re
 import sys
 
 import typing
 from typing import Iterable, Tuple
-from pydash import _
 
 import requests
 
 import github3
 import github3.issues
 from github3.exceptions import NotFoundError
 from github3.github import GitHub
@@ -714,32 +713,30 @@
             raise NotFoundError(resp=response)
 
         buffer = io.BytesIO()
         asset.download(buffer)
         return buffer.getvalue().decode()
 
     def release_versions(self):
-        for tag_name in self.release_tags():
+        for tag_name in self._release_tags():
             try:
                 version.parse_to_semver(tag_name)
                 yield tag_name
                 # XXX should rather return a "Version" object, containing both parsed and original
             except ValueError:
                 pass # ignore
 
-    def release_tags(self):
-        return _.chain(
-            self.repository.releases()
-        ).filter(
-            lambda release: not release.draft and not release.prerelease
-        ).map(
-            'tag_name'
-        ).filter(
-            lambda tag: tag is not None
-        ).value()
+    def _release_tags(self):
+        for release in self.repository.releases():
+            if release.draft or release.prerelease:
+                continue
+            if not (tag := release.tag_name):
+                continue
+
+            yield tag
 
     def search_issues_in_repo(self, query: str):
         query = f'repo:{self.owner}/{self.repository_name} {query}'
         search_result = self.github.search_issues(query)
         return search_result
 
     def is_pr_created_by_org_member(self, pull_request_number):
```

### Comparing `gardener-cicd-libs-1.2116.0/github/webhook.py` & `gardener-cicd-libs-1.2117.0/github/webhook.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/gitutil.py` & `gardener-cicd-libs-1.2117.0/gitutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/gziputil.py` & `gardener-cicd-libs-1.2117.0/gziputil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/http_requests.py` & `gardener-cicd-libs-1.2117.0/http_requests.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/mail/__init__.py` & `gardener-cicd-libs-1.2117.0/product/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/mail/template_mailer.py` & `gardener-cicd-libs-1.2117.0/mail/template_mailer.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/mailutil.py` & `gardener-cicd-libs-1.2117.0/mailutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/product/__init__.py` & `gardener-cicd-libs-1.2117.0/slackclient/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/product/util.py` & `gardener-cicd-libs-1.2117.0/product/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/product/v2.py` & `gardener-cicd-libs-1.2117.0/product/v2.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/release_notes/__init__.py` & `gardener-cicd-libs-1.2117.0/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/release_notes/fetch.py` & `gardener-cicd-libs-1.2117.0/release_notes/fetch.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/release_notes/markdown.py` & `gardener-cicd-libs-1.2117.0/release_notes/markdown.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/release_notes/model.py` & `gardener-cicd-libs-1.2117.0/release_notes/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/release_notes/utils.py` & `gardener-cicd-libs-1.2117.0/release_notes/utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/reutil.py` & `gardener-cicd-libs-1.2117.0/reutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/setup.py` & `gardener-cicd-libs-1.2117.0/setup.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/slackclient/__init__.py` & `gardener-cicd-libs-1.2117.0/test/concourse/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,7 +8,23 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+import sys
+import os
+
+# add modules from root dir to module search path
+# so unit test modules can use regular imports
+sys.path.extend(
+    (
+        os.path.join(
+            os.path.realpath(os.path.dirname(__file__)),
+            os.pardir,
+            os.pardir
+        ),
+        os.path.realpath(os.path.dirname(__file__))
+    )
+)
```

### Comparing `gardener-cicd-libs-1.2116.0/slackclient/util.py` & `gardener-cicd-libs-1.2117.0/slackclient/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/tarutil.py` & `gardener-cicd-libs-1.2117.0/tarutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/__init__.py` & `gardener-cicd-libs-1.2117.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/_test_utils.py` & `gardener-cicd-libs-1.2117.0/test/_test_utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/__init__.py` & `gardener-cicd-libs-1.2117.0/test/container/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/client_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/client_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/factory_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/factory_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/model/__init__.py` & `gardener-cicd-libs-1.2117.0/test/concourse/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/model/job_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/model/job_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/model/resources_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/model/resources_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/model/step_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/model/step_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/model/traits/__init__.py` & `gardener-cicd-libs-1.2117.0/test/concourse/model/traits/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/model/traits/component_descriptor_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/model/traits/component_descriptor_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/model/traits/filter_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/model/traits/filter_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/model/traits/slack_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/model/traits/slack_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/resources/__init__.py` & `gardener-cicd-libs-1.2117.0/test/concourse/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/resources/github_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/resources/github_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/steps/__init__.py` & `gardener-cicd-libs-1.2117.0/test/concourse/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/steps/component_descriptor_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/steps/component_descriptor_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/steps/notification_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/steps/notification_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/steps/release_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/steps/release_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -166,58 +166,14 @@
         examinee().validate()
 
     def test_validation_fails_on_invalid_semver(self, examinee):
         with pytest.raises(ValueError):
             examinee(release_version='invalid_semver').validate()
 
 
-class TestPublishReleaseNotesStep:
-    @pytest.fixture()
-    def examinee(self, tmp_path):
-        cd_v2 = cm.ComponentDescriptor(
-            component=cm.Component(
-                name='example.com/a_name',
-                version='1.2.3',
-                repositoryContexts=[],
-                provider={
-                    'name': 'some provider',
-                },
-                sources=[],
-                componentReferences=[],
-                resources=[],
-            ),
-            meta=cm.Metadata(),
-        )
-
-        def _examinee(
-            github_helper=MagicMock(),
-            githubrepobranch=GitHubRepoBranch(
-                github_config='test_config',
-                repo_owner='test_owner',
-                repo_name='test_name',
-                branch='master',
-            ),
-            repository_hostname="example.com",
-            repository_path="a_name",
-            repo_dir=str(tmp_path),
-            release_version='1.0.0',
-        ):
-            return concourse.steps.release.PublishReleaseNotesStep(
-                component=cd_v2.component,
-                github_helper=github_helper,
-                githubrepobranch=githubrepobranch,
-                repo_dir=repo_dir,
-                release_version=release_version,
-            )
-        return _examinee
-
-    def test_validation(self, examinee):
-        examinee().validate()
-
-
 class TestTryCleanupDraftReleaseStep:
     @pytest.fixture()
     def examinee(self):
         def _examinee(
             github_helper=MagicMock(),
         ):
             return concourse.steps.release.TryCleanupDraftReleasesStep(
```

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/steps/test_utils.py` & `gardener-cicd-libs-1.2117.0/test/concourse/steps/test_utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/steps/update_component_deps_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/steps/update_component_deps_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/steps/version_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/steps/version_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/concourse/util_test.py` & `gardener-cicd-libs-1.2117.0/test/concourse/util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/container/__init__.py` & `gardener-cicd-libs-1.2117.0/test/github/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/github/__init__.py` & `gardener-cicd-libs-1.2117.0/test/product_/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/github/github_util_test.py` & `gardener-cicd-libs-1.2117.0/test/github/github_util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/reutil_test.py` & `gardener-cicd-libs-1.2117.0/test/reutil_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/test/version_test.py` & `gardener-cicd-libs-1.2117.0/test/version_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/unixutil/model.py` & `gardener-cicd-libs-1.2117.0/unixutil/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/unixutil/scan.py` & `gardener-cicd-libs-1.2117.0/unixutil/scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2116.0/version.py` & `gardener-cicd-libs-1.2117.0/version.py`

 * *Files identical despite different names*

