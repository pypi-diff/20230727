# Comparing `tmp/port_ocean-0.1.2rc2.tar.gz` & `tmp/port_ocean-0.1.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.2rc2.tar", max compression
+gzip compressed data, was "port_ocean-0.1.2rc3.tar", max compression
```

## Comparing `port_ocean-0.1.2rc2.tar` & `port_ocean-0.1.2rc3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0    11357 2023-07-26 19:07:52.321389 port_ocean-0.1.2rc2/LICENSE
--rw-r--r--   0        0        0     4639 2023-07-26 19:07:52.321389 port_ocean-0.1.2rc2/README.md
--rw-r--r--   0        0        0      270 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/__init__.py
--rw-r--r--   0        0        0      328 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cli.py
--rw-r--r--   0        0        0      278 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/__init__.py
--rw-r--r--   0        0        0     1134 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/list_integrations.py
--rw-r--r--   0        0        0     1057 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/main.py
--rw-r--r--   0        0        0     1710 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/new.py
--rw-r--r--   0        0        0     2306 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/pull.py
--rw-r--r--   0        0        0     1537 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/sail.py
--rw-r--r--   0        0        0      536 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/version.py
--rw-r--r--   0        0        0      429 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       42 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2698 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0       12 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
--rw-r--r--   0        0        0      388 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
--rw-r--r--   0        0        0      292 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      449 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1680 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      655 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0       12 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
--rw-r--r--   0        0        0      898 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
--rw-r--r--   0        0        0       65 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
--rw-r--r--   0        0        0     1669 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1920 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0       54 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2563 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2309 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     2928 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/blueprints.py
--rw-r--r--   0        0        0     5623 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3909 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      781 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2701 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/config/base.py
--rw-r--r--   0        0        0     1259 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/config/dynamic.py
--rw-r--r--   0        0        0     1133 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     4147 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/context/event.py
--rw-r--r--   0        0        0     4286 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/base.py
--rw-r--r--   0        0        0      607 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/__init__.py
--rw-r--r--   0        0        0      554 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/base.py
--rw-r--r--   0        0        0     2555 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/factory.py
--rw-r--r--   0        0        0     1165 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/http/event_listener.py
--rw-r--r--   0        0        0     3128 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/kafka/event_listener.py
--rw-r--r--   0        0        0     1867 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/polling/event_listener.py
--rw-r--r--   0        0        0     2799 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/polling/utils.py
--rw-r--r--   0        0        0      716 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/__init__.py
--rw-r--r--   0        0        0      869 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/base.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/__init__.py
--rw-r--r--   0        0        0     7977 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/applier.py
--rw-r--r--   0        0        0     1339 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
--rw-r--r--   0        0        0      988 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     1392 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entity_processor/__init__.py
--rw-r--r--   0        0        0      955 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entity_processor/base.py
--rw-r--r--   0        0        0     2685 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      396 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1810 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     1912 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      698 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2569 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0    11843 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0     1683 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/utils.py
--rw-r--r--   0        0        0     1368 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/models.py
--rw-r--r--   0        0        0      781 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/ocean_types.py
--rw-r--r--   0        0        0     1957 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      532 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      407 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/port_defaults.py
--rw-r--r--   0        0        0      554 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2475 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/middlewares.py
--rw-r--r--   0        0        0     2266 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/ocean.py
--rw-r--r--   0        0        0     7164 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/port_defaults.py
--rw-r--r--   0        0        0        0 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/py.typed
--rw-r--r--   0        0        0     2837 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/run.py
--rw-r--r--   0        0        0     1007 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/utils.py
--rw-r--r--   0        0        0     3461 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/pyproject.toml
--rw-r--r--   0        0        0     6359 1970-01-01 00:00:00.000000 port_ocean-0.1.2rc2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 19:43:37.416559 port_ocean-0.1.2rc3/LICENSE
+-rw-r--r--   0        0        0     4639 2023-07-26 19:43:37.416559 port_ocean-0.1.2rc3/README.md
+-rw-r--r--   0        0        0      270 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/__init__.py
+-rw-r--r--   0        0        0      328 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0      278 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1134 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/list_integrations.py
+-rw-r--r--   0        0        0     1057 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/main.py
+-rw-r--r--   0        0        0     1710 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/new.py
+-rw-r--r--   0        0        0     2306 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/pull.py
+-rw-r--r--   0        0        0     1537 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/sail.py
+-rw-r--r--   0        0        0      536 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/version.py
+-rw-r--r--   0        0        0      429 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       42 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0       12 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
+-rw-r--r--   0        0        0      388 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
+-rw-r--r--   0        0        0      292 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      449 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1680 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      655 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       12 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
+-rw-r--r--   0        0        0      898 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
+-rw-r--r--   0        0        0       65 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1920 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2563 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2309 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     2928 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/blueprints.py
+-rw-r--r--   0        0        0     5623 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3909 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      781 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     2701 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1259 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/config/dynamic.py
+-rw-r--r--   0        0        0     1197 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     4147 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4286 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/base.py
+-rw-r--r--   0        0        0      607 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/__init__.py
+-rw-r--r--   0        0        0      580 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/base.py
+-rw-r--r--   0        0        0     2555 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/factory.py
+-rw-r--r--   0        0        0     1165 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/http/event_listener.py
+-rw-r--r--   0        0        0     3128 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/kafka/event_listener.py
+-rw-r--r--   0        0        0     1867 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/polling/event_listener.py
+-rw-r--r--   0        0        0     2799 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/polling/utils.py
+-rw-r--r--   0        0        0      716 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/__init__.py
+-rw-r--r--   0        0        0      869 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/base.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/__init__.py
+-rw-r--r--   0        0        0     7977 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/applier.py
+-rw-r--r--   0        0        0     1339 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
+-rw-r--r--   0        0        0      988 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     1392 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entity_processor/__init__.py
+-rw-r--r--   0        0        0      955 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entity_processor/base.py
+-rw-r--r--   0        0        0     2685 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1810 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     1912 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      698 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2569 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0    11843 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0     1683 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/utils.py
+-rw-r--r--   0        0        0     1368 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/models.py
+-rw-r--r--   0        0        0      781 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/ocean_types.py
+-rw-r--r--   0        0        0     1957 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      532 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      407 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/port_defaults.py
+-rw-r--r--   0        0        0      554 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2475 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     2266 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/ocean.py
+-rw-r--r--   0        0        0     7164 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/port_defaults.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/py.typed
+-rw-r--r--   0        0        0     2837 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/run.py
+-rw-r--r--   0        0        0     1007 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/utils.py
+-rw-r--r--   0        0        0     3461 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/pyproject.toml
+-rw-r--r--   0        0        0     6359 1970-01-01 00:00:00.000000 port_ocean-0.1.2rc3/PKG-INFO
```

### Comparing `port_ocean-0.1.2rc2/LICENSE` & `port_ocean-0.1.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/README.md` & `port_ocean-0.1.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/cli/commands/list_integrations.py` & `port_ocean-0.1.2rc3/port_ocean/cli/commands/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/cli/commands/main.py` & `port_ocean-0.1.2rc3/port_ocean/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/cli/commands/new.py` & `port_ocean-0.1.2rc3/port_ocean/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/cli/commands/pull.py` & `port_ocean-0.1.2rc3/port_ocean/cli/commands/pull.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/cli/commands/sail.py` & `port_ocean-0.1.2rc3/port_ocean/cli/commands/sail.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/cli/commands/version.py` & `port_ocean-0.1.2rc3/port_ocean/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md` & `port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml` & `port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py` & `port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.2rc3/port_ocean/clients/port/authentication.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/clients/port/client.py` & `port_ocean-0.1.2rc3/port_ocean/clients/port/client.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/blueprints.py` & `port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/blueprints.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/clients/port/types.py` & `port_ocean-0.1.2rc3/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/clients/port/utils.py` & `port_ocean-0.1.2rc3/port_ocean/clients/port/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/config/base.py` & `port_ocean-0.1.2rc3/port_ocean/config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/config/dynamic.py` & `port_ocean-0.1.2rc3/port_ocean/config/dynamic.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/config/integration.py` & `port_ocean-0.1.2rc3/port_ocean/config/integration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Literal
 
-from pydantic import BaseSettings, BaseModel
+from pydantic import BaseSettings, BaseModel, Extra
 
 from port_ocean.config.base import BaseOceanSettings
 from port_ocean.core.event_listener import EventListenerSettingsType
 
 
-class PortSettings(BaseModel):
+class PortSettings(BaseModel, extra=Extra.allow):
     client_id: str
     client_secret: str
     base_url: str = "https://api.getport.io"
 
 
-class IntegrationSettings(BaseModel):
+class IntegrationSettings(BaseModel, extra=Extra.allow):
     identifier: str
     type: str
     config: dict[str, Any]
 
 
-class IntegrationConfiguration(BaseOceanSettings):
+class IntegrationConfiguration(BaseOceanSettings, extra=Extra.allow):
     port: PortSettings
     event_listener: EventListenerSettingsType
     batch_work_size: int = 20
     initialize_port_resources: bool = False
     integration: IntegrationSettings
 
     class Config:
```

### Comparing `port_ocean-0.1.2rc2/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.2rc3/port_ocean/consumers/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/context/event.py` & `port_ocean-0.1.2rc3/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/context/ocean.py` & `port_ocean-0.1.2rc3/port_ocean/context/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/event_listener/__init__.py` & `port_ocean-0.1.2rc3/port_ocean/core/event_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/event_listener/base.py` & `port_ocean-0.1.2rc3/port_ocean/core/event_listener/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import abstractmethod
 from typing import TypedDict, Callable, Any, Awaitable
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Extra
 
 
 class EventListenerEvents(TypedDict):
     on_resync: Callable[[dict[Any, Any]], Awaitable[None]]
 
 
 class BaseEventListener:
@@ -16,12 +16,12 @@
         self.events = events
 
     @abstractmethod
     async def start(self) -> None:
         pass
 
 
-class EventListenerSettings(BaseModel):
+class EventListenerSettings(BaseModel, extra=Extra.allow):
     type: str
 
     def to_request(self) -> dict[str, Any]:
         return {"type": self.type}
```

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/event_listener/factory.py` & `port_ocean-0.1.2rc3/port_ocean/core/event_listener/factory.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/event_listener/http/event_listener.py` & `port_ocean-0.1.2rc3/port_ocean/core/event_listener/http/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/event_listener/kafka/event_listener.py` & `port_ocean-0.1.2rc3/port_ocean/core/event_listener/kafka/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/event_listener/polling/event_listener.py` & `port_ocean-0.1.2rc3/port_ocean/core/event_listener/polling/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/event_listener/polling/utils.py` & `port_ocean-0.1.2rc3/port_ocean/core/event_listener/polling/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/handlers/__init__.py` & `port_ocean-0.1.2rc3/port_ocean/core/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/base.py` & `port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/applier.py` & `port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/applier.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py` & `port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py` & `port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py` & `port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/handlers/entity_processor/base.py` & `port_ocean-0.1.2rc3/port_ocean/core/handlers/entity_processor/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/handlers/entity_processor/jq_entity_processor.py` & `port_ocean-0.1.2rc3/port_ocean/core/handlers/entity_processor/jq_entity_processor.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.2rc3/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.2rc3/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/integrations/base.py` & `port_ocean-0.1.2rc3/port_ocean/core/integrations/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/sync.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/utils.py` & `port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/models.py` & `port_ocean-0.1.2rc3/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/ocean_types.py` & `port_ocean-0.1.2rc3/port_ocean/core/ocean_types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/core/utils.py` & `port_ocean-0.1.2rc3/port_ocean/core/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/exceptions/core.py` & `port_ocean-0.1.2rc3/port_ocean/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/logger_setup.py` & `port_ocean-0.1.2rc3/port_ocean/logger_setup.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/middlewares.py` & `port_ocean-0.1.2rc3/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/ocean.py` & `port_ocean-0.1.2rc3/port_ocean/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/port_defaults.py` & `port_ocean-0.1.2rc3/port_ocean/port_defaults.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/run.py` & `port_ocean-0.1.2rc3/port_ocean/run.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/port_ocean/utils.py` & `port_ocean-0.1.2rc3/port_ocean/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc2/pyproject.toml` & `port_ocean-0.1.2rc3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.2rc2"
+version = "0.1.2rc3"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 homepage = "https://app.getport.io"
 repository = "https://github.com/port-labs/Port-Ocean"
 
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
```

### Comparing `port_ocean-0.1.2rc2/PKG-INFO` & `port_ocean-0.1.2rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.2rc2
+Version: 0.1.2rc3
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Home-page: https://app.getport.io
 Keywords: ocean,port-ocean,port
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: FastAPI
```

