# Comparing `tmp/devapps-2023.6.20.tar.gz` & `tmp/devapps-2023.7.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devapps-2023.6.20.tar", max compression
+gzip compressed data, was "devapps-2023.7.27.tar", max compression
```

## Comparing `devapps-2023.6.20.tar` & `devapps-2023.7.27.tar`

### file list

```diff
@@ -1,148 +1,150 @@
--rw-r--r--   0        0        0     1323 2022-05-05 20:54:49.110883 devapps-2023.6.20/LICENSE
--rw-r--r--   0        0        0      992 2023-06-20 14:21:54.336663 devapps-2023.6.20/README.md
--rw-r--r--   0        0        0     5914 2023-06-20 14:21:38.025659 devapps-2023.6.20/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-22 14:30:25.715938 devapps-2023.6.20/src/ax/utils/__init__.py
--rw-r--r--   0        0        0       28 2023-03-22 14:30:25.715938 devapps-2023.6.20/src/ax/utils/ax_tree/__init__.py
--rwxr-xr-x   0        0        0    88440 2023-03-22 14:30:25.716939 devapps-2023.6.20/src/ax/utils/ax_tree/_ax_tree.so
--rw-r--r--   0        0        0    10033 2023-03-22 14:30:25.716939 devapps-2023.6.20/src/ax/utils/ax_tree/ax_tree.py
--rwxr-xr-x   0        0        0      491 2023-05-17 15:36:04.919861 devapps-2023.6.20/src/devapp/__init__.py
--rwxr-xr-x   0        0        0    19220 2023-05-17 15:36:04.919861 devapps-2023.6.20/src/devapp/app.py
--rwxr-xr-x   0        0        0        0 2023-05-17 15:36:04.919861 devapps-2023.6.20/src/devapp/app_token/__init__.py
--rwxr-xr-x   0        0        0     1201 2023-05-17 15:36:04.920861 devapps-2023.6.20/src/devapp/app_token/create_tokens.py
--rwxr-xr-x   0        0        0     2230 2023-05-17 15:36:04.920861 devapps-2023.6.20/src/devapp/app_token/read_tokens.py
--rwxr-xr-x   0        0        0      151 2023-05-17 15:36:04.921861 devapps-2023.6.20/src/devapp/app_token/verify_token
--rwxr-xr-x   0        0        0      297 2023-05-17 15:36:04.921861 devapps-2023.6.20/src/devapp/components/__init__.py
--rwxr-xr-x   0        0        0     6980 2023-05-17 15:36:04.921861 devapps-2023.6.20/src/devapp/components/cloudfoundry.py
--rwxr-xr-x   0        0        0     5956 2023-05-17 15:36:04.922861 devapps-2023.6.20/src/devapp/components/gitlab.py
--rwxr-xr-x   0        0        0     4828 2023-05-17 15:36:04.922861 devapps-2023.6.20/src/devapp/components/gitlab_runner.py
--rwxr-xr-x   0        0        0      150 2023-05-17 15:36:04.922861 devapps-2023.6.20/src/devapp/da.py
--rwxr-xr-x   0        0        0     1321 2023-05-17 15:36:04.922861 devapps-2023.6.20/src/devapp/dev_mode.py
--rwxr-xr-x   0        0        0     1636 2023-05-17 15:36:04.923861 devapps-2023.6.20/src/devapp/gevent_patched.py
--rwxr-xr-x   0        0        0     1549 2023-05-17 15:36:04.923861 devapps-2023.6.20/src/devapp/layer.py
--rwxr-xr-x   0        0        0      188 2023-05-17 15:36:04.923861 devapps-2023.6.20/src/devapp/lib/README.md
--rwxr-xr-x   0        0        0        0 2023-05-17 15:36:04.923861 devapps-2023.6.20/src/devapp/lib/__init__.py
--rwxr-xr-x   0        0        0   123141 2023-05-17 15:36:04.924861 devapps-2023.6.20/src/devapp/lib/sh.py
--rwxr-xr-x   0        0        0     2343 2023-05-17 15:36:04.925861 devapps-2023.6.20/src/devapp/load.py
--rwxr-xr-x   0        0        0      655 2023-05-17 15:36:04.925861 devapps-2023.6.20/src/devapp/logo
--rwxr-xr-x   0        0        0     1671 2023-05-17 15:36:04.925861 devapps-2023.6.20/src/devapp/max.py
--rw-r--r--   0        0        0     1933 2023-05-17 15:36:04.925861 devapps-2023.6.20/src/devapp/operations/resources.py
--rwxr-xr-x   0        0        0     1551 2023-05-17 15:36:04.926861 devapps-2023.6.20/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py
--rwxr-xr-x   0        0        0     6445 2023-05-17 15:36:04.926861 devapps-2023.6.20/src/devapp/plugins/dev_devapp/repo_sym_links.py
--rw-r--r--   0        0        0     3090 2023-05-17 15:36:04.926861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resource_install.py
--rw-r--r--   0        0        0     4577 2023-05-17 15:36:04.926861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resource_run.py
--rw-r--r--   0        0        0     8983 2023-05-17 15:36:04.927861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resources.py.dis
--rw-r--r--   0        0        0      671 2023-05-17 15:36:04.927861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resources_list.py
--rw-r--r--   0        0        0      879 2023-05-17 15:36:04.927861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/wait_for_port.py
--rwxr-xr-x   0        0        0     8688 2023-05-17 15:36:04.927861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/container_build.py
--rwxr-xr-x   0        0        0    10257 2023-05-17 15:36:04.928861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/container_pull.py
--rwxr-xr-x   0        0        0    28013 2023-05-17 15:36:04.928861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/fs_build.py
--rwxr-xr-x   0        0        0    13318 2023-05-17 15:36:04.928861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py
--rwxr-xr-x   0        0        0     9232 2023-05-17 15:36:04.929861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py
--rwxr-xr-x   0        0        0    12668 2023-05-17 15:36:04.929861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py
--rwxr-xr-x   0        0        0     8750 2023-05-17 15:36:04.929861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/kubectl/__init__.py
--rwxr-xr-x   0        0        0     2975 2023-05-17 15:36:04.930861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/life_cycle.py
--rw-r--r--   0        0        0     1573 2023-05-17 15:36:04.930861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/log_view.py
--rwxr-xr-x   0        0        0     2140 2023-05-18 08:36:34.543057 devapps-2023.6.20/src/devapp/plugins/ops_devapp/pkgs.py
--rwxr-xr-x   0        0        0    12996 2023-05-31 11:31:49.834517 devapps-2023.6.20/src/devapp/plugins/ops_devapp/project/__init__.py
--rw-r--r--   0        0        0     9960 2023-05-17 15:36:04.930861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py
--rw-r--r--   0        0        0     4994 2023-05-17 15:36:04.931861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/run.py
--rwxr-xr-x   0        0        0     7865 2023-06-16 15:07:07.410741 devapps-2023.6.20/src/devapp/plugins/ops_devapp/system/__init__.py
--rw-r--r--   0        0        0     2649 2023-06-16 16:56:09.507836 devapps-2023.6.20/src/devapp/plugins/ops_devapp/system/templates/inst_base.sh
--rw-r--r--   0        0        0     2657 2023-06-16 16:00:30.337863 devapps-2023.6.20/src/devapp/plugins/ops_devapp/system/tools.py
--rwxr-xr-x   0        0        0    28235 2023-05-17 15:36:04.931861 devapps-2023.6.20/src/devapp/run.py
--rwxr-xr-x   0        0        0    25984 2023-05-17 15:36:04.931861 devapps-2023.6.20/src/devapp/spec/build.py
--rwxr-xr-x   0        0        0     2929 2023-05-17 15:36:04.932861 devapps-2023.6.20/src/devapp/spec/find_paths_in_fs_components.py
--rwxr-xr-x   0        0        0    16176 2023-05-17 15:36:04.932861 devapps-2023.6.20/src/devapp/spec/fs_components.py
--rwxr-xr-x   0        0        0     1715 2023-05-17 15:36:04.933861 devapps-2023.6.20/src/devapp/spec/links.py
--rwxr-xr-x   0        0        0     2481 2023-05-17 15:36:04.933861 devapps-2023.6.20/src/devapp/spec/os_tools.py
--rwxr-xr-x   0        0        0     7913 2023-05-17 15:36:04.933861 devapps-2023.6.20/src/devapp/spec/templ.py
--rwxr-xr-x   0        0        0     1600 2023-05-17 15:36:04.933861 devapps-2023.6.20/src/devapp/spec/templates/unit
--rwxr-xr-x   0        0        0     7586 2023-05-17 15:36:04.934861 devapps-2023.6.20/src/devapp/spec/tools.py
--rwxr-xr-x   0        0        0    30671 2023-05-17 15:36:04.934861 devapps-2023.6.20/src/devapp/t
--rw-r--r--   0        0        0     3559 2023-05-17 15:36:04.934861 devapps-2023.6.20/src/devapp/testing/auto_docs.py
--rw-r--r--   0        0        0      443 2023-05-17 15:36:04.935861 devapps-2023.6.20/src/devapp/tests/test_unit_devapp.py
--rwxr-xr-x   0        0        0    13808 2023-05-17 15:36:04.935861 devapps-2023.6.20/src/devapp/third/rpl
--rwxr-xr-x   0        0        0    50126 2023-06-16 15:44:29.254501 devapps-2023.6.20/src/devapp/tools/__init__.py
--rw-r--r--   0        0        0     4025 2023-05-17 15:36:04.936861 devapps-2023.6.20/src/devapp/tools/flag.py
--rw-r--r--   0        0        0      731 2023-05-17 15:36:04.936861 devapps-2023.6.20/src/devapp/tools/http.py
--rw-r--r--   0        0        0    35701 2023-05-17 15:36:04.936861 devapps-2023.6.20/src/devapp/tools/infra/__init__.py
--rw-r--r--   0        0        0    16618 2023-05-17 15:36:04.937861 devapps-2023.6.20/src/devapp/tools/infra/actions.py
--rw-r--r--   0        0        0     3089 2023-05-17 15:36:04.937861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/000:functions.sh
--rwxr-xr-x   0        0        0      375 2023-05-17 15:36:04.937861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/001:add_sudo_user.sh
--rwxr-xr-x   0        0        0     1521 2023-05-17 15:36:04.938861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh
--rwxr-xr-x   0        0        0      448 2023-05-17 15:36:04.938861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/100:docker.sh
--rwxr-xr-x   0        0        0      324 2023-05-17 15:36:04.938861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/200:tools.sh
--rwxr-xr-x   0        0        0      760 2023-05-17 15:36:04.938861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/300:dns.sh
--rwxr-xr-x   0        0        0     4375 2023-05-17 15:36:04.938861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/500:k3s.sh
--rwxr-xr-x   0        0        0      943 2023-05-17 15:36:04.939861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/501:kind.sh
--rwxr-xr-x   0        0        0    17210 2023-05-17 15:36:04.939861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/502:k3s.sh
--rw-r--r--   0        0        0      276 2023-05-17 15:36:04.939861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/510:label_workers.sh
--rwxr-xr-x   0        0        0      661 2023-05-17 15:36:04.940861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/600:longhorn.sh
--rw-r--r--   0        0        0     1737 2023-05-17 15:36:04.941861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh
--rw-r--r--   0        0        0    26850 2023-05-17 15:36:04.942861 devapps-2023.6.20/src/devapp/tools/old.py
--rw-r--r--   0        0        0     4415 2023-05-17 15:36:04.942861 devapps-2023.6.20/src/devapp/tools/plugin.py
--rw-r--r--   0        0        0    27729 2023-06-12 11:18:59.001038 devapps-2023.6.20/src/devapp/tools/resource.py
--rw-r--r--   0        0        0     1861 2023-05-17 15:36:04.942861 devapps-2023.6.20/src/devapp/tools/times.py
--rwxr-xr-x   0        0        0        0 2023-05-17 15:36:04.943861 devapps-2023.6.20/src/devapp/utils/__init__.py
--rwxr-xr-x   0        0        0    15787 2023-05-17 15:36:04.943861 devapps-2023.6.20/src/devapp/utils/os_.py
--rwxr-xr-x   0        0        0     1871 2023-05-17 15:36:04.943861 devapps-2023.6.20/src/devapp/utils/py_source_env.py
--rwxr-xr-x   0        0        0     9335 2023-05-17 15:36:04.944861 devapps-2023.6.20/src/devapp/utils/rx_tools.py
--rwxr-xr-x   0        0        0    11529 2023-05-17 15:36:04.944861 devapps-2023.6.20/src/devapp/utils/vault.py
--rwxr-xr-x   0        0        0     2134 2023-06-20 09:40:12.936499 devapps-2023.6.20/src/devapp/utils/watch_dog.py
--rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.734938 devapps-2023.6.20/src/mdvl/__init__.py
--rwxr-xr-x   0        0        0    20402 2023-05-02 08:41:56.784342 devapps-2023.6.20/src/mdvl/mdvl.py
--rwxr-xr-x   0        0        0     2317 2023-03-22 14:30:25.735939 devapps-2023.6.20/src/mdvl/tools.py
--rwxr-xr-x   0        0        0      519 2023-05-17 15:36:04.945861 devapps-2023.6.20/src/structlogging/__init__.py
--rwxr-xr-x   0        0        0     1559 2023-05-17 15:36:04.945861 devapps-2023.6.20/src/structlogging/adapters.py
--rwxr-xr-x   0        0        0       88 2023-05-17 15:36:04.946861 devapps-2023.6.20/src/structlogging/common.py
--rwxr-xr-x   0        0        0     5503 2023-05-17 15:36:04.946861 devapps-2023.6.20/src/structlogging/config.py
--rwxr-xr-x   0        0        0     1618 2023-05-17 15:36:04.946861 devapps-2023.6.20/src/structlogging/formatters.py
--rwxr-xr-x   0        0        0     2640 2023-05-17 15:36:04.946861 devapps-2023.6.20/src/structlogging/processors.py
--rwxr-xr-x   0        0        0     5472 2023-05-17 15:36:04.946861 devapps-2023.6.20/src/structlogging/renderers.py
--rwxr-xr-x   0        0        0    11172 2023-05-17 15:36:04.947861 devapps-2023.6.20/src/structlogging/sl.py
--rw-r--r--   0        0        0     4022 2023-05-17 15:36:04.947861 devapps-2023.6.20/src/structlogging/stacktrace.py
--rwxr-xr-x   0        0        0     1355 2023-05-17 15:36:04.947861 devapps-2023.6.20/src/structlogging/tests/test_structlogging.py
--rwxr-xr-x   0        0        0      886 2023-05-02 12:47:20.254964 devapps-2023.6.20/src/theming/__init__.py
--rwxr-xr-x   0        0        0    14865 2023-05-02 12:47:20.254964 devapps-2023.6.20/src/theming/absl_color_help.py
--rwxr-xr-x   0        0        0     4345 2023-05-02 12:47:20.255964 devapps-2023.6.20/src/theming/ansi2html.py
--rwxr-xr-x   0        0        0    11888 2023-05-02 12:47:20.255964 devapps-2023.6.20/src/theming/ansi2html.sh
--rwxr-xr-x   0        0        0     3030 2023-05-02 12:47:20.255964 devapps-2023.6.20/src/theming/ansistrm.py
--rwxr-xr-x   0        0        0    10066 2023-05-02 12:47:20.255964 devapps-2023.6.20/src/theming/ax_xml.py
--rwxr-xr-x   0        0        0    10495 2023-05-02 12:47:20.255964 devapps-2023.6.20/src/theming/camel_snake.py
--rwxr-xr-x   0        0        0     7517 2023-05-02 12:47:20.256964 devapps-2023.6.20/src/theming/charting.py
--rwxr-xr-x   0        0        0     3392 2023-05-02 12:47:20.256964 devapps-2023.6.20/src/theming/colorhilite.py
--rwxr-xr-x   0        0        0     1113 2023-05-02 12:47:20.256964 devapps-2023.6.20/src/theming/filesize/README.txt
--rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.256964 devapps-2023.6.20/src/theming/filesize/__init__.py
--rwxr-xr-x   0        0        0     2549 2023-05-02 12:47:20.256964 devapps-2023.6.20/src/theming/filesize/filesize.py
--rwxr-xr-x   0        0        0     3756 2023-05-02 12:47:20.257964 devapps-2023.6.20/src/theming/formatters.py
--rw-r--r--   0        0        0     3807 2023-05-02 12:47:20.257964 devapps-2023.6.20/src/theming/formatting/markdown.py
--rw-r--r--   0        0        0     1241 2023-05-02 12:47:20.257964 devapps-2023.6.20/src/theming/formatting/viz_sequence.py
--rwxr-xr-x   0        0        0     3410 2023-05-02 12:47:20.257964 devapps-2023.6.20/src/theming/html_tools.py
--rwxr-xr-x   0        0        0    11409 2023-05-02 12:47:20.257964 devapps-2023.6.20/src/theming/inflect.py
--rwxr-xr-x   0        0        0      460 2023-05-02 12:47:20.258964 devapps-2023.6.20/src/theming/msgs.py
--rwxr-xr-x   0        0        0     9864 2023-05-02 12:47:20.258964 devapps-2023.6.20/src/theming/pretty_print.py
--rwxr-xr-x   0        0        0    55699 2023-05-02 12:47:20.258964 devapps-2023.6.20/src/theming/tablepretty.py
--rwxr-xr-x   0        0        0    13998 2023-05-02 12:47:20.259964 devapps-2023.6.20/src/theming/term.py
--rwxr-xr-x   0        0        0     1468 2023-05-02 12:47:20.259964 devapps-2023.6.20/src/theming/term_struct_hilite.py
--rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.6.20/src/theming/test
--rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.6.20/src/theming/tests/__init__.py
--rwxr-xr-x   0        0        0     9454 2023-05-02 12:47:20.260964 devapps-2023.6.20/src/theming/tests/test_text_formatting.py
--rwxr-xr-x   0        0        0     1063 2023-05-02 12:47:20.260964 devapps-2023.6.20/src/theming/tracebacks.py
--rwxr-xr-x   0        0        0     3011 2023-05-02 12:47:20.260964 devapps-2023.6.20/src/theming/unicode_chars.py
--rwxr-xr-x   0        0        0    23138 2023-03-23 18:50:41.169018 devapps-2023.6.20/src/tree_builder/__init__.py
--rwxr-xr-x   0        0        0    19864 2023-03-23 18:50:41.169018 devapps-2023.6.20/src/tree_builder/arch/__init__.py.bak
--rwxr-xr-x   0        0        0     7762 2023-03-23 18:50:41.169018 devapps-2023.6.20/src/tree_builder/arch/links.py.bak
--rwxr-xr-x   0        0        0    11455 2023-03-23 18:50:41.169018 devapps-2023.6.20/src/tree_builder/arch/o.py
--rwxr-xr-x   0        0        0    19872 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/arch/old
--rwxr-xr-x   0        0        0    10911 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/arch/olinit
--rwxr-xr-x   0        0        0    11597 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/arch/oo
--rwxr-xr-x   0        0        0      154 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/arch/py2.py
--rwxr-xr-x   0        0        0     7968 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/arch/render.py.bak
--rwxr-xr-x   0        0        0     2078 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/chrome_reload.sh
--rwxr-xr-x   0        0        0     5502 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/delivery2.py
--rwxr-xr-x   0        0        0    10773 2023-03-23 18:50:41.171018 devapps-2023.6.20/src/tree_builder/links.py
--rwxr-xr-x   0        0        0      218 2023-03-23 18:50:41.171018 devapps-2023.6.20/src/tree_builder/py3.py
--rwxr-xr-x   0        0        0     8028 2023-03-23 18:50:41.171018 devapps-2023.6.20/src/tree_builder/render.py
--rwxr-xr-x   0        0        0       21 2023-03-23 18:50:41.171018 devapps-2023.6.20/src/tree_builder/version.py
--rw-r--r--   0        0        0     3129 2023-06-20 14:21:57.163617 devapps-2023.6.20/setup.py
--rw-r--r--   0        0        0     1805 2023-06-20 14:21:57.163899 devapps-2023.6.20/PKG-INFO
+-rw-r--r--   0        0        0     1323 2022-05-05 20:54:49.110883 devapps-2023.7.27/LICENSE
+-rw-r--r--   0        0        0      992 2023-07-27 08:43:52.594271 devapps-2023.7.27/README.md
+-rw-r--r--   0        0        0     5914 2023-07-27 08:43:35.511256 devapps-2023.7.27/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-22 14:30:25.715938 devapps-2023.7.27/src/ax/utils/__init__.py
+-rw-r--r--   0        0        0       28 2023-03-22 14:30:25.715938 devapps-2023.7.27/src/ax/utils/ax_tree/__init__.py
+-rwxr-xr-x   0        0        0    88440 2023-03-22 14:30:25.716939 devapps-2023.7.27/src/ax/utils/ax_tree/_ax_tree.so
+-rw-r--r--   0        0        0    10033 2023-03-22 14:30:25.716939 devapps-2023.7.27/src/ax/utils/ax_tree/ax_tree.py
+-rwxr-xr-x   0        0        0      491 2023-05-17 15:36:04.919861 devapps-2023.7.27/src/devapp/__init__.py
+-rwxr-xr-x   0        0        0    19182 2023-07-25 14:11:32.320292 devapps-2023.7.27/src/devapp/app.py
+-rwxr-xr-x   0        0        0        0 2023-05-17 15:36:04.919861 devapps-2023.7.27/src/devapp/app_token/__init__.py
+-rwxr-xr-x   0        0        0     1201 2023-05-17 15:36:04.920861 devapps-2023.7.27/src/devapp/app_token/create_tokens.py
+-rwxr-xr-x   0        0        0     2230 2023-05-17 15:36:04.920861 devapps-2023.7.27/src/devapp/app_token/read_tokens.py
+-rwxr-xr-x   0        0        0      151 2023-05-17 15:36:04.921861 devapps-2023.7.27/src/devapp/app_token/verify_token
+-rwxr-xr-x   0        0        0      297 2023-05-17 15:36:04.921861 devapps-2023.7.27/src/devapp/components/__init__.py
+-rwxr-xr-x   0        0        0     6980 2023-05-17 15:36:04.921861 devapps-2023.7.27/src/devapp/components/cloudfoundry.py
+-rwxr-xr-x   0        0        0     5956 2023-05-17 15:36:04.922861 devapps-2023.7.27/src/devapp/components/gitlab.py
+-rwxr-xr-x   0        0        0     4828 2023-05-17 15:36:04.922861 devapps-2023.7.27/src/devapp/components/gitlab_runner.py
+-rwxr-xr-x   0        0        0      150 2023-05-17 15:36:04.922861 devapps-2023.7.27/src/devapp/da.py
+-rwxr-xr-x   0        0        0     1321 2023-05-17 15:36:04.922861 devapps-2023.7.27/src/devapp/dev_mode.py
+-rwxr-xr-x   0        0        0     1636 2023-05-17 15:36:04.923861 devapps-2023.7.27/src/devapp/gevent_patched.py
+-rwxr-xr-x   0        0        0     1549 2023-05-17 15:36:04.923861 devapps-2023.7.27/src/devapp/layer.py
+-rwxr-xr-x   0        0        0      188 2023-05-17 15:36:04.923861 devapps-2023.7.27/src/devapp/lib/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-17 15:36:04.923861 devapps-2023.7.27/src/devapp/lib/__init__.py
+-rwxr-xr-x   0        0        0   123141 2023-05-17 15:36:04.924861 devapps-2023.7.27/src/devapp/lib/sh.py
+-rwxr-xr-x   0        0        0     2343 2023-05-17 15:36:04.925861 devapps-2023.7.27/src/devapp/load.py
+-rwxr-xr-x   0        0        0      655 2023-05-17 15:36:04.925861 devapps-2023.7.27/src/devapp/logo
+-rwxr-xr-x   0        0        0     1671 2023-05-17 15:36:04.925861 devapps-2023.7.27/src/devapp/max.py
+-rw-r--r--   0        0        0     2028 2023-07-27 08:42:51.567219 devapps-2023.7.27/src/devapp/operations/resources.py
+-rwxr-xr-x   0        0        0     3867 2023-07-19 22:50:13.730659 devapps-2023.7.27/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py
+-rwxr-xr-x   0        0        0     6445 2023-05-17 15:36:04.926861 devapps-2023.7.27/src/devapp/plugins/dev_devapp/repo_sym_links.py
+-rw-r--r--   0        0        0     3090 2023-05-17 15:36:04.926861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/arch/resource_install.py
+-rw-r--r--   0        0        0     4577 2023-05-17 15:36:04.926861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/arch/resource_run.py
+-rw-r--r--   0        0        0     8983 2023-05-17 15:36:04.927861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/arch/resources.py.dis
+-rw-r--r--   0        0        0      671 2023-05-17 15:36:04.927861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/arch/resources_list.py
+-rw-r--r--   0        0        0      879 2023-05-17 15:36:04.927861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/arch/wait_for_port.py
+-rwxr-xr-x   0        0        0     8688 2023-05-17 15:36:04.927861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/container_build.py
+-rwxr-xr-x   0        0        0    10257 2023-05-17 15:36:04.928861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/container_pull.py
+-rwxr-xr-x   0        0        0    28013 2023-05-17 15:36:04.928861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/fs_build.py
+-rwxr-xr-x   0        0        0    13318 2023-05-17 15:36:04.928861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py
+-rwxr-xr-x   0        0        0     9232 2023-05-17 15:36:04.929861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py
+-rwxr-xr-x   0        0        0    12668 2023-05-17 15:36:04.929861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py
+-rwxr-xr-x   0        0        0     8750 2023-05-17 15:36:04.929861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/kubectl/__init__.py
+-rwxr-xr-x   0        0        0     2975 2023-05-17 15:36:04.930861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/life_cycle.py
+-rw-r--r--   0        0        0     1573 2023-05-17 15:36:04.930861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/log_view.py
+-rwxr-xr-x   0        0        0     2140 2023-05-18 08:36:34.543057 devapps-2023.7.27/src/devapp/plugins/ops_devapp/pkgs.py
+-rwxr-xr-x   0        0        0    12851 2023-07-26 12:40:54.765479 devapps-2023.7.27/src/devapp/plugins/ops_devapp/project/__init__.py
+-rw-r--r--   0        0        0     9960 2023-05-17 15:36:04.930861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py
+-rw-r--r--   0        0        0     4994 2023-05-17 15:36:04.931861 devapps-2023.7.27/src/devapp/plugins/ops_devapp/run.py
+-rwxr-xr-x   0        0        0    10798 2023-07-25 14:41:16.886324 devapps-2023.7.27/src/devapp/plugins/ops_devapp/system/__init__.py
+-rw-r--r--   0        0        0     4577 2023-07-26 13:49:06.320980 devapps-2023.7.27/src/devapp/plugins/ops_devapp/system/templates/inst_base.sh
+-rw-r--r--   0        0        0     3823 2023-07-25 08:15:57.232745 devapps-2023.7.27/src/devapp/plugins/ops_devapp/system/tools.py
+-rwxr-xr-x   0        0        0    28235 2023-05-17 15:36:04.931861 devapps-2023.7.27/src/devapp/run.py
+-rwxr-xr-x   0        0        0    25984 2023-05-17 15:36:04.931861 devapps-2023.7.27/src/devapp/spec/build.py
+-rwxr-xr-x   0        0        0     2929 2023-05-17 15:36:04.932861 devapps-2023.7.27/src/devapp/spec/find_paths_in_fs_components.py
+-rwxr-xr-x   0        0        0    16176 2023-05-17 15:36:04.932861 devapps-2023.7.27/src/devapp/spec/fs_components.py
+-rwxr-xr-x   0        0        0     1715 2023-05-17 15:36:04.933861 devapps-2023.7.27/src/devapp/spec/links.py
+-rwxr-xr-x   0        0        0     2481 2023-05-17 15:36:04.933861 devapps-2023.7.27/src/devapp/spec/os_tools.py
+-rwxr-xr-x   0        0        0     7913 2023-05-17 15:36:04.933861 devapps-2023.7.27/src/devapp/spec/templ.py
+-rwxr-xr-x   0        0        0     1600 2023-05-17 15:36:04.933861 devapps-2023.7.27/src/devapp/spec/templates/unit
+-rwxr-xr-x   0        0        0     7586 2023-05-17 15:36:04.934861 devapps-2023.7.27/src/devapp/spec/tools.py
+-rwxr-xr-x   0        0        0    30671 2023-05-17 15:36:04.934861 devapps-2023.7.27/src/devapp/t
+-rw-r--r--   0        0        0     3559 2023-05-17 15:36:04.934861 devapps-2023.7.27/src/devapp/testing/auto_docs.py
+-rw-r--r--   0        0        0      443 2023-05-17 15:36:04.935861 devapps-2023.7.27/src/devapp/tests/test_unit_devapp.py
+-rwxr-xr-x   0        0        0    13808 2023-05-17 15:36:04.935861 devapps-2023.7.27/src/devapp/third/rpl
+-rwxr-xr-x   0        0        0    50126 2023-06-16 15:44:29.254501 devapps-2023.7.27/src/devapp/tools/__init__.py
+-rw-r--r--   0        0        0     2901 2023-07-20 01:05:43.626207 devapps-2023.7.27/src/devapp/tools/assets/tmux.conf
+-rw-r--r--   0        0        0     4025 2023-05-17 15:36:04.936861 devapps-2023.7.27/src/devapp/tools/flag.py
+-rw-r--r--   0        0        0      731 2023-05-17 15:36:04.936861 devapps-2023.7.27/src/devapp/tools/http.py
+-rw-r--r--   0        0        0    35701 2023-05-17 15:36:04.936861 devapps-2023.7.27/src/devapp/tools/infra/__init__.py
+-rw-r--r--   0        0        0    16618 2023-05-17 15:36:04.937861 devapps-2023.7.27/src/devapp/tools/infra/actions.py
+-rw-r--r--   0        0        0     3089 2023-05-17 15:36:04.937861 devapps-2023.7.27/src/devapp/tools/infra/playbooks/000:functions.sh
+-rwxr-xr-x   0        0        0      375 2023-05-17 15:36:04.937861 devapps-2023.7.27/src/devapp/tools/infra/playbooks/001:add_sudo_user.sh
+-rwxr-xr-x   0        0        0     1521 2023-05-17 15:36:04.938861 devapps-2023.7.27/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh
+-rwxr-xr-x   0        0        0      448 2023-05-17 15:36:04.938861 devapps-2023.7.27/src/devapp/tools/infra/playbooks/100:docker.sh
+-rwxr-xr-x   0        0        0      324 2023-05-17 15:36:04.938861 devapps-2023.7.27/src/devapp/tools/infra/playbooks/200:tools.sh
+-rwxr-xr-x   0        0        0      760 2023-05-17 15:36:04.938861 devapps-2023.7.27/src/devapp/tools/infra/playbooks/300:dns.sh
+-rwxr-xr-x   0        0        0     4375 2023-05-17 15:36:04.938861 devapps-2023.7.27/src/devapp/tools/infra/playbooks/500:k3s.sh
+-rwxr-xr-x   0        0        0      943 2023-05-17 15:36:04.939861 devapps-2023.7.27/src/devapp/tools/infra/playbooks/501:kind.sh
+-rwxr-xr-x   0        0        0    17210 2023-05-17 15:36:04.939861 devapps-2023.7.27/src/devapp/tools/infra/playbooks/502:k3s.sh
+-rw-r--r--   0        0        0      276 2023-05-17 15:36:04.939861 devapps-2023.7.27/src/devapp/tools/infra/playbooks/510:label_workers.sh
+-rwxr-xr-x   0        0        0      661 2023-05-17 15:36:04.940861 devapps-2023.7.27/src/devapp/tools/infra/playbooks/600:longhorn.sh
+-rw-r--r--   0        0        0     1737 2023-05-17 15:36:04.941861 devapps-2023.7.27/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh
+-rw-r--r--   0        0        0    26850 2023-05-17 15:36:04.942861 devapps-2023.7.27/src/devapp/tools/old.py
+-rw-r--r--   0        0        0     4415 2023-05-17 15:36:04.942861 devapps-2023.7.27/src/devapp/tools/plugin.py
+-rw-r--r--   0        0        0    27989 2023-07-17 23:09:55.497437 devapps-2023.7.27/src/devapp/tools/resource.py
+-rw-r--r--   0        0        0     1861 2023-05-17 15:36:04.942861 devapps-2023.7.27/src/devapp/tools/times.py
+-rw-r--r--   0        0        0     4592 2023-07-25 14:52:34.602736 devapps-2023.7.27/src/devapp/tools/tmux.py
+-rwxr-xr-x   0        0        0        0 2023-05-17 15:36:04.943861 devapps-2023.7.27/src/devapp/utils/__init__.py
+-rwxr-xr-x   0        0        0    15787 2023-05-17 15:36:04.943861 devapps-2023.7.27/src/devapp/utils/os_.py
+-rwxr-xr-x   0        0        0     1871 2023-05-17 15:36:04.943861 devapps-2023.7.27/src/devapp/utils/py_source_env.py
+-rwxr-xr-x   0        0        0     9335 2023-05-17 15:36:04.944861 devapps-2023.7.27/src/devapp/utils/rx_tools.py
+-rwxr-xr-x   0        0        0    11529 2023-05-17 15:36:04.944861 devapps-2023.7.27/src/devapp/utils/vault.py
+-rwxr-xr-x   0        0        0     2134 2023-06-20 09:40:12.936499 devapps-2023.7.27/src/devapp/utils/watch_dog.py
+-rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.734938 devapps-2023.7.27/src/mdvl/__init__.py
+-rwxr-xr-x   0        0        0    20402 2023-05-02 08:41:56.784342 devapps-2023.7.27/src/mdvl/mdvl.py
+-rwxr-xr-x   0        0        0     2317 2023-03-22 14:30:25.735939 devapps-2023.7.27/src/mdvl/tools.py
+-rwxr-xr-x   0        0        0      519 2023-05-17 15:36:04.945861 devapps-2023.7.27/src/structlogging/__init__.py
+-rwxr-xr-x   0        0        0     1559 2023-05-17 15:36:04.945861 devapps-2023.7.27/src/structlogging/adapters.py
+-rwxr-xr-x   0        0        0       88 2023-05-17 15:36:04.946861 devapps-2023.7.27/src/structlogging/common.py
+-rwxr-xr-x   0        0        0     5503 2023-05-17 15:36:04.946861 devapps-2023.7.27/src/structlogging/config.py
+-rwxr-xr-x   0        0        0     1618 2023-05-17 15:36:04.946861 devapps-2023.7.27/src/structlogging/formatters.py
+-rwxr-xr-x   0        0        0     2640 2023-05-17 15:36:04.946861 devapps-2023.7.27/src/structlogging/processors.py
+-rwxr-xr-x   0        0        0     5472 2023-05-17 15:36:04.946861 devapps-2023.7.27/src/structlogging/renderers.py
+-rwxr-xr-x   0        0        0    11172 2023-05-17 15:36:04.947861 devapps-2023.7.27/src/structlogging/sl.py
+-rw-r--r--   0        0        0     4022 2023-05-17 15:36:04.947861 devapps-2023.7.27/src/structlogging/stacktrace.py
+-rwxr-xr-x   0        0        0     1355 2023-05-17 15:36:04.947861 devapps-2023.7.27/src/structlogging/tests/test_structlogging.py
+-rwxr-xr-x   0        0        0      886 2023-05-02 12:47:20.254964 devapps-2023.7.27/src/theming/__init__.py
+-rwxr-xr-x   0        0        0    14865 2023-05-02 12:47:20.254964 devapps-2023.7.27/src/theming/absl_color_help.py
+-rwxr-xr-x   0        0        0     4345 2023-05-02 12:47:20.255964 devapps-2023.7.27/src/theming/ansi2html.py
+-rwxr-xr-x   0        0        0    11888 2023-05-02 12:47:20.255964 devapps-2023.7.27/src/theming/ansi2html.sh
+-rwxr-xr-x   0        0        0     3030 2023-05-02 12:47:20.255964 devapps-2023.7.27/src/theming/ansistrm.py
+-rwxr-xr-x   0        0        0    10066 2023-05-02 12:47:20.255964 devapps-2023.7.27/src/theming/ax_xml.py
+-rwxr-xr-x   0        0        0    10495 2023-05-02 12:47:20.255964 devapps-2023.7.27/src/theming/camel_snake.py
+-rwxr-xr-x   0        0        0     7517 2023-05-02 12:47:20.256964 devapps-2023.7.27/src/theming/charting.py
+-rwxr-xr-x   0        0        0     3392 2023-05-02 12:47:20.256964 devapps-2023.7.27/src/theming/colorhilite.py
+-rwxr-xr-x   0        0        0     1113 2023-05-02 12:47:20.256964 devapps-2023.7.27/src/theming/filesize/README.txt
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.256964 devapps-2023.7.27/src/theming/filesize/__init__.py
+-rwxr-xr-x   0        0        0     2549 2023-05-02 12:47:20.256964 devapps-2023.7.27/src/theming/filesize/filesize.py
+-rwxr-xr-x   0        0        0     3756 2023-05-02 12:47:20.257964 devapps-2023.7.27/src/theming/formatters.py
+-rw-r--r--   0        0        0     3807 2023-05-02 12:47:20.257964 devapps-2023.7.27/src/theming/formatting/markdown.py
+-rw-r--r--   0        0        0     1241 2023-05-02 12:47:20.257964 devapps-2023.7.27/src/theming/formatting/viz_sequence.py
+-rwxr-xr-x   0        0        0     3410 2023-05-02 12:47:20.257964 devapps-2023.7.27/src/theming/html_tools.py
+-rwxr-xr-x   0        0        0    11409 2023-05-02 12:47:20.257964 devapps-2023.7.27/src/theming/inflect.py
+-rwxr-xr-x   0        0        0      460 2023-05-02 12:47:20.258964 devapps-2023.7.27/src/theming/msgs.py
+-rwxr-xr-x   0        0        0     9864 2023-05-02 12:47:20.258964 devapps-2023.7.27/src/theming/pretty_print.py
+-rwxr-xr-x   0        0        0    55699 2023-05-02 12:47:20.258964 devapps-2023.7.27/src/theming/tablepretty.py
+-rwxr-xr-x   0        0        0    13998 2023-05-02 12:47:20.259964 devapps-2023.7.27/src/theming/term.py
+-rwxr-xr-x   0        0        0     1468 2023-05-02 12:47:20.259964 devapps-2023.7.27/src/theming/term_struct_hilite.py
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.7.27/src/theming/test
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.7.27/src/theming/tests/__init__.py
+-rwxr-xr-x   0        0        0     9454 2023-05-02 12:47:20.260964 devapps-2023.7.27/src/theming/tests/test_text_formatting.py
+-rwxr-xr-x   0        0        0     1063 2023-05-02 12:47:20.260964 devapps-2023.7.27/src/theming/tracebacks.py
+-rwxr-xr-x   0        0        0     3011 2023-05-02 12:47:20.260964 devapps-2023.7.27/src/theming/unicode_chars.py
+-rwxr-xr-x   0        0        0    23138 2023-03-23 18:50:41.169018 devapps-2023.7.27/src/tree_builder/__init__.py
+-rwxr-xr-x   0        0        0    19864 2023-03-23 18:50:41.169018 devapps-2023.7.27/src/tree_builder/arch/__init__.py.bak
+-rwxr-xr-x   0        0        0     7762 2023-03-23 18:50:41.169018 devapps-2023.7.27/src/tree_builder/arch/links.py.bak
+-rwxr-xr-x   0        0        0    11455 2023-03-23 18:50:41.169018 devapps-2023.7.27/src/tree_builder/arch/o.py
+-rwxr-xr-x   0        0        0    19872 2023-03-23 18:50:41.170018 devapps-2023.7.27/src/tree_builder/arch/old
+-rwxr-xr-x   0        0        0    10911 2023-03-23 18:50:41.170018 devapps-2023.7.27/src/tree_builder/arch/olinit
+-rwxr-xr-x   0        0        0    11597 2023-03-23 18:50:41.170018 devapps-2023.7.27/src/tree_builder/arch/oo
+-rwxr-xr-x   0        0        0      154 2023-03-23 18:50:41.170018 devapps-2023.7.27/src/tree_builder/arch/py2.py
+-rwxr-xr-x   0        0        0     7968 2023-03-23 18:50:41.170018 devapps-2023.7.27/src/tree_builder/arch/render.py.bak
+-rwxr-xr-x   0        0        0     2078 2023-03-23 18:50:41.170018 devapps-2023.7.27/src/tree_builder/chrome_reload.sh
+-rwxr-xr-x   0        0        0     5502 2023-03-23 18:50:41.170018 devapps-2023.7.27/src/tree_builder/delivery2.py
+-rwxr-xr-x   0        0        0    10773 2023-03-23 18:50:41.171018 devapps-2023.7.27/src/tree_builder/links.py
+-rwxr-xr-x   0        0        0      218 2023-03-23 18:50:41.171018 devapps-2023.7.27/src/tree_builder/py3.py
+-rwxr-xr-x   0        0        0     8028 2023-03-23 18:50:41.171018 devapps-2023.7.27/src/tree_builder/render.py
+-rwxr-xr-x   0        0        0       21 2023-03-23 18:50:41.171018 devapps-2023.7.27/src/tree_builder/version.py
+-rw-r--r--   0        0        0     3160 2023-07-27 08:43:55.124260 devapps-2023.7.27/setup.py
+-rw-r--r--   0        0        0     1805 2023-07-27 08:43:55.124540 devapps-2023.7.27/PKG-INFO
```

### Comparing `devapps-2023.6.20/LICENSE` & `devapps-2023.7.27/LICENSE`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/README.md` & `devapps-2023.7.27/README.md`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/pyproject.toml` & `devapps-2023.7.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "devapps"
-version = "2023.06.20"
+version = "2023.07.27"
 description = "Apps - End to End."
 authors = ["Gunther Klessinger <g_kle_ss_ing_er@gmx.de>"]
 license = "BSD"
 readme = "README.md"
 repository = "https://github.com/AXGKl/devapps"
 homepage = "https://axgkl.github.io/devapps"
 keywords = []
```

### Comparing `devapps-2023.6.20/src/ax/utils/ax_tree/_ax_tree.so` & `devapps-2023.7.27/src/ax/utils/ax_tree/_ax_tree.so`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/ax/utils/ax_tree/ax_tree.py` & `devapps-2023.7.27/src/ax/utils/ax_tree/ax_tree.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/app.py` & `devapps-2023.7.27/src/devapp/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,14 @@
     l.extend(['--environ_flags'])
     # FLG = flags.FLAGS
     FLG(l)  # <----------- Flag parsing
     # now reset their values from env
     tools.set_flag_vals_from_env()
     kw_log = {}
     sl.setup_logging(**kw_log)
-    breakpoint()   # FIXME BREAKPOINT
     log = sl.get_logger(name)
     set_app(name, log)
 
 
 running = [0]
```

### Comparing `devapps-2023.6.20/src/devapp/app_token/create_tokens.py` & `devapps-2023.7.27/src/devapp/app_token/create_tokens.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/app_token/read_tokens.py` & `devapps-2023.7.27/src/devapp/app_token/read_tokens.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/components/cloudfoundry.py` & `devapps-2023.7.27/src/devapp/components/cloudfoundry.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/components/gitlab.py` & `devapps-2023.7.27/src/devapp/components/gitlab.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/components/gitlab_runner.py` & `devapps-2023.7.27/src/devapp/components/gitlab_runner.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/dev_mode.py` & `devapps-2023.7.27/src/devapp/dev_mode.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/gevent_patched.py` & `devapps-2023.7.27/src/devapp/gevent_patched.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/layer.py` & `devapps-2023.7.27/src/devapp/layer.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/lib/sh.py` & `devapps-2023.7.27/src/devapp/lib/sh.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/load.py` & `devapps-2023.7.27/src/devapp/load.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/logo` & `devapps-2023.7.27/src/devapp/logo`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/max.py` & `devapps-2023.7.27/src/devapp/max.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/operations/resources.py` & `devapps-2023.7.27/src/devapp/operations/resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,18 @@
         return {'cmd_pre': 'export TMUX_TMPDIR="%s"; ' % d, 'cmd': 'tmux'}
     return cmd
 
 
 class rsc:
     """For services we change dir to project."""
 
+    # class lc_system:
+    #     cmd = 'ops system_lifecycle'
+    #     environ = ['lc_hubs']
+
     class redis_server:
         provides = ['redis-server', 'redis-cli']
         cmd = 'redis-server'
         run = redis_server
         pkg = 'redis-server'
         port = 6379
         systemd = 'redis-server'
```

### Comparing `devapps-2023.6.20/src/devapp/plugins/dev_devapp/repo_sym_links.py` & `devapps-2023.7.27/src/devapp/plugins/dev_devapp/repo_sym_links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resource_install.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/arch/resource_install.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resource_run.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/arch/resource_run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resources.py.dis` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/arch/resources.py.dis`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resources_list.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/arch/resources_list.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/wait_for_port.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/arch/wait_for_port.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/container_build.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/container_build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/container_pull.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/container_pull.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/fs_build.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/fs_build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/kubectl/__init__.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/kubectl/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/life_cycle.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/life_cycle.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/log_view.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/log_view.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/pkgs.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/pkgs.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/project/__init__.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/project/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,14 @@
 class Flags(api.CommonFlags):
     autoshort = ''
 
     class force:
         n = 'Assume y on all questions. Required when started w/o a tty'
         d = False
 
-    #     class skip_inst_when_found:
-    #         n = 'Do not install resources which are present on the host already'
-    #         d = False
     class force_reinstall:
         n = 'Do not only install resources detected uninstalled but reinstall all'
         d = False
 
     class init_at:
         n = 'Set up project in given directory. env vars / relative dirs supported. Sets install action implicitly'
```

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/run.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/system/templates/inst_base.sh` & `devapps-2023.7.27/src/devapp/tools/infra/playbooks/000:functions.sh`

 * *Files 25% similar despite different names*

```diff
@@ -1,107 +1,133 @@
-#!/usr/bin/env bash
-# wget <url> | bash  OR source (not run)
+#!/bin/bash
+_='# Useful functions
 
-set -a
-node="%(node)s"
-lc_hubs="%(lc_hubs)s"
-app_libs="%(app_libs)s"
-d_project="%(d_project)s"
-PATH="$HOME/.local/bin:$PATH"
-set +a
-
-# anything we copied here before is exe:
-chmod +x "$HOME/.local/bin/"*
-
-#inst_url="$inst_protocol://$inst_host"
-function d_artifacts { echo "$MAMBA_ROOT_PREFIX/artifacts/hubpkgs"; }
-
-function sh {
-    echo -e "🟩 $*k"
-    eval "$*"
+  This is run at the very start and creates /root/functions.sh, which all others source
+'
+cluster_name="%(env.cluster_name)s"
+dir_project="%(env.dir_project)s"
+names="%(env.names)s"
+function_filter="%(env.function_filter)s"
+
+SKIP_PRESENT=20
+
+function set_fact { echo -e "%(marker)s \x1b[48;5;56m$1\x1b[0m $2"; }
+function deindent {
+    (
+        IFS='' # drop only once (i.e. the first) 4 spaces:
+        while read -r line; do echo "${line/    /}"; done
+    )
 }
 function die {
-    echo -e "🟥 $*"
+    echo -e "\x1b[48;5;124mERROR $name: $*\x1b[0m"
+    set_fact ERR "$*"
     exit 1
 }
-function activate_home_base {
-    . "$HOME/.bashrc"
-    #. micromamba/etc/profile.d/micromamba.sh
-    micromamba activate base
-}
-function check_bootstrapped {
-    micromamba activate 2>/dev/null && return 0 # e.g. mamba docker container
-    test -e "$HOME/micromamba" && activate_home_base && echo "Mamba activated: $MAMBA_ROOT_PREFIX" && return 0
-    return 1
-}
-function install_bzip {
-    test "$UID" == "0" || {
-        echo "Please install bzip2 as root"
-        exit 1
+
+function have { type $1 1>/dev/null 2>/dev/null; }
+function h1 {
+    echo -e "\x1b[1;38;49m $name \x1b[1;30;41m $*\x1b[0;37m"
+}
+function info {
+    echo -e "INFO: $name $*"
+}
+
+function do_ {
+    local filter="$function_filter"
+    test "$1" == "always" && {
+        filter=
+        shift
     }
-    type apt-get && {
-        apt-get update
-        apt-get install bzip2 && return 0
+
+    local func="$1"
+    test -z "$filter" || {
+        if [[ $func != *$filter* ]]; then
+            h1 "$func skipped (filtered)"
+            return 0
+        fi
     }
-    type yum && { yum install -y bzip2 && return; }
-    exit 1
+    h1 "$func"
+    eval "$@"
+    local res=$?
+    test $res == $SKIP_PRESENT && {
+        h1 "$func skipped (present already)"
+        return 0
+    }
+    test $res != 0 && die "$1 failed"
+    return $res
 }
-function bootstrap {
-    type bzip2 || install_bzip
-    builtin cd
-    curl micro.mamba.pm/install.sh | bash
-    activate_home_base
-}
-function ensure_channel {
-    echo -e 'channels:\n  - conda-forge\n' >"$HOME/.condarc"
-}
-function ensure_mm {
-    local h="$HOME/.bashrc"
-    local line='function mm { micromamba "$@"; }'
-    grep "$line" <"$h" && return 0
-    echo "$line" >>"$h"
-    source "$h"
-}
-function ensure_base_tools {
-    local t r="$MAMBA_ROOT_PREFIX"
-    test -z "$r" && {
-        echo "No mamba"
-        exit 1
+function shcmd {
+    info "$@"
+    eval "$@"
+}
+
+function transfer {
+    local src="$1"
+    local dst="$2"
+    local ip="$3"
+    mkdir -p "$(dirname "$dst")"
+    scp_ "root@$ip:$src" "$dst"
+}
+
+function transfer_kubeconfig {
+    local fn api_host ip
+    api_host="${2?}"
+    ip="${3?}"
+    fn="$(kubeconf)"
+    transfer "$1" "$fn" "$ip"
+    sed -i "s/127.0.0.1/${api_host}/g" "$fn"
+    chmod 600 "$fn" # helm says group readable is unsecure
+    touch environ
+    # adding all fo them, user can comment then:
+    echo "export KUBECONFIG=\"$fn\"" >>"$dir_project/environ"
+    echo "source $dir_project/environ, to activate KUBECONFIG=$fn"
+    # takes a while (ssl)
+    for i in 1 2 3 4 5; do
+        K get nodes --request-timeout=2 --show-labels | grep kubernetes.io && return
+        sleep 1
+    done
+    die "local kubectl failed"
+}
+
+# query the drops cache by node and key:
+function kv { cat "$fn_cache" | jq -r '."'$1'"."'$2'"'; }
+
+function kubeconf { echo "$dir_project/conf/k8s/$cluster_name/config.yaml"; }
+
+function K {
+    export KUBECONFIG="$(kubeconf)"
+    kubectl "$@"
+}
+
+function HELM {
+    export KUBECONFIG="$(kubeconf)"
+    helm "$@"
+}
+
+function pkg_inst {
+    local i
+    type apt 2>/dev/null && i=apt || i=dnf
+    info "package system is $i"
+    $i install -y "$@"
+}
+
+function scp_ { scp -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null "$@"; }
+
+function ssh_ { ssh -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null "$@"; }
+
+function waitproc {
+    # wait until a process is completed or present
+    local no=false
+    test "$1" == "no" && {
+        no=true
+        shift
     }
-    local pkgs=""
-    micromamba list >pkgs
-    tools="python $app_libs"
-    for t in git curl gcc jq fzf; do type "$t" || tools="$tools $t"; done
-    for t in $tools; do grep "$t" <pkgs || pkgs="$t $pkgs"; done
-    test -n "$pkgs" || return 0
-    sh micromamba install --quiet -y "$pkgs" && return 0
-    die "failure pkgs install $pkgs"
-}
-
-function ensure_lc_app_pkg {
-    #local pips="$(pip list)"
-    set -x
-    d="$HOME/.cache/priv_pips"
-    pip install --find-links="$d" "$d_project" && return 0
-    die "pip failed. libs missing?"
-}
-
-function connect {
-    mkdir -p "$d_project"
-    cd "$_"
-    git init
-    curl "$inst_url/system.py" >system.py
-    export PYTHONPATH="$d_project"
-    app client --lc_hubs="$inst_host" --lc_tabs=System --lc_client_name="system:$node" -cf=system:System -ll 10
-}
-
-function main {
-    sh check_bootstrapped || bootstrap
-    sh ensure_channel
-    sh ensure_mm
-    sh activate_home_base
-    sh ensure_base_tools
-    sh ensure_lc_app_pkg
-    sh connect
+    while true; do
+        $no && { pgrep "$1" || return 0; }
+        $no || { pgrep "$1" && return 0; }
+        sleep 1
+        echo "awaiting $1"
+    done
+
 }
 
-main "$@"
+return 2>/dev/null || mv "$0" "functions.sh"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `devapps-2023.6.20/src/devapp/plugins/ops_devapp/system/tools.py` & `devapps-2023.7.27/src/devapp/plugins/ops_devapp/system/tools.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from devapp.app import app, FLG
 from devapp.tools import exists, project, write_file, read_file, dir_of, download_file
+from devapp.tools import abspath
 from devapp.app import FLG, app, run_app, do, system
 import sys
 from functools import partial
 import time
 import json
 
 now = time.time
@@ -92,28 +93,69 @@
 USER = os.environ['USER']
 workdir = f'/tmp/ops_system_{USER}'
 
 from threading import Thread
 
 
 def spawn(f, *a, **kw):
-    if FLG.dbg_non_parallel:
+    app.info(f.__qualname__, args=a)
+    if FLG.dbg_non_parallel or len(FLG.node) == 1:
         f(*a, **kw)
         return
 
     def k(f=f, a=a, kw=kw):
         try:
             f(*a, **kw)
         except Exception as ex:
             api.err.append(ex.args)
 
     t = Thread(target=k)
     t.start()
 
 
+no_node = 'XX'
+
+
+def single_node_cmds(as_str=False):
+    def r(a):
+        for n in FLG.node:
+            a = a.replace(n, no_node)
+        return a
+
+    l = [r(i) for i in list(sys.argv)]
+    cmds = []
+    for n in FLG.node:
+        f = list(l)
+        f.extend(['--node', n])
+        if as_str:
+            f = ' '.join([f'"{i}"' for i in f])
+        cmds.append(f)
+    return cmds
+
+
+def prep_make_workdir_and_abspath_flags():
+    FLG.node = [i for i in FLG.node if not i == no_node]
+    os.makedirs(workdir, exist_ok=True)
+    l = [abspath(i) for i in FLG.transfer_install_local_dirs]
+    FLG.transfer_install_local_dirs = l
+    FLG.system_spec = abspath(FLG.system_spec)
+
+
+def tar_any_project_files():
+    f = [i.strip() for i in FLG.transfer_project_files.split(',')]
+    if not f or not f[0]:
+        FLG.transfer_project_files = None
+        return
+    if any([i for i in f if not exists(i)]):
+        app.die('Not found', files=f)
+    cmd = f'tar cfvz proj_files.tgz {" ".join(f)}'
+    do(system, cmd)
+    FLG.transfer_project_files = abspath(f'./proj_files.tgz')
+
+
 import sys
 
 from rich.console import Console
 from rich.table import Table
 
 
 def out_table(*attrs, title=''):
```

### Comparing `devapps-2023.6.20/src/devapp/run.py` & `devapps-2023.7.27/src/devapp/run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/spec/build.py` & `devapps-2023.7.27/src/devapp/spec/build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/spec/find_paths_in_fs_components.py` & `devapps-2023.7.27/src/devapp/spec/find_paths_in_fs_components.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/spec/fs_components.py` & `devapps-2023.7.27/src/devapp/spec/fs_components.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/spec/links.py` & `devapps-2023.7.27/src/devapp/spec/links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/spec/os_tools.py` & `devapps-2023.7.27/src/devapp/spec/os_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/spec/templ.py` & `devapps-2023.7.27/src/devapp/spec/templ.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/spec/templates/unit` & `devapps-2023.7.27/src/devapp/spec/templates/unit`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/spec/tools.py` & `devapps-2023.7.27/src/devapp/spec/tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/t` & `devapps-2023.7.27/src/devapp/t`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/testing/auto_docs.py` & `devapps-2023.7.27/src/devapp/testing/auto_docs.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/third/rpl` & `devapps-2023.7.27/src/devapp/third/rpl`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/__init__.py` & `devapps-2023.7.27/src/devapp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/flag.py` & `devapps-2023.7.27/src/devapp/tools/flag.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/http.py` & `devapps-2023.7.27/src/devapp/tools/http.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/infra/__init__.py` & `devapps-2023.7.27/src/devapp/tools/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/infra/actions.py` & `devapps-2023.7.27/src/devapp/tools/infra/actions.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh` & `devapps-2023.7.27/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/infra/playbooks/300:dns.sh` & `devapps-2023.7.27/src/devapp/tools/infra/playbooks/300:dns.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/infra/playbooks/500:k3s.sh` & `devapps-2023.7.27/src/devapp/tools/infra/playbooks/500:k3s.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/infra/playbooks/501:kind.sh` & `devapps-2023.7.27/src/devapp/tools/infra/playbooks/501:kind.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/infra/playbooks/502:k3s.sh` & `devapps-2023.7.27/src/devapp/tools/infra/playbooks/502:k3s.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/infra/playbooks/600:longhorn.sh` & `devapps-2023.7.27/src/devapp/tools/infra/playbooks/600:longhorn.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh` & `devapps-2023.7.27/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/old.py` & `devapps-2023.7.27/src/devapp/tools/old.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/plugin.py` & `devapps-2023.7.27/src/devapp/tools/plugin.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/tools/resource.py` & `devapps-2023.7.27/src/devapp/tools/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,14 +370,16 @@
             img = rsc.pkg.split('layers:', 1)[1]
             system('ops container_pull --repo "%s" --dir "%s.img"' % (img, d))
             s = '--skip_filesystem_adaptions'
             system('ops container_build --dirs "%s.img" --target_dir "%s" %s' % (d, d, s))
 
     def write_unit_file(name, fn, rsc, instance):
         pn = project.root().rsplit('/', 1)[-1]
+        name = exported_name(rsc, name)
+
         inst_name = f'{name}-{instance}' if instance else name
         m = {
             'name': inst_name,
             'descr': '%s %s ' % (g(rsc, 'n', inst_name), pn),
             'ctime': time.ctime(),
             'exec_start': fn,
             'env_instance': instance if instance else '',
@@ -407,29 +409,31 @@
             # if cmd == 'dot':
             #    breakpoint()  # FIXME BREAKPOINT
             if isinstance(spec, str):
                 spec = {}
             app.debug('writing bin/' + cmd, cmd=fcmd)
             pre_exec = spec.pop('pre_exec', '')
             spec_env = spec.pop('env', {})
-            fn = project.root() + '/bin/%s' % cmd
+            fn_name = exported_name(rsc, cmd)
+            fn = project.root() + '/bin/%s' % fn_name
             have = read_file(fn, '')
             marker = '-AUTOCREATED- '
             if have and len(have.split('\n' + marker, 1)[0].splitlines()) > 8:
                 return app.warn(
                     'Skipping write of starter file, marker was manually removed',
                     fn=fn,
                     marker=marker,
                 )
             call = sys.argv[0]
             args = ' '.join(sys.argv[1:])
             if call.endswith('/ops'):
                 call = call.rsplit('/', 1)[-1] + ' ' + args
             else:
                 call = call + '\\\n' + args
+            i = rsc
             r = [
                 '#!/usr/bin/env bash',
                 '',
                 '# Delete line containing "%s" to avoid overwrites of this file at project init'
                 % marker,
                 "_='%s" % time.ctime(),
                 marker,
@@ -740,24 +744,30 @@
         if k in listed_attrs and not isinstance(vn, list):
             vn = [vn]
         if vn != v:
             setattr(rsc, k, vn)
 
     rsc.doc = rsc.__doc__ or ''
     rsc.name = rsc.__name__
+    rsc.bin_name = exported_name(rsc)
     rsc.module = rsc.__module__.replace('.operations.resources', '')
     rsc.__repr__ = lambda r: str(to_dict(r))
     rsc.__str__ = lambda r: to_str(r)
     rsc.module_dir = S.rsc_dirs[fn]
-    rsc.host_conf_dir = '$PROJECT_ROOT/conf/${host:-$HOSTNAME}/' + rsc.name
+    rsc.host_conf_dir = '$PROJECT_ROOT/conf/${host:-$HOSTNAME}/' + exported_name(rsc)
     rsc.disabled = g(rsc, 'disabled', g(rsc, 'd', False))
     rsc.installed = g(rsc, 'installed', False)
     [repl_callable(rsc, k, getattr(rsc, k)) for k in dir(rsc) if not k.startswith('_')]
 
 
+exported_name = lambda rsc, d=None: os.environ.get(
+    f'{rsc.name}_name', d if d else rsc.name
+)
+
+
 def to_str(rsc):
     svc = g(rsc, 'systemd')
     i = 'i' if g(rsc, 'installed') else ' '
     d = 'd' if rsc.disabled else ' '
     s = 's' if svc else ' '
     n = svc if svc else rsc.name
     return '%s %s %s %s %s' % (s, i, d, n, g(rsc, 'provides', ''))
```

### Comparing `devapps-2023.6.20/src/devapp/tools/times.py` & `devapps-2023.7.27/src/devapp/tools/times.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/utils/os_.py` & `devapps-2023.7.27/src/devapp/utils/os_.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/utils/py_source_env.py` & `devapps-2023.7.27/src/devapp/utils/py_source_env.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/utils/rx_tools.py` & `devapps-2023.7.27/src/devapp/utils/rx_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/utils/vault.py` & `devapps-2023.7.27/src/devapp/utils/vault.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/devapp/utils/watch_dog.py` & `devapps-2023.7.27/src/devapp/utils/watch_dog.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/mdvl/mdvl.py` & `devapps-2023.7.27/src/mdvl/mdvl.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/mdvl/tools.py` & `devapps-2023.7.27/src/mdvl/tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/structlogging/__init__.py` & `devapps-2023.7.27/src/structlogging/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/structlogging/adapters.py` & `devapps-2023.7.27/src/structlogging/adapters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/structlogging/config.py` & `devapps-2023.7.27/src/structlogging/config.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/structlogging/formatters.py` & `devapps-2023.7.27/src/structlogging/formatters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/structlogging/processors.py` & `devapps-2023.7.27/src/structlogging/processors.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/structlogging/renderers.py` & `devapps-2023.7.27/src/structlogging/renderers.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/structlogging/sl.py` & `devapps-2023.7.27/src/structlogging/sl.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/structlogging/stacktrace.py` & `devapps-2023.7.27/src/structlogging/stacktrace.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/structlogging/tests/test_structlogging.py` & `devapps-2023.7.27/src/structlogging/tests/test_structlogging.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/__init__.py` & `devapps-2023.7.27/src/theming/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/absl_color_help.py` & `devapps-2023.7.27/src/theming/absl_color_help.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/ansi2html.py` & `devapps-2023.7.27/src/theming/ansi2html.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/ansi2html.sh` & `devapps-2023.7.27/src/theming/ansi2html.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/ansistrm.py` & `devapps-2023.7.27/src/theming/ansistrm.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/ax_xml.py` & `devapps-2023.7.27/src/theming/ax_xml.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/camel_snake.py` & `devapps-2023.7.27/src/theming/camel_snake.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/charting.py` & `devapps-2023.7.27/src/theming/charting.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/colorhilite.py` & `devapps-2023.7.27/src/theming/colorhilite.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/filesize/README.txt` & `devapps-2023.7.27/src/theming/filesize/README.txt`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/filesize/filesize.py` & `devapps-2023.7.27/src/theming/filesize/filesize.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/formatters.py` & `devapps-2023.7.27/src/theming/formatters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/formatting/markdown.py` & `devapps-2023.7.27/src/theming/formatting/markdown.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/formatting/viz_sequence.py` & `devapps-2023.7.27/src/theming/formatting/viz_sequence.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/html_tools.py` & `devapps-2023.7.27/src/theming/html_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/inflect.py` & `devapps-2023.7.27/src/theming/inflect.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/pretty_print.py` & `devapps-2023.7.27/src/theming/pretty_print.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/tablepretty.py` & `devapps-2023.7.27/src/theming/tablepretty.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/term.py` & `devapps-2023.7.27/src/theming/term.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/term_struct_hilite.py` & `devapps-2023.7.27/src/theming/term_struct_hilite.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/tests/test_text_formatting.py` & `devapps-2023.7.27/src/theming/tests/test_text_formatting.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/tracebacks.py` & `devapps-2023.7.27/src/theming/tracebacks.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/theming/unicode_chars.py` & `devapps-2023.7.27/src/theming/unicode_chars.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/tree_builder/__init__.py` & `devapps-2023.7.27/src/tree_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/tree_builder/arch/__init__.py.bak` & `devapps-2023.7.27/src/tree_builder/arch/__init__.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/tree_builder/arch/links.py.bak` & `devapps-2023.7.27/src/tree_builder/arch/links.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/tree_builder/arch/o.py` & `devapps-2023.7.27/src/tree_builder/arch/o.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/tree_builder/arch/old` & `devapps-2023.7.27/src/tree_builder/arch/old`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/tree_builder/arch/olinit` & `devapps-2023.7.27/src/tree_builder/arch/olinit`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/tree_builder/arch/oo` & `devapps-2023.7.27/src/tree_builder/arch/oo`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/tree_builder/arch/render.py.bak` & `devapps-2023.7.27/src/tree_builder/arch/render.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/tree_builder/chrome_reload.sh` & `devapps-2023.7.27/src/tree_builder/chrome_reload.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/tree_builder/delivery2.py` & `devapps-2023.7.27/src/tree_builder/delivery2.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/tree_builder/links.py` & `devapps-2023.7.27/src/tree_builder/links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/src/tree_builder/render.py` & `devapps-2023.7.27/src/tree_builder/render.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.6.20/setup.py` & `devapps-2023.7.27/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
  'tree_builder.arch']
 
 package_data = \
 {'': ['*'],
  'devapp': ['third/*'],
  'devapp.plugins.ops_devapp.system': ['templates/*'],
  'devapp.spec': ['templates/*'],
+ 'devapp.tools': ['assets/*'],
  'devapp.tools.infra': ['playbooks/*']}
 
 install_requires = \
 ['absl-py',
  'inflection',
  'jsondiff',
  'pycond',
@@ -62,15 +63,15 @@
                      'dev = devapp.tools.plugin:main',
                      'fui = interactive.cli:main',
                      'myapp = devapp.tools.plugin:main',
                      'ops = devapp.tools.plugin:main']}
 
 setup_kwargs = {
     'name': 'devapps',
-    'version': '2023.6.20',
+    'version': '2023.7.27',
     'description': 'Apps - End to End.',
     'long_description': '# devapps\n\n\n<!-- badges -->\n[![docs pages][docs pages_img]][docs pages] [![gh-ci][gh-ci_img]][gh-ci] [![pkg][pkg_img]][pkg] [![code_style][code_style_img]][code_style] \n\n[docs pages]: https://axgkl.github.io/devapps/\n[docs pages_img]: https://axgkl.github.io/devapps/img/badge_docs.svg\n[gh-ci]: https://github.com/AXGKl/devapps/actions/workflows/ci.yml\n[gh-ci_img]: https://github.com/AXGKl/devapps/actions/workflows/ci.yml/badge.svg\n[pkg]: https://pypi.com/\n[pkg_img]: https://axgkl.github.io/devapps/img/badge_pypi.svg\n[code_style]: https://pypi.org/project/axblack/\n[code_style_img]: https://axgkl.github.io/devapps/img/badge_axblack.svg\n<!-- badges -->\n\n\nEnabler repo for dev *and* ops friendly apps, in a normalized way.\n\nIncludes:\n\n- logging (structlog)\n- cli flags handling (abseil, with addons)\n- docutools (mkdocs-material)\n- project setup\n- (test) resources management, including daemons and container filesystem layers\n\nand more.\n\n\n\n\nDocumentation: https://axgkl.github.io/devapps/',
     'author': 'Gunther Klessinger',
     'author_email': 'g_kle_ss_ing_er@gmx.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://axgkl.github.io/devapps',
```

### Comparing `devapps-2023.6.20/PKG-INFO` & `devapps-2023.7.27/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devapps
-Version: 2023.6.20
+Version: 2023.7.27
 Summary: Apps - End to End.
 Home-page: https://axgkl.github.io/devapps
 License: BSD
 Author: Gunther Klessinger
 Author-email: g_kle_ss_ing_er@gmx.de
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

