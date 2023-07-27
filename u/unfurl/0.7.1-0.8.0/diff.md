# Comparing `tmp/unfurl-0.7.1.tar.gz` & `tmp/unfurl-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unfurl-0.7.1.tar", last modified: Tue Jun 13 00:06:29 2023, max compression
+gzip compressed data, was "unfurl-0.8.0.tar", last modified: Thu Jul 27 05:43:09 2023, max compression
```

## Comparing `unfurl-0.7.1.tar` & `unfurl-0.8.0.tar`

### file list

```diff
@@ -1,190 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.130778 unfurl-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 00:06:25.000000 unfurl-0.7.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      282 2023-06-13 00:06:25.000000 unfurl-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-06-13 00:06:29.130778 unfurl-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-06-13 00:06:26.000000 unfurl-0.7.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-06-13 00:06:29.130778 unfurl-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 00:06:26.000000 unfurl-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.118777 unfurl-0.7.1/unfurl/
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44262 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/changelog-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    50240 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/cloudmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    50040 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.118777 unfurl-0.7.1/unfurl/configurators/
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    17357 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/dns-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/docker-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/helm-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16659 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/kompose.py
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/supervisor-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20833 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/configurators/terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)    30685 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.118777 unfurl-0.7.1/unfurl/filter_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/filter_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/filter_plugins/ref.py
--rw-r--r--   0 runner    (1001) docker     (123)    45653 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    57945 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    56589 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/localenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/lookup_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/lookup_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/lookup_plugins/unfurl.py
--rw-r--r--   0 runner    (1001) docker     (123)    16094 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/manifest-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    30360 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    25719 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    17599 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    44296 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    45532 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/planrequests.py
--rw-r--r--   0 runner    (1001) docker     (123)    22039 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/projectpaths.py
--rw-r--r--   0 runner    (1001) docker     (123)    33741 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    43549 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    53433 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    61741 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/templates/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/aws/unfurl.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/dashboard/manifest.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/dashboard/unfurl.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/templates/digitalocean/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/digitalocean/unfurl.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/templates/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/gcp/unfurl.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/gitignore.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/templates/home/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/home/manifest-template.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/home/unfurl.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/templates/local/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/local/ensemble-examples.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/local-unfurl-template.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/manifest-template.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/manifest.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/templates/python3.10/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/python3.10/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    65571 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/python3.10/Pipfile.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/templates/python3.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/python3.11/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    61319 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/python3.11/Pipfile.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/templates/python3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/python3.7/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    67532 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/python3.7/Pipfile.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/templates/python3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/python3.8/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    67182 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/python3.8/Pipfile.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/templates/python3.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/python3.9/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    66663 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/python3.9/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/secrets.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/service-template.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/unfurl.local.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/templates/unfurl.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    74712 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/to_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    60896 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/tosca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/tosca_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/tosca_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/tosca_plugins/artifacts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/tosca_plugins/googlecloud.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/tosca_plugins/k8s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/tosca_plugins/localhost.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/tosca_plugins/tosca-ext.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/unfurl-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    23855 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.122777 unfurl-0.7.1/unfurl/vendor/sphinx-jsonschema/
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/sphinx-jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/sphinx-jsonschema/wide_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.126778 unfurl-0.7.1/unfurl/vendor/toscaparser/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.126778 unfurl-0.7.1/unfurl/vendor/toscaparser/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/dataentity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.126778 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/
--rw-r--r--   0 runner    (1001) docker     (123)    32477 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    33031 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/artifacttype.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/attribute_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/capabilitytype.py
--rw-r--r--   0 runner    (1001) docker     (123)    24807 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/grouptype.py
--rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    15138 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/nodetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/policytype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/portspectype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/property_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/relationshiptype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/scalarunit.py
--rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/statefulentitytype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/elements/tosca_type_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/entity_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.130778 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/exttools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.130778 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/mec/
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/mec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.130778 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/nfv/
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/nfv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.114777 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/nfv/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.130778 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/nfv/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py
--rw-r--r--   0 runner    (1001) docker     (123)    39174 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/nodetemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.130778 unfurl-0.7.1/unfurl/vendor/toscaparser/prereq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/prereq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/prereq/csar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/relationship_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/substitution_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/topology_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/tosca_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/tpl_relationship_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/unsupportedtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.130778 unfurl-0.7.1/unfurl/vendor/toscaparser/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/utils/gettextutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/utils/urlutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/utils/validateutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/utils/yamlparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/vendor/toscaparser/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    33481 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/yamlloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    40399 2023-06-13 00:06:26.000000 unfurl-0.7.1/unfurl/yamlmanifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:29.118777 unfurl-0.7.1/unfurl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-06-13 00:06:29.000000 unfurl-0.7.1/unfurl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-13 00:06:29.000000 unfurl-0.7.1/unfurl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:06:29.000000 unfurl-0.7.1/unfurl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-13 00:06:29.000000 unfurl-0.7.1/unfurl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:06:29.000000 unfurl-0.7.1/unfurl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-13 00:06:29.000000 unfurl-0.7.1/unfurl.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-13 00:06:29.000000 unfurl-0.7.1/unfurl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 00:06:29.000000 unfurl-0.7.1/unfurl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.531596 unfurl-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 05:43:06.000000 unfurl-0.8.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      282 2023-07-27 05:43:06.000000 unfurl-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-27 05:43:09.531596 unfurl-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-07-27 05:43:06.000000 unfurl-0.8.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-07-27 05:43:09.531596 unfurl-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 05:43:06.000000 unfurl-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.515596 unfurl-0.8.0/unfurl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44262 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/changelog-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    51759 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/cloudmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51932 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.515596 unfurl-0.8.0/unfurl/configurators/
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/dns-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/docker-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/helm-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16772 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/k8s.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.515596 unfurl-0.8.0/unfurl/configurators/k8s_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/k8s_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/k8s_ansible/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/k8s_ansible/args_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.515596 unfurl-0.8.0/unfurl/configurators/k8s_ansible/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/k8s_ansible/client/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/k8s_ansible/client/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/k8s_ansible/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/k8s_ansible/k8sdynamicclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/kompose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/supervisor-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20833 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/configurators/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30685 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.515596 unfurl-0.8.0/unfurl/filter_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/filter_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/filter_plugins/ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45833 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59277 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56715 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/localenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.515596 unfurl-0.8.0/unfurl/lookup_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/lookup_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/lookup_plugins/unfurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16094 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/manifest-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30966 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25719 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44296 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45879 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/planrequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22281 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/projectpaths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34493 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43549 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83124 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61817 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.515596 unfurl-0.8.0/unfurl/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.515596 unfurl-0.8.0/unfurl/templates/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/aws/unfurl.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.515596 unfurl-0.8.0/unfurl/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/dashboard/manifest.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/dashboard/unfurl.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.515596 unfurl-0.8.0/unfurl/templates/digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/digitalocean/unfurl.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.519596 unfurl-0.8.0/unfurl/templates/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/gcp/unfurl.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/gitignore.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.519596 unfurl-0.8.0/unfurl/templates/home/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/home/manifest-template.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/home/unfurl.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.519596 unfurl-0.8.0/unfurl/templates/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/local/ensemble-examples.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/local-unfurl-template.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/manifest-template.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/manifest.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.519596 unfurl-0.8.0/unfurl/templates/python3.10/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/python3.10/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    63707 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/python3.10/Pipfile.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.519596 unfurl-0.8.0/unfurl/templates/python3.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/python3.11/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    59455 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/python3.11/Pipfile.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.519596 unfurl-0.8.0/unfurl/templates/python3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/python3.7/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    64048 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/python3.7/Pipfile.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.519596 unfurl-0.8.0/unfurl/templates/python3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/python3.8/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    63706 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/python3.8/Pipfile.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.519596 unfurl-0.8.0/unfurl/templates/python3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/python3.9/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    63706 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/python3.9/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/secrets.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/service-template.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/unfurl.local.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/templates/unfurl.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    79136 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61314 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/tosca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.519596 unfurl-0.8.0/unfurl/tosca_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/tosca_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/tosca_plugins/artifacts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/tosca_plugins/googlecloud.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/tosca_plugins/k8s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/tosca_plugins/localhost.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/tosca_plugins/tosca-ext.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/unfurl-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24152 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.519596 unfurl-0.8.0/unfurl/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.519596 unfurl-0.8.0/unfurl/vendor/sphinx-jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/vendor/sphinx-jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/vendor/sphinx-jsonschema/wide_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.527596 unfurl-0.8.0/unfurl/vendor/toscaparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.527596 unfurl-0.8.0/unfurl/vendor/toscaparser/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/dataentity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.531596 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)    32477 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    33031 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/artifacttype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/attribute_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/capabilitytype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24807 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/grouptype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15138 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/nodetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/policytype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/portspectype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/property_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/relationshiptype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/scalarunit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/statefulentitytype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/elements/tosca_type_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/entity_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.531596 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/exttools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.531596 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/mec/
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/mec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.531596 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/nfv/
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/nfv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.511596 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/nfv/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.531596 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/nfv/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39174 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14324 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/nodetemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.531596 unfurl-0.8.0/unfurl/vendor/toscaparser/prereq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/prereq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/prereq/csar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/relationship_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/substitution_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/topology_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/tosca_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/tpl_relationship_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/unsupportedtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.531596 unfurl-0.8.0/unfurl/vendor/toscaparser/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/utils/gettextutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/utils/urlutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/utils/validateutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/utils/yamlparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-27 05:43:07.000000 unfurl-0.8.0/unfurl/vendor/toscaparser/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36571 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/yamlloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40951 2023-07-27 05:43:06.000000 unfurl-0.8.0/unfurl/yamlmanifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:09.515596 unfurl-0.8.0/unfurl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-27 05:43:09.000000 unfurl-0.8.0/unfurl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-27 05:43:09.000000 unfurl-0.8.0/unfurl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:43:09.000000 unfurl-0.8.0/unfurl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-27 05:43:09.000000 unfurl-0.8.0/unfurl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:43:09.000000 unfurl-0.8.0/unfurl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 05:43:09.000000 unfurl-0.8.0/unfurl.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-27 05:43:09.000000 unfurl-0.8.0/unfurl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 05:43:09.000000 unfurl-0.8.0/unfurl.egg-info/top_level.txt
```

### Comparing `unfurl-0.7.1/LICENSE` & `unfurl-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/PKG-INFO` & `unfurl-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: unfurl
-Version: 0.7.1
+Version: 0.8.0
 Summary: use Git to record and deploy changes to your DevOps infrastructure
 Home-page: https://github.com/onecommons/unfurl
 Author: Adam Souzis
 Author-email: adam@onecommons.org
 License: MIT
+Project-URL: Homepage, https://www.unfurl.cloud
+Project-URL: Documentation, https://docs.unfurl.run
+Project-URL: Repository, https://github.com/onecommons/unfurl
+Project-URL: Changelog, https://github.com/onecommons/unfurl/blob/main/CHANGELOG.md
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
-Metadata-Version: 2.1 Name: unfurl Version: 0.7.1 Summary: use Git to record
+Metadata-Version: 2.1 Name: unfurl Version: 0.8.0 Summary: use Git to record
 and deploy changes to your DevOps infrastructure Home-page: https://github.com/
 onecommons/unfurl Author: Adam Souzis Author-email: adam@onecommons.org
-License: MIT Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-Provides-Extra: full Provides-Extra: server Provides-Extra: test License-File:
-LICENSE
+License: MIT Project-URL: Homepage, https://www.unfurl.cloud Project-URL:
+Documentation, https://docs.unfurl.run Project-URL: Repository, https://
+github.com/onecommons/unfurl Project-URL: Changelog, https://github.com/
+onecommons/unfurl/blob/main/CHANGELOG.md Platform: UNKNOWN Classifier:
+Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
+Intended Audience :: Developers Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown Provides-Extra: full Provides-Extra:
+server Provides-Extra: test License-File: LICENSE
                [https://docs.unfurl.run/_images/unfurl_logo.svg]
                                 [PyPI_version]
 # Introduction Unfurl is a command line tool for managing your DevOps
 infrastructure. Unfurl lets you easily track configuration, secrets, software
 and code dependencies, and deployment history all in git. Unfurl can integrate
 with the DevOps tools you are already using -- like Terraform, Ansible, and
 Helm -- allowing you to encapsulate your DevOps processes into reusable
```

### Comparing `unfurl-0.7.1/README.md` & `unfurl-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/setup.cfg` & `unfurl-0.8.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -14,27 +14,30 @@
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+project_urls = 
+	Homepage = https://www.unfurl.cloud
+	Documentation = https://docs.unfurl.run
+	Repository = https://github.com/onecommons/unfurl
+	Changelog = https://github.com/onecommons/unfurl/blob/main/CHANGELOG.md
 
 [extras]
 full = 
-	boto
 	boto3
 	docker[tls]
 	octodns==0.9.14
 	openshift
 	supervisor
 	google-cloud-compute==1.3.2
 	google-cloud-dns==0.34.0
 	google-auth
-	python-gitlab<=3.4.0
 	gunicorn==20.1.0
 	redis==4.3.5
 server = 
 	gunicorn==20.1.0
 	redis==4.3.5
 
 [bdist_wheel]
```

### Comparing `unfurl-0.7.1/unfurl/__init__.py` & `unfurl-0.8.0/unfurl/__init__.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/__main__.py` & `unfurl-0.8.0/unfurl/__main__.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/cloudmap.py` & `unfurl-0.8.0/unfurl/cloudmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 import gitlab
 from gitlab.v4.objects import Project, Group, ProjectTag, ProjectBranch
 
 from .tosca import NodeSpec, ToscaSpec
 
 from .support import ContainerImage
 
-from .to_json import blueprint_metadata
+from .to_json import node_type_to_graphql
 from .repo import (
     GitRepo,
     is_git_worktree,
     normalize_git_url,
     sanitize_url,
     split_git_url,
 )
@@ -113,14 +113,22 @@
 
 
 def filter_dict(d: dict) -> dict:
     # exclude empty values
     return {k: v for k, v in d.items() if v}
 
 
+def match_namespace(path: str, namespace: str) -> bool:
+    if not namespace or path == namespace:
+        return True
+    if not path:
+        return False
+    # don't match on partial segments
+    return path.startswith(os.path.join(namespace, ""))
+
 @dataclass
 class Repository:
     git: str  # hostname and path without protocols, unique key for this record
     path: str  # project path relative to base location of git repositories on the host
     initial_revision: str = ""
     name: str = ""
     protocols: List[str] = field(default_factory=list)
@@ -163,20 +171,15 @@
                 if scheme == "ssh":
                     return "git@" + self.git.replace("/", ":", 1)
                 else:
                     return scheme + "://" + self.git
         return ""
 
     def match_path(self, path: str) -> bool:
-        if not path or path == self.path:
-            return True
-        if not self.path:
-            return False
-        # don't match on partial segments
-        return self.path.startswith(os.path.join(path, ""))
+        return match_namespace(self.path, path)
 
     @property
     def key(self):
         if self.git.endswith(".git"):
             return self.git[:-4]
         return self.git
 
@@ -224,15 +227,17 @@
 
     # push local HEAD to remote "main" branch
     # skip the pipeline because that might cause additional commits
     remote = repo.repo.remotes[remote_name]
     pushinfolist = remote.push(o="ci.skip", follow_tags=True, force=force)
     pushinfo = pushinfolist[0]
     if pushinfolist.error:
-        logger.error(f"pushed to {sanitize_url(remote.url, True)} failed: {pushinfo.summary}")
+        logger.error(
+            f"pushed to {sanitize_url(remote.url, True)} failed: {pushinfo.summary}"
+        )
     else:
         logger.info(f"pushed to {sanitize_url(remote.url, True)}: {pushinfo.summary}")
 
 
 T = TypeVar("T", bound="Notable")
 
 
@@ -252,21 +257,25 @@
     folders: Sequence[str] = ()
     artifact_type = EntitySchema.GenericFile
 
     def __init__(self, root_path: str, folder: str, file: str):
         self.root_path = root_path
         self.folder = folder
         self.file = file
+        self.fragment = ""
         self.metadata: Dict[str, Any] = {}
         self.artifacts: List[ArtifactDict] = []
 
     @property
     def path(self) -> str:
         if self.file:
-            return os.path.join(self.folder, self.file)
+            path = os.path.join(self.folder, self.file)
+            if self.fragment:
+                return path + "#" + self.fragment
+            return path
         else:
             return self.folder
 
     @property
     def full_path(self) -> str:
         return os.path.join(self.root_path, self.folder, self.file)
 
@@ -314,33 +323,39 @@
         if localenv.manifestPath:
             self.artifact_type = self._get_artifacttype(localenv.manifestPath)
             manifest = localenv.get_manifest()
             rel_path = str(
                 Path(localenv.manifestPath).relative_to(Path(self.root_path))
             )
             self.folder, self.file = os.path.split(rel_path)
+            assert manifest.tosca
+            self.fragment = manifest.tosca.fragment
             spec = manifest.tosca
             assert spec
-            assert spec.template
+            assert spec.template and spec.template.tpl
             metadata = spec.template.tpl.get("metadata") or spec.template.tpl or {}
             self.metadata.update(
                 dict(
                     name=metadata.get("template_name"),
                     version=metadata.get("template_version"),
                     description=spec.template.description,
                 )
             )
             node = self._get_root_node(spec)
             schema_repo = manifest.repositories.get("types")
             if schema_repo:
                 self.metadata["schema"] = schema_repo.url.strip(":")
             if node:
+                assert node.toscaEntityTemplate.type_definition
+                type_dict = node_type_to_graphql(
+                    node.topology, node.toscaEntityTemplate.type_definition, {}, True
+                )
                 self.metadata.update(
                     dict(
-                        type=node.type,
+                        type=filter_dict(type_dict),
                         dependencies=list(self.find_dependencies(node).values()),
                     )
                 )
                 image_name = self.find_image_dependency(node)
                 if image_name:
                     self.artifacts.append(
                         {image_name: dict(type=EntitySchema.OCIImage)}
@@ -490,25 +505,25 @@
         logger.debug(f"looking for repos in {root}")
         if root:
             for working_dir in find_git_repos(root):
                 self._add_repo(working_dir)
         self.repos_root = root
 
     @staticmethod
-    def _choose_remote(remotes: List[git.Remote], hint: str):
+    def _choose_remote(remotes: List[git.Remote], hint: str) -> git.Remote:
         host = origin = canonical = None
         for remote in remotes:
             if remote.name == hint:
                 host = remote
             elif remote.name == "origin":
                 origin = remote
             elif remote.name == "canonical":
                 canonical = remote
         # find best candidate
-        return origin or host or canonical or remotes[0]
+        return host or origin or canonical or remotes[0]
 
     def find_repo(self, url: str, hint: str) -> Optional[GitRepo]:
         remotes = self.remotes.get(get_remote_git_url(url))
         if remotes:
             # find best candidate
             remote = self._choose_remote(remotes, hint)
             return self.repos[cast(str, remote.repo.working_tree_dir)]
@@ -602,14 +617,15 @@
         if self.artifacts:
             self.db["artifacts"] = {
                 a: self.artifacts[a] for a in sorted(self.artifacts)
             }
         self.config.save()
 
     def clone_repo(self, repo_info: Repository, url: str) -> GitRepo:
+        # XXX handle conflict when same path, different host
         download_path = str(Path(self.repos_root) / repo_info.path)
         repo = git.Repo.clone_from(url or repo_info.git_url(), download_path)
         return GitRepo(repo)
 
     def analyze_repo(self, repo: GitRepo) -> List[Notable]:
         notables: List[Notable] = []
 
@@ -646,15 +662,15 @@
         repo_info.add_notables(notables)
         for n in notables:
             for a in n.artifacts:
                 self.artifacts.update(a)
         return notables
 
 
-def get_remote_git_url(url):
+def get_remote_git_url(url: str) -> str:
     """Return the location of the git server without the scheme or user"""
     parts = urlparse(url)
     if not parts.netloc and not parts.scheme and "@" in url:
         # scp style used by git: user@server:project.git
         parts = urlparse("ssh://" + url.replace(":", "/", 1))
     if parts.netloc:
         user, sep, host = parts.netloc.rpartition("@")
@@ -722,35 +738,50 @@
         return repo
 
 
 class LocalRepositoryHost(RepositoryHost, _LocalGitRepos):
     """
     Locally manage git repositories from any origin using the git protocol.
     """
+    def __init__(self, local_repo_root: str = "", namespace: str = "") -> None:
+        _LocalGitRepos.__init__(self, local_repo_root)
+        self.path = namespace
 
     def has_repository(self, repo_info: Repository) -> bool:
         return repo_info.git in self.remotes
 
     def include_local_repo(self, repo: GitRepo) -> bool:
-        return bool(repo.remote)  # XXX check host and namespace filters too
+        return bool(repo.remote)
 
     def from_host(self, directory: Directory):
         """Pull latest and update the cloudmap to match the local repositories."""
         for repo in self.repos.values():
             if self.include_local_repo(repo):
-                repo.pull()  # XXX make optional?
-                assert repo.repo.working_dir
                 path = str(
-                    Path(repo.repo.working_dir).relative_to(
+                    Path(repo.working_dir).relative_to(
                         Path(os.path.abspath(self.repos_root))
                     )
                 )
-                repository = self.git_to_repository(repo, path)
+                if not match_namespace(path, self.path):
+                    continue
+                # prefer "canonical" remote
+                remote = _LocalGitRepos._choose_remote(repo.repo.remotes, "canonical")
+                assert repo.repo.working_dir
+                if not os.getenv("UNFURL_SKIP_UPSTREAM_CHECK"):
+                    repo.pull(remote.name)
+                repository = self.git_to_repository(remote, path)
+                repository.initial_revision = repo.get_initial_revision()
                 previous = directory.repositories.get(repository.key)
-                directory.repositories[repository.key] = repository
+                if previous:
+                    # don't replace metadata from remote host
+                    if not previous.initial_revision:
+                        previous.initial_revision = repository.initial_revision
+                    repository = previous
+                else:
+                    directory.repositories[repository.key] = repository
                 directory.maybe_analyze(
                     repository, repo, previous.notable if previous else {}
                 )
 
     def to_host(self, directory: Directory, merge: bool, force: bool) -> bool:
         """Push cloudmap revisions to origin."""
         matched = False
@@ -762,31 +793,30 @@
                     if cloudmap_local_repo:
                         repo.pull(cloudmap_local_repo.working_dir)
                 repo.push()
                 matched = True
         return matched
 
     @staticmethod
-    def git_to_repository(repo: GitRepo, path: str) -> "Repository":
-        assert repo.remote  # origin
-        url = repo.remote.url
+    def git_to_repository(remote: git.Remote, path: str) -> "Repository":
+        url = remote.url
         record = Repository(
             git=get_remote_git_url(url),
             path=path,
             protocols=[urlparse(url).scheme or "ssh"],
-            initial_revision=repo.get_initial_revision(),
         )
         # to get default branch:
         # first line of git ls-remote --symref url
         # ref: refs/heads/main	HEAD
 
         # add origin's refs as branches
         # refs iterates over .git/refs/remotes/origin/*
-        remote_refs = sorted(repo.repo.remote().refs, key=lambda r: r.name)
+        remote_refs = sorted(remote.refs, key=lambda r: r.name)
         # (git fetch --tags to get the latest tag refs)
+        # XXX include branches for all remotes that point to the same url
         record.branches = {
             ref.remote_head: ref.commit.hexsha
             for ref in remote_refs
             if ref.remote_head != "HEAD"
         }
         # XXX add other remotes as mirrors?
         return record
@@ -868,17 +898,15 @@
                 repo = self.fetch_repo(remote_url, r, directory)
                 directory.maybe_analyze(r, repo, previous.notable if previous else {})
 
     def _get_projects_from_group(self, group, projects):
         for p in group.projects.list(iterator=True):
             projects[p.path_with_namespace][0] = p  # type: ignore
         for subgroup in group.subgroups.list(iterator=True):
-            self._get_projects_from_group(
-                self.gitlab.groups.get(subgroup.id), projects
-            )
+            self._get_projects_from_group(self.gitlab.groups.get(subgroup.id), projects)
 
     def to_host(self, directory: Directory, merge: bool, force: bool) -> bool:
         """
         Create or update projects in a gitlab instance.
         If the target project has changed, update the records.
 
         If merge is True and there a local repositories associate with the directory,
@@ -913,15 +941,17 @@
 
         for name in projects:
             dest, repo_info = projects[name]
             if repo_info:
                 if dest:
                     # if both exist, update any changed metadata
                     if self.dryrun:
-                        logger.info("dry run: skipping creating updating project %s", name)
+                        logger.info(
+                            "dry run: skipping creating updating project %s", name
+                        )
                     else:
                         self.update_project_metadata(repo_info, dest)
                     do_merge = not force and merge
                 else:
                     if self.dryrun:
                         logger.info("dry run: skipping creating project %s", name)
                         continue
@@ -940,15 +970,18 @@
                             repo = self.fetch_repo(remote_url, repo_info, directory)
                             # clone source repo and push to dest
                             dest_branch = (
                                 f"{self.name}/{repo_info.get_default_branch()}"
                             )
                             commit = repo.repo.head.commit
                             branch_exists = dest_branch in repo.repo.references
-                            if not branch_exists or commit != repo.repo.references[dest_branch].commit:
+                            if (
+                                not branch_exists
+                                or commit != repo.repo.references[dest_branch].commit
+                            ):
                                 # now update project repository
                                 logger.info(
                                     f"{force and '(force) ' or ' '}{do_merge and 'merging' or 'pushing'} local repository to {repo.safe_url}"
                                 )
                                 if self.dryrun:
                                     summary = cast(str, commit.summary)
                                     logger.info(
@@ -1208,15 +1241,15 @@
                 host_config = dict(type="local", clone_root=clone_root)
             elif ":" in name:
                 # assume it's an url pointing to gitlab or unfurl cloud instance
                 host_config = dict(type="gitlab", url=name)
             else:
                 raise UnfurlError(f"no repository host named {name} found")
         if host_config["type"] == "local":
-            return LocalRepositoryHost(host_config.get("clone_root", clone_root))
+            return LocalRepositoryHost(host_config.get("clone_root", clone_root), namespace)
 
         assert host_config["type"] in ["gitlab", "unfurl.cloud"]
         config = local_env.map_value(host_config, environment.get("variables"))
         if visibility:
             config["visibility"] = visibility
         return GitlabManager(name, config, namespace)
```

### Comparing `unfurl-0.7.1/unfurl/configurator.py` & `unfurl-0.8.0/unfurl/configurator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright (c) 2020 Adam Souzis
 # SPDX-License-Identifier: MIT
+import inspect
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Generator,
     List,
     Optional,
@@ -67,37 +68,36 @@
 
 # Tell mypy the logger is of type UnfurlLogger
 logger = cast(UnfurlLogger, logging.getLogger("unfurl.task"))
 
 
 class ConfiguratorResult:
     """
-    Modified indicates whether the underlying state of configuration,
-    was changed i.e. the physically altered the system this configuration represents.
+    Represents the result of a task that ran. 
 
-    status reports the Status of the current configuration.
+    See :py:meth:`TaskView.done` for more documentation.
     """
 
     def __init__(
         self,
         success: bool,
         modified: Optional[bool],
         status: Optional[Status] = None,
-        configChanged: bool = None,
+        configChanged: Optional[bool] = None,
         result: object = None,
         outputs: Optional[dict] = None,
         exception: Optional[UnfurlTaskError] = None,
     ) -> None:
         self.modified = modified
         self.status = to_enum(Status, status)
         self.configChanged = configChanged
         self.result = result
         self.success = success
         self.outputs = outputs
-        self.exception = None
+        self.exception = exception
 
     def __str__(self) -> str:
         result = "" if self.result is None else str(self.result)[:240] + "..."
         return (
             "changes: "
             + (
                 " ".join(
@@ -128,81 +128,121 @@
         if name:
             register_class(cls.__module__ + "." + cls.__name__, cls, name)
         return cls
 
 
 @six.add_metaclass(AutoRegisterClass)
 class Configurator:
+    """
+    Base class for implementing `Configurators`. 
+    Subclasses should at least implement a :py:meth:`~Configurator.run`, for example:
+
+    .. code-block:: python
+
+        class MinimalConfigurator(Configurator):
+            def run(self, task):
+                assert self.can_run(task)
+                return Status.ok    
+
+    """
+
     short_name: Optional[str] = None
     """shortName can be used to customize the "short name" of the configurator
     as an alternative to using the full name ("module.class") when setting the implementation on an operation.
     (Titlecase recommended)"""
 
     exclude_from_digest: Tuple[str, ...] = ()
 
     attribute_output_metadata_key: Optional[str] = None
 
+    __is_generator: Optional[bool] = None
+
     @classmethod
     def set_config_spec_args(klass, kw: dict, target: EntityInstance) -> dict:
         return kw
 
     def __init__(self, configurationSpec: ConfigurationSpec) -> None:
         self.configSpec = configurationSpec
 
+    def _run(self, task: "TaskView") -> Generator:
+        # internal function to convert user defined run() to a generator
+        result = self.run(task)
+        if isinstance(result, ConfiguratorResult):
+            yield result
+        elif isinstance(result, Status):
+            yield task.done(None, None, result)
+        elif isinstance(result, (bool, type(None))):
+            yield task.done(result)
+        else:
+            raise UnfurlTaskError(task, "bad return valuate")
+
+    def _is_generator(self):
+        if self.__is_generator is None:
+            self.__is_generator = inspect.isgeneratorfunction(self.run)
+        return self.__is_generator
+
     def get_generator(self, task: "TaskView") -> Generator:
-        return self.run(task)
+        if self._is_generator():
+            return self.run(task)  # type: ignore
+        else:
+            return self._run(task)
 
     def render(self, task: "TaskView") -> Any:
         """
-        This method is called is called during the planning phase to give the configurator an
+        This method is called during the planning phase to give the configurator an
         opportunity to do early validation and error detection and generate any plan information or configuration files that the user may want to review before the running the deployment task.
 
         Property access and writes will be tracked and used to establish dynamic dependencies between instances so the plan can be ordered properly. Any updates made to instances maybe reverted if it has dependencies on attributes that might be changed later in the plan, so this method should be idempotent.
 
         Returns:
             The value returned here will subsequently be available as ``task.rendered``
         """
         return None
 
     # yields a JobRequest, TaskRequest or a ConfiguratorResult
-    def run(self, task: "TaskView") -> Generator:
+    def run(self, task: "TaskView") -> Union[Generator, ConfiguratorResult, Status, bool]:
         """
-        This should perform the operation specified in the :class:`ConfigurationSpec`
-        on the :obj:`task.target`.
+        Subclasses of Configurator need to implement this method.
+        It should perform the operation specified in the :class:`ConfigurationSpec`
+        on the :obj:`task.target`. It can be either a generator that yields one or more :class:`JobRequest` or :class:`TaskRequest`
+        or a regular function.
 
         Args:
-            task (:class:`TaskView`) The task currently running.
+            task (:class:`TaskView`): The task currently running.
 
         Yields:
-            Should yield either a :class:`JobRequest`, :class:`TaskRequest`
-            or a :class:`ConfiguratorResult` when done
+            Optionally ``run`` can yield either a :class:`JobRequest`, :class:`TaskRequest` to run subtasks
+            and finally a :class:`ConfiguratorResult` when done
+
+        Returns:
+            If ``run`` is not defined as a generator it must return either a :py:class:`~unfurl.support.Status`, a ``bool`` or a :class:`ConfiguratorResult` to indicate if the task succeeded and any changes to the target's state.
         """
         yield task.done(False)
 
     def can_dry_run(self, task: "TaskView") -> bool:
         """
         Returns whether this configurator can handle a dry-runs for the given task.
         (And should check :attr:`.TaskView.dry_run` in during run().
 
         Args:
-            task (:obj:`TaskView`) The task about to be run.
+            task (:obj:`TaskView`): The task about to be run.
 
         Returns:
             bool
         """
         return False
 
     def can_run(self, task: "TaskView") -> Union[bool, str]:
         """
         Return whether or not the configurator can execute the given task
         depending on if this configurator support the requested action and parameters
         and given the current state of the target instance?
 
         Args:
-            task (:class:`TaskView`) The task that is about to be run.
+            task (:class:`TaskView`): The task that is about to be run.
 
         Returns:
             (bool or str): Should return True or a message describing why the task couldn't be run.
         """
         return True
 
     def should_run(self, task: "TaskView") -> Union[bool, Priority]:
@@ -261,18 +301,16 @@
         Examine the previous :class:`ChangeRecord` generated by the previous time this operation
         was performed on the target instance and return whether it should be rerun or not.
 
         The default implementation recalculates the digest of input parameters that
         were accessed in the previous run.
 
         Args:
-            task (:class:`TaskView`) The task that might execute this operation.
-
-        Args:
-            changest (:class:`ChangeRecord`) The task that might execute this operation.
+            task (:class:`TaskView`): The task that might execute this operation.
+            changeset (:class:`ChangeRecordRecord`): The task that might execute this operation.
 
         Returns:
             bool: True if configuration's digest has changed, False if it is the same.
         """
         _parameters = getattr(changeset, "digestKeys", "")
         newKeys = {k for k in task.inputs.keys() if k not in self.exclude_from_digest}
         task.logger.debug("checking digest for %s: %s", task.target.name, _parameters)
@@ -423,14 +461,15 @@
         self._manifest = manifest
         self.messages: List[object] = []
         self._addedResources: List[NodeInstance] = []
         self._dependenciesChanged = False
         self.dependencies: List["Operational"] = dependencies or []
         self._resourceChanges = ResourceChanges()
         self._workFolders: Dict[str, WorkFolder] = {}
+        self._failed_paths: List[str] = []
         self._rendering = False
         self._environ: object = None
         # public:
         self.operation_host = find_operation_host(target, configSpec.operation_host)
 
     @property
     def environ(self) -> Dict[str, str]:
@@ -661,31 +700,37 @@
             target=self.target.name,
             reason=self.reason,
             cwd=self.cwd,
         )
 
     @staticmethod
     def find_connection(
-        ctx: RefContext, target: NodeInstance, relation: str = "tosca.relationships.ConnectsTo"
+        ctx: RefContext,
+        target: NodeInstance,
+        relation: str = "tosca.relationships.ConnectsTo",
     ) -> Optional[RelationshipInstance]:
         """
         Find a relationship that this task can use to connect to the given instance.
         First look for relationship between the task's target instance and the given instance.
         If none is found, see if there a default connection of the given type.
 
         Args:
             target (NodeInstance): The instance to connect to.
-            relation (str, optional): The relationship type. Defaults to "tosca.relationships.ConnectsTo".
+            relation (str, optional): The relationship type. Defaults to ``tosca.relationships.ConnectsTo``.
 
         Returns:
             RelationshipInstance or None: The connection instance.
         """
-        connection = cast(Optional[RelationshipInstance], Ref(
-            f"$OPERATION_HOST::.requirements::*[.type={relation}][.target=$target]",
-            vars=dict(target=target)).resolve_one(ctx))
+        connection = cast(
+            Optional[RelationshipInstance],
+            Ref(
+                f"$OPERATION_HOST::.requirements::*[.type={relation}][.target=$target]",
+                vars=dict(target=target),
+            ).resolve_one(ctx),
+        )
 
         # alternative query: [.type=unfurl.nodes.K8sCluster]::.capabilities::.relationships::[.type=unfurl.relationships.ConnectsTo.K8sCluster][.source=$OPERATION_HOST]
         if not connection:
             # no connection, see if there's a default relationship template defined for this target
             endpoints = target.get_default_relationships(relation)
             if endpoints:
                 connection = endpoints[0]
@@ -752,15 +797,15 @@
         status: Optional[Status] = None,
         result: Optional[Union[dict, str]] = None,
         outputs: Optional[
             dict
         ] = None,  # so the docstring says dict, but ConfiguratorResult
         captureException: Optional[object] = None,
     ) -> ConfiguratorResult:
-        """:py:meth:`unfurl.configurator.Configurator.run` should call this method and yield its return value before terminating.
+        """:py:meth:`unfurl.configurator.Configurator.run` should call this method and return or yield its return value before terminating.
 
         >>> yield task.done(True)
 
         Args:
 
           success (bool):  indicates if this operation completed without an error.
           modified (bool): (optional) indicates whether the physical instance was modified by this operation.
@@ -964,21 +1009,25 @@
             updated = True
 
         template = resourceSpec.get("template")
         if template:
             assert self._manifest.tosca
             if isinstance(template, dict):
                 tname = existingResource.template.name
-                existingResource.template = existingResource.template.topology.add_node_template(
-                    tname, template
+                existingResource.template = (
+                    existingResource.template.topology.add_node_template(
+                        tname, template
+                    )
                 )
             elif (
                 isinstance(template, str) and template != existingResource.template.name
             ):
-                nodeSpec = existingResource.template.topology.get_node_template(template)
+                nodeSpec = existingResource.template.topology.get_node_template(
+                    template
+                )
                 if not nodeSpec:
                     raise UnfurlTaskError(
                         self,
                         f"couldn't update TOSCA template for {existingResource.name}: '{template}' is not defined",
                     )
                 existingResource.template = nodeSpec
             updated = True
@@ -1134,15 +1183,17 @@
         while self._workFolders:
             _, wf = self._workFolders.popitem()
             wf.discard()
 
     def fail_work_folders(self) -> None:
         while self._workFolders:
             _, wf = self._workFolders.popitem()
-            wf.failed()
+            failed_path = wf.failed()
+            if failed_path:
+                self._failed_paths.append(failed_path)
 
     def apply_work_folders(self, *names: str) -> None:
         if not names:  # no args were passed, apply them all
             names = self._workFolders.keys()  # type: ignore
         for name in names:
             wf = self._workFolders.get(name)
             if wf and (wf.always_apply or self.status == Status.ok):  # type: ignore
```

### Comparing `unfurl-0.7.1/unfurl/configurators/__init__.py` & `unfurl-0.8.0/unfurl/configurators/__init__.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/configurators/ansible.py` & `unfurl-0.8.0/unfurl/configurators/ansible.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,14 +427,19 @@
     inventoryArgs = ["-i", _inventory] if _inventory else []
     args = ["ansible-playbook"] + inventoryArgs + (args or []) + [playbook]
     return args
 
 
 def _run_playbooks(args, params=None, vault_secrets=None):
     logger.info("running " + " ".join(args))
+    # collections may have been installed while the job is running, need reset the loader to pick those up
+    from ansible.plugins.loader import _configure_collection_loader
+    from ansible.utils.collection_loader._collection_finder import AnsibleCollectionConfig
+    AnsibleCollectionConfig._collection_finder = None
+    _configure_collection_loader()
     cli = PlaybookCLI(args)
 
     context._init_global_context = _init_global_context
     cli.parse()
 
     # replace C.DEFAULT_STDOUT_CALLBACK with our own so we have control over logging
     # config/base.yml sets C.DEFAULT_STDOUT_CALLBACK == 'default' (ansible/plugins/callback/default.py)
```

### Comparing `unfurl-0.7.1/unfurl/configurators/dns-template.yaml` & `unfurl-0.8.0/unfurl/configurators/dns-template.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/configurators/dns.py` & `unfurl-0.8.0/unfurl/configurators/dns.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/configurators/docker-template.yaml` & `unfurl-0.8.0/unfurl/configurators/docker-template.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Copyright (c) 2020 Adam Souzis
 # SPDX-License-Identifier: MIT
 tosca_definitions_version: tosca_simple_unfurl_1_0_0
+imports:
+  - repository: unfurl
+    file: tosca_plugins/artifacts.yaml
 data_types:
   unfurl.datatypes.DockerContainer:
     # properties match Docker compose schema
     # see https://docs.docker.com/compose/compose-file/compose-file-v3
     metadata:
       additionalProperties: true
     properties:
@@ -117,26 +120,27 @@
         type: string
         default: "{{ '.::.artifacts::image::.repository::credential::token' | eval }}"
         required: false
 
     interfaces:
       defaults:
         implementation:
+          primary: community.docker
           className: unfurl.configurators.ansible.AnsibleConfigurator
         outputs:
           container: # dict matching docker container inspect output, including HostPort
           image_path:
         inputs:
           playbook:
             eval:
               template: |
                 #jinja2: variable_start_string: '<%', variable_end_string: '%>'
                 {% filter from_yaml %}
                 {%if 'registry_user' | eval %}
-                - docker_login:
+                - community.docker.docker_login:
                      # https://docs.ansible.com/ansible/latest/modules/docker_login_module.html#docker-login-module
                      # https://github.com/ansible/ansible/blob/stable-2.8/lib/ansible/modules/cloud/docker/docker_login.py
                      username: "<% SELF.registry_user %>"
                      password: "<% SELF.registry_password %>"
                      registry_url: "<% SELF.registry_url %>"
                 {% endif %}
                 - set_fact:
```

### Comparing `unfurl-0.7.1/unfurl/configurators/gcp.py` & `unfurl-0.8.0/unfurl/configurators/gcp.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/configurators/helm-template.yaml` & `unfurl-0.8.0/unfurl/configurators/helm-template.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       +HELM_KUBETOKEN:
           eval: $connections::K8sCluster::token
       +HELM_KUBEAPISERVER:
           eval:
             if: $connections::K8sCluster::api_server
             then:
               if: "{{ '//' in '$connections::K8sCluster::api_server' | eval }}"
-              then: 
+              then:
                 eval: $connections::K8sCluster::api_server
               else: "{{ '$connections::K8sCluster::protocol' | eval }}://{{ '$connections::K8sCluster::api_server' | eval }}"
             else: null
       +HELM_KUBECAFILE:
           eval: $connections::K8sCluster::cluster_ca_certificate_file
       +HELM_NAMESPACE:
           eval: $connections::K8sCluster::namespace
@@ -86,15 +86,16 @@
                   {% endfor%}
                 {%endif%}
         discover:
           implementation: helm
           inputs:
             command: helm repo list -o json {% if task.verbose > 0 %}--debug{%endif%}
             done:
-              success: True # helm repo list returns error if there are no repos so set success true regardless
+              success: true # helm repo list returns error if there are no repos so set success true regardless
+              modified: false
             resultTemplate: |
               {%if returncode == 0 %}
                 {%for json in stdout | from_json %}
                   - name: {{ json.name }}-helm-repo
                     template:
                       type: unfurl.nodes.HelmRepository
                       properties:
@@ -141,16 +142,19 @@
               chart: { get_property: ["SELF", "chart"] }
               release_name: { get_property: ["SELF", "release_name"] }
               dryrun: "--dry-run"
               chart_values: { get_property: ["SELF", "chart_values"] }
               command:
                 eval:
                   template: >-
-                    helm {{inputs.helmcmd}} {{inputs.release_name}} {{inputs.chart }} -o json 
+                    helm {{inputs.helmcmd}} {{inputs.release_name}} {{inputs.chart }} -o json
                       {% if SELF.namespace %}--namespace {{ SELF.namespace }}{% endif %}
+                      {%if lookup('env', 'KUBE_INSECURE') %}
+                      --kube-insecure-skip-tls-verify
+                      {% endif %}
                       {% if inputs.chart_values | default('', true) %}
                       --values {{ valuesfile }}
                       {% endif %}
                       {% if task.verbose > 0 %}--debug{%endif%}
                       {% if task.timeout %}--timeout {{task.timeout}}{%endif%}
                       {% if inputs.helmcmd == 'upgrade' %}--reuse-values{%endif%}
                       {% if inputs.flags is defined -%}
@@ -212,15 +216,15 @@
             implementation:
               primary: helm
               environment: *environment
             inputs:
               command:
                 eval:
                   template: >-
-                    helm uninstall {{ "release_name" | eval }} 
+                    helm uninstall {{ "release_name" | eval }}
                       {% if SELF.namespace %}--namespace {{ SELF.namespace }}{% endif %}
                       {% if task.verbose > 0 %}--debug{%endif%}
                       {% if task.timeout %}--timeout {{task.timeout}}{%endif%}
                       {% if inputs.flags is defined -%}
                         {% for flag, value in inputs.flags.items() %}
                           --{{flag}} "{{value | quote }}"
                         {% endfor%}
@@ -228,14 +232,19 @@
               # XXX add result template that removes added resources
 
       Install:
         operations:
           check:
             invoke: Helm.execute
             inputs:
+              done:
+                success: true # helm status returns an error if the release doesn't exist
+                modified: false
+              resultTemplate: |
+                - readyState: {%if returncode == 0 %}ok{%else%}absent{%endif%}
               helmcmd: status
               dryrun: "--dry-run"
               # don't pass these as cmd arguments
               chart: ""
               chart_values: ""
           discover:
             invoke: Helm.execute
```

### Comparing `unfurl-0.7.1/unfurl/configurators/k8s.py` & `unfurl-0.8.0/unfurl/configurators/k8s.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,17 @@
 from ..configurator import Configurator, TaskView
 from ..support import Status, Priority, to_kubernetes_label
 from ..runtime import EntityInstance, NodeInstance, RelationshipInstance
 from ..util import UnfurlTaskError, wrap_sensitive_value, sensitive_dict
 from .ansible import AnsibleConfigurator
 from ..yamlloader import yaml
 from ..eval import Ref, RefContext, set_eval_func, map_value
+from .k8s_ansible import get_api_client
 import subprocess
 import json
-from ansible_collections.kubernetes.core.plugins.module_utils.common import (
-    K8sAnsibleMixin,
-)
-
-# XXX need to define fail_json
-# class K8sAnsibleClient(K8sAnsibleMixin):
-# def fail_json(msg):
 
 
 def _get_connection_config(instance):
     # Given an endpoint capability or a connection relationship, return a dictionary of connection settings.
     # https://docs.ansible.com/ansible/latest/collections/kubernetes/core/k8s_module.html
     #  for connection settings
     # https://github.com/ansible-collections/kubernetes.core/blob/7f7008fecc9e5d16340e9b0bff510b7cde2f2cfd/plugins/connection/kubectl.py
@@ -139,15 +133,15 @@
     if namespace:
         config["namespace"] = cast(NodeInstance, namespace).attributes["name"]
     return config
 
 
 set_eval_func(
     "kubernetes_current_namespace",
-    lambda args, ctx: _get_connection(ctx).get("namespace") if ctx.task else None,
+    lambda args, ctx: _get_connection(ctx).get("namespace"),
 )
 
 
 def get_kubectl_args(ctx: RefContext):
     connection = _get_connection(ctx)
     options = []
     for key, value in connection.items():
@@ -198,15 +192,15 @@
       .dockerconfigjson: {b64encode(json.dumps(data).encode()).decode()}
     """
 
 
 class ClusterConfigurator(Configurator):
     @staticmethod
     def _get_host(connectionConfig):
-        client = K8sAnsibleMixin().get_api_client(**connectionConfig)
+        client = get_api_client(**connectionConfig)
         url = client.configuration.host
         if url:
             return re.sub("^https?://", "", url)
         return url
 
     def can_run(self, task):
         if task.configSpec.operation not in ["check", "discover"]:
@@ -289,14 +283,24 @@
                     for container in containers:
                         for env in container.get("env") or []:
                             if "value" in env:
                                 env["value"] = task.sensitive(env["value"])
 
 
 class ResourceConfigurator(AnsibleConfigurator):
+
+    @classmethod
+    def set_config_spec_args(klass, kw: dict, target: EntityInstance):
+        artifact = target.template.find_or_create_artifact(
+            "kubernetes.core", predefined=True
+        )
+        if artifact:
+            kw["dependencies"].append(artifact)
+        return kw
+
     def get_generator(self, task):
         if task.dry_run:
             return self.dry_run(task)
         else:
             return self.run(task)
 
     def dry_run(self, task):
@@ -305,15 +309,15 @@
 
     def make_secret(self, data, type="Opaque"):
         return dict(
             type=type,
             apiVersion="v1",
             kind="Secret",
             data=sensitive_dict(
-                {k: b64encode(str(v).encode()).decode() for k, v in data.items()}
+                {k: b64encode(str(v).encode()).decode() for k, v in data.items() if v is not None}
             ),
         )
 
     def get_definition(self, task):
         if task.target.template.is_compatible_type("unfurl.nodes.K8sNamespace"):
             return dict(apiVersion="v1", kind="Namespace")
```

### Comparing `unfurl-0.7.1/unfurl/configurators/kompose.py` & `unfurl-0.8.0/unfurl/configurators/kompose.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/configurators/shell.py` & `unfurl-0.8.0/unfurl/configurators/shell.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/configurators/supervisor-template.yaml` & `unfurl-0.8.0/unfurl/configurators/supervisor-template.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/configurators/supervisor.py` & `unfurl-0.8.0/unfurl/configurators/supervisor.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/configurators/terraform.py` & `unfurl-0.8.0/unfurl/configurators/terraform.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/eval.py` & `unfurl-0.8.0/unfurl/eval.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/filter_plugins/ref.py` & `unfurl-0.8.0/unfurl/filter_plugins/ref.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # Copyright (c) 2020 Adam Souzis
 # SPDX-License-Identifier: MIT
 from unfurl.eval import Ref, map_value
 from unfurl.projectpaths import _abspath, _getdir
-from unfurl.support import to_dns_label, to_googlecloud_label, to_kubernetes_label, to_label
+from unfurl.support import (
+    to_dns_label,
+    to_googlecloud_label,
+    to_kubernetes_label,
+    to_label,
+)
 from unfurl.util import which, wrap_sensitive_value
 from jinja2.filters import contextfilter  # type: ignore
 
 # from ansible.errors import AnsibleError, AnsibleFilterError
 
 
 @contextfilter
@@ -72,25 +77,32 @@
 #         indent=indent,
 #         allow_unicode=True,
 #         default_flow_style=False,
 #         **kw
 #     )
 #     return to_text(transformed)
 
+SAFE_FILTERS = {
+    "ref": ref,
+    "eval": ref,
+    "mapValue": map_value_filter,
+    "map_value": map_value_filter,
+    "sensitive": wrap_sensitive_value,
+    "to_label": to_label,
+    "to_dns_label": to_dns_label,
+    "to_kubernetes_label": to_kubernetes_label,
+    "to_googlecloud_label": to_googlecloud_label,
+}
+
+ALL_FILTERS = dict(
+    SAFE_FILTERS,
+    **{
+        "abspath": abspath,
+        "get_dir": get_dir,
+        "which": which,
+    }
+)
 
 
 class FilterModule:
     def filters(self):
-        return {
-            "ref": ref,
-            "eval": ref,
-            "mapValue": map_value_filter,
-            "map_value": map_value_filter,
-            "abspath": abspath,
-            "get_dir": get_dir,
-            "which": which,
-            "sensitive": wrap_sensitive_value,
-            "to_label": to_label,
-            "to_dns_label": to_dns_label,
-            "to_kubernetes_label": to_kubernetes_label,
-            "to_googlecloud_label": to_googlecloud_label,
-        }
+        return ALL_FILTERS
```

### Comparing `unfurl-0.7.1/unfurl/init.py` & `unfurl-0.8.0/unfurl/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1209,26 +1209,32 @@
         pipfileLocation = os.path.abspath(pipfileLocation)
 
     try:
         cwd = os.getcwd()
         os.chdir(projectDir)
         # need to set env vars and change current dir before importing pipenv
         from pipenv import environments
-        from pipenv.core import do_install
+        try:
+            from pipenv.routines.install import do_install
+            kw: Dict = dict(categories=[], extra_pip_args=[])
+        except ImportError:
+            from pipenv.core import do_install
+            kw = dict(extra_index_url=[])
+
         from pipenv.project import Project as PipEnvProject
 
         pythonPath = os.environ["PIPENV_PYTHON"]
         assert pythonPath, pythonPath
         if not pipfileLocation:
             pipfileLocation = pipfile_template_dir(pythonPath)
         if not os.path.isdir(pipfileLocation):
             return f'Pipfile location is not a valid directory: "{pipfileLocation}"'
         copy_pipfiles(pipfileLocation, projectDir)
 
-        kw: Dict = dict(python=pythonPath, extra_index_url=[])
+        kw["python"] = pythonPath
         pipenv_project = PipEnvProject()
         # need to run without args first so lock isn't overwritten
         retcode = _run_pip_env(do_install, pipenv_project, kw)
         if retcode:
             return f"Pipenv (step 1) failed: {retcode}"
 
         # we need to set these so pipenv doesn't try to recreate the virtual environment
```

### Comparing `unfurl-0.7.1/unfurl/job.py` & `unfurl-0.8.0/unfurl/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,15 @@
     change_detection: str = "evaluate"
     repair: str = "error"
     force: bool = False
     check: bool = False
     prune: bool = False
     destroyunmanaged: bool = False
     upgrade: bool = False
+    dryrun: bool = False
 
     defaults = dict(
         global_defaults,
         parentJob=parentJob,
         instance=instance,
         instances=None,
         template=None,
@@ -498,15 +499,15 @@
         name = self.configSpec.name
         if self.configSpec.operation and self.configSpec.operation not in name:
             name = name + ":" + self.configSpec.operation
         if self.reason and self.reason not in name:
             return name + ":" + self.reason
         return name
 
-    def summary(self, asJson=False):
+    def summary(self, asJson=False, add_rendered=False):
         if self.target.name != self.target.template.name:
             rname = f"{self.target.name} ({self.target.template.name})"
         else:
             rname = self.target.name
 
         if self.configSpec.name != self.configSpec.className:
             cname = f"{self.configSpec.name} ({self.configSpec.className})"
@@ -531,14 +532,21 @@
             else self.target_status.name,
             targetState=self.target_state and self.target_state.name or None,
             changed=self.modified_target,
             configurator=configurator,
             priority=self.priority.name,
             reason=self.reason or "",
         )
+        if add_rendered:
+            summary["rendered_paths"] = [
+                path
+                for path in [wf.cwd for wf in self._workFolders.values()]
+                + self._failed_paths
+                if os.path.exists(path)
+            ]
 
         if asJson:
             return summary
         else:
             return (
                 "{operation} on instance {rname} (type {type}, status {targetStatus}) "
                 + "using configurator {cname}, priority: {priority}, reason: {reason}"
@@ -586,15 +594,15 @@
         rootResource: TopologyInstance,
         jobOptions: JobOptions,
         previousId: Optional[str] = None,
     ) -> None:
         assert isinstance(jobOptions, JobOptions)
         self.__dict__.update(jobOptions.__dict__)
         super().__init__(self.parentJob, self.startTime, Status.ok, previousId)  # type: ignore
-        self.dry_run = jobOptions.dryrun  # type: ignore
+        self.dry_run = jobOptions.dryrun
         self.jobOptions = jobOptions
         self.manifest = manifest
         self.rootResource = rootResource
         self.jobRequestQueue: List[JobRequest] = []
         self.unexpectedAbort: Optional[UnfurlError] = None
         self.workDone: Dict[int, ConfigTask] = collections.OrderedDict()
         self.timeElapsed: float = 0
@@ -642,15 +650,15 @@
                 self.jobOptions.instance  # type: ignore
             )
         ):
             logger.warning(
                 'selected instance not found: "%s"', self.jobOptions.instance  # type: ignore
             )
 
-    def render(self) -> Tuple[List[PlanRequest], List[PlanRequest], List[UnfurlError]]:
+    def render(self) -> Tuple[List[PlanRequest], List[PlanRequest], List[PlanRequest]]:
         if self.plan_requests is None:
             ready: Sequence[PlanRequest] = self.create_plan()
         else:
             ready = self.plan_requests[:]
 
         # run artifact job requests before render
         if self.external_requests:
@@ -658,40 +666,40 @@
             plan, count = self._plan_summary([], self.external_requests)
             logger.info(msg + "\n%s", plan, extra=dict(truncate=0))
 
         # currently external jobs are just for installing artifacts
         # we want to run these even if we just generating a plan
         self.external_jobs = self.run_external(planOnly=False)
         if self.external_jobs and self.external_jobs[-1].status == Status.error:
-            return [], [], [UnfurlError("error running job on external ensemble")]
+            return [], [], []
 
         ready, notReady, errors = do_render_requests(self, ready)
         return ready, notReady, errors
 
     @staticmethod
-    def _yield_serious_errors(errors):
-        for e in errors:
-            task = getattr(e, "task", None)  # if UnfurlTaskError
-            if not task or task.priority >= Priority.required:
-                yield e
+    def _yield_serious_errors(errors: List[PlanRequest]) -> Iterable[UnfurlTaskError]:
+        for req in errors:
+            if not req.task or req.task.priority >= Priority.required:
+                if req.render_errors:
+                    yield from req.render_errors
 
-    def _run(
+    def _run_requests(
         self,
         rendered_requests: Optional[
-            Tuple[List[PlanRequest], List[PlanRequest], List[UnfurlError]]
+            Tuple[List[PlanRequest], List[PlanRequest], List[PlanRequest]]
         ] = None,
     ) -> ResourceRef:
         if rendered_requests:
-            ready, notReady, errors = rendered_requests
+            ready, notReady, failed = rendered_requests
         else:
-            ready, notReady, errors = self.render()
+            ready, notReady, failed = self.render()
 
         self.workDone = collections.OrderedDict()
 
-        serious_errors = list(self._yield_serious_errors(errors))
+        serious_errors = list(self._yield_serious_errors(failed))
         if serious_errors:
             logger.error(
                 "Aborting job: there were errors during rendering: %s", serious_errors
             )
             return self.rootResource
 
         # XXX update_plan(ready, unfulfilled) # try to reorder so we can add to ready
@@ -722,47 +730,73 @@
                 ready, notReady = set_fulfilled_stragglers(notReady, check_target)
             logger.trace(
                 "ready %s; not ready %s; completed: %s", ready, notReady, completed
             )
 
             # the first time we render them all, after that only re-render requests if their dependencies were fulfilled
             # the last time (when completed is empty) don't have render valid dependencies as unfulfilled
-            ready, unfulfilled, errors = do_render_requests(
+            ready, unfulfilled, errored = do_render_requests(
                 self, ready, notReady, check_target
             )
+            failed.extend(errored)
             if not ready and not completed:
                 break  # none of the stragglers are ready, give up
             if unfulfilled:
                 logger.trace("marking unfulfilled as not ready %s", unfulfilled)
                 # XXX update_plan(ready, unfulfilled) # try to reorder so we can add to ready
                 notReady.extend(unfulfilled)
 
+        for req in failed:
+            if req.render_errors:
+                err_msg = str(req.render_errors[0])
+            else:
+                err_msg = "render failed"
+            self._add_unrendered_task(req, err_msg)
+
         # if there were circular dependencies or errors then notReady won't be empty
         if notReady:
             for req in get_render_requests(notReady):
                 if (
                     self.jobOptions.workflow == "deploy" and not req.include_in_plan()
                 ):  # we don't want to run these
                     continue
                 message = req.get_notready_message()
-                if req.task:
-                    req.task.logger.info(message)
-                    req.task.finished(ConfiguratorResult(False, False, result=message))
-                    self.add_work(req.task)
+                self._add_unrendered_task(req, message)
 
         # force outputs to be evaluated now and commit the changes
         # so any attributes that were evaluated computing the outputs are saved in the manifest.
         outputs = serialize_value(self.get_outputs())
         if outputs:
             logger.info("Job outputs: %s", outputs)
         if self.rootResource.attributeManager:
             self.rootResource.attributeManager.commit_changes()
         return self.rootResource
 
-    def run(self, rendered: Tuple[list, list, list]) -> None:
+    def _add_unrendered_task(self, req: PlanRequest, message: str):
+        if req.task:
+            req.task.logger.info(message)
+            req.task.finished(ConfiguratorResult(False, False, result=message))
+            self.add_work(req.task)
+
+    def _run(self, ready: List[PlanRequest], notReady: List[PlanRequest], errors: List[PlanRequest]) -> None:
+        jobOptions = self.jobOptions
+        try:
+            display.verbosity = jobOptions.verbose
+            self._run_requests((ready, notReady, errors))
+        except JobAborted as e:
+            self.local_status = Status.error  # type: ignore
+            logger.error("Aborting job: %s", e)
+        except Exception:
+            self.local_status = Status.error  # type: ignore
+            self.unexpectedAbort = UnfurlError(
+                "unexpected exception while running job", True, True
+            )
+        self._apply_workfolders()
+
+    def run(self, rendered: Tuple[List[PlanRequest], List[PlanRequest], List[PlanRequest]]) -> None:
         manifest = self.manifest
         startTime = perf_counter()
         jobOptions = self.jobOptions
         with change_cwd(manifest.get_base_dir()):
             try:
                 ready, notReady, errors = rendered
                 if not jobOptions.out:  # type: ignore
@@ -776,27 +810,15 @@
                     for repo in manifest.repositories.values():
                         if repo.is_dirty():
                             logger.error(
                                 "aborting run: uncommitted files in %s (--dirty=ok to override)",
                                 repo.working_dir,
                             )
                             return None
-                try:
-                    display.verbosity = jobOptions.verbose
-                    self._run((ready, notReady, errors))
-                except JobAborted as e:
-                    self.local_status = Status.error  # type: ignore
-                    logger.error("Aborting job: %s", e)
-                except Exception:
-                    self.local_status = Status.error  # type: ignore
-                    self.unexpectedAbort = UnfurlError(
-                        "unexpected exception while running job", True, True
-                    )
-
-                self._apply_workfolders()
+                self._run(ready, notReady, errors)
                 manifest.commit_job(self)
             finally:
                 self.timeElapsed = perf_counter() - startTime
                 manifest.unlock()
 
     def _apply_workfolders(self) -> None:
         for task in self.workDone.values():
@@ -817,17 +839,17 @@
         self.instances = self.jobOptions.instances  # type: ignore
 
     def create_plan(self) -> List[TaskRequestGroup]:
         self.validate_job_options()
         joboptions = self.jobOptions
         self._update_joboption_instances()
         self.plan_requests = []
-        WorkflowPlan = Plan.get_plan_class_for_workflow(joboptions.workflow)  # type: ignore
+        WorkflowPlan = Plan.get_plan_class_for_workflow(joboptions.workflow)
         if not WorkflowPlan:
-            raise UnfurlError(f"unknown workflow: {joboptions.workflow}")  # type: ignore
+            raise UnfurlError(f"unknown workflow: {joboptions.workflow}")
 
         if not self.jobOptions.parentJob:
             # don't do this when running a nested job
             # (planned was already removed and new tasks have already been rendered there)
             rmtree(os.path.join(self.rootResource.base_dir, Folders.Planned))
         plan = WorkflowPlan(self.rootResource, self.manifest.tosca, joboptions)
         plan_requests = list(plan.execute_plan())
@@ -917,39 +939,44 @@
         if self.jobRequestQueue:
             self.jobRequestQueue.remove(jobRequest)
         instance_specs = jobRequest.get_instance_specs()
         jobOptions = self.jobOptions.copy(parentJob=self, instances=instance_specs)
         childJob = create_job(self.manifest, jobOptions)
         childJob.set_task_id(self.increment_task_count())
         assert childJob.parentJob is self
-        childJob._run()
+        childJob._run_requests()
         return childJob
 
     def run_external(self, **opts: Any) -> List["Job"]:
         # note: manifest.lock() will raise error if there circular dependencies
         external_jobs = []
-        external_requests = self.external_requests[:]  # type: ignore
+        external_requests = self.external_requests[:] if self.external_requests else []
         while external_requests:
             manifest, requests = external_requests.pop(0)
             instance_specs = []
             for request in requests:
                 assert isinstance(
                     request, JobRequest
                 ), "only JobRequest currently supported"
                 instance_specs.extend(request.get_instance_specs())
             jobOptions = self.jobOptions.copy(
                 instances=instance_specs,
-                masterJob=self.jobOptions.masterJob or self,  # type: ignore
+                masterJob=self.jobOptions.masterJob or self,
                 **opts,
             )
+            # currently external jobs only install artifacts needed for running the job so always disable dryrun
+            jobOptions.dryrun = False
             external_job = create_job(manifest, jobOptions)
             external_jobs.append(external_job)
             rendered, count = _render(external_job)
             if not jobOptions.planOnly and count:
-                external_job.run(rendered)
+                if manifest is not self.manifest:
+                    external_job.run(rendered)
+                else:
+                    external_job._run(*rendered)
             if external_job.status == Status.error:
                 break
         return external_jobs
 
     def should_run_task(self, task: ConfigTask) -> Tuple[bool, str]:
         """
         Checked at runtime right before each task is run
@@ -1220,15 +1247,15 @@
         * Notification of creation or deletion of a resource
         * Requests a resource with requested metadata, if it doesn't exist, a task is run to make it so
         (e.g. add a dns entry, install a package).
 
         Returns a task.
         """
         task.target.root.set_attribute_manager(task._attributeManager)
-        errors: Any = None
+        errors: Optional[str] = None
         ok, errors = self.can_run_task(task)
         if not ok:
             return task.finished(ConfiguratorResult(False, False, result=errors))
 
         task.start()
         change = None
         while True:
@@ -1238,18 +1265,22 @@
                 UnfurlTaskError(task, "configurator.run failed")
                 return task.finished(ConfiguratorResult(False, None, Status.error))
             if isinstance(result, PlanRequest):
                 if depth >= self.MAX_NESTED_SUBTASKS:
                     UnfurlTaskError(task, "too many subtasks spawned")
                     change = task.finished(ConfiguratorResult(False, None))
                 else:
-                    ready, _, errors = do_render_requests(self, [result])
+                    ready, _, error_reqs = do_render_requests(self, [result])
                     if not ready:
-                        return result.task.finished(  # type: ignore
-                            ConfiguratorResult(False, False, result=errors)
+                        err_msg = "render failed"
+                        if error_reqs and error_reqs[0].render_errors:
+                            err_msg = str(error_reqs[0].render_errors[0])
+                        assert result.task
+                        return result.task.finished(
+                            ConfiguratorResult(False, False, result=err_msg)
                         )
                     change = self.apply(ready, depth + 1)
             elif isinstance(result, JobRequest):
                 job = self.run_job_request(result)
                 change = job
             elif isinstance(result, ConfiguratorResult):
                 retVal = task.finished(result)
@@ -1309,24 +1340,24 @@
 
     def _json_plan_summary(
         self, pretty: bool = False, include_rendered: bool = True
     ) -> Union[str, list]:
         return JobReporter.json_plan_summary(self, pretty, include_rendered)
 
     def json_summary(
-        self, pretty: bool = False, external: bool = False
+        self, pretty: bool = False, external: bool = False, add_rendered: bool = False
     ) -> Union[str, Dict[str, Any]]:
         job = dict(id=self.changeId, status=self.status.name)
         job.update(self.stats())  # type: ignore
         if not self.startTime:  # skip if startTime was explicitly set
             job["timeElapsed"] = self.timeElapsed  # type: ignore
         summary = dict(
             job=job,
             outputs=serialize_value(self.get_outputs()),
-            tasks=[task.summary(True) for task in self.workDone.values()],
+            tasks=[task.summary(True, add_rendered) for task in self.workDone.values()],
         )
         if external:
             summary["ensemble"] = self.manifest.path
         if self.external_jobs:
             summary["external_jobs"] = [
                 external.json_summary(external=True) for external in self.external_jobs
             ]
```

### Comparing `unfurl-0.7.1/unfurl/localenv.py` & `unfurl-0.8.0/unfurl/localenv.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 By convention, the "home" project defines a localhost instance and adds it to its context.
 """
 import os
 import os.path
 import re
 from typing import (
     Any,
+    Callable,
     Iterable,
     Dict,
     List,
     Optional,
     OrderedDict,
     Tuple,
     Union,
@@ -965,19 +966,21 @@
 
         if parent:
             self.parent = parent
             self._projects: dict = parent._projects
             self._manifests: dict = parent._manifests
             self.homeConfigPath: Optional[str] = parent.homeConfigPath
             self.homeProject: Optional[Project] = parent.homeProject
+            self.make_resolver: Optional[Callable] = parent.make_resolver
         else:
             self._projects = {}
             self._manifests = {}
             self.homeConfigPath = get_home_config_path(homePath)
             self.homeProject = self._get_home_project()
+            self.make_resolver = None
 
         self._resolve_path_and_project(manifestPath, can_be_empty)  # type: ignore
         if override_context:
             # set after _resolve_path_and_project() is called
             self.manifest_context_name = override_context
         if project:
             # this arg is used in init.py when creating a project
```

### Comparing `unfurl-0.7.1/unfurl/lock.py` & `unfurl-0.8.0/unfurl/lock.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/logs.py` & `unfurl-0.8.0/unfurl/logs.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/lookup_plugins/unfurl.py` & `unfurl-0.8.0/unfurl/lookup_plugins/unfurl.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/manifest-schema.json` & `unfurl-0.8.0/unfurl/manifest-schema.json`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/manifest.py` & `unfurl-0.8.0/unfurl/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2020 Adam Souzis
 # SPDX-License-Identifier: MIT
 from collections.abc import Mapping
 import datetime
 import os.path
 import hashlib
 import json
-from typing import Dict, List, Optional, Any, Sequence, TYPE_CHECKING, cast
+from typing import Dict, List, Optional, Any, Sequence, TYPE_CHECKING, Tuple, cast
 from ruamel.yaml.comments import CommentedMap
 
 from .tosca import EntitySpec, NodeSpec, ToscaSpec, TOSCA_VERSION, ArtifactSpec
 
 from .support import (
     ResourceChanges,
     AttributeManager,
@@ -95,77 +95,80 @@
         self.repo = self._find_repo()
         self.currentCommitId = self.repo and self.repo.revision
         # self.revisions = RevisionManager(self)
         self.changeSets: Optional[Dict[str, ChangeRecordRecord]] = None
         self.tosca = None
         self.specDigest = None
         self.repositories: Dict[str, RepoView] = {}
-        self.package_specs: Dict[str, PackageSpec] = {}
+        self.package_specs: List[PackageSpec] = []
         self.packages: PackagesType = {}
         if self.localEnv:
             # before we start parsing the manifest, add the repositories in the environment
             self._add_repositories_from_environment()
         self.imports = Imports()
         self.imports.manifest = self
         self._importedManifests: Dict = {}
         self.cache: Dict[str, Any] = {}
 
-    def _add_repositories_from_environment(self):
+    def _add_repositories_from_environment(self) -> None:
         assert self.localEnv
         context = self.localEnv.get_context()
         repositories = {}
         for key, value in relabel_dict(context, self.localEnv, "repositories").items():
             if "." in key:  # assume it's a package not a repository name
                 assert isinstance(value, dict)
-                self.package_specs[key] = PackageSpec(
+                self.package_specs.append( PackageSpec(
                     key, value.get("url"), value.get("revision")
-                )
+                ))
             else:
                 repositories[key] = value
         env_package_spec = context.get("variables", {}).get(
             "UNFURL_PACKAGE_RULES", os.getenv("UNFURL_PACKAGE_RULES")
         )
         if env_package_spec:
             for key, value in taketwo(env_package_spec.split()):
-                self.package_specs[key] = PackageSpec(key, value, None)
-        resolver = self.get_import_resolver(self)
+                self.package_specs.append( PackageSpec(key, value, None) )
+        resolver = self.get_import_resolver()
         for name, tpl in repositories.items():
             toscaRepository = resolver.get_repository(name, tpl)
             self.repositories[name] = RepoView(toscaRepository, None)
 
-    def _set_spec(self, spec, more_spec=None, skip_validation=False):
+    def _set_spec(self, spec, more_spec=None, skip_validation=False, fragment=""):
         """
         Set the TOSCA service template.
         """
         repositories = {
             name: repo.repository.tpl for name, repo in self.repositories.items()
         }
         self.tosca = self._load_spec(
-            spec, self.path, repositories, more_spec, skip_validation
+            spec, self.path, repositories, more_spec, skip_validation, fragment
         )
         self.specDigest = self.get_spec_digest(spec)
 
     def _find_repo(self) -> Optional["GitRepo"]:
         # check if this path exists in the repo
         repo = self.localEnv and self.localEnv.instanceRepo
         if repo:
             # this check is expensive and not that important so skip
             return repo
             # path = repo.find_path(self.path)[0]
             # if path and (path, 0) in repo.repo.index.entries:
             #     return repo
         return None
 
-    def _load_spec(self, spec, path, repositories, more_spec, skip_validation=False):
+    def _load_spec(self, spec, path, repositories, more_spec, skip_validation, fragment):
         if "service_template" in spec:
             toscaDef = spec["service_template"] or {}
+            fragment += "/service_template"
         elif "tosca" in spec:  # backward compat
             toscaDef = spec["tosca"] or {}
+            fragment += "/tosca"
         else:
             toscaDef = {}
+            fragment = ""
 
         repositoriesTpl = toscaDef.setdefault("repositories", CommentedMap())
         for name, value in repositories.items():
             if name not in repositoriesTpl:
                 repositoriesTpl[name] = value
 
         # make sure this is present
@@ -183,15 +186,15 @@
             toscaDef = yaml_dict_cls(toscaDef.items())
         if getattr(toscaDef, "base_dir", None) and (
             not path or toscaDef.base_dir != os.path.dirname(path)
         ):
             # note: we only recorded the baseDir not the name of the included file
             path = toscaDef.base_dir
         return ToscaSpec(
-            toscaDef, spec, path, self.get_import_resolver(expand=True), skip_validation
+            toscaDef, spec, path, self.get_import_resolver(expand=True), skip_validation, fragment
         )
 
     def get_spec_digest(self, spec):
         m = hashlib.sha1()  # use same digest function as git
         assert self.tosca
         t = self.tosca.template
         for tpl in [spec, t.topology_template.custom_defs, t.nested_tosca_tpls]:
@@ -580,15 +583,15 @@
         return repository
 
     def _update_repositories(
         self, config, inlineRepositories=None, resolver: Optional[ImportResolver] = None
     ) -> Dict[str, dict]:
         # Called during parse time when including files
         if not resolver:
-            resolver = self.get_import_resolver(self)
+            resolver = self.get_import_resolver()
         # we need to fetch this every call since the config might have changed:
         repositories = self._get_repositories(config)
         for name, tpl in repositories.items():
             # only set if we haven't seen this repository before
             if name not in self.repositories:
                 toscaRepository = resolver.get_repository(name, tpl)
                 self.repositories[name] = RepoView(toscaRepository, None)
@@ -645,23 +648,24 @@
         if self.localEnv and self.localEnv.project:
             if self.localEnv.project is self.localEnv.homeProject:
                 inProject = self.localEnv.project.projectRoot in self.path  # type: ignore
             else:
                 inProject = True
         if inProject and "project" not in repositories:
             repositories["project"] = self.localEnv.project.project_repoview  # type: ignore
+            repositories["project"].package = False
 
         if "spec" not in repositories:
             # if not found assume it points the project root or self if not in a project
             if inProject:
                 assert self.localEnv and self.localEnv.project
                 repositories["spec"] = self.localEnv.project.project_repoview  # type: ignore
             else:
                 repositories["spec"] = repositories["self"]
-        repositories["spec"].package = False
+            repositories["spec"].package = False
         return {name: repo.repository.tpl for name, repo in self.repositories.items()}
 
     def load_yaml_include(
         self,
         yamlConfig,
         templatePath,
         baseDir,
@@ -709,33 +713,40 @@
                 return "", None
             raise UnfurlError(msg)
 
         resolver = self.get_import_resolver(warnWhenNotFound, config=expanded)
         repositories = self._update_repositories(
             expanded or yamlConfig.config, inlineRepository, resolver
         )
+        if self.localEnv and self.localEnv.project:
+            repository_root = self.localEnv.project.projectRoot
+        else:
+            repository_root=self.get_base_dir()
         loader = toscaparser.imports.ImportsLoader(
             None,
             get_base_dir(baseDir),
             repositories=repositories,
             resolver=resolver,
+            repository_root=repository_root
         )
         import_spec = dict(
             file=artifactTpl["file"], repository=artifactTpl.get("repository")
         )
-        path, doc = loader.load_yaml(import_spec)
+        base, path, doc = loader.load_yaml(import_spec)
         if doc is None:
             logger.warning(
                 f"document include {templatePath} does not exist (base: {baseDir})"
             )
         return path, doc
 
     def get_import_resolver(
-        self, ignoreFileNotFound=False, expand=False, config=None
+        self, ignoreFileNotFound: bool=False, expand: bool=False, config: Optional[dict]=None
     ) -> ImportResolver:
+        if self.localEnv and self.localEnv.make_resolver:
+            return self.localEnv.make_resolver(self, ignoreFileNotFound, expand, config)
         return SimpleCacheResolver(self, ignoreFileNotFound, expand, config)
 
     def last_commit_time(self) -> Optional[datetime.datetime]:
         # return seconds (0 if not found)
         repo = self.repo
         if not repo:
             return None
```

### Comparing `unfurl-0.7.1/unfurl/merge.py` & `unfurl-0.8.0/unfurl/merge.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/packages.py` & `unfurl-0.8.0/unfurl/packages.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,18 +30,17 @@
 
 ```
 environments:
   defaults:
     repositories:
       # set the repository URL and optionally the version for the given package
       unfurl.cloud/onecommons/blueprints/wordpress:
-        url: https://unfurl.cloud/user/repo.git#main # choose an explicit repository and revision or replace with another package?
-        revision: 1.2.15 # (optional) pin explicit revision for this package
+        url: https://unfurl.cloud/user/repo.git#main # set the package to a specific repository url that also sets the branch
 
-      # replace a package with another
+      # if url is set to a package identifier, replace a package with another
       unfurl.cloud/onecommons/unfurl-types:
         url: github.com/user1/myfork
 
       # A trailing * applies the rule to all packages that match
       unfurl.cloud/onecommons/*:
           url: https://staging.unfurl.cloud/onecommons/*
       
@@ -50,26 +49,29 @@
         url: github.com/user1/myforks.git/ghost
         revision: 1.6.1 # e.g. a security patch
 ```
 
 You can also set these rules in ``UNFURL_PACKAGE_RULES`` environment variable where the key value pairs are separated by spaces. This example defines two rules:
 
 ```UNFURL_PACKAGE_RULES="unfurl.cloud/onecommons/* #main unfurl.cloud/onecommons/unfurl-types github.com/user1/myfork"```
+
+The first rule sets the revision of matching packages to the branch "main", the second replaces one package with another package.
 """
 import re
-from typing import Dict, List, NamedTuple, Optional, Union, cast
+from typing import Dict, List, NamedTuple, Optional, Tuple, Union, cast
 from typing_extensions import Literal
 from urllib.parse import urlparse
-from .repo import RepoView, is_url_or_git_path, split_git_url, get_remote_tags
+from .repo import RepoView, split_git_url, get_remote_tags
 from .logs import getLogger
 from .util import UnfurlError
 from toscaparser.utils.validateutils import TOSCAVersionProperty
 
 logger = getLogger("unfurl")
 
+
 class UnfurlPackageUpdateNeeded(UnfurlError):
     pass
 
 
 def is_semver(revision: Optional[str], include_unreleased=False) -> bool:
     """Return true if ``revision`` looks like a semver with major version >= 1"""
     return bool(
@@ -95,21 +97,30 @@
             self.package_id, self.url, revision = get_package_id_from_url(url)
         else:
             self.url = None
             self.package_id = None
             revision = None
         self.revision = minimum_version or revision
         self.lock_to_commit: str = ""
+        if ":" in self.package_spec or "#" in self.package_spec:
+            raise UnfurlError(
+                f"Malformed package spec: {self.package_spec} must be a package id not an URL"
+            )
+        if not (self.url or self.package_id or self.revision):
+            raise UnfurlError(
+                f"Malformed package spec: {self.package_spec}: missing url or package id"
+            )
 
-    def __str__(self):
+    def __repr__(self):
         return f"PackageSpec({self.package_spec}:{self.package_id} {self.revision} {self.url})"
 
     def matches(self, package: "Package") -> bool:
         # * use the package name (or prefix) as the name of the repository to specify replacement or name resolution
         candidate = package.package_id
+        # print("match", candidate, self.package_spec, candidate.startswith(self.package_spec.rstrip("*")))
         if self.package_spec.endswith("*"):
             return candidate.startswith(self.package_spec.rstrip("*"))
         elif "#" in self.package_spec:
             package_id, revision = self.package_spec.split("#")
             # match exact match with package and revision
             return candidate == package_id and revision == package.revision
         else:
@@ -118,14 +129,18 @@
     def update(self, package: "Package") -> str:
         # if the package's package_id was replaced return that
         if self.package_spec.endswith("*"):
             if self.url:
                 package.url = self.url.replace(
                     "*", package.package_id[len(self.package_spec) - 1 :]
                 )
+                if self.revision:
+                    package.revision = self.revision
+                    # PackageSpec.url used above will always have revision stripped off
+                    package.url = package.url + "#" + package.revision_tag
                 return ""
             elif self.package_id:
                 replaced_id = package.package_id
                 package.package_id = self.package_id.replace(
                     "*", package.package_id[len(self.package_spec) - 1 :]
                 )
                 package.url = ""
@@ -151,62 +166,68 @@
             replaced_id = package.package_id
             if replaced_id != self.package_id:
                 package.package_id = self.package_id
                 return replaced_id
         return ""
 
     @staticmethod
-    def update_package(
-        package_specs: Dict[str, "PackageSpec"], package: "Package"
-    ) -> bool:
+    def update_package(package_specs: List["PackageSpec"], package: "Package") -> bool:
         """_summary_
 
         Args:
             package_specs (PackageSpec): Rules to apply to the package.
             package (Package): Package will be updated in-place if there are rules that apply to it.
 
         Raises:
             UnfurlError: If applying the rules creates a circular reference.
 
         Returns:
             bool: True if the package was updated
         """
         old = []
-        while True:
-            for pkg_spec in package_specs.values():
+        changed = False
+        replaced = True
+        # if the package_id changes, start over
+        while replaced:
+            replaced = False
+            for pkg_spec in package_specs:
                 if pkg_spec.matches(package):
                     replaced_id = pkg_spec.update(package)
                     logger.trace(
-                        "updated package %s using rule %s: replaced %s",
+                        "updated package %s using rule %s: old package_id was %s",
                         package,
                         pkg_spec,
                         replaced_id,
                     )
+                    changed = True
                     if not replaced_id:
+                        # same package_id, only url or revision changed
+                        # if not package.url:
+                        #    # use default url pattern for the package_id
                         if not package.url:
-                            # use default url pattern for the package_id
                             package.set_url_from_package_id()
-                        return True  # we're done
+                        continue
                     if replaced_id in old:
                         raise UnfurlError(
                             f"Circular reference in package rules: {replaced_id}"
                         )
+                    replaced = True
                     old.append(replaced_id)
                     break  # package_id replaced start over
             else:
-                # no matches found, we're done
+                # package_id wasn't replaced, make sure url is set
                 if not package.url:
                     # use default url pattern for the package_id
                     package.set_url_from_package_id()
-                return bool(old)
+        return changed
 
 
 def get_package_id_from_url(url: str) -> Package_Url_Info:
-    if url.startswith(".") or url.startswith("file:"):
-        # this isn't a package id or a git url
+    if url.startswith(".") or url.startswith("file:") or url.startswith("git-local"):
+        # this isn't a package id or a non-local git url
         return Package_Url_Info(None, url, None)
 
     # package_ids can have a revision in the fragment
     url, repopath, revision = split_git_url(url)
     parts = urlparse(url)
     path = parts.path.strip("/")
     if path.endswith(".git"):
@@ -235,25 +256,27 @@
 def get_package_from_url(url_: str):
     package_id, url, revision = get_package_id_from_url(url_)
     if package_id is None:
         return None
     return Package(package_id, url, revision)
 
 
-def get_url_with_latest_revision(url: str) -> str:
+def get_url_with_latest_revision(url: str, get_remote_tags=get_remote_tags) -> str:
     pkg = get_package_from_url(url)
     if not pkg:
         return url
-    pkg.set_version_from_repo()
+    pkg.set_version_from_repo(get_remote_tags)
     pkg.set_url_from_package_id()
     return pkg.url
 
 
 class Package:
-    def __init__(self, package_id: str, url: Optional[str], minimum_version: Optional[str]):
+    def __init__(
+        self, package_id: str, url: Optional[str], minimum_version: Optional[str]
+    ):
         self.package_id = package_id
         self.revision = minimum_version
         if url is None:
             self.set_url_from_package_id()
         self.url = cast(str, url)
         self.repositories: List[RepoView] = []
         self.discovered_revision = False
@@ -268,31 +291,42 @@
         # return tag prefix to match version tags with
         if repopath:
             # strip out major version suffix:
             # if repopath looks "foo" or "foo/v2", return "foo/v"
             return re.sub(r"(/v\d+)?$", "", repopath) + "/v"
         return "v"
 
-    def find_latest_semver_from_repo(self) -> Optional[str]:
+    def find_latest_semver_from_repo(self, get_remote_tags) -> Optional[str]:
         prefix = self.version_tag_prefix()
+        logger.debug(
+            f"looking for remote tags {prefix}* for {self.url} using {get_remote_tags}"
+        )
         # get an sorted list of tags and strip the prefix from them
-        vtags = [tag[len(prefix) :] for tag in get_remote_tags(self.url, prefix + "*")]
+        url, repopath, urlrevision = split_git_url(self.url)
+        vtags = [tag[len(prefix) :] for tag in get_remote_tags(url, prefix + "*")]
         # only include tags look like a semver with major version of 1 or higher
         # (We exclude unreleased versions because we want to treat the repository
         # as if it didn't specify a semver at all. Unrelease versions have no backwards compatibility
         # guarantees so we don't want to treat the repository as pinned to a particular revision.
         tags = [vtag for vtag in vtags if is_semver(vtag, True)]
         if tags:
             return tags[0]
         return None
 
-    def set_version_from_repo(self):
-        self.revision = self.find_latest_semver_from_repo()
+    def set_version_from_repo(self, get_remote_tags) -> bool:
+        revision = self.find_latest_semver_from_repo(get_remote_tags)
         # set flag to indicate the revision wasn't explicitly specified
-        self.discovered_revision = True
+        if revision != self.revision:
+            # e.g. if no revision was specified and there are no version tags, don't set discovered_revision
+            # so the package continues to rely on the default branch, not future tags
+            self.revision = revision
+            self.discovered_revision = True
+            return True
+        else:
+            return False
 
     def set_url_from_package_id(self):
         self.url = package_id_to_url(self.package_id, self.revision_tag)
 
     @property
     def revision_tag(self) -> str:
         if not self.revision:
@@ -303,26 +337,27 @@
             # since "^v" is in the semver regex, make sure don't end up with "vv"
             return self.version_tag_prefix() + self.revision.lstrip("v")
 
     def is_mutable_ref(self) -> bool:
         # is this package pointing to ref that could change?
         return not self.lock_to_commit
         # XXX if revision, see if its tag or branch
+        # if self.discovered_revision: return True
         # treat tags immutable unless it looks like a non-exact semver tag:
         # return not self.revision or self.has_semver() or self.revision_is_branch()
 
     def add_reference(self, repoview: RepoView) -> bool:
         if repoview not in self.repositories:
             self.repositories.append(repoview)
             repoview.package = self
             # we need to set the path, url, and revision to match the package
             if self.revision:
                 url, repopath, urlrevision = split_git_url(self.url)
                 repoview.path = repopath
-                repoview.revision = self.revision
+                repoview.revision = self.revision_tag
                 repoview.repository.url = f"{url}#{self.revision_tag}:{repopath}"
             else:
                 repoview.repository.url = self.url
             return True
         return False
 
     def has_semver(self, include_unreleased=False) -> bool:
@@ -353,15 +388,18 @@
         )
 
 
 PackagesType = Dict[str, Union[Literal[False], Package]]
 
 
 def resolve_package(
-    repoview: RepoView, packages: PackagesType, package_specs: Dict[str, PackageSpec]
+    repoview: RepoView,
+    packages: PackagesType,
+    package_specs: List[PackageSpec],
+    get_remote_tags=get_remote_tags,
 ) -> Optional["Package"]:
     """
     If repository references a package, register it with existing package or create a new one.
     A error is raised if a package's version conficts with the repository's version requirement.
     """
     package_id, url, revision = get_package_id_from_url(repoview.url)
     if not package_id:
@@ -377,15 +415,15 @@
         if not package.url:
             # the repository didn't specify a full url and there wasn't already an existing package or package spec
             raise UnfurlError(
                 f'Could not find a repository that matched package "{package.package_id}"'
             )
         if not package.revision:
             # no version specified, use the latest version tagged in the repository
-            package.set_version_from_repo()
+            package.set_version_from_repo(get_remote_tags)
         if not changed and not package.revision:
             # don't treat repository as a package
             repoview.package = False
             packages[package.package_id] = False
             return None
         packages[package_id] = package
     else:
```

### Comparing `unfurl-0.7.1/unfurl/plan.py` & `unfurl-0.8.0/unfurl/plan.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/planrequests.py` & `unfurl-0.8.0/unfurl/planrequests.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,22 @@
     Union,
     cast,
 )
 import shlex
 import sys
 import os
 import os.path
-
+from toscaparser.elements.interfaces import OperationDef
 from toscaparser.nodetemplate import NodeTemplate
 from .tosca import EntitySpec
 
 if TYPE_CHECKING:
     from .job import Job, ConfigTask, JobOptions
     from .configurator import Dependency
+    from .manifest import Manifest
 
 from .util import (
     lookup_class,
     load_module,
     find_schema_errors,
     UnfurlError,
     UnfurlTaskError,
@@ -747,15 +748,15 @@
             ready.append(req)
             continue
         # found one, so not ready
         notReady.append(req)
     return ready, notReady
 
 
-def _prepare_request(job: "Job", req: PlanRequest, errors: List) -> bool:
+def _prepare_request(job: "Job", req: PlanRequest, errors: List[PlanRequest]) -> bool:
     if not isinstance(req, TaskRequest):
         return True
     if req.task:
         task = req.task
         task._attributeManager.attributes = {}
         task.target.root.set_attribute_manager(task._attributeManager)
     else:
@@ -783,17 +784,17 @@
     except Exception:
         proceed = False
         # note: failed rendering may be re-tried later if it has dependencies
         error = UnfurlTaskError(task, "should_run_task failed", logging.DEBUG)
     finally:
         task.restore_envvars()
     if error:
+        errors.append(req)
         task._reset()
         task._attributeManager.attributes = {}  # rollback changes
-        errors.append(error)
     else:
         task.commit_changes()
     return proceed
 
 
 def _render_request(
     job: "Job",
@@ -886,18 +887,18 @@
 
 
 def do_render_requests(
     job,
     requests: Sequence[PlanRequest],
     future_requests: List[PlanRequest] = [],
     check_target: str = "",
-) -> Tuple[List[PlanRequest], List[PlanRequest], List[UnfurlError]]:
+) -> Tuple[List[PlanRequest], List[PlanRequest], List[PlanRequest]]:
     ready: List[PlanRequest] = []
     notReady: List[PlanRequest] = []
-    errors: List[UnfurlError] = []
+    errors: List[PlanRequest] = []
     flattened_requests = list(
         r for r in get_render_requests(requests) if _prepare_request(job, r, errors)
     )
     not_required: List[PlanRequest] = []
     render_requests = collections.deque(flattened_requests)
 
     notready_group = None
@@ -923,15 +924,15 @@
                 # i.e (for now): a setstate request
                 _add_to_req_list(ready, request)
                 continue
             deps, error = _render_request(
                 job, request, flattened_requests + future_requests, check_target
             )
             if error:
-                errors.append(error)
+                errors.append(request)
             elif deps:
                 notready_group = request.group
                 _add_to_req_list(notReady, request)
             else:
                 _add_to_req_list(ready, request)
             not_required = _reevaluate_not_required(not_required, render_requests)
 
@@ -964,15 +965,15 @@
             filterReason,
         )
         return None  # treat as filtered step
 
     return req
 
 
-def _find_implementation(interface: str, operation: str, template: EntitySpec):
+def _find_implementation(interface: str, operation: str, template: EntitySpec) -> Optional[OperationDef]:
     default = None
     for iDef in template.get_interfaces():
         if iDef.interfacename == interface or iDef.type == interface:
             if iDef.name == operation:
                 return iDef
     return default
 
@@ -1006,15 +1007,15 @@
         # XXX need to evaluate matches
         return parent
     raise UnfurlError(
         f"could not find parent instance {parentTemplate.name} for child {source.name}"
     )
 
 
-def create_instance_from_spec(_manifest, target: EntityInstance, rname: str, resourceSpec):
+def create_instance_from_spec(_manifest: "Manifest", target: EntityInstance, rname: str, resourceSpec):
     pname = resourceSpec.get("parent")
     # get the actual parent if pname is a reserved name:
     if pname in [".self", "SELF"]:
         resourceSpec["parent"] = target.name
     elif pname == "HOST":
         if target.parent:
             resourceSpec["parent"] = target.parent.name
@@ -1083,31 +1084,34 @@
 ):
     """implementation can either be a named artifact (including a python configurator class),
     or a file path"""
     interface, sep, action = operation.rpartition(".")
     iDef = _find_implementation(interface, action, resource.template)
     if iDef and iDef.name != "default":
         iDef = _maybe_mock(iDef, resource.template)
+        assert iDef
         # merge inputs
         if inputs:
-            inputs = dict(iDef.inputs, **inputs)
+            cls = getattr(iDef.inputs, "mapCtor", iDef.inputs.__class__)
+            inputs = cls(iDef.inputs, **inputs)
         else:
             inputs = iDef.inputs or {}
         if iDef.invoke:
             # get the implementation from the operation specified with the "invoke" key
             iinterface, sep, iaction = iDef.invoke.rpartition(".")
             iDef = _find_implementation(iinterface, iaction, resource.template)
-            inputs = dict(iDef.inputs, **inputs)
+            if iDef:
+                cls = getattr(iDef.inputs, "mapCtor", iDef.inputs.__class__)
+                inputs = cls(iDef.inputs, **inputs)
 
+    kw = None
+    if iDef:
         kw = _get_config_spec_args_from_implementation(
             iDef, inputs, resource, operation_host
         )
-    else:
-        kw = None
-
     if kw:
         kw["interface"] = interface
         if reason:
             name = f"for {reason}: {interface}.{action}"
             if reason == jobOptions.workflow:
                 # set the task's workflow instead of using the default ("deploy")
                 kw["workflow"] = reason
@@ -1215,15 +1219,15 @@
         return set_default_command(kw, guessing)
     else:
         # error couldn't resolve className
         logger.warning("could not find configurator class: %s", className)
         return None
 
 
-def _get_config_spec_args_from_implementation(iDef, inputs, target, operation_host):
+def _get_config_spec_args_from_implementation(iDef: OperationDef, inputs, target, operation_host):
     implementation = iDef.implementation
     kw = dict(
         inputs=inputs,
         outputs=iDef.outputs,
         operation_host=operation_host,
         entry_state=iDef.entry_state,
     )
```

### Comparing `unfurl-0.7.1/unfurl/projectpaths.py` & `unfurl-0.8.0/unfurl/projectpaths.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,17 +121,18 @@
     Updates to these directories through this class are performed transactionally --
     accessing a directory through this class marks it for writing and creates a
     copy of it in the ``planning`` directory.
 
     If a task completes successfully ``apply()`` is called, which copies it back to the
     permanent location of the folder.
     """
+
     always_apply = False
 
-    def __init__(self, task, location, preserve):
+    def __init__(self, task, location: str, preserve: bool):
         self.task = task  # owner
         self.pending_state = True
         self.location = location
         self.preserve = preserve
         # the permanent location:
         self._active = self._get_job_path(task, location, Folders.Active).rstrip(os.sep)
         self._pending = self._get_job_path(task, location, Folders.Planned).rstrip(
@@ -200,18 +201,20 @@
             # don't encrypt files that arent' being commited to the repo
             # or already going to be encrypted (i.e. the secrets folders)
             yaml = cleartext_yaml
         write_file(ctx, contents, path, self.location, encoding, yaml=yaml)
         return path
 
     @staticmethod
-    def _get_job_path(task, name, pending):
+    def _get_job_path(task, name: str, pending: str):
         instance = task.target
         if name in [Folders.artifacts, Folders.secrets, Folders.local, Folders.tasks]:
-            return os.path.join(instance.base_dir, pending, name, _get_instance_dir_name(instance))
+            return os.path.join(
+                instance.base_dir, pending, name, _get_instance_dir_name(instance)
+            )
         elif name == Folders.operation:
             return os.path.join(
                 instance.base_dir,
                 pending,
                 "tasks",
                 _get_instance_dir_name(instance),
                 task.configSpec.operation,
@@ -221,15 +224,17 @@
                 instance.base_dir,
                 pending,
                 "tasks",
                 _get_instance_dir_name(instance),
                 task.configSpec.workflow,
             )
         elif name == Folders.tasks:
-            return os.path.join(instance.base_dir, pending, "tasks", _get_instance_dir_name(instance))
+            return os.path.join(
+                instance.base_dir, pending, "tasks", _get_instance_dir_name(instance)
+            )
         else:
             assert False, f"unexpected name '{name}' for workfolder"
 
     def _start(self):
         # create the .pending folder
         pendingpath = self._pending
         if self.preserve and os.path.exists(self._active):
@@ -240,45 +245,50 @@
         self.task.logger.trace(
             'created pending project path "%s" for %s',
             pendingpath,
             self.task.target.name,
         )
         return pendingpath
 
-    def apply(self):
+    def apply(self) -> str:
         # save_as_previous = False
         pendingpath = self._pending
+        renamed_path = ""
         if os.path.exists(pendingpath):
             if os.path.exists(self._active):
                 # if save_as_previous:
                 #     previouspath = self._get_job_path(
                 #         self.task, self.location, self.PREVIOUS_EXT
                 #     )
                 #     if os.path.exists(previouspath):
                 #         self._rmtree(previouspath)
                 #     # rename the current version as previous
                 #     self._rename_dir(self._active, previouspath)
                 # else:
                 self._rmtree(self._active)
             # rename the pending version as the current one
             self._rename_dir(pendingpath, self._active)
+            renamed_path = self._active
         self.pending_state = False
+        return renamed_path
 
-    def discard(self):
+    def discard(self) -> None:
         pendingpath = self._pending
         if os.path.exists(pendingpath):
             self._rmtree(pendingpath)
 
-    def failed(self):
+    def failed(self) -> str:
         pendingpath = self._pending
+        errorpath = ""
         if os.path.exists(pendingpath):
             error_dir = "failed." + self.task.changeId
             errorpath = self._get_job_path(self.task, self.location, error_dir)
             self._rename_dir(pendingpath, errorpath)
         self.pending_state = False
+        return errorpath
 
     def _rename_dir(self, src, dst):
         return rename_dir(src, dst, self.task.logger)
 
     def _rmtree(self, path):
         return rmtree(path, self.task.logger)
 
@@ -552,15 +562,15 @@
     :spec.home: Directory unique to the current instance's TOSCA template (committed to the spec repository).
     :spec.local: Local directory unique to the current instance's TOSCA template (excluded from repository).
     :project: The root directory of the current project.
     :unfurl.home: The location of home project (UNFURL_HOME).
 
     Otherwise look for a repository with the given name and return its path or None if not found.
     """
-    
+
     instance = ctx.currentResource
     spec = instance.template and instance.template.spec
     if not name or name == ".":
         # the folder of the current resource's ensemble
         return instance.base_dir
     elif name == "src":
         # folder of the source file
```

### Comparing `unfurl-0.7.1/unfurl/repo.py` & `unfurl-0.8.0/unfurl/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,17 @@
         parts = urlparse(url)
         # remove password and .git
         user, sep, host = parts.netloc.rpartition("@")
         if sep and hard == 1:
             netloc = f"{user.partition(':')[0]}@{host}"
         else:  # hard >= 2
             netloc = host
-        if hard == 3 and parts.path.endswith(".git"):
-            path = parts.path[:-4]
-        else:
-            path = parts.path
+        path = parts.path.rstrip("/")
+        if hard == 3 and path.endswith(".git"):
+            path = path[:-4]
         return parts._replace(netloc=netloc, path=path).geturl()
     return url
 
 
 def sanitize_url(url: str, redact=True) -> str:
     if "://" in url and "@" in url:  # sanitize
         parts = urlparse(url)
@@ -137,28 +136,32 @@
         # e.g. myrepo.git#mybranch, myrepo.git#pull/42/head, myrepo.git#:myfolder, myrepo.git#master:myfolder
         revision, sep, path = parts.fragment.partition(":")
         giturl, sep, frag = url.partition("#")
         return giturl, path, revision
     return url, "", ""
 
 
+@lru_cache(None)
+def memoized_remote_tags(url, pattern="*") -> List[str]:
+    return get_remote_tags(url, pattern)
+
+
 # git fetch <remote> 'refs/tags/*:refs/tags/*' if our clones are shallow
-@lru_cache(None)  # XXX won't get up dates in server mode
 def get_remote_tags(url, pattern="*") -> List[str]:
     # https://github.com/gitpython-developers/GitPython/issues/1071
     # https://myshittycode.com/2020/10/02/git-querying-tags-without-cloning-the-repository/
     # -v:refname is version sort in reverse order
     # -c versionsort.suffix=- ensures 1.0.0-XXXXXX comes before 1.0.0.
     blob = git.cmd.Git()(c="versionsort.suffix=-").ls_remote(
         url, pattern, sort="-v:refname", tags=True
     )
     # len("b90df3d12413db22d051db1f7c7286cdd2f00b66\trefs/tags/") == 51
     # filter out ^{} references (see https://stackoverflow.com/questions/12938972/what-does-mean-in-git)
     tags = [line[51:] for line in blob.split("\n") if not line.endswith("^{}")]
-    logger.debug("got %s remote tags with pattern %s from %s", len(tags), pattern, url)
+    logger.debug("got %s remote tags with pattern %s from %s", len(tags), pattern, sanitize_url(url))
     return tags
 
 
 class _ProgressPrinter(git.RemoteProgress):
     gitUrl = ""
 
     def update(self, op_code, cur_count, max_count=None, message=""):
@@ -235,15 +238,15 @@
         if localPath is not None and not self.is_path_excluded(localPath):
             return localPath
         return None
 
     def is_path_excluded(self, localPath):
         return False
 
-    def find_path(self, path, importLoader=None):
+    def find_path(self, path: str, importLoader=None):
         base = self.working_dir
         if not base:  # XXX support bare repos
             return None, None, None
         repoRoot = os.path.abspath(base)
         abspath = os.path.abspath(path).rstrip("/")
         if repoRoot in abspath:
             # XXX find pinned
@@ -277,42 +280,54 @@
         assert not name.endswith(".git"), name
         return name
 
     def project_path(self) -> str:
         return self.get_path_for_git_repo(self.url, False)
 
     @classmethod
-    def create_working_dir(cls, gitUrl, localRepoPath, revision=None, depth=1):
+    def create_working_dir(
+        cls, gitUrl, localRepoPath, revision=None, depth=1, username=None, password=None
+    ):
         localRepoPath = localRepoPath or "."
         if os.path.exists(localRepoPath):
             if not os.path.isdir(localRepoPath) or os.listdir(localRepoPath):
                 raise UnfurlError(
                     f"couldn't create directory, it already exists and isn't empty: {localRepoPath}"
                 )
         parent_dir = os.path.dirname(localRepoPath)
         if parent_dir.strip("/"):
             os.makedirs(parent_dir, exist_ok=True)
         cleanurl = sanitize_url(gitUrl)
         logger.info("Fetching %s %s to %s", cleanurl, revision or "", localRepoPath)
         kwargs: Dict[str, Any] = dict(recurse_submodules=True, no_single_branch=True)
-        if depth == 1:
+        if depth:
             kwargs["depth"] = depth
             kwargs["shallow_submodules"] = True
         non_interactive = (
             os.getenv("CI") or not PY_COLORS
         )  # if CI or color output disabled
         if not non_interactive:
             # we're running in an interactive session
             progress = _ProgressPrinter()
             progress.gitUrl = cleanurl
             kwargs["progress"] = progress  # type: ignore
         try:
             if revision:
                 kwargs["branch"] = revision
-            repo = git.Repo.clone_from(gitUrl, localRepoPath, **kwargs)  # type: ignore
+            # equivalent to git.Repo.clone_from() with add_transient_credentials() added
+            gitcmd = git.Repo.GitCommandWrapperType(os.getcwd())
+            if username:
+                add_transient_credentials(gitcmd, gitUrl, username, password)
+            repo = git.Repo._clone(
+                gitcmd,
+                gitUrl,
+                localRepoPath,
+                git.GitCmdObjectDB,
+                **kwargs,
+            )
         except git.exc.GitCommandError as err:  # type: ignore
             raise UnfurlError(
                 f'couldn\'t create working directory, clone failed: "{err._cmdline}"\nTry re-running that command to diagnose the problem.'
             )
         Repo.ignore_dir(localRepoPath)
         return GitRepo(repo)
 
@@ -401,14 +416,18 @@
                 return add_user_to_url(url, credential["user"], credential["token"])
             else:
                 return url
         else:
             assert self.repo
             return self.repo.url
 
+    def has_credentials(self):
+        parts = urlparse(self.url)
+        return "@" in parts.netloc
+
     def as_git_url(self, sanitize=False) -> str:
         hard = 2 if sanitize else 0
         url, path, revision = split_git_url(self.url)
         if self.package:
             revision = self.package.revision_tag
         else:
             revision = self.revision or ""
@@ -497,15 +516,17 @@
         return self.repo.run_cmd(["status", self.path or "."])[1]
 
     def _secrets_status(self):
         assert self.repo
         modified = "\n   ".join(
             [
                 str(filepath.relative_to(self.repo.working_dir))
-                for filepath, dotsecrets in find_dirty_secrets(self.working_dir, self.repo)
+                for filepath, dotsecrets in find_dirty_secrets(
+                    self.working_dir, self.repo
+                )
             ]
         )
         if modified:
             return f"\n\nSecrets to be committed:\n   {modified}"
         return ""
 
     def get_repo_status(self, dirty=False):
@@ -553,35 +574,39 @@
         if self.name:
             record["name"] = self.name
         if self.origin:
             record["origin"] = normalize_git_url(self.origin, 1)
         return record
 
 
+def add_transient_credentials(git, url, username, password):
+    transient_url = add_user_to_url(url, username, password)
+    replacement = f'url."{transient_url}".insteadOf="{url}"'
+    # _git_options get cleared after next git command is issued
+    git._git_options = git.transform_kwargs(
+        split_single_char_options=True, c=replacement
+    )
+
+
 class GitRepo(Repo):
     def __init__(self, gitrepo: git.Repo):
         self.repo = gitrepo
         self.url = self.working_dir or str(gitrepo.git_dir)
         remote = self.remote
         if remote:
             # note: these might not look like absolute urls, e.g. git@github.com:onecommons/unfurl.git
             self.url = remote.url
         self.push_url: Optional[str] = None
 
     def add_transient_push_credentials(self, username, password):
         if not self.remote:
             return
-        url = add_user_to_url(self.url, username, password)
         if self.push_url is None:
             self.push_url = self.repo.git.remote("get-url", "--push", self.remote.name)
-        replacement = f'url."{url}".insteadOf="{self.push_url}"'
-        # _git_options get cleared after next git command is issued
-        self.repo.git._git_options = self.repo.git.transform_kwargs(
-            split_single_char_options=True, c=replacement
-        )
+        add_transient_credentials(self.repo.git, self.push_url, username, password)
 
     def set_url_credentials(
         self, username: str, password: str, fetch_only=False
     ) -> None:
         remote = self.remote
         if remote:
             if username or password:
@@ -694,18 +719,19 @@
           tuple(int(status), str(stdout), str(stderr))
         """
         gitcmd = self.repo.git
         call: List[str] = [gitcmd.GIT_PYTHON_GIT_EXECUTABLE or "git"]
         # add persistent git options
         call.extend(gitcmd._persistent_git_options)
         call.extend(list(args))
+        call.extend(gitcmd.transform_kwargs(**kw))
 
         # note: sets cwd to working_dir
         return gitcmd.execute(  # type: ignore
-            call, with_exceptions=with_exceptions, with_extended_output=True, **kw
+            call, with_exceptions=with_exceptions, with_extended_output=True
         )
 
     def add_to_local_git_ignore(self, rule):
         path = os.path.join(self.repo.git_dir, "info")
         if not os.path.exists(path):
             os.makedirs(path)
         exclude_path = os.path.join(path, "exclude")
```

### Comparing `unfurl-0.7.1/unfurl/reporting.py` & `unfurl-0.8.0/unfurl/reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,15 @@
         console = getConsole(record=True)
         if not job.workDone:
             console.print(
                 f"Job {job.changeId} completed: [{job.status.color}]{job.status.name}[/]. No tasks ran."
             )
             return console.export_text()
 
-        logger.info("", extra=dict(json=job.json_summary()))
+        logger.info("", extra=dict(json=job.json_summary(add_rendered=True)))
         title = "Job %s completed in %.3fs: [%s]%s[/]. %s:\n    " % (
             job.changeId,
             job.timeElapsed,
             job.status.color,
             job.status.name,
             job.stats(asMessage=True),
         )
```

### Comparing `unfurl-0.7.1/unfurl/result.py` & `unfurl-0.8.0/unfurl/result.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/runtime.py` & `unfurl-0.8.0/unfurl/runtime.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/support.py` & `unfurl-0.8.0/unfurl/support.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,26 +313,27 @@
         return v
     v_type = type(v)
     return v_type(wrap_var(item) for item in v)
 
 
 unsafe_proxy._wrap_sequence = _wrap_sequence
 
-
 def _sandboxed_template(value: str, ctx: SafeRefContext, vars, _UnfurlUndefined):
     from jinja2.sandbox import SandboxedEnvironment
     from jinja2.nativetypes import NativeCodeGenerator, native_concat
+    from .filter_plugins import ref
 
     SandboxedEnvironment.code_generator_class = NativeCodeGenerator
     SandboxedEnvironment.concat = staticmethod(native_concat)  # type: ignore
     env = SandboxedEnvironment()
 
     if not ctx.strict:
         env.undefined = _UnfurlUndefined
     ctx.templar = None
+    env.filters.update(ref.SAFE_FILTERS)
     return env.from_string(value).render(vars)
 
 
 def apply_template(value: str, ctx: RefContext, overrides=None) -> Any:
     if not isinstance(value, str):
         msg = f"Error rendering template: source must be a string, not {type(value)}"
         if ctx.strict:
```

### Comparing `unfurl-0.7.1/unfurl/templates/aws/unfurl.yaml.j2` & `unfurl-0.8.0/unfurl/templates/aws/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/templates/dashboard/manifest.yaml.j2` & `unfurl-0.8.0/unfurl/templates/dashboard/manifest.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/templates/digitalocean/unfurl.yaml.j2` & `unfurl-0.8.0/unfurl/templates/digitalocean/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/templates/gcp/unfurl.yaml.j2` & `unfurl-0.8.0/unfurl/templates/gcp/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/templates/home/manifest-template.yaml.j2` & `unfurl-0.8.0/unfurl/templates/home/manifest-template.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/templates/home/unfurl.yaml.j2` & `unfurl-0.8.0/unfurl/templates/home/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/templates/local/ensemble-examples.yaml` & `unfurl-0.8.0/unfurl/templates/local/ensemble-examples.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/templates/local-unfurl-template.yaml.j2` & `unfurl-0.8.0/unfurl/templates/local-unfurl-template.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/templates/manifest-template.yaml.j2` & `unfurl-0.8.0/unfurl/templates/manifest-template.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/templates/manifest.yaml.j2` & `unfurl-0.8.0/unfurl/templates/manifest.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/templates/python3.10/Pipfile` & `unfurl-0.8.0/unfurl/templates/python3.10/Pipfile`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 [[source]]
 url = "https://pypi.org/simple"
 verify_ssl = true
 name = "pypi"
 
 [packages]
-pipenv = "==2022.1.8"
-click = ">=8.0.1"
-click-log = "*"
+pipenv = "==2023.7.3"
+click = ">=8.0.1,<8.1.4"
 pyrsistent = "==0.15.7"
 jsonschema = {version = "==3.2", extras = ["format_nongpl"]}
 "ruamel.yaml" = "==0.17.21"
-ansible = "<5.0,>=4.2.0"
+charset-normalizer = "==2.1.1"
+cryptography = "==38.0.3"
+ansible-core = "==2.12.10"
+gitpython = "==3.1.30"
+rich = "==12.4.4"
 pbr = "==5.9.0"
 cliff = "==3.10.1"
+pyyaml = ">=6.0"
 python-dateutil = ">=2.8"
 stevedore = "==3.5.0"
 requests = ">=2.14.2"
 importlib-metadata = "<=4.12.0"
-docker = {extras = ["tls"], version = "*"}
-openshift = "==0.13.1"
-octodns = "==0.9.14"
-boto = "*"
-boto3 = "*"
-supervisor = "*"
-google-auth = "*"
-GitPython = "==3.1.30"
-PyYAML = ">=6.0"
-Jinja2 = "<=3.1.2"
+certifi = "*"
 itsdangerous = "==2.0.1"
-MarkupSafe = "<=2.1.1"
+markupsafe = "<=2.1.1"
+jinja2 = "<=3.1.2"
 typing-extensions = "==4.1.1"
-rich = "==12.4.4"
 flask = "<=2.1.3"
 flask-caching = "<=2.0.1"
+flask-cors = "==3.0.10"
 uvicorn = "<=0.18.2"
-google-cloud-compute = "==1.3.2"
-google-cloud-dns = "==0.34.0"
-grpcio = "==1.50.0"
 python-gitlab = "==3.13.0"
-certifi = "*"
+docker = {version = "*", extras = ["tls"]}
 kubernetes = "==24.2.0"
+octodns = "==0.9.14"
+boto3 = "*"
+supervisor = "*"
+google-cloud-compute = "==1.3.2"
+google-cloud-dns = "==0.34.0"
+google-auth = "*"
 gunicorn = "==20.1.0"
 redis = "==4.4.4"
-flask-cors = "==3.0.10"
-charset-normalizer = "==2.1.1"
-cryptography = "==38.0.3"
 
 [dev-packages]
 
 [requires]
 python_version = "3.10"
```

### Comparing `unfurl-0.7.1/unfurl/templates/python3.10/Pipfile.lock` & `unfurl-0.8.0/unfurl/templates/python3.10/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.972316066066066%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'7bd243a348ce4d7298051f9a5e3fb83f76025ac951f44aa3b181f0ad3e7c5a0a'}}",*

 * * "'default'": "{'ansible-core': {'hashes': "*

 * *              "['sha256:feb1df61738cfc1f5e893b42a2ec1a7de32977d67e86707b45eb63d0c5c3c236'], "*

 * *              "'version': '==2.12.10', 'index': 'pypi', delete: ['markers']}, 'boto3': {'hashes': "*

 * *              "['sha256:cfcb20d5784428f31d89889e68b26efeda90f231c3119eef4af8b25ad405c55f', "*

 * *              "'sha256:d5ac6599951fdd519ed26c6fe15c41a7aa4021 […]*

```diff
@@ -1,38 +1,31 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "951c7c30f1956f4f461b49ef58bcd4090a335bcbc224027df59351886488c39c"
+            "sha256": "7bd243a348ce4d7298051f9a5e3fb83f76025ac951f44aa3b181f0ad3e7c5a0a"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.10"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
-        "ansible": {
-            "hashes": [
-                "sha256:88af9479e81a3931bb3a1b8c4eeb252cd4f38c03daafd6a5aa120d6b0d70d45c"
-            ],
-            "index": "pypi",
-            "version": "==4.10.0"
-        },
         "ansible-core": {
             "hashes": [
-                "sha256:9159cc3b85e2d115f62f975b5155d96466e2a09a1c2e9b91de0c781f9089fc54"
+                "sha256:feb1df61738cfc1f5e893b42a2ec1a7de32977d67e86707b45eb63d0c5c3c236"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==2.11.12"
+            "index": "pypi",
+            "version": "==2.12.10"
         },
         "async-timeout": {
             "hashes": [
                 "sha256:2163e1640ddb52b7a8c80d0a67a08587e5d245cc9c553a74a847056bc2976b15",
                 "sha256:8ca1e4fcf50d07413d66d1a5e416e42cfdf5851c981d679a09851a6853383b3c"
             ],
             "markers": "python_version >= '3.6'",
@@ -50,37 +43,29 @@
             "hashes": [
                 "sha256:01be3ee61bb714e9090fcc5c10f4cf546c396331c620c6ae50a2321b28ed3199",
                 "sha256:0fbf5efbe78d466a26753e1dee3272423a3adc989d6a778c700e89a3f8ff0d88"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.5.1"
         },
-        "boto": {
-            "hashes": [
-                "sha256:147758d41ae7240dc989f0039f27da8ca0d53734be0eb869ef16e3adcfa462e8",
-                "sha256:ea0d3b40a2d852767be77ca343b58a9e3a4b00d9db440efb8da74b4e58025e5a"
-            ],
-            "index": "pypi",
-            "version": "==2.49.0"
-        },
         "boto3": {
             "hashes": [
-                "sha256:a2778c5729d3dc0b3688c9f0d103543d7ec5ff44a4fd0e84d0d542e2dff05e62",
-                "sha256:ee0b8f8d238d4e1cf50fa6a185e4e066955b6105e9838a80b1b6582cd327dfdf"
+                "sha256:cfcb20d5784428f31d89889e68b26efeda90f231c3119eef4af8b25ad405c55f",
+                "sha256:d5ac6599951fdd519ed26c6fe15c41a7aa4021cb9adce33167344f8ce5cdb07b"
             ],
             "index": "pypi",
-            "version": "==1.26.152"
+            "version": "==1.28.12"
         },
         "botocore": {
             "hashes": [
-                "sha256:02a3205cc8579d4be6d537e63d72aebbf3f70f3aedcf40b3cae9dc2e24c774d0",
-                "sha256:f6319ecdbe3d325878f837cac2874e461b4d90691bb2d2186f980bce3b3cfcc8"
+                "sha256:7e5db466c762a071bb58c9a39d070f1333ce4f4ba6fdf9820ba21e87bd4c7e29",
+                "sha256:86380672151866b5e425636e3ebad74f2b83e7163e36ef5d38d11a04b9cba33b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.152"
+            "version": "==1.31.12"
         },
         "cachelib": {
             "hashes": [
                 "sha256:42d49f2fad9310dd946d7be73d46776bcd4d5fde4f49ad210cfdd447fbdfc346",
                 "sha256:593faeee62a7c037d50fc835617a01b887503f972fb52b188ae7e50e9cb69740"
             ],
             "markers": "python_version >= '3.7'",
@@ -92,19 +77,19 @@
                 "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.3.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "index": "pypi",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -183,22 +168,14 @@
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
             "version": "==8.1.3"
         },
-        "click-log": {
-            "hashes": [
-                "sha256:3970f8570ac54491237bcdb3d8ab5e3eef6c057df29f8c3d1151a51a9c23b975",
-                "sha256:a43e394b528d52112af599f2fc9e4b7cf3c15f94e53581f74fa6867e68c91756"
-            ],
-            "index": "pypi",
-            "version": "==0.4.0"
-        },
         "cliff": {
             "hashes": [
                 "sha256:045aee3f3c64471965d7ad507ce8474a4e2f20815fbb5405a770f8596a2a00a0",
                 "sha256:a21da482714b9f0b0e9bafaaf2f6a8b3b14161bb47f62e10e28d2fe4ff4b1626"
             ],
             "index": "pypi",
             "version": "==3.10.1"
@@ -317,53 +294,53 @@
                 "sha256:ed7b00096790213e09eb11c97cc6e2b757f15f3d2f85833cd2d3ec3fe37c1722"
             ],
             "index": "pypi",
             "version": "==38.0.3"
         },
         "distlib": {
             "hashes": [
-                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
-                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
+                "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057",
+                "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"
             ],
-            "version": "==0.3.6"
+            "version": "==0.3.7"
         },
         "dnspython": {
             "hashes": [
-                "sha256:224e32b03eb46be70e12ef6d64e0be123a64e621ab4c0822ff6d450d52a540b9",
-                "sha256:89141536394f909066cabd112e3e1a37e4e654db00a25308b0f130bc3152eb46"
+                "sha256:5b7488477388b8c0b70a8ce93b227c5603bc7b77f1565afe8e729c36c51447d7",
+                "sha256:c33971c79af5be968bb897e95c2448e11a645ee84d93b265ce0b7aabe5dfdca8"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4.0'",
-            "version": "==2.3.0"
+            "markers": "python_version >= '3.8' and python_version < '4.0'",
+            "version": "==2.4.1"
         },
         "docker": {
             "extras": [
                 "tls"
             ],
             "hashes": [
                 "sha256:aa6d17830045ba5ef0168d5eaa34d37beeb113948c413affe1d5991fc11f9a20",
                 "sha256:aecd2277b8bf8e506e484f6ab7aec39abe0038e29fa4a6d3ba86c3fe01844ed9"
             ],
             "index": "pypi",
             "version": "==6.1.3"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
-                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
+                "sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5",
+                "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.1.1"
+            "version": "==1.1.2"
         },
         "filelock": {
             "hashes": [
-                "sha256:42f1e4ff2b497311213d61ad7aac5fed9050608e5309573f101eefa94143134a",
-                "sha256:82b1f7da46f0ae42abf1bc78e548667f484ac59d2bcec38c713cee7e2eb51e83"
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.12.1"
+            "version": "==3.12.2"
         },
         "flask": {
             "hashes": [
                 "sha256:15972e5017df0575c3d6c090ba168b6db90259e620ac8d7ea813a396bad5b6cb",
                 "sha256:9013281a7402ad527f8fd56375164f3aa021ecfaff89bfe3825346c24f87e04c"
             ],
             "index": "pypi",
@@ -386,15 +363,15 @@
             "version": "==3.0.10"
         },
         "fqdn": {
             "hashes": [
                 "sha256:105ed3677e767fb5ca086a0c1f4bb66ebc3c100be518f0e0d755d9eae164d89f",
                 "sha256:3a179af3761e4df6eb2e026ff9e1a3033d3587bf980a0b1b2e1e5d08d7358014"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4.0'",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
             "version": "==1.5.1"
         },
         "gitdb": {
             "hashes": [
                 "sha256:6eb990b69df4e15bad899ea868dc46572c3f75339735663b81de79b06f17eb9a",
                 "sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7"
             ],
@@ -410,43 +387,43 @@
             "version": "==3.1.30"
         },
         "google-api-core": {
             "extras": [
                 "grpc"
             ],
             "hashes": [
-                "sha256:4b9bb5d5a380a0befa0573b302651b8a9a89262c1730e37bf423cec511804c22",
-                "sha256:ce222e27b0de0d7bc63eb043b956996d6dccab14cc3b690aaea91c9cc99dc16e"
+                "sha256:25d29e05a0058ed5f19c61c0a78b1b53adea4d9364b464d014fbda941f6d1c9a",
+                "sha256:d92a5a92dc36dd4f4b9ee4e55528a90e432b059f93aee6ad857f9de8cc7ae94a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.11.0"
+            "version": "==2.11.1"
         },
         "google-auth": {
             "hashes": [
-                "sha256:a9cfa88b3e16196845e64a3658eb953992129d13ac7337b064c6546f77c17183",
-                "sha256:ea165e014c7cbd496558796b627c271aa8c18b4cba79dc1cc962b24c5efdfb85"
+                "sha256:164cba9af4e6e4e40c3a4f90a1a6c12ee56f14c0b4868d1ca91b32826ab334ce",
+                "sha256:d61d1b40897407b574da67da1a833bdc10d5a11642566e506565d1b1a46ba873"
             ],
             "index": "pypi",
-            "version": "==2.19.1"
+            "version": "==2.22.0"
         },
         "google-cloud-compute": {
             "hashes": [
                 "sha256:1ddd1be44d278754fc2643be7aa8d66838235ce44cfbacbeeadf3952ec020e95",
                 "sha256:21bd66251356d70bfd5f40211b42b936335490f7433b3b6fae7c498077e2c3fa"
             ],
             "index": "pypi",
             "version": "==1.3.2"
         },
         "google-cloud-core": {
             "hashes": [
-                "sha256:8417acf6466be2fa85123441696c4badda48db314c607cf1e5d543fa8bdc22fe",
-                "sha256:b9529ee7047fd8d4bf4a2182de619154240df17fbe60ead399078c1ae152af9a"
+                "sha256:37b80273c8d7eee1ae816b3a20ae43585ea50506cb0e60f3cf5be5f87f1373cb",
+                "sha256:fbd11cad3e98a7e5b0343dc07cb1039a5ffd7a5bb96e1f1e27cee4bda4a90863"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.3.2"
+            "version": "==2.3.3"
         },
         "google-cloud-dns": {
             "hashes": [
                 "sha256:41609782fa91df41e5ebfd48b127bb421a3b1821f5d49d900c484d13c0672167",
                 "sha256:bd75d6e9fd456ce643ee936a113a1ead5405704515caa679db30d7f036e447f3"
             ],
             "index": "pypi",
@@ -458,62 +435,61 @@
                 "sha256:b35d530fe825fb4227857bc47ad84c33c809ac96f312e13182bdeaa2abe1178a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.59.1"
         },
         "grpcio": {
             "hashes": [
-                "sha256:05f7c248e440f538aaad13eee78ef35f0541e73498dd6f832fe284542ac4b298",
-                "sha256:080b66253f29e1646ac53ef288c12944b131a2829488ac3bac8f52abb4413c0d",
-                "sha256:12b479839a5e753580b5e6053571de14006157f2ef9b71f38c56dc9b23b95ad6",
-                "sha256:156f8009e36780fab48c979c5605eda646065d4695deea4cfcbcfdd06627ddb6",
-                "sha256:15f9e6d7f564e8f0776770e6ef32dac172c6f9960c478616c366862933fa08b4",
-                "sha256:177afaa7dba3ab5bfc211a71b90da1b887d441df33732e94e26860b3321434d9",
-                "sha256:1a4cd8cb09d1bc70b3ea37802be484c5ae5a576108bad14728f2516279165dd7",
-                "sha256:1d8d02dbb616c0a9260ce587eb751c9c7dc689bc39efa6a88cc4fa3e9c138a7b",
-                "sha256:2b71916fa8f9eb2abd93151fafe12e18cebb302686b924bd4ec39266211da525",
-                "sha256:2d9fd6e38b16c4d286a01e1776fdf6c7a4123d99ae8d6b3f0b4a03a34bf6ce45",
-                "sha256:3b611b3de3dfd2c47549ca01abfa9bbb95937eb0ea546ea1d762a335739887be",
-                "sha256:3e4244c09cc1b65c286d709658c061f12c61c814be0b7030a2d9966ff02611e0",
-                "sha256:40838061e24f960b853d7bce85086c8e1b81c6342b1f4c47ff0edd44bbae2722",
-                "sha256:4b123fbb7a777a2fedec684ca0b723d85e1d2379b6032a9a9b7851829ed3ca9a",
-                "sha256:531f8b46f3d3db91d9ef285191825d108090856b3bc86a75b7c3930f16ce432f",
-                "sha256:67dd41a31f6fc5c7db097a5c14a3fa588af54736ffc174af4411d34c4f306f68",
-                "sha256:7489dbb901f4fdf7aec8d3753eadd40839c9085967737606d2c35b43074eea24",
-                "sha256:8d4c8e73bf20fb53fe5a7318e768b9734cf122fe671fcce75654b98ba12dfb75",
-                "sha256:8e69aa4e9b7f065f01d3fdcecbe0397895a772d99954bb82eefbb1682d274518",
-                "sha256:8e8999a097ad89b30d584c034929f7c0be280cd7851ac23e9067111167dcbf55",
-                "sha256:906f4d1beb83b3496be91684c47a5d870ee628715227d5d7c54b04a8de802974",
-                "sha256:92d7635d1059d40d2ec29c8bf5ec58900120b3ce5150ef7414119430a4b2dd5c",
-                "sha256:931e746d0f75b2a5cff0a1197d21827a3a2f400c06bace036762110f19d3d507",
-                "sha256:95ce51f7a09491fb3da8cf3935005bff19983b77c4e9437ef77235d787b06842",
-                "sha256:9eea18a878cffc804506d39c6682d71f6b42ec1c151d21865a95fae743fda500",
-                "sha256:a23d47f2fc7111869f0ff547f771733661ff2818562b04b9ed674fa208e261f4",
-                "sha256:a4c23e54f58e016761b576976da6a34d876420b993f45f66a2bfb00363ecc1f9",
-                "sha256:a50a1be449b9e238b9bd43d3857d40edf65df9416dea988929891d92a9f8a778",
-                "sha256:ab5d0e3590f0a16cb88de4a3fa78d10eb66a84ca80901eb2c17c1d2c308c230f",
-                "sha256:ae23daa7eda93c1c49a9ecc316e027ceb99adbad750fbd3a56fa9e4a2ffd5ae0",
-                "sha256:af98d49e56605a2912cf330b4627e5286243242706c3a9fa0bcec6e6f68646fc",
-                "sha256:b2f77a90ba7b85bfb31329f8eab9d9540da2cf8a302128fb1241d7ea239a5469",
-                "sha256:baab51dcc4f2aecabf4ed1e2f57bceab240987c8b03533f1cef90890e6502067",
-                "sha256:ca8a2254ab88482936ce941485c1c20cdeaef0efa71a61dbad171ab6758ec998",
-                "sha256:cb11464f480e6103c59d558a3875bd84eed6723f0921290325ebe97262ae1347",
-                "sha256:ce8513aee0af9c159319692bfbf488b718d1793d764798c3d5cff827a09e25ef",
-                "sha256:cf151f97f5f381163912e8952eb5b3afe89dec9ed723d1561d59cabf1e219a35",
-                "sha256:d144ad10eeca4c1d1ce930faa105899f86f5d99cecfe0d7224f3c4c76265c15e",
-                "sha256:d534d169673dd5e6e12fb57cc67664c2641361e1a0885545495e65a7b761b0f4",
-                "sha256:d75061367a69808ab2e84c960e9dce54749bcc1e44ad3f85deee3a6c75b4ede9",
-                "sha256:d84d04dec64cc4ed726d07c5d17b73c343c8ddcd6b59c7199c801d6bbb9d9ed1",
-                "sha256:de411d2b030134b642c092e986d21aefb9d26a28bf5a18c47dd08ded411a3bc5",
-                "sha256:e07fe0d7ae395897981d16be61f0db9791f482f03fee7d1851fe20ddb4f69c03",
-                "sha256:ea8ccf95e4c7e20419b7827aa5b6da6f02720270686ac63bd3493a651830235c",
-                "sha256:f7025930039a011ed7d7e7ef95a1cb5f516e23c5a6ecc7947259b67bea8e06ca"
+                "sha256:06e84ad9ae7668a109e970c7411e7992751a116494cba7c4fb877656527f9a57",
+                "sha256:0ff789ae7d8ddd76d2ac02e7d13bfef6fc4928ac01e1dcaa182be51b6bcc0aaa",
+                "sha256:10954662f77dc36c9a1fb5cc4a537f746580d6b5734803be1e587252682cda8d",
+                "sha256:139f66656a762572ae718fa0d1f2dce47c05e9fbf7a16acd704c354405b97df9",
+                "sha256:1c31e52a04e62c8577a7bf772b3e7bed4df9c9e0dd90f92b6ffa07c16cab63c9",
+                "sha256:33971197c47965cc1d97d78d842163c283e998223b151bab0499b951fd2c0b12",
+                "sha256:345356b307cce5d14355e8e055b4ca5f99bc857c33a3dc1ddbc544fca9cd0475",
+                "sha256:373b48f210f43327a41e397391715cd11cfce9ded2fe76a5068f9bacf91cc226",
+                "sha256:3ccb621749a81dc7755243665a70ce45536ec413ef5818e013fe8dfbf5aa497b",
+                "sha256:42a3bbb2bc07aef72a7d97e71aabecaf3e4eb616d39e5211e2cfe3689de860ca",
+                "sha256:42e63904ee37ae46aa23de50dac8b145b3596f43598fa33fe1098ab2cbda6ff5",
+                "sha256:4eb37dd8dd1aa40d601212afa27ca5be255ba792e2e0b24d67b8af5e012cdb7d",
+                "sha256:51173e8fa6d9a2d85c14426bdee5f5c4a0654fd5fddcc21fe9d09ab0f6eb8b35",
+                "sha256:5144feb20fe76e73e60c7d73ec3bf54f320247d1ebe737d10672480371878b48",
+                "sha256:5344be476ac37eb9c9ad09c22f4ea193c1316bf074f1daf85bddb1b31fda5116",
+                "sha256:6108e5933eb8c22cd3646e72d5b54772c29f57482fd4c41a0640aab99eb5071d",
+                "sha256:6a007a541dff984264981fbafeb052bfe361db63578948d857907df9488d8774",
+                "sha256:6ee26e9dfb3996aff7c870f09dc7ad44a5f6732b8bdb5a5f9905737ac6fd4ef1",
+                "sha256:750de923b456ca8c0f1354d6befca45d1f3b3a789e76efc16741bd4132752d95",
+                "sha256:7c5ede2e2558f088c49a1ddda19080e4c23fb5d171de80a726b61b567e3766ed",
+                "sha256:830215173ad45d670140ff99aac3b461f9be9a6b11bee1a17265aaaa746a641a",
+                "sha256:8391cea5ce72f4a12368afd17799474015d5d3dc00c936a907eb7c7eaaea98a5",
+                "sha256:8940d6de7068af018dfa9a959a3510e9b7b543f4c405e88463a1cbaa3b2b379a",
+                "sha256:89a49cc5ad08a38b6141af17e00d1dd482dc927c7605bc77af457b5a0fca807c",
+                "sha256:900bc0096c2ca2d53f2e5cebf98293a7c32f532c4aeb926345e9747452233950",
+                "sha256:97e0efaebbfd222bcaac2f1735c010c1d3b167112d9d237daebbeedaaccf3d1d",
+                "sha256:9e04d4e4cfafa7c5264e535b5d28e786f0571bea609c3f0aaab13e891e933e9c",
+                "sha256:a4c60abd950d6de3e4f1ddbc318075654d275c29c846ab6a043d6ed2c52e4c8c",
+                "sha256:a6ff459dac39541e6a2763a4439c4ca6bc9ecb4acc05a99b79246751f9894756",
+                "sha256:a72797549935c9e0b9bc1def1768c8b5a709538fa6ab0678e671aec47ebfd55e",
+                "sha256:af4063ef2b11b96d949dccbc5a987272f38d55c23c4c01841ea65a517906397f",
+                "sha256:b975b85d1d5efc36cf8b237c5f3849b64d1ba33d6282f5e991f28751317504a1",
+                "sha256:bf0b9959e673505ee5869950642428046edb91f99942607c2ecf635f8a4b31c9",
+                "sha256:c0c85c5cbe8b30a32fa6d802588d55ffabf720e985abe9590c7c886919d875d4",
+                "sha256:c3f3237a57e42f79f1e560726576aedb3a7ef931f4e3accb84ebf6acc485d316",
+                "sha256:c3fa3ab0fb200a2c66493828ed06ccd1a94b12eddbfb985e7fd3e5723ff156c6",
+                "sha256:c435f5ce1705de48e08fcbcfaf8aee660d199c90536e3e06f2016af7d6a938dd",
+                "sha256:c90da4b124647547a68cf2f197174ada30c7bb9523cb976665dfd26a9963d328",
+                "sha256:cbdf2c498e077282cd427cfd88bdce4668019791deef0be8155385ab2ba7837f",
+                "sha256:d1fbad1f9077372b6587ec589c1fc120b417b6c8ad72d3e3cc86bbbd0a3cee93",
+                "sha256:d39f5d4af48c138cb146763eda14eb7d8b3ccbbec9fe86fb724cd16e0e914c64",
+                "sha256:ddb4a6061933bd9332b74eac0da25f17f32afa7145a33a0f9711ad74f924b1b8",
+                "sha256:ded637176addc1d3eef35331c39acc598bac550d213f0a1bedabfceaa2244c87",
+                "sha256:f20fd21f7538f8107451156dd1fe203300b79a9ddceba1ee0ac8132521a008ed",
+                "sha256:fda2783c12f553cdca11c08e5af6eecbd717280dc8fbe28a110897af1c15a88c"
             ],
-            "index": "pypi",
-            "version": "==1.50.0"
+            "version": "==1.56.2"
         },
         "grpcio-status": {
             "hashes": [
                 "sha256:2c33bbdbe20188b2953f46f31af669263b6ee2a9b2d38fa0d36ee091532e21bf",
                 "sha256:53695f45da07437b7c344ee4ef60d370fd2850179f5a28bb26d8e2aa1102ec11"
             ],
             "version": "==1.48.2"
@@ -579,18 +555,18 @@
                 "sha256:90261b206d6defd58fdd5e85f478bf633a2901798906be2ad389150c5c60edbe"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.1"
         },
         "jsonpointer": {
             "hashes": [
-                "sha256:51801e558539b4e9cd268638c078c6c5746c9ac96bc38152d443400e4f3793e9",
-                "sha256:97cba51526c829282218feb99dab1b1e6bdf8efd1c43dc9d57be093c0d69c99a"
+                "sha256:15d51bba20eea3165644553647711d150376234112651b4f1811022aecad7d7a",
+                "sha256:585cee82b70211fa9e6043b7bb89db6e1aa49524340dde8ad6b63206ea689d88"
             ],
-            "version": "==2.3"
+            "version": "==2.4"
         },
         "jsonschema": {
             "extras": [
                 "format_nongpl"
             ],
             "hashes": [
                 "sha256:4e5b3cf8216f577bee9ce139cbe72eca3ea4f292ec60928ff24758ce626cd163",
@@ -651,19 +627,19 @@
                 "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
             ],
             "index": "pypi",
             "version": "==2.1.1"
         },
         "natsort": {
             "hashes": [
-                "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
-                "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
+                "sha256:45312c4a0e5507593da193dedd04abb1469253b601ecaf63445ad80f0a1ea581",
+                "sha256:4732914fb471f56b5cce04d7bae6f164a592c7712e1c85f9ef585e197299521c"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==8.3.1"
+            "version": "==8.4.0"
         },
         "oauthlib": {
             "hashes": [
                 "sha256:8139f29aac13e25d502680e9e19963e83f16838d48a0d71c287fe40e7067fbca",
                 "sha256:9859c40929662bec5d64f34d01c99e093149682a3f38915dc0655d5a633dd918"
             ],
             "markers": "python_version >= '3.6'",
@@ -673,21 +649,14 @@
             "hashes": [
                 "sha256:9c31bd5cdbdbe5ef678cb01ac0564461790126acb9c3ab51a0f63fc9eaf608c8",
                 "sha256:aa629a2b75714a5c15c47125b6e1c4226492d7fe4c5b348c081c8b4cf87ce0ae"
             ],
             "index": "pypi",
             "version": "==0.9.14"
         },
-        "openshift": {
-            "hashes": [
-                "sha256:a060afb7565dda18b2749857867d80ab22b2f4143264519f493a9cabccc3b8a8"
-            ],
-            "index": "pypi",
-            "version": "==0.13.1"
-        },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
@@ -696,45 +665,37 @@
             "hashes": [
                 "sha256:e547125940bcc052856ded43be8e101f63828c2d94239ffbe2b327ba3d5ccf0a",
                 "sha256:e8dca2f4b43560edef58813969f52a56cef023146cbb8931626db80e6c1c4308"
             ],
             "index": "pypi",
             "version": "==5.9.0"
         },
-        "pip": {
-            "hashes": [
-                "sha256:0e7c86f486935893c708287b30bd050a36ac827ec7fe5e43fe7cb198dd835fba",
-                "sha256:3ef6ac33239e4027d9a5598a381b9d30880a1477e50039db2eac6e8a8f6d1b18"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.1.2"
-        },
         "pipenv": {
             "hashes": [
-                "sha256:3b80b4512934b9d8e8ce12c988394642ff96bb697680e5b092e59af503178327",
-                "sha256:f84d7119239b22ab2ac2b8fbc7d619d83cf41135206d72a17c4f151cda529fd0"
+                "sha256:116061545d4e2281cbc799f7736a715ee5ddf0a6f63c09f4263a4a6a0779fe93",
+                "sha256:404de9ff6a2464e20e52aaad71db2d4f8f2900f2177fc45a47f6315686cb2e5b"
             ],
             "index": "pypi",
-            "version": "==2022.1.8"
+            "version": "==2023.7.3"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:0ade98a4895e87dc51d47151f7d2ec290365a585151d97b4d8d6312ed6132fed",
-                "sha256:e48fabd87db8f3a7df7150a4a5ea22c546ee8bc39bc2473244730d4b56d2cc4e"
+                "sha256:1b42b450ad933e981d56e59f1b97495428c9bd60698baab9f3eb3d00d5822421",
+                "sha256:ad8291ae0ae5072f66c16945166cb11c63394c7a3ad1b1bc9828ca3162da8c2f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.3"
+            "version": "==3.9.1"
         },
         "pluggy": {
             "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
+                "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
+                "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.0.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.2.0"
         },
         "pprintpp": {
             "hashes": [
                 "sha256:b6b4dcdd0c0c0d75e4d7b2f21a9e933e5b2ce62b26e1a54537f9651ae5a5c01d",
                 "sha256:ea826108e2c7f49dc6d66c752973c3fc9749142a798d6b254e1e301cfdbc6403"
             ],
             "version": "==0.4.0"
@@ -745,19 +706,19 @@
                 "sha256:03481bca25ae0c28958c8cd6ac5165c159ce89f7ccde04d5c899b24b68bb13b7"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==3.8.0"
         },
         "proto-plus": {
             "hashes": [
-                "sha256:0e8cda3d5a634d9895b75c573c9352c16486cb75deb0e078b5fda34db4243165",
-                "sha256:de34e52d6c9c6fcd704192f09767cb561bb4ee64e70eede20b0834d841f0be4d"
+                "sha256:a49cd903bc0b6ab41f76bf65510439d56ca76f868adf0274e738bfdd096894df",
+                "sha256:fdcd09713cbd42480740d2fe29c990f7fbd885a67efc328aa8be6ee3e9f76a6b"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==1.22.2"
+            "version": "==1.22.3"
         },
         "protobuf": {
             "hashes": [
                 "sha256:03038ac1cfbc41aa21f6afcbcd357281d7521b4157926f30ebecc8d4ea59dcb7",
                 "sha256:28545383d61f55b57cf4df63eebd9827754fd2dc25f80c5253f9184235db242c",
                 "sha256:2e3427429c9cffebf259491be0af70189607f365c2f41c7c3764af6f337105f2",
                 "sha256:398a9e0c3eaceb34ec1aee71894ca3299605fa8e761544934378bbc6c97de23b",
@@ -799,15 +760,15 @@
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==0.3.0"
         },
         "pycountry": {
             "hashes": [
                 "sha256:b2163a246c585894d808f18783e19137cb70a0c18fb36748dc01fc6f109c1646"
             ],
-            "markers": "python_version >= '3.6' and python_version < '4.0'",
+            "markers": "python_version >= '3.6' and python_version < '4'",
             "version": "==22.3.5"
         },
         "pycountry-convert": {
             "hashes": [
                 "sha256:095d310f746bf2a5ef713b3a82eea28a27262286223765b1e7be8a5c4fa7e9b9",
                 "sha256:5e33883a88b3cb752d332ca2358ac6c4de4defc86a2b93b713b36338e914952e"
             ],
@@ -826,19 +787,19 @@
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pyparsing": {
             "hashes": [
-                "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb",
-                "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
+                "sha256:d554a96d1a7d3ddaf7183104485bc19fd80543ad6ac5bdb6426719d766fb06c1",
+                "sha256:edb662d6fe322d6e990b1594b5feaeadf806803359e3d4d42f11e295e588f0ea"
             ],
             "markers": "python_full_version >= '3.6.8'",
-            "version": "==3.0.9"
+            "version": "==3.1.0"
         },
         "pyperclip": {
             "hashes": [
                 "sha256:105254a8b04934f0bc84e9c24eb360a591aaf6535c9def5f29d92af107a9bf57"
             ],
             "version": "==1.8.2"
         },
@@ -847,35 +808,35 @@
                 "sha256:cdc7b5e3ed77bed61270a47d35434a30617b9becdf2478af76ad2c6ade307280"
             ],
             "index": "pypi",
             "version": "==0.15.7"
         },
         "pytest": {
             "hashes": [
-                "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295",
-                "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"
+                "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
+                "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.3.2"
+            "version": "==7.4.0"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6",
                 "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.1.0"
         },
         "pytest-mock": {
             "hashes": [
-                "sha256:f4c973eeae0282963eb293eb173ce91b091a79c1334455acfac9ddee8a1c784b",
-                "sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f"
+                "sha256:21c279fff83d70763b05f8874cc9cfb3fcacd6d354247a976f9529d19f9acf39",
+                "sha256:7f6b125602ac6d743e523ae0bfa71e1a697a2f5534064528c6ff84c2f7c2fc7f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.10.0"
+            "version": "==3.11.1"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "index": "pypi",
@@ -885,67 +846,59 @@
             "hashes": [
                 "sha256:85ae778d8953aba87ad4b78aef7fbb5dae053980d2c20ff200bea29799685743",
                 "sha256:ad502b72b5d1137f4af37d4a68ae20fe7d6c9778f67cbe2aec566f7995053c7d"
             ],
             "index": "pypi",
             "version": "==3.13.0"
         },
-        "python-string-utils": {
-            "hashes": [
-                "sha256:dcf9060b03f07647c0a603408dc8b03f807f3b54a05c6e19eb14460256fac0cb",
-                "sha256:f1a88700baf99db1a9b6953f44181ad9ca56623c81e257e6009707e2e7851fa4"
-            ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.0"
-        },
         "pyyaml": {
             "hashes": [
-                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
-                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
-                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
-                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
-                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
-                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
-                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
-                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
-                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
-                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
-                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
-                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
-                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
-                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
-                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
-                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
-                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
-                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
-                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
-                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
-                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
-                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
-                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
-                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
-                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
-                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
-                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
-                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
-                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
-                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
-                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
-                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
-                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
-                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
-                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
-                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
-                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
-                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
-                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
-                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
+                "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
+                "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
+                "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
+                "sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27",
+                "sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595",
+                "sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62",
+                "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98",
+                "sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696",
+                "sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d",
+                "sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867",
+                "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47",
+                "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486",
+                "sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6",
+                "sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3",
+                "sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007",
+                "sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938",
+                "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
+                "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
+                "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
+                "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
+                "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
+                "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
+                "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
+                "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
+                "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
+                "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
+                "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
+                "sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924",
+                "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34",
+                "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43",
+                "sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859",
+                "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673",
+                "sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a",
+                "sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab",
+                "sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa",
+                "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c",
+                "sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585",
+                "sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d",
+                "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"
             ],
             "index": "pypi",
-            "version": "==6.0"
+            "version": "==6.0.1"
         },
         "redis": {
             "hashes": [
                 "sha256:68226f7ede928db8302f29ab088a157f41061fa946b7ae865452b6d7838bbffb",
                 "sha256:da92a39fec86438d3f1e2a1db33c312985806954fe860120b582a8430e231d8f"
             ],
             "index": "pypi",
@@ -1012,15 +965,15 @@
             "version": "==12.4.4"
         },
         "rsa": {
             "hashes": [
                 "sha256:90260d9058e514786967344d0ef75fa8727eed8a7d2e43ce9f4bcf1b536174f7",
                 "sha256:e38464a49c6c85d7f1351b0126661487a7e0a14a50f1675ec50eb34d4f20ef21"
             ],
-            "markers": "python_version >= '3.6' and python_version < '4.0'",
+            "markers": "python_version >= '3.6' and python_version < '4'",
             "version": "==4.9"
         },
         "ruamel.yaml": {
             "hashes": [
                 "sha256:742b35d3d665023981bd6d16b3d24248ce5df75fdb4e2924e93a05c1f8b61ca7",
                 "sha256:8b7ce697a2f212752a35c1ac414471dc16c424c9573be4926b56ff3f5d23b7af"
             ],
@@ -1076,19 +1029,19 @@
                 "sha256:640bb492711f4c0c0905e1f62b6aaeb771881935ad27884852411f8e9cacbca9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.6.1"
         },
         "setuptools": {
             "hashes": [
-                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
-                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.8.0"
+            "version": "==68.0.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
@@ -1148,19 +1101,19 @@
                 "sha256:cade07c403c397f9fe275492a48c1b869efd175d5d8a692df649e6e7e2ed8f4e"
             ],
             "index": "pypi",
             "version": "==0.18.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
-                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
+                "sha256:43a3052be36080548bdee0b42919c88072037d50d56c28bd3f853cbe92b953ff",
+                "sha256:fd8a78f46f6b99a67b7ec5cf73f92357891a7b3a40fd97637c27f854aae3b9e0"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.23.0"
+            "version": "==20.24.2"
         },
         "virtualenv-clone": {
             "hashes": [
                 "sha256:418ee935c36152f8f153c79824bb93eaf6f0f7984bae31d3f48f350b9183501a",
                 "sha256:44d5263bceed0bac3e1424d64f798095233b64def1c5689afa43dc3223caf5b0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1178,40 +1131,40 @@
                 "sha256:29bc7e8752c0a1bd4a1f03c14d6e6a72e93d82193738fa860cbff59d0fcc11bf",
                 "sha256:c225b674c83fa923be93d235330ce0300373d02885cef23238813b0d5668304a"
             ],
             "version": "==1.13"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:3566f8467cd350874c4913816355642a4942f6c1ed1e9406e3d42fae6d6c072a",
-                "sha256:b96f3bce3e54e3486ebe6504bc22bd4c140392bd2eb71764db29be8f2639aa65"
+                "sha256:c951af98631d24f8df89ab1019fc365f2227c0892f12fd150e935607c79dd0dd",
+                "sha256:f1f9f2ad5291f0225a49efad77abf9e700b6fef553900623060dad6e26503b9d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.5.3"
+            "version": "==1.6.1"
         },
         "werkzeug": {
             "hashes": [
                 "sha256:935539fa1413afbb9195b24880778422ed620c0fc09670945185cce4d91a8890",
                 "sha256:98c774df2f91b05550078891dee5f0eb0cb797a522c757a2452b9cee5b202330"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==2.3.6"
         },
         "wheel": {
             "hashes": [
-                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
-                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
+                "sha256:55a0f0a5a84869bce5ba775abfd9c462e3a6b1b7b7ec69d72c0b83d673a5114d",
+                "sha256:7e9be3bbd0078f6147d82ed9ed957e323e7708f57e134743d2edef3a7b7972a9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.40.0"
+            "version": "==0.41.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
-                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
+                "sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0",
+                "sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.15.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.16.2"
         }
     },
     "develop": {}
 }
```

### Comparing `unfurl-0.7.1/unfurl/templates/python3.11/Pipfile` & `unfurl-0.8.0/unfurl/templates/python3.11/Pipfile`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 [[source]]
 url = "https://pypi.org/simple"
 verify_ssl = true
 name = "pypi"
 
 [packages]
-pipenv = "==2022.1.8"
-click = ">=8.0.1"
-click-log = "*"
+pipenv = "==2023.7.3"
+click = ">=8.0.1,<8.1.4"
 pyrsistent = "==0.15.7"
 jsonschema = {version = "==3.2", extras = ["format_nongpl"]}
 "ruamel.yaml" = "==0.17.21"
-ansible = ">=4.2.0,<5.0"
+charset-normalizer = "==2.1.1"
+cryptography = "==38.0.3"
+ansible-core = "==2.12.10"
 gitpython = "==3.1.30"
 rich = "==12.4.4"
 pbr = "==5.9.0"
 cliff = "==3.10.1"
 pyyaml = ">=6.0"
 python-dateutil = ">=2.8"
 stevedore = "==3.5.0"
 requests = ">=2.14.2"
 importlib-metadata = "<=4.12.0"
+certifi = "*"
 itsdangerous = "==2.0.1"
 markupsafe = "<=2.1.1"
 jinja2 = "<=3.1.2"
 typing-extensions = "==4.1.1"
 flask = "<=2.1.3"
 flask-caching = "<=2.0.1"
+flask-cors = "==3.0.10"
 uvicorn = "<=0.18.2"
-docker = {extras = ["tls"], version = "*"}
-openshift = "==0.13.1"
+python-gitlab = "==3.13.0"
+docker = {version = "*", extras = ["tls"]}
+kubernetes = "==24.2.0"
 octodns = "==0.9.14"
-boto = "*"
 boto3 = "*"
 supervisor = "*"
 google-cloud-compute = "==1.3.2"
 google-cloud-dns = "==0.34.0"
 google-auth = "*"
-grpcio = "==1.50.0"
-python-gitlab = "==3.13.0"
-certifi = "*"
-kubernetes = "==24.2.0"
 gunicorn = "==20.1.0"
 redis = "==4.4.4"
-flask-cors = "==3.0.10"
-charset-normalizer = "==2.1.1"
-cryptography = "==38.0.3"
 
 [dev-packages]
 
 [requires]
 python_version = "3.11"
```

### Comparing `unfurl-0.7.1/unfurl/templates/python3.11/Pipfile.lock` & `unfurl-0.8.0/unfurl/templates/python3.7/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9567832341269842%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'4288ec0537151a92dcfa635eb39e1571f68907b53c618bb5f54d6df30a354172'}, 'requires': "*

 * *            "{'python_version': '3.7'}}",*

 * * "'default'": "{'ansible-core': {'index': 'pypi', delete: ['markers']}, 'boto3': {'hashes': "*

 * *              "['sha256:cfcb20d5784428f31d89889e68b26efeda90f231c3119eef4af8b25ad405c55f', "*

 * *              "'sha256:d5ac6599951fdd519ed26c6fe15c41a7aa4021cb9adce33167344f8ce5cdb07b'], "*

 * *              "'version': '==1.28.12'}, 'botocore': {'hashe […]*

```diff
@@ -1,37 +1,30 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "b109f40f6130058dd7f51c4cf0f7cc0835fdff8ad368cf900dd31784971c5704"
+            "sha256": "4288ec0537151a92dcfa635eb39e1571f68907b53c618bb5f54d6df30a354172"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.11"
+            "python_version": "3.7"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
-        "ansible": {
-            "hashes": [
-                "sha256:88af9479e81a3931bb3a1b8c4eeb252cd4f38c03daafd6a5aa120d6b0d70d45c"
-            ],
-            "index": "pypi",
-            "version": "==4.10.0"
-        },
         "ansible-core": {
             "hashes": [
                 "sha256:9159cc3b85e2d115f62f975b5155d96466e2a09a1c2e9b91de0c781f9089fc54"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "index": "pypi",
             "version": "==2.11.12"
         },
         "async-timeout": {
             "hashes": [
                 "sha256:2163e1640ddb52b7a8c80d0a67a08587e5d245cc9c553a74a847056bc2976b15",
                 "sha256:8ca1e4fcf50d07413d66d1a5e416e42cfdf5851c981d679a09851a6853383b3c"
             ],
@@ -50,37 +43,37 @@
             "hashes": [
                 "sha256:01be3ee61bb714e9090fcc5c10f4cf546c396331c620c6ae50a2321b28ed3199",
                 "sha256:0fbf5efbe78d466a26753e1dee3272423a3adc989d6a778c700e89a3f8ff0d88"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.5.1"
         },
-        "boto": {
-            "hashes": [
-                "sha256:147758d41ae7240dc989f0039f27da8ca0d53734be0eb869ef16e3adcfa462e8",
-                "sha256:ea0d3b40a2d852767be77ca343b58a9e3a4b00d9db440efb8da74b4e58025e5a"
-            ],
-            "index": "pypi",
-            "version": "==2.49.0"
-        },
         "boto3": {
             "hashes": [
-                "sha256:a2778c5729d3dc0b3688c9f0d103543d7ec5ff44a4fd0e84d0d542e2dff05e62",
-                "sha256:ee0b8f8d238d4e1cf50fa6a185e4e066955b6105e9838a80b1b6582cd327dfdf"
+                "sha256:cfcb20d5784428f31d89889e68b26efeda90f231c3119eef4af8b25ad405c55f",
+                "sha256:d5ac6599951fdd519ed26c6fe15c41a7aa4021cb9adce33167344f8ce5cdb07b"
             ],
             "index": "pypi",
-            "version": "==1.26.152"
+            "version": "==1.28.12"
         },
         "botocore": {
             "hashes": [
-                "sha256:02a3205cc8579d4be6d537e63d72aebbf3f70f3aedcf40b3cae9dc2e24c774d0",
-                "sha256:f6319ecdbe3d325878f837cac2874e461b4d90691bb2d2186f980bce3b3cfcc8"
+                "sha256:7e5db466c762a071bb58c9a39d070f1333ce4f4ba6fdf9820ba21e87bd4c7e29",
+                "sha256:86380672151866b5e425636e3ebad74f2b83e7163e36ef5d38d11a04b9cba33b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.152"
+            "version": "==1.31.12"
+        },
+        "cached-property": {
+            "hashes": [
+                "sha256:9fa5755838eecbb2d234c3aa390bd80fbd3ac6b6869109bfc1b499f7bd89a130",
+                "sha256:df4f613cf7ad9a588cc381aaf4a512d26265ecebd5eb9e1ba12f1319eb85a6a0"
+            ],
+            "markers": "python_version < '3.8'",
+            "version": "==1.5.2"
         },
         "cachelib": {
             "hashes": [
                 "sha256:42d49f2fad9310dd946d7be73d46776bcd4d5fde4f49ad210cfdd447fbdfc346",
                 "sha256:593faeee62a7c037d50fc835617a01b887503f972fb52b188ae7e50e9cb69740"
             ],
             "markers": "python_version >= '3.7'",
@@ -92,19 +85,19 @@
                 "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.3.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "index": "pypi",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -183,22 +176,14 @@
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
             "version": "==8.1.3"
         },
-        "click-log": {
-            "hashes": [
-                "sha256:3970f8570ac54491237bcdb3d8ab5e3eef6c057df29f8c3d1151a51a9c23b975",
-                "sha256:a43e394b528d52112af599f2fc9e4b7cf3c15f94e53581f74fa6867e68c91756"
-            ],
-            "index": "pypi",
-            "version": "==0.4.0"
-        },
         "cliff": {
             "hashes": [
                 "sha256:045aee3f3c64471965d7ad507ce8474a4e2f20815fbb5405a770f8596a2a00a0",
                 "sha256:a21da482714b9f0b0e9bafaaf2f6a8b3b14161bb47f62e10e28d2fe4ff4b1626"
             ],
             "index": "pypi",
             "version": "==3.10.1"
@@ -317,18 +302,18 @@
                 "sha256:ed7b00096790213e09eb11c97cc6e2b757f15f3d2f85833cd2d3ec3fe37c1722"
             ],
             "index": "pypi",
             "version": "==38.0.3"
         },
         "distlib": {
             "hashes": [
-                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
-                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
+                "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057",
+                "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"
             ],
-            "version": "==0.3.6"
+            "version": "==0.3.7"
         },
         "dnspython": {
             "hashes": [
                 "sha256:224e32b03eb46be70e12ef6d64e0be123a64e621ab4c0822ff6d450d52a540b9",
                 "sha256:89141536394f909066cabd112e3e1a37e4e654db00a25308b0f130bc3152eb46"
             ],
             "markers": "python_version >= '3.7' and python_version < '4.0'",
@@ -341,14 +326,22 @@
             "hashes": [
                 "sha256:aa6d17830045ba5ef0168d5eaa34d37beeb113948c413affe1d5991fc11f9a20",
                 "sha256:aecd2277b8bf8e506e484f6ab7aec39abe0038e29fa4a6d3ba86c3fe01844ed9"
             ],
             "index": "pypi",
             "version": "==6.1.3"
         },
+        "exceptiongroup": {
+            "hashes": [
+                "sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5",
+                "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==1.1.2"
+        },
         "filelock": {
             "hashes": [
                 "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
                 "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.12.2"
@@ -378,15 +371,15 @@
             "version": "==3.0.10"
         },
         "fqdn": {
             "hashes": [
                 "sha256:105ed3677e767fb5ca086a0c1f4bb66ebc3c100be518f0e0d755d9eae164d89f",
                 "sha256:3a179af3761e4df6eb2e026ff9e1a3033d3587bf980a0b1b2e1e5d08d7358014"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4.0'",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
             "version": "==1.5.1"
         },
         "gitdb": {
             "hashes": [
                 "sha256:6eb990b69df4e15bad899ea868dc46572c3f75339735663b81de79b06f17eb9a",
                 "sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7"
             ],
@@ -402,43 +395,43 @@
             "version": "==3.1.30"
         },
         "google-api-core": {
             "extras": [
                 "grpc"
             ],
             "hashes": [
-                "sha256:10c06f7739fe57781f87523375e8e1a3a4674bf6392cd6131a3222182b971320",
-                "sha256:34f24bd1d5f72a8c4519773d99ca6bf080a6c4e041b4e9f024fe230191dda62e"
+                "sha256:25d29e05a0058ed5f19c61c0a78b1b53adea4d9364b464d014fbda941f6d1c9a",
+                "sha256:d92a5a92dc36dd4f4b9ee4e55528a90e432b059f93aee6ad857f9de8cc7ae94a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.10.2"
+            "version": "==2.11.1"
         },
         "google-auth": {
             "hashes": [
-                "sha256:a9cfa88b3e16196845e64a3658eb953992129d13ac7337b064c6546f77c17183",
-                "sha256:ea165e014c7cbd496558796b627c271aa8c18b4cba79dc1cc962b24c5efdfb85"
+                "sha256:164cba9af4e6e4e40c3a4f90a1a6c12ee56f14c0b4868d1ca91b32826ab334ce",
+                "sha256:d61d1b40897407b574da67da1a833bdc10d5a11642566e506565d1b1a46ba873"
             ],
             "index": "pypi",
-            "version": "==2.19.1"
+            "version": "==2.22.0"
         },
         "google-cloud-compute": {
             "hashes": [
                 "sha256:1ddd1be44d278754fc2643be7aa8d66838235ce44cfbacbeeadf3952ec020e95",
                 "sha256:21bd66251356d70bfd5f40211b42b936335490f7433b3b6fae7c498077e2c3fa"
             ],
             "index": "pypi",
             "version": "==1.3.2"
         },
         "google-cloud-core": {
             "hashes": [
-                "sha256:8417acf6466be2fa85123441696c4badda48db314c607cf1e5d543fa8bdc22fe",
-                "sha256:b9529ee7047fd8d4bf4a2182de619154240df17fbe60ead399078c1ae152af9a"
+                "sha256:37b80273c8d7eee1ae816b3a20ae43585ea50506cb0e60f3cf5be5f87f1373cb",
+                "sha256:fbd11cad3e98a7e5b0343dc07cb1039a5ffd7a5bb96e1f1e27cee4bda4a90863"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.3.2"
+            "version": "==2.3.3"
         },
         "google-cloud-dns": {
             "hashes": [
                 "sha256:41609782fa91df41e5ebfd48b127bb421a3b1821f5d49d900c484d13c0672167",
                 "sha256:bd75d6e9fd456ce643ee936a113a1ead5405704515caa679db30d7f036e447f3"
             ],
             "index": "pypi",
@@ -450,62 +443,61 @@
                 "sha256:b35d530fe825fb4227857bc47ad84c33c809ac96f312e13182bdeaa2abe1178a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.59.1"
         },
         "grpcio": {
             "hashes": [
-                "sha256:05f7c248e440f538aaad13eee78ef35f0541e73498dd6f832fe284542ac4b298",
-                "sha256:080b66253f29e1646ac53ef288c12944b131a2829488ac3bac8f52abb4413c0d",
-                "sha256:12b479839a5e753580b5e6053571de14006157f2ef9b71f38c56dc9b23b95ad6",
-                "sha256:156f8009e36780fab48c979c5605eda646065d4695deea4cfcbcfdd06627ddb6",
-                "sha256:15f9e6d7f564e8f0776770e6ef32dac172c6f9960c478616c366862933fa08b4",
-                "sha256:177afaa7dba3ab5bfc211a71b90da1b887d441df33732e94e26860b3321434d9",
-                "sha256:1a4cd8cb09d1bc70b3ea37802be484c5ae5a576108bad14728f2516279165dd7",
-                "sha256:1d8d02dbb616c0a9260ce587eb751c9c7dc689bc39efa6a88cc4fa3e9c138a7b",
-                "sha256:2b71916fa8f9eb2abd93151fafe12e18cebb302686b924bd4ec39266211da525",
-                "sha256:2d9fd6e38b16c4d286a01e1776fdf6c7a4123d99ae8d6b3f0b4a03a34bf6ce45",
-                "sha256:3b611b3de3dfd2c47549ca01abfa9bbb95937eb0ea546ea1d762a335739887be",
-                "sha256:3e4244c09cc1b65c286d709658c061f12c61c814be0b7030a2d9966ff02611e0",
-                "sha256:40838061e24f960b853d7bce85086c8e1b81c6342b1f4c47ff0edd44bbae2722",
-                "sha256:4b123fbb7a777a2fedec684ca0b723d85e1d2379b6032a9a9b7851829ed3ca9a",
-                "sha256:531f8b46f3d3db91d9ef285191825d108090856b3bc86a75b7c3930f16ce432f",
-                "sha256:67dd41a31f6fc5c7db097a5c14a3fa588af54736ffc174af4411d34c4f306f68",
-                "sha256:7489dbb901f4fdf7aec8d3753eadd40839c9085967737606d2c35b43074eea24",
-                "sha256:8d4c8e73bf20fb53fe5a7318e768b9734cf122fe671fcce75654b98ba12dfb75",
-                "sha256:8e69aa4e9b7f065f01d3fdcecbe0397895a772d99954bb82eefbb1682d274518",
-                "sha256:8e8999a097ad89b30d584c034929f7c0be280cd7851ac23e9067111167dcbf55",
-                "sha256:906f4d1beb83b3496be91684c47a5d870ee628715227d5d7c54b04a8de802974",
-                "sha256:92d7635d1059d40d2ec29c8bf5ec58900120b3ce5150ef7414119430a4b2dd5c",
-                "sha256:931e746d0f75b2a5cff0a1197d21827a3a2f400c06bace036762110f19d3d507",
-                "sha256:95ce51f7a09491fb3da8cf3935005bff19983b77c4e9437ef77235d787b06842",
-                "sha256:9eea18a878cffc804506d39c6682d71f6b42ec1c151d21865a95fae743fda500",
-                "sha256:a23d47f2fc7111869f0ff547f771733661ff2818562b04b9ed674fa208e261f4",
-                "sha256:a4c23e54f58e016761b576976da6a34d876420b993f45f66a2bfb00363ecc1f9",
-                "sha256:a50a1be449b9e238b9bd43d3857d40edf65df9416dea988929891d92a9f8a778",
-                "sha256:ab5d0e3590f0a16cb88de4a3fa78d10eb66a84ca80901eb2c17c1d2c308c230f",
-                "sha256:ae23daa7eda93c1c49a9ecc316e027ceb99adbad750fbd3a56fa9e4a2ffd5ae0",
-                "sha256:af98d49e56605a2912cf330b4627e5286243242706c3a9fa0bcec6e6f68646fc",
-                "sha256:b2f77a90ba7b85bfb31329f8eab9d9540da2cf8a302128fb1241d7ea239a5469",
-                "sha256:baab51dcc4f2aecabf4ed1e2f57bceab240987c8b03533f1cef90890e6502067",
-                "sha256:ca8a2254ab88482936ce941485c1c20cdeaef0efa71a61dbad171ab6758ec998",
-                "sha256:cb11464f480e6103c59d558a3875bd84eed6723f0921290325ebe97262ae1347",
-                "sha256:ce8513aee0af9c159319692bfbf488b718d1793d764798c3d5cff827a09e25ef",
-                "sha256:cf151f97f5f381163912e8952eb5b3afe89dec9ed723d1561d59cabf1e219a35",
-                "sha256:d144ad10eeca4c1d1ce930faa105899f86f5d99cecfe0d7224f3c4c76265c15e",
-                "sha256:d534d169673dd5e6e12fb57cc67664c2641361e1a0885545495e65a7b761b0f4",
-                "sha256:d75061367a69808ab2e84c960e9dce54749bcc1e44ad3f85deee3a6c75b4ede9",
-                "sha256:d84d04dec64cc4ed726d07c5d17b73c343c8ddcd6b59c7199c801d6bbb9d9ed1",
-                "sha256:de411d2b030134b642c092e986d21aefb9d26a28bf5a18c47dd08ded411a3bc5",
-                "sha256:e07fe0d7ae395897981d16be61f0db9791f482f03fee7d1851fe20ddb4f69c03",
-                "sha256:ea8ccf95e4c7e20419b7827aa5b6da6f02720270686ac63bd3493a651830235c",
-                "sha256:f7025930039a011ed7d7e7ef95a1cb5f516e23c5a6ecc7947259b67bea8e06ca"
+                "sha256:06e84ad9ae7668a109e970c7411e7992751a116494cba7c4fb877656527f9a57",
+                "sha256:0ff789ae7d8ddd76d2ac02e7d13bfef6fc4928ac01e1dcaa182be51b6bcc0aaa",
+                "sha256:10954662f77dc36c9a1fb5cc4a537f746580d6b5734803be1e587252682cda8d",
+                "sha256:139f66656a762572ae718fa0d1f2dce47c05e9fbf7a16acd704c354405b97df9",
+                "sha256:1c31e52a04e62c8577a7bf772b3e7bed4df9c9e0dd90f92b6ffa07c16cab63c9",
+                "sha256:33971197c47965cc1d97d78d842163c283e998223b151bab0499b951fd2c0b12",
+                "sha256:345356b307cce5d14355e8e055b4ca5f99bc857c33a3dc1ddbc544fca9cd0475",
+                "sha256:373b48f210f43327a41e397391715cd11cfce9ded2fe76a5068f9bacf91cc226",
+                "sha256:3ccb621749a81dc7755243665a70ce45536ec413ef5818e013fe8dfbf5aa497b",
+                "sha256:42a3bbb2bc07aef72a7d97e71aabecaf3e4eb616d39e5211e2cfe3689de860ca",
+                "sha256:42e63904ee37ae46aa23de50dac8b145b3596f43598fa33fe1098ab2cbda6ff5",
+                "sha256:4eb37dd8dd1aa40d601212afa27ca5be255ba792e2e0b24d67b8af5e012cdb7d",
+                "sha256:51173e8fa6d9a2d85c14426bdee5f5c4a0654fd5fddcc21fe9d09ab0f6eb8b35",
+                "sha256:5144feb20fe76e73e60c7d73ec3bf54f320247d1ebe737d10672480371878b48",
+                "sha256:5344be476ac37eb9c9ad09c22f4ea193c1316bf074f1daf85bddb1b31fda5116",
+                "sha256:6108e5933eb8c22cd3646e72d5b54772c29f57482fd4c41a0640aab99eb5071d",
+                "sha256:6a007a541dff984264981fbafeb052bfe361db63578948d857907df9488d8774",
+                "sha256:6ee26e9dfb3996aff7c870f09dc7ad44a5f6732b8bdb5a5f9905737ac6fd4ef1",
+                "sha256:750de923b456ca8c0f1354d6befca45d1f3b3a789e76efc16741bd4132752d95",
+                "sha256:7c5ede2e2558f088c49a1ddda19080e4c23fb5d171de80a726b61b567e3766ed",
+                "sha256:830215173ad45d670140ff99aac3b461f9be9a6b11bee1a17265aaaa746a641a",
+                "sha256:8391cea5ce72f4a12368afd17799474015d5d3dc00c936a907eb7c7eaaea98a5",
+                "sha256:8940d6de7068af018dfa9a959a3510e9b7b543f4c405e88463a1cbaa3b2b379a",
+                "sha256:89a49cc5ad08a38b6141af17e00d1dd482dc927c7605bc77af457b5a0fca807c",
+                "sha256:900bc0096c2ca2d53f2e5cebf98293a7c32f532c4aeb926345e9747452233950",
+                "sha256:97e0efaebbfd222bcaac2f1735c010c1d3b167112d9d237daebbeedaaccf3d1d",
+                "sha256:9e04d4e4cfafa7c5264e535b5d28e786f0571bea609c3f0aaab13e891e933e9c",
+                "sha256:a4c60abd950d6de3e4f1ddbc318075654d275c29c846ab6a043d6ed2c52e4c8c",
+                "sha256:a6ff459dac39541e6a2763a4439c4ca6bc9ecb4acc05a99b79246751f9894756",
+                "sha256:a72797549935c9e0b9bc1def1768c8b5a709538fa6ab0678e671aec47ebfd55e",
+                "sha256:af4063ef2b11b96d949dccbc5a987272f38d55c23c4c01841ea65a517906397f",
+                "sha256:b975b85d1d5efc36cf8b237c5f3849b64d1ba33d6282f5e991f28751317504a1",
+                "sha256:bf0b9959e673505ee5869950642428046edb91f99942607c2ecf635f8a4b31c9",
+                "sha256:c0c85c5cbe8b30a32fa6d802588d55ffabf720e985abe9590c7c886919d875d4",
+                "sha256:c3f3237a57e42f79f1e560726576aedb3a7ef931f4e3accb84ebf6acc485d316",
+                "sha256:c3fa3ab0fb200a2c66493828ed06ccd1a94b12eddbfb985e7fd3e5723ff156c6",
+                "sha256:c435f5ce1705de48e08fcbcfaf8aee660d199c90536e3e06f2016af7d6a938dd",
+                "sha256:c90da4b124647547a68cf2f197174ada30c7bb9523cb976665dfd26a9963d328",
+                "sha256:cbdf2c498e077282cd427cfd88bdce4668019791deef0be8155385ab2ba7837f",
+                "sha256:d1fbad1f9077372b6587ec589c1fc120b417b6c8ad72d3e3cc86bbbd0a3cee93",
+                "sha256:d39f5d4af48c138cb146763eda14eb7d8b3ccbbec9fe86fb724cd16e0e914c64",
+                "sha256:ddb4a6061933bd9332b74eac0da25f17f32afa7145a33a0f9711ad74f924b1b8",
+                "sha256:ded637176addc1d3eef35331c39acc598bac550d213f0a1bedabfceaa2244c87",
+                "sha256:f20fd21f7538f8107451156dd1fe203300b79a9ddceba1ee0ac8132521a008ed",
+                "sha256:fda2783c12f553cdca11c08e5af6eecbd717280dc8fbe28a110897af1c15a88c"
             ],
-            "index": "pypi",
-            "version": "==1.50.0"
+            "version": "==1.56.2"
         },
         "grpcio-status": {
             "hashes": [
                 "sha256:2c33bbdbe20188b2953f46f31af669263b6ee2a9b2d38fa0d36ee091532e21bf",
                 "sha256:53695f45da07437b7c344ee4ef60d370fd2850179f5a28bb26d8e2aa1102ec11"
             ],
             "version": "==1.48.2"
@@ -571,18 +563,18 @@
                 "sha256:90261b206d6defd58fdd5e85f478bf633a2901798906be2ad389150c5c60edbe"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.1"
         },
         "jsonpointer": {
             "hashes": [
-                "sha256:51801e558539b4e9cd268638c078c6c5746c9ac96bc38152d443400e4f3793e9",
-                "sha256:97cba51526c829282218feb99dab1b1e6bdf8efd1c43dc9d57be093c0d69c99a"
+                "sha256:15d51bba20eea3165644553647711d150376234112651b4f1811022aecad7d7a",
+                "sha256:585cee82b70211fa9e6043b7bb89db6e1aa49524340dde8ad6b63206ea689d88"
             ],
-            "version": "==2.3"
+            "version": "==2.4"
         },
         "jsonschema": {
             "extras": [
                 "format_nongpl"
             ],
             "hashes": [
                 "sha256:4e5b3cf8216f577bee9ce139cbe72eca3ea4f292ec60928ff24758ce626cd163",
@@ -643,19 +635,19 @@
                 "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
             ],
             "index": "pypi",
             "version": "==2.1.1"
         },
         "natsort": {
             "hashes": [
-                "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
-                "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
+                "sha256:45312c4a0e5507593da193dedd04abb1469253b601ecaf63445ad80f0a1ea581",
+                "sha256:4732914fb471f56b5cce04d7bae6f164a592c7712e1c85f9ef585e197299521c"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==8.3.1"
+            "version": "==8.4.0"
         },
         "oauthlib": {
             "hashes": [
                 "sha256:8139f29aac13e25d502680e9e19963e83f16838d48a0d71c287fe40e7067fbca",
                 "sha256:9859c40929662bec5d64f34d01c99e093149682a3f38915dc0655d5a633dd918"
             ],
             "markers": "python_version >= '3.6'",
@@ -665,21 +657,14 @@
             "hashes": [
                 "sha256:9c31bd5cdbdbe5ef678cb01ac0564461790126acb9c3ab51a0f63fc9eaf608c8",
                 "sha256:aa629a2b75714a5c15c47125b6e1c4226492d7fe4c5b348c081c8b4cf87ce0ae"
             ],
             "index": "pypi",
             "version": "==0.9.14"
         },
-        "openshift": {
-            "hashes": [
-                "sha256:a060afb7565dda18b2749857867d80ab22b2f4143264519f493a9cabccc3b8a8"
-            ],
-            "index": "pypi",
-            "version": "==0.13.1"
-        },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
@@ -688,68 +673,60 @@
             "hashes": [
                 "sha256:e547125940bcc052856ded43be8e101f63828c2d94239ffbe2b327ba3d5ccf0a",
                 "sha256:e8dca2f4b43560edef58813969f52a56cef023146cbb8931626db80e6c1c4308"
             ],
             "index": "pypi",
             "version": "==5.9.0"
         },
-        "pip": {
-            "hashes": [
-                "sha256:0e7c86f486935893c708287b30bd050a36ac827ec7fe5e43fe7cb198dd835fba",
-                "sha256:3ef6ac33239e4027d9a5598a381b9d30880a1477e50039db2eac6e8a8f6d1b18"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.1.2"
-        },
         "pipenv": {
             "hashes": [
-                "sha256:3b80b4512934b9d8e8ce12c988394642ff96bb697680e5b092e59af503178327",
-                "sha256:f84d7119239b22ab2ac2b8fbc7d619d83cf41135206d72a17c4f151cda529fd0"
+                "sha256:116061545d4e2281cbc799f7736a715ee5ddf0a6f63c09f4263a4a6a0779fe93",
+                "sha256:404de9ff6a2464e20e52aaad71db2d4f8f2900f2177fc45a47f6315686cb2e5b"
             ],
             "index": "pypi",
-            "version": "==2022.1.8"
+            "version": "==2023.7.3"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:0ade98a4895e87dc51d47151f7d2ec290365a585151d97b4d8d6312ed6132fed",
-                "sha256:e48fabd87db8f3a7df7150a4a5ea22c546ee8bc39bc2473244730d4b56d2cc4e"
+                "sha256:69de5933ec873bd7ddae497f004be17cf200bce048dc987c28fc4e347d5349ff",
+                "sha256:e13f076e0f725f1beb58e7d26f80eff94099941740d3c664db03efecd6561271"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.3"
+            "version": "==2.6.1"
         },
         "pluggy": {
             "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
+                "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
+                "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.0.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.2.0"
         },
         "pprintpp": {
             "hashes": [
                 "sha256:b6b4dcdd0c0c0d75e4d7b2f21a9e933e5b2ce62b26e1a54537f9651ae5a5c01d",
                 "sha256:ea826108e2c7f49dc6d66c752973c3fc9749142a798d6b254e1e301cfdbc6403"
             ],
             "version": "==0.4.0"
         },
         "prettytable": {
             "hashes": [
-                "sha256:031eae6a9102017e8c7c7906460d150b7ed78b20fd1d8c8be4edaf88556c07ce",
-                "sha256:03481bca25ae0c28958c8cd6ac5165c159ce89f7ccde04d5c899b24b68bb13b7"
+                "sha256:ef8334ee40b7ec721651fc4d37ecc7bb2ef55fde5098d994438f0dfdaa385c0c",
+                "sha256:f4aaf2ed6e6062a82fd2e6e5289bbbe705ec2788fe401a3a1f62a1cea55526d2"
             ],
-            "markers": "python_version >= '3.8'",
-            "version": "==3.8.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.7.0"
         },
         "proto-plus": {
             "hashes": [
-                "sha256:0e8cda3d5a634d9895b75c573c9352c16486cb75deb0e078b5fda34db4243165",
-                "sha256:de34e52d6c9c6fcd704192f09767cb561bb4ee64e70eede20b0834d841f0be4d"
+                "sha256:a49cd903bc0b6ab41f76bf65510439d56ca76f868adf0274e738bfdd096894df",
+                "sha256:fdcd09713cbd42480740d2fe29c990f7fbd885a67efc328aa8be6ee3e9f76a6b"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==1.22.2"
+            "version": "==1.22.3"
         },
         "protobuf": {
             "hashes": [
                 "sha256:03038ac1cfbc41aa21f6afcbcd357281d7521b4157926f30ebecc8d4ea59dcb7",
                 "sha256:28545383d61f55b57cf4df63eebd9827754fd2dc25f80c5253f9184235db242c",
                 "sha256:2e3427429c9cffebf259491be0af70189607f365c2f41c7c3764af6f337105f2",
                 "sha256:398a9e0c3eaceb34ec1aee71894ca3299605fa8e761544934378bbc6c97de23b",
@@ -791,15 +768,15 @@
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==0.3.0"
         },
         "pycountry": {
             "hashes": [
                 "sha256:b2163a246c585894d808f18783e19137cb70a0c18fb36748dc01fc6f109c1646"
             ],
-            "markers": "python_version >= '3.6' and python_version < '4.0'",
+            "markers": "python_version >= '3.6' and python_version < '4'",
             "version": "==22.3.5"
         },
         "pycountry-convert": {
             "hashes": [
                 "sha256:095d310f746bf2a5ef713b3a82eea28a27262286223765b1e7be8a5c4fa7e9b9",
                 "sha256:5e33883a88b3cb752d332ca2358ac6c4de4defc86a2b93b713b36338e914952e"
             ],
@@ -818,19 +795,19 @@
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pyparsing": {
             "hashes": [
-                "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb",
-                "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
+                "sha256:d554a96d1a7d3ddaf7183104485bc19fd80543ad6ac5bdb6426719d766fb06c1",
+                "sha256:edb662d6fe322d6e990b1594b5feaeadf806803359e3d4d42f11e295e588f0ea"
             ],
             "markers": "python_full_version >= '3.6.8'",
-            "version": "==3.0.9"
+            "version": "==3.1.0"
         },
         "pyperclip": {
             "hashes": [
                 "sha256:105254a8b04934f0bc84e9c24eb360a591aaf6535c9def5f29d92af107a9bf57"
             ],
             "version": "==1.8.2"
         },
@@ -839,35 +816,35 @@
                 "sha256:cdc7b5e3ed77bed61270a47d35434a30617b9becdf2478af76ad2c6ade307280"
             ],
             "index": "pypi",
             "version": "==0.15.7"
         },
         "pytest": {
             "hashes": [
-                "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295",
-                "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"
+                "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
+                "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.3.2"
+            "version": "==7.4.0"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6",
                 "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.1.0"
         },
         "pytest-mock": {
             "hashes": [
-                "sha256:f4c973eeae0282963eb293eb173ce91b091a79c1334455acfac9ddee8a1c784b",
-                "sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f"
+                "sha256:21c279fff83d70763b05f8874cc9cfb3fcacd6d354247a976f9529d19f9acf39",
+                "sha256:7f6b125602ac6d743e523ae0bfa71e1a697a2f5534064528c6ff84c2f7c2fc7f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.10.0"
+            "version": "==3.11.1"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "index": "pypi",
@@ -877,67 +854,59 @@
             "hashes": [
                 "sha256:85ae778d8953aba87ad4b78aef7fbb5dae053980d2c20ff200bea29799685743",
                 "sha256:ad502b72b5d1137f4af37d4a68ae20fe7d6c9778f67cbe2aec566f7995053c7d"
             ],
             "index": "pypi",
             "version": "==3.13.0"
         },
-        "python-string-utils": {
-            "hashes": [
-                "sha256:dcf9060b03f07647c0a603408dc8b03f807f3b54a05c6e19eb14460256fac0cb",
-                "sha256:f1a88700baf99db1a9b6953f44181ad9ca56623c81e257e6009707e2e7851fa4"
-            ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.0"
-        },
         "pyyaml": {
             "hashes": [
-                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
-                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
-                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
-                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
-                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
-                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
-                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
-                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
-                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
-                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
-                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
-                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
-                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
-                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
-                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
-                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
-                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
-                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
-                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
-                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
-                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
-                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
-                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
-                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
-                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
-                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
-                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
-                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
-                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
-                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
-                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
-                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
-                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
-                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
-                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
-                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
-                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
-                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
-                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
-                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
+                "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
+                "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
+                "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
+                "sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27",
+                "sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595",
+                "sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62",
+                "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98",
+                "sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696",
+                "sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d",
+                "sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867",
+                "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47",
+                "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486",
+                "sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6",
+                "sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3",
+                "sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007",
+                "sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938",
+                "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
+                "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
+                "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
+                "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
+                "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
+                "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
+                "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
+                "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
+                "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
+                "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
+                "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
+                "sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924",
+                "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34",
+                "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43",
+                "sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859",
+                "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673",
+                "sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a",
+                "sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab",
+                "sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa",
+                "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c",
+                "sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585",
+                "sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d",
+                "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"
             ],
             "index": "pypi",
-            "version": "==6.0"
+            "version": "==6.0.1"
         },
         "redis": {
             "hashes": [
                 "sha256:68226f7ede928db8302f29ab088a157f41061fa946b7ae865452b6d7838bbffb",
                 "sha256:da92a39fec86438d3f1e2a1db33c312985806954fe860120b582a8430e231d8f"
             ],
             "index": "pypi",
@@ -1004,40 +973,83 @@
             "version": "==12.4.4"
         },
         "rsa": {
             "hashes": [
                 "sha256:90260d9058e514786967344d0ef75fa8727eed8a7d2e43ce9f4bcf1b536174f7",
                 "sha256:e38464a49c6c85d7f1351b0126661487a7e0a14a50f1675ec50eb34d4f20ef21"
             ],
-            "markers": "python_version >= '3.6' and python_version < '4.0'",
+            "markers": "python_version >= '3.6' and python_version < '4'",
             "version": "==4.9"
         },
         "ruamel.yaml": {
             "hashes": [
                 "sha256:742b35d3d665023981bd6d16b3d24248ce5df75fdb4e2924e93a05c1f8b61ca7",
                 "sha256:8b7ce697a2f212752a35c1ac414471dc16c424c9573be4926b56ff3f5d23b7af"
             ],
             "index": "pypi",
             "version": "==0.17.21"
         },
+        "ruamel.yaml.clib": {
+            "hashes": [
+                "sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e",
+                "sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3",
+                "sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5",
+                "sha256:1a6391a7cabb7641c32517539ca42cf84b87b667bad38b78d4d42dd23e957c81",
+                "sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497",
+                "sha256:2aa261c29a5545adfef9296b7e33941f46aa5bbd21164228e833412af4c9c75f",
+                "sha256:3110a99e0f94a4a3470ff67fc20d3f96c25b13d24c6980ff841e82bafe827cac",
+                "sha256:3243f48ecd450eddadc2d11b5feb08aca941b5cd98c9b1db14b2fd128be8c697",
+                "sha256:370445fd795706fd291ab00c9df38a0caed0f17a6fb46b0f607668ecb16ce763",
+                "sha256:40d030e2329ce5286d6b231b8726959ebbe0404c92f0a578c0e2482182e38282",
+                "sha256:41d0f1fa4c6830176eef5b276af04c89320ea616655d01327d5ce65e50575c94",
+                "sha256:4a4d8d417868d68b979076a9be6a38c676eca060785abaa6709c7b31593c35d1",
+                "sha256:4b3a93bb9bc662fc1f99c5c3ea8e623d8b23ad22f861eb6fce9377ac07ad6072",
+                "sha256:5bc0667c1eb8f83a3752b71b9c4ba55ef7c7058ae57022dd9b29065186a113d9",
+                "sha256:763d65baa3b952479c4e972669f679fe490eee058d5aa85da483ebae2009d231",
+                "sha256:7bdb4c06b063f6fd55e472e201317a3bb6cdeeee5d5a38512ea5c01e1acbdd93",
+                "sha256:8831a2cedcd0f0927f788c5bdf6567d9dc9cc235646a434986a852af1cb54b4b",
+                "sha256:91a789b4aa0097b78c93e3dc4b40040ba55bef518f84a40d4442f713b4094acb",
+                "sha256:92460ce908546ab69770b2e576e4f99fbb4ce6ab4b245345a3869a0a0410488f",
+                "sha256:99e77daab5d13a48a4054803d052ff40780278240a902b880dd37a51ba01a307",
+                "sha256:9c7617df90c1365638916b98cdd9be833d31d337dbcd722485597b43c4a215bf",
+                "sha256:a234a20ae07e8469da311e182e70ef6b199d0fbeb6c6cc2901204dd87fb867e8",
+                "sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b",
+                "sha256:be2a7ad8fd8f7442b24323d24ba0b56c51219513cfa45b9ada3b87b76c374d4b",
+                "sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640",
+                "sha256:c3ca1fbba4ae962521e5eb66d72998b51f0f4d0f608d3c0347a48e1af262efa7",
+                "sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a",
+                "sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71",
+                "sha256:d5e51e2901ec2366b79f16c2299a03e74ba4531ddcfacc1416639c557aef0ad8",
+                "sha256:da538167284de58a52109a9b89b8f6a53ff8437dd6dc26d33b57bf6699153122",
+                "sha256:debc87a9516b237d0466a711b18b6ebeb17ba9f391eb7f91c649c5c4ec5006c7",
+                "sha256:df5828871e6648db72d1c19b4bd24819b80a755c4541d3409f0f7acd0f335c80",
+                "sha256:ecdf1a604009bd35c674b9225a8fa609e0282d9b896c03dd441a91e5f53b534e",
+                "sha256:efa08d63ef03d079dcae1dfe334f6c8847ba8b645d08df286358b1f5293d24ab",
+                "sha256:f01da5790e95815eb5a8a138508c01c758e5f5bc0ce4286c4f7028b8dd7ac3d0",
+                "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646",
+                "sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38"
+            ],
+            "markers": "platform_python_implementation == 'CPython' and python_version < '3.11'",
+            "version": "==0.2.7"
+        },
         "s3transfer": {
             "hashes": [
                 "sha256:3c0da2d074bf35d6870ef157158641178a4204a6e689e82546083e31e0311346",
                 "sha256:640bb492711f4c0c0905e1f62b6aaeb771881935ad27884852411f8e9cacbca9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.6.1"
         },
         "setuptools": {
             "hashes": [
-                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
-                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.8.0"
+            "version": "==68.0.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
@@ -1063,14 +1075,22 @@
             "hashes": [
                 "sha256:2ecaede32fc25af814696374b79e42644ecaba5c09494c51016ffda9602d0f08",
                 "sha256:34761bae1a23c58192281a5115fb07fbf22c9b0133c08166beffc70fed3ebc12"
             ],
             "index": "pypi",
             "version": "==4.2.5"
         },
+        "tomli": {
+            "hashes": [
+                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
+                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==2.0.1"
+        },
         "typing-extensions": {
             "hashes": [
                 "sha256:1a9462dcc3347a79b1f1c0271fbe79e844580bb598bafa1ed208b94da3cdcd42",
                 "sha256:21c85e0fe4b9a155d0799430b0ad741cdce7e359660ccbd8b530613e8df88ce2"
             ],
             "index": "pypi",
             "version": "==4.1.1"
@@ -1089,19 +1109,19 @@
                 "sha256:cade07c403c397f9fe275492a48c1b869efd175d5d8a692df649e6e7e2ed8f4e"
             ],
             "index": "pypi",
             "version": "==0.18.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
-                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
+                "sha256:09ddbe1af0c8ed2bb4d6ed226b9e6415718ad18aef9fa0ba023d96b7a8356049",
+                "sha256:4c104ccde994f8b108163cf9ba58f3d11511d9403de87fb9b4f52bf33dbc8668"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.23.0"
+            "version": "==20.21.1"
         },
         "virtualenv-clone": {
             "hashes": [
                 "sha256:418ee935c36152f8f153c79824bb93eaf6f0f7984bae31d3f48f350b9183501a",
                 "sha256:44d5263bceed0bac3e1424d64f798095233b64def1c5689afa43dc3223caf5b0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1119,35 +1139,35 @@
                 "sha256:29bc7e8752c0a1bd4a1f03c14d6e6a72e93d82193738fa860cbff59d0fcc11bf",
                 "sha256:c225b674c83fa923be93d235330ce0300373d02885cef23238813b0d5668304a"
             ],
             "version": "==1.13"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:3566f8467cd350874c4913816355642a4942f6c1ed1e9406e3d42fae6d6c072a",
-                "sha256:b96f3bce3e54e3486ebe6504bc22bd4c140392bd2eb71764db29be8f2639aa65"
+                "sha256:c951af98631d24f8df89ab1019fc365f2227c0892f12fd150e935607c79dd0dd",
+                "sha256:f1f9f2ad5291f0225a49efad77abf9e700b6fef553900623060dad6e26503b9d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.5.3"
+            "version": "==1.6.1"
         },
         "werkzeug": {
             "hashes": [
-                "sha256:935539fa1413afbb9195b24880778422ed620c0fc09670945185cce4d91a8890",
-                "sha256:98c774df2f91b05550078891dee5f0eb0cb797a522c757a2452b9cee5b202330"
+                "sha256:2e1ccc9417d4da358b9de6f174e3ac094391ea1d4fbef2d667865d819dfd0afe",
+                "sha256:56433961bc1f12533306c624f3be5e744389ac61d722175d543e1751285da612"
             ],
-            "markers": "python_version >= '3.8'",
-            "version": "==2.3.6"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.2.3"
         },
         "wheel": {
             "hashes": [
-                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
-                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
+                "sha256:55a0f0a5a84869bce5ba775abfd9c462e3a6b1b7b7ec69d72c0b83d673a5114d",
+                "sha256:7e9be3bbd0078f6147d82ed9ed957e323e7708f57e134743d2edef3a7b7972a9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.40.0"
+            "version": "==0.41.0"
         },
         "zipp": {
             "hashes": [
                 "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
                 "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
```

### Comparing `unfurl-0.7.1/unfurl/templates/python3.7/Pipfile` & `unfurl-0.8.0/unfurl/templates/python3.7/Pipfile`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,48 @@
 [[source]]
-name = "pypi"
 url = "https://pypi.org/simple"
 verify_ssl = true
-
-[dev-packages]
+name = "pypi"
 
 [packages]
-pipenv = "==2022.1.8"
-click = ">=8.0.1"
-click-log = "*"
+pipenv = "==2023.7.3"
+click = "<8.1.4,>=8.0.1"
+pyrsistent = "==0.15.7"
 jsonschema = {version = "==3.2", extras = ["format_nongpl"]}
 "ruamel.yaml" = "==0.17.21"
-docker = {extras = ["tls"], version = "*"}
+charset-normalizer = "==2.1.1"
+cryptography = "==38.0.3"
+ansible-core = "==2.11.12"
+gitpython = "==3.1.30"
+rich = "==12.4.4"
 pbr = "==5.9.0"
 cliff = "==3.10.1"
+pyyaml = ">=6.0"
 python-dateutil = ">=2.8"
-six = ">=1.10.0"
 stevedore = "==3.5.0"
 requests = ">=2.14.2"
-enum34 = "*"
-subprocess32 = "*"
-ansible = "<5.0,>=4.2.0"
-mitogen = "==0.2.7"
-openshift = "==0.13.1"
-octodns = "==0.9.14"
-Jinja2 = "<=3.1.2"
-GitPython = "==3.1.30"
-Babel = "!=2.4.0,>=2.3.4"
-PyYAML = ">=6.0"
-boto = "*"
-boto3 = "*"
-supervisor = "*"
-google-auth = "*"
-pyrsistent = "==0.15.7"
 importlib-metadata = "<=4.12.0"
-cryptography = "==38.0.3"
+certifi = "*"
 itsdangerous = "==2.0.1"
-MarkupSafe = "<=2.1.1"
+markupsafe = "<=2.1.1"
+jinja2 = "<=3.1.2"
 typing-extensions = "==4.1.1"
-rich = "==12.4.4"
 flask = "<=2.1.3"
 flask-caching = "<=2.0.1"
+flask-cors = "==3.0.10"
 uvicorn = "<=0.18.2"
-google-cloud-compute = "==1.3.2"
-google-cloud-dns = "==0.34.0"
-grpcio = "==1.50.0"
 python-gitlab = "==3.13.0"
-certifi = "*"
+docker = {version = "*", extras = ["tls"]}
 kubernetes = "==24.2.0"
+octodns = "==0.9.14"
+boto3 = "*"
+supervisor = "*"
+google-cloud-compute = "==1.3.2"
+google-cloud-dns = "==0.34.0"
+google-auth = "*"
 gunicorn = "==20.1.0"
 redis = "==4.4.4"
-flask-cors = "==3.0.10"
-charset-normalizer = "==2.1.1"
+
+[dev-packages]
 
 [requires]
 python_version = "3.7"
```

### Comparing `unfurl-0.7.1/unfurl/templates/python3.7/Pipfile.lock` & `unfurl-0.8.0/unfurl/templates/python3.8/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9531695156695156%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'bc74a8f707316c6e372d81e12a6f5a74fb9b92602d795354c5bb254fc82795d1'}, 'requires': "*

 * *            "{'python_version': '3.8'}}",*

 * * "'default'": "{'ansible-core': {'hashes': "*

 * *              "['sha256:feb1df61738cfc1f5e893b42a2ec1a7de32977d67e86707b45eb63d0c5c3c236'], "*

 * *              "'version': '==2.12.10', 'index': 'pypi', delete: ['markers']}, 'boto3': {'hashes': "*

 * *              "['sha256:cfcb20d5784428f31d89889e68b26efeda90f231c3119eef4af8b25ad405c55f', "*

 * *        […]*

```diff
@@ -1,38 +1,31 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "a0c8310a0895d0e12e4e685e1c752eb8dfaeda2c108569a1c9f202a233878161"
+            "sha256": "bc74a8f707316c6e372d81e12a6f5a74fb9b92602d795354c5bb254fc82795d1"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.7"
+            "python_version": "3.8"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
-        "ansible": {
-            "hashes": [
-                "sha256:88af9479e81a3931bb3a1b8c4eeb252cd4f38c03daafd6a5aa120d6b0d70d45c"
-            ],
-            "index": "pypi",
-            "version": "==4.10.0"
-        },
         "ansible-core": {
             "hashes": [
-                "sha256:9159cc3b85e2d115f62f975b5155d96466e2a09a1c2e9b91de0c781f9089fc54"
+                "sha256:feb1df61738cfc1f5e893b42a2ec1a7de32977d67e86707b45eb63d0c5c3c236"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==2.11.12"
+            "index": "pypi",
+            "version": "==2.12.10"
         },
         "async-timeout": {
             "hashes": [
                 "sha256:2163e1640ddb52b7a8c80d0a67a08587e5d245cc9c553a74a847056bc2976b15",
                 "sha256:8ca1e4fcf50d07413d66d1a5e416e42cfdf5851c981d679a09851a6853383b3c"
             ],
             "markers": "python_version >= '3.6'",
@@ -50,53 +43,29 @@
             "hashes": [
                 "sha256:01be3ee61bb714e9090fcc5c10f4cf546c396331c620c6ae50a2321b28ed3199",
                 "sha256:0fbf5efbe78d466a26753e1dee3272423a3adc989d6a778c700e89a3f8ff0d88"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.5.1"
         },
-        "babel": {
-            "hashes": [
-                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
-                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
-            ],
-            "index": "pypi",
-            "version": "==2.12.1"
-        },
-        "boto": {
-            "hashes": [
-                "sha256:147758d41ae7240dc989f0039f27da8ca0d53734be0eb869ef16e3adcfa462e8",
-                "sha256:ea0d3b40a2d852767be77ca343b58a9e3a4b00d9db440efb8da74b4e58025e5a"
-            ],
-            "index": "pypi",
-            "version": "==2.49.0"
-        },
         "boto3": {
             "hashes": [
-                "sha256:a2778c5729d3dc0b3688c9f0d103543d7ec5ff44a4fd0e84d0d542e2dff05e62",
-                "sha256:ee0b8f8d238d4e1cf50fa6a185e4e066955b6105e9838a80b1b6582cd327dfdf"
+                "sha256:cfcb20d5784428f31d89889e68b26efeda90f231c3119eef4af8b25ad405c55f",
+                "sha256:d5ac6599951fdd519ed26c6fe15c41a7aa4021cb9adce33167344f8ce5cdb07b"
             ],
             "index": "pypi",
-            "version": "==1.26.152"
+            "version": "==1.28.12"
         },
         "botocore": {
             "hashes": [
-                "sha256:02a3205cc8579d4be6d537e63d72aebbf3f70f3aedcf40b3cae9dc2e24c774d0",
-                "sha256:f6319ecdbe3d325878f837cac2874e461b4d90691bb2d2186f980bce3b3cfcc8"
+                "sha256:7e5db466c762a071bb58c9a39d070f1333ce4f4ba6fdf9820ba21e87bd4c7e29",
+                "sha256:86380672151866b5e425636e3ebad74f2b83e7163e36ef5d38d11a04b9cba33b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.152"
-        },
-        "cached-property": {
-            "hashes": [
-                "sha256:9fa5755838eecbb2d234c3aa390bd80fbd3ac6b6869109bfc1b499f7bd89a130",
-                "sha256:df4f613cf7ad9a588cc381aaf4a512d26265ecebd5eb9e1ba12f1319eb85a6a0"
-            ],
-            "markers": "python_version < '3.8'",
-            "version": "==1.5.2"
+            "version": "==1.31.12"
         },
         "cachelib": {
             "hashes": [
                 "sha256:42d49f2fad9310dd946d7be73d46776bcd4d5fde4f49ad210cfdd447fbdfc346",
                 "sha256:593faeee62a7c037d50fc835617a01b887503f972fb52b188ae7e50e9cb69740"
             ],
             "markers": "python_version >= '3.7'",
@@ -108,19 +77,19 @@
                 "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.3.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "index": "pypi",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -199,22 +168,14 @@
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
             "version": "==8.1.3"
         },
-        "click-log": {
-            "hashes": [
-                "sha256:3970f8570ac54491237bcdb3d8ab5e3eef6c057df29f8c3d1151a51a9c23b975",
-                "sha256:a43e394b528d52112af599f2fc9e4b7cf3c15f94e53581f74fa6867e68c91756"
-            ],
-            "index": "pypi",
-            "version": "==0.4.0"
-        },
         "cliff": {
             "hashes": [
                 "sha256:045aee3f3c64471965d7ad507ce8474a4e2f20815fbb5405a770f8596a2a00a0",
                 "sha256:a21da482714b9f0b0e9bafaaf2f6a8b3b14161bb47f62e10e28d2fe4ff4b1626"
             ],
             "index": "pypi",
             "version": "==3.10.1"
@@ -333,62 +294,53 @@
                 "sha256:ed7b00096790213e09eb11c97cc6e2b757f15f3d2f85833cd2d3ec3fe37c1722"
             ],
             "index": "pypi",
             "version": "==38.0.3"
         },
         "distlib": {
             "hashes": [
-                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
-                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
+                "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057",
+                "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"
             ],
-            "version": "==0.3.6"
+            "version": "==0.3.7"
         },
         "dnspython": {
             "hashes": [
-                "sha256:224e32b03eb46be70e12ef6d64e0be123a64e621ab4c0822ff6d450d52a540b9",
-                "sha256:89141536394f909066cabd112e3e1a37e4e654db00a25308b0f130bc3152eb46"
+                "sha256:5b7488477388b8c0b70a8ce93b227c5603bc7b77f1565afe8e729c36c51447d7",
+                "sha256:c33971c79af5be968bb897e95c2448e11a645ee84d93b265ce0b7aabe5dfdca8"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4.0'",
-            "version": "==2.3.0"
+            "markers": "python_version >= '3.8' and python_version < '4.0'",
+            "version": "==2.4.1"
         },
         "docker": {
             "extras": [
                 "tls"
             ],
             "hashes": [
                 "sha256:aa6d17830045ba5ef0168d5eaa34d37beeb113948c413affe1d5991fc11f9a20",
                 "sha256:aecd2277b8bf8e506e484f6ab7aec39abe0038e29fa4a6d3ba86c3fe01844ed9"
             ],
             "index": "pypi",
             "version": "==6.1.3"
         },
-        "enum34": {
-            "hashes": [
-                "sha256:a98a201d6de3f2ab3db284e70a33b0f896fbf35f8086594e8c9e74b909058d53",
-                "sha256:c3858660960c984d6ab0ebad691265180da2b43f07e061c0f8dca9ef3cffd328",
-                "sha256:cce6a7477ed816bd2542d03d53db9f0db935dd013b70f336a95c73979289f248"
-            ],
-            "index": "pypi",
-            "version": "==1.1.10"
-        },
         "exceptiongroup": {
             "hashes": [
-                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
-                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
+                "sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5",
+                "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.1.1"
+            "version": "==1.1.2"
         },
         "filelock": {
             "hashes": [
-                "sha256:42f1e4ff2b497311213d61ad7aac5fed9050608e5309573f101eefa94143134a",
-                "sha256:82b1f7da46f0ae42abf1bc78e548667f484ac59d2bcec38c713cee7e2eb51e83"
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.12.1"
+            "version": "==3.12.2"
         },
         "flask": {
             "hashes": [
                 "sha256:15972e5017df0575c3d6c090ba168b6db90259e620ac8d7ea813a396bad5b6cb",
                 "sha256:9013281a7402ad527f8fd56375164f3aa021ecfaff89bfe3825346c24f87e04c"
             ],
             "index": "pypi",
@@ -411,15 +363,15 @@
             "version": "==3.0.10"
         },
         "fqdn": {
             "hashes": [
                 "sha256:105ed3677e767fb5ca086a0c1f4bb66ebc3c100be518f0e0d755d9eae164d89f",
                 "sha256:3a179af3761e4df6eb2e026ff9e1a3033d3587bf980a0b1b2e1e5d08d7358014"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4.0'",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
             "version": "==1.5.1"
         },
         "gitdb": {
             "hashes": [
                 "sha256:6eb990b69df4e15bad899ea868dc46572c3f75339735663b81de79b06f17eb9a",
                 "sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7"
             ],
@@ -435,43 +387,43 @@
             "version": "==3.1.30"
         },
         "google-api-core": {
             "extras": [
                 "grpc"
             ],
             "hashes": [
-                "sha256:4b9bb5d5a380a0befa0573b302651b8a9a89262c1730e37bf423cec511804c22",
-                "sha256:ce222e27b0de0d7bc63eb043b956996d6dccab14cc3b690aaea91c9cc99dc16e"
+                "sha256:25d29e05a0058ed5f19c61c0a78b1b53adea4d9364b464d014fbda941f6d1c9a",
+                "sha256:d92a5a92dc36dd4f4b9ee4e55528a90e432b059f93aee6ad857f9de8cc7ae94a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.11.0"
+            "version": "==2.11.1"
         },
         "google-auth": {
             "hashes": [
-                "sha256:a9cfa88b3e16196845e64a3658eb953992129d13ac7337b064c6546f77c17183",
-                "sha256:ea165e014c7cbd496558796b627c271aa8c18b4cba79dc1cc962b24c5efdfb85"
+                "sha256:164cba9af4e6e4e40c3a4f90a1a6c12ee56f14c0b4868d1ca91b32826ab334ce",
+                "sha256:d61d1b40897407b574da67da1a833bdc10d5a11642566e506565d1b1a46ba873"
             ],
             "index": "pypi",
-            "version": "==2.19.1"
+            "version": "==2.22.0"
         },
         "google-cloud-compute": {
             "hashes": [
                 "sha256:1ddd1be44d278754fc2643be7aa8d66838235ce44cfbacbeeadf3952ec020e95",
                 "sha256:21bd66251356d70bfd5f40211b42b936335490f7433b3b6fae7c498077e2c3fa"
             ],
             "index": "pypi",
             "version": "==1.3.2"
         },
         "google-cloud-core": {
             "hashes": [
-                "sha256:8417acf6466be2fa85123441696c4badda48db314c607cf1e5d543fa8bdc22fe",
-                "sha256:b9529ee7047fd8d4bf4a2182de619154240df17fbe60ead399078c1ae152af9a"
+                "sha256:37b80273c8d7eee1ae816b3a20ae43585ea50506cb0e60f3cf5be5f87f1373cb",
+                "sha256:fbd11cad3e98a7e5b0343dc07cb1039a5ffd7a5bb96e1f1e27cee4bda4a90863"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.3.2"
+            "version": "==2.3.3"
         },
         "google-cloud-dns": {
             "hashes": [
                 "sha256:41609782fa91df41e5ebfd48b127bb421a3b1821f5d49d900c484d13c0672167",
                 "sha256:bd75d6e9fd456ce643ee936a113a1ead5405704515caa679db30d7f036e447f3"
             ],
             "index": "pypi",
@@ -483,62 +435,61 @@
                 "sha256:b35d530fe825fb4227857bc47ad84c33c809ac96f312e13182bdeaa2abe1178a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.59.1"
         },
         "grpcio": {
             "hashes": [
-                "sha256:05f7c248e440f538aaad13eee78ef35f0541e73498dd6f832fe284542ac4b298",
-                "sha256:080b66253f29e1646ac53ef288c12944b131a2829488ac3bac8f52abb4413c0d",
-                "sha256:12b479839a5e753580b5e6053571de14006157f2ef9b71f38c56dc9b23b95ad6",
-                "sha256:156f8009e36780fab48c979c5605eda646065d4695deea4cfcbcfdd06627ddb6",
-                "sha256:15f9e6d7f564e8f0776770e6ef32dac172c6f9960c478616c366862933fa08b4",
-                "sha256:177afaa7dba3ab5bfc211a71b90da1b887d441df33732e94e26860b3321434d9",
-                "sha256:1a4cd8cb09d1bc70b3ea37802be484c5ae5a576108bad14728f2516279165dd7",
-                "sha256:1d8d02dbb616c0a9260ce587eb751c9c7dc689bc39efa6a88cc4fa3e9c138a7b",
-                "sha256:2b71916fa8f9eb2abd93151fafe12e18cebb302686b924bd4ec39266211da525",
-                "sha256:2d9fd6e38b16c4d286a01e1776fdf6c7a4123d99ae8d6b3f0b4a03a34bf6ce45",
-                "sha256:3b611b3de3dfd2c47549ca01abfa9bbb95937eb0ea546ea1d762a335739887be",
-                "sha256:3e4244c09cc1b65c286d709658c061f12c61c814be0b7030a2d9966ff02611e0",
-                "sha256:40838061e24f960b853d7bce85086c8e1b81c6342b1f4c47ff0edd44bbae2722",
-                "sha256:4b123fbb7a777a2fedec684ca0b723d85e1d2379b6032a9a9b7851829ed3ca9a",
-                "sha256:531f8b46f3d3db91d9ef285191825d108090856b3bc86a75b7c3930f16ce432f",
-                "sha256:67dd41a31f6fc5c7db097a5c14a3fa588af54736ffc174af4411d34c4f306f68",
-                "sha256:7489dbb901f4fdf7aec8d3753eadd40839c9085967737606d2c35b43074eea24",
-                "sha256:8d4c8e73bf20fb53fe5a7318e768b9734cf122fe671fcce75654b98ba12dfb75",
-                "sha256:8e69aa4e9b7f065f01d3fdcecbe0397895a772d99954bb82eefbb1682d274518",
-                "sha256:8e8999a097ad89b30d584c034929f7c0be280cd7851ac23e9067111167dcbf55",
-                "sha256:906f4d1beb83b3496be91684c47a5d870ee628715227d5d7c54b04a8de802974",
-                "sha256:92d7635d1059d40d2ec29c8bf5ec58900120b3ce5150ef7414119430a4b2dd5c",
-                "sha256:931e746d0f75b2a5cff0a1197d21827a3a2f400c06bace036762110f19d3d507",
-                "sha256:95ce51f7a09491fb3da8cf3935005bff19983b77c4e9437ef77235d787b06842",
-                "sha256:9eea18a878cffc804506d39c6682d71f6b42ec1c151d21865a95fae743fda500",
-                "sha256:a23d47f2fc7111869f0ff547f771733661ff2818562b04b9ed674fa208e261f4",
-                "sha256:a4c23e54f58e016761b576976da6a34d876420b993f45f66a2bfb00363ecc1f9",
-                "sha256:a50a1be449b9e238b9bd43d3857d40edf65df9416dea988929891d92a9f8a778",
-                "sha256:ab5d0e3590f0a16cb88de4a3fa78d10eb66a84ca80901eb2c17c1d2c308c230f",
-                "sha256:ae23daa7eda93c1c49a9ecc316e027ceb99adbad750fbd3a56fa9e4a2ffd5ae0",
-                "sha256:af98d49e56605a2912cf330b4627e5286243242706c3a9fa0bcec6e6f68646fc",
-                "sha256:b2f77a90ba7b85bfb31329f8eab9d9540da2cf8a302128fb1241d7ea239a5469",
-                "sha256:baab51dcc4f2aecabf4ed1e2f57bceab240987c8b03533f1cef90890e6502067",
-                "sha256:ca8a2254ab88482936ce941485c1c20cdeaef0efa71a61dbad171ab6758ec998",
-                "sha256:cb11464f480e6103c59d558a3875bd84eed6723f0921290325ebe97262ae1347",
-                "sha256:ce8513aee0af9c159319692bfbf488b718d1793d764798c3d5cff827a09e25ef",
-                "sha256:cf151f97f5f381163912e8952eb5b3afe89dec9ed723d1561d59cabf1e219a35",
-                "sha256:d144ad10eeca4c1d1ce930faa105899f86f5d99cecfe0d7224f3c4c76265c15e",
-                "sha256:d534d169673dd5e6e12fb57cc67664c2641361e1a0885545495e65a7b761b0f4",
-                "sha256:d75061367a69808ab2e84c960e9dce54749bcc1e44ad3f85deee3a6c75b4ede9",
-                "sha256:d84d04dec64cc4ed726d07c5d17b73c343c8ddcd6b59c7199c801d6bbb9d9ed1",
-                "sha256:de411d2b030134b642c092e986d21aefb9d26a28bf5a18c47dd08ded411a3bc5",
-                "sha256:e07fe0d7ae395897981d16be61f0db9791f482f03fee7d1851fe20ddb4f69c03",
-                "sha256:ea8ccf95e4c7e20419b7827aa5b6da6f02720270686ac63bd3493a651830235c",
-                "sha256:f7025930039a011ed7d7e7ef95a1cb5f516e23c5a6ecc7947259b67bea8e06ca"
+                "sha256:06e84ad9ae7668a109e970c7411e7992751a116494cba7c4fb877656527f9a57",
+                "sha256:0ff789ae7d8ddd76d2ac02e7d13bfef6fc4928ac01e1dcaa182be51b6bcc0aaa",
+                "sha256:10954662f77dc36c9a1fb5cc4a537f746580d6b5734803be1e587252682cda8d",
+                "sha256:139f66656a762572ae718fa0d1f2dce47c05e9fbf7a16acd704c354405b97df9",
+                "sha256:1c31e52a04e62c8577a7bf772b3e7bed4df9c9e0dd90f92b6ffa07c16cab63c9",
+                "sha256:33971197c47965cc1d97d78d842163c283e998223b151bab0499b951fd2c0b12",
+                "sha256:345356b307cce5d14355e8e055b4ca5f99bc857c33a3dc1ddbc544fca9cd0475",
+                "sha256:373b48f210f43327a41e397391715cd11cfce9ded2fe76a5068f9bacf91cc226",
+                "sha256:3ccb621749a81dc7755243665a70ce45536ec413ef5818e013fe8dfbf5aa497b",
+                "sha256:42a3bbb2bc07aef72a7d97e71aabecaf3e4eb616d39e5211e2cfe3689de860ca",
+                "sha256:42e63904ee37ae46aa23de50dac8b145b3596f43598fa33fe1098ab2cbda6ff5",
+                "sha256:4eb37dd8dd1aa40d601212afa27ca5be255ba792e2e0b24d67b8af5e012cdb7d",
+                "sha256:51173e8fa6d9a2d85c14426bdee5f5c4a0654fd5fddcc21fe9d09ab0f6eb8b35",
+                "sha256:5144feb20fe76e73e60c7d73ec3bf54f320247d1ebe737d10672480371878b48",
+                "sha256:5344be476ac37eb9c9ad09c22f4ea193c1316bf074f1daf85bddb1b31fda5116",
+                "sha256:6108e5933eb8c22cd3646e72d5b54772c29f57482fd4c41a0640aab99eb5071d",
+                "sha256:6a007a541dff984264981fbafeb052bfe361db63578948d857907df9488d8774",
+                "sha256:6ee26e9dfb3996aff7c870f09dc7ad44a5f6732b8bdb5a5f9905737ac6fd4ef1",
+                "sha256:750de923b456ca8c0f1354d6befca45d1f3b3a789e76efc16741bd4132752d95",
+                "sha256:7c5ede2e2558f088c49a1ddda19080e4c23fb5d171de80a726b61b567e3766ed",
+                "sha256:830215173ad45d670140ff99aac3b461f9be9a6b11bee1a17265aaaa746a641a",
+                "sha256:8391cea5ce72f4a12368afd17799474015d5d3dc00c936a907eb7c7eaaea98a5",
+                "sha256:8940d6de7068af018dfa9a959a3510e9b7b543f4c405e88463a1cbaa3b2b379a",
+                "sha256:89a49cc5ad08a38b6141af17e00d1dd482dc927c7605bc77af457b5a0fca807c",
+                "sha256:900bc0096c2ca2d53f2e5cebf98293a7c32f532c4aeb926345e9747452233950",
+                "sha256:97e0efaebbfd222bcaac2f1735c010c1d3b167112d9d237daebbeedaaccf3d1d",
+                "sha256:9e04d4e4cfafa7c5264e535b5d28e786f0571bea609c3f0aaab13e891e933e9c",
+                "sha256:a4c60abd950d6de3e4f1ddbc318075654d275c29c846ab6a043d6ed2c52e4c8c",
+                "sha256:a6ff459dac39541e6a2763a4439c4ca6bc9ecb4acc05a99b79246751f9894756",
+                "sha256:a72797549935c9e0b9bc1def1768c8b5a709538fa6ab0678e671aec47ebfd55e",
+                "sha256:af4063ef2b11b96d949dccbc5a987272f38d55c23c4c01841ea65a517906397f",
+                "sha256:b975b85d1d5efc36cf8b237c5f3849b64d1ba33d6282f5e991f28751317504a1",
+                "sha256:bf0b9959e673505ee5869950642428046edb91f99942607c2ecf635f8a4b31c9",
+                "sha256:c0c85c5cbe8b30a32fa6d802588d55ffabf720e985abe9590c7c886919d875d4",
+                "sha256:c3f3237a57e42f79f1e560726576aedb3a7ef931f4e3accb84ebf6acc485d316",
+                "sha256:c3fa3ab0fb200a2c66493828ed06ccd1a94b12eddbfb985e7fd3e5723ff156c6",
+                "sha256:c435f5ce1705de48e08fcbcfaf8aee660d199c90536e3e06f2016af7d6a938dd",
+                "sha256:c90da4b124647547a68cf2f197174ada30c7bb9523cb976665dfd26a9963d328",
+                "sha256:cbdf2c498e077282cd427cfd88bdce4668019791deef0be8155385ab2ba7837f",
+                "sha256:d1fbad1f9077372b6587ec589c1fc120b417b6c8ad72d3e3cc86bbbd0a3cee93",
+                "sha256:d39f5d4af48c138cb146763eda14eb7d8b3ccbbec9fe86fb724cd16e0e914c64",
+                "sha256:ddb4a6061933bd9332b74eac0da25f17f32afa7145a33a0f9711ad74f924b1b8",
+                "sha256:ded637176addc1d3eef35331c39acc598bac550d213f0a1bedabfceaa2244c87",
+                "sha256:f20fd21f7538f8107451156dd1fe203300b79a9ddceba1ee0ac8132521a008ed",
+                "sha256:fda2783c12f553cdca11c08e5af6eecbd717280dc8fbe28a110897af1c15a88c"
             ],
-            "index": "pypi",
-            "version": "==1.50.0"
+            "version": "==1.56.2"
         },
         "grpcio-status": {
             "hashes": [
                 "sha256:2c33bbdbe20188b2953f46f31af669263b6ee2a9b2d38fa0d36ee091532e21bf",
                 "sha256:53695f45da07437b7c344ee4ef60d370fd2850179f5a28bb26d8e2aa1102ec11"
             ],
             "version": "==1.48.2"
@@ -604,18 +555,18 @@
                 "sha256:90261b206d6defd58fdd5e85f478bf633a2901798906be2ad389150c5c60edbe"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.1"
         },
         "jsonpointer": {
             "hashes": [
-                "sha256:51801e558539b4e9cd268638c078c6c5746c9ac96bc38152d443400e4f3793e9",
-                "sha256:97cba51526c829282218feb99dab1b1e6bdf8efd1c43dc9d57be093c0d69c99a"
+                "sha256:15d51bba20eea3165644553647711d150376234112651b4f1811022aecad7d7a",
+                "sha256:585cee82b70211fa9e6043b7bb89db6e1aa49524340dde8ad6b63206ea689d88"
             ],
-            "version": "==2.3"
+            "version": "==2.4"
         },
         "jsonschema": {
             "extras": [
                 "format_nongpl"
             ],
             "hashes": [
                 "sha256:4e5b3cf8216f577bee9ce139cbe72eca3ea4f292ec60928ff24758ce626cd163",
@@ -674,28 +625,21 @@
                 "sha256:efc1913fd2ca4f334418481c7e595c00aad186563bbc1ec76067848c7ca0a933",
                 "sha256:f121a1420d4e173a5d96e47e9a0c0dcff965afdf1626d28de1460815f7c4ee7a",
                 "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
             ],
             "index": "pypi",
             "version": "==2.1.1"
         },
-        "mitogen": {
-            "hashes": [
-                "sha256:c2dd28d6b964699822455f6c91acedc16324913586837f046a76e2e4ac1d716c"
-            ],
-            "index": "pypi",
-            "version": "==0.2.7"
-        },
         "natsort": {
             "hashes": [
-                "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
-                "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
+                "sha256:45312c4a0e5507593da193dedd04abb1469253b601ecaf63445ad80f0a1ea581",
+                "sha256:4732914fb471f56b5cce04d7bae6f164a592c7712e1c85f9ef585e197299521c"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==8.3.1"
+            "version": "==8.4.0"
         },
         "oauthlib": {
             "hashes": [
                 "sha256:8139f29aac13e25d502680e9e19963e83f16838d48a0d71c287fe40e7067fbca",
                 "sha256:9859c40929662bec5d64f34d01c99e093149682a3f38915dc0655d5a633dd918"
             ],
             "markers": "python_version >= '3.6'",
@@ -705,21 +649,14 @@
             "hashes": [
                 "sha256:9c31bd5cdbdbe5ef678cb01ac0564461790126acb9c3ab51a0f63fc9eaf608c8",
                 "sha256:aa629a2b75714a5c15c47125b6e1c4226492d7fe4c5b348c081c8b4cf87ce0ae"
             ],
             "index": "pypi",
             "version": "==0.9.14"
         },
-        "openshift": {
-            "hashes": [
-                "sha256:a060afb7565dda18b2749857867d80ab22b2f4143264519f493a9cabccc3b8a8"
-            ],
-            "index": "pypi",
-            "version": "==0.13.1"
-        },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
@@ -728,68 +665,60 @@
             "hashes": [
                 "sha256:e547125940bcc052856ded43be8e101f63828c2d94239ffbe2b327ba3d5ccf0a",
                 "sha256:e8dca2f4b43560edef58813969f52a56cef023146cbb8931626db80e6c1c4308"
             ],
             "index": "pypi",
             "version": "==5.9.0"
         },
-        "pip": {
-            "hashes": [
-                "sha256:0e7c86f486935893c708287b30bd050a36ac827ec7fe5e43fe7cb198dd835fba",
-                "sha256:3ef6ac33239e4027d9a5598a381b9d30880a1477e50039db2eac6e8a8f6d1b18"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.1.2"
-        },
         "pipenv": {
             "hashes": [
-                "sha256:3b80b4512934b9d8e8ce12c988394642ff96bb697680e5b092e59af503178327",
-                "sha256:f84d7119239b22ab2ac2b8fbc7d619d83cf41135206d72a17c4f151cda529fd0"
+                "sha256:116061545d4e2281cbc799f7736a715ee5ddf0a6f63c09f4263a4a6a0779fe93",
+                "sha256:404de9ff6a2464e20e52aaad71db2d4f8f2900f2177fc45a47f6315686cb2e5b"
             ],
             "index": "pypi",
-            "version": "==2022.1.8"
+            "version": "==2023.7.3"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:69de5933ec873bd7ddae497f004be17cf200bce048dc987c28fc4e347d5349ff",
-                "sha256:e13f076e0f725f1beb58e7d26f80eff94099941740d3c664db03efecd6561271"
+                "sha256:1b42b450ad933e981d56e59f1b97495428c9bd60698baab9f3eb3d00d5822421",
+                "sha256:ad8291ae0ae5072f66c16945166cb11c63394c7a3ad1b1bc9828ca3162da8c2f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.6.1"
+            "version": "==3.9.1"
         },
         "pluggy": {
             "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
+                "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
+                "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.0.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.2.0"
         },
         "pprintpp": {
             "hashes": [
                 "sha256:b6b4dcdd0c0c0d75e4d7b2f21a9e933e5b2ce62b26e1a54537f9651ae5a5c01d",
                 "sha256:ea826108e2c7f49dc6d66c752973c3fc9749142a798d6b254e1e301cfdbc6403"
             ],
             "version": "==0.4.0"
         },
         "prettytable": {
             "hashes": [
-                "sha256:ef8334ee40b7ec721651fc4d37ecc7bb2ef55fde5098d994438f0dfdaa385c0c",
-                "sha256:f4aaf2ed6e6062a82fd2e6e5289bbbe705ec2788fe401a3a1f62a1cea55526d2"
+                "sha256:031eae6a9102017e8c7c7906460d150b7ed78b20fd1d8c8be4edaf88556c07ce",
+                "sha256:03481bca25ae0c28958c8cd6ac5165c159ce89f7ccde04d5c899b24b68bb13b7"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.7.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.8.0"
         },
         "proto-plus": {
             "hashes": [
-                "sha256:0e8cda3d5a634d9895b75c573c9352c16486cb75deb0e078b5fda34db4243165",
-                "sha256:de34e52d6c9c6fcd704192f09767cb561bb4ee64e70eede20b0834d841f0be4d"
+                "sha256:a49cd903bc0b6ab41f76bf65510439d56ca76f868adf0274e738bfdd096894df",
+                "sha256:fdcd09713cbd42480740d2fe29c990f7fbd885a67efc328aa8be6ee3e9f76a6b"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==1.22.2"
+            "version": "==1.22.3"
         },
         "protobuf": {
             "hashes": [
                 "sha256:03038ac1cfbc41aa21f6afcbcd357281d7521b4157926f30ebecc8d4ea59dcb7",
                 "sha256:28545383d61f55b57cf4df63eebd9827754fd2dc25f80c5253f9184235db242c",
                 "sha256:2e3427429c9cffebf259491be0af70189607f365c2f41c7c3764af6f337105f2",
                 "sha256:398a9e0c3eaceb34ec1aee71894ca3299605fa8e761544934378bbc6c97de23b",
@@ -831,15 +760,15 @@
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==0.3.0"
         },
         "pycountry": {
             "hashes": [
                 "sha256:b2163a246c585894d808f18783e19137cb70a0c18fb36748dc01fc6f109c1646"
             ],
-            "markers": "python_version >= '3.6' and python_version < '4.0'",
+            "markers": "python_version >= '3.6' and python_version < '4'",
             "version": "==22.3.5"
         },
         "pycountry-convert": {
             "hashes": [
                 "sha256:095d310f746bf2a5ef713b3a82eea28a27262286223765b1e7be8a5c4fa7e9b9",
                 "sha256:5e33883a88b3cb752d332ca2358ac6c4de4defc86a2b93b713b36338e914952e"
             ],
@@ -858,19 +787,19 @@
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pyparsing": {
             "hashes": [
-                "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb",
-                "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
+                "sha256:d554a96d1a7d3ddaf7183104485bc19fd80543ad6ac5bdb6426719d766fb06c1",
+                "sha256:edb662d6fe322d6e990b1594b5feaeadf806803359e3d4d42f11e295e588f0ea"
             ],
             "markers": "python_full_version >= '3.6.8'",
-            "version": "==3.0.9"
+            "version": "==3.1.0"
         },
         "pyperclip": {
             "hashes": [
                 "sha256:105254a8b04934f0bc84e9c24eb360a591aaf6535c9def5f29d92af107a9bf57"
             ],
             "version": "==1.8.2"
         },
@@ -879,35 +808,35 @@
                 "sha256:cdc7b5e3ed77bed61270a47d35434a30617b9becdf2478af76ad2c6ade307280"
             ],
             "index": "pypi",
             "version": "==0.15.7"
         },
         "pytest": {
             "hashes": [
-                "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295",
-                "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"
+                "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
+                "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.3.2"
+            "version": "==7.4.0"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6",
                 "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.1.0"
         },
         "pytest-mock": {
             "hashes": [
-                "sha256:f4c973eeae0282963eb293eb173ce91b091a79c1334455acfac9ddee8a1c784b",
-                "sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f"
+                "sha256:21c279fff83d70763b05f8874cc9cfb3fcacd6d354247a976f9529d19f9acf39",
+                "sha256:7f6b125602ac6d743e523ae0bfa71e1a697a2f5534064528c6ff84c2f7c2fc7f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.10.0"
+            "version": "==3.11.1"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "index": "pypi",
@@ -917,75 +846,59 @@
             "hashes": [
                 "sha256:85ae778d8953aba87ad4b78aef7fbb5dae053980d2c20ff200bea29799685743",
                 "sha256:ad502b72b5d1137f4af37d4a68ae20fe7d6c9778f67cbe2aec566f7995053c7d"
             ],
             "index": "pypi",
             "version": "==3.13.0"
         },
-        "python-string-utils": {
-            "hashes": [
-                "sha256:dcf9060b03f07647c0a603408dc8b03f807f3b54a05c6e19eb14460256fac0cb",
-                "sha256:f1a88700baf99db1a9b6953f44181ad9ca56623c81e257e6009707e2e7851fa4"
-            ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.0"
-        },
-        "pytz": {
-            "hashes": [
-                "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
-                "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
-            ],
-            "markers": "python_version < '3.9'",
-            "version": "==2023.3"
-        },
         "pyyaml": {
             "hashes": [
-                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
-                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
-                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
-                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
-                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
-                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
-                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
-                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
-                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
-                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
-                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
-                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
-                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
-                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
-                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
-                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
-                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
-                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
-                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
-                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
-                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
-                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
-                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
-                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
-                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
-                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
-                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
-                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
-                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
-                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
-                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
-                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
-                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
-                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
-                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
-                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
-                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
-                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
-                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
-                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
+                "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
+                "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
+                "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
+                "sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27",
+                "sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595",
+                "sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62",
+                "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98",
+                "sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696",
+                "sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d",
+                "sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867",
+                "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47",
+                "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486",
+                "sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6",
+                "sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3",
+                "sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007",
+                "sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938",
+                "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
+                "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
+                "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
+                "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
+                "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
+                "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
+                "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
+                "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
+                "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
+                "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
+                "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
+                "sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924",
+                "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34",
+                "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43",
+                "sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859",
+                "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673",
+                "sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a",
+                "sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab",
+                "sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa",
+                "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c",
+                "sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585",
+                "sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d",
+                "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"
             ],
             "index": "pypi",
-            "version": "==6.0"
+            "version": "==6.0.1"
         },
         "redis": {
             "hashes": [
                 "sha256:68226f7ede928db8302f29ab088a157f41061fa946b7ae865452b6d7838bbffb",
                 "sha256:da92a39fec86438d3f1e2a1db33c312985806954fe860120b582a8430e231d8f"
             ],
             "index": "pypi",
@@ -1052,15 +965,15 @@
             "version": "==12.4.4"
         },
         "rsa": {
             "hashes": [
                 "sha256:90260d9058e514786967344d0ef75fa8727eed8a7d2e43ce9f4bcf1b536174f7",
                 "sha256:e38464a49c6c85d7f1351b0126661487a7e0a14a50f1675ec50eb34d4f20ef21"
             ],
-            "markers": "python_version >= '3.6' and python_version < '4.0'",
+            "markers": "python_version >= '3.6' and python_version < '4'",
             "version": "==4.9"
         },
         "ruamel.yaml": {
             "hashes": [
                 "sha256:742b35d3d665023981bd6d16b3d24248ce5df75fdb4e2924e93a05c1f8b61ca7",
                 "sha256:8b7ce697a2f212752a35c1ac414471dc16c424c9573be4926b56ff3f5d23b7af"
             ],
@@ -1116,26 +1029,26 @@
                 "sha256:640bb492711f4c0c0905e1f62b6aaeb771881935ad27884852411f8e9cacbca9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.6.1"
         },
         "setuptools": {
             "hashes": [
-                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
-                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.8.0"
+            "version": "==68.0.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
-            "index": "pypi",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
             "version": "==1.16.0"
         },
         "smmap": {
             "hashes": [
                 "sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94",
                 "sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936"
             ],
@@ -1146,23 +1059,14 @@
             "hashes": [
                 "sha256:a547de73308fd7e90075bb4d301405bebf705292fa90a90fc3bcf9133f58616c",
                 "sha256:f40253887d8712eaa2bb0ea3830374416736dc8ec0e22f5a65092c1174c44335"
             ],
             "index": "pypi",
             "version": "==3.5.0"
         },
-        "subprocess32": {
-            "hashes": [
-                "sha256:88e37c1aac5388df41cc8a8456bb49ebffd321a3ad4d70358e3518176de3a56b",
-                "sha256:e45d985aef903c5b7444d34350b05da91a9e0ea015415ab45a21212786c649d0",
-                "sha256:eb2937c80497978d181efa1b839ec2d9622cf9600a039a79d0e108d1f9aec79d"
-            ],
-            "index": "pypi",
-            "version": "==3.5.4"
-        },
         "supervisor": {
             "hashes": [
                 "sha256:2ecaede32fc25af814696374b79e42644ecaba5c09494c51016ffda9602d0f08",
                 "sha256:34761bae1a23c58192281a5115fb07fbf22c9b0133c08166beffc70fed3ebc12"
             ],
             "index": "pypi",
             "version": "==4.2.5"
@@ -1197,19 +1101,19 @@
                 "sha256:cade07c403c397f9fe275492a48c1b869efd175d5d8a692df649e6e7e2ed8f4e"
             ],
             "index": "pypi",
             "version": "==0.18.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:09ddbe1af0c8ed2bb4d6ed226b9e6415718ad18aef9fa0ba023d96b7a8356049",
-                "sha256:4c104ccde994f8b108163cf9ba58f3d11511d9403de87fb9b4f52bf33dbc8668"
+                "sha256:43a3052be36080548bdee0b42919c88072037d50d56c28bd3f853cbe92b953ff",
+                "sha256:fd8a78f46f6b99a67b7ec5cf73f92357891a7b3a40fd97637c27f854aae3b9e0"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.21.1"
+            "version": "==20.24.2"
         },
         "virtualenv-clone": {
             "hashes": [
                 "sha256:418ee935c36152f8f153c79824bb93eaf6f0f7984bae31d3f48f350b9183501a",
                 "sha256:44d5263bceed0bac3e1424d64f798095233b64def1c5689afa43dc3223caf5b0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1227,40 +1131,40 @@
                 "sha256:29bc7e8752c0a1bd4a1f03c14d6e6a72e93d82193738fa860cbff59d0fcc11bf",
                 "sha256:c225b674c83fa923be93d235330ce0300373d02885cef23238813b0d5668304a"
             ],
             "version": "==1.13"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:3566f8467cd350874c4913816355642a4942f6c1ed1e9406e3d42fae6d6c072a",
-                "sha256:b96f3bce3e54e3486ebe6504bc22bd4c140392bd2eb71764db29be8f2639aa65"
+                "sha256:c951af98631d24f8df89ab1019fc365f2227c0892f12fd150e935607c79dd0dd",
+                "sha256:f1f9f2ad5291f0225a49efad77abf9e700b6fef553900623060dad6e26503b9d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.5.3"
+            "version": "==1.6.1"
         },
         "werkzeug": {
             "hashes": [
-                "sha256:2e1ccc9417d4da358b9de6f174e3ac094391ea1d4fbef2d667865d819dfd0afe",
-                "sha256:56433961bc1f12533306c624f3be5e744389ac61d722175d543e1751285da612"
+                "sha256:935539fa1413afbb9195b24880778422ed620c0fc09670945185cce4d91a8890",
+                "sha256:98c774df2f91b05550078891dee5f0eb0cb797a522c757a2452b9cee5b202330"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.2.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.3.6"
         },
         "wheel": {
             "hashes": [
-                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
-                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
+                "sha256:55a0f0a5a84869bce5ba775abfd9c462e3a6b1b7b7ec69d72c0b83d673a5114d",
+                "sha256:7e9be3bbd0078f6147d82ed9ed957e323e7708f57e134743d2edef3a7b7972a9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.40.0"
+            "version": "==0.41.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
-                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
+                "sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0",
+                "sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.15.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.16.2"
         }
     },
     "develop": {}
 }
```

### Comparing `unfurl-0.7.1/unfurl/templates/python3.8/Pipfile` & `unfurl-0.8.0/unfurl/templates/python3.8/Pipfile`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,48 @@
 [[source]]
-name = "pypi"
 url = "https://pypi.org/simple"
 verify_ssl = true
-
-[dev-packages]
+name = "pypi"
 
 [packages]
-pipenv = "==2022.1.8"
-click = ">=8.0.1"
-click-log = "*"
+pipenv = "==2023.7.3"
+click = ">=8.0.1,<8.1.4"
+pyrsistent = "==0.15.7"
 jsonschema = {version = "==3.2", extras = ["format_nongpl"]}
 "ruamel.yaml" = "==0.17.21"
-docker = {extras = ["tls"], version = "*"}
+charset-normalizer = "==2.1.1"
+cryptography = "==38.0.3"
+ansible-core = "==2.12.10"
+gitpython = "==3.1.30"
+rich = "==12.4.4"
 pbr = "==5.9.0"
 cliff = "==3.10.1"
+pyyaml = ">=6.0"
 python-dateutil = ">=2.8"
-six = ">=1.10.0"
 stevedore = "==3.5.0"
 requests = ">=2.14.2"
-enum34 = "*"
-Jinja2 = "<=3.1.2"
-GitPython = "==3.1.30"
-Babel = ">=2.3.4,!=2.4.0"
-PyYAML = ">=6.0"
-subprocess32 = "*"
-ansible = "<5.0,>=4.2.0"
-mitogen = "==0.2.7"
-openshift = "==0.13.1"
-octodns = "==0.9.14"
-boto = "*"
-boto3 = "*"
-supervisor = "*"
-pyrsistent = "==0.15.7"
-google-auth = "*"
 importlib-metadata = "<=4.12.0"
-cryptography = "==38.0.3"
+certifi = "*"
 itsdangerous = "==2.0.1"
-MarkupSafe = "<=2.1.1"
+markupsafe = "<=2.1.1"
+jinja2 = "<=3.1.2"
 typing-extensions = "==4.1.1"
-rich = "==12.4.4"
 flask = "<=2.1.3"
 flask-caching = "<=2.0.1"
+flask-cors = "==3.0.10"
 uvicorn = "<=0.18.2"
-google-cloud-compute = "==1.3.2"
-google-cloud-dns = "==0.34.0"
-grpcio = "==1.50.0"
 python-gitlab = "==3.13.0"
-certifi = "*"
+docker = {version = "*", extras = ["tls"]}
 kubernetes = "==24.2.0"
+octodns = "==0.9.14"
+boto3 = "*"
+supervisor = "*"
+google-cloud-compute = "==1.3.2"
+google-cloud-dns = "==0.34.0"
+google-auth = "*"
 gunicorn = "==20.1.0"
 redis = "==4.4.4"
-flask-cors = "==3.0.10"
-charset-normalizer = "==2.1.1"
+
+[dev-packages]
 
 [requires]
 python_version = "3.8"
```

### Comparing `unfurl-0.7.1/unfurl/templates/python3.8/Pipfile.lock` & `unfurl-0.8.0/unfurl/templates/python3.9/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9554597701149424%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'cb59ddd622f3b1feaa3ca32607b1e4e958f144bd9aeb139c73e1ec7605ab6045'}, 'requires': "*

 * *            "{'python_version': '3.9'}}",*

 * * "'default'": "{'ansible-core': {'hashes': "*

 * *              "['sha256:feb1df61738cfc1f5e893b42a2ec1a7de32977d67e86707b45eb63d0c5c3c236'], "*

 * *              "'version': '==2.12.10', 'index': 'pypi', delete: ['markers']}, 'boto3': {'hashes': "*

 * *              "['sha256:cfcb20d5784428f31d89889e68b26efeda90f231c3119eef4af8b25ad405c55f', "*

 * *        […]*

```diff
@@ -1,38 +1,31 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "1f90f0c6400af72bfe725654d0711a4c30c2decbdc1f1b720c764cdb37a55428"
+            "sha256": "cb59ddd622f3b1feaa3ca32607b1e4e958f144bd9aeb139c73e1ec7605ab6045"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.8"
+            "python_version": "3.9"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
-        "ansible": {
-            "hashes": [
-                "sha256:88af9479e81a3931bb3a1b8c4eeb252cd4f38c03daafd6a5aa120d6b0d70d45c"
-            ],
-            "index": "pypi",
-            "version": "==4.10.0"
-        },
         "ansible-core": {
             "hashes": [
-                "sha256:9159cc3b85e2d115f62f975b5155d96466e2a09a1c2e9b91de0c781f9089fc54"
+                "sha256:feb1df61738cfc1f5e893b42a2ec1a7de32977d67e86707b45eb63d0c5c3c236"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==2.11.12"
+            "index": "pypi",
+            "version": "==2.12.10"
         },
         "async-timeout": {
             "hashes": [
                 "sha256:2163e1640ddb52b7a8c80d0a67a08587e5d245cc9c553a74a847056bc2976b15",
                 "sha256:8ca1e4fcf50d07413d66d1a5e416e42cfdf5851c981d679a09851a6853383b3c"
             ],
             "markers": "python_version >= '3.6'",
@@ -50,45 +43,29 @@
             "hashes": [
                 "sha256:01be3ee61bb714e9090fcc5c10f4cf546c396331c620c6ae50a2321b28ed3199",
                 "sha256:0fbf5efbe78d466a26753e1dee3272423a3adc989d6a778c700e89a3f8ff0d88"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.5.1"
         },
-        "babel": {
-            "hashes": [
-                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
-                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
-            ],
-            "index": "pypi",
-            "version": "==2.12.1"
-        },
-        "boto": {
-            "hashes": [
-                "sha256:147758d41ae7240dc989f0039f27da8ca0d53734be0eb869ef16e3adcfa462e8",
-                "sha256:ea0d3b40a2d852767be77ca343b58a9e3a4b00d9db440efb8da74b4e58025e5a"
-            ],
-            "index": "pypi",
-            "version": "==2.49.0"
-        },
         "boto3": {
             "hashes": [
-                "sha256:a2778c5729d3dc0b3688c9f0d103543d7ec5ff44a4fd0e84d0d542e2dff05e62",
-                "sha256:ee0b8f8d238d4e1cf50fa6a185e4e066955b6105e9838a80b1b6582cd327dfdf"
+                "sha256:cfcb20d5784428f31d89889e68b26efeda90f231c3119eef4af8b25ad405c55f",
+                "sha256:d5ac6599951fdd519ed26c6fe15c41a7aa4021cb9adce33167344f8ce5cdb07b"
             ],
             "index": "pypi",
-            "version": "==1.26.152"
+            "version": "==1.28.12"
         },
         "botocore": {
             "hashes": [
-                "sha256:02a3205cc8579d4be6d537e63d72aebbf3f70f3aedcf40b3cae9dc2e24c774d0",
-                "sha256:f6319ecdbe3d325878f837cac2874e461b4d90691bb2d2186f980bce3b3cfcc8"
+                "sha256:7e5db466c762a071bb58c9a39d070f1333ce4f4ba6fdf9820ba21e87bd4c7e29",
+                "sha256:86380672151866b5e425636e3ebad74f2b83e7163e36ef5d38d11a04b9cba33b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.152"
+            "version": "==1.31.12"
         },
         "cachelib": {
             "hashes": [
                 "sha256:42d49f2fad9310dd946d7be73d46776bcd4d5fde4f49ad210cfdd447fbdfc346",
                 "sha256:593faeee62a7c037d50fc835617a01b887503f972fb52b188ae7e50e9cb69740"
             ],
             "markers": "python_version >= '3.7'",
@@ -100,19 +77,19 @@
                 "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.3.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "index": "pypi",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -191,22 +168,14 @@
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
             "version": "==8.1.3"
         },
-        "click-log": {
-            "hashes": [
-                "sha256:3970f8570ac54491237bcdb3d8ab5e3eef6c057df29f8c3d1151a51a9c23b975",
-                "sha256:a43e394b528d52112af599f2fc9e4b7cf3c15f94e53581f74fa6867e68c91756"
-            ],
-            "index": "pypi",
-            "version": "==0.4.0"
-        },
         "cliff": {
             "hashes": [
                 "sha256:045aee3f3c64471965d7ad507ce8474a4e2f20815fbb5405a770f8596a2a00a0",
                 "sha256:a21da482714b9f0b0e9bafaaf2f6a8b3b14161bb47f62e10e28d2fe4ff4b1626"
             ],
             "index": "pypi",
             "version": "==3.10.1"
@@ -325,62 +294,53 @@
                 "sha256:ed7b00096790213e09eb11c97cc6e2b757f15f3d2f85833cd2d3ec3fe37c1722"
             ],
             "index": "pypi",
             "version": "==38.0.3"
         },
         "distlib": {
             "hashes": [
-                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
-                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
+                "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057",
+                "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"
             ],
-            "version": "==0.3.6"
+            "version": "==0.3.7"
         },
         "dnspython": {
             "hashes": [
-                "sha256:224e32b03eb46be70e12ef6d64e0be123a64e621ab4c0822ff6d450d52a540b9",
-                "sha256:89141536394f909066cabd112e3e1a37e4e654db00a25308b0f130bc3152eb46"
+                "sha256:5b7488477388b8c0b70a8ce93b227c5603bc7b77f1565afe8e729c36c51447d7",
+                "sha256:c33971c79af5be968bb897e95c2448e11a645ee84d93b265ce0b7aabe5dfdca8"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.3.0"
+            "markers": "python_version >= '3.8' and python_version < '4.0'",
+            "version": "==2.4.1"
         },
         "docker": {
             "extras": [
                 "tls"
             ],
             "hashes": [
                 "sha256:aa6d17830045ba5ef0168d5eaa34d37beeb113948c413affe1d5991fc11f9a20",
                 "sha256:aecd2277b8bf8e506e484f6ab7aec39abe0038e29fa4a6d3ba86c3fe01844ed9"
             ],
             "index": "pypi",
             "version": "==6.1.3"
         },
-        "enum34": {
-            "hashes": [
-                "sha256:a98a201d6de3f2ab3db284e70a33b0f896fbf35f8086594e8c9e74b909058d53",
-                "sha256:c3858660960c984d6ab0ebad691265180da2b43f07e061c0f8dca9ef3cffd328",
-                "sha256:cce6a7477ed816bd2542d03d53db9f0db935dd013b70f336a95c73979289f248"
-            ],
-            "index": "pypi",
-            "version": "==1.1.10"
-        },
         "exceptiongroup": {
             "hashes": [
-                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
-                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
+                "sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5",
+                "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.1.1"
+            "version": "==1.1.2"
         },
         "filelock": {
             "hashes": [
-                "sha256:42f1e4ff2b497311213d61ad7aac5fed9050608e5309573f101eefa94143134a",
-                "sha256:82b1f7da46f0ae42abf1bc78e548667f484ac59d2bcec38c713cee7e2eb51e83"
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.12.1"
+            "version": "==3.12.2"
         },
         "flask": {
             "hashes": [
                 "sha256:15972e5017df0575c3d6c090ba168b6db90259e620ac8d7ea813a396bad5b6cb",
                 "sha256:9013281a7402ad527f8fd56375164f3aa021ecfaff89bfe3825346c24f87e04c"
             ],
             "index": "pypi",
@@ -427,43 +387,43 @@
             "version": "==3.1.30"
         },
         "google-api-core": {
             "extras": [
                 "grpc"
             ],
             "hashes": [
-                "sha256:4b9bb5d5a380a0befa0573b302651b8a9a89262c1730e37bf423cec511804c22",
-                "sha256:ce222e27b0de0d7bc63eb043b956996d6dccab14cc3b690aaea91c9cc99dc16e"
+                "sha256:25d29e05a0058ed5f19c61c0a78b1b53adea4d9364b464d014fbda941f6d1c9a",
+                "sha256:d92a5a92dc36dd4f4b9ee4e55528a90e432b059f93aee6ad857f9de8cc7ae94a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.11.0"
+            "version": "==2.11.1"
         },
         "google-auth": {
             "hashes": [
-                "sha256:a9cfa88b3e16196845e64a3658eb953992129d13ac7337b064c6546f77c17183",
-                "sha256:ea165e014c7cbd496558796b627c271aa8c18b4cba79dc1cc962b24c5efdfb85"
+                "sha256:164cba9af4e6e4e40c3a4f90a1a6c12ee56f14c0b4868d1ca91b32826ab334ce",
+                "sha256:d61d1b40897407b574da67da1a833bdc10d5a11642566e506565d1b1a46ba873"
             ],
             "index": "pypi",
-            "version": "==2.19.1"
+            "version": "==2.22.0"
         },
         "google-cloud-compute": {
             "hashes": [
                 "sha256:1ddd1be44d278754fc2643be7aa8d66838235ce44cfbacbeeadf3952ec020e95",
                 "sha256:21bd66251356d70bfd5f40211b42b936335490f7433b3b6fae7c498077e2c3fa"
             ],
             "index": "pypi",
             "version": "==1.3.2"
         },
         "google-cloud-core": {
             "hashes": [
-                "sha256:8417acf6466be2fa85123441696c4badda48db314c607cf1e5d543fa8bdc22fe",
-                "sha256:b9529ee7047fd8d4bf4a2182de619154240df17fbe60ead399078c1ae152af9a"
+                "sha256:37b80273c8d7eee1ae816b3a20ae43585ea50506cb0e60f3cf5be5f87f1373cb",
+                "sha256:fbd11cad3e98a7e5b0343dc07cb1039a5ffd7a5bb96e1f1e27cee4bda4a90863"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.3.2"
+            "version": "==2.3.3"
         },
         "google-cloud-dns": {
             "hashes": [
                 "sha256:41609782fa91df41e5ebfd48b127bb421a3b1821f5d49d900c484d13c0672167",
                 "sha256:bd75d6e9fd456ce643ee936a113a1ead5405704515caa679db30d7f036e447f3"
             ],
             "index": "pypi",
@@ -475,62 +435,61 @@
                 "sha256:b35d530fe825fb4227857bc47ad84c33c809ac96f312e13182bdeaa2abe1178a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.59.1"
         },
         "grpcio": {
             "hashes": [
-                "sha256:05f7c248e440f538aaad13eee78ef35f0541e73498dd6f832fe284542ac4b298",
-                "sha256:080b66253f29e1646ac53ef288c12944b131a2829488ac3bac8f52abb4413c0d",
-                "sha256:12b479839a5e753580b5e6053571de14006157f2ef9b71f38c56dc9b23b95ad6",
-                "sha256:156f8009e36780fab48c979c5605eda646065d4695deea4cfcbcfdd06627ddb6",
-                "sha256:15f9e6d7f564e8f0776770e6ef32dac172c6f9960c478616c366862933fa08b4",
-                "sha256:177afaa7dba3ab5bfc211a71b90da1b887d441df33732e94e26860b3321434d9",
-                "sha256:1a4cd8cb09d1bc70b3ea37802be484c5ae5a576108bad14728f2516279165dd7",
-                "sha256:1d8d02dbb616c0a9260ce587eb751c9c7dc689bc39efa6a88cc4fa3e9c138a7b",
-                "sha256:2b71916fa8f9eb2abd93151fafe12e18cebb302686b924bd4ec39266211da525",
-                "sha256:2d9fd6e38b16c4d286a01e1776fdf6c7a4123d99ae8d6b3f0b4a03a34bf6ce45",
-                "sha256:3b611b3de3dfd2c47549ca01abfa9bbb95937eb0ea546ea1d762a335739887be",
-                "sha256:3e4244c09cc1b65c286d709658c061f12c61c814be0b7030a2d9966ff02611e0",
-                "sha256:40838061e24f960b853d7bce85086c8e1b81c6342b1f4c47ff0edd44bbae2722",
-                "sha256:4b123fbb7a777a2fedec684ca0b723d85e1d2379b6032a9a9b7851829ed3ca9a",
-                "sha256:531f8b46f3d3db91d9ef285191825d108090856b3bc86a75b7c3930f16ce432f",
-                "sha256:67dd41a31f6fc5c7db097a5c14a3fa588af54736ffc174af4411d34c4f306f68",
-                "sha256:7489dbb901f4fdf7aec8d3753eadd40839c9085967737606d2c35b43074eea24",
-                "sha256:8d4c8e73bf20fb53fe5a7318e768b9734cf122fe671fcce75654b98ba12dfb75",
-                "sha256:8e69aa4e9b7f065f01d3fdcecbe0397895a772d99954bb82eefbb1682d274518",
-                "sha256:8e8999a097ad89b30d584c034929f7c0be280cd7851ac23e9067111167dcbf55",
-                "sha256:906f4d1beb83b3496be91684c47a5d870ee628715227d5d7c54b04a8de802974",
-                "sha256:92d7635d1059d40d2ec29c8bf5ec58900120b3ce5150ef7414119430a4b2dd5c",
-                "sha256:931e746d0f75b2a5cff0a1197d21827a3a2f400c06bace036762110f19d3d507",
-                "sha256:95ce51f7a09491fb3da8cf3935005bff19983b77c4e9437ef77235d787b06842",
-                "sha256:9eea18a878cffc804506d39c6682d71f6b42ec1c151d21865a95fae743fda500",
-                "sha256:a23d47f2fc7111869f0ff547f771733661ff2818562b04b9ed674fa208e261f4",
-                "sha256:a4c23e54f58e016761b576976da6a34d876420b993f45f66a2bfb00363ecc1f9",
-                "sha256:a50a1be449b9e238b9bd43d3857d40edf65df9416dea988929891d92a9f8a778",
-                "sha256:ab5d0e3590f0a16cb88de4a3fa78d10eb66a84ca80901eb2c17c1d2c308c230f",
-                "sha256:ae23daa7eda93c1c49a9ecc316e027ceb99adbad750fbd3a56fa9e4a2ffd5ae0",
-                "sha256:af98d49e56605a2912cf330b4627e5286243242706c3a9fa0bcec6e6f68646fc",
-                "sha256:b2f77a90ba7b85bfb31329f8eab9d9540da2cf8a302128fb1241d7ea239a5469",
-                "sha256:baab51dcc4f2aecabf4ed1e2f57bceab240987c8b03533f1cef90890e6502067",
-                "sha256:ca8a2254ab88482936ce941485c1c20cdeaef0efa71a61dbad171ab6758ec998",
-                "sha256:cb11464f480e6103c59d558a3875bd84eed6723f0921290325ebe97262ae1347",
-                "sha256:ce8513aee0af9c159319692bfbf488b718d1793d764798c3d5cff827a09e25ef",
-                "sha256:cf151f97f5f381163912e8952eb5b3afe89dec9ed723d1561d59cabf1e219a35",
-                "sha256:d144ad10eeca4c1d1ce930faa105899f86f5d99cecfe0d7224f3c4c76265c15e",
-                "sha256:d534d169673dd5e6e12fb57cc67664c2641361e1a0885545495e65a7b761b0f4",
-                "sha256:d75061367a69808ab2e84c960e9dce54749bcc1e44ad3f85deee3a6c75b4ede9",
-                "sha256:d84d04dec64cc4ed726d07c5d17b73c343c8ddcd6b59c7199c801d6bbb9d9ed1",
-                "sha256:de411d2b030134b642c092e986d21aefb9d26a28bf5a18c47dd08ded411a3bc5",
-                "sha256:e07fe0d7ae395897981d16be61f0db9791f482f03fee7d1851fe20ddb4f69c03",
-                "sha256:ea8ccf95e4c7e20419b7827aa5b6da6f02720270686ac63bd3493a651830235c",
-                "sha256:f7025930039a011ed7d7e7ef95a1cb5f516e23c5a6ecc7947259b67bea8e06ca"
+                "sha256:06e84ad9ae7668a109e970c7411e7992751a116494cba7c4fb877656527f9a57",
+                "sha256:0ff789ae7d8ddd76d2ac02e7d13bfef6fc4928ac01e1dcaa182be51b6bcc0aaa",
+                "sha256:10954662f77dc36c9a1fb5cc4a537f746580d6b5734803be1e587252682cda8d",
+                "sha256:139f66656a762572ae718fa0d1f2dce47c05e9fbf7a16acd704c354405b97df9",
+                "sha256:1c31e52a04e62c8577a7bf772b3e7bed4df9c9e0dd90f92b6ffa07c16cab63c9",
+                "sha256:33971197c47965cc1d97d78d842163c283e998223b151bab0499b951fd2c0b12",
+                "sha256:345356b307cce5d14355e8e055b4ca5f99bc857c33a3dc1ddbc544fca9cd0475",
+                "sha256:373b48f210f43327a41e397391715cd11cfce9ded2fe76a5068f9bacf91cc226",
+                "sha256:3ccb621749a81dc7755243665a70ce45536ec413ef5818e013fe8dfbf5aa497b",
+                "sha256:42a3bbb2bc07aef72a7d97e71aabecaf3e4eb616d39e5211e2cfe3689de860ca",
+                "sha256:42e63904ee37ae46aa23de50dac8b145b3596f43598fa33fe1098ab2cbda6ff5",
+                "sha256:4eb37dd8dd1aa40d601212afa27ca5be255ba792e2e0b24d67b8af5e012cdb7d",
+                "sha256:51173e8fa6d9a2d85c14426bdee5f5c4a0654fd5fddcc21fe9d09ab0f6eb8b35",
+                "sha256:5144feb20fe76e73e60c7d73ec3bf54f320247d1ebe737d10672480371878b48",
+                "sha256:5344be476ac37eb9c9ad09c22f4ea193c1316bf074f1daf85bddb1b31fda5116",
+                "sha256:6108e5933eb8c22cd3646e72d5b54772c29f57482fd4c41a0640aab99eb5071d",
+                "sha256:6a007a541dff984264981fbafeb052bfe361db63578948d857907df9488d8774",
+                "sha256:6ee26e9dfb3996aff7c870f09dc7ad44a5f6732b8bdb5a5f9905737ac6fd4ef1",
+                "sha256:750de923b456ca8c0f1354d6befca45d1f3b3a789e76efc16741bd4132752d95",
+                "sha256:7c5ede2e2558f088c49a1ddda19080e4c23fb5d171de80a726b61b567e3766ed",
+                "sha256:830215173ad45d670140ff99aac3b461f9be9a6b11bee1a17265aaaa746a641a",
+                "sha256:8391cea5ce72f4a12368afd17799474015d5d3dc00c936a907eb7c7eaaea98a5",
+                "sha256:8940d6de7068af018dfa9a959a3510e9b7b543f4c405e88463a1cbaa3b2b379a",
+                "sha256:89a49cc5ad08a38b6141af17e00d1dd482dc927c7605bc77af457b5a0fca807c",
+                "sha256:900bc0096c2ca2d53f2e5cebf98293a7c32f532c4aeb926345e9747452233950",
+                "sha256:97e0efaebbfd222bcaac2f1735c010c1d3b167112d9d237daebbeedaaccf3d1d",
+                "sha256:9e04d4e4cfafa7c5264e535b5d28e786f0571bea609c3f0aaab13e891e933e9c",
+                "sha256:a4c60abd950d6de3e4f1ddbc318075654d275c29c846ab6a043d6ed2c52e4c8c",
+                "sha256:a6ff459dac39541e6a2763a4439c4ca6bc9ecb4acc05a99b79246751f9894756",
+                "sha256:a72797549935c9e0b9bc1def1768c8b5a709538fa6ab0678e671aec47ebfd55e",
+                "sha256:af4063ef2b11b96d949dccbc5a987272f38d55c23c4c01841ea65a517906397f",
+                "sha256:b975b85d1d5efc36cf8b237c5f3849b64d1ba33d6282f5e991f28751317504a1",
+                "sha256:bf0b9959e673505ee5869950642428046edb91f99942607c2ecf635f8a4b31c9",
+                "sha256:c0c85c5cbe8b30a32fa6d802588d55ffabf720e985abe9590c7c886919d875d4",
+                "sha256:c3f3237a57e42f79f1e560726576aedb3a7ef931f4e3accb84ebf6acc485d316",
+                "sha256:c3fa3ab0fb200a2c66493828ed06ccd1a94b12eddbfb985e7fd3e5723ff156c6",
+                "sha256:c435f5ce1705de48e08fcbcfaf8aee660d199c90536e3e06f2016af7d6a938dd",
+                "sha256:c90da4b124647547a68cf2f197174ada30c7bb9523cb976665dfd26a9963d328",
+                "sha256:cbdf2c498e077282cd427cfd88bdce4668019791deef0be8155385ab2ba7837f",
+                "sha256:d1fbad1f9077372b6587ec589c1fc120b417b6c8ad72d3e3cc86bbbd0a3cee93",
+                "sha256:d39f5d4af48c138cb146763eda14eb7d8b3ccbbec9fe86fb724cd16e0e914c64",
+                "sha256:ddb4a6061933bd9332b74eac0da25f17f32afa7145a33a0f9711ad74f924b1b8",
+                "sha256:ded637176addc1d3eef35331c39acc598bac550d213f0a1bedabfceaa2244c87",
+                "sha256:f20fd21f7538f8107451156dd1fe203300b79a9ddceba1ee0ac8132521a008ed",
+                "sha256:fda2783c12f553cdca11c08e5af6eecbd717280dc8fbe28a110897af1c15a88c"
             ],
-            "index": "pypi",
-            "version": "==1.50.0"
+            "version": "==1.56.2"
         },
         "grpcio-status": {
             "hashes": [
                 "sha256:2c33bbdbe20188b2953f46f31af669263b6ee2a9b2d38fa0d36ee091532e21bf",
                 "sha256:53695f45da07437b7c344ee4ef60d370fd2850179f5a28bb26d8e2aa1102ec11"
             ],
             "version": "==1.48.2"
@@ -596,18 +555,18 @@
                 "sha256:90261b206d6defd58fdd5e85f478bf633a2901798906be2ad389150c5c60edbe"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.1"
         },
         "jsonpointer": {
             "hashes": [
-                "sha256:51801e558539b4e9cd268638c078c6c5746c9ac96bc38152d443400e4f3793e9",
-                "sha256:97cba51526c829282218feb99dab1b1e6bdf8efd1c43dc9d57be093c0d69c99a"
+                "sha256:15d51bba20eea3165644553647711d150376234112651b4f1811022aecad7d7a",
+                "sha256:585cee82b70211fa9e6043b7bb89db6e1aa49524340dde8ad6b63206ea689d88"
             ],
-            "version": "==2.3"
+            "version": "==2.4"
         },
         "jsonschema": {
             "extras": [
                 "format_nongpl"
             ],
             "hashes": [
                 "sha256:4e5b3cf8216f577bee9ce139cbe72eca3ea4f292ec60928ff24758ce626cd163",
@@ -666,28 +625,21 @@
                 "sha256:efc1913fd2ca4f334418481c7e595c00aad186563bbc1ec76067848c7ca0a933",
                 "sha256:f121a1420d4e173a5d96e47e9a0c0dcff965afdf1626d28de1460815f7c4ee7a",
                 "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
             ],
             "index": "pypi",
             "version": "==2.1.1"
         },
-        "mitogen": {
-            "hashes": [
-                "sha256:c2dd28d6b964699822455f6c91acedc16324913586837f046a76e2e4ac1d716c"
-            ],
-            "index": "pypi",
-            "version": "==0.2.7"
-        },
         "natsort": {
             "hashes": [
-                "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
-                "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
+                "sha256:45312c4a0e5507593da193dedd04abb1469253b601ecaf63445ad80f0a1ea581",
+                "sha256:4732914fb471f56b5cce04d7bae6f164a592c7712e1c85f9ef585e197299521c"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==8.3.1"
+            "version": "==8.4.0"
         },
         "oauthlib": {
             "hashes": [
                 "sha256:8139f29aac13e25d502680e9e19963e83f16838d48a0d71c287fe40e7067fbca",
                 "sha256:9859c40929662bec5d64f34d01c99e093149682a3f38915dc0655d5a633dd918"
             ],
             "markers": "python_version >= '3.6'",
@@ -697,21 +649,14 @@
             "hashes": [
                 "sha256:9c31bd5cdbdbe5ef678cb01ac0564461790126acb9c3ab51a0f63fc9eaf608c8",
                 "sha256:aa629a2b75714a5c15c47125b6e1c4226492d7fe4c5b348c081c8b4cf87ce0ae"
             ],
             "index": "pypi",
             "version": "==0.9.14"
         },
-        "openshift": {
-            "hashes": [
-                "sha256:a060afb7565dda18b2749857867d80ab22b2f4143264519f493a9cabccc3b8a8"
-            ],
-            "index": "pypi",
-            "version": "==0.13.1"
-        },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
@@ -720,45 +665,37 @@
             "hashes": [
                 "sha256:e547125940bcc052856ded43be8e101f63828c2d94239ffbe2b327ba3d5ccf0a",
                 "sha256:e8dca2f4b43560edef58813969f52a56cef023146cbb8931626db80e6c1c4308"
             ],
             "index": "pypi",
             "version": "==5.9.0"
         },
-        "pip": {
-            "hashes": [
-                "sha256:0e7c86f486935893c708287b30bd050a36ac827ec7fe5e43fe7cb198dd835fba",
-                "sha256:3ef6ac33239e4027d9a5598a381b9d30880a1477e50039db2eac6e8a8f6d1b18"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.1.2"
-        },
         "pipenv": {
             "hashes": [
-                "sha256:3b80b4512934b9d8e8ce12c988394642ff96bb697680e5b092e59af503178327",
-                "sha256:f84d7119239b22ab2ac2b8fbc7d619d83cf41135206d72a17c4f151cda529fd0"
+                "sha256:116061545d4e2281cbc799f7736a715ee5ddf0a6f63c09f4263a4a6a0779fe93",
+                "sha256:404de9ff6a2464e20e52aaad71db2d4f8f2900f2177fc45a47f6315686cb2e5b"
             ],
             "index": "pypi",
-            "version": "==2022.1.8"
+            "version": "==2023.7.3"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:0ade98a4895e87dc51d47151f7d2ec290365a585151d97b4d8d6312ed6132fed",
-                "sha256:e48fabd87db8f3a7df7150a4a5ea22c546ee8bc39bc2473244730d4b56d2cc4e"
+                "sha256:1b42b450ad933e981d56e59f1b97495428c9bd60698baab9f3eb3d00d5822421",
+                "sha256:ad8291ae0ae5072f66c16945166cb11c63394c7a3ad1b1bc9828ca3162da8c2f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.3"
+            "version": "==3.9.1"
         },
         "pluggy": {
             "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
+                "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
+                "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.0.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.2.0"
         },
         "pprintpp": {
             "hashes": [
                 "sha256:b6b4dcdd0c0c0d75e4d7b2f21a9e933e5b2ce62b26e1a54537f9651ae5a5c01d",
                 "sha256:ea826108e2c7f49dc6d66c752973c3fc9749142a798d6b254e1e301cfdbc6403"
             ],
             "version": "==0.4.0"
@@ -769,19 +706,19 @@
                 "sha256:03481bca25ae0c28958c8cd6ac5165c159ce89f7ccde04d5c899b24b68bb13b7"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==3.8.0"
         },
         "proto-plus": {
             "hashes": [
-                "sha256:0e8cda3d5a634d9895b75c573c9352c16486cb75deb0e078b5fda34db4243165",
-                "sha256:de34e52d6c9c6fcd704192f09767cb561bb4ee64e70eede20b0834d841f0be4d"
+                "sha256:a49cd903bc0b6ab41f76bf65510439d56ca76f868adf0274e738bfdd096894df",
+                "sha256:fdcd09713cbd42480740d2fe29c990f7fbd885a67efc328aa8be6ee3e9f76a6b"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==1.22.2"
+            "version": "==1.22.3"
         },
         "protobuf": {
             "hashes": [
                 "sha256:03038ac1cfbc41aa21f6afcbcd357281d7521b4157926f30ebecc8d4ea59dcb7",
                 "sha256:28545383d61f55b57cf4df63eebd9827754fd2dc25f80c5253f9184235db242c",
                 "sha256:2e3427429c9cffebf259491be0af70189607f365c2f41c7c3764af6f337105f2",
                 "sha256:398a9e0c3eaceb34ec1aee71894ca3299605fa8e761544934378bbc6c97de23b",
@@ -850,19 +787,19 @@
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pyparsing": {
             "hashes": [
-                "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb",
-                "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
+                "sha256:d554a96d1a7d3ddaf7183104485bc19fd80543ad6ac5bdb6426719d766fb06c1",
+                "sha256:edb662d6fe322d6e990b1594b5feaeadf806803359e3d4d42f11e295e588f0ea"
             ],
             "markers": "python_full_version >= '3.6.8'",
-            "version": "==3.0.9"
+            "version": "==3.1.0"
         },
         "pyperclip": {
             "hashes": [
                 "sha256:105254a8b04934f0bc84e9c24eb360a591aaf6535c9def5f29d92af107a9bf57"
             ],
             "version": "==1.8.2"
         },
@@ -871,35 +808,35 @@
                 "sha256:cdc7b5e3ed77bed61270a47d35434a30617b9becdf2478af76ad2c6ade307280"
             ],
             "index": "pypi",
             "version": "==0.15.7"
         },
         "pytest": {
             "hashes": [
-                "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295",
-                "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"
+                "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
+                "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.3.2"
+            "version": "==7.4.0"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6",
                 "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.1.0"
         },
         "pytest-mock": {
             "hashes": [
-                "sha256:f4c973eeae0282963eb293eb173ce91b091a79c1334455acfac9ddee8a1c784b",
-                "sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f"
+                "sha256:21c279fff83d70763b05f8874cc9cfb3fcacd6d354247a976f9529d19f9acf39",
+                "sha256:7f6b125602ac6d743e523ae0bfa71e1a697a2f5534064528c6ff84c2f7c2fc7f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.10.0"
+            "version": "==3.11.1"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "index": "pypi",
@@ -909,75 +846,59 @@
             "hashes": [
                 "sha256:85ae778d8953aba87ad4b78aef7fbb5dae053980d2c20ff200bea29799685743",
                 "sha256:ad502b72b5d1137f4af37d4a68ae20fe7d6c9778f67cbe2aec566f7995053c7d"
             ],
             "index": "pypi",
             "version": "==3.13.0"
         },
-        "python-string-utils": {
-            "hashes": [
-                "sha256:dcf9060b03f07647c0a603408dc8b03f807f3b54a05c6e19eb14460256fac0cb",
-                "sha256:f1a88700baf99db1a9b6953f44181ad9ca56623c81e257e6009707e2e7851fa4"
-            ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.0"
-        },
-        "pytz": {
-            "hashes": [
-                "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
-                "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
-            ],
-            "markers": "python_version < '3.9'",
-            "version": "==2023.3"
-        },
         "pyyaml": {
             "hashes": [
-                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
-                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
-                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
-                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
-                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
-                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
-                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
-                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
-                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
-                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
-                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
-                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
-                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
-                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
-                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
-                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
-                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
-                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
-                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
-                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
-                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
-                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
-                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
-                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
-                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
-                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
-                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
-                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
-                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
-                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
-                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
-                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
-                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
-                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
-                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
-                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
-                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
-                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
-                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
-                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
+                "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
+                "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
+                "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
+                "sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27",
+                "sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595",
+                "sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62",
+                "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98",
+                "sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696",
+                "sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d",
+                "sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867",
+                "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47",
+                "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486",
+                "sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6",
+                "sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3",
+                "sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007",
+                "sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938",
+                "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
+                "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
+                "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
+                "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
+                "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
+                "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
+                "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
+                "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
+                "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
+                "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
+                "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
+                "sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924",
+                "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34",
+                "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43",
+                "sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859",
+                "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673",
+                "sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a",
+                "sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab",
+                "sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa",
+                "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c",
+                "sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585",
+                "sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d",
+                "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"
             ],
             "index": "pypi",
-            "version": "==6.0"
+            "version": "==6.0.1"
         },
         "redis": {
             "hashes": [
                 "sha256:68226f7ede928db8302f29ab088a157f41061fa946b7ae865452b6d7838bbffb",
                 "sha256:da92a39fec86438d3f1e2a1db33c312985806954fe860120b582a8430e231d8f"
             ],
             "index": "pypi",
@@ -1108,26 +1029,26 @@
                 "sha256:640bb492711f4c0c0905e1f62b6aaeb771881935ad27884852411f8e9cacbca9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.6.1"
         },
         "setuptools": {
             "hashes": [
-                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
-                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.8.0"
+            "version": "==68.0.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
-            "index": "pypi",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
             "version": "==1.16.0"
         },
         "smmap": {
             "hashes": [
                 "sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94",
                 "sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936"
             ],
@@ -1138,23 +1059,14 @@
             "hashes": [
                 "sha256:a547de73308fd7e90075bb4d301405bebf705292fa90a90fc3bcf9133f58616c",
                 "sha256:f40253887d8712eaa2bb0ea3830374416736dc8ec0e22f5a65092c1174c44335"
             ],
             "index": "pypi",
             "version": "==3.5.0"
         },
-        "subprocess32": {
-            "hashes": [
-                "sha256:88e37c1aac5388df41cc8a8456bb49ebffd321a3ad4d70358e3518176de3a56b",
-                "sha256:e45d985aef903c5b7444d34350b05da91a9e0ea015415ab45a21212786c649d0",
-                "sha256:eb2937c80497978d181efa1b839ec2d9622cf9600a039a79d0e108d1f9aec79d"
-            ],
-            "index": "pypi",
-            "version": "==3.5.4"
-        },
         "supervisor": {
             "hashes": [
                 "sha256:2ecaede32fc25af814696374b79e42644ecaba5c09494c51016ffda9602d0f08",
                 "sha256:34761bae1a23c58192281a5115fb07fbf22c9b0133c08166beffc70fed3ebc12"
             ],
             "index": "pypi",
             "version": "==4.2.5"
@@ -1189,19 +1101,19 @@
                 "sha256:cade07c403c397f9fe275492a48c1b869efd175d5d8a692df649e6e7e2ed8f4e"
             ],
             "index": "pypi",
             "version": "==0.18.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
-                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
+                "sha256:43a3052be36080548bdee0b42919c88072037d50d56c28bd3f853cbe92b953ff",
+                "sha256:fd8a78f46f6b99a67b7ec5cf73f92357891a7b3a40fd97637c27f854aae3b9e0"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.23.0"
+            "version": "==20.24.2"
         },
         "virtualenv-clone": {
             "hashes": [
                 "sha256:418ee935c36152f8f153c79824bb93eaf6f0f7984bae31d3f48f350b9183501a",
                 "sha256:44d5263bceed0bac3e1424d64f798095233b64def1c5689afa43dc3223caf5b0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1219,40 +1131,40 @@
                 "sha256:29bc7e8752c0a1bd4a1f03c14d6e6a72e93d82193738fa860cbff59d0fcc11bf",
                 "sha256:c225b674c83fa923be93d235330ce0300373d02885cef23238813b0d5668304a"
             ],
             "version": "==1.13"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:3566f8467cd350874c4913816355642a4942f6c1ed1e9406e3d42fae6d6c072a",
-                "sha256:b96f3bce3e54e3486ebe6504bc22bd4c140392bd2eb71764db29be8f2639aa65"
+                "sha256:c951af98631d24f8df89ab1019fc365f2227c0892f12fd150e935607c79dd0dd",
+                "sha256:f1f9f2ad5291f0225a49efad77abf9e700b6fef553900623060dad6e26503b9d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.5.3"
+            "version": "==1.6.1"
         },
         "werkzeug": {
             "hashes": [
                 "sha256:935539fa1413afbb9195b24880778422ed620c0fc09670945185cce4d91a8890",
                 "sha256:98c774df2f91b05550078891dee5f0eb0cb797a522c757a2452b9cee5b202330"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==2.3.6"
         },
         "wheel": {
             "hashes": [
-                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
-                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
+                "sha256:55a0f0a5a84869bce5ba775abfd9c462e3a6b1b7b7ec69d72c0b83d673a5114d",
+                "sha256:7e9be3bbd0078f6147d82ed9ed957e323e7708f57e134743d2edef3a7b7972a9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.40.0"
+            "version": "==0.41.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
-                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
+                "sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0",
+                "sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.15.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.16.2"
         }
     },
     "develop": {}
 }
```

### Comparing `unfurl-0.7.1/unfurl/templates/python3.9/Pipfile` & `unfurl-0.8.0/unfurl/templates/python3.9/Pipfile`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,48 @@
 [[source]]
 url = "https://pypi.org/simple"
 verify_ssl = true
 name = "pypi"
 
 [packages]
-pipenv = "==2022.1.8"
-click = ">=8.0.1"
-click-log = "*"
+pipenv = "==2023.7.3"
+click = ">=8.0.1,<8.1.4"
 pyrsistent = "==0.15.7"
 jsonschema = {version = "==3.2", extras = ["format_nongpl"]}
 "ruamel.yaml" = "==0.17.21"
-ansible = "<5.0,>=4.2.0"
+charset-normalizer = "==2.1.1"
+cryptography = "==38.0.3"
+ansible-core = "==2.12.10"
+gitpython = "==3.1.30"
+rich = "==12.4.4"
 pbr = "==5.9.0"
 cliff = "==3.10.1"
+pyyaml = ">=6.0"
 python-dateutil = ">=2.8"
-six = ">=1.10.0"
 stevedore = "==3.5.0"
 requests = ">=2.14.2"
-enum34 = "*"
 importlib-metadata = "<=4.12.0"
-subprocess32 = "*"
-docker = {extras = ["tls"], version = "*"}
-openshift = "==0.13.1"
-octodns = "==0.9.14"
-boto = "*"
-boto3 = "*"
-supervisor = "*"
-google-auth = "*"
-GitPython = "==3.1.30"
-Babel = ">=2.3.4,!=2.4.0"
-PyYAML = ">=6.0"
-cryptography = "==38.0.3"
-Jinja2 = "<=3.1.2"
+certifi = "*"
 itsdangerous = "==2.0.1"
-MarkupSafe = "<=2.1.1"
+markupsafe = "<=2.1.1"
+jinja2 = "<=3.1.2"
 typing-extensions = "==4.1.1"
-rich = "==12.4.4"  # MIT
 flask = "<=2.1.3"
 flask-caching = "<=2.0.1"
+flask-cors = "==3.0.10"
 uvicorn = "<=0.18.2"
-google-cloud-compute = "==1.3.2"
-google-cloud-dns = "==0.34.0"
-grpcio = "==1.50.0"
 python-gitlab = "==3.13.0"
-certifi = "*"
+docker = {version = "*", extras = ["tls"]}
 kubernetes = "==24.2.0"
+octodns = "==0.9.14"
+boto3 = "*"
+supervisor = "*"
+google-cloud-compute = "==1.3.2"
+google-cloud-dns = "==0.34.0"
+google-auth = "*"
 gunicorn = "==20.1.0"
 redis = "==4.4.4"
-flask-cors = "==3.0.10"
-charset-normalizer = "==2.1.1"
 
 [dev-packages]
 
 [requires]
 python_version = "3.9"
```

### Comparing `unfurl-0.7.1/unfurl/templates/python3.9/Pipfile.lock` & `unfurl-0.8.0/unfurl/templates/python3.11/Pipfile.lock`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9534600389863548%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'9c6081b0d417c6246dd35e3e5678cd9e8306d8a926517a10addebf1685784532'}, 'requires': "*

 * *            "{'python_version': '3.11'}}",*

 * * "'default'": "{'ansible-core': {'hashes': "*

 * *              "['sha256:feb1df61738cfc1f5e893b42a2ec1a7de32977d67e86707b45eb63d0c5c3c236'], "*

 * *              "'version': '==2.12.10', 'index': 'pypi', delete: ['markers']}, 'boto3': {'hashes': "*

 * *              "['sha256:cfcb20d5784428f31d89889e68b26efeda90f231c3119eef4af8b25ad405c55f', "*

 * *       […]*

```diff
@@ -1,38 +1,31 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "1dd9e913fbcd065998070331f4d878fcbf94ebf02fcb5a19920fac8a52c3ac2a"
+            "sha256": "9c6081b0d417c6246dd35e3e5678cd9e8306d8a926517a10addebf1685784532"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.9"
+            "python_version": "3.11"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
-        "ansible": {
-            "hashes": [
-                "sha256:88af9479e81a3931bb3a1b8c4eeb252cd4f38c03daafd6a5aa120d6b0d70d45c"
-            ],
-            "index": "pypi",
-            "version": "==4.10.0"
-        },
         "ansible-core": {
             "hashes": [
-                "sha256:9159cc3b85e2d115f62f975b5155d96466e2a09a1c2e9b91de0c781f9089fc54"
+                "sha256:feb1df61738cfc1f5e893b42a2ec1a7de32977d67e86707b45eb63d0c5c3c236"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==2.11.12"
+            "index": "pypi",
+            "version": "==2.12.10"
         },
         "async-timeout": {
             "hashes": [
                 "sha256:2163e1640ddb52b7a8c80d0a67a08587e5d245cc9c553a74a847056bc2976b15",
                 "sha256:8ca1e4fcf50d07413d66d1a5e416e42cfdf5851c981d679a09851a6853383b3c"
             ],
             "markers": "python_version >= '3.6'",
@@ -50,45 +43,29 @@
             "hashes": [
                 "sha256:01be3ee61bb714e9090fcc5c10f4cf546c396331c620c6ae50a2321b28ed3199",
                 "sha256:0fbf5efbe78d466a26753e1dee3272423a3adc989d6a778c700e89a3f8ff0d88"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.5.1"
         },
-        "babel": {
-            "hashes": [
-                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
-                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
-            ],
-            "index": "pypi",
-            "version": "==2.12.1"
-        },
-        "boto": {
-            "hashes": [
-                "sha256:147758d41ae7240dc989f0039f27da8ca0d53734be0eb869ef16e3adcfa462e8",
-                "sha256:ea0d3b40a2d852767be77ca343b58a9e3a4b00d9db440efb8da74b4e58025e5a"
-            ],
-            "index": "pypi",
-            "version": "==2.49.0"
-        },
         "boto3": {
             "hashes": [
-                "sha256:a2778c5729d3dc0b3688c9f0d103543d7ec5ff44a4fd0e84d0d542e2dff05e62",
-                "sha256:ee0b8f8d238d4e1cf50fa6a185e4e066955b6105e9838a80b1b6582cd327dfdf"
+                "sha256:cfcb20d5784428f31d89889e68b26efeda90f231c3119eef4af8b25ad405c55f",
+                "sha256:d5ac6599951fdd519ed26c6fe15c41a7aa4021cb9adce33167344f8ce5cdb07b"
             ],
             "index": "pypi",
-            "version": "==1.26.152"
+            "version": "==1.28.12"
         },
         "botocore": {
             "hashes": [
-                "sha256:02a3205cc8579d4be6d537e63d72aebbf3f70f3aedcf40b3cae9dc2e24c774d0",
-                "sha256:f6319ecdbe3d325878f837cac2874e461b4d90691bb2d2186f980bce3b3cfcc8"
+                "sha256:7e5db466c762a071bb58c9a39d070f1333ce4f4ba6fdf9820ba21e87bd4c7e29",
+                "sha256:86380672151866b5e425636e3ebad74f2b83e7163e36ef5d38d11a04b9cba33b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.152"
+            "version": "==1.31.12"
         },
         "cachelib": {
             "hashes": [
                 "sha256:42d49f2fad9310dd946d7be73d46776bcd4d5fde4f49ad210cfdd447fbdfc346",
                 "sha256:593faeee62a7c037d50fc835617a01b887503f972fb52b188ae7e50e9cb69740"
             ],
             "markers": "python_version >= '3.7'",
@@ -100,19 +77,19 @@
                 "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.3.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "index": "pypi",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -191,22 +168,14 @@
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
             "version": "==8.1.3"
         },
-        "click-log": {
-            "hashes": [
-                "sha256:3970f8570ac54491237bcdb3d8ab5e3eef6c057df29f8c3d1151a51a9c23b975",
-                "sha256:a43e394b528d52112af599f2fc9e4b7cf3c15f94e53581f74fa6867e68c91756"
-            ],
-            "index": "pypi",
-            "version": "==0.4.0"
-        },
         "cliff": {
             "hashes": [
                 "sha256:045aee3f3c64471965d7ad507ce8474a4e2f20815fbb5405a770f8596a2a00a0",
                 "sha256:a21da482714b9f0b0e9bafaaf2f6a8b3b14161bb47f62e10e28d2fe4ff4b1626"
             ],
             "index": "pypi",
             "version": "==3.10.1"
@@ -325,62 +294,45 @@
                 "sha256:ed7b00096790213e09eb11c97cc6e2b757f15f3d2f85833cd2d3ec3fe37c1722"
             ],
             "index": "pypi",
             "version": "==38.0.3"
         },
         "distlib": {
             "hashes": [
-                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
-                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
+                "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057",
+                "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"
             ],
-            "version": "==0.3.6"
+            "version": "==0.3.7"
         },
         "dnspython": {
             "hashes": [
-                "sha256:224e32b03eb46be70e12ef6d64e0be123a64e621ab4c0822ff6d450d52a540b9",
-                "sha256:89141536394f909066cabd112e3e1a37e4e654db00a25308b0f130bc3152eb46"
+                "sha256:5b7488477388b8c0b70a8ce93b227c5603bc7b77f1565afe8e729c36c51447d7",
+                "sha256:c33971c79af5be968bb897e95c2448e11a645ee84d93b265ce0b7aabe5dfdca8"
             ],
-            "markers": "python_version >= '3.7' and python_full_version < '4.0.0'",
-            "version": "==2.3.0"
+            "markers": "python_version >= '3.8' and python_version < '4.0'",
+            "version": "==2.4.1"
         },
         "docker": {
             "extras": [
                 "tls"
             ],
             "hashes": [
                 "sha256:aa6d17830045ba5ef0168d5eaa34d37beeb113948c413affe1d5991fc11f9a20",
                 "sha256:aecd2277b8bf8e506e484f6ab7aec39abe0038e29fa4a6d3ba86c3fe01844ed9"
             ],
             "index": "pypi",
             "version": "==6.1.3"
         },
-        "enum34": {
-            "hashes": [
-                "sha256:a98a201d6de3f2ab3db284e70a33b0f896fbf35f8086594e8c9e74b909058d53",
-                "sha256:c3858660960c984d6ab0ebad691265180da2b43f07e061c0f8dca9ef3cffd328",
-                "sha256:cce6a7477ed816bd2542d03d53db9f0db935dd013b70f336a95c73979289f248"
-            ],
-            "index": "pypi",
-            "version": "==1.1.10"
-        },
-        "exceptiongroup": {
-            "hashes": [
-                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
-                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
-            ],
-            "markers": "python_version < '3.11'",
-            "version": "==1.1.1"
-        },
         "filelock": {
             "hashes": [
-                "sha256:42f1e4ff2b497311213d61ad7aac5fed9050608e5309573f101eefa94143134a",
-                "sha256:82b1f7da46f0ae42abf1bc78e548667f484ac59d2bcec38c713cee7e2eb51e83"
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.12.1"
+            "version": "==3.12.2"
         },
         "flask": {
             "hashes": [
                 "sha256:15972e5017df0575c3d6c090ba168b6db90259e620ac8d7ea813a396bad5b6cb",
                 "sha256:9013281a7402ad527f8fd56375164f3aa021ecfaff89bfe3825346c24f87e04c"
             ],
             "index": "pypi",
@@ -403,15 +355,15 @@
             "version": "==3.0.10"
         },
         "fqdn": {
             "hashes": [
                 "sha256:105ed3677e767fb5ca086a0c1f4bb66ebc3c100be518f0e0d755d9eae164d89f",
                 "sha256:3a179af3761e4df6eb2e026ff9e1a3033d3587bf980a0b1b2e1e5d08d7358014"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_full_version < '4.0.0'",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
             "version": "==1.5.1"
         },
         "gitdb": {
             "hashes": [
                 "sha256:6eb990b69df4e15bad899ea868dc46572c3f75339735663b81de79b06f17eb9a",
                 "sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7"
             ],
@@ -427,43 +379,43 @@
             "version": "==3.1.30"
         },
         "google-api-core": {
             "extras": [
                 "grpc"
             ],
             "hashes": [
-                "sha256:4b9bb5d5a380a0befa0573b302651b8a9a89262c1730e37bf423cec511804c22",
-                "sha256:ce222e27b0de0d7bc63eb043b956996d6dccab14cc3b690aaea91c9cc99dc16e"
+                "sha256:10c06f7739fe57781f87523375e8e1a3a4674bf6392cd6131a3222182b971320",
+                "sha256:34f24bd1d5f72a8c4519773d99ca6bf080a6c4e041b4e9f024fe230191dda62e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.11.0"
+            "version": "==2.10.2"
         },
         "google-auth": {
             "hashes": [
-                "sha256:a9cfa88b3e16196845e64a3658eb953992129d13ac7337b064c6546f77c17183",
-                "sha256:ea165e014c7cbd496558796b627c271aa8c18b4cba79dc1cc962b24c5efdfb85"
+                "sha256:164cba9af4e6e4e40c3a4f90a1a6c12ee56f14c0b4868d1ca91b32826ab334ce",
+                "sha256:d61d1b40897407b574da67da1a833bdc10d5a11642566e506565d1b1a46ba873"
             ],
             "index": "pypi",
-            "version": "==2.19.1"
+            "version": "==2.22.0"
         },
         "google-cloud-compute": {
             "hashes": [
                 "sha256:1ddd1be44d278754fc2643be7aa8d66838235ce44cfbacbeeadf3952ec020e95",
                 "sha256:21bd66251356d70bfd5f40211b42b936335490f7433b3b6fae7c498077e2c3fa"
             ],
             "index": "pypi",
             "version": "==1.3.2"
         },
         "google-cloud-core": {
             "hashes": [
-                "sha256:8417acf6466be2fa85123441696c4badda48db314c607cf1e5d543fa8bdc22fe",
-                "sha256:b9529ee7047fd8d4bf4a2182de619154240df17fbe60ead399078c1ae152af9a"
+                "sha256:37b80273c8d7eee1ae816b3a20ae43585ea50506cb0e60f3cf5be5f87f1373cb",
+                "sha256:fbd11cad3e98a7e5b0343dc07cb1039a5ffd7a5bb96e1f1e27cee4bda4a90863"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.3.2"
+            "version": "==2.3.3"
         },
         "google-cloud-dns": {
             "hashes": [
                 "sha256:41609782fa91df41e5ebfd48b127bb421a3b1821f5d49d900c484d13c0672167",
                 "sha256:bd75d6e9fd456ce643ee936a113a1ead5405704515caa679db30d7f036e447f3"
             ],
             "index": "pypi",
@@ -475,62 +427,61 @@
                 "sha256:b35d530fe825fb4227857bc47ad84c33c809ac96f312e13182bdeaa2abe1178a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.59.1"
         },
         "grpcio": {
             "hashes": [
-                "sha256:05f7c248e440f538aaad13eee78ef35f0541e73498dd6f832fe284542ac4b298",
-                "sha256:080b66253f29e1646ac53ef288c12944b131a2829488ac3bac8f52abb4413c0d",
-                "sha256:12b479839a5e753580b5e6053571de14006157f2ef9b71f38c56dc9b23b95ad6",
-                "sha256:156f8009e36780fab48c979c5605eda646065d4695deea4cfcbcfdd06627ddb6",
-                "sha256:15f9e6d7f564e8f0776770e6ef32dac172c6f9960c478616c366862933fa08b4",
-                "sha256:177afaa7dba3ab5bfc211a71b90da1b887d441df33732e94e26860b3321434d9",
-                "sha256:1a4cd8cb09d1bc70b3ea37802be484c5ae5a576108bad14728f2516279165dd7",
-                "sha256:1d8d02dbb616c0a9260ce587eb751c9c7dc689bc39efa6a88cc4fa3e9c138a7b",
-                "sha256:2b71916fa8f9eb2abd93151fafe12e18cebb302686b924bd4ec39266211da525",
-                "sha256:2d9fd6e38b16c4d286a01e1776fdf6c7a4123d99ae8d6b3f0b4a03a34bf6ce45",
-                "sha256:3b611b3de3dfd2c47549ca01abfa9bbb95937eb0ea546ea1d762a335739887be",
-                "sha256:3e4244c09cc1b65c286d709658c061f12c61c814be0b7030a2d9966ff02611e0",
-                "sha256:40838061e24f960b853d7bce85086c8e1b81c6342b1f4c47ff0edd44bbae2722",
-                "sha256:4b123fbb7a777a2fedec684ca0b723d85e1d2379b6032a9a9b7851829ed3ca9a",
-                "sha256:531f8b46f3d3db91d9ef285191825d108090856b3bc86a75b7c3930f16ce432f",
-                "sha256:67dd41a31f6fc5c7db097a5c14a3fa588af54736ffc174af4411d34c4f306f68",
-                "sha256:7489dbb901f4fdf7aec8d3753eadd40839c9085967737606d2c35b43074eea24",
-                "sha256:8d4c8e73bf20fb53fe5a7318e768b9734cf122fe671fcce75654b98ba12dfb75",
-                "sha256:8e69aa4e9b7f065f01d3fdcecbe0397895a772d99954bb82eefbb1682d274518",
-                "sha256:8e8999a097ad89b30d584c034929f7c0be280cd7851ac23e9067111167dcbf55",
-                "sha256:906f4d1beb83b3496be91684c47a5d870ee628715227d5d7c54b04a8de802974",
-                "sha256:92d7635d1059d40d2ec29c8bf5ec58900120b3ce5150ef7414119430a4b2dd5c",
-                "sha256:931e746d0f75b2a5cff0a1197d21827a3a2f400c06bace036762110f19d3d507",
-                "sha256:95ce51f7a09491fb3da8cf3935005bff19983b77c4e9437ef77235d787b06842",
-                "sha256:9eea18a878cffc804506d39c6682d71f6b42ec1c151d21865a95fae743fda500",
-                "sha256:a23d47f2fc7111869f0ff547f771733661ff2818562b04b9ed674fa208e261f4",
-                "sha256:a4c23e54f58e016761b576976da6a34d876420b993f45f66a2bfb00363ecc1f9",
-                "sha256:a50a1be449b9e238b9bd43d3857d40edf65df9416dea988929891d92a9f8a778",
-                "sha256:ab5d0e3590f0a16cb88de4a3fa78d10eb66a84ca80901eb2c17c1d2c308c230f",
-                "sha256:ae23daa7eda93c1c49a9ecc316e027ceb99adbad750fbd3a56fa9e4a2ffd5ae0",
-                "sha256:af98d49e56605a2912cf330b4627e5286243242706c3a9fa0bcec6e6f68646fc",
-                "sha256:b2f77a90ba7b85bfb31329f8eab9d9540da2cf8a302128fb1241d7ea239a5469",
-                "sha256:baab51dcc4f2aecabf4ed1e2f57bceab240987c8b03533f1cef90890e6502067",
-                "sha256:ca8a2254ab88482936ce941485c1c20cdeaef0efa71a61dbad171ab6758ec998",
-                "sha256:cb11464f480e6103c59d558a3875bd84eed6723f0921290325ebe97262ae1347",
-                "sha256:ce8513aee0af9c159319692bfbf488b718d1793d764798c3d5cff827a09e25ef",
-                "sha256:cf151f97f5f381163912e8952eb5b3afe89dec9ed723d1561d59cabf1e219a35",
-                "sha256:d144ad10eeca4c1d1ce930faa105899f86f5d99cecfe0d7224f3c4c76265c15e",
-                "sha256:d534d169673dd5e6e12fb57cc67664c2641361e1a0885545495e65a7b761b0f4",
-                "sha256:d75061367a69808ab2e84c960e9dce54749bcc1e44ad3f85deee3a6c75b4ede9",
-                "sha256:d84d04dec64cc4ed726d07c5d17b73c343c8ddcd6b59c7199c801d6bbb9d9ed1",
-                "sha256:de411d2b030134b642c092e986d21aefb9d26a28bf5a18c47dd08ded411a3bc5",
-                "sha256:e07fe0d7ae395897981d16be61f0db9791f482f03fee7d1851fe20ddb4f69c03",
-                "sha256:ea8ccf95e4c7e20419b7827aa5b6da6f02720270686ac63bd3493a651830235c",
-                "sha256:f7025930039a011ed7d7e7ef95a1cb5f516e23c5a6ecc7947259b67bea8e06ca"
+                "sha256:06e84ad9ae7668a109e970c7411e7992751a116494cba7c4fb877656527f9a57",
+                "sha256:0ff789ae7d8ddd76d2ac02e7d13bfef6fc4928ac01e1dcaa182be51b6bcc0aaa",
+                "sha256:10954662f77dc36c9a1fb5cc4a537f746580d6b5734803be1e587252682cda8d",
+                "sha256:139f66656a762572ae718fa0d1f2dce47c05e9fbf7a16acd704c354405b97df9",
+                "sha256:1c31e52a04e62c8577a7bf772b3e7bed4df9c9e0dd90f92b6ffa07c16cab63c9",
+                "sha256:33971197c47965cc1d97d78d842163c283e998223b151bab0499b951fd2c0b12",
+                "sha256:345356b307cce5d14355e8e055b4ca5f99bc857c33a3dc1ddbc544fca9cd0475",
+                "sha256:373b48f210f43327a41e397391715cd11cfce9ded2fe76a5068f9bacf91cc226",
+                "sha256:3ccb621749a81dc7755243665a70ce45536ec413ef5818e013fe8dfbf5aa497b",
+                "sha256:42a3bbb2bc07aef72a7d97e71aabecaf3e4eb616d39e5211e2cfe3689de860ca",
+                "sha256:42e63904ee37ae46aa23de50dac8b145b3596f43598fa33fe1098ab2cbda6ff5",
+                "sha256:4eb37dd8dd1aa40d601212afa27ca5be255ba792e2e0b24d67b8af5e012cdb7d",
+                "sha256:51173e8fa6d9a2d85c14426bdee5f5c4a0654fd5fddcc21fe9d09ab0f6eb8b35",
+                "sha256:5144feb20fe76e73e60c7d73ec3bf54f320247d1ebe737d10672480371878b48",
+                "sha256:5344be476ac37eb9c9ad09c22f4ea193c1316bf074f1daf85bddb1b31fda5116",
+                "sha256:6108e5933eb8c22cd3646e72d5b54772c29f57482fd4c41a0640aab99eb5071d",
+                "sha256:6a007a541dff984264981fbafeb052bfe361db63578948d857907df9488d8774",
+                "sha256:6ee26e9dfb3996aff7c870f09dc7ad44a5f6732b8bdb5a5f9905737ac6fd4ef1",
+                "sha256:750de923b456ca8c0f1354d6befca45d1f3b3a789e76efc16741bd4132752d95",
+                "sha256:7c5ede2e2558f088c49a1ddda19080e4c23fb5d171de80a726b61b567e3766ed",
+                "sha256:830215173ad45d670140ff99aac3b461f9be9a6b11bee1a17265aaaa746a641a",
+                "sha256:8391cea5ce72f4a12368afd17799474015d5d3dc00c936a907eb7c7eaaea98a5",
+                "sha256:8940d6de7068af018dfa9a959a3510e9b7b543f4c405e88463a1cbaa3b2b379a",
+                "sha256:89a49cc5ad08a38b6141af17e00d1dd482dc927c7605bc77af457b5a0fca807c",
+                "sha256:900bc0096c2ca2d53f2e5cebf98293a7c32f532c4aeb926345e9747452233950",
+                "sha256:97e0efaebbfd222bcaac2f1735c010c1d3b167112d9d237daebbeedaaccf3d1d",
+                "sha256:9e04d4e4cfafa7c5264e535b5d28e786f0571bea609c3f0aaab13e891e933e9c",
+                "sha256:a4c60abd950d6de3e4f1ddbc318075654d275c29c846ab6a043d6ed2c52e4c8c",
+                "sha256:a6ff459dac39541e6a2763a4439c4ca6bc9ecb4acc05a99b79246751f9894756",
+                "sha256:a72797549935c9e0b9bc1def1768c8b5a709538fa6ab0678e671aec47ebfd55e",
+                "sha256:af4063ef2b11b96d949dccbc5a987272f38d55c23c4c01841ea65a517906397f",
+                "sha256:b975b85d1d5efc36cf8b237c5f3849b64d1ba33d6282f5e991f28751317504a1",
+                "sha256:bf0b9959e673505ee5869950642428046edb91f99942607c2ecf635f8a4b31c9",
+                "sha256:c0c85c5cbe8b30a32fa6d802588d55ffabf720e985abe9590c7c886919d875d4",
+                "sha256:c3f3237a57e42f79f1e560726576aedb3a7ef931f4e3accb84ebf6acc485d316",
+                "sha256:c3fa3ab0fb200a2c66493828ed06ccd1a94b12eddbfb985e7fd3e5723ff156c6",
+                "sha256:c435f5ce1705de48e08fcbcfaf8aee660d199c90536e3e06f2016af7d6a938dd",
+                "sha256:c90da4b124647547a68cf2f197174ada30c7bb9523cb976665dfd26a9963d328",
+                "sha256:cbdf2c498e077282cd427cfd88bdce4668019791deef0be8155385ab2ba7837f",
+                "sha256:d1fbad1f9077372b6587ec589c1fc120b417b6c8ad72d3e3cc86bbbd0a3cee93",
+                "sha256:d39f5d4af48c138cb146763eda14eb7d8b3ccbbec9fe86fb724cd16e0e914c64",
+                "sha256:ddb4a6061933bd9332b74eac0da25f17f32afa7145a33a0f9711ad74f924b1b8",
+                "sha256:ded637176addc1d3eef35331c39acc598bac550d213f0a1bedabfceaa2244c87",
+                "sha256:f20fd21f7538f8107451156dd1fe203300b79a9ddceba1ee0ac8132521a008ed",
+                "sha256:fda2783c12f553cdca11c08e5af6eecbd717280dc8fbe28a110897af1c15a88c"
             ],
-            "index": "pypi",
-            "version": "==1.50.0"
+            "version": "==1.56.2"
         },
         "grpcio-status": {
             "hashes": [
                 "sha256:2c33bbdbe20188b2953f46f31af669263b6ee2a9b2d38fa0d36ee091532e21bf",
                 "sha256:53695f45da07437b7c344ee4ef60d370fd2850179f5a28bb26d8e2aa1102ec11"
             ],
             "version": "==1.48.2"
@@ -596,18 +547,18 @@
                 "sha256:90261b206d6defd58fdd5e85f478bf633a2901798906be2ad389150c5c60edbe"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.1"
         },
         "jsonpointer": {
             "hashes": [
-                "sha256:51801e558539b4e9cd268638c078c6c5746c9ac96bc38152d443400e4f3793e9",
-                "sha256:97cba51526c829282218feb99dab1b1e6bdf8efd1c43dc9d57be093c0d69c99a"
+                "sha256:15d51bba20eea3165644553647711d150376234112651b4f1811022aecad7d7a",
+                "sha256:585cee82b70211fa9e6043b7bb89db6e1aa49524340dde8ad6b63206ea689d88"
             ],
-            "version": "==2.3"
+            "version": "==2.4"
         },
         "jsonschema": {
             "extras": [
                 "format_nongpl"
             ],
             "hashes": [
                 "sha256:4e5b3cf8216f577bee9ce139cbe72eca3ea4f292ec60928ff24758ce626cd163",
@@ -668,19 +619,19 @@
                 "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
             ],
             "index": "pypi",
             "version": "==2.1.1"
         },
         "natsort": {
             "hashes": [
-                "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
-                "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
+                "sha256:45312c4a0e5507593da193dedd04abb1469253b601ecaf63445ad80f0a1ea581",
+                "sha256:4732914fb471f56b5cce04d7bae6f164a592c7712e1c85f9ef585e197299521c"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==8.3.1"
+            "version": "==8.4.0"
         },
         "oauthlib": {
             "hashes": [
                 "sha256:8139f29aac13e25d502680e9e19963e83f16838d48a0d71c287fe40e7067fbca",
                 "sha256:9859c40929662bec5d64f34d01c99e093149682a3f38915dc0655d5a633dd918"
             ],
             "markers": "python_version >= '3.6'",
@@ -690,21 +641,14 @@
             "hashes": [
                 "sha256:9c31bd5cdbdbe5ef678cb01ac0564461790126acb9c3ab51a0f63fc9eaf608c8",
                 "sha256:aa629a2b75714a5c15c47125b6e1c4226492d7fe4c5b348c081c8b4cf87ce0ae"
             ],
             "index": "pypi",
             "version": "==0.9.14"
         },
-        "openshift": {
-            "hashes": [
-                "sha256:a060afb7565dda18b2749857867d80ab22b2f4143264519f493a9cabccc3b8a8"
-            ],
-            "index": "pypi",
-            "version": "==0.13.1"
-        },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
@@ -713,45 +657,37 @@
             "hashes": [
                 "sha256:e547125940bcc052856ded43be8e101f63828c2d94239ffbe2b327ba3d5ccf0a",
                 "sha256:e8dca2f4b43560edef58813969f52a56cef023146cbb8931626db80e6c1c4308"
             ],
             "index": "pypi",
             "version": "==5.9.0"
         },
-        "pip": {
-            "hashes": [
-                "sha256:0e7c86f486935893c708287b30bd050a36ac827ec7fe5e43fe7cb198dd835fba",
-                "sha256:3ef6ac33239e4027d9a5598a381b9d30880a1477e50039db2eac6e8a8f6d1b18"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.1.2"
-        },
         "pipenv": {
             "hashes": [
-                "sha256:3b80b4512934b9d8e8ce12c988394642ff96bb697680e5b092e59af503178327",
-                "sha256:f84d7119239b22ab2ac2b8fbc7d619d83cf41135206d72a17c4f151cda529fd0"
+                "sha256:116061545d4e2281cbc799f7736a715ee5ddf0a6f63c09f4263a4a6a0779fe93",
+                "sha256:404de9ff6a2464e20e52aaad71db2d4f8f2900f2177fc45a47f6315686cb2e5b"
             ],
             "index": "pypi",
-            "version": "==2022.1.8"
+            "version": "==2023.7.3"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:0ade98a4895e87dc51d47151f7d2ec290365a585151d97b4d8d6312ed6132fed",
-                "sha256:e48fabd87db8f3a7df7150a4a5ea22c546ee8bc39bc2473244730d4b56d2cc4e"
+                "sha256:1b42b450ad933e981d56e59f1b97495428c9bd60698baab9f3eb3d00d5822421",
+                "sha256:ad8291ae0ae5072f66c16945166cb11c63394c7a3ad1b1bc9828ca3162da8c2f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.3"
+            "version": "==3.9.1"
         },
         "pluggy": {
             "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
+                "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
+                "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.0.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.2.0"
         },
         "pprintpp": {
             "hashes": [
                 "sha256:b6b4dcdd0c0c0d75e4d7b2f21a9e933e5b2ce62b26e1a54537f9651ae5a5c01d",
                 "sha256:ea826108e2c7f49dc6d66c752973c3fc9749142a798d6b254e1e301cfdbc6403"
             ],
             "version": "==0.4.0"
@@ -762,19 +698,19 @@
                 "sha256:03481bca25ae0c28958c8cd6ac5165c159ce89f7ccde04d5c899b24b68bb13b7"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==3.8.0"
         },
         "proto-plus": {
             "hashes": [
-                "sha256:0e8cda3d5a634d9895b75c573c9352c16486cb75deb0e078b5fda34db4243165",
-                "sha256:de34e52d6c9c6fcd704192f09767cb561bb4ee64e70eede20b0834d841f0be4d"
+                "sha256:a49cd903bc0b6ab41f76bf65510439d56ca76f868adf0274e738bfdd096894df",
+                "sha256:fdcd09713cbd42480740d2fe29c990f7fbd885a67efc328aa8be6ee3e9f76a6b"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==1.22.2"
+            "version": "==1.22.3"
         },
         "protobuf": {
             "hashes": [
                 "sha256:03038ac1cfbc41aa21f6afcbcd357281d7521b4157926f30ebecc8d4ea59dcb7",
                 "sha256:28545383d61f55b57cf4df63eebd9827754fd2dc25f80c5253f9184235db242c",
                 "sha256:2e3427429c9cffebf259491be0af70189607f365c2f41c7c3764af6f337105f2",
                 "sha256:398a9e0c3eaceb34ec1aee71894ca3299605fa8e761544934378bbc6c97de23b",
@@ -816,15 +752,15 @@
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==0.3.0"
         },
         "pycountry": {
             "hashes": [
                 "sha256:b2163a246c585894d808f18783e19137cb70a0c18fb36748dc01fc6f109c1646"
             ],
-            "markers": "python_version >= '3.6' and python_full_version < '4.0.0'",
+            "markers": "python_version >= '3.6' and python_version < '4'",
             "version": "==22.3.5"
         },
         "pycountry-convert": {
             "hashes": [
                 "sha256:095d310f746bf2a5ef713b3a82eea28a27262286223765b1e7be8a5c4fa7e9b9",
                 "sha256:5e33883a88b3cb752d332ca2358ac6c4de4defc86a2b93b713b36338e914952e"
             ],
@@ -843,19 +779,19 @@
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pyparsing": {
             "hashes": [
-                "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb",
-                "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
+                "sha256:d554a96d1a7d3ddaf7183104485bc19fd80543ad6ac5bdb6426719d766fb06c1",
+                "sha256:edb662d6fe322d6e990b1594b5feaeadf806803359e3d4d42f11e295e588f0ea"
             ],
             "markers": "python_full_version >= '3.6.8'",
-            "version": "==3.0.9"
+            "version": "==3.1.0"
         },
         "pyperclip": {
             "hashes": [
                 "sha256:105254a8b04934f0bc84e9c24eb360a591aaf6535c9def5f29d92af107a9bf57"
             ],
             "version": "==1.8.2"
         },
@@ -864,35 +800,35 @@
                 "sha256:cdc7b5e3ed77bed61270a47d35434a30617b9becdf2478af76ad2c6ade307280"
             ],
             "index": "pypi",
             "version": "==0.15.7"
         },
         "pytest": {
             "hashes": [
-                "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295",
-                "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"
+                "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
+                "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.3.2"
+            "version": "==7.4.0"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6",
                 "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.1.0"
         },
         "pytest-mock": {
             "hashes": [
-                "sha256:f4c973eeae0282963eb293eb173ce91b091a79c1334455acfac9ddee8a1c784b",
-                "sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f"
+                "sha256:21c279fff83d70763b05f8874cc9cfb3fcacd6d354247a976f9529d19f9acf39",
+                "sha256:7f6b125602ac6d743e523ae0bfa71e1a697a2f5534064528c6ff84c2f7c2fc7f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.10.0"
+            "version": "==3.11.1"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "index": "pypi",
@@ -902,67 +838,59 @@
             "hashes": [
                 "sha256:85ae778d8953aba87ad4b78aef7fbb5dae053980d2c20ff200bea29799685743",
                 "sha256:ad502b72b5d1137f4af37d4a68ae20fe7d6c9778f67cbe2aec566f7995053c7d"
             ],
             "index": "pypi",
             "version": "==3.13.0"
         },
-        "python-string-utils": {
-            "hashes": [
-                "sha256:dcf9060b03f07647c0a603408dc8b03f807f3b54a05c6e19eb14460256fac0cb",
-                "sha256:f1a88700baf99db1a9b6953f44181ad9ca56623c81e257e6009707e2e7851fa4"
-            ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.0"
-        },
         "pyyaml": {
             "hashes": [
-                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
-                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
-                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
-                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
-                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
-                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
-                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
-                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
-                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
-                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
-                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
-                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
-                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
-                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
-                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
-                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
-                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
-                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
-                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
-                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
-                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
-                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
-                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
-                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
-                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
-                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
-                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
-                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
-                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
-                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
-                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
-                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
-                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
-                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
-                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
-                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
-                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
-                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
-                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
-                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
+                "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
+                "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
+                "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
+                "sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27",
+                "sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595",
+                "sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62",
+                "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98",
+                "sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696",
+                "sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d",
+                "sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867",
+                "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47",
+                "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486",
+                "sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6",
+                "sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3",
+                "sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007",
+                "sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938",
+                "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
+                "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
+                "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
+                "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
+                "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
+                "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
+                "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
+                "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
+                "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
+                "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
+                "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
+                "sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924",
+                "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34",
+                "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43",
+                "sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859",
+                "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673",
+                "sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a",
+                "sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab",
+                "sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa",
+                "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c",
+                "sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585",
+                "sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d",
+                "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"
             ],
             "index": "pypi",
-            "version": "==6.0"
+            "version": "==6.0.1"
         },
         "redis": {
             "hashes": [
                 "sha256:68226f7ede928db8302f29ab088a157f41061fa946b7ae865452b6d7838bbffb",
                 "sha256:da92a39fec86438d3f1e2a1db33c312985806954fe860120b582a8430e231d8f"
             ],
             "index": "pypi",
@@ -1029,90 +957,47 @@
             "version": "==12.4.4"
         },
         "rsa": {
             "hashes": [
                 "sha256:90260d9058e514786967344d0ef75fa8727eed8a7d2e43ce9f4bcf1b536174f7",
                 "sha256:e38464a49c6c85d7f1351b0126661487a7e0a14a50f1675ec50eb34d4f20ef21"
             ],
-            "markers": "python_version >= '3.6' and python_full_version < '4.0.0'",
+            "markers": "python_version >= '3.6' and python_version < '4'",
             "version": "==4.9"
         },
         "ruamel.yaml": {
             "hashes": [
                 "sha256:742b35d3d665023981bd6d16b3d24248ce5df75fdb4e2924e93a05c1f8b61ca7",
                 "sha256:8b7ce697a2f212752a35c1ac414471dc16c424c9573be4926b56ff3f5d23b7af"
             ],
             "index": "pypi",
             "version": "==0.17.21"
         },
-        "ruamel.yaml.clib": {
-            "hashes": [
-                "sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e",
-                "sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3",
-                "sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5",
-                "sha256:1a6391a7cabb7641c32517539ca42cf84b87b667bad38b78d4d42dd23e957c81",
-                "sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497",
-                "sha256:2aa261c29a5545adfef9296b7e33941f46aa5bbd21164228e833412af4c9c75f",
-                "sha256:3110a99e0f94a4a3470ff67fc20d3f96c25b13d24c6980ff841e82bafe827cac",
-                "sha256:3243f48ecd450eddadc2d11b5feb08aca941b5cd98c9b1db14b2fd128be8c697",
-                "sha256:370445fd795706fd291ab00c9df38a0caed0f17a6fb46b0f607668ecb16ce763",
-                "sha256:40d030e2329ce5286d6b231b8726959ebbe0404c92f0a578c0e2482182e38282",
-                "sha256:41d0f1fa4c6830176eef5b276af04c89320ea616655d01327d5ce65e50575c94",
-                "sha256:4a4d8d417868d68b979076a9be6a38c676eca060785abaa6709c7b31593c35d1",
-                "sha256:4b3a93bb9bc662fc1f99c5c3ea8e623d8b23ad22f861eb6fce9377ac07ad6072",
-                "sha256:5bc0667c1eb8f83a3752b71b9c4ba55ef7c7058ae57022dd9b29065186a113d9",
-                "sha256:763d65baa3b952479c4e972669f679fe490eee058d5aa85da483ebae2009d231",
-                "sha256:7bdb4c06b063f6fd55e472e201317a3bb6cdeeee5d5a38512ea5c01e1acbdd93",
-                "sha256:8831a2cedcd0f0927f788c5bdf6567d9dc9cc235646a434986a852af1cb54b4b",
-                "sha256:91a789b4aa0097b78c93e3dc4b40040ba55bef518f84a40d4442f713b4094acb",
-                "sha256:92460ce908546ab69770b2e576e4f99fbb4ce6ab4b245345a3869a0a0410488f",
-                "sha256:99e77daab5d13a48a4054803d052ff40780278240a902b880dd37a51ba01a307",
-                "sha256:9c7617df90c1365638916b98cdd9be833d31d337dbcd722485597b43c4a215bf",
-                "sha256:a234a20ae07e8469da311e182e70ef6b199d0fbeb6c6cc2901204dd87fb867e8",
-                "sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b",
-                "sha256:be2a7ad8fd8f7442b24323d24ba0b56c51219513cfa45b9ada3b87b76c374d4b",
-                "sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640",
-                "sha256:c3ca1fbba4ae962521e5eb66d72998b51f0f4d0f608d3c0347a48e1af262efa7",
-                "sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a",
-                "sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71",
-                "sha256:d5e51e2901ec2366b79f16c2299a03e74ba4531ddcfacc1416639c557aef0ad8",
-                "sha256:da538167284de58a52109a9b89b8f6a53ff8437dd6dc26d33b57bf6699153122",
-                "sha256:debc87a9516b237d0466a711b18b6ebeb17ba9f391eb7f91c649c5c4ec5006c7",
-                "sha256:df5828871e6648db72d1c19b4bd24819b80a755c4541d3409f0f7acd0f335c80",
-                "sha256:ecdf1a604009bd35c674b9225a8fa609e0282d9b896c03dd441a91e5f53b534e",
-                "sha256:efa08d63ef03d079dcae1dfe334f6c8847ba8b645d08df286358b1f5293d24ab",
-                "sha256:f01da5790e95815eb5a8a138508c01c758e5f5bc0ce4286c4f7028b8dd7ac3d0",
-                "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646",
-                "sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38"
-            ],
-            "markers": "platform_python_implementation == 'CPython' and python_version < '3.11'",
-            "version": "==0.2.7"
-        },
         "s3transfer": {
             "hashes": [
                 "sha256:3c0da2d074bf35d6870ef157158641178a4204a6e689e82546083e31e0311346",
                 "sha256:640bb492711f4c0c0905e1f62b6aaeb771881935ad27884852411f8e9cacbca9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.6.1"
         },
         "setuptools": {
             "hashes": [
-                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
-                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.8.0"
+            "version": "==68.0.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
-            "index": "pypi",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
             "version": "==1.16.0"
         },
         "smmap": {
             "hashes": [
                 "sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94",
                 "sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936"
             ],
@@ -1123,39 +1008,22 @@
             "hashes": [
                 "sha256:a547de73308fd7e90075bb4d301405bebf705292fa90a90fc3bcf9133f58616c",
                 "sha256:f40253887d8712eaa2bb0ea3830374416736dc8ec0e22f5a65092c1174c44335"
             ],
             "index": "pypi",
             "version": "==3.5.0"
         },
-        "subprocess32": {
-            "hashes": [
-                "sha256:88e37c1aac5388df41cc8a8456bb49ebffd321a3ad4d70358e3518176de3a56b",
-                "sha256:e45d985aef903c5b7444d34350b05da91a9e0ea015415ab45a21212786c649d0",
-                "sha256:eb2937c80497978d181efa1b839ec2d9622cf9600a039a79d0e108d1f9aec79d"
-            ],
-            "index": "pypi",
-            "version": "==3.5.4"
-        },
         "supervisor": {
             "hashes": [
                 "sha256:2ecaede32fc25af814696374b79e42644ecaba5c09494c51016ffda9602d0f08",
                 "sha256:34761bae1a23c58192281a5115fb07fbf22c9b0133c08166beffc70fed3ebc12"
             ],
             "index": "pypi",
             "version": "==4.2.5"
         },
-        "tomli": {
-            "hashes": [
-                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
-                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
-            ],
-            "markers": "python_version < '3.11'",
-            "version": "==2.0.1"
-        },
         "typing-extensions": {
             "hashes": [
                 "sha256:1a9462dcc3347a79b1f1c0271fbe79e844580bb598bafa1ed208b94da3cdcd42",
                 "sha256:21c85e0fe4b9a155d0799430b0ad741cdce7e359660ccbd8b530613e8df88ce2"
             ],
             "index": "pypi",
             "version": "==4.1.1"
@@ -1174,19 +1042,19 @@
                 "sha256:cade07c403c397f9fe275492a48c1b869efd175d5d8a692df649e6e7e2ed8f4e"
             ],
             "index": "pypi",
             "version": "==0.18.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
-                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
+                "sha256:43a3052be36080548bdee0b42919c88072037d50d56c28bd3f853cbe92b953ff",
+                "sha256:fd8a78f46f6b99a67b7ec5cf73f92357891a7b3a40fd97637c27f854aae3b9e0"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.23.0"
+            "version": "==20.24.2"
         },
         "virtualenv-clone": {
             "hashes": [
                 "sha256:418ee935c36152f8f153c79824bb93eaf6f0f7984bae31d3f48f350b9183501a",
                 "sha256:44d5263bceed0bac3e1424d64f798095233b64def1c5689afa43dc3223caf5b0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1204,40 +1072,40 @@
                 "sha256:29bc7e8752c0a1bd4a1f03c14d6e6a72e93d82193738fa860cbff59d0fcc11bf",
                 "sha256:c225b674c83fa923be93d235330ce0300373d02885cef23238813b0d5668304a"
             ],
             "version": "==1.13"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:3566f8467cd350874c4913816355642a4942f6c1ed1e9406e3d42fae6d6c072a",
-                "sha256:b96f3bce3e54e3486ebe6504bc22bd4c140392bd2eb71764db29be8f2639aa65"
+                "sha256:c951af98631d24f8df89ab1019fc365f2227c0892f12fd150e935607c79dd0dd",
+                "sha256:f1f9f2ad5291f0225a49efad77abf9e700b6fef553900623060dad6e26503b9d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.5.3"
+            "version": "==1.6.1"
         },
         "werkzeug": {
             "hashes": [
                 "sha256:935539fa1413afbb9195b24880778422ed620c0fc09670945185cce4d91a8890",
                 "sha256:98c774df2f91b05550078891dee5f0eb0cb797a522c757a2452b9cee5b202330"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==2.3.6"
         },
         "wheel": {
             "hashes": [
-                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
-                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
+                "sha256:55a0f0a5a84869bce5ba775abfd9c462e3a6b1b7b7ec69d72c0b83d673a5114d",
+                "sha256:7e9be3bbd0078f6147d82ed9ed957e323e7708f57e134743d2edef3a7b7972a9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.40.0"
+            "version": "==0.41.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
-                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
+                "sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0",
+                "sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.15.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.16.2"
         }
     },
     "develop": {}
 }
```

### Comparing `unfurl-0.7.1/unfurl/templates/secrets.yaml.j2` & `unfurl-0.8.0/unfurl/templates/secrets.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/templates/service-template.yaml.j2` & `unfurl-0.8.0/unfurl/templates/service-template.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/templates/unfurl.local.yaml.j2` & `unfurl-0.8.0/unfurl/templates/unfurl.local.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/templates/unfurl.yaml.j2` & `unfurl-0.8.0/unfurl/templates/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/to_json.py` & `unfurl-0.8.0/unfurl/to_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import os
 import os.path
 import sys
 import itertools
 import json
 import datetime
 from time import perf_counter
+import traceback
 from typing import (
     Any,
     Dict,
     Iterator,
     List,
     NewType,
     Optional,
@@ -30,14 +31,15 @@
     cast,
     TYPE_CHECKING,
 )
 from collections import Counter
 from collections.abc import Mapping, MutableSequence
 from typing_extensions import TypedDict
 from urllib.parse import urlparse
+from toscaparser.imports import is_url
 from toscaparser.substitution_mappings import SubstitutionMappings
 from toscaparser.properties import Property
 from toscaparser.elements.constraints import Schema
 from toscaparser.elements.property_definition import PropertyDef
 from toscaparser.elements.nodetype import NodeType
 from toscaparser.elements.relationshiptype import RelationshipType
 from toscaparser.elements.statefulentitytype import StatefulEntityType
@@ -45,14 +47,15 @@
 from toscaparser.common.exception import ExceptionCollector
 from toscaparser.elements.scalarunit import get_scalarunit_class
 from toscaparser.elements.datatype import DataType
 from toscaparser.elements.portspectype import PortSpec
 from toscaparser.activities import ConditionClause
 from toscaparser.nodetemplate import NodeTemplate
 from toscaparser.relationship_template import RelationshipTemplate
+from .repo import sanitize_url
 from .runtime import EntityInstance, TopologyInstance
 from .yamlmanifest import YamlManifest
 from .merge import merge_dicts, patch_dict
 from .logs import sensitive, is_sensitive, getLogger
 from .tosca import (
     EntitySpec,
     NodeSpec,
@@ -243,15 +246,15 @@
         custom_defs,
     )
     toscaSchema = prop.schema
     tosca_type = toscaSchema.type
     schema = {}
     if toscaSchema.title or p.name:
         schema["title"] = toscaSchema.title or p.name
-    if toscaSchema.default is not None and not is_value_computed(toscaSchema.default):
+    if toscaSchema.default is not None and not is_server_only_expression(toscaSchema.default):
         schema["default"] = toscaSchema.default
     if toscaSchema.required:
         schema["required"] = True
     if toscaSchema.description:
         schema["description"] = toscaSchema.description
 
     metadata = toscaSchema.schema.get("metadata")
@@ -292,15 +295,16 @@
     return schema
 
 
 def _requirement_visibility(topology: TopologySpec, name: str, req) -> str:
     if name in ["dependency", "installer"]:
         # skip artifact requirements and the base TOSCA relationship type that every node has
         return "omit"
-    node = req.get("node")
+    #  reqconstaint_from_nodetemplate() adds match
+    node = req.get("match") or req.get("node")
     metadata = req.get("metadata") or {}
     if metadata.get("visibility"):
         return metadata["visibility"]
     if metadata.get("internal"):
         return "hidden"
     if node:
         nodespec = topology.get_node_template(node)
@@ -388,15 +392,15 @@
             if reqtypename:
                 _annotate_requirement(reqobj, reqtypename, topology, types)
 
     return name, req, reqobj
 
 
 def requirement_to_graphql(
-    topology: TopologySpec, req_dict: dict
+    topology: TopologySpec, req_dict: dict, include_omitted = False
 ) -> Optional[GraphqlObject]:
     """
     type RequirementConstraint {
         name: String!
         title: String
         description: String
         resourceType: ResourceType!
@@ -413,15 +417,15 @@
     name, req, reqobj = _make_req(req_dict)
     if "min" not in reqobj:
         # set defaults
         reqobj["min"] = 1
         reqobj["max"] = 1
 
     visibility = _requirement_visibility(topology, name, req)
-    if visibility == "omit":
+    if not include_omitted and visibility == "omit":
         return None
 
     if visibility != "inherit":
         reqobj["visibility"] = visibility
 
     if reqobj["max"] == 0:
         return None
@@ -433,14 +437,15 @@
         if nodetype in topology.node_templates:
             reqobj["match"] = nodetype
             nodetype = topology.node_templates[nodetype].type
         nodetype = expand_prefix(nodetype)
     else:
         nodetype = req.get("capability")
         if not nodetype:
+            # XXX check for "relationship" and get it's valid_target_types
             logger.warning(
                 "skipping constraint %s, there was no type specified ", req_dict
             )
             return None
     reqobj["resourceType"] = nodetype
     return reqobj
 
@@ -454,14 +459,15 @@
     if not typedef:
         return
     name = typedef.type
     if name not in extends:
         extends.append(name)
     if types is not None and name not in types:
         node_type_to_graphql(topology, typedef, types)
+    ExceptionCollector.collecting = True
     for p in typedef.parent_types():
         _get_extends(topology, p, extends, types)
 
 
 def template_visibility(t: EntitySpec, discovered):
     metadata = t.toscaEntityTemplate.entity_tpl.get("metadata")
     if metadata:
@@ -475,41 +481,41 @@
     if "default" in t.directives:
         return "hidden"
     if discovered and t.nested_name in discovered:
         return "omit"
     return "inherit"
 
 
-def is_property_user_visible(p: PropertyDef):
+def is_property_user_visible(p: PropertyDef) -> bool:
     user_settable = p.schema.get("metadata", {}).get("user_settable")
     if user_settable is not None:
         return user_settable
     if p.default is not None or is_computed(p):
         return False
     return True
 
 
-def is_value_computed(value):
+def is_server_only_expression(value) -> bool:
     if isinstance(value, list):
         return any(is_function(item) or is_template(item) for item in value)
-    if isinstance(value, dict) and "_generate" in value:  # special case for client
+    if _is_front_end_expression(value):  # special case for client
         return False
     return is_function(value) or is_template(value)
 
 
-def is_computed(p):  # p: Property | PropertyDef
+def is_computed(p) -> bool:  # p: Property | PropertyDef
     # XXX be smarter about is_computed() if the user should be able to override the default
     if isinstance(p.schema, Schema):
         metadata = p.schema.metadata
     else:
         metadata = p.schema.get("metadata") or {}
     return (
         p.name in ["tosca_id", "state", "tosca_name"]
-        or is_value_computed(p.value)
-        or (p.value is None and is_value_computed(p.default))
+        or is_server_only_expression(p.value)
+        or (p.value is None and is_server_only_expression(p.default))
         or metadata.get("computed")
     )
 
 
 def always_export(p: Property) -> bool:
     if isinstance(p.schema, Schema):
         metadata = p.schema.metadata
@@ -541,17 +547,21 @@
 
 # def property_value_to_json(p, value):
 #     if is_computed(p):
 #         return None
 #     return attribute_value_to_json(p, value)
 
 
-def _is_get_env_or_secret(value) -> bool:
+def _is_front_end_expression(value) -> bool:
     if isinstance(value, dict):
-        return "get_env" in value or "secret" in value or "_generate" in value
+        if "eval" in value:
+            expr = value['eval']
+            return "abspath" in expr or "get_dir" in expr
+        else:
+            return "get_env" in value or "secret" in value or "_generate" in value
     return False
 
 
 class PropertyVisitor:
     redacted = False
     user_settable = False
 
@@ -564,15 +574,15 @@
             self.redacted = True
             return sensitive.redacted_str
         else:
             return value
 
     def attribute_value_to_json(self, p, value):
         if p.schema.metadata.get("sensitive"):
-            if is_value_computed(value) or _is_get_env_or_secret(value):
+            if is_server_only_expression(value) or _is_front_end_expression(value):
                 return value
             self.redacted = True
             return sensitive.redacted_str
 
         if isinstance(value, PortSpec):
             return value.spec
         elif isinstance(value, dict) and p.type in [
@@ -588,19 +598,57 @@
         return self.redact_if_sensitive(value)
 
 
 def attribute_value_to_json(p, value):
     return PropertyVisitor().attribute_value_to_json(p, value)
 
 
+def _get_source_info(source_info: dict) -> dict:
+    _import = {}
+    root = source_info["root"]
+    prefix = source_info.get("prefix")
+    if prefix:
+        _import["prefix"] = prefix
+    repository = source_info.get("repository")
+    if repository:
+        _import["repository"] = repository
+        _import["url"] = root
+        _import["file"] = source_info["file"]
+    else:
+        path = source_info["path"]
+        base = source_info["base"]
+        # make path relative to the import base (not the file that imported)
+        # and include the fragment if present
+        # base and path will both be local file paths
+        _import["file"] = path[len(base) :].strip('/') + "".join(
+            source_info["file"].partition("#")[1:]
+        )
+        if is_url(root):
+            _import["url"] = root
+        # otherwise import relative to main service template
+    return _import
+
+
+def add_root_source_info(jsontype: ResourceType, repo_url: str, base_path: str) -> None:
+    # if the type wasn't imported add source info pointing at the root service template
+    source_info = jsontype.get("_sourceinfo")
+    if not source_info:
+        # not an import, type defined in main service template file
+        # or it's an import relative to the root, just include the root import because it will in turn import this import
+        jsontype["_sourceinfo"] = dict(url=sanitize_url(repo_url, False), file=base_path)
+    elif "url" not in source_info:
+        # it's an import relative to the root, set to the repo's url
+        source_info["url"] = sanitize_url(repo_url, False)
+
 # XXX outputs: only include "public" attributes?
 def node_type_to_graphql(
     topology: TopologySpec,
     type_definition: StatefulEntityType,
     types: ResourceTypesByName,
+    summary: bool = False,
 ) -> ResourceType:
     """
     type ResourceType {
       name: String!
       title: String
       extends: [ResourceType!]
       description: String
@@ -610,29 +658,29 @@
       details_url: String
       inputsSchema: JSON
       computedPropertiesSchema: JSON
       outputsSchema: JSON
       requirements: [RequirementConstraint!]
       implementations: [String]
       implementation_requirements: [String]
+      _sourceinfo: JSON
     }
     """
     custom_defs = topology.topology_template.custom_defs
+    typename = type_definition.type
     jsontype = ResourceType(
         GraphqlObject(
             dict(
-                name=type_definition.type,  # fully qualified name
+                name=typename,  # fully qualified name
                 title=type_definition.type.split(".")[-1],  # short, readable name
                 description=type_definition.get_value("description") or "",
             )
         )
     )
-    types[
-        type_definition.type
-    ] = jsontype  # set now to avoid circular reference via _get_extends
+    types[typename] = jsontype  # set now to avoid circular reference via _get_extends
     metadata = type_definition.get_value("metadata")
     inherited_metadata = type_definition.get_value("metadata", parent=True)
     visibility = "inherit"
     if inherited_metadata:
         if "badge" in inherited_metadata:
             jsontype["badge"] = inherited_metadata["badge"]
         if "icon" in inherited_metadata:
@@ -640,40 +688,61 @@
         if "details_url" in inherited_metadata:
             jsontype["details_url"] = inherited_metadata["details_url"]
     if metadata:
         if "title" in metadata:
             jsontype["title"] = metadata["title"]
         if metadata.get("internal"):
             visibility = "hidden"
+
+    if typename in custom_defs:
+        _source = custom_defs[typename].get("_source")
+        if isinstance(_source, dict):  # could be str or None
+            jsontype["_sourceinfo"] = _get_source_info(_source)
+
+    if type_definition.defs is None:
+        logger.warning("%s is missing type definition", type_definition.type)
+        return jsontype
+
+    extends: List[str] = []
+    # add ancestors classes to extends
+    _get_extends(topology, type_definition, extends, types)
+    if isinstance(type_definition, NodeType):
+        # add capabilities types to extends
+        for cap in type_definition.get_capability_typedefs():
+            _get_extends(topology, cap, extends, None)
+    jsontype["extends"] = extends
+
+    operations = set(
+        op.name
+        for op in EntityTemplate._create_interfaces(type_definition, None)
+        if op.interfacetype != "Mock"
+    )
+    jsontype["implementations"] = sorted(operations)
+    jsontype[
+        "implementation_requirements"
+    ] = type_definition.get_interface_requirements()
+
+    if summary:
+        return jsontype
+
     jsontype["visibility"] = visibility
 
     propertydefs = list(
         (p, is_property_user_visible(p))
         for p in type_definition.get_properties_def_objects()
     )
     jsontype["inputsSchema"] = tosca_type_to_jsonschema(
         custom_defs, (p[0] for p in propertydefs if p[1]), None
     )
     jsontype["computedPropertiesSchema"] = tosca_type_to_jsonschema(
         custom_defs, (p[0] for p in propertydefs if not p[1]), None
     )
 
-    extends: List[str] = []
-    # add ancestors classes to extends
-    _get_extends(topology, type_definition, extends, types)
-    jsontype["extends"] = extends
     if not type_definition.is_derived_from("tosca.nodes.Root"):
         return jsontype
-    if type_definition.defs is None:
-        logger.warning("%s is missing type definition", type_definition.type)
-        return jsontype
-
-    # add capabilities types to extends
-    for cap in type_definition.get_capability_typedefs():
-        _get_extends(topology, cap, extends, None)
 
     # treat each capability as a complex property
     add_capabilities_as_properties(
         jsontype["inputsSchema"]["properties"], type_definition, custom_defs
     )
     # XXX only include "public" attributes?
     attributedefs = (
@@ -692,24 +761,14 @@
             None,
             [
                 requirement_to_graphql(topology, req)
                 for req in type_definition.get_all_requirements()
             ],
         )
     )
-
-    operations = set(
-        op.name
-        for op in EntityTemplate._create_interfaces(type_definition, None)
-        if op.interfacetype != "Mock"
-    )
-    jsontype["implementations"] = sorted(operations)
-    jsontype[
-        "implementation_requirements"
-    ] = type_definition.get_interface_requirements()
     return jsontype
 
 
 def _make_typedef(
     typename: str, custom_defs: CustomDefs
 ) -> Optional[StatefulEntityType]:
     typedef = None
@@ -727,36 +786,37 @@
 def _update_root_type(jsontype: GraphqlObject, sub_map: SubstitutionMappings):
     "Modify a type representation so that it can be used with template with a nested topology."
 
     # don't display any properties set by the inner topology
     for name, value in sub_map.get_declared_properties().items():
         inputsSchema = jsontype["inputsSchema"]["properties"].get(name)
         if inputsSchema:
-            if is_value_computed(value):
+            if is_server_only_expression(value):
                 del jsontype["inputsSchema"]["properties"][name]
             else:
                 inputsSchema["default"] = value
         else:
             jsontype["computedPropertiesSchema"]["properties"].pop(name, None)
 
     # make optional any requirements that were set in the inner topology
     names = sub_map.get_declared_requirement_names()
-    for req in jsontype["requirements"]:
+    for req in jsontype.get("requirements", []):
         if req["name"] in names:
             req["min"] = 0
     # templates created with this type need to have the substitute directive
     jsontype["directives"] = ["substitute"]
 
 
-def to_graphql_nodetypes(spec: ToscaSpec, include_all=True) -> ResourceTypesByName:
+def to_graphql_nodetypes(spec: ToscaSpec, include_all: bool) -> ResourceTypesByName:
     # node types are readonly, so mapping doesn't need to be bijective
     types = cast(ResourceTypesByName, {})
     topology = spec.topology
     assert topology
     custom_defs = topology.topology_template.custom_defs
+    ExceptionCollector.collecting = True
     # create these ones first
     # XXX detect error later if these types are being used elsewhere
     for nested_topology in spec.nested_topologies:
         sub_map = nested_topology.topology_template.substitution_mappings
         if sub_map:
             typedef = sub_map.node_type
             if typedef:
@@ -838,15 +898,15 @@
     return typedef
 
 
 def template_properties_to_json(nodetemplate: NodeTemplate, visitor):
     # if they aren't only include ones with an explicity value
     for p in nodetemplate.get_properties_objects():
         computed = is_computed(p)
-        if computed and not _is_get_env_or_secret(p.value):
+        if computed and not _is_front_end_expression(p.value):
             # don't expose values that are expressions to the user
             value = None
         else:
             value = visitor.attribute_value_to_json(p, p.value)
         user_visible = is_property_user_visible(p)
         if user_visible:
             visitor.user_settable = True
@@ -865,53 +925,75 @@
 ) -> Optional[GraphqlObject]:
     name, req_dict = _get_req(req)
     # we need to call _get_explicit_relationship() to make sure all the requirements relationships are created
     # _get_explicit_relationship returns req_dict merged with its type definition
     req_dict, rel_template = nodespec.toscaEntityTemplate._get_explicit_relationship(
         name, req_dict
     )
-    if "constraint" in req_dict.get("metadata", {}):
-        # this happens when we import graphql json directly
-        reqconstraint = req_dict["metadata"]["constraint"]
+    if nodespec.type not in types:
+        typeobj = _node_typename_to_graphql(nodespec.type, nodespec.topology, types)
+        if not typeobj:
+            return None
     else:
-        reqconstraint = requirement_to_graphql(nodespec.topology, {name: req_dict})
+        typeobj = types[nodespec.type]
+
+    match = req_dict.get("node")
+    reqconstraint = reqconstaint_from_nodetemplate(nodespec, name, req_dict)
     if reqconstraint is None:
         return None
 
-    typeobj = types[nodespec.type]
     if "substitute" in typeobj.get("directives", []):
         # we've might have modified the type in _update_root_type()
         # and the tosca object won't know about that change so set it now
         for typeconstraint in typeobj["requirements"]:
             if name == typeconstraint["name"]:
                 reqconstraint["min"] = typeconstraint["min"]
 
     _annotate_requirement(
         reqconstraint, reqconstraint["resourceType"], nodespec.topology, types
     )
     reqjson = GraphqlObject(
         dict(constraint=reqconstraint, name=name, match=None, __typename="Requirement")
     )
-    if req_dict.get("node") and not _get_typedef(
-        req_dict["node"], nodespec.topology.topology_template.custom_defs
+    if match and not _get_typedef(
+        match, nodespec.topology.topology_template.custom_defs
     ):
         # it's not a type, assume it's a node template
         # (the node template name might not match a template if it is only defined in the deployment blueprints)
-        match = req_dict["node"]
         reqjson["match"] = match
     return reqjson
 
 
+def reqconstaint_from_nodetemplate(nodespec: EntitySpec, name: str, req_dict: dict):
+    if "constraint" in req_dict.get("metadata", {}):
+        # this happens when we import graphql json directly
+        reqconstraint = req_dict["metadata"]["constraint"]
+    else:
+        # "node" on a node template's requirement in TOSCA yaml is the node match so don't use as part of the constraint
+        # use the type's "node" (unless the requirement isn't defined on the type at all)
+        typeReqDef = nodespec.toscaEntityTemplate.type_definition.get_requirement_definition(name)
+        if typeReqDef:
+            # preserve node as "match" for _requirement_visibility
+            req_dict["match"] = req_dict.get("node")
+            if "node" in typeReqDef:
+                req_dict["node"] = typeReqDef["node"]
+            elif "capability" in req_dict:
+                req_dict.pop("node", None)
+            # else: empty typeReqDef, leave req_dict alone
+        reqconstraint = requirement_to_graphql(nodespec.topology, {name: req_dict})
+    return reqconstraint
+
+
 def _find_typename(
     nodetemplate: EntityTemplate,
     types: ResourceTypesByName,
 ) -> str:
     # XXX
     # if we substituting template, generate a new type
-    # json type for root of imported blueprint only include unfulfilled requirements 
+    # json type for root of imported blueprint only include unfulfilled requirements
     # and set defaults on properties set by the inner root
     return nodetemplate.type
 
 
 def nodetemplate_to_json(
     node_spec: EntitySpec,
     types: ResourceTypesByName,
@@ -1342,26 +1424,27 @@
     if last_commit_time:
         template["commitTime"] = js_timestamp(last_commit_time)
     return blueprint, template
 
 
 def _to_graphql(
     localEnv: LocalEnv,
+    root_url: str = "",
 ) -> Tuple[GraphqlDB, YamlManifest, GraphqlObject, ResourceTypesByName]:
     # set skip_validation because we want to be able to dump incomplete service templates
     manifest = localEnv.get_manifest(skip_validation=True, safe_mode=True)
     db = GraphqlDB({})
     spec = manifest.tosca
     assert spec
     tpl = spec.template.tpl
     assert spec.topology and tpl
     types_repo = tpl.get("repositories").get("types")
     if types_repo:  # only export types, avoid built-in repositories
         db["repositories"] = {"types": types_repo}
-    types = to_graphql_nodetypes(spec)
+    types = to_graphql_nodetypes(spec, bool(root_url))
     db["ResourceType"] = types
     db["ResourceTemplate"] = {}
     environment_instances = {}
     connection_types = cast(ResourceTypesByName, {})
     for node_spec in spec.topology.node_templates.values():
         toscaEntityTemplate = node_spec.toscaEntityTemplate
         t = nodetemplate_to_json(node_spec, types)
@@ -1405,14 +1488,23 @@
         dict(
             connections=connections,
             primary_provider=connections.get("primary_provider"),
             instances=environment_instances,
             repositories=manifest.context.get("repositories") or {},
         )
     )
+    assert manifest.repo
+    file_path = manifest.get_tosca_file_path()
+    if root_url:
+        # if include_all, assume this export is for another repository
+        # (see get_types in server.py)
+        for t in types.values():
+            add_root_source_info(t, root_url, file_path)
+        for t in connection_types.values():
+            add_root_source_info(t, root_url, file_path)
     return db, manifest, env, connection_types
 
 
 def _add_resources(
     db: GraphqlDB,
     relationships: Dict[str, List[GraphqlObject]],
     root: TopologyInstance,
@@ -1462,17 +1554,15 @@
         url = outputs["url"]
     else:
         # computed outputs might not be saved, so try to evaluate it now
         try:
             url = manifest.rootResource.attributes["outputs"].get("url")
         except UnfurlError as e:
             url = None  # this can be raised if the evaluation is unsafe
-            logger.warning(
-                f"export could not evaluate output 'url': {e}"
-            )
+            logger.warning(f"export could not evaluate output 'url': {e}")
 
     if url:
         deployment["url"] = url
     elif primary_resource and primary_resource.get("attributes"):
         for prop in primary_resource["attributes"]:
             if prop["name"] == "url":
                 deployment["url"] = prop["value"]
@@ -1519,16 +1609,16 @@
     _set_deployment_url(manifest, deployment, primary_resource)
     if primary_resource and primary_resource["title"] == primary_name:
         primary_resource["title"] = deployment["title"]
     db["Deployment"] = {name: deployment}
     return deployment
 
 
-def to_blueprint(localEnv: LocalEnv, existing: Optional[str] = None) -> GraphqlDB:
-    db, manifest, env, env_types = _to_graphql(localEnv)
+def to_blueprint(localEnv: LocalEnv, root_url: Optional[str] = None) -> GraphqlDB:
+    db, manifest, env, env_types = _to_graphql(localEnv, root_url or "")
     assert manifest.tosca
     blueprint, root_name = to_graphql_blueprint(manifest.tosca, db)
     deployment_blueprints = get_deployment_blueprints(
         manifest, blueprint, root_name, db
     )
     db["DeploymentTemplate"] = deployment_blueprints
     blueprint["deploymentTemplates"] = list(deployment_blueprints)
@@ -1567,14 +1657,26 @@
             if not jsontype.get("implementations") and jsontype.get("requirements"):
                 # hack: if we're a "compound" type that is just a sum of its requirement, add an implementation so it is included
                 jsontype["implementations"] = ["create"]
         elif jsontype.get("implementations"):
             jsontype["implementations"] = []
 
 
+def _node_typename_to_graphql(
+    reqtypename: str,
+    topology: TopologySpec,
+    types: ResourceTypesByName,
+) -> Optional[ResourceType]:
+    custom_defs = topology.topology_template.custom_defs
+    typedef = _make_typedef(reqtypename, custom_defs)
+    if typedef:
+        return node_type_to_graphql(topology, typedef, types)
+    return None
+
+
 def annotate_requirements(topology: TopologySpec, types: ResourceTypesByName) -> None:
     for jsontype in list(types.values()):  # _annotate_requirement() might modify types
         for req in jsontype.get("requirements") or []:
             _annotate_requirement(req, req["resourceType"], topology, types)
 
 
 def _annotate_requirement(
@@ -1582,19 +1684,16 @@
     reqtypename: str,
     topology: TopologySpec,
     types: ResourceTypesByName,
 ) -> None:
     # req is a RequirementConstraint dict
     reqtype = types.get(reqtypename)
     if not reqtype:
-        custom_defs = topology.topology_template.custom_defs
-        typedef = _make_typedef(reqtypename, custom_defs)
-        if typedef:
-            reqtype = node_type_to_graphql(topology, typedef, types)
-        else:
+        reqtype = _node_typename_to_graphql(reqtypename, topology, types)
+        if not reqtype:
             return
 
     if "node_filter" not in req:
         return
     node_filter = req["node_filter"]
     req_filters = node_filter.get("requirements")
     # node_filter properties might refer to properties that are only present on some subtypes
@@ -1706,16 +1805,20 @@
             blueprintdb, manifest, env, env_types = _to_graphql(localLocalEnv)
             env["name"] = name
             env["instances"].update(default_imported_instances)
             instances = localEnv.project.contexts[name].get("instances")
             env["instances"].update(_set_shared_instances(instances))
             environments[name] = env
             all_connection_types.update(env_types)
-        except Exception:
+        except Exception as err:
             logger.error("error exporting environment %s", name, exc_info=True)
+            details = "".join(
+                traceback.TracebackException.from_exception(err).format()
+            )
+            environments[name] = dict(error="Internal Error", details=details)  # type: ignore
 
     db["DeploymentEnvironment"] = environments
     if blueprintdb:
         # XXX re-enable this?
         # if blueprintdb.get("repositories", {}).get("types"):
         #     # don't include ResourceTypes if we are including a types repository
         #     db["ResourceType"] = all_connection_types
@@ -1873,15 +1976,15 @@
                 p = Property(
                     name,
                     value,
                     dict(type="any"),
                     instance.template.toscaEntityTemplate.custom_def,
                 )
             if p.schema.get("metadata", {}).get("visibility") != "hidden":
-                if is_sensitive(value) and _is_get_env_or_secret(p.value):
+                if is_sensitive(value) and _is_front_end_expression(p.value):
                     value = p.value
                 else:
                     value = attribute_value_to_json(p, value)
                 attrs.append(dict(name=p.name, value=value))
 
     for prop in instance.template.propertyDefs.values():
         if prop.default is not None and prop.name not in instance._properties:
```

### Comparing `unfurl-0.7.1/unfurl/tosca.py` & `unfurl-0.8.0/unfurl/tosca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) 2020 Adam Souzis
 # SPDX-License-Identifier: MIT
 """
 TOSCA implementation
 """
 import copy
 
+from toscaparser.elements.interfaces import OperationDef
+
 from .tosca_plugins import TOSCA_VERSION
 from .util import (
     UnfurlError,
     UnfurlValidationError,
     get_base_dir,
     check_class_registry,
     env_var_value,
@@ -248,28 +250,30 @@
 
     def _parse_template(
         self,
         path: Optional[str],
         inputs: Optional[Dict[str, Any]],
         toscaDef: Dict[str, Any],
         resolver,
+        fragment,
     ):
         # need to set a path for the import loader
         mode = os.getenv("UNFURL_VALIDATION_MODE")
         additionalProperties = False
         if mode is not None:
             additionalProperties = "additionalProperties" in mode
             ToscaTemplate.strict = "reqcheck" in mode
         EntityTemplate.additionalProperties = additionalProperties
         self.template = ToscaTemplate(
             path=path,
             parsed_params=inputs,
             yaml_dict_tpl=toscaDef,
             import_resolver=resolver,
             verify=False,  # we display the error messages ourselves so we don't need to verify here
+            fragment=fragment,
         )
         ExceptionCollector.collecting = True  # don't stop collecting validation errors
         ExceptionCollector.near = " while instantiating the spec"
         self.topology = TopologySpec(
             self.template.topology_template, self, None, inputs
         )
         self.load_imported_default_templates()
@@ -310,15 +314,16 @@
 
     def __init__(
         self,
         toscaDef: Union[ToscaTemplate, Dict[str, Any]],
         spec: Optional[Dict[str, Any]] = None,
         path: Optional[str] = None,
         resolver=None,
-        skip_validation=False,
+        skip_validation: bool = False,
+        fragment: str = "",
     ):
         self.discovered: Optional[CommentedMap] = None
         self.nested_discovered: Dict[str, dict] = {}
         self.nested_topologies: List["TopologySpec"] = []
         self._topology_templates: Dict[int, "TopologySpec"] = {}
         if spec:
             inputs = cast(Optional[Dict[str, Any]], spec.get("inputs"))
@@ -339,29 +344,29 @@
                 )
 
             if spec:
                 self.load_instances(toscaDef, spec)
 
             logger.info("Validating TOSCA template at %s", path)
             try:
-                self._parse_template(path, inputs, toscaDef, resolver)
+                self._parse_template(path, inputs, toscaDef, resolver, fragment)
             except:
                 if (
                     not ExceptionCollector.exceptionsCaught()
                     or not self.template
                     or not self.topology
                 ):
                     raise  # unexpected error
 
             # copy errors because self._patch() might clear them
             errorsSoFar = ExceptionCollector.exceptions[:]
             patched = self._patch(toscaDef, path, errorsSoFar)
             if patched:
                 # overlay and evaluate_imports modifies tosaDef in-place, try reparsing it
-                self._parse_template(path, inputs, toscaDef, resolver)
+                self._parse_template(path, inputs, toscaDef, resolver, fragment)
             else:  # restore previously errors
                 ExceptionCollector.exceptions[:0] = errorsSoFar
 
             if ExceptionCollector.exceptionsCaught():
                 message = "\n".join(
                     ExceptionCollector.getExceptionsReport(
                         full=(get_console_log_level() < logging.INFO)
@@ -383,14 +388,18 @@
 
     @property
     def base_dir(self) -> str:
         if self.template.path is None:
             return ""
         return get_base_dir(self.template.path)
 
+    @property
+    def fragment(self) -> str:
+        return self.template.fragment
+
     def _get_project_dir(self, home=False):
         # hacky
         if self.template and self.template.import_resolver:
             manifest = self.template.import_resolver.manifest
             if manifest.localEnv:
                 if home:
                     if manifest.localEnv.homeProject:
@@ -691,15 +700,15 @@
 
     def _resolve(self, key):
         """Make attributes available to expressions"""
         if key in ["name", "type", "uri", "groups", "policies"]:
             return getattr(self, key)
         raise KeyError(key)
 
-    def get_interfaces(self):
+    def get_interfaces(self) -> List[OperationDef]:
         return self.toscaEntityTemplate.interfaces
 
     @property
     def groups(self):
         if not self.spec:
             return
         for g in self.spec.groups.values():
@@ -988,19 +997,19 @@
             # get_relationship_templates() is a list of RelationshipTemplates that target the node
             rIds = {id(r.toscaEntityTemplate) for r in self._relationships}
             for r in self.toscaEntityTemplate.get_relationship_templates():
                 if id(r) not in rIds and r.capability:
                     self._relationships.append(RelationshipSpec(r, self.topology, self))
         return self._relationships
 
-    def get_capability_interfaces(self):
+    def get_capability_interfaces(self) -> List[OperationDef]:
         idefs = [r.get_interfaces() for r in self._get_relationship_specs()]
         return [i for elem in idefs for i in elem if i.name != "default"]
 
-    def get_requirement_interfaces(self):
+    def get_requirement_interfaces(self) -> List[OperationDef]:
         idefs = [r.get_interfaces() for r in self.requirements.values()]
         return [i for elem in idefs for i in elem if i.name != "default"]
 
     @property
     def capabilities(self) -> Dict[str, "CapabilitySpec"]:
         if self._capabilities is None:
             self._capabilities = {
@@ -1189,15 +1198,15 @@
     @property
     def artifacts(self):
         return self.parentNode.artifacts
 
     def get_uri(self):
         return self.parentNode.name + "~q~" + self.name
 
-    def get_interfaces(self):
+    def get_interfaces(self) -> List[OperationDef]:
         return self.relationship.get_interfaces() if self.relationship else []
 
     def get_nodefilter_properties(self):
         # XXX should merge type_tpl with entity_tpl
         return get_nodefilters(self.type_tpl, "properties")
 
     def get_nodefilter_requirements(self):
@@ -1230,15 +1239,15 @@
     def parent(self):
         return self.parentNode
 
     @property
     def artifacts(self):
         return self.parentNode.artifacts
 
-    def get_interfaces(self):
+    def get_interfaces(self) -> List[OperationDef]:
         # capabilities don't have their own interfaces
         return self.parentNode.get_interfaces()
 
     def get_uri(self):
         # capabilities aren't standalone templates
         # this is demanagled by getTemplate()
         return self.parentNode.name + "~c~" + self.name
@@ -1321,15 +1330,15 @@
         )
         copy.inputs = self.inputs.copy()
         return copy
 
     def get_node_template(self, name: str) -> Optional[NodeSpec]:
         return self.node_templates.get(name)
 
-    def get_interfaces(self):
+    def get_interfaces(self) -> List[OperationDef]:
         # doesn't have any interfaces
         return []
 
     def is_compatible_target(self, targetStr):
         if self.name == targetStr:
             return True
         return False
@@ -1577,17 +1586,19 @@
 
     def get_path(self, resolver=None) -> Optional[str]:
         return self.get_path_and_fragment(resolver)[0]
 
     def get_path_and_fragment(
         self, resolver=None
     ) -> Tuple[Optional[str], Optional[str]]:
-        if not resolver and self.spec:
+        if not resolver:
+            assert self.spec
             resolver = self.spec.template.import_resolver
 
+        assert resolver
         path, fragment = resolver.resolve_to_local_path(
             self.base_dir, self.file, self.toscaEntityTemplate.repository
         )
         return path, fragment
 
     def as_import_spec(self):
         return dict(file=self.file, repository=self.toscaEntityTemplate.repository)
```

### Comparing `unfurl-0.7.1/unfurl/tosca_plugins/googlecloud.yaml` & `unfurl-0.8.0/unfurl/tosca_plugins/googlecloud.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/tosca_plugins/k8s.yaml` & `unfurl-0.8.0/unfurl/tosca_plugins/k8s.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/tosca_plugins/localhost.yaml` & `unfurl-0.8.0/unfurl/tosca_plugins/localhost.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/tosca_plugins/tosca-ext.yaml` & `unfurl-0.8.0/unfurl/tosca_plugins/tosca-ext.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/unfurl-schema.json` & `unfurl-0.8.0/unfurl/unfurl-schema.json`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/util.py` & `unfurl-0.8.0/unfurl/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     Any,
     Dict,
     Generator,
     Iterable,
     List,
     MutableMapping,
     Optional,
+    Sequence,
     Set,
     Tuple,
     Union,
     Iterator,
     TYPE_CHECKING,
     cast,
 )
@@ -99,20 +100,22 @@
         return ""
 
 
 class UnfurlError(Exception):
     def __init__(
         self, message: object, saveStack: bool = False, log: bool = False
     ) -> None:
+        stackInfo = None
         if saveStack:
             (etype, value, traceback) = sys.exc_info()
             if value:
                 message = str(message) + ": " + str(value)
+                stackInfo = (etype, value, traceback)
         super().__init__(message)
-        self.stackInfo = (etype, value, traceback) if saveStack and value else None
+        self.stackInfo = stackInfo
         if log:
             logger.error(message, exc_info=True)
 
     def get_stack_trace(self) -> str:
         if not self.stackInfo:
             return ""
         return "".join(traceback.format_exception(*self.stackInfo))
@@ -623,14 +626,24 @@
     for i, x in enumerate(seq):
         if (i + 1) % 2 == 0:
             yield last, x
         else:
             last = x
 
 
+def unique_name(name: str, existing: Sequence) -> str:
+    counter = 1
+    basename = name
+    while name in existing:
+        # create Repository instance with a unique name
+        name = basename + str(counter)
+        counter += 1
+    return name
+
+
 def substitute_env(contents, env=None, preserve_missing=False):
     """
     Replace ${NAME} or ${NAME:default value} with the value of the environment variable $NAME
     Use \${NAME} to ignore
     """
     if env is None:
         env = os.environ
```

### Comparing `unfurl-0.7.1/unfurl/vendor/sphinx-jsonschema/__init__.py` & `unfurl-0.8.0/unfurl/vendor/sphinx-jsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/sphinx-jsonschema/wide_format.py` & `unfurl-0.8.0/unfurl/vendor/sphinx-jsonschema/wide_format.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/__init__.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/__init__.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/activities.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/activities.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/artifacts.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/artifacts.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/capabilities.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/capabilities.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/common/exception.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/common/exception.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/dataentity.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/dataentity.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_0.yaml` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_0.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_3.yaml` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_3.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/artifacttype.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/artifacttype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/attribute_definition.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/attribute_definition.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/capabilitytype.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/capabilitytype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/constraints.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/constraints.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/datatype.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/datatype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/entity_type.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/entity_type.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/grouptype.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/grouptype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/interfaces.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,14 +342,15 @@
         for op in list(defs):
             if op in INTERFACE_DEF_RESERVED_WORDS:
                 continue
             op_def = defs[op]
             if not isinstance(op_def, dict):
                 if op_def == "not_implemented":
                     continue
+                # if empty, copy the shared implementation
                 op_def = cls(implementation=op_def or implementation)
             elif implementation and not op_def.get('implementation'):
                 op_def['implementation'] = implementation
             if _source:
                 op_def['_source'] = _source
             iface = OperationDef(type_definition,
                                  interface_type,
```

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/nodetype.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/nodetype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/policytype.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/policytype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/portspectype.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/portspectype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/property_definition.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/property_definition.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/relationshiptype.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/relationshiptype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/scalarunit.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/scalarunit.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/statefulentitytype.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/statefulentitytype.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,18 @@
                 self.defs = self.TOSCA_DEF[entitytype]
             else:
                 self.defs = None
                 ExceptionCollector.appendException(
                     MissingTypeError(what=entitytype))
         self.type = entitytype
         self.custom_def = custom_def
-        self._source = self.defs and self.defs.get("_source") or None
+        source = self.defs and self.defs.get("_source") or None
+        if isinstance(source, dict):
+            source = source.get("path")
+        self._source = source
         self.__ancestors = None
         self._interfaces = None
         self._property_defs = None
         self._attribute_defs = None
         self._validate_interfaces()
 
     def ancestors(self):
```

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/elements/tosca_type_validation.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/elements/tosca_type_validation.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/entity_template.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/entity_template.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/exttools.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/exttools.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml` & `unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml` & `unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml` & `unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/functions.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/functions.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/groups.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/groups.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/imports.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/imports.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,20 +87,25 @@
         "repository",
         "namespace_uri",
         "namespace_prefix",
         "when",
     )
 
     def __init__(
-        self, importslist, path, type_definition_list=None, repositories=None, resolver=None
+        self, importslist, path, type_definition_list=None, repositories=None, resolver=None, repository_root=None,
     ):
         self.importslist = importslist
         self.custom_defs = {}
-        self.nested_tosca_tpls = []
+        self.nested_tosca_tpls = {}
         self.resolver = resolver or ImportResolver()
+        self.repository_root = None
+        if repository_root is not None:
+            if not is_url(normalize_path(repository_root)):
+                repository_root = get_base(repository_root)
+            self.repository_root = repository_root
         self.path = path
         self.repositories = repositories or {}
         # names of type definition sections
         self.type_definition_list = type_definition_list or []
         if importslist is not None:
             if not path:
                 msg = _("Input tosca template is not provided.")
@@ -137,54 +142,66 @@
                     import_name = None
                     import_def = import_tpl
 
             else:  # import_def is just the uri string
                 import_name = None
                 import_def = import_tpl
 
-            full_file_name, imported_tpl = self.load_yaml(import_def, import_name)
+            base, full_file_name, imported_tpl = self.load_yaml(import_def, import_name)
             if full_file_name is None:
                 return
 
             namespace_prefix = None
+            repository_name = None
             if isinstance(import_def, dict):
                 namespace_prefix = import_def.get(self.NAMESPACE_PREFIX)
+                repository_name = import_def.get(self.REPOSITORY)
+                file_name = import_def.get(self.FILE)
+            else:
+                file_name = import_def
+
             if imported_tpl:
                 TypeValidation(imported_tpl, import_tpl)
-                self._update_custom_def(imported_tpl, namespace_prefix, full_file_name)
-            # XXX should save prefix too
-            self._update_nested_tosca_tpls(full_file_name, imported_tpl)
+                self._update_custom_def(imported_tpl, namespace_prefix, full_file_name,
+                                        repository_name, base, file_name)
+            root_path = base if repository_name else self.repository_root
+            self._update_nested_tosca_tpls(full_file_name, root_path, imported_tpl, namespace_prefix)
 
-    def _update_custom_def(self, imported_tpl, namespace_prefix, path):
+    def _update_custom_def(self, imported_tpl, namespace_prefix, path, repository_name, base, file_name):
         path = os.path.normpath(path)
+        if repository_name:
+            root_path = self.resolver.get_repository_url(self, repository_name)
+        else:
+            root_path = self.repository_root
         for type_def_section in self.type_definition_list:
             outer_custom_types = imported_tpl.get(type_def_section)
             if outer_custom_types:
                 if type_def_section in [
                     "node_types",
                     "relationship_types",
                     "artifact_types",
                 ]:
                     for custom_def in outer_custom_types.values():
-                        custom_def["_source"] = path
+                        custom_def["_source"] = dict(path=path, prefix=namespace_prefix,
+                                                     root=root_path, repository=repository_name,
+                                                     base=base, file=file_name)
                 if namespace_prefix:
                     prefix_custom_types = {}
                     for type_def_key in outer_custom_types:
                         namespace_prefix_to_key = namespace_prefix + "." + type_def_key
                         prefix_custom_types[
                             namespace_prefix_to_key
                         ] = outer_custom_types[type_def_key]
                     self.custom_defs.update(prefix_custom_types)
                 else:
                     self.custom_defs.update(outer_custom_types)
 
-    def _update_nested_tosca_tpls(self, full_file_name, custom_tpl):
+    def _update_nested_tosca_tpls(self, full_file_name, root_path, custom_tpl, namespace_prefix):
         if full_file_name and custom_tpl:
-            topo_tpl = {full_file_name: custom_tpl}
-            self.nested_tosca_tpls.append(topo_tpl)
+            self.nested_tosca_tpls[full_file_name] = (custom_tpl, root_path, namespace_prefix)
 
     def _validate_import_keys(self, import_name, import_uri_def):
         if self.FILE not in import_uri_def.keys():
             log.warning(
                 'Missing keyname "file" in import "%(name)s".' % {"name": import_name}
             )
             ExceptionCollector.appendException(
@@ -204,25 +221,25 @@
                     )
                 )
 
     def load_yaml(self, import_uri_def, import_name=None):
         url_info = self.resolve_import(import_uri_def, import_name)
         if url_info is not None:
             try:
-                path, fragment, ctx = url_info
+                base, path, fragment, ctx = url_info
                 doc, ctx = self.resolver.load_yaml(path, fragment, ctx)
             except Exception as e:
                 msg = _('Import "%s" is not valid.') % path
                 url_exc = URLException(what=msg)
                 url_exc.__cause__ = e
                 ExceptionCollector.appendException(url_exc)
-                return None, None
-            return getattr(doc, "path", path), doc
+                return None, None, None
+            return base, getattr(doc, "path", path), doc
         else:
-            return None, None
+            return None, None, None
 
     def resolve_import(self, import_uri_def, import_name=None):
         """Handle custom types defined in imported template files
 
         This method loads the custom type definitions referenced in "imports"
         section of the TOSCA YAML template by determining whether each import
         is specified via a file reference (by relative or absolute path) or a
@@ -244,26 +261,28 @@
         file_name, sep, fragment = file_name.partition("#")
         path = normalize_path(file_name)
         doc_base = get_base(self.path)
         if repository_name:
             if is_url(path) or os.path.isabs(path):
                 msg = _(
                     'Absolute URL "%(name)s" cannot be used '
-                    'when a repository is specified ("%(repository)").'
+                    'when a repository is specified ("%(repository)s").'
                 ) % {"name": file_name, "repository": repository_name}
                 ExceptionCollector.appendException(ImportError(msg))
                 return None
 
             base = self.resolver.get_repository_url(self, repository_name)
             if base is None:  # couldn't resolve
                 return None
             if self.path and not is_url(base) and not os.path.isabs(base):
                 # repository is set to a relative local path
                 base = os.path.normpath(os.path.join(doc_base, base))
             path, ctx = self.resolver.resolve_url(self, base, os.path.normpath(path), repository_name)
+            if path is None:
+                return None
         else:
             base = ""
             if not is_url(path):
                 if os.path.isabs(path):
                     if self.path and is_url(self.path):
                         msg = _(
                             'Absolute file name "%(name)s" cannot be '
@@ -281,15 +300,17 @@
                             "in a pre-parsed input template."
                         ) % {"name": file_name}
                         ExceptionCollector.appendException(ImportError(msg))
                         return None
                     base = doc_base
                     # so join with the current location of import
             path, ctx = self.resolver.resolve_url(self, base, path, repository_name)
-        return path, fragment, ctx
+            if path is None:
+                return None
+        return base, path, fragment, ctx
 
     def _resolve_import_template(self, import_name, import_uri_def):
         if isinstance(import_uri_def, dict):
             self._validate_import_keys(import_name, import_uri_def)
             file_name = import_uri_def.get(self.FILE)
             repository = import_uri_def.get(self.REPOSITORY)
             repos = self.repositories.keys()
```

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/nodetemplate.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/nodetemplate.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/parameters.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/parameters.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/policy.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/policy.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/prereq/csar.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/prereq/csar.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,19 +175,18 @@
                     os.path.join(self.temp_dir, tpl_filename))
 
                 # Get list of nested templates
                 nested_tosca_tpls = custom_service.get_nested_tosca_tpls()
 
                 # Validate external references of each nested template.
                 if nested_tosca_tpls:
-                    for tosca_tpl in nested_tosca_tpls:
-                        for filename, tpl in tosca_tpl.items():
-                            self._validate_external_artifact_imports(
-                                tpl,
-                                filename)
+                    for filename, (tpl, repository_name, prefix) in nested_tosca_tpls.items():
+                        self._validate_external_artifact_imports(
+                            tpl,
+                            filename)
 
     def _validate_external_references(self, main_tpl):
         """Extracts files referenced in the main template
 
         These references are currently supported:
         * imports
         * interface implementations
```

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/properties.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/properties.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/relationship_template.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/relationship_template.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/repositories.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/repositories.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/reservation.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/reservation.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/shell.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/shell.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/steps.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/steps.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/substitution_mappings.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/substitution_mappings.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/topology_template.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/topology_template.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/tosca_template.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/tosca_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,20 +65,21 @@
                            'tosca_simple_yaml_1_2': SPECIAL_SECTIONS,
                            'tosca_simple_yaml_1_3': SPECIAL_SECTIONS}
 
     ADDITIONAL_SECTIONS.update(exttools.get_sections())
 
     '''Load the template data.'''
     def __init__(self, path=None, parsed_params=None, a_file=True,
-                 yaml_dict_tpl=None, import_resolver=None, verify=True):
+                 yaml_dict_tpl=None, import_resolver=None, verify=True, fragment=""):
 
         ExceptionCollector.start()
         self.a_file = a_file
         self.input_path = None
         self.path = None
+        self.fragment = fragment
         self.tpl = None
         self.import_resolver = import_resolver
         self.nested_tosca_tpls = {}
         self.nested_topologies = {}
         if path:
             self.input_path = path
             # don't validate or load if yaml_dict_tpl was set
@@ -179,53 +180,53 @@
         return self.topology_template.policies
 
     def get_type_sections(self):
         return [TYPES, NODE_TYPES, CAPABILITY_TYPES, RELATIONSHIP_TYPES,
                  DATA_TYPES, ARTIFACT_TYPES, INTERFACE_TYPES, POLICY_TYPES, GROUP_TYPES]
 
     def _get_all_custom_defs(self):
-        custom_defs, nested_tosca_tpls = self._get_custom_defs(self.tpl, self.path)
+        custom_defs, nested_tosca_tpls = self._get_custom_defs(self.tpl, self.path, self.path)
         self.nested_tosca_tpls = nested_tosca_tpls
         # Handle custom types defined in current template file
         for type_def in self.get_type_sections():
             inner_custom_types = self.tpl.get(type_def)
             if inner_custom_types:
                 custom_defs.update(inner_custom_types)
         return custom_defs
 
-    def _get_custom_defs(self, tpl, path):
+    def _get_custom_defs(self, tpl, path, root_path):
         custom_defs_final = {}
         tosca_tpls = {}
-        custom_defs, nested_imports = self.load_imports(path, tpl)
-        for imported in nested_imports:
-            filename, import_tpl = list(imported.items())[0]
-            tosca_tpls.update(imported)
-            import_defs, nested_tosca_tpls = self._get_custom_defs(import_tpl, filename)
+        custom_defs, nested_imports = self.load_imports(path, tpl, root_path)
+        for filename, (import_tpl, root_path, prefix) in nested_imports.items():
+            tosca_tpls[filename] = import_tpl
+            import_defs, nested_tosca_tpls = self._get_custom_defs(import_tpl, filename, root_path)
             custom_defs_final.update(import_defs)
             tosca_tpls.update(nested_tosca_tpls)
         if custom_defs:
             custom_defs_final.update(custom_defs)
         return custom_defs_final, tosca_tpls
 
-    def load_imports(self, path, tpl):
+    def load_imports(self, path, tpl, root_path):
         """Handle custom types defined in imported template files
 
         This method loads the custom type definitions referenced in "imports"
         section of the TOSCA YAML template.
         """
         imports = tpl.get("imports")
         if not imports:
             return {}, {}
 
         type_sections = self.get_type_sections()
         imports_loader = toscaparser.imports.ImportsLoader(
-            None, path, type_sections, self.tpl.get("repositories"), self.import_resolver
+            None, path, type_sections, self.tpl.get("repositories"),
+            self.import_resolver, root_path
         )
         imports_loader.resolver.load_imports(imports_loader, imports)
-        # nested_tosca_tpls is list of {file_path : tpl} of the imported templates
+        # nested_tosca_tpls is Dict[file_path, (tpl, repository_name, prefix)] of the imported templates
         nested_tosca_tpls = imports_loader.get_nested_tosca_tpls()
         # custom defs are merged together (with possibly namespace prefix)
         custom_defs = imports_loader.get_custom_defs()
         return custom_defs, nested_tosca_tpls
 
     def _handle_nested_tosca_templates_with_topology(self, custom_types):
         ExceptionCollector.near = ""
```

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/tpl_relationship_graph.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/tpl_relationship_graph.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/triggers.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/triggers.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/unsupportedtype.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/unsupportedtype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/utils/gettextutils.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/utils/gettextutils.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/utils/urlutils.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/utils/urlutils.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/utils/validateutils.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/utils/validateutils.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/utils/yamlparser.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/utils/yamlparser.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/vendor/toscaparser/workflow.py` & `unfurl-0.8.0/unfurl/vendor/toscaparser/workflow.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.7.1/unfurl/yamlloader.py` & `unfurl-0.8.0/unfurl/yamlloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,40 +27,42 @@
     filter_env,
     to_bytes,
     to_text,
     sensitive_str,
     sensitive_bytes,
     sensitive_dict,
     sensitive_list,
+    unique_name,
     wrap_sensitive_value,
     UnfurlError,
     UnfurlValidationError,
     find_schema_errors,
     get_base_dir,
 )
 from .merge import (
     expand_doc,
     make_map_with_base,
     find_anchor,
     _cache_anchors,
     restore_includes,
 )
-from .repo import Repo, RepoView, GitRepo, is_url_or_git_path, split_git_url
+from .repo import Repo, RepoView, add_user_to_url, split_git_url, memoized_remote_tags
 from .packages import UnfurlPackageUpdateNeeded, resolve_package
 from .logs import getLogger
 from toscaparser.common.exception import URLException, ExceptionCollector
 from toscaparser.utils.gettextutils import _
 import toscaparser.imports
 from toscaparser.repositories import Repository
 
 from ansible.parsing.vault import VaultLib, VaultSecret
 from ansible.parsing.yaml.objects import AnsibleMapping
 from ansible.parsing.yaml.loader import AnsibleLoader, AnsibleConstructor
 from ansible.utils.unsafe_proxy import AnsibleUnsafeText, AnsibleUnsafeBytes
 from time import perf_counter
+from jinja2.runtime import DebugUndefined
 
 logger = getLogger("unfurl")
 
 yaml_perf = 0.0
 
 CLEARTEXT_VAULT = VaultLib(secrets=[("cleartext", b"")])
 
@@ -89,17 +91,14 @@
 
 
 def _use_clear_text(vault):
     clear_id = CLEARTEXT_VAULT.secrets[0][0]
     return vault.secrets and all(s[0] == clear_id for s in vault.secrets)
 
 
-from jinja2.runtime import DebugUndefined
-
-
 def represent_undefined(dumper, data):
     msg = f"cannot represent an object: <{data}> of type {type(data)}"
     if isinstance(data, DebugUndefined):
         return dumper.represent_scalar("tag:yaml.org,2002:str", repr(msg))
     else:
         raise RepresenterError(msg)
 
@@ -242,15 +241,16 @@
     return urllib.request.urlopen(
         url, context=ssl.create_default_context(cafile=certifi.where())
     )
 
 
 _refResolver = RefResolver("", None)
 
-GetURLType = Optional[Tuple[str, bool, Optional[str]]]
+# context for the resolved url or local path: is_file, repo_view, base url or path, file_name
+ImportResolver_Context = Tuple[bool, Optional[RepoView], str, str]
 
 
 class ImportResolver(toscaparser.imports.ImportResolver):
     # get_repository() is called by the tosca template
     # load_yaml() called by the ImportsLoader with the resolved path or url returned by resolve_file_reference()
 
     def __init__(
@@ -258,15 +258,14 @@
     ):
         self.manifest = manifest
         self.readonly = bool(manifest.localEnv and manifest.localEnv.readonly)
         self.ignoreFileNotFound = ignoreFileNotFound
         self.yamlloader = manifest.loader
         self.expand = expand
         self.config = config or {}
-        self.repo_refs: Dict[str, GitRepo] = {}
 
     def __getstate__(self):
         state = self.__dict__.copy()
         state["yamlloader"] = None
         return state
 
     def load_imports(
@@ -277,24 +276,19 @@
         while True:
             try:
                 return super().load_imports(importsLoader, importslist)
             except UnfurlPackageUpdateNeeded:
                 pass  # reload
 
     def get_repository(self, name: str, tpl: dict, unique=False) -> Repository:
-        counter = 1
-        basename = name
-        while name in self.manifest.repositories:
-            if unique:
-                # create Repository instance with a unique name
-                name = basename + str(counter)
-                counter += 1
-            else:
-                # don't create another Repository instance
-                return self.manifest.repositories[name].repository
+        if not unique and name in self.manifest.repositories:
+            # don't create another Repository instance
+            return self.manifest.repositories[name].repository
+        else:
+            name = unique_name(name, list(self.manifest.repositories))
 
         if isinstance(tpl, dict) and "url" in tpl:
             url = tpl["url"]
             if (
                 "://" not in url and "@" in url
             ):  # scp style used by git: user@server:project.git
                 # convert to ssh://user@server/project.git
@@ -317,25 +311,37 @@
                     credential, context.get("variables")
                 )
 
         return Repository(name, tpl)
 
     confine_user_paths = True
 
-    def _has_path_escaped(self, path, repository_name=None):
+    def _has_path_escaped(self, path, repository_name=None, base=None):
         if not self.confine_user_paths:
             return False
         if repository_name:
-            if path.startswith("..") or os.path.isabs(path):
+            if os.path.normpath(path).startswith("..") or os.path.isabs(path):
                 msg = f'Path not allowed outside of repository {repository_name}: "{path}"'
                 ExceptionCollector.appendException(ImportError(msg))
                 return True
             else:
                 return False
 
+        if base:
+            # relative to file
+            absbase = os.path.abspath(base)
+            if not absbase[-1] != "/":
+                absbase += "/"
+            if not os.path.abspath(path).startswith(absbase):
+                msg = f'Path not allowed outside of repository or document root "{absbase}": "{path}"'
+                ExceptionCollector.appendException(ImportError(msg))
+                return True
+            else:
+                return False
+
         # user supplied path can't be outside of the project or the home project
         if self.manifest.localEnv and self.manifest.localEnv.project:
             if os.path.abspath(path).startswith(
                 os.path.abspath(os.path.dirname(__file__))
             ):
                 # special case for built-in "unfurl" repository
                 return False
@@ -348,15 +354,14 @@
                 ):
                     msg = f'Path "{os.path.abspath(path)}" not allowed outside of project: "{self.manifest.localEnv.project.projectRoot}"'
                     ExceptionCollector.appendException(ImportError(msg))
                     return True
         return False
 
     def _find_repoview(self, url: str) -> RepoView:
-        # if create, creates a new one
         repo_view = None
         git_url, path, revision = split_git_url(url)  # we only support git urls
         assert self.manifest.localEnv
         repoview_or_url = self.manifest.localEnv._find_git_repo(git_url, revision)
         if isinstance(repoview_or_url, RepoView):
             repo_view = repoview_or_url
         else:
@@ -371,14 +376,15 @@
         self,
         repo_view: RepoView,
         base: str,
         file_name: str,
     ) -> str:
         commit = repo_view.package.lock_to_commit if repo_view.package else ""
         if not repo_view.repo:
+            # calls LocalEnv.find_or_create_working_dir()
             repo, file_path, revision, bare = self.manifest.find_repo_from_git_url(
                 repo_view.as_git_url(), base
             )
             if repo:
                 repo_view.repo = repo
             else:
                 raise UnfurlError(
@@ -394,15 +400,43 @@
             path = self._get_bare_path(repo, file_path, revision)
         else:
             path = os.path.join(repo.working_dir, file_path, file_name or "").rstrip(
                 "/"
             )
         return path
 
-    def resolve_url(self, importsLoader, base, file_name, repository_name):
+    def get_remote_tags(self, url, pattern="*") -> List[str]:
+        # apply credentials to url like find_repo_from_git_url() does
+        if self.manifest.repo:
+            candidate_parts = urlsplit(self.manifest.repo.url)
+            password = candidate_parts.password
+        else:
+            password = ""
+            candidate_parts = None
+        if password:
+            url_parts = urlsplit(url)
+            assert candidate_parts
+            if (
+                candidate_parts.hostname == url_parts.hostname
+                and candidate_parts.port == url_parts.port
+            ):
+                # rewrite url to add credentials
+                url = add_user_to_url(
+                    url, candidate_parts.username, password
+                )
+        return memoized_remote_tags(url, pattern="*")
+
+    def resolve_url(
+        self,
+        importsLoader: toscaparser.imports.ImportsLoader,
+        base: str,
+        file_name: str,
+        repository_name: Optional[str],
+    ) -> Tuple[Optional[str], Optional[ImportResolver_Context]]:
+        # resolve to an url or absolute path along with context
         if repository_name:
             if self._has_path_escaped(file_name, repository_name):
                 # can't be ".." or absolute path
                 return None, None
             repo_view = self.manifest.repositories.get(repository_name)
             if not repo_view:
                 repository = self.get_repository(
@@ -410,41 +444,55 @@
                 )
                 repo_view = self.manifest.add_repository(None, repository, "")
         else:
             # if file_name is relative, base will be set (to the importsLoader's path)
             url = os.path.join(base, file_name)
             if not toscaparser.imports.is_url(url):
                 # url is a local path
-                if self._has_path_escaped(url):
+                repository_root = None  # default to checking if its in the project
+                if importsLoader.repository_root:
+                    if toscaparser.imports.is_url(importsLoader.repository_root):
+                        # just make sure we didn't break out of the base
+                        repository_root = base
+                    else:
+                        repository_root = importsLoader.repository_root
+                if self._has_path_escaped(url, base=repository_root):
                     return None, None
                 return url, (True, None, base, file_name)
             repo_view = self._find_repoview(url)
             assert repo_view
 
         assert repo_view
         if repo_view.package is None:
             # need to resolve if its a package
             # if repoview.repository references a package, set the repository's url
             # and register this reference with the package
             # might raise error if version conflict
             resolve_package(
-                repo_view, self.manifest.packages, self.manifest.package_specs
+                repo_view,
+                self.manifest.packages,
+                self.manifest.package_specs,
+                self.get_remote_tags,
             )
         repo_view.add_file_ref(file_name)
         path = toscaparser.imports.normalize_path(repo_view.url)
         is_file = not toscaparser.imports.is_url(path)
         if is_file:
             # repository is a local path
             # so use the resolved base
             path = os.path.join(base, file_name)
             if self._has_path_escaped(path):
                 return None, None
         return path, (is_file, repo_view, base, file_name)
 
-    def resolve_to_local_path(self, base_dir, file_name, repository_name):
+    def resolve_to_local_path(
+        self, base_dir, file_name, repository_name
+    ) -> Tuple[Optional[str], Optional[str]]:
+        # this should only be called during deploy time when an operation needs direct access to directories in the repository
+        # (see ArtifactSpec.get_path_and_fragment)
         if repository_name:
             rv = self.manifest.repositories.get(repository_name)
             if rv:
                 repository_tpl = rv.repository.tpl
                 repositories = {repository_name: repository_tpl}
             else:
                 repositories = (
@@ -456,37 +504,48 @@
             repositories = {}
         loader = toscaparser.imports.ImportsLoader(
             None, base_dir, repositories=repositories, resolver=self
         )
         tpl = dict(file=file_name, repository=repository_name)
         url_info = loader.resolve_import(tpl)
         if url_info:
-            url, fragment, ctx = url_info
-            is_file, repo_view, base, file_name = ctx
+            base, url, fragment, ctx = url_info
+            is_file, repo_view, base, file_name = cast(ImportResolver_Context, ctx)
             if is_file:
                 # already a path
                 return url, fragment
             else:
                 # clone git repository if necessary
-                return self._resolve_repo_to_path(repo_view, base, file_name), fragment
+                assert repo_view  # if url must
+                return (
+                    self._really_resolve_to_local_path(repo_view, base, file_name),
+                    fragment,
+                )
         return None, None
 
+    def _really_resolve_to_local_path(
+        self,
+        repo_view: RepoView,
+        base: str,
+        file_name: str,
+    ) -> str:
+        return self._resolve_repo_to_path(repo_view, base, file_name)
+
     def _get_bare_path(self, repo, filePath, revision):
         # # XXX support empty filePath or when filePath is a directory -- need to checkout the tree
         path = repo.working_dir
         if not filePath:
             raise UnfurlError(
                 f"local repository for '{path}' can not checkout revision '{revision}'"
             )
         elif repo.repo.rev_parse(revision + ":" + filePath).type != "blob":
             raise UnfurlError(
                 f"can't retrieve '{filePath}' with revision '{revision}' from local repository for '{path}'"
             )
         url = "git-ref:" + repo.url
-        # self.repo_refs[url] = repo
         return f"{url}#{revision}:{filePath}"
 
     def _open(self, path: str, isFile: bool) -> Tuple[Optional[TextIO], bool]:
         ok_to_show = True
         if path.startswith("git-ref:"):
             # XXX we need both the commit and revision if we don't have the full git repo
             url, filePath, revision = split_git_url(path[len("git-ref:") :])
@@ -541,19 +600,21 @@
                 else:
                     raise
 
     def load_yaml(
         self,
         path: str,
         fragment: Optional[str],
-        ctx,
-    ) -> Tuple[Any, Any]:
+        ctx: ImportResolver_Context,
+    ) -> Tuple[Any, bool]:
+        # ctx is set by self.resolve_url()
         is_file, repo_view, base, file_name = ctx
         if not is_file:
             # clone git repository if necessary
+            assert repo_view  # urls must have a repo_view
             path = self._resolve_repo_to_path(repo_view, base, file_name)
             is_file = True
         return self._really_load_yaml(path, is_file, fragment)
 
     def _really_load_yaml(
         self,
         path: str,
@@ -571,14 +632,16 @@
 
             with f:
                 contents = f.read()
                 doc = load_yaml(yaml, contents, path, self.readonly)
                 yaml_dict = yaml_dict_type(self.readonly)
                 if isinstance(doc, yaml_dict):
                     if self.expand:
+                        # XXX doc won't have a loadTemplate attribute set so document includes aren't support here
+                        # to support relative includes in a file in a repository, the repository root would have to be passed to the load include hook
                         includes, doc = expand_doc(
                             doc,
                             cls=make_map_with_base(doc, get_base_dir(path), yaml_dict),
                         )
                         doc.includes = includes
                     doc.path = path
             if fragment and doc:
@@ -603,20 +666,21 @@
             self.manifest.cache[doc_key] = (val, count + 1)
             return val
         return None
 
     def load_yaml(
         self,
         path: str,
-        fragment,
-        ctx,
-    ) -> Tuple[Any, Any]:
+        fragment: Optional[str],
+        ctx: ImportResolver_Context,
+    ) -> Tuple[Any, bool]:
         is_file, repo_view, base, file_name = ctx
         if not is_file:
             # clone git repository if necessary
+            assert repo_view  # urls must have a repo_view
             path = self._resolve_repo_to_path(repo_view, base, file_name)
         doc = self.get_cache((path, fragment))
         if doc is None:
             doc, cacheable = self._really_load_yaml(path, True, fragment)
             if cacheable:
                 self.set_cache((path, fragment), doc)
         else:
```

### Comparing `unfurl-0.7.1/unfurl/yamlmanifest.py` & `unfurl-0.8.0/unfurl/yamlmanifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from collections.abc import MutableSequence, Mapping
 import numbers
 import os
 import os.path
 import itertools
 
 from . import DefaultNames
-from .util import UnfurlError, to_yaml_text, filter_env
+from .util import UnfurlError, get_base_dir, to_yaml_text, filter_env
 from .merge import patch_dict, intersect_dict
 from .yamlloader import YamlConfig, make_yaml
 from .result import serialize_value
 from .support import ResourceChanges, Defaults, Status
 from .localenv import LocalEnv
 from .lock import Lock
 from .manifest import Manifest, relabel_dict, ChangeRecordRecord
@@ -211,17 +211,18 @@
         if localEnv:
             self.context = localEnv.get_context(self.context)
         inputs = spec.get("inputs") or {}
         context_inputs = self.context.get("inputs")
         if context_inputs:
             inputs.update(context_inputs)
         spec["inputs"] = inputs
-        lock = manifest.get("lock")
-        if lock:
-            Lock.apply_to_packages(lock, self.package_specs)
+        # XXX fix when lock_to_commit is enabled
+        # lock = manifest.get("lock")
+        # if lock:
+        #     Lock.apply_to_packages(lock, self.package_specs)
         # _update_repositories might not have been called while parsing
         # call it now to make sure we set up the built-in repositories
         self._update_repositories(manifest)
 
     @property
     def uris(self) -> List[str]:
         uris: List[str] = []
@@ -248,15 +249,18 @@
         return self.manifest.config.setdefault("metadata", CommentedMap())
 
     @property
     def yaml(self):
         return self.manifest.yaml
 
     def get_base_dir(self):
-        return self.manifest.get_base_dir()
+        if self.path:
+            return get_base_dir(self.path)
+        else:
+            return "."
 
     def is_path_to_self(self, path):
         if self.path is None or path is None:
             return False
         return os.path.abspath(self.path) == os.path.abspath(path)
 
     def get_saved_outputs(self):
@@ -326,15 +330,15 @@
                 k: v.copy()
                 for k, v in self.context["instances"].items()
                 if "imported" not in v
             }
             self._load_resource_templates(
                 env_instances, spec.setdefault("instances", {}), True
             )
-        self._set_spec(spec, more_spec, skip_validation)
+        self._set_spec(spec, more_spec, skip_validation, "spec")
         assert self.tosca
         if self.localEnv:
             msg = f'Loading ensemble "{self.path}" in environment "{self.localEnv.manifest_context_name}"'
             if self.tosca.topology and self.tosca.topology.primary_provider:
                 msg += f' with a primary_provider of type "{self.tosca.topology.primary_provider.type}"'
             logger.info(msg)
 
@@ -622,14 +626,26 @@
             # unlink first to avoid race (this will fail on Windows)
             os.unlink(self.lockfilepath)
             self.lockfile.close()
             self.lockfile = None
             return True
         return False
 
+    def get_tosca_file_path(self) -> str:
+        if not self.tosca:
+            return ""
+        assert self.tosca.template
+        if self.repo:
+            file_path = self.repo.find_path(self.tosca.template.path or "")[0] or ""
+        else:
+            file_path = self.tosca.template.path or ""
+        if self.tosca.fragment:
+            return file_path + "#" + self.tosca.fragment
+        return file_path
+
     def find_last_operation(self, target, operation) -> Optional[ChangeRecordRecord]:
         if self._operationIndex is None:
             operationIndex: Dict[Tuple[str, str], str] = {}
             if self.changeSets:
                 # add list() for 3.7
                 for change in reversed(list(self.changeSets.values())):
                     if not change.target or not change.operation:
```

### Comparing `unfurl-0.7.1/unfurl.egg-info/PKG-INFO` & `unfurl-0.8.0/unfurl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: unfurl
-Version: 0.7.1
+Version: 0.8.0
 Summary: use Git to record and deploy changes to your DevOps infrastructure
 Home-page: https://github.com/onecommons/unfurl
 Author: Adam Souzis
 Author-email: adam@onecommons.org
 License: MIT
+Project-URL: Homepage, https://www.unfurl.cloud
+Project-URL: Documentation, https://docs.unfurl.run
+Project-URL: Repository, https://github.com/onecommons/unfurl
+Project-URL: Changelog, https://github.com/onecommons/unfurl/blob/main/CHANGELOG.md
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
-Metadata-Version: 2.1 Name: unfurl Version: 0.7.1 Summary: use Git to record
+Metadata-Version: 2.1 Name: unfurl Version: 0.8.0 Summary: use Git to record
 and deploy changes to your DevOps infrastructure Home-page: https://github.com/
 onecommons/unfurl Author: Adam Souzis Author-email: adam@onecommons.org
-License: MIT Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-Provides-Extra: full Provides-Extra: server Provides-Extra: test License-File:
-LICENSE
+License: MIT Project-URL: Homepage, https://www.unfurl.cloud Project-URL:
+Documentation, https://docs.unfurl.run Project-URL: Repository, https://
+github.com/onecommons/unfurl Project-URL: Changelog, https://github.com/
+onecommons/unfurl/blob/main/CHANGELOG.md Platform: UNKNOWN Classifier:
+Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
+Intended Audience :: Developers Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown Provides-Extra: full Provides-Extra:
+server Provides-Extra: test License-File: LICENSE
                [https://docs.unfurl.run/_images/unfurl_logo.svg]
                                 [PyPI_version]
 # Introduction Unfurl is a command line tool for managing your DevOps
 infrastructure. Unfurl lets you easily track configuration, secrets, software
 and code dependencies, and deployment history all in git. Unfurl can integrate
 with the DevOps tools you are already using -- like Terraform, Ansible, and
 Helm -- allowing you to encapsulate your DevOps processes into reusable
```

### Comparing `unfurl-0.7.1/unfurl.egg-info/SOURCES.txt` & `unfurl-0.8.0/unfurl.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -51,14 +51,21 @@
 unfurl/configurators/helm-template.yaml
 unfurl/configurators/k8s.py
 unfurl/configurators/kompose.py
 unfurl/configurators/shell.py
 unfurl/configurators/supervisor-template.yaml
 unfurl/configurators/supervisor.py
 unfurl/configurators/terraform.py
+unfurl/configurators/k8s_ansible/__init__.py
+unfurl/configurators/k8s_ansible/apply.py
+unfurl/configurators/k8s_ansible/args_common.py
+unfurl/configurators/k8s_ansible/exceptions.py
+unfurl/configurators/k8s_ansible/k8sdynamicclient.py
+unfurl/configurators/k8s_ansible/client/discovery.py
+unfurl/configurators/k8s_ansible/client/resource.py
 unfurl/filter_plugins/__init__.py
 unfurl/filter_plugins/ref.py
 unfurl/lookup_plugins/__init__.py
 unfurl/lookup_plugins/unfurl.py
 unfurl/templates/gitignore.j2
 unfurl/templates/local-unfurl-template.yaml.j2
 unfurl/templates/manifest-template.yaml.j2
```

### Comparing `unfurl-0.7.1/unfurl.egg-info/requires.txt` & `unfurl-0.8.0/unfurl.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,67 @@
 MarkupSafe<=2.1.1
 PyYAML>=6.0
-ansible<5.0,>=4.2.0
 certifi
 charset-normalizer==2.1.1
-click-log
-click>=8.0.1
+click<8.1.4,>=8.0.1
 cliff==3.10.1
 cryptography==38.0.3
 flask-caching<=2.0.1
 flask<=2.1.3
 flask_cors==3.0.10
 itsdangerous==2.0.1
 jinja2<=3.1.2
 jsonschema[format_nongpl]==3.2
 pbr==5.9.0
-pipenv==2022.1.8
+pipenv==2023.7.3
 python-dateutil>=2.8
+python-gitlab==3.13.0
 requests>=2.28
 rich==12.4.4
 ruamel.yaml==0.17.21
 stevedore==3.5.0
 typing_extensions==4.1.1
 uvicorn<=0.18.2
 
 [:(python_version<'3')]
 pyrsistent==0.15.7
 
-[:(python_version<'3.7')]
-GitPython==3.1.20
-
 [:(python_version<'3.8')]
+ansible-core==2.11.12
 importlib-metadata<=4.12.0
 
 [:(python_version>='3.7')]
 GitPython==3.1.30
 
+[:(python_version>='3.8')]
+ansible-core==2.12.10
+
 [full]
-boto
 boto3
 docker[tls]
 google-auth
 google-cloud-compute==1.3.2
 google-cloud-dns==0.34.0
 gunicorn==20.1.0
 octodns==0.9.14
 openshift
-python-gitlab<=3.4.0
 redis==4.3.5
 supervisor
 
 [server]
 gunicorn==20.1.0
 redis==4.3.5
 
 [test]
 boto3==1.21.46
 botocore==1.24.46
 coverage
 jinja2==3.1.2
 moto[server]==3.1.4
-mypy==0.950
+mypy==1.4.1
 pytest
 pytest-cov
 pytest-profiling
 pytest-xdist[psutil]
 types-six==1.16.15
 werkzeug==2.2.3
```

