# Comparing `tmp/networklab-1.5.4.post1.tar.gz` & `tmp/networklab-1.5.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networklab-1.5.4.post1.tar", last modified: Sun Jun 25 16:16:30 2023, max compression
+gzip compressed data, was "networklab-1.5.5.dev1.tar", last modified: Thu Jul 27 10:49:01 2023, max compression
```

## Comparing `networklab-1.5.4.post1.tar` & `networklab-1.5.5.dev1.tar`

### file list

```diff
@@ -1,624 +1,644 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.437453 networklab-1.5.4.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-25 16:16:30.437453 networklab-1.5.4.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.365451 networklab-1.5.4.post1/netsim/
--rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/addressing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.365451 networklab-1.5.4.post1/netsim/ansible/
--rwxr-xr-x   0 runner    (1001) docker     (123)      900 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/collect-configs.ansible
--rwxr-xr-x   0 runner    (1001) docker     (123)     2899 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/config.ansible
--rwxr-xr-x   0 runner    (1001) docker     (123)     1269 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/create-config.ansible
--rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/display-neighbors.ansible
--rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/initial-config.ansible
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/missing.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.369451 networklab-1.5.4.post1/netsim/ansible/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/create-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/arcos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/asa.yml
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/eos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/frr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/ios.yml
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/junos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/linux-clab.yml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/linux.yml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/none.yml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/sros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/vyos.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-custom-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-module.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/arcos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/asa.yml
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/eos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/ios.yml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/junos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/sros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/vyos.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/fortinet.fortios.fortios/
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/frr/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/frr/deploy-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/frr/mpls-clab.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/iosxr/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/iosxr/initial.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/linux/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/linux/initial-clab.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/nxos/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/nxos/initial.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/readiness-check/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/readiness-check/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/readiness-check/eos-clab.yml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/readiness-check/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/readiness-check/vsrx.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/vmx/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/vmx/initial.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.377452 networklab-1.5.4.post1/netsim/ansible/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.377452 networklab-1.5.4.post1/netsim/ansible/templates/bfd/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/none.j2
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.381452 networklab-1.5.4.post1/netsim/ansible/templates/bgp/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/arubacx.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/asa.j2
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/asa.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/dellos10.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/eos.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/frr.bgp-config.j2
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/ios.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/none.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros7.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/srlinux.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/vyos.macro.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.381452 networklab-1.5.4.post1/netsim/ansible/templates/eigrp/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/eigrp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/eigrp/nxos.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.381452 networklab-1.5.4.post1/netsim/ansible/templates/evpn/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/frr.evpn-config.j2
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.381452 networklab-1.5.4.post1/netsim/ansible/templates/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.389452 networklab-1.5.4.post1/netsim/ansible/templates/initial/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/arcos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/arubacx.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/arubacx.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/asa.j2
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/csr.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/dellos10.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/eos.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/ios.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/ios.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/junos.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/junos.vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.389452 networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/hosts.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/ubuntu.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/vanilla.j2
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/linux-clab.j2
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/linux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/nxos.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros7.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros7.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/vyos.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/vyos.vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.389452 networklab-1.5.4.post1/netsim/ansible/templates/isis/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/asa.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/missing.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.393452 networklab-1.5.4.post1/netsim/ansible/templates/mpls/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/arubacx.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.6pe.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.bgp-lu.j2
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/frr.frr-config.j2
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/frr.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/frr.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/ios.6pe.j2
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/ios.bgp-lu.j2
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/ios.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/ios.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/junos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/junos.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/routeros.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/routeros7.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/sros.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/sros.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/vyos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.397452 networklab-1.5.4.post1/netsim/ansible/templates/ospf/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/arcos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/eos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/eos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/frr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/frr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/ios.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/ios.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/junos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/junos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/none.j2
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/nxos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/nxos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/srlinux.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/vyos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/vyos.ospfv3.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.401452 networklab-1.5.4.post1/netsim/ansible/templates/sr/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/sr/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/sr/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/sr/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/sr/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/sr/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/sr/sros.openconfig.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.401452 networklab-1.5.4.post1/netsim/ansible/templates/srv6/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/srv6/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.401452 networklab-1.5.4.post1/netsim/ansible/templates/vlan/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/csr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/vmx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/vptx.j2
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/vsrx.j2
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.405452 networklab-1.5.4.post1/netsim/ansible/templates/vrf/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.frr-config.j2
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/junos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/nxos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.409452 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/csr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.409452 networklab-1.5.4.post1/netsim/augment/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    40803 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/topology.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.413452 networklab-1.5.4.post1/netsim/cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9700 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/alias.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/clab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/down.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/empty.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/external_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/up.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/usage.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.413452 networklab-1.5.4.post1/netsim/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/data/filemaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/data/global_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    20638 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/data/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    19573 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/data/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.413452 networklab-1.5.4.post1/netsim/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/defaults/addressing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/defaults/attributes.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/defaults/automation.yml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/defaults/hints.yml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/defaults/multilab.yml
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/defaults/ports.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.417452 networklab-1.5.4.post1/netsim/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/arubacx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/asav.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/asav.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/csr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/eos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/eos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/fortios.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/frr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/iosv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/iosv.yml
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/junos.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/linux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/none.yml
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/sros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/unknown.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/unknown.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vmx.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vmx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vptx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vsrx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vsrx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vyos.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.357451 networklab-1.5.4.post1/netsim/extra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.417452 networklab-1.5.4.post1/netsim/extra/ebgp.utils/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/default-originate.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/topology.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.417452 networklab-1.5.4.post1/netsim/extra/multilab/
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/multilab/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.417452 networklab-1.5.4.post1/netsim/extra/none/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/none/none.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.421453 networklab-1.5.4.post1/netsim/extra/proxy-arp/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/proxy-arp/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/proxy-arp/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/proxy-arp/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.421453 networklab-1.5.4.post1/netsim/install/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2162 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/ansible.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3619 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/containerlab.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/grpc.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.421453 networklab-1.5.4.post1/netsim/install/libvirt/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/arubacx.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.421453 networklab-1.5.4.post1/netsim/install/libvirt/asav/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/asav/day0-config
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/asav.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/csr.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/dellos10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/eos.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/eos.xml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/iosv.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/iosv.xml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/iosxr.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/nxos.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/nxos.xml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/routeros7.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.421453 networklab-1.5.4.post1/netsim/install/libvirt/vptx/
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vptx/juniper.conf
--rwxr-xr-x   0 runner    (1001) docker     (123)     1089 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vptx/make-config.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vptx/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vptx.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vptx.xml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.421453 networklab-1.5.4.post1/netsim/install/libvirt/vsrx/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vsrx/juniper.conf
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vsrx.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3185 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/ubuntu.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.425453 networklab-1.5.4.post1/netsim/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    23624 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/_dataplane.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/bfd.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/bfd.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/bgp.yml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/eigrp.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/eigrp.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/evpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/evpn.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/gateway.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/isis.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/isis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/mpls.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/mpls.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/ospf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/ospf.yml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/sr.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/sr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/srv6.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/srv6.yml
--rw-r--r--   0 runner    (1001) docker     (123)    58909 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/vlan.yml
--rw-r--r--   0 runner    (1001) docker     (123)    22607 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/vrf.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/vrf.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/vxlan.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/vxlan.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/d2.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/d2.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/graph.yml
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/graphite.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/none.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/clab.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/clab.yml
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/external.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/external.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/virtualbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/virtualbox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/read_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/ansible.cfg.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.361451 networklab-1.5.4.post1/netsim/templates/provider/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/templates/provider/clab/
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/clab/clab.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/templates/provider/clab/frr/
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/clab/frr/daemons.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/templates/provider/clab/linux/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/clab/linux/hosts.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/templates/provider/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/external/external.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.433453 networklab-1.5.4.post1/netsim/templates/provider/libvirt/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/Vagrantfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/arcos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/arubacx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/asav-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/csr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/cumulus-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/define-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/dellos10-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/eos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/fortios-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/frr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/iosv-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/iosxr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/libvirt-bridge.j2
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/libvirt-tunnel.j2
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/linux-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/none-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/nxos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/routeros-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/routeros7-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/vagrant-libvirt.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/vptx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/vsrx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/vyos-domain.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.433453 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/Vagrantfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/arcos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/cumulus-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/eos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/frr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/linux-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/nxos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/virtualbox-network.j2
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/virtualbox-ports.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.433453 networklab-1.5.4.post1/netsim/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/tests/clab.yml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/tests/libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/tests/virtualbox.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.433453 networklab-1.5.4.post1/netsim/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/tools/graphite.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/tools/graphite.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.433453 networklab-1.5.4.post1/netsim/tools/suzieq/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/tools/suzieq/suzieq-cfg.yml
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/tools/suzieq.yml
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/topology-defaults.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.433453 networklab-1.5.4.post1/netsim/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/utils/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.437453 networklab-1.5.4.post1/networklab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-25 16:16:30.000000 networklab-1.5.4.post1/networklab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21010 2023-06-25 16:16:30.000000 networklab-1.5.4.post1/networklab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 16:16:30.000000 networklab-1.5.4.post1/networklab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-25 16:16:30.000000 networklab-1.5.4.post1/networklab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 16:16:30.000000 networklab-1.5.4.post1/networklab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-25 16:16:30.000000 networklab-1.5.4.post1/networklab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 16:16:30.437453 networklab-1.5.4.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.437453 networklab-1.5.4.post1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3462 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/tests/test_transformation.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.902616 networklab-1.5.5.dev1/
+-rw-r--r--   0 pipi       (501) staff       (20)     1153 2022-05-02 06:40:29.000000 networklab-1.5.5.dev1/LICENSE.md
+-rw-r--r--   0 pipi       (501) staff       (20)      254 2021-12-28 08:07:36.000000 networklab-1.5.5.dev1/MANIFEST.in
+-rw-r--r--   0 pipi       (501) staff       (20)     3744 2023-07-27 10:49:01.902439 networklab-1.5.5.dev1/PKG-INFO
+-rw-r--r--   0 pipi       (501) staff       (20)     3030 2023-07-11 15:49:20.000000 networklab-1.5.5.dev1/README.md
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.730672 networklab-1.5.5.dev1/netsim/
+-rwxr-xr-x   0 pipi       (501) staff       (20)       51 2023-07-27 05:47:27.000000 networklab-1.5.5.dev1/netsim/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)    13301 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/addressing.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.732179 networklab-1.5.5.dev1/netsim/ansible/
+-rwxr-xr-x   0 pipi       (501) staff       (20)      900 2022-12-18 17:58:58.000000 networklab-1.5.5.dev1/netsim/ansible/collect-configs.ansible
+-rwxr-xr-x   0 pipi       (501) staff       (20)     2899 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/ansible/config.ansible
+-rwxr-xr-x   0 pipi       (501) staff       (20)     1269 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/create-config.ansible
+-rwxr--r--   0 pipi       (501) staff       (20)      295 2022-10-25 08:11:07.000000 networklab-1.5.5.dev1/netsim/ansible/display-neighbors.ansible
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3460 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/ansible/initial-config.ansible
+-rw-r--r--   0 pipi       (501) staff       (20)      401 2022-12-22 15:59:29.000000 networklab-1.5.5.dev1/netsim/ansible/missing.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.732878 networklab-1.5.5.dev1/netsim/ansible/tasks/
+-rw-r--r--   0 pipi       (501) staff       (20)      720 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/create-config.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.739641 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/
+-rw-r--r--   0 pipi       (501) staff       (20)      333 2022-05-02 05:23:35.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/arcos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      592 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/arubacx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      157 2022-11-10 07:29:53.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/asa.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      717 2022-05-02 05:23:46.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/cumulus.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      841 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      376 2022-04-17 16:31:22.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      159 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/eos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      555 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/frr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      159 2022-12-19 08:16:52.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/ios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      163 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/iosxr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      204 2022-12-18 17:58:58.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/junos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      593 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/linux-clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      278 2022-12-22 08:33:55.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/linux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      140 2022-03-20 08:56:05.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/none.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      161 2022-05-02 06:40:29.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/nxos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      777 2022-05-02 05:37:23.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/routeros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      240 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3328 2023-03-06 07:47:06.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/srlinux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     4846 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/sros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      551 2022-12-18 17:58:58.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/vyos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3196 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-custom-config.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2250 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-module.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.743693 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/
+-rw-r--r--   0 pipi       (501) staff       (20)      160 2021-07-09 15:23:10.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/arcos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      110 2022-11-10 07:29:53.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/asa.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      254 2022-03-07 15:39:35.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/cumulus.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      308 2022-03-07 15:39:45.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      115 2022-04-17 16:31:22.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      112 2022-03-07 15:40:03.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/eos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      346 2021-12-11 08:49:40.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      110 2022-12-19 08:45:45.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/ios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      107 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/iosxr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      124 2021-07-09 15:23:10.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/junos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      113 2021-07-09 15:23:10.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/nxos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      195 2021-11-27 09:09:57.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/routeros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      195 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      721 2022-03-07 17:07:35.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/srlinux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      469 2022-03-07 17:07:35.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/sros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2021-11-27 09:09:57.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/vyos.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.744174 networklab-1.5.5.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/
+-rw-r--r--   0 pipi       (501) staff       (20)     2645 2022-01-20 07:34:11.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2494 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.744483 networklab-1.5.5.dev1/netsim/ansible/tasks/frr/
+-rw-r--r--   0 pipi       (501) staff       (20)      555 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/frr/deploy-config.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      243 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/frr/mpls-clab.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.744708 networklab-1.5.5.dev1/netsim/ansible/tasks/iosxr/
+-rw-r--r--   0 pipi       (501) staff       (20)      900 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/iosxr/initial.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.744931 networklab-1.5.5.dev1/netsim/ansible/tasks/linux/
+-rw-r--r--   0 pipi       (501) staff       (20)     1504 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/linux/initial-clab.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.745140 networklab-1.5.5.dev1/netsim/ansible/tasks/nxos/
+-rw-r--r--   0 pipi       (501) staff       (20)      291 2022-12-05 12:30:42.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/nxos/initial.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.745827 networklab-1.5.5.dev1/netsim/ansible/tasks/readiness-check/
+-rw-r--r--   0 pipi       (501) staff       (20)      491 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/readiness-check/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      125 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/readiness-check/eos-clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/readiness-check/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      502 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/readiness-check/vsrx.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.746091 networklab-1.5.5.dev1/netsim/ansible/tasks/vmx/
+-rw-r--r--   0 pipi       (501) staff       (20)     1707 2022-12-22 09:02:46.000000 networklab-1.5.5.dev1/netsim/ansible/tasks/vmx/initial.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.746343 networklab-1.5.5.dev1/netsim/ansible/templates/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.748254 networklab-1.5.5.dev1/netsim/ansible/templates/bfd/
+-rw-r--r--   0 pipi       (501) staff       (20)      618 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bfd/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      700 2022-12-11 11:47:34.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bfd/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      599 2022-01-09 08:37:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bfd/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2022-01-09 08:37:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bfd/none.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      834 2022-01-09 08:37:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bfd/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      611 2022-01-09 08:37:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bfd/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1267 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bfd/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      486 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bfd/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.755310 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/
+-rw-r--r--   0 pipi       (501) staff       (20)     1363 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/arubacx.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      888 2022-11-10 07:29:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/asa.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      778 2022-11-10 07:29:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/asa.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       74 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3040 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1257 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/dellos10.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1755 2022-12-11 16:40:37.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/eos.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2621 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/frr.bgp-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       66 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1369 2023-02-07 15:05:29.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/ios.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1830 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2308 2022-05-02 06:40:29.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/none.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1696 2022-09-01 07:44:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1045 2022-05-02 06:40:29.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/routeros.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1075 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/routeros7.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-05-02 06:40:29.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/srlinux.cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      316 2022-12-18 17:58:58.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     8056 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/srlinux.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3504 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      534 2022-10-25 08:00:46.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2873 2022-05-02 06:40:29.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/sros.md-cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-01-30 15:43:37.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1492 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/bgp/vyos.macro.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.755628 networklab-1.5.5.dev1/netsim/ansible/templates/eigrp/
+-rw-r--r--   0 pipi       (501) staff       (20)     1234 2023-02-07 15:05:29.000000 networklab-1.5.5.dev1/netsim/ansible/templates/eigrp/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      862 2022-02-14 14:03:36.000000 networklab-1.5.5.dev1/netsim/ansible/templates/eigrp/nxos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.758102 networklab-1.5.5.dev1/netsim/ansible/templates/evpn/
+-rw-r--r--   0 pipi       (501) staff       (20)      903 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/evpn/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1143 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/ansible/templates/evpn/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1621 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/ansible/templates/evpn/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-12-15 16:40:50.000000 networklab-1.5.5.dev1/netsim/ansible/templates/evpn/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1631 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/ansible/templates/evpn/frr.evpn-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       35 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/evpn/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1677 2023-01-30 13:30:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/evpn/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1853 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/ansible/templates/evpn/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1239 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/evpn/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2883 2022-09-25 16:03:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/evpn/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.760177 networklab-1.5.5.dev1/netsim/ansible/templates/gateway/
+-rw-r--r--   0 pipi       (501) staff       (20)     1346 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/gateway/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1244 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/ansible/templates/gateway/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1162 2022-11-17 08:20:15.000000 networklab-1.5.5.dev1/netsim/ansible/templates/gateway/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      951 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/ansible/templates/gateway/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      739 2022-12-14 07:49:49.000000 networklab-1.5.5.dev1/netsim/ansible/templates/gateway/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      727 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/ansible/templates/gateway/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      613 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/ansible/templates/gateway/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      953 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/ansible/templates/gateway/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1006 2022-11-17 08:20:15.000000 networklab-1.5.5.dev1/netsim/ansible/templates/gateway/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.768715 networklab-1.5.5.dev1/netsim/ansible/templates/initial/
+-rw-r--r--   0 pipi       (501) staff       (20)      836 2022-01-05 16:01:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/arcos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1200 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      480 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/arubacx.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      466 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/arubacx.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1122 2022-11-10 07:29:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/asa.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       44 2022-12-18 17:58:58.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/csr.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     5288 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1342 2022-10-22 08:18:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1643 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      537 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/dellos10.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2201 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      261 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/eos.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3945 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2371 2022-12-18 17:58:58.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      157 2022-12-14 07:50:27.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/ios.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      378 2022-09-11 07:46:54.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/ios.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1717 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2118 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1706 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/junos.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1607 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/junos.vrf.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.769397 networklab-1.5.5.dev1/netsim/ansible/templates/initial/linux/
+-rw-r--r--   0 pipi       (501) staff       (20)      923 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/linux/hosts.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3481 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/linux/ubuntu.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2026 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/linux/vanilla.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      283 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/linux-clab.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      434 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/linux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1937 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      393 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/nxos.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1413 2022-06-20 08:57:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      546 2022-06-20 08:57:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/routeros.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      498 2022-08-18 15:16:48.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/routeros.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1571 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      611 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/routeros7.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      352 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/routeros7.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      968 2022-01-05 16:01:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/srlinux.cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3479 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     4863 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1434 2022-01-05 16:01:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/sros.md-cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2622 2022-01-06 16:04:54.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2782 2022-11-10 07:29:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      250 2022-06-20 08:57:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/vyos.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      101 2022-08-18 15:17:06.000000 networklab-1.5.5.dev1/netsim/ansible/templates/initial/vyos.vrf.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.772078 networklab-1.5.5.dev1/netsim/ansible/templates/isis/
+-rw-r--r--   0 pipi       (501) staff       (20)      887 2022-11-10 07:29:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/isis/asa.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1241 2022-02-14 14:03:36.000000 networklab-1.5.5.dev1/netsim/ansible/templates/isis/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1149 2022-02-14 14:03:36.000000 networklab-1.5.5.dev1/netsim/ansible/templates/isis/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1505 2022-12-20 08:16:04.000000 networklab-1.5.5.dev1/netsim/ansible/templates/isis/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1168 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/isis/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2225 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/isis/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1701 2022-02-14 14:03:36.000000 networklab-1.5.5.dev1/netsim/ansible/templates/isis/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-11-23 16:08:58.000000 networklab-1.5.5.dev1/netsim/ansible/templates/isis/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1426 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/ansible/templates/isis/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1550 2022-01-06 06:47:23.000000 networklab-1.5.5.dev1/netsim/ansible/templates/isis/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1262 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/isis/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      136 2021-12-06 08:23:27.000000 networklab-1.5.5.dev1/netsim/ansible/templates/missing.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.778747 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/
+-rw-r--r--   0 pipi       (501) staff       (20)      149 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      203 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/arubacx.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      333 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      670 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/eos.6pe.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1089 2022-04-01 07:43:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/eos.bgp-lu.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      289 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      410 2022-04-01 07:43:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/eos.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      413 2022-04-01 07:43:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/eos.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      195 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/frr.frr-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      272 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      562 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/frr.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      327 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/frr.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      208 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/ios.6pe.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      611 2022-08-11 09:57:08.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/ios.bgp-lu.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      302 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      257 2022-04-01 07:43:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/ios.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      326 2022-04-01 07:43:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/ios.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      328 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      542 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/junos.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      656 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/junos.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      151 2022-04-06 16:02:55.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      383 2022-04-06 16:02:55.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/routeros.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      412 2022-04-06 16:02:55.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      198 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      382 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/routeros7.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      408 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      272 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1159 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/sros.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      342 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/sros.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      432 2022-04-17 16:31:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      462 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/vyos.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      668 2022-04-17 16:31:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.787548 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/
+-rw-r--r--   0 pipi       (501) staff       (20)      488 2022-01-06 08:25:20.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/arcos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      198 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1040 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1061 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      199 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      778 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      791 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1228 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      200 2022-04-17 16:31:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      838 2022-04-17 16:31:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      834 2022-04-17 16:31:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:46.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1032 2022-02-14 14:03:36.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/eos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      967 2022-09-04 08:58:45.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/eos.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      222 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      737 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/frr.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      713 2022-12-20 07:49:03.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/frr.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      897 2022-02-14 14:03:36.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/ios.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      871 2022-02-14 14:03:36.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/ios.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      194 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      948 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      936 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      430 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1082 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/junos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1084 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/junos.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/none.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      152 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      987 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/nxos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      995 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/nxos.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2141 2022-04-06 16:02:55.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      478 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1145 2022-01-05 16:01:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/srlinux.cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      304 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1801 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/srlinux.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1964 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1038 2022-01-21 21:00:25.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/sros.md-cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      618 2021-12-28 08:07:36.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      385 2022-03-09 10:04:56.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      957 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/vyos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      869 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/ospf/vyos.ospfv3.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.788875 networklab-1.5.5.dev1/netsim/ansible/templates/sr/
+-rw-r--r--   0 pipi       (501) staff       (20)      245 2021-07-09 15:23:10.000000 networklab-1.5.5.dev1/netsim/ansible/templates/sr/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      270 2021-07-09 15:23:10.000000 networklab-1.5.5.dev1/netsim/ansible/templates/sr/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1127 2023-01-12 13:45:42.000000 networklab-1.5.5.dev1/netsim/ansible/templates/sr/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2286 2023-01-04 17:29:57.000000 networklab-1.5.5.dev1/netsim/ansible/templates/sr/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1237 2023-01-04 17:30:40.000000 networklab-1.5.5.dev1/netsim/ansible/templates/sr/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      945 2021-12-28 08:07:36.000000 networklab-1.5.5.dev1/netsim/ansible/templates/sr/sros.openconfig.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.789092 networklab-1.5.5.dev1/netsim/ansible/templates/srv6/
+-rw-r--r--   0 pipi       (501) staff       (20)     4092 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/srv6/sros.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.799973 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/
+-rw-r--r--   0 pipi       (501) staff       (20)      561 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1186 2022-12-18 14:12:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/csr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1730 2022-12-18 14:12:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      949 2022-11-17 08:20:15.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      757 2022-12-15 11:32:15.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1212 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      457 2022-12-14 07:49:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      776 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      432 2022-06-20 08:57:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1115 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2756 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1909 2023-04-02 11:32:00.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      815 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/vmx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1029 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/vptx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       25 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/vsrx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      771 2022-06-20 08:57:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vlan/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.814515 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/
+-rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      920 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/arubacx.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      180 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1068 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      492 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      106 2022-04-17 16:31:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      690 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/dellos10.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      182 2022-09-10 16:16:52.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      888 2022-09-10 16:21:58.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/eos.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1189 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/eos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-11 07:35:29.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1027 2022-05-02 06:40:29.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1679 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/frr.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      412 2022-10-24 12:44:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/frr.frr-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      524 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      762 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/ios.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      716 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/ios.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-10 16:23:03.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      880 2022-10-24 08:27:03.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2169 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/junos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      693 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1169 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/nxos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      173 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      989 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1540 2022-08-18 15:19:05.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      182 2022-04-06 16:02:55.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1721 2022-05-01 16:20:27.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1095 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros7.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      185 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      463 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1336 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1272 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1272 2022-12-07 14:41:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/vyos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      535 2022-04-17 16:31:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1037 2022-04-17 16:31:22.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.817417 networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/
+-rw-r--r--   0 pipi       (501) staff       (20)      423 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      570 2022-12-18 14:12:35.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/csr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1011 2022-12-15 13:56:36.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      420 2022-09-16 11:40:01.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      381 2022-12-15 14:02:16.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1929 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      662 2022-12-15 14:02:29.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2234 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2579 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1315 2022-09-16 11:40:09.000000 networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      740 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/api.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.820265 networklab-1.5.5.dev1/netsim/augment/
+-rw-r--r--   0 pipi       (501) staff       (20)      230 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/augment/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     6449 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/augment/components.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2803 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/augment/config.py
+-rw-r--r--   0 pipi       (501) staff       (20)     6452 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/augment/devices.py
+-rw-r--r--   0 pipi       (501) staff       (20)    18000 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/augment/groups.py
+-rw-r--r--   0 pipi       (501) staff       (20)    40803 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/augment/links.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3248 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/augment/main.py
+-rw-r--r--   0 pipi       (501) staff       (20)    12868 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/augment/nodes.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2810 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/augment/plugin.py
+-rw-r--r--   0 pipi       (501) staff       (20)     7621 2023-07-13 14:26:22.000000 networklab-1.5.5.dev1/netsim/augment/topology.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/callback.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.832986 networklab-1.5.5.dev1/netsim/cli/
+-rwxr-xr-x   0 pipi       (501) staff       (20)     9773 2023-07-27 05:51:10.000000 networklab-1.5.5.dev1/netsim/cli/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)      319 2022-08-23 07:24:58.000000 networklab-1.5.5.dev1/netsim/cli/alias.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1716 2023-07-09 07:35:25.000000 networklab-1.5.5.dev1/netsim/cli/ansible.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4169 2023-07-09 07:35:25.000000 networklab-1.5.5.dev1/netsim/cli/clab.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2680 2022-03-20 09:12:02.000000 networklab-1.5.5.dev1/netsim/cli/collect.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1392 2022-03-07 15:33:10.000000 networklab-1.5.5.dev1/netsim/cli/config.py
+-rw-r--r--   0 pipi       (501) staff       (20)     5545 2023-07-09 07:35:25.000000 networklab-1.5.5.dev1/netsim/cli/connect.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2974 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/cli/create.py
+-rw-r--r--   0 pipi       (501) staff       (20)     7029 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/cli/down.py
+-rw-r--r--   0 pipi       (501) staff       (20)       63 2023-03-06 07:47:06.000000 networklab-1.5.5.dev1/netsim/cli/empty.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     6323 2023-07-27 06:04:59.000000 networklab-1.5.5.dev1/netsim/cli/external_commands.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1583 2023-07-13 14:12:56.000000 networklab-1.5.5.dev1/netsim/cli/graph.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3181 2023-04-02 11:32:00.000000 networklab-1.5.5.dev1/netsim/cli/initial.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2043 2023-07-13 14:28:37.000000 networklab-1.5.5.dev1/netsim/cli/inspect.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2027 2023-07-09 07:35:25.000000 networklab-1.5.5.dev1/netsim/cli/install.py
+-rw-r--r--   0 pipi       (501) staff       (20)     9994 2023-07-09 07:35:25.000000 networklab-1.5.5.dev1/netsim/cli/libvirt.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1332 2023-04-10 10:10:02.000000 networklab-1.5.5.dev1/netsim/cli/read.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1424 2023-07-13 14:13:04.000000 networklab-1.5.5.dev1/netsim/cli/report.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1354 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/cli/restart.py
+-rw-r--r--   0 pipi       (501) staff       (20)     9161 2023-07-09 07:35:25.000000 networklab-1.5.5.dev1/netsim/cli/show.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4774 2023-07-09 07:35:25.000000 networklab-1.5.5.dev1/netsim/cli/status.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3431 2023-07-09 07:35:25.000000 networklab-1.5.5.dev1/netsim/cli/test.py
+-rw-r--r--   0 pipi       (501) staff       (20)    10868 2023-07-27 10:32:32.000000 networklab-1.5.5.dev1/netsim/cli/up.py
+-rw-r--r--   0 pipi       (501) staff       (20)      417 2021-06-25 12:25:32.000000 networklab-1.5.5.dev1/netsim/cli/usage.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2287 2023-07-13 14:38:47.000000 networklab-1.5.5.dev1/netsim/cli/usage.txt
+-rw-r--r--   0 pipi       (501) staff       (20)      180 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/cli/version.py
+-rw-r--r--   0 pipi       (501) staff       (20)      752 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/common.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.834486 networklab-1.5.5.dev1/netsim/data/
+-rw-r--r--   0 pipi       (501) staff       (20)     4332 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/data/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3076 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/data/filemaps.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1329 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/data/global_vars.py
+-rw-r--r--   0 pipi       (501) staff       (20)    20638 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/data/types.py
+-rw-r--r--   0 pipi       (501) staff       (20)    19573 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/data/validate.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.836157 networklab-1.5.5.dev1/netsim/defaults/
+-rw-r--r--   0 pipi       (501) staff       (20)      294 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/defaults/addressing.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2452 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/defaults/attributes.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      112 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/defaults/automation.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      610 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/defaults/hints.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      363 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/defaults/multilab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)       86 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/defaults/ports.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.843582 networklab-1.5.5.dev1/netsim/devices/
+-rw-r--r--   0 pipi       (501) staff       (20)     1812 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/devices/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)      854 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/devices/arubacx.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1128 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/devices/arubacx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      950 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/devices/asav.py
+-rw-r--r--   0 pipi       (501) staff       (20)      798 2023-04-02 11:32:00.000000 networklab-1.5.5.dev1/netsim/devices/asav.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      740 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/devices/csr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1049 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/devices/cumulus.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      748 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/devices/cumulus_nvue.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/devices/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2241 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/devices/eos.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1642 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/devices/eos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      502 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/devices/fortios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1210 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/devices/frr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      822 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/devices/iosv.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1449 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/devices/iosv.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      949 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/devices/iosxr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/devices/junos.py
+-rw-r--r--   0 pipi       (501) staff       (20)      757 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/devices/linux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1148 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/devices/none.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      923 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/devices/nxos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      507 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/devices/routeros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/devices/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1355 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/devices/srlinux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1671 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/devices/sros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      932 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/devices/unknown.py
+-rw-r--r--   0 pipi       (501) staff       (20)      115 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/devices/unknown.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/devices/vmx.py
+-rw-r--r--   0 pipi       (501) staff       (20)      827 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/devices/vmx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/devices/vptx.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1638 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/devices/vptx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/devices/vsrx.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1275 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/devices/vsrx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1008 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/devices/vyos.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.726102 networklab-1.5.5.dev1/netsim/extra/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.843876 networklab-1.5.5.dev1/netsim/extra/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     2215 2022-09-04 16:06:08.000000 networklab-1.5.5.dev1/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.846877 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.847494 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     2171 2023-02-02 15:17:54.000000 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)     4976 2023-04-15 13:39:23.000000 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-311.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)      681 2022-12-22 16:28:14.000000 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/default-originate.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1198 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2162 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1528 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1891 2022-12-19 09:40:05.000000 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     4470 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/plugin.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1695 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      263 2022-08-21 12:51:31.000000 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/topology.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2877 2022-08-27 11:27:47.000000 networklab-1.5.5.dev1/netsim/extra/ebgp.utils/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.847843 networklab-1.5.5.dev1/netsim/extra/multilab/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.848446 networklab-1.5.5.dev1/netsim/extra/multilab/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     1787 2023-01-30 16:32:51.000000 networklab-1.5.5.dev1/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)     3509 2023-04-15 10:43:11.000000 networklab-1.5.5.dev1/netsim/extra/multilab/__pycache__/plugin.cpython-311.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)     3051 2023-02-07 15:05:29.000000 networklab-1.5.5.dev1/netsim/extra/multilab/plugin.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.848761 networklab-1.5.5.dev1/netsim/extra/none/
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.5.dev1/netsim/extra/none/none.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.849538 networklab-1.5.5.dev1/netsim/extra/proxy-arp/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.850483 networklab-1.5.5.dev1/netsim/extra/proxy-arp/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-02-02 15:17:59.000000 networklab-1.5.5.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)     1772 2023-04-15 10:43:07.000000 networklab-1.5.5.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-311.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)      934 2022-10-24 08:42:48.000000 networklab-1.5.5.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)      890 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/extra/proxy-arp/plugin.py
+-rw-r--r--   0 pipi       (501) staff       (20)      717 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/extra/proxy-arp/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      682 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/extra/proxy-arp/sros.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.851913 networklab-1.5.5.dev1/netsim/install/
+-rwxr--r--   0 pipi       (501) staff       (20)     2162 2023-03-13 11:11:29.000000 networklab-1.5.5.dev1/netsim/install/ansible.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3619 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/install/containerlab.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)      745 2023-01-13 19:14:18.000000 networklab-1.5.5.dev1/netsim/install/grpc.sh
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.855478 networklab-1.5.5.dev1/netsim/install/libvirt/
+-rw-r--r--   0 pipi       (501) staff       (20)     1183 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/install/libvirt/arubacx.txt
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.855698 networklab-1.5.5.dev1/netsim/install/libvirt/asav/
+-rw-r--r--   0 pipi       (501) staff       (20)      972 2023-04-02 11:32:00.000000 networklab-1.5.5.dev1/netsim/install/libvirt/asav/day0-config
+-rw-r--r--   0 pipi       (501) staff       (20)      369 2023-04-02 11:32:00.000000 networklab-1.5.5.dev1/netsim/install/libvirt/asav.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1219 2022-12-11 18:08:47.000000 networklab-1.5.5.dev1/netsim/install/libvirt/csr.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1493 2022-04-17 16:31:22.000000 networklab-1.5.5.dev1/netsim/install/libvirt/dellos10.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     2214 2022-03-09 10:04:56.000000 networklab-1.5.5.dev1/netsim/install/libvirt/eos.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1531 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/install/libvirt/eos.xml.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1665 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/install/libvirt/iosv.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     2911 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/install/libvirt/iosv.xml.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.855974 networklab-1.5.5.dev1/netsim/install/libvirt/iosxr/
+-rw-r--r--   0 pipi       (501) staff       (20)      360 2022-12-21 10:32:36.000000 networklab-1.5.5.dev1/netsim/install/libvirt/iosxr/iosxr_config.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1044 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/install/libvirt/iosxr.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-01-28 18:41:01.000000 networklab-1.5.5.dev1/netsim/install/libvirt/nxos.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1523 2022-09-25 07:16:04.000000 networklab-1.5.5.dev1/netsim/install/libvirt/nxos.xml.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      940 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/install/libvirt/routeros7.txt
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.856678 networklab-1.5.5.dev1/netsim/install/libvirt/vptx/
+-rw-r--r--   0 pipi       (501) staff       (20)     1994 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/install/libvirt/vptx/juniper.conf
+-rwxr-xr-x   0 pipi       (501) staff       (20)     1089 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/install/libvirt/vptx/make-config.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)      654 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/install/libvirt/vptx/run.sh
+-rw-r--r--   0 pipi       (501) staff       (20)     1653 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/install/libvirt/vptx.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     2552 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/install/libvirt/vptx.xml.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.856865 networklab-1.5.5.dev1/netsim/install/libvirt/vsrx/
+-rw-r--r--   0 pipi       (501) staff       (20)     2243 2022-03-09 10:04:56.000000 networklab-1.5.5.dev1/netsim/install/libvirt/vsrx/juniper.conf
+-rw-r--r--   0 pipi       (501) staff       (20)      540 2022-03-09 10:04:56.000000 networklab-1.5.5.dev1/netsim/install/libvirt/vsrx.txt
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3185 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/install/libvirt.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)     1881 2022-11-04 10:28:02.000000 networklab-1.5.5.dev1/netsim/install/ubuntu.sh
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.873160 networklab-1.5.5.dev1/netsim/modules/
+-rw-r--r--   0 pipi       (501) staff       (20)    23644 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     6155 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/modules/_dataplane.py
+-rw-r--r--   0 pipi       (501) staff       (20)    10721 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/modules/_routing.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3923 2023-01-14 09:41:51.000000 networklab-1.5.5.dev1/netsim/modules/bfd.py
+-rw-r--r--   0 pipi       (501) staff       (20)      724 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/bfd.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    21025 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/modules/bgp.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1843 2023-07-13 14:46:51.000000 networklab-1.5.5.dev1/netsim/modules/bgp.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      496 2023-01-12 16:03:44.000000 networklab-1.5.5.dev1/netsim/modules/eigrp.py
+-rw-r--r--   0 pipi       (501) staff       (20)      318 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/eigrp.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    17695 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/modules/evpn.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1119 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/evpn.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     6763 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/modules/gateway.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1029 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/gateway.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      141 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/initial.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2579 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/modules/isis.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1074 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/isis.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     7051 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/modules/mpls.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1060 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/mpls.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3764 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/ospf.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1389 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/ospf.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      152 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/modules/sr.py
+-rw-r--r--   0 pipi       (501) staff       (20)      417 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/sr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-14 09:55:20.000000 networklab-1.5.5.dev1/netsim/modules/srv6.py
+-rw-r--r--   0 pipi       (501) staff       (20)      518 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/srv6.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    58909 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/modules/vlan.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1246 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/vlan.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    22607 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/modules/vrf.py
+-rw-r--r--   0 pipi       (501) staff       (20)      458 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/vrf.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     9043 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/modules/vxlan.py
+-rw-r--r--   0 pipi       (501) staff       (20)      591 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/modules/vxlan.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.880971 networklab-1.5.5.dev1/netsim/outputs/
+-rw-r--r--   0 pipi       (501) staff       (20)     2233 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/outputs/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     7386 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/outputs/ansible.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1786 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/outputs/common.py
+-rw-r--r--   0 pipi       (501) staff       (20)    10023 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/outputs/d2.py
+-rw-r--r--   0 pipi       (501) staff       (20)      545 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/outputs/d2.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2805 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/outputs/devices.py
+-rw-r--r--   0 pipi       (501) staff       (20)      255 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/outputs/format.py
+-rw-r--r--   0 pipi       (501) staff       (20)     7556 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/outputs/graph.py
+-rw-r--r--   0 pipi       (501) staff       (20)      218 2023-04-02 11:32:00.000000 networklab-1.5.5.dev1/netsim/outputs/graph.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      641 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/outputs/graphite.py
+-rw-r--r--   0 pipi       (501) staff       (20)      278 2021-08-22 05:50:16.000000 networklab-1.5.5.dev1/netsim/outputs/json.py
+-rw-r--r--   0 pipi       (501) staff       (20)      228 2021-12-18 16:49:49.000000 networklab-1.5.5.dev1/netsim/outputs/none.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1838 2023-04-02 11:32:00.000000 networklab-1.5.5.dev1/netsim/outputs/provider.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2235 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/outputs/report.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2893 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/outputs/tools.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1678 2023-07-13 14:21:52.000000 networklab-1.5.5.dev1/netsim/outputs/yaml.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.883742 networklab-1.5.5.dev1/netsim/providers/
+-rw-r--r--   0 pipi       (501) staff       (20)     8911 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/providers/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3873 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/providers/clab.py
+-rw-r--r--   0 pipi       (501) staff       (20)      965 2023-05-16 06:09:38.000000 networklab-1.5.5.dev1/netsim/providers/clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      836 2022-12-24 16:57:23.000000 networklab-1.5.5.dev1/netsim/providers/external.py
+-rw-r--r--   0 pipi       (501) staff       (20)      157 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/providers/external.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    12596 2023-07-27 10:24:43.000000 networklab-1.5.5.dev1/netsim/providers/libvirt.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1157 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/providers/libvirt.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      210 2022-12-24 16:57:30.000000 networklab-1.5.5.dev1/netsim/providers/virtualbox.py
+-rw-r--r--   0 pipi       (501) staff       (20)      320 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/providers/virtualbox.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     8373 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/read_topology.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.884052 networklab-1.5.5.dev1/netsim/templates/
+-rw-r--r--   0 pipi       (501) staff       (20)      469 2022-05-26 14:27:51.000000 networklab-1.5.5.dev1/netsim/templates/ansible.cfg.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.727449 networklab-1.5.5.dev1/netsim/templates/provider/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.884343 networklab-1.5.5.dev1/netsim/templates/provider/clab/
+-rw-r--r--   0 pipi       (501) staff       (20)     3251 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/templates/provider/clab/clab.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.884554 networklab-1.5.5.dev1/netsim/templates/provider/clab/frr/
+-rw-r--r--   0 pipi       (501) staff       (20)     2935 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/templates/provider/clab/frr/daemons.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.884859 networklab-1.5.5.dev1/netsim/templates/provider/clab/linux/
+-rw-r--r--   0 pipi       (501) staff       (20)      604 2023-01-12 13:45:42.000000 networklab-1.5.5.dev1/netsim/templates/provider/clab/linux/hosts.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.885154 networklab-1.5.5.dev1/netsim/templates/provider/external/
+-rw-r--r--   0 pipi       (501) staff       (20)     1318 2022-12-18 14:12:35.000000 networklab-1.5.5.dev1/netsim/templates/provider/external/external.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.894550 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/
+-rw-r--r--   0 pipi       (501) staff       (20)      683 2023-07-27 10:09:42.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/Vagrantfile.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      332 2022-01-25 17:29:43.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/arcos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      410 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/arubacx-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      427 2022-11-10 07:29:53.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/asav-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      445 2022-12-11 17:33:57.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/csr-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:59:15.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/cumulus-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1177 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1297 2023-03-06 07:47:06.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/define-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      438 2022-04-17 16:31:22.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/dellos10-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      355 2022-01-25 17:30:38.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/eos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      258 2022-01-25 17:30:42.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/fortios-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/frr-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      380 2022-12-11 10:03:46.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/iosv-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1835 2023-01-12 13:38:07.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/iosxr-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      952 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/libvirt-bridge.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      668 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/libvirt-tunnel.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2023-06-25 15:22:47.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/linux-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       52 2021-12-28 08:07:36.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/none-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      814 2022-12-12 17:43:45.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/nxos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      309 2022-01-25 17:31:10.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/routeros-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      347 2022-10-19 17:10:38.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/routeros7-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1283 2023-01-28 07:18:50.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/vagrant-libvirt.xml
+-rw-r--r--   0 pipi       (501) staff       (20)     2728 2023-06-10 16:45:53.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/vptx-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      740 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/vsrx-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      223 2022-01-25 17:31:29.000000 networklab-1.5.5.dev1/netsim/templates/provider/libvirt/vyos-domain.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.897011 networklab-1.5.5.dev1/netsim/templates/provider/virtualbox/
+-rw-r--r--   0 pipi       (501) staff       (20)      818 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/templates/provider/virtualbox/Vagrantfile.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      274 2022-01-25 17:34:51.000000 networklab-1.5.5.dev1/netsim/templates/provider/virtualbox/arcos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      192 2022-09-05 16:28:24.000000 networklab-1.5.5.dev1/netsim/templates/provider/virtualbox/cumulus-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      108 2022-01-25 17:35:32.000000 networklab-1.5.5.dev1/netsim/templates/provider/virtualbox/eos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      192 2023-06-25 16:15:11.000000 networklab-1.5.5.dev1/netsim/templates/provider/virtualbox/frr-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      191 2022-01-25 17:35:37.000000 networklab-1.5.5.dev1/netsim/templates/provider/virtualbox/linux-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      321 2022-01-25 17:36:47.000000 networklab-1.5.5.dev1/netsim/templates/provider/virtualbox/nxos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      217 2021-04-11 18:37:32.000000 networklab-1.5.5.dev1/netsim/templates/provider/virtualbox/virtualbox-network.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      323 2021-04-11 18:37:32.000000 networklab-1.5.5.dev1/netsim/templates/provider/virtualbox/virtualbox-ports.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.897906 networklab-1.5.5.dev1/netsim/templates/tests/
+-rw-r--r--   0 pipi       (501) staff       (20)      255 2022-12-11 17:33:46.000000 networklab-1.5.5.dev1/netsim/templates/tests/clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      181 2022-12-11 09:54:53.000000 networklab-1.5.5.dev1/netsim/templates/tests/libvirt.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      185 2022-12-11 09:54:58.000000 networklab-1.5.5.dev1/netsim/templates/tests/virtualbox.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.899077 networklab-1.5.5.dev1/netsim/tools/
+-rw-r--r--   0 pipi       (501) staff       (20)      764 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/tools/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     5106 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/tools/graphite.py
+-rw-r--r--   0 pipi       (501) staff       (20)      614 2023-05-15 07:05:40.000000 networklab-1.5.5.dev1/netsim/tools/graphite.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.899276 networklab-1.5.5.dev1/netsim/tools/suzieq/
+-rw-r--r--   0 pipi       (501) staff       (20)      304 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/tools/suzieq/suzieq-cfg.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      643 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/tools/suzieq.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      542 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/netsim/topology-defaults.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.900815 networklab-1.5.5.dev1/netsim/utils/
+-rw-r--r--   0 pipi       (501) staff       (20)       78 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/netsim/utils/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2216 2023-07-27 05:43:15.000000 networklab-1.5.5.dev1/netsim/utils/files.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4079 2023-07-09 07:35:25.000000 networklab-1.5.5.dev1/netsim/utils/log.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3248 2023-04-02 11:32:00.000000 networklab-1.5.5.dev1/netsim/utils/status.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1784 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/utils/strings.py
+-rw-r--r--   0 pipi       (501) staff       (20)     5411 2023-07-09 07:35:01.000000 networklab-1.5.5.dev1/netsim/utils/templates.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.901889 networklab-1.5.5.dev1/networklab.egg-info/
+-rw-r--r--   0 pipi       (501) staff       (20)     3744 2023-07-27 10:49:01.000000 networklab-1.5.5.dev1/networklab.egg-info/PKG-INFO
+-rw-r--r--   0 pipi       (501) staff       (20)    21652 2023-07-27 10:49:01.000000 networklab-1.5.5.dev1/networklab.egg-info/SOURCES.txt
+-rw-r--r--   0 pipi       (501) staff       (20)        1 2023-07-27 10:49:01.000000 networklab-1.5.5.dev1/networklab.egg-info/dependency_links.txt
+-rw-r--r--   0 pipi       (501) staff       (20)       51 2023-07-27 10:49:01.000000 networklab-1.5.5.dev1/networklab.egg-info/entry_points.txt
+-rw-r--r--   0 pipi       (501) staff       (20)      120 2023-07-27 10:49:01.000000 networklab-1.5.5.dev1/networklab.egg-info/requires.txt
+-rw-r--r--   0 pipi       (501) staff       (20)        7 2023-07-27 10:49:01.000000 networklab-1.5.5.dev1/networklab.egg-info/top_level.txt
+-rw-r--r--   0 pipi       (501) staff       (20)      181 2023-04-27 06:49:41.000000 networklab-1.5.5.dev1/requirements.txt
+-rw-r--r--   0 pipi       (501) staff       (20)       38 2023-07-27 10:49:01.902729 networklab-1.5.5.dev1/setup.cfg
+-rw-r--r--   0 pipi       (501) staff       (20)     1477 2022-11-25 15:02:55.000000 networklab-1.5.5.dev1/setup.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 10:49:01.902046 networklab-1.5.5.dev1/tests/
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3462 2023-01-28 06:30:20.000000 networklab-1.5.5.dev1/tests/test_transformation.py
```

### Comparing `networklab-1.5.4.post1/LICENSE.md` & `networklab-1.5.5.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/PKG-INFO` & `networklab-1.5.5.dev1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.4.post1
+Version: 1.5.5.dev1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -37,32 +37,32 @@
 The latest release is [release 1.5.4](https://github.com/ipspace/netlab/releases/tag/release_1.5.4). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netlab.tools/release/) first.
 
 The latest release before the changes made in release 1.5.0 is [release 1.4.3](https://github.com/ipspace/netlab/releases/tag/release_1.4.3).
 
 ## An overview of tools:
 
 **netlab up**
-: Uses **netlab create** to create configuration files, starts the virtual lab, and uses **netlab initial** to deploy device configurations. [More details](https://netlab.tools/netlab/up/)
+: Uses **[netlab create](https://netlab.tools/netlab/create/)** to create configuration files, starts the virtual lab, and uses **[netlab initial](https://netlab.tools/netlab/initial/)** to deploy device configurations, including IP addressing, LLDP, OSPF, BGP, IS-IS, EIGRP, VRRP, VLANs, VRFs, MPLS, SR-MPLS, VXLAN, EVPN and SRv6. [More details](https://netlab.tools/netlab/up/)
 
 **netlab down**
 : Destroys the virtual lab. [More details](https://netlab.tools/netlab/down/)
 
 **netlab restart**
 : Restart and/or reconfigure the virtual lab. [More details](https://netlab.tools/netlab/restart/)
 
-**netlab create**
-: Creates a full-blown network topology, Vagrantfile and Ansible inventory from a simple list of nodes and links. [More details](https://netlab.tools/netlab/create/)
-
-**netlab initial**
-: Using topology data generated by **netlab create** and default device configuration templates configures common device parameters, protocols that should have been enabled (LLDP, OSPF, IS-IS, BGP, SR-MPLS), enables interfaces, and configures IP addresses on interfaces. [More details](https://netlab.tools/netlab/initial/)
-
 **netlab config**
-: Applies any Jinja2 configuration templates to network devices.
+: Applies additional Jinja2 configuration templates to network devices.
 
 **netlab collect**
 : Using Ansible fact gathering or other device-specific Ansible modules, collects device configurations and saves them in specified directory (default: **config**).
 
 **netlab connect**
 : Use SSH or **docker exec** to [connect to a lab device](https://netlab.tools/netlab/connect/) using device names, management network IP addresses (**ansible_host**), SSH port, and username/passwords specified in lab topology or *netlab* device defaults.
 
+**netlab report**
+: Creates a report from the transformed lab topology data.  [More details](https://netlab.tools/netlab/report/)
+
+**netlab graph**
+: Creates a lab topology graph description in Graphviz or D2 format. [More details](https://netlab.tools/netlab/graph/)
+
 **netlab show**
-: Display system settings in tabular format. [More details](https://netlab.tools/netlab/show/)
+: Display system settings in tabular, text, or YAML format. [More details](https://netlab.tools/netlab/show/)
```

### Comparing `networklab-1.5.4.post1/README.md` & `networklab-1.5.5.dev1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,32 +17,32 @@
 The latest release is [release 1.5.4](https://github.com/ipspace/netlab/releases/tag/release_1.5.4). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netlab.tools/release/) first.
 
 The latest release before the changes made in release 1.5.0 is [release 1.4.3](https://github.com/ipspace/netlab/releases/tag/release_1.4.3).
 
 ## An overview of tools:
 
 **netlab up**
-: Uses **netlab create** to create configuration files, starts the virtual lab, and uses **netlab initial** to deploy device configurations. [More details](https://netlab.tools/netlab/up/)
+: Uses **[netlab create](https://netlab.tools/netlab/create/)** to create configuration files, starts the virtual lab, and uses **[netlab initial](https://netlab.tools/netlab/initial/)** to deploy device configurations, including IP addressing, LLDP, OSPF, BGP, IS-IS, EIGRP, VRRP, VLANs, VRFs, MPLS, SR-MPLS, VXLAN, EVPN and SRv6. [More details](https://netlab.tools/netlab/up/)
 
 **netlab down**
 : Destroys the virtual lab. [More details](https://netlab.tools/netlab/down/)
 
 **netlab restart**
 : Restart and/or reconfigure the virtual lab. [More details](https://netlab.tools/netlab/restart/)
 
-**netlab create**
-: Creates a full-blown network topology, Vagrantfile and Ansible inventory from a simple list of nodes and links. [More details](https://netlab.tools/netlab/create/)
-
-**netlab initial**
-: Using topology data generated by **netlab create** and default device configuration templates configures common device parameters, protocols that should have been enabled (LLDP, OSPF, IS-IS, BGP, SR-MPLS), enables interfaces, and configures IP addresses on interfaces. [More details](https://netlab.tools/netlab/initial/)
-
 **netlab config**
-: Applies any Jinja2 configuration templates to network devices.
+: Applies additional Jinja2 configuration templates to network devices.
 
 **netlab collect**
 : Using Ansible fact gathering or other device-specific Ansible modules, collects device configurations and saves them in specified directory (default: **config**).
 
 **netlab connect**
 : Use SSH or **docker exec** to [connect to a lab device](https://netlab.tools/netlab/connect/) using device names, management network IP addresses (**ansible_host**), SSH port, and username/passwords specified in lab topology or *netlab* device defaults.
 
+**netlab report**
+: Creates a report from the transformed lab topology data.  [More details](https://netlab.tools/netlab/report/)
+
+**netlab graph**
+: Creates a lab topology graph description in Graphviz or D2 format. [More details](https://netlab.tools/netlab/graph/)
+
 **netlab show**
-: Display system settings in tabular format. [More details](https://netlab.tools/netlab/show/)
+: Display system settings in tabular, text, or YAML format. [More details](https://netlab.tools/netlab/show/)
```

### Comparing `networklab-1.5.4.post1/netsim/addressing.py` & `networklab-1.5.5.dev1/netsim/addressing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/collect-configs.ansible` & `networklab-1.5.5.dev1/netsim/ansible/collect-configs.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/config.ansible` & `networklab-1.5.5.dev1/netsim/ansible/config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/create-config.ansible` & `networklab-1.5.5.dev1/netsim/ansible/create-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/initial-config.ansible` & `networklab-1.5.5.dev1/netsim/ansible/initial-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/create-config.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/create-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/arubacx.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/cumulus.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/frr.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/linux-clab.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/linux-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/routeros.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/routeros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/srlinux.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/sros.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/vyos.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-config/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-custom-config.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-custom-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-module.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/deploy-module.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/srlinux.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/fetch-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/frr/deploy-config.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/frr/deploy-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/iosxr/initial.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/iosxr/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/linux/initial-clab.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/linux/initial-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/tasks/vmx/initial.yml` & `networklab-1.5.5.dev1/netsim/ansible/tasks/vmx/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bfd/arubacx.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bfd/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bfd/eos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bfd/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bfd/ios.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bfd/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bfd/nxos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bfd/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bfd/srlinux.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bfd/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bfd/sros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bfd/sros.j2`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                (l.ospf.bfd if 'ospf' in l and 'bfd' in l.ospf else False) %}
 {% set isis_bfd_v6 = l.isis.bfd.ipv6|default(False) if 'isis' in l and 'bfd' in l.isis else False %}
 {% if l.ipv4|default(False) and bfd_v4 %}
 - path: configure/router[router-name=Base]/interface[interface-name={{ifname}}]/ipv4/bfd
   val:
 {{ bfd_params( 'bfd' not in l or l.bfd ) }}
 {% endif %}
-{% if (l.ipv6|default(False) and isis_bfd_v6 %}
+{% if l.ipv6|default(False) and isis_bfd_v6 %}
 - path: configure/router[router-name=Base]/interface[interface-name={{ifname}}]/ipv6/bfd
   val:
 {{ bfd_params( 'bfd' not in l or l.bfd ) }}
 {% endif %}
 {% endmacro %}
 
 replace:
```

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/arubacx.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/arubacx.macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/arubacx.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/asa.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/asa.macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/asa.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/cumulus_nvue.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/dellos10.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/dellos10.macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/dellos10.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/eos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/eos.macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/eos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/frr.bgp-config.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/frr.bgp-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/ios.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/ios.macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/ios.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/iosxr.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/junos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/nxos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros.macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/routeros.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros7.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros7.macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/routeros7.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/srlinux.cli.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/srlinux.macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.md-cli.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.openconfig.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/vyos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/bgp/vyos.macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/bgp/vyos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/eigrp/ios.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/eigrp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/eigrp/nxos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/eigrp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/evpn/arubacx.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/evpn/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/evpn/cumulus.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/evpn/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/evpn/dellos10.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/evpn/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/evpn/eos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/evpn/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/evpn/frr.evpn-config.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/evpn/frr.evpn-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/evpn/nxos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/evpn/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/evpn/srlinux.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/evpn/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/evpn/sros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/evpn/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/evpn/vyos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/evpn/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/gateway/arubacx.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/gateway/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/gateway/cumulus.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/gateway/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/gateway/dellos10.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/gateway/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/gateway/eos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/gateway/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/gateway/ios.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/gateway/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/gateway/nxos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/gateway/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/gateway/srlinux.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/gateway/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/gateway/sros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/gateway/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/gateway/vyos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/gateway/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/arcos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/arcos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/arubacx.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/asa.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/cumulus.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/cumulus_nvue.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/dellos10.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/dellos10.vrf.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/dellos10.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/eos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/frr.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/ios.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/iosxr.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/junos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/junos.vlan.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/junos.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/junos.vrf.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/junos.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/hosts.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/ubuntu.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/linux/ubuntu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/vanilla.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/linux/vanilla.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/nxos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros.vlan.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/routeros.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros7.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros7.vlan.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/routeros7.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/srlinux.cli.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/srlinux.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/sros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/sros.md-cli.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/sros.openconfig.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/initial/vyos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/initial/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/isis/asa.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/isis/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/isis/eos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/isis/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/isis/frr.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/isis/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/isis/ios.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/isis/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/isis/iosxr.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/isis/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/isis/junos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/isis/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/isis/nxos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/isis/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/isis/srlinux.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/isis/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/isis/sros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/isis/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/isis/sros.openconfig.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/isis/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/isis/vyos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/isis/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.6pe.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/mpls/eos.6pe.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.bgp-lu.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/mpls/eos.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/mpls/frr.ldp.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/mpls/frr.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/mpls/ios.bgp-lu.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/mpls/ios.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/mpls/junos.ldp.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/mpls/junos.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/mpls/junos.mplsvpn.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/mpls/junos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/mpls/sros.ldp.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/mpls/sros.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus_nvue.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/eos.ospfv2.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/eos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/eos.ospfv3.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/eos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/frr.ospfv2.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/frr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/frr.ospfv3.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/frr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/ios.ospfv2.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/ios.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/ios.ospfv3.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/ios.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/junos.ospfv2.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/junos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/junos.ospfv3.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/junos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/nxos.ospfv2.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/nxos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/nxos.ospfv3.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/nxos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/routeros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/srlinux.cli.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/srlinux.macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/sros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/sros.j2`

 * *Files 20% similar despite different names*

```diff
@@ -3,32 +3,38 @@
 {% macro ospf_config(af,ospf,vrf_interfaces,include_system) %}
 {% set pid = ospf.process|default(0) %}
 {% set ospfv = 'ospf3' if af=='ipv6' else 'ospf' %}
 
 {% macro ospf_interface(l) %}
 {{ declare_router(l,sub_path="/"+ospfv+"[ospf-instance="+pid|string + "]") }}
   val:
-{% if ospf.reference_bandwidth is defined %}
+{%  if ospf.reference_bandwidth is defined %}
    reference-bandwidth: {{ ospf.reference_bandwidth * 1000 }} # in kbps
-{% endif %}
+{%  endif %}
    admin-state: enable
    area:
    - area-id: "{{ l.ospf.area }}"
      interface:
      - interface-name: "{{ if_name(l.ifname) }}"
-{% if l.ospf.passive|default(False) %}
+{%  if l.ospf.passive|default(False) %}
        passive: True
-{% endif %}
+{%  endif %}
 {%  if l.ospf.bfd|default(False) %}
-       bfd-liveness: { }
+       bfd-liveness: {% if not ospf.strict_bfd|default(False) %}{ }
+{%     else +%}
+        strict: True
+{%      if ospf.strict_bfd_delay|default(0) > 0 %}
+        strict-mode-holddown: {{ ospf.strict_bfd_delay }}
+{%      endif %}
+{%     endif %}
 {%  endif %}
        # mtu: 1500 # SRL defaults to 1500, now supporting global mtu settings
 {# TODO: Add support for multi-area adjacencies and 'secondary' interface-type #}
-{%  if l.ospf.network_type|default("") in ["broadcast","non-broadcast","point-to-point"] %}
-       interface-type: "{{ l.ospf.network_type }}"
+{%  if l.ospf.network_type|default("") in ["broadcast","non-broadcast","point-to-point","point-to-multipoint"] %}
+       interface-type: "{{ 'p2mp-nbma' if l.ospf.network_type=='point-to-multipoint' else l.ospf.network_type }}"
 {%  endif %}
 {%  if l.ospf.cost is defined %}
        metric: {{ l.ospf.cost }}
 {%  endif %}
 {% endmacro %}
 
 {% set system_if = { 'ifname': "system", 'ospf': { 'passive': True, 'area': ospf.area }, af: True } %}
```

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/sros.md-cli.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/sros.openconfig.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/vyos.ospfv2.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/vyos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/ospf/vyos.ospfv3.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/ospf/vyos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/sr/junos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/sr/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/sr/srlinux.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/sr/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/sr/sros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/sr/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/sr/sros.openconfig.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/sr/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/srv6/sros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/srv6/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vlan/arubacx.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vlan/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vlan/csr.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vlan/cumulus.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vlan/dellos10.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vlan/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vlan/eos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vlan/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vlan/frr.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vlan/nxos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vlan/routeros7.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vlan/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vlan/srlinux.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vlan/sros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vlan/vmx.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vlan/vmx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vlan/vptx.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vlan/vptx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vlan/vyos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.bgp.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/arubacx.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.bgp.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/dellos10.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.bgp-macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/eos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.bgp.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/eos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.bgp.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/frr.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.bgp-macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/ios.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.bgp.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/ios.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/junos.bgp.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/junos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/junos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/nxos.bgp.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/nxos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.bgp.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.bgp.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros7.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/srlinux.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/sros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.bgp.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/vyos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/csr.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/cumulus.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/frr.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/frr.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 #!/bin/bash
 #
 set -e # Exit immediately when any command fails
 #
 
+{% set use_evpn = vxlan.flooding|default('') == 'evpn' %}
+
 {% macro create_vxlan_interface(vni,br_name,vrf=None,mtu=1500) %}
 ip link add vxlan{{ vni }} type vxlan \
   id {{ vni }} \
   dstport 4789 \
-  local {{ vxlan.vtep }} {{ 'nolearning' if vxlan.flooding|default('') == 'evpn' else '' }}
+  local {{ vxlan.vtep }} {{ 'nolearning' if use_evpn else '' }}
 #
 # Add it to the VLAN bridge (create if needed for l3 vnis); disable STP
 if [ ! -e /sys/devices/virtual/net/{{ br_name}} ]; then
 brctl addbr {{ br_name }}
 ip link set up dev {{ br_name }}
 fi
 brctl addif {{ br_name }} vxlan{{ vni }}
 brctl stp {{ br_name }} off
-ip link set mtu {{ mtu }} dev vxlan{{ vni }}
+# Do not generate ipv6 link-local address for VXLAN devices
+ip link set mtu {{ mtu }} addrgenmode none dev vxlan{{ vni }}
+{% if use_evpn %}
+# Disable dynamic MAC learning for evpn, see https://docs.frrouting.org/en/latest/evpn.html
+bridge link set dev vxlan{{ vni }} learning off
+{% endif %}
 ip link set up dev vxlan{{ vni }}
 {% if vrf %}
 ip link set {{ br_name }} master {{ vrf }}
 {% endif %}
 {% endmacro %}
 
 # Determine max MTU used on interfaces, to configure VXLAN interface
```

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/nxos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/srlinux.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/sros.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/vyos.j2` & `networklab-1.5.5.dev1/netsim/ansible/templates/vxlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/api.py` & `networklab-1.5.5.dev1/netsim/api.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/augment/components.py` & `networklab-1.5.5.dev1/netsim/augment/components.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/augment/config.py` & `networklab-1.5.5.dev1/netsim/augment/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/augment/groups.py` & `networklab-1.5.5.dev1/netsim/augment/groups.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/augment/links.py` & `networklab-1.5.5.dev1/netsim/augment/links.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/augment/main.py` & `networklab-1.5.5.dev1/netsim/augment/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,28 @@
 from .. import addressing
 from .. import augment
 from .. import providers
 from .. import modules
 from .. import devices as quirks
 from ..data import global_vars
 
-def transform_setup(topology: Box) -> None:
+def topology_init(topology: Box) -> None:
   global_vars.init(topology)
   augment.config.attributes(topology)
+  augment.devices.augment_device_settings(topology)
+
+def transform_setup(topology: Box) -> None:
+  topology_init(topology)
   augment.topology.check_required_elements(topology)
   topology.nodes = augment.nodes.create_node_dict(topology.nodes)
   if 'links' in topology:
     augment.links.links_init(topology)
 
   augment.components.expand_components(topology)
 
-  augment.devices.augment_device_settings(topology)
   augment.plugin.init(topology)                                         # Initialize plugins very early on in case they modify extra attributes
   augment.plugin.execute('init',topology)
   augment.topology.check_tools(topology)
   common.exit_on_error()
 
   augment.topology.extend_attribute_list(topology.defaults)             # Attributes have to be extended before group init
   augment.topology.extend_module_attribute_list(topology)               # ... or we won't recognize node attributes in groups
```

### Comparing `networklab-1.5.4.post1/netsim/augment/nodes.py` & `networklab-1.5.5.dev1/netsim/augment/nodes.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/augment/plugin.py` & `networklab-1.5.5.dev1/netsim/augment/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 import typing
 import importlib
 import importlib.util
 
 from box import Box
 from .. import common
-from ..utils.templates import get_moddir
+from ..utils.files import get_moddir
 from .. import data
 
 def load_plugin_from_path(path: str, plugin: str) -> typing.Optional[object]:
   module_path = path+'/'+plugin
   if not os.path.exists(module_path):
     if os.path.exists(module_path+'.py'):
       module_path = module_path+'.py'
```

### Comparing `networklab-1.5.4.post1/netsim/augment/topology.py` & `networklab-1.5.5.dev1/netsim/augment/topology.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,13 +174,16 @@
 #
 
 def cleanup_topology(topology: Box) -> Box:
   topo_copy = Box(topology,box_dots=True)
 
   # Remove PFX generators from addressing section
   #
+  if not 'addressing' in topo_copy:
+    return topo_copy
+
   for k,v in topo_copy.addressing.items():
     for p in list(v.keys()):
       if "_pfx" in p or "_eui" in p:
         v.pop(p,None)
 
   return topo_copy
```

### Comparing `networklab-1.5.4.post1/netsim/callback.py` & `networklab-1.5.5.dev1/netsim/callback.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/cli/__init__.py` & `networklab-1.5.5.dev1/netsim/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
                   help='Verbose logging (add multiple flags for increased verbosity)')
   parser.add_argument('--warning', dest='warning', action='store_true',help=argparse.SUPPRESS)
   parser.add_argument('--raise_on_error', dest='raise_on_error', action='store_true',help=argparse.SUPPRESS)
   if debugging:
     parser.add_argument('--debug', dest='debug', action='store',nargs='*',
                     choices=[
                       'all','addr','cli','links','libvirt','modules','plugin','template',
-                      'vlan','vrf','quirks','validate','addressing','groups','quirks','status'
+                      'vlan','vrf','quirks','validate','addressing','groups','quirks','status',
+                      'external'
                     ],
                     help=argparse.SUPPRESS)
 
   return parser
 
 def topology_parse_args() -> argparse.ArgumentParser:
   parser = argparse.ArgumentParser(description='Common topology arguments',add_help=False)
@@ -142,15 +143,14 @@
     return None
 
   if isinstance(topology.message,str):                      # We have a single message
     return topology.message if default_message else None    # If the action is OK with getting the default message return it
 
   if not isinstance(topology.message,Box):                  # Otherwise we should be dealing with a dict
     common.fatal('topology message should be a string or a dict')
-    return None
 
   return topology.message.get(action,None)                  # Return action-specific message if it exists
 
 """
 lab_status_update -- generic lab status callback
 
 * Get the lab ID (or default)
@@ -229,30 +229,34 @@
     usage.run([])
     sys.exit()
 
   arg_start = 2
   mod = None
   cmd = sys.argv[1]
 
-  mod_path = os.path.dirname(__file__) + f"/{cmd}.py"
-  if not os.path.isfile(mod_path):
-    print("Unknown netlab command '%s'\nUse 'netlab usage' to get the list of valid commands" % cmd)
-    sys.exit(1)
+  if cmd in ['-h','--help']:
+    cmd = 'usage'
 
   if cmd == 'debug':
     arg_start = 3
+    cmd = sys.argv[2]
     mod = importlib.import_module("."+sys.argv[2],__name__)
   elif quick_commands.get(cmd,None):
     quick_commands[cmd](sys.argv[arg_start:])
     return
-  else:
-    try:
-      mod = importlib.import_module("."+cmd,__name__)
-    except Exception as ex:
-      common.fatal(f"Error importing {__name__}.{cmd}: {ex}")
+
+  mod_path = os.path.dirname(__file__) + f"/{cmd}.py"
+  if not os.path.isfile(mod_path):
+    print("Unknown netlab command '%s'\nUse 'netlab usage' to get the list of valid commands" % cmd)
+    sys.exit(1)
+
+  try:
+    mod = importlib.import_module("."+cmd,__name__)
+  except Exception as ex:
+    common.fatal(f"Error importing {__name__}.{cmd}: {ex}")
 
   if mod:
     if hasattr(mod,'run'):
       mod.run(sys.argv[arg_start:])   # type: ignore
       return
     else:
       common.fatal(f"Module {__name__}.{cmd} does not have a valid entry point")
```

### Comparing `networklab-1.5.4.post1/netsim/cli/ansible.py` & `networklab-1.5.5.dev1/netsim/cli/ansible.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,31 +30,27 @@
 def inventory(name: str) -> typing.Optional[dict]:
   try:
     result = subprocess.run(['ansible-inventory','--host',name],capture_output=True,check=True,text=True)
     try:
       return json.loads(result.stdout)
     except:
       common.fatal('Cannot parse JSON data returned by ansible-inventory','inventory')
-    return None
 
   except:
     try:
       subprocess.run(['ansible-inventory','-h'],capture_output=True,check=True)
     except Exception as ex:
       common.fatal(f'Cannot execute ansible-inventory command\n  {ex}','inventory')
 
     common.fatal('Cannot get Ansible inventory data for %s with ansible-inventory. Is the host name correct?' % name,'inventory')
 
-  return None
-
 def playbook(name: str, args: typing.List[str]) -> None:
   pbname = find_playbook(name)
   if not pbname:
     common.fatal("Cannot find Ansible playbook %s, aborting" % name)
-    return
 
   if common.VERBOSE:
     print("Running Ansible playbook %s" % pbname)
 
   cmd = ['ansible-playbook',pbname]
   cmd.extend(args)
```

### Comparing `networklab-1.5.4.post1/netsim/cli/clab.py` & `networklab-1.5.5.dev1/netsim/cli/clab.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import subprocess
 import shutil
 
 from box import Box
 
 from .. import common
 from .. import read_topology
+from ..utils import files as _files
 from . import external_commands
 from . import collect
 from . import fs_cleanup
 
 def tarball_parse(args: typing.List[str], settings: Box) -> argparse.Namespace:
   parser = argparse.ArgumentParser(
     prog='netlab clab tarball',
@@ -63,15 +64,14 @@
 
   return None
 
 def clab_config_adjust(infile: str, outfile: str, configs: str) -> None:
   clab = read_topology.read_yaml(infile)
   if not clab:
     common.fatal("Cannot read clab.yml configuration file, aborting")
-    return
 
   clab_yml = common.get_yaml_string(clab)
   if not ('topology' in clab and 'nodes' in clab.topology):
     common.fatal(f'Containerlab configuration file {infile} is weird: cannot find topology.nodes dictionary')
 
   try:
     cfglist = os.listdir(configs)
@@ -85,17 +85,15 @@
       print(f"Found config file for {n}: {cfgfile}")
       clab.topology.nodes[n]['startup-config'] = cfgfile
 
   final_clab_yml = common.get_yaml_string(clab) 
   if final_clab_yml == clab_yml:
     common.fatal(f'No relevant configuration files were found in {configs} directory, aborting')
 
-  output = common.open_output_file(outfile)
-  output.write(final_clab_yml)
-  output.close()
+  _files.create_file_from_text(outfile,final_clab_yml)
 
 def clab_tarball(cli_args: typing.List[str], settings: Box) -> None:
   args = tarball_parse(cli_args,settings)
 
   if not os.path.exists('clab.yml'):
     common.fatal('Containerlab configuration file clab.yml not found, aborting...')
 
@@ -126,13 +124,12 @@
   settings = read_topology.read_yaml('package:topology-defaults.yml')
   if not cli_args:
     clab_usage()
     return
 
   if not settings:
     common.fatal("Cannot read the system defaults","clab")
-    return
 
   if cli_args[0] == 'tarball':
     clab_tarball(cli_args[1:],settings)
   else:
     clab_usage()
```

### Comparing `networklab-1.5.4.post1/netsim/cli/collect.py` & `networklab-1.5.5.dev1/netsim/cli/collect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/cli/config.py` & `networklab-1.5.5.dev1/netsim/cli/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/cli/connect.py` & `networklab-1.5.5.dev1/netsim/cli/connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,8 +180,7 @@
   host = args.host
   if host in topology.nodes:
     connect_to_node(host,rest,topology,log_level)
   elif host in topology.tools:
     connect_to_tool(host,rest,topology,log_level)
   else:
     common.fatal(f'Unknown host or external tool {host}')
-    return
```

### Comparing `networklab-1.5.4.post1/netsim/cli/create.py` & `networklab-1.5.5.dev1/netsim/cli/create.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/cli/down.py` & `networklab-1.5.5.dev1/netsim/cli/down.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/cli/external_commands.py` & `networklab-1.5.5.dev1/netsim/cli/external_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 # Run external commands from netlab CLI
 #
 import typing
 import os
 import subprocess
 from box import Box
 
-from .. import common
 from . import is_dry_run
-from ..utils import strings
+from ..utils import strings,log
 
 def print_step(n: int, txt: str, spacing: typing.Optional[bool] = False) -> None:
   if spacing:
     print()
   print("Step %d: %s" % (n,txt))
   print("=" * 72)
 
@@ -31,35 +30,39 @@
 """
 def run_command(
     cmd : typing.Union[str,list],
     check_result : bool = False,
     ignore_errors: bool = False,
     return_stdout: bool = False) -> typing.Union[bool,str]:
 
-  if common.debug_active('cli'):
+  if log.debug_active('cli'):
     print(f"Not running: {cmd}")
     return True
 
   if is_dry_run():
     print(f"DRY RUN: {cmd}")
     return True
 
-  common.print_verbose(f"run_command executing: {cmd}")
+  if log.VERBOSE or log.debug_active('external'):
+    print(f"run_command executing: {cmd}")
+
   if isinstance(cmd,str):
     cmd = [ arg for arg in cmd.split(" ") if arg not in (""," ") ]
 
   try:
     result = subprocess.run(cmd,capture_output=check_result,check=True,text=True)
+    if log.debug_active('external'):
+      print(f'... run result: {result}')
     if not check_result:
       return True
     if return_stdout:
       return result.stdout
     return result.stdout != ""
   except Exception as ex:
-    if not common.QUIET and not ignore_errors:
+    if not log.QUIET and not ignore_errors:
       print( f"Error executing {stringify(cmd)}:\n  {ex}" )
     return False
 
 def test_probe(p : typing.Union[str,list,Box]) -> bool:
   if isinstance(p,str):
     return bool(run_command(p,check_result=True))
 
@@ -68,73 +71,73 @@
       if not test_probe(p_item):
         return False
     return True
 
   elif isinstance(p,Box):
     OK = bool(run_command(p.cmd,check_result=True,ignore_errors=True))
     if not OK:
-      common.fatal(p.err)
+      log.fatal(p.err)
     return OK
 
   else:
-    common.fatal(f"Internal error: invalid probe specification: {p}")
+    log.fatal(f"Internal error: invalid probe specification: {p}")
     return False
 
 def set_ansible_flags(cmd : list) -> list:
-  if common.VERBOSE:
-    cmd.append("-" + "v" * common.VERBOSE)
+  if log.VERBOSE:
+    cmd.append("-" + "v" * log.VERBOSE)
 
-  if common.QUIET:
+  if log.QUIET:
     os.environ["ANSIBLE_STDOUT_CALLBACK"] = "selective"
 
   return cmd
 
 def run_probes(settings: Box, provider: str, step: int = 0) -> None:
   if step:
     print_step(step,f"Checking virtualization provider installation: {provider}",spacing = True)
-  elif common.VERBOSE:
+  elif log.VERBOSE:
     print("Checking virtualization provider installation")
   for p in settings.providers[provider].probe:
     if not test_probe(p):
-      common.fatal("%s failed, aborting" % p)
-  if common.VERBOSE or step and not is_dry_run():
+      log.fatal("%s failed, aborting" % p)
+  if log.VERBOSE or step and not is_dry_run():
     print(".. all tests succeeded, moving on\n")
 
 def start_lab(settings: Box, provider: str, step: int = 2, cli_command: str = "test", exec_command: typing.Optional[str] = None) -> None:
   if exec_command is None:
     exec_command = settings.providers[provider].start
   print_step(step,f"starting the lab -- {provider}: {exec_command}")
   if not run_command(exec_command):
-    common.fatal(f"{exec_command} failed, aborting...",cli_command)
+    log.fatal(f"{exec_command} failed, aborting...",cli_command)
 
 def deploy_configs(step : int = 3, command: str = "test", fast: typing.Optional[bool] = False) -> None:
   print_step(step,"deploying initial device configurations",spacing = True)
   cmd = ["netlab","initial"]
-  if common.VERBOSE:
-    cmd.append("-" + "v" * common.VERBOSE)
+  if log.VERBOSE:
+    cmd.append("-" + "v" * log.VERBOSE)
 
   if os.environ.get('NETLAB_FAST_CONFIG',None) or fast:
     cmd.append("--fast")
 
   if not run_command(set_ansible_flags(cmd)):
-    common.fatal("netlab initial failed, aborting...",command)
+    log.fatal("netlab initial failed, aborting...",command)
 
 def custom_configs(config : str, group: str, step : int = 4, command: str = "test") -> None:
   print_step(step,"deploying custom configuration template %s for group %s" % (config,group))
   cmd = ["netlab","config",config,"--limit",group]
 
   if not run_command(set_ansible_flags(cmd)):
-    common.fatal("netlab config failed, aborting...",command)
+    log.fatal("netlab config failed, aborting...",command)
 
 def stop_lab(settings: Box, provider: str, step: int = 4, command: str = "test", exec_command: typing.Optional[str] = None) -> None:
   print_step(step,f"stopping the lab: {provider}",True)
   if exec_command is None:
     exec_command = settings.providers[provider].stop
   if not run_command(exec_command):
-    common.fatal(f"{exec_command} failed, aborting...",command)
+    log.fatal(f"{exec_command} failed, aborting...",command)
 
 """
 Get a runtime-related parameter for a tool
 """
 def get_tool_runtime_param(tool: str, param: str, verbose: bool, topology: Box) -> typing.Optional[typing.Any]:
   tdata = topology.defaults.tools[tool] + topology.tools[tool]
   runtime = tdata.runtime or 'docker'
```

### Comparing `networklab-1.5.4.post1/netsim/cli/initial.py` & `networklab-1.5.5.dev1/netsim/cli/initial.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/cli/install.py` & `networklab-1.5.5.dev1/netsim/cli/install.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     help='Run the specified installation script')
 
   return parser.parse_args(args)
 
 def run(cli_args: typing.List[str]) -> None:
   if not cli_args:
     common.fatal("Specify an installation script to run or use -h to get help","install")
-    return
 
   args = install_parse(cli_args)
 
   moddir = Path(__file__).resolve().parent.parent
   env = { key:value for (key,value) in os.environ.items() }
   if args.verbose:
     env['FLAG_APT'] = '-V'
```

### Comparing `networklab-1.5.4.post1/netsim/cli/libvirt.py` & `networklab-1.5.5.dev1/netsim/cli/libvirt.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 import shutil
 import sys
 
 from box import Box
 
 from .. import common
 from .. import read_topology
-from ..utils import strings,status
+from ..utils import strings,status,templates,log
 from . import external_commands
 from ..providers.libvirt import create_vagrant_network,LIBVIRT_MANAGEMENT_NETWORK_NAME
+from ..utils import files as _files
 
 def package_parse(args: typing.List[str], settings: Box) -> argparse.Namespace:
   devs = [ k for k in settings.devices.keys() if settings.devices[k].libvirt.create or settings.devices[k].libvirt.create_template ]
   parser = argparse.ArgumentParser(
     prog='netlab libvirt package',
     description='Package a virtual machine into a libvirt Vagrant box')
   parser.add_argument(
@@ -96,30 +97,30 @@
     pass
 
 def lp_preinstall_hook(args: argparse.Namespace,settings: Box) -> None:
   devdata = settings.devices[args.device]
   if not 'pre_install' in devdata.libvirt:
     return
   print("Running pre-install hooks")
-  pre_inst_script = common.get_moddir() / "install/libvirt" / devdata.libvirt.pre_install / "run.sh"
+  pre_inst_script = _files.get_moddir() / "install/libvirt" / devdata.libvirt.pre_install / "run.sh"
 
   if not os.access(pre_inst_script, os.X_OK):
     print(" - run file not executable - skipping.")
     return
 
   abort_on_failure(pre_inst_script)
   print("... done\n")
 
 def lp_create_bootstrap_iso(args: argparse.Namespace,settings: Box) -> None:
   devdata = settings.devices[args.device]
   if not 'create_iso' in devdata.libvirt:
     return
   print("Creating bootstrap ISO image")
 
-  isodir = common.get_moddir() / "install/libvirt" / devdata.libvirt.create_iso
+  isodir = _files.get_moddir() / "install/libvirt" / devdata.libvirt.create_iso
   shutil.rmtree('iso',ignore_errors=True)
   shutil.copytree(isodir,'iso')
   if os.path.exists('bootstrap.iso'):
     os.remove('bootstrap.iso')
 
   abort_on_failure("mkisofs -l --iso-level 4 -o bootstrap.iso iso")
   print("... done\n")
@@ -137,25 +138,35 @@
 
 """)
   if devdata.libvirt.create:
     cmd = devdata.libvirt.create.replace("\n","")
     abort_on_failure(cmd)
   elif devdata.libvirt.create_template:
     data = get_template_data(devdata)
-    template = common.template(devdata.libvirt.create_template,data,"install/libvirt",)
+    tname = devdata.libvirt.create_template
+    try:
+      template = templates.render_template(
+                  j2_file=tname,
+                  data=data,
+                  path="install/libvirt")
+    except Exception as ex:
+      log.fatal(
+        text=f"Error rendering {tname}\n{strings.extra_data_printout(str(ex))}",
+        module='libvirt')
+
     pathlib.Path("template.xml").write_text(template)
     abort_on_failure("virsh define template.xml")
     abort_on_failure("virsh start --console vm_box")
 
   vm_cleanup('vm_box')
 
 def lp_create_box(args: argparse.Namespace,settings: Box) -> None:
-  with open("metadata.json","w") as metadata:
-    metadata.write('{"provider":"libvirt","format":"qcow2","virtual_size":4}\n')
-    metadata.close()
+  _files.create_file_from_text(
+    fname="metadata.json",
+    txt='{"provider":"libvirt","format":"qcow2","virtual_size":4}\n')
   print("Downloading vagrant-libvirt create_box.sh script")
   abort_on_failure('curl -O https://raw.githubusercontent.com/vagrant-libvirt/vagrant-libvirt/master/tools/create_box.sh')
 
   boxfile = f"{args.device}.box"
   if os.path.isfile(boxfile):
     print(f"Removing old {boxfile}")
     os.remove(boxfile)
@@ -208,17 +219,21 @@
         }
       ]
     }
   ]
 }
 """)
   print("Creating box metadata in box.json")
-  with open("box.json","w") as metadata:
-    metadata.write(json.substitute(boxname=boxname,description=description,version=version,device=args.device,path=os.getcwd()))
-    metadata.close()
+  _files.create_file_from_text(
+    fname="box.json",
+    txt=json.substitute(
+      boxname=boxname,
+      description=description,
+      version=version,
+      device=args.device,path=os.getcwd()))
   print("""
 
 Importing Vagrant box
 =====================
 """)
   if not external_commands.run_command("vagrant box add box.json"):
     print("""
@@ -266,15 +281,15 @@
   if not 'vm' in skip:
     lp_create_vm(args,settings)
   stop_vagrant_network()
   if not 'box' in skip:
     lp_create_box(args,settings)
 
 def config_parse(args: typing.List[str], settings: Box) -> argparse.Namespace:
-  moddir = common.get_moddir()
+  moddir = _files.get_moddir()
   devs = map(
     lambda x: pathlib.Path(x).stem,
     glob.glob(str(moddir / "install/libvirt/*txt")))
   parser = argparse.ArgumentParser(
     prog='netlab libvirt config',
     description='Display Vagrant network device box configuration guidelines')
   parser.add_argument(
@@ -282,25 +297,24 @@
     action='store',
     choices=list(devs),
     help='Network device you want to create')
   return parser.parse_args(args)
 
 def libvirt_config(cli_args: typing.List[str], settings: Box) -> None:
   args = config_parse(cli_args,settings)
-  helpfile = common.get_moddir() / "install/libvirt" / (args.device+".txt")
+  helpfile = _files.get_moddir() / "install/libvirt" / (args.device+".txt")
   print(helpfile.read_text())
 
 def libvirt_usage() -> None:
   print("Usage: netlab libvirt package|config --help")
 
 def run(cli_args: typing.List[str]) -> None:
   topology = read_topology.load("package:cli/empty.yml","","package:topology-defaults.yml")
   if not topology:
     common.fatal("Cannot read the system defaults","libvirt")
-    return
 
   if not cli_args:
     libvirt_usage()
     return
 
   if cli_args[0] == 'package':
     libvirt_package(cli_args[1:],topology)
```

### Comparing `networklab-1.5.4.post1/netsim/cli/read.py` & `networklab-1.5.5.dev1/netsim/cli/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/cli/restart.py` & `networklab-1.5.5.dev1/netsim/cli/restart.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/cli/status.py` & `networklab-1.5.5.dev1/netsim/cli/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,8 +153,7 @@
   lab_states = status.read_status(topology)
   args = status_parse(cli_args)
   common.set_logging_flags(args)
   if args.action in action_map:
     action_map[args.action](topology,args,lab_states)
   else:
     common.fatal(f'Unknown action {args.action}')
-    return
```

### Comparing `networklab-1.5.4.post1/netsim/cli/test.py` & `networklab-1.5.5.dev1/netsim/cli/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,19 +84,17 @@
   if args.verbose:
     print("... done, test completed\n")
 
 def run(cli_args: typing.List[str]) -> None:
   settings = read_topology.read_yaml('package:topology-defaults.yml')
   if not cli_args:
     common.fatal("Specify the virtualization environment to test or use -h to get help","test")
-    return
 
   if not settings:
     common.fatal("Cannot read the global defaults","test")
-    return
 
   args = test_parse(cli_args,settings)
   if os.path.exists(args.workdir):
     common.fatal("Directory %s already exists, aborting" % args.workdir,"test")
 
   if args.verbose:
     utils.log.set_logging_flags(args)
```

### Comparing `networklab-1.5.4.post1/netsim/cli/up.py` & `networklab-1.5.5.dev1/netsim/cli/up.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,21 @@
 import typing
 import argparse
 import os
 
 from box import Box
 from pathlib import Path
 
-from .. import common
 from . import create
 from . import external_commands, set_dry_run, is_dry_run
 from . import common_parse_args, get_message
 from . import lab_status_update, lab_status_change, get_lab_id
 from .. import providers
 from .. import read_topology
-from ..utils import status
+from ..utils import status,log
 
 #
 # Extra arguments for 'netlab up' command
 #
 def up_parse_args(standalone: bool) -> argparse.ArgumentParser:
   parse_parents = [ common_parse_args() ] if standalone else []
   parser = argparse.ArgumentParser(
@@ -63,20 +62,19 @@
 Get lab topology from the snapshot file or run the transformation process
 """
 def get_topology(args: argparse.Namespace, cli_args: typing.List[str]) -> Box:
   up_args_parser = up_parse_args(bool(args.snapshot))         # (re)create the correct parser
 
   if args.snapshot:                                           # If we're using the snapshot file...
     args = up_args_parser.parse_args(cli_args)                # ... and reparse
-    common.set_logging_flags(args)                            # ... use these arguments to set logging flags and read the snapshot
+    log.set_logging_flags(args)                               # ... use these arguments to set logging flags and read the snapshot
 
     topology = read_topology.read_yaml(filename=args.snapshot)
     if topology is None:
-      common.fatal(f'Cannot read snapshot file {args.snapshot}, aborting...')
-      return Box({})                                          # pragma: no-cover
+      log.fatal(f'Cannot read snapshot file {args.snapshot}, aborting...')
 
     print(f"Using transformed lab topology from snapshot file {args.snapshot}")
   else:                                                       # No snapshot file, use 'netlab create' parser
     topology = create.run(cli_args,'up','Create configuration files, start a virtual lab, and configure it',up_args_parser)
 
   return topology
 
@@ -131,15 +129,15 @@
 
 Otherwise use 'netlab status' to check the status of labs running on this machine, or
 'netlab down' to shut down the other lab running in this directory.
 
 If you are sure that no other lab is running in this directory, remove the
 netlab.lock file manually and retry.
 ''')
-  common.fatal('Cannot start another lab in the same directory')
+  log.fatal('Cannot start another lab in the same directory')
 
 """
 check_lab_instance -- print an error message if the lab instance is already running in a different directory
 """
 def check_lab_instance(topology: Box) -> None:
   lab_id = get_lab_id(topology)                   # Get the current lab instance ID from lab topology
   lab_states = status.read_status(topology)       # Read the state of existing lab instances
@@ -156,15 +154,15 @@
 
 Please use 'netlab status' to check the status of labs running on this machine.
 You can stop the other lab instance with 'netlab status cleanup {lab_id}'.
 
 If you think your netlab status file is corrupt, use 'netlab status reset' to
 delete it.
 ''')
-  common.fatal(f'aborting "netlab up" request')
+  log.fatal(f'aborting "netlab up" request')
 
 """
 Execute provider probes
 """
 def provider_probes(topology: Box, step: int = 2) -> None:
   p_provider = topology.provider
 
@@ -189,15 +187,18 @@
   if sname is not None:
     exec_command = topology.defaults.providers[pname][sname].start
   else:
     exec_command = topology.defaults.providers[pname].start
 
   exec_list = exec_command if isinstance(exec_command,list) else [ exec_command ]
   for cmd in exec_list:
-    external_commands.start_lab(topology.defaults,sname or pname,3,"netlab up",cmd)
+    print(f"provider {p_name}: executing {cmd}")
+    if not external_commands.run_command(cmd):
+      log.fatal(f"{cmd} failed, aborting...","netlab up")
+
   p_module.call('post_start_lab',p_topology)
 
   lab_status_change(topology,f'{p_name} workload started')
 
 """
 Recreate secondary configuration file
 """
@@ -211,37 +212,37 @@
   filename = sp_data.filename                                         # Get the secondary configuration filename
   print(f"Recreating {filename} configuration file for {s_provider} provider")
   sp_module.create(s_topology,filename)                               # ... and create the new configuration file
 
 """
 Deploy initial configuration
 """
-def deploy_initial_config(args: argparse.Namespace, topology: Box) -> None:
+def deploy_initial_config(args: argparse.Namespace, topology: Box, step: int) -> None:
   if args.no_config:
     print("\nInitial configuration skipped, run 'netlab initial' to configure the devices")
     return
 
   lab_status_change(topology,f'deploying initial configuration')
-  external_commands.deploy_configs(4,"netlab up",args.fast_config)
+  external_commands.deploy_configs(step,"netlab up",args.fast_config)
   message = get_message(topology,'up',False)
   if message:
     print(f"\n\n{message}")
   lab_status_change(topology,f'initial configuration complete')
 
 """
 Deploy external tools
 """
-def start_external_tools(args: argparse.Namespace, topology: Box) -> None:
+def start_external_tools(args: argparse.Namespace, topology: Box, step: int) -> None:
   if not 'tools' in topology:
     return
   if args.no_tools:
     print("\nExternal tools not started, start them manually")
     return
 
-  print ("\nStarting external tools...")
+  external_commands.print_step(step,f"Starting external tools")
   lab_status_change(topology,f'starting external tools')
   for tool in topology.tools.keys():
     cmds = external_commands.get_tool_command(tool,'up',topology)
     if cmds is None:
       continue
     external_commands.execute_tool_commands(cmds,topology)
     msg = external_commands.get_tool_message(tool,topology)
@@ -264,34 +265,37 @@
     check_existing_lab()
 
   topology = get_topology(args,cli_args)
   if not is_dry_run():
     check_lab_instance(topology)
 
   settings = topology.defaults
-  if common.QUIET:
+  if log.QUIET:
     os.environ["ANSIBLE_STDOUT_CALLBACK"] = "selective"
 
   provider_probes(topology)
 
   p_provider = topology.provider
   p_module = providers._Provider.load(p_provider,topology.defaults.providers[p_provider])
   providers.mark_providers(topology)
   p_module.call('pre_output_transform',topology)
 
   status_start_lab(topology)
   if 'err_conflict' in topology.defaults:
-    common.fatal(f'race condition, lab instance already running in {topology.defaults.err_conflict}')
-    return
+    log.fatal(f'race condition, lab instance already running in {topology.defaults.err_conflict}')
 
   if not is_dry_run():
     status.lock_directory()
 
+  step = 3
+  external_commands.print_step(step,f"Starting the lab: {p_provider}")
   start_provider_lab(topology,p_provider)
+
   for s_provider in topology[p_provider].providers:
-    print()
+    step += 1
+    external_commands.print_step(step,f"Starting the lab: {s_provider}",spacing=True)
     recreate_secondary_config(topology,p_provider,s_provider)
     start_provider_lab(topology,p_provider,s_provider)
 
-  deploy_initial_config(args,topology)
-  start_external_tools(args,topology)
+  deploy_initial_config(args,topology,step+1)
+  start_external_tools(args,topology,step+2)
   lab_status_change(topology,'started')
```

### Comparing `networklab-1.5.4.post1/netsim/cli/usage.txt` & `networklab-1.5.5.dev1/netsim/cli/usage.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,68 @@
 Usage:
 
     netlab <command> <parameters>
 
-High-level commands
-===================
+Creating the lab
+================
 
 up          Create virtualization provider and network automation configuration
             files, start the virtual lab, and deploy initial device configurations
 
-down        Destroy the virtual lab
-
-restart     Restart the lab (netlab down followed by netlab up) using the
-            transformed lab topology in the netlab snapshot file
-
-Topology manipulation commands
-==============================
-
 create      Create virtualization provider and network automation configuration
             file. Assuming you're using Vagrant and Ansible, it creates
             Vagrantfile, hosts.yml and ansible.cfg. This command can also be
             used to create graph specifications or output transformed topology 
             in YAML or JSON format.
 
+restart     Restart the lab (netlab down followed by netlab up) using the
+            transformed lab topology in the netlab snapshot file
+
+Configuring and Controlling the Lab
+===================================
+
+connect     Connect to network devices using SSH or 'docker exec'
+
+collect     Collect device configurations from network devices and save them in
+            specified directory
+
+down        Destroy the virtual lab
+
+Reports and graphs
+==================
+status      Display the state of lab instances running on the current server
+
+report      Create a report based on transfomed lab topology data
+
+graph       Create a graph description in Graphviz or D2 format
+
+inspect     Helps you inspect data structures in transformed lab topology
+
+show        Display system settings
+
 Device configuration commands
 =============================
-
 initial     Runs initial-config Ansible playbook to deploy initial- and module-
             specific configurations to network devices, or to create a directory
             with initial device configurations
 
-connect     Connect to network devices using SSH or 'docker exec'
-
 config      Use a custom configuration template to configure network devices
 
-collect     Collect device configurations from network devices and save them in
-            specified directory
-
 Notes:
 * Device configuration commands require Ansible version 2.9 or higher
 
-Convenience commands
-====================
+Installation commands
+=====================
 
 install     Runs installation scripts to install nice-to-have Ubuntu software,
             Ansible and vagrant/libvirt
+
 test        Tests libvirt or VirtualBox installation by building a 3-router
             virtual lab using Cumulus VX
-alias       Create aliases for old netsim-tools CLI commands
-read        Read network topology data and output the results
-            (used mostly for troubleshooting)
+
+libvirt     Build Vagrant boxes for vagrant-libvirt provider
+
 version     Prints the version of netlab package
+
+Provider-specific commands
+==========================
+clab        containerlab utilities
```

### Comparing `networklab-1.5.4.post1/netsim/data/__init__.py` & `networklab-1.5.5.dev1/netsim/data/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,32 +23,23 @@
   for k in d.keys():
     if isinstance(d[k],dict):
       null_to_string(d[k])
     elif d[k] is None:
       d[k] = ""
 
 #
-# Safe get from a hierarchical dictionary (won't create new objects)
+# Recursively remove null values from a box
 #
 
-def get_from_box(b: Box, selector: typing.Union[str,typing.List[str]], partial: bool = False) -> typing.Optional[typing.Any]:
-  print('WARNING: get_from_box is deprecated, please fix your plugins')
-  if isinstance(selector,str):
-    selector = selector.split('.')
-
-  for idx,k in enumerate(selector):
-    if not k in b:
-      return b if partial and idx > 0 else None   # return partial result if request assuming we got at least one match before
-
-    if not isinstance(b[k],dict):                                       # we are at a leaf node
-      return b[k] if partial or idx == len(selector) - 1 else None      # ... return the value if we're at the end of
-                                                                        # ... the chain or accept partial lookup
-    b = b[k]
-
-  return b
+def remove_null_values(d: Box) -> None:
+  for k in list(d.keys()):                                  # Iterate over box keys
+    if d[k] is None:
+      d.pop(k)                                              # Remove null values
+    elif isinstance(d[k],Box):
+      remove_null_values(d[k])                              # ... and recurse into child boxes
 
 #
 # Get a global setting or corresponding system default. Use for attributes that are not propagated or early in the
 # transformation logic when the module attributes haven't been propagated yet
 #
 # Use 'get_global_parameter' to get a single value and 'get_global_settings' to get a merged dictionary of
 # default and topology settings
```

### Comparing `networklab-1.5.4.post1/netsim/data/filemaps.py` & `networklab-1.5.5.dev1/netsim/data/filemaps.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/data/global_vars.py` & `networklab-1.5.5.dev1/netsim/data/global_vars.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/data/types.py` & `networklab-1.5.5.dev1/netsim/data/types.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/data/validate.py` & `networklab-1.5.5.dev1/netsim/data/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/defaults/attributes.yml` & `networklab-1.5.5.dev1/netsim/defaults/attributes.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/__init__.py` & `networklab-1.5.5.dev1/netsim/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/arubacx.py` & `networklab-1.5.5.dev1/netsim/devices/arubacx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/arubacx.yml` & `networklab-1.5.5.dev1/netsim/devices/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/asav.py` & `networklab-1.5.5.dev1/netsim/devices/asav.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/asav.yml` & `networklab-1.5.5.dev1/netsim/devices/asav.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/csr.yml` & `networklab-1.5.5.dev1/netsim/devices/dellos10.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,46 @@
-description: Cisco CSR 1000v
-interface_name: GigabitEthernet{ifindex}
-loopback_interface_name: Loopback{ifindex}
-tunnel_interface_name: Tunnel{ifindex}
-ifindex_offset: 2
-virtualbox:
-  image: cisco/csr1000v
-group_vars:
-  ansible_user: vagrant
-  ansible_ssh_pass: vagrant
-  ansible_become_method: enable
-  ansible_become_password: vagrant
-  ansible_network_os: ios
-  ansible_connection: network_cli
-  netlab_device_type: csr
-node:
-  min_mtu: 1500
+description: Dell OS10
+interface_name: ethernet1/1/{ifindex}
+mgmt_if: mgmt1/1/1
+loopback_interface_name: loopback{ifindex}
 features:
-  bgp:
-    local_as: True
-    vrf_local_as: True
-    local_as_ibgp: True
-    activate_af: True
   initial:
     ipv4:
       unnumbered: True
     ipv6:
       lla: True
-  ospf:
-    unnumbered: True
-  isis:
-    unnumbered:
-      ipv4: True
-      ipv6: True
-      network: True
-  mpls:
-    ldp: True
-    bgp: True
-    vpn: True
-    6pe: True
+  bgp:
+    local_as: True
+    vrf_local_as: True
+    activate_af: True
+    ipv6_lla: True
+    rfc8950: True
   vlan:
     model: switch
-    svi_interface_name: BDI{vlan}
+    svi_interface_name: virtual-network{vlan}
+  evpn:
+    irb: True
+    asymmetrical_irb: True
   gateway:
-    protocol: [ vrrp ]
+    protocol: [ anycast, vrrp ]
+clab:
+  image: vrnetlab/vr-ftosv
+  node:
+    kind: vr-ftosv
+  interface:
+    name: eth{ifindex}
 libvirt:
-  image: cisco/csr1000v
+  image: dell/os10
   create:
-    virt-install --connect=qemu:///system --name=vm_box --os-variant=rhel4.0 --arch=x86_64 --cpu host --vcpus=1 --hvm
-      --ram=4096 --disk path=vm.qcow2,bus=ide,format=qcow2 --network=network:vagrant-libvirt,model=virtio --graphics none --import
+    virt-install --connect=qemu:///system --name=vm_box --arch=x86_64 --cpu host --vcpus=2 --hvm
+      --ram=2048 --network=network:vagrant-libvirt,model=virtio --graphics none --import
+      --disk path=vm.qcow2,format=qcow2,bus=sata
+      --disk path=hdb_OS10-installer.qcow2,format=qcow2,bus=virtio
+      --disk path=hdc_OS10-platform.qcow2,format=qcow2,bus=virtio
+group_vars:
+  ansible_network_os: dellos10
+  ansible_connection: network_cli
+  ansible_user: vagrant
+  ansible_ssh_pass: vagrant
 external:
   image: none
-graphite.icon: router
+graphite.icon: switch
```

### Comparing `networklab-1.5.4.post1/netsim/devices/cumulus.yml` & `networklab-1.5.5.dev1/netsim/devices/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/cumulus_nvue.yml` & `networklab-1.5.5.dev1/netsim/devices/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/dellos10.yml` & `networklab-1.5.5.dev1/netsim/devices/iosxr.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,38 @@
-description: Dell OS10
-interface_name: ethernet1/1/{ifindex}
-mgmt_if: mgmt1/1/1
-loopback_interface_name: loopback{ifindex}
+description: Cisco IOS XRv
+mgmt_if: MgmtEth0/RP0/CPU0/0
+interface_name: GigabitEthernet0/0/0/{ifindex}
+ifindex_offset: 0
+group_vars:
+  ansible_user: vagrant
+  ansible_ssh_pass: vagrant
+  ansible_become_method: enable
+  ansible_become_password: vagrant
+  ansible_network_os: iosxr
+  ansible_connection: network_cli
 features:
   initial:
     ipv4:
       unnumbered: True
     ipv6:
       lla: True
+  ospf:
+    unnumbered: True
+  isis:
+    unnumbered:
+      ipv4: True
+      ipv6: True
+      network: True
   bgp:
-    local_as: True
-    vrf_local_as: True
     activate_af: True
-    ipv6_lla: True
-    rfc8950: True
-  vlan:
-    model: switch
-    svi_interface_name: virtual-network{vlan}
-  evpn:
-    irb: True
-    asymmetrical_irb: True
-  gateway:
-    protocol: [ anycast, vrrp ]
-clab:
-  image: vrnetlab/vr-ftosv
-  node:
-    kind: vr-ftosv
-  interface:
-    name: eth{ifindex}
-libvirt:
-  image: dell/os10
-  create:
-    virt-install --connect=qemu:///system --name=vm_box --arch=x86_64 --cpu host --vcpus=2 --hvm
-      --ram=2048 --network=network:vagrant-libvirt,model=virtio --graphics none --import
-      --disk path=vm.qcow2,format=qcow2,bus=sata
-      --disk path=hdb_OS10-installer.qcow2,format=qcow2,bus=virtio
-      --disk path=hdc_OS10-platform.qcow2,format=qcow2,bus=virtio
-group_vars:
-  ansible_network_os: dellos10
-  ansible_connection: network_cli
-  ansible_user: vagrant
-  ansible_ssh_pass: vagrant
 external:
   image: none
-graphite.icon: switch
+libvirt:
+  image: cisco/iosxr
+  create:
+    virt-install --connect=qemu:///system --network network=vagrant-libvirt,model=e1000 --name=vm_box
+      --cpu host --arch=x86_64 --vcpus=2 --ram=8192
+      --virt-type=kvm
+      --disk path=vm.qcow2,format=qcow2,device=disk,bus=ide
+      --graphics none --import
+##      create_iso: iosxr
+##          --disk path=bootstrap.iso,format=iso,device=cdrom
```

### Comparing `networklab-1.5.4.post1/netsim/devices/eos.py` & `networklab-1.5.5.dev1/netsim/devices/eos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/eos.yml` & `networklab-1.5.5.dev1/netsim/devices/iosv.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,59 @@
-description: Arista vEOS VM or cEOS container
-interface_name: Ethernet{ifindex}
-mgmt_if: Management1
+description: Cisco IOSv
+interface_name: GigabitEthernet0/{ifindex}
 loopback_interface_name: Loopback{ifindex}
 tunnel_interface_name: Tunnel{ifindex}
-virtualbox:
-  image: arista/veos
 group_vars:
   ansible_user: vagrant
   ansible_ssh_pass: vagrant
-  ansible_network_os: eos
+  ansible_become_method: enable
+  ansible_become_password: vagrant
+  ansible_network_os: ios
   ansible_connection: network_cli
+  netlab_device_type: ios
+libvirt:
+  image: cisco/iosv
+  create_template: iosv.xml.j2
+#      create:
+#        virt-install --connect=qemu:///system --name=vm_box --os-type=linux --arch=x86_64 --cpu host --vcpus=1
+#          --noacpi --machine=pc-1.0 --virt-type=kvm --watchdog i6300esb,action=reset --ram=512
+#          --disk path=vm.qcow2,bus=virtio,format=qcow2,cache=writethrough
+#          --network=network:vagrant-libvirt,model=e1000 --graphics none --import
+virtualbox:
+  image: cisco/iosv
 features:
+  bfd: true
   bgp:
-    local_as: True
-    vrf_local_as: True
-    local_as_ibgp: True
-    activate_af: True
+    local_as: true
+    vrf_local_as: true
+    local_as_ibgp: true
+    activate_af: true
   initial:
-    system_mtu: True
     ipv4:
-      unnumbered: True
+      unnumbered: false
     ipv6:
-      lla: True
+      lla: true
   ospf:
-    unnumbered: True
+    unnumbered: true
   isis:
     unnumbered:
-      ipv4: True
-      ipv6: True
-      network: True
+      ipv4: true
+      ipv6: true
+      network: true
+  eigrp: true
   mpls:
-    ldp: True
-    bgp: True
-    vpn: True
-    6pe: True
+    ldp: true
+    bgp: true
+    vpn: true
+    6pe: true
   vlan:
-    model: l3-switch
-    svi_interface_name: Vlan{vlan}
+    model: router
+    svi_interface_name: BVI{bvi}
     subif_name: "{ifname}.{subif_index}"
-    native_routed: True
-  evpn:
-    irb: True
-    asymmetrical_irb: True
-    bundle: [ vlan_aware ]
+    mixed_trunk: true
+    native_routed: true
+  vrf: true
   gateway:
-    protocol: [ anycast, vrrp ]
-clab:
-  interface:
-    name: et{ifindex}
-  node:
-    kind: ceos
-    env:
-      INTFTYPE: et
-  mgmt_if: Management0
-  image: ceos:4.26.4M
-  group_vars:
-    ansible_user: admin
-    ansible_ssh_pass: admin
-    ansible_become: yes
-    ansible_become_method: enable
-libvirt:
-  image: arista/veos
-  create_template: eos.xml.j2
-#      create: |
-#        virt-install --connect=qemu:///system --name=vm_box --os-type=linux --arch=x86_64 --cpu host --vcpus=2 --hvm
-#          --ram=2048 --disk path=vm.qcow2,bus=ide,format=qcow2 --network=network:vagrant-libvirt,model=virtio --graphics none --import
+    protocol: [ vrrp ]
 external:
   image: none
-graphite.icon: switch
+graphite.icon: router
```

### Comparing `networklab-1.5.4.post1/netsim/devices/frr.yml` & `networklab-1.5.5.dev1/netsim/devices/frr.yml`

 * *Files 15% similar despite different names*

```diff
@@ -29,30 +29,34 @@
     ansible_user: vagrant
     ansible_ssh_pass: vagrant
 external:
   image: none
 features:
   initial:
     ipv4:
-      unnumbered: True
+      unnumbered: true
     ipv6:
-      lla: True
+      lla: true
+  bgp:
+    activate_af: true
+    ipv6_lla: true
+    local_as: true
+    rfc8950: true
+    vrf_local_as: true
+  evpn:
+    irb: true
+  isis: true
+  mpls:
+    ldp: true
+    vpn: true
+  ospf: true
   vlan:
+    mixed_trunk: true
     model: router
-    svi_interface_name: "vlan{vlan}"
-    subif_name: "{ifname}.{vlan.access_id}"
-    mixed_trunk: True
-    native_routed: True
-  evpn:
-    irb: True
+    native_routed: true
+    subif_name: '{ifname}.{vlan.access_id}'
+    svi_interface_name: vlan{vlan}
   vrf:
-    keep_module: True # Don't remove vrf module even if no interfaces are associated with any vrfs
-  bgp:
-    activate_af: True
-    ipv6_lla: True
-    rfc8950: True
-    local_as: True
-    vrf_local_as: True
-  mpls:
-    ldp: True
-    vpn: True
+    keep_module: true
+  vxlan: true
+
 graphite.icon: router
```

### Comparing `networklab-1.5.4.post1/netsim/devices/iosv.py` & `networklab-1.5.5.dev1/netsim/devices/iosv.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/iosv.yml` & `networklab-1.5.5.dev1/netsim/devices/none.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-description: Cisco IOSv
-interface_name: GigabitEthernet0/{ifindex}
+description: Dummy device used to test topology transformation
+#
+# Most features are enabled on the dummy device -- this file is a pretty
+# good template if you want to figure out what device features there are.
+#
+interface_name: eth{ifindex}
 loopback_interface_name: Loopback{ifindex}
 tunnel_interface_name: Tunnel{ifindex}
-group_vars:
-  ansible_user: vagrant
-  ansible_ssh_pass: vagrant
-  ansible_become_method: enable
-  ansible_become_password: vagrant
-  ansible_network_os: ios
-  ansible_connection: network_cli
-  netlab_device_type: ios
-libvirt:
-  image: cisco/iosv
-  create_template: iosv.xml.j2
-#      create:
-#        virt-install --connect=qemu:///system --name=vm_box --os-type=linux --arch=x86_64 --cpu host --vcpus=1
-#          --noacpi --machine=pc-1.0 --virt-type=kvm --watchdog i6300esb,action=reset --ram=512
-#          --disk path=vm.qcow2,bus=virtio,format=qcow2,cache=writethrough
-#          --network=network:vagrant-libvirt,model=e1000 --graphics none --import
 virtualbox:
-  image: cisco/iosv
+  image: none
+libvirt:
+  image: none
+clab:
+  image: none
+external:
+  image: none
+group_vars:
+  ansible_connection: paramiko_ssh
+  ansible_network_os: none
 features:
   bgp:
     local_as: True
     vrf_local_as: True
     local_as_ibgp: True
     activate_af: True
+    ipv6_lla: True
+    rfc8950: True
   initial:
     ipv4:
-      unnumbered: False
+      unnumbered: True
     ipv6:
       lla: True
   ospf:
     unnumbered: True
   isis:
     unnumbered:
       ipv4: True
       ipv6: True
       network: True
   mpls:
     ldp: True
     bgp: True
     vpn: True
     6pe: True
+  evpn:
+    irb: True
+    asymmetrical_irb: True
+    bundle: [ vlan_aware ]
+  gateway:
+    protocol: [ anycast, vrrp ]
   vlan:
-    model: router
-    svi_interface_name: BVI{bvi}
-    subif_name: "{ifname}.{subif_index}"
+    model: l3-switch
+    svi_interface_name: Vlan{vlan}
+    subif_name: "{ifname}.{vlan.access_id}"
     mixed_trunk: True
     native_routed: True
-  gateway:
-    protocol: [ vrrp ]
-external:
-  image: none
-graphite.icon: router
```

### Comparing `networklab-1.5.4.post1/netsim/devices/iosxr.yml` & `networklab-1.5.5.dev1/netsim/devices/vsrx.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,53 @@
-description: Cisco IOS XRv
-mgmt_if: MgmtEth0/RP0/CPU0/0
-interface_name: GigabitEthernet0/0/0/{ifindex}
+description: Juniper vSRX 3.0
+interface_name: ge-0/0/{ifindex}
+loopback_interface_name: "lo0.{ifindex}"
 ifindex_offset: 0
+mgmt_if: fxp0
+virtualbox:
+  image: juniper/vsrx3
 group_vars:
   ansible_user: vagrant
-  ansible_ssh_pass: vagrant
-  ansible_become_method: enable
-  ansible_become_password: vagrant
-  ansible_network_os: iosxr
-  ansible_connection: network_cli
+  ansible_ssh_pass: Vagrant
+  ansible_network_os: junos
+  ansible_connection: netconf
+  netlab_console_connection: ssh
+  netlab_device_type: vsrx
 features:
   initial:
     ipv4:
       unnumbered: True
     ipv6:
       lla: True
   ospf:
     unnumbered: True
   isis:
     unnumbered:
       ipv4: True
       ipv6: True
-      network: True
-  bgp:
-    activate_af: True
-external:
-  image: none
+  vlan:
+    model: router
+    subif_name: "{ifname}.{vlan.access_id}"
+    mixed_trunk: False
+    native_routed: True
+  mpls:
+    ldp: True
+    vpn: True
 libvirt:
-  image: cisco/iosxr
+  image: juniper/vsrx3
+  create_iso: vsrx
   create:
-    virt-install --connect=qemu:///system --network network=vagrant-libvirt,model=e1000 --name=vm_box
-      --cpu host --arch=x86_64 --vcpus=2 --ram=8192
-      --virt-type=kvm
-      --disk path=vm.qcow2,format=qcow2,device=disk,bus=ide
-      --graphics none --import
-##      create_iso: iosxr
-##          --disk path=bootstrap.iso,format=iso,device=cdrom
+    virt-install --connect=qemu:///system --name=vm_box --os-variant=freebsd10.0 --arch=x86_64 --cpu host --vcpus=2 --hvm
+      --ram=4096 --disk path=vm.qcow2,bus=ide,format=qcow2 --disk path=bootstrap.iso,device=cdrom,bus=ide
+      --boot hd --network=network:vagrant-libvirt,model=virtio --graphics none --import
+clab:
+  image: vrnetlab/vr-vsrx:23.1R1.8
+  node:
+    kind: vr-vsrx
+  interface:
+    name: eth{ifindex+1}
+  group_vars:
+    ansible_user: admin
+    ansible_ssh_pass: "admin@123"
+external:
+  image: none
+graphite.icon: firewall
```

### Comparing `networklab-1.5.4.post1/netsim/devices/junos.py` & `networklab-1.5.5.dev1/netsim/devices/junos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/linux.yml` & `networklab-1.5.5.dev1/netsim/devices/linux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/none.yml` & `networklab-1.5.5.dev1/netsim/devices/eos.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,74 @@
-description: Dummy device used to test topology transformation
-#
-# Most features are enabled on the dummy device -- this file is a pretty
-# good template if you want to figure out what device features there are.
-#
-interface_name: eth{ifindex}
+description: Arista vEOS VM or cEOS container
+interface_name: Ethernet{ifindex}
+mgmt_if: Management1
 loopback_interface_name: Loopback{ifindex}
 tunnel_interface_name: Tunnel{ifindex}
 virtualbox:
-  image: none
-libvirt:
-  image: none
-clab:
-  image: none
-external:
-  image: none
+  image: arista/veos
 group_vars:
-  ansible_connection: paramiko_ssh
-  ansible_network_os: none
+  ansible_user: vagrant
+  ansible_ssh_pass: vagrant
+  ansible_network_os: eos
+  ansible_connection: network_cli
 features:
-  bgp:
-    local_as: True
-    vrf_local_as: True
-    local_as_ibgp: True
-    activate_af: True
-    ipv6_lla: True
-    rfc8950: True
   initial:
+    system_mtu: true
     ipv4:
-      unnumbered: True
+      unnumbered: true
     ipv6:
-      lla: True
-  ospf:
-    unnumbered: True
-  isis:
-    unnumbered:
-      ipv4: True
-      ipv6: True
-      network: True
-  mpls:
-    ldp: True
-    bgp: True
-    vpn: True
-    6pe: True
+      lla: true
+  bfd: true
+  bgp:
+    activate_af: true
+    local_as: true
+    local_as_ibgp: true
+    vrf_local_as: true
   evpn:
-    irb: True
-    asymmetrical_irb: True
+    asymmetrical_irb: true
     bundle: [ vlan_aware ]
+    irb: true
   gateway:
     protocol: [ anycast, vrrp ]
+  isis:
+    unnumbered:
+      ipv4: true
+      ipv6: true
+      network: true
+  mpls:
+    6pe: true
+    bgp: true
+    ldp: true
+    vpn: true
+  ospf:
+    unnumbered: true
+  sr: true
   vlan:
     model: l3-switch
+    native_routed: true
+    subif_name: '{ifname}.{subif_index}'
     svi_interface_name: Vlan{vlan}
-    subif_name: "{ifname}.{vlan.access_id}"
-    mixed_trunk: True
-    native_routed: True
+  vrf: true
+  vxlan: true
+clab:
+  interface:
+    name: et{ifindex}
+  node:
+    kind: ceos
+    env:
+      INTFTYPE: et
+  mgmt_if: Management0
+  image: ceos:4.26.4M
+  group_vars:
+    ansible_user: admin
+    ansible_ssh_pass: admin
+    ansible_become: yes
+    ansible_become_method: enable
+libvirt:
+  image: arista/veos
+  create_template: eos.xml.j2
+#      create: |
+#        virt-install --connect=qemu:///system --name=vm_box --os-type=linux --arch=x86_64 --cpu host --vcpus=2 --hvm
+#          --ram=2048 --disk path=vm.qcow2,bus=ide,format=qcow2 --network=network:vagrant-libvirt,model=virtio --graphics none --import
+external:
+  image: none
+graphite.icon: switch
```

### Comparing `networklab-1.5.4.post1/netsim/devices/nxos.yml` & `networklab-1.5.5.dev1/netsim/devices/nxos.yml`

 * *Files 11% similar despite different names*

```diff
@@ -11,31 +11,37 @@
   ansible_connection: network_cli
 bfd:           # NXOS requires lower default timer values
   min_rx: 500
 evpn._start_transit_vlan: 3800
 features:
   initial:
     ipv4:
-      unnumbered: True
+      unnumbered: true
     ipv6:
-      lla: True
-  ospf:
-    unnumbered: True
+      lla: true
+  bfd: true
+  bgp: true
+  eigrp: true
+  evpn:
+    irb: true
+  gateway:
+    protocol: [ vrrp ]
   isis:
     unnumbered:
-      ipv4: True
-      ipv6: True
+      ipv4: true
+      ipv6: true
+  ospf:
+    unnumbered: true
   vlan:
     model: l3-switch
+    native_routed: true
+    subif_name: '{ifname}.{subif_index}'
     svi_interface_name: vlan{vlan}
-    subif_name: "{ifname}.{subif_index}"
-    native_routed: True
-  evpn:
-    irb: True
-  gateway:
-    protocol: [ vrrp ]
+  vrf: true
+  vxlan: true
+
 libvirt:
   create_template: nxos.xml.j2
   image: cisco/nexus9300v
 external:
   image: none
 graphite.icon: nexus5000
```

### Comparing `networklab-1.5.4.post1/netsim/devices/routeros7.yml` & `networklab-1.5.5.dev1/netsim/devices/routeros7.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/srlinux.yml` & `networklab-1.5.5.dev1/netsim/devices/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/sros.yml` & `networklab-1.5.5.dev1/netsim/devices/sros.yml`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
   initial:
     ipv4:
       unnumbered: True
     ipv6:
       lla: True
   ospf:
     unnumbered: True
+    strict_bfd: True # RFC9355 support
   isis:
     unnumbered:
       ipv4: True
       ipv6: True
       network: False # SROS treats the interfaces as point-to-point and forms at most 1 adjacency
   bgp:
     local_as: True
```

### Comparing `networklab-1.5.4.post1/netsim/devices/unknown.py` & `networklab-1.5.5.dev1/netsim/devices/unknown.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/vmx.py` & `networklab-1.5.5.dev1/netsim/devices/vmx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/vmx.yml` & `networklab-1.5.5.dev1/netsim/devices/vmx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/vptx.py` & `networklab-1.5.5.dev1/netsim/devices/vptx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/vptx.yml` & `networklab-1.5.5.dev1/netsim/devices/vptx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/vsrx.py` & `networklab-1.5.5.dev1/netsim/devices/vsrx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/devices/vsrx.yml` & `networklab-1.5.5.dev1/netsim/devices/vyos.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,52 @@
-description: Juniper vSRX 3.0
-interface_name: ge-0/0/{ifindex}
-loopback_interface_name: "lo0.{ifindex}"
-ifindex_offset: 0
-mgmt_if: fxp0
-virtualbox:
-  image: juniper/vsrx3
+description: Vyatta VyOS VM/container
+interface_name: eth{ifindex}
+loopback_interface_name: "dum{ifindex}"
+mgmt_if: eth0
+libvirt:
+  image: vyos/current
 group_vars:
-  ansible_user: vagrant
-  ansible_ssh_pass: Vagrant
-  ansible_network_os: junos
-  ansible_connection: netconf
-  netlab_console_connection: ssh
-  netlab_device_type: vsrx
+  ansible_network_os: vyos
+  ansible_connection: paramiko
+  ansible_user: vyos
+  ansible_ssh_pass: vyos
+  docker_shell: su - vyos
 features:
   initial:
     ipv4:
       unnumbered: True
     ipv6:
       lla: True
   ospf:
     unnumbered: True
-  isis:
-    unnumbered:
-      ipv4: True
-      ipv6: True
-  vlan:
-    model: router
-    subif_name: "{ifname}.{vlan.access_id}"
-    mixed_trunk: False
-    native_routed: True
+  bgp:
+    local_as: True
+    vrf_local_as: True
+    activate_af: True
+    ipv6_lla: True
+    rfc8950: True
   mpls:
     ldp: True
     vpn: True
-libvirt:
-  image: juniper/vsrx3
-  create_iso: vsrx
-  create:
-    virt-install --connect=qemu:///system --name=vm_box --os-variant=freebsd10.0 --arch=x86_64 --cpu host --vcpus=2 --hvm
-      --ram=4096 --disk path=vm.qcow2,bus=ide,format=qcow2 --disk path=bootstrap.iso,device=cdrom,bus=ide
-      --boot hd --network=network:vagrant-libvirt,model=virtio --graphics none --import
+  vlan:
+    model: l3-switch
+    svi_interface_name: "br0.{vlan}"
+    subif_name: "{ifname}.{vlan.access_id}"
+    native_routed: True
+  evpn:
+    irb: True
+    asymmetrical_irb: True
+  gateway:
+    protocol: [ vrrp ]
 clab:
-  image: vrnetlab/vr-vsrx:23.1R1.8
+  image: ghcr.io/sysoleg/vyos-container
+  mtu: 1500
   node:
-    kind: vr-vsrx
-  interface:
-    name: eth{ifindex+1}
+    kind: linux
+    binds:
+      '/lib/modules': '/lib/modules'
   group_vars:
-    ansible_user: admin
-    ansible_ssh_pass: "admin@123"
+    ansible_connection: docker
+    ansible_user: vyos
 external:
   image: none
-graphite.icon: firewall
+graphite.icon: router
```

### Comparing `networklab-1.5.4.post1/netsim/extra/ebgp.utils/default-originate.yml` & `networklab-1.5.5.dev1/netsim/extra/ebgp.utils/default-originate.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/extra/ebgp.utils/eos.j2` & `networklab-1.5.5.dev1/netsim/extra/ebgp.utils/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/extra/ebgp.utils/frr.j2` & `networklab-1.5.5.dev1/netsim/extra/ebgp.utils/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/extra/ebgp.utils/ios.j2` & `networklab-1.5.5.dev1/netsim/extra/ebgp.utils/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/extra/ebgp.utils/junos.j2` & `networklab-1.5.5.dev1/netsim/extra/ebgp.utils/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/extra/ebgp.utils/plugin.py` & `networklab-1.5.5.dev1/netsim/extra/ebgp.utils/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/extra/ebgp.utils/routeros7.j2` & `networklab-1.5.5.dev1/netsim/extra/ebgp.utils/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/extra/ebgp.utils/srlinux.j2` & `networklab-1.5.5.dev1/netsim/extra/ebgp.utils/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/extra/ebgp.utils/vyos.j2` & `networklab-1.5.5.dev1/netsim/extra/ebgp.utils/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/extra/multilab/plugin.py` & `networklab-1.5.5.dev1/netsim/extra/multilab/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/extra/proxy-arp/plugin.py` & `networklab-1.5.5.dev1/netsim/extra/proxy-arp/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/extra/proxy-arp/srlinux.j2` & `networklab-1.5.5.dev1/netsim/extra/proxy-arp/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/extra/proxy-arp/sros.j2` & `networklab-1.5.5.dev1/netsim/extra/proxy-arp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/ansible.sh` & `networklab-1.5.5.dev1/netsim/install/ansible.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/containerlab.sh` & `networklab-1.5.5.dev1/netsim/install/containerlab.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/grpc.sh` & `networklab-1.5.5.dev1/netsim/install/grpc.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/arubacx.txt` & `networklab-1.5.5.dev1/netsim/install/libvirt/arubacx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/asav/day0-config` & `networklab-1.5.5.dev1/netsim/install/libvirt/asav/day0-config`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/csr.txt` & `networklab-1.5.5.dev1/netsim/install/libvirt/csr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/dellos10.txt` & `networklab-1.5.5.dev1/netsim/install/libvirt/dellos10.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/eos.txt` & `networklab-1.5.5.dev1/netsim/install/libvirt/eos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/eos.xml.j2` & `networklab-1.5.5.dev1/netsim/install/libvirt/eos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/iosv.txt` & `networklab-1.5.5.dev1/netsim/install/libvirt/iosv.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/iosv.xml.j2` & `networklab-1.5.5.dev1/netsim/install/libvirt/iosv.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/iosxr.txt` & `networklab-1.5.5.dev1/netsim/install/libvirt/iosxr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/nxos.txt` & `networklab-1.5.5.dev1/netsim/install/libvirt/nxos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/nxos.xml.j2` & `networklab-1.5.5.dev1/netsim/install/libvirt/nxos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/routeros7.txt` & `networklab-1.5.5.dev1/netsim/install/libvirt/routeros7.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/vptx/juniper.conf` & `networklab-1.5.5.dev1/netsim/install/libvirt/vptx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/vptx/make-config.sh` & `networklab-1.5.5.dev1/netsim/install/libvirt/vptx/make-config.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/vptx/run.sh` & `networklab-1.5.5.dev1/netsim/install/libvirt/vptx/run.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/vptx.txt` & `networklab-1.5.5.dev1/netsim/install/libvirt/vptx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/vptx.xml.j2` & `networklab-1.5.5.dev1/netsim/install/libvirt/vptx.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/vsrx/juniper.conf` & `networklab-1.5.5.dev1/netsim/install/libvirt/vsrx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt/vsrx.txt` & `networklab-1.5.5.dev1/netsim/install/libvirt/vsrx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/libvirt.sh` & `networklab-1.5.5.dev1/netsim/install/libvirt.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/install/ubuntu.sh` & `networklab-1.5.5.dev1/netsim/install/ubuntu.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/modules/__init__.py` & `networklab-1.5.5.dev1/netsim/modules/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 from .. import common,data
 from ..data.validate import must_be_list
 from ..callback import Callback
 from ..augment import devices
 
 # List of attributes we don't want propagated from defaults to global/node
 #
-no_propagate_list = ["attributes","extra_attributes","requires","supported_on","no_propagate","config_after","transform_after"]
+no_propagate_list = [
+  "attributes","extra_attributes","features",
+  "requires","supported_on","no_propagate",
+  "config_after","transform_after"]
 
 """
 Return the authoritative list of all modules.
 
 A module is a top-level 'defaults' dictionary key if the value is a dictionary with 'supported_on' key
 """
 def list_of_modules(topology: Box) -> list:
```

### Comparing `networklab-1.5.4.post1/netsim/modules/_dataplane.py` & `networklab-1.5.5.dev1/netsim/modules/_dataplane.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/modules/_routing.py` & `networklab-1.5.5.dev1/netsim/modules/_routing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/modules/bfd.py` & `networklab-1.5.5.dev1/netsim/modules/bfd.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/modules/bfd.yml` & `networklab-1.5.5.dev1/netsim/modules/bfd.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # BFD (RFC 5880) default settings and attributes
 #
-supported_on: [ srlinux, sros, iosv, csr, nxos, eos, vyos, arubacx, none ]
+# Also supported on: eos, csr, iosv
+#
+supported_on: [ srlinux, sros, nxos, vyos, arubacx, none ]
 min_echo_rx: 0      # Echo function, 0=disabled by default
 multiplier: 3       # Detection time multiplier, number of packets lost before down
 attributes:
   global:
     min_tx: { type: int, min_value: 1 }
     min_rx: { type: int, min_value: 1 }
     min_echo_rx: { type: int, min_value: 0 }
```

### Comparing `networklab-1.5.4.post1/netsim/modules/bgp.py` & `networklab-1.5.5.dev1/netsim/modules/bgp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/modules/bgp.yml` & `networklab-1.5.5.dev1/netsim/modules/bgp.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # BGP default settings and attributes
 #
-supported_on: [ cumulus, cumulus_nvue, eos, frr, csr, iosv, nxos, asav, vsrx, vyos, routeros,
+# Also supported on: eos, csr, frr, iosv, nxos
+#
+supported_on: [ cumulus, cumulus_nvue, asav, vsrx, vyos, routeros,
   srlinux, sros, none, dellos10, routeros7, vmx, iosxr, arubacx, vptx, none ]
 ebgp_role: external
 advertise_roles: [ stub ]
 advertise_loopback: True
 community:
   ibgp: [ standard, extended ]
   ebgp: [ standard ]
@@ -46,16 +48,23 @@
     originate: list
     advertise_loopback:
     sessions:
     activate:
     community:
     router_id: { type: ipv4, use: id }
     local_as: asn
-    replace_global_as: bool [
+    replace_global_as: bool
   vrf:
     router_id: { type: ipv4, use: id }
   node_copy: [ local_as, replace_global_as ]
   link:
     advertise: bool
   interface:
     local_as: asn
     replace_global_as: bool
+features:
+  local_as: Supports local-as functionality
+  vrf_local_as: Supports local-as within a VRF
+  local_as_ibgp: Can use local-as to create IBGP sesssion
+  activate_af: Can control activation of individual address families
+  ipv6_lla: Can run EBGP sessions over IPv6 link-local addresses
+  rfc8950: Can run IPv4 AF over IPv6 LLA EBGP session
```

### Comparing `networklab-1.5.4.post1/netsim/modules/evpn.py` & `networklab-1.5.5.dev1/netsim/modules/evpn.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/modules/gateway.py` & `networklab-1.5.5.dev1/netsim/modules/gateway.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/modules/gateway.yml` & `networklab-1.5.5.dev1/netsim/modules/gateway.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Gateway (FHRP) default settings and attributes
 #
-supported_on: [ none, eos, cumulus, iosv, csr, nxos, sros, srlinux, vyos, dellos10, arubacx ]
+# Also supported on: eos, csr, nxos, iosv
+#
+supported_on: [ none, cumulus, sros, srlinux, vyos, dellos10, arubacx ]
 transform_after: [ vlan, vrf, ospf, isis, eigrp ]
 config_after: [ vlan,vrf ]
 id: -2
 protocol: anycast
 anycast:
   mac: 0200.cafe.00ff
   unicast: True
@@ -38,7 +40,9 @@
       unicast: bool
       mac: mac
     vrrp:
       group: int
       priority: int
       preempt: bool
   link_to_neighbor: True
+features:
+  protocol: Supported FHRP protocols
```

### Comparing `networklab-1.5.4.post1/netsim/modules/isis.py` & `networklab-1.5.5.dev1/netsim/modules/isis.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/modules/isis.yml` & `networklab-1.5.5.dev1/netsim/modules/isis.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # ISIS default settings and attributes
 #
-supported_on: [ eos, frr, csr, iosv, nxos, asav, vsrx, srlinux, sros, vyos, vmx, iosxr, vptx, none ]
+# Also supported on csr, eos, frr, iosv, nxos
+#
+supported_on: [ asav, vsrx, srlinux, sros, vyos, vmx, iosxr, vptx, none ]
 area: "49.0001"
 type: level-2
 transform_after: [ vlan,vrf ]
 config_after: [ vlan ]
 attributes:
   global:
     af:
@@ -30,7 +32,12 @@
     type: { type: str, valid_values: [ level-1 ,level-2, level-1-2 ] }
     bfd:
       ipv4: bool
       ipv6: bool
       _alt_types: [ bool ]
     network_type: { type: str, valid_values: [ point-to-point ] }
     passive: bool
+features:
+  unnumbered:
+    ipv4: IPv4 unnumbered interfaces
+    ipv6: IPv6 unnumbered interfaces
+    network: multi-access unnumbered links
```

### Comparing `networklab-1.5.4.post1/netsim/modules/mpls.py` & `networklab-1.5.5.dev1/netsim/modules/mpls.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/modules/ospf.py` & `networklab-1.5.5.dev1/netsim/modules/ospf.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,15 +54,34 @@
 
 class OSPF(_Module):
 
   def node_post_transform(self, node: Box, topology: Box) -> None:
     features = devices.get_device_features(node,topology.defaults)
 
     _routing.router_id(node,'ospf',topology.pools)
+    
+    # If strict BFD is requested, check if the node supports it
+    if isinstance(node.get('ospf.bfd',None),Box) and node.get('ospf.bfd.strict',False):
+      if features.get('ospf.strict_bfd',False):
+        if 'bfd' in node.get('module',[]):
+          node.ospf.strict_bfd = True
+          node.ospf.strict_bfd_delay = node.get('ospf.bfd.strict_delay',0)
+        else:
+          common.error(
+            f'{node.name} uses strict BFD with OSPF without enabling the "bfd" module',
+            common.IncorrectValue,
+            'ospf')
+      else:
+        common.error(
+          f'{node.name} uses strict BFD with OSPF which is not supported by {node.device} device',
+          common.IncorrectValue,
+          'ospf')
+
     bfd.bfd_link_state(node,'ospf')
+
     #
     # Cleanup routing protocol from external/disabled interfaces
     for intf in node.get('interfaces',[]):
       if not _routing.external(intf,'ospf'):                # Remove external interfaces from OSPF process
         _routing.passive(intf,'ospf')                       # Set passive flag on other OSPF interfaces
         err = _routing.network_type(intf,'ospf',['point-to-point','point-to-multipoint','broadcast','non-broadcast'])
         if err:
```

### Comparing `networklab-1.5.4.post1/netsim/modules/ospf.yml` & `networklab-1.5.5.dev1/netsim/modules/ospf.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # OSPFv2/OSPFv3 default settings and attributes
 #
+# Also supported on csr, eos, frr, iosv, nxos
+#
 area: 0.0.0.0
 supported_on: [
-  arcos, cumulus, cumulus_nvue, eos, fortios, frr, csr, iosv, nxos, vsrx, vyos, routeros,
+  arcos, cumulus, cumulus_nvue, fortios, vsrx, vyos, routeros,
   srlinux, sros, dellos10, routeros7, vmx, iosxr, arubacx, vptx, none ]
 transform_after: [ vlan,vrf ]
 config_after: [ vlan ]
 attributes:
   global:
     af:
       _list_to_dict: True
@@ -15,14 +17,16 @@
       ipv6: bool
     area: { type: ipv4, use: id }
     process: { type: int, min_value: 1 }
     reference_bandwidth: { type: int, min_value: 1 }
     bfd:
       ipv4: bool
       ipv6: bool
+      strict: bool                                              # Support RFC9355
+      strict_delay: { type: int, min_value: 0, max_value: 600 } # optional delay in seconds
       _alt_types: [ bool ]
   node:
     af:
     area:
     process:
     reference_bandwidth:
     bfd:
@@ -34,7 +38,10 @@
     router_id: { type: ipv4, use: id }
   link:
     cost: { type: int, min_value: 1, max_value: 65534 }
     area: { type: ipv4, use: id }
     bfd: bool
     passive: bool
     network_type: { type: str, valid_values: [ point-to-point,point-to-multipoint,broadcast,non-broadcast ] }
+features:
+  unnumbered: Can run OSPFv2 over unnumbered IPv4 interfaces
+  strict_bfd: Supports strict BFD mode (RFC 9355)
```

### Comparing `networklab-1.5.4.post1/netsim/modules/srv6.py` & `networklab-1.5.5.dev1/netsim/modules/srv6.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/modules/vlan.py` & `networklab-1.5.5.dev1/netsim/modules/vlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/modules/vlan.yml` & `networklab-1.5.5.dev1/netsim/modules/vlan.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # VLAN default settings and attributes
 #
-supported_on: [ eos, iosv, csr, vyos, dellos10, srlinux, none, routeros, nxos, frr, cumulus, sros, routeros7, vmx, vsrx, arubacx, vptx, none ]
+# Also supported on csr, eos, frr, iosv, nxos
+#
+supported_on: [ vyos, dellos10, srlinux, none, routeros, cumulus, sros, routeros7, vmx, vsrx, arubacx, vptx, none ]
 no_propagate: [ start_vlan_id, mode ]
 start_vlan_id: 1000
 mode: irb
 attributes:
   global:
     mode: { type: str, valid_values: [ bridge, irb, route] }
   node:
@@ -26,7 +28,11 @@
   phy_ifattr: [ bridge, ifindex, parentindex, ifname, linkindex, type, vlan, mtu, _selfloop_ifindex ]
   #
   # Keep these subinterface attributes
   keep_subif: [ vlan, ifindex, ifname, type ]
   extra:
     global: [ vlans ]
     node: [ vlans ]
+features:
+  model: Conceptual device configuration model
+  mixed_trunk: Supports trunk interfaces with mixed routed/bridged VLANs
+  native_routed: Supports native layer-3 interface on a trunk port
```

### Comparing `networklab-1.5.4.post1/netsim/modules/vrf.py` & `networklab-1.5.5.dev1/netsim/modules/vrf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/modules/vxlan.py` & `networklab-1.5.5.dev1/netsim/modules/vxlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/modules/vxlan.yml` & `networklab-1.5.5.dev1/netsim/modules/vxlan.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # VXLAN default settings and attributes
 #
-supported_on: [ eos, nxos, vyos, csr, dellos10, srlinux, frr, cumulus, sros, arubacx, vptx, none ]
+# Also supported on csr, eos, frr, nxos
+#
+supported_on: [ vyos, dellos10, srlinux, cumulus, sros, arubacx, vptx, none ]
 requires: [ vlan ]
 config_after: [ vrf ] # For platforms that suppport L3 VXLAN, vrfs must be created first
 transform_after: [ vlan, vrf ]
 domain: global
 flooding: static
 start_vni: 100000
 attributes:
```

### Comparing `networklab-1.5.4.post1/netsim/outputs/__init__.py` & `networklab-1.5.5.dev1/netsim/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/outputs/ansible.py` & `networklab-1.5.5.dev1/netsim/outputs/ansible.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import os
 from box import Box
 
 from .. import common
 from . import _TopologyOutput,check_writeable
 from ..augment import nodes
 from ..augment import devices
+from ..utils import templates,strings,log
+from ..utils import files as _files
 
 forwarded_port_name = { 'ssh': 'ansible_port', }
 
 def copy_provider_inventory(host: Box, p_data: Box) -> None:
   if 'inventory' in p_data:
     for k,v in p_data.inventory.items():
       host[k] = v
@@ -132,18 +134,15 @@
   print(common.get_yaml_string(inventory))
 
 def write_yaml(data: Box, fname: str, header: str) -> None:
   dirname = os.path.dirname(fname)
   if dirname and not os.path.exists(dirname):
     os.makedirs(dirname)
 
-  with open(fname,"w") as output:
-    output.write(header)
-    output.write(common.get_yaml_string(data))
-    output.close()
+  _files.create_file_from_text(fname,header+"\n"+strings.get_yaml_string(data))
 
 min_inventory_data = [ 'id','ansible_host','ansible_port','ansible_connection','ansible_user','ansible_ssh_pass' ]
 
 def ansible_inventory(topology: Box, fname: typing.Optional[str] = 'hosts.yml', hostvars: typing.Optional[str] = 'dirs') -> None:
   inventory = create(topology)
 
 #  import ipdb; ipdb.set_trace()
@@ -189,19 +188,28 @@
 
 def ansible_config(config_file: typing.Union[str,None] = 'ansible.cfg', inventory_file: typing.Union[str,None] = 'hosts.yml') -> None:
   if not config_file:
     config_file = 'ansible.cfg'
   if not inventory_file:
     inventory_file = 'hosts.yml'
 
-  with open(config_file,"w") as output:
-    output.write(common.template('ansible.cfg.j2',{ 'inventory': inventory_file or 'hosts.yml' },'templates','ansible'))
-    output.close()
-    if not common.QUIET:
-      print("Created Ansible configuration file: %s" % config_file)
+  try:
+    cfg_text = templates.render_template(
+                j2_file='ansible.cfg.j2',
+                data={'inventory': inventory_file or 'hosts.yml'},
+                path='templates',
+                extra_path=_files.get_search_path('ansible'))
+  except Exception as ex:
+    log.fatal(
+      text=f"Error rendering ansible.cfg\n{strings.extra_data_printout(str(ex))}",
+      module='ansible')
+
+  _files.create_file_from_text(config_file,cfg_text)
+  if not common.QUIET:
+    print("Created Ansible configuration file: %s" % config_file)
 
 class AnsibleInventory(_TopologyOutput):
 
   def write(self, topology: Box) -> None:
     check_writeable('Ansible inventory')
     hostfile = self.settings.hostfile or 'hosts.yml'
     configfile = self.settings.configfile or 'ansible.cfg'
```

### Comparing `networklab-1.5.4.post1/netsim/outputs/common.py` & `networklab-1.5.5.dev1/netsim/outputs/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/outputs/d2.py` & `networklab-1.5.5.dev1/netsim/outputs/d2.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 #
 import typing
 
 import yaml
 import os
 from box import Box
 
-from .. import common
 from ..data import get_box
 from ..data.validate import must_be_list
 from . import _TopologyOutput
+from ..utils import files as _files
+from ..utils import log
 
 '''
 Copy default settings into a D2 map converting Python dictionaries into
 dotted-name format D2 is using
 '''
 def dump_d2_dict(f : typing.TextIO, data: dict, indent: str) -> None: 
   for k,v in data.items():
@@ -156,25 +157,25 @@
     return
 
   placed_hosts = []
   for g,v in topology.groups.items():
     if g in groups:
       for n in v.members:
         if n in placed_hosts:
-          common.error(
+          log.error(
             f'Cannot create overlapping graph clusters: node {n} is in two groups',
-            common.IncorrectValue,
+            log.IncorrectValue,
             'graph')
           continue
         else:
           maps.groups[g].nodes[n] = topology.nodes[n]
           placed_hosts.append(n)
 
 def graph_topology(topology: Box, fname: str, settings: Box,g_format: typing.Optional[list]) -> bool:
-  f = common.open_output_file(fname)
+  f = _files.open_output_file(fname)
   maps = build_maps(topology)
 
   if 'groups' in settings:
     must_be_list(
       parent=settings,
       key='groups',path='defaults.outputs.graph',
       true_value=list(topology.get('groups',{}).keys()),
@@ -223,18 +224,18 @@
 
   f.write(f'{node.d2.name} {arrow_dir} {nodes[session.name].d2.name} {{\n')
   copy_d2_attr(f,session.type,settings,'  ')
   f.write('}\n')
 
 def graph_bgp(topology: Box, fname: str, settings: Box,g_format: typing.Optional[list]) -> bool:
   if not 'bgp' in topology.get('module',{}):
-    common.error('BGP graph format can only be used to draw topologies using BGP')
+    log.error('BGP graph format can only be used to draw topologies using BGP',module='d2')
     return False
 
-  f = common.open_output_file(fname)
+  f = _files.open_output_file(fname)
 
   rr_session = settings.get('rr_sessions',False)
   if g_format is not None and len(g_format) > 1:
     rr_session = g_format[1] == 'rr'
 
   maps = build_maps(topology)
   graph_clusters(f,maps.bgp,settings,topology.nodes)
@@ -272,18 +273,18 @@
     output_format = 'topology'
 
     topology = get_box(topology)                       # Create a local copy of the topology
     set_d2_attr(topology)
     if hasattr(self,'filenames'):
       graphfile = self.filenames[0]
       if len(self.filenames) > 1:
-        common.error('Extra output filename(s) ignored: %s' % str(self.filenames[1:]),common.IncorrectValue,'graph')
+        log.error('Extra output filename(s) ignored: %s' % str(self.filenames[1:]),log.IncorrectValue,'d2')
 
     if self.format:
       output_format = self.format[0]
 
     if output_format in graph_dispatch:
       if graph_dispatch[output_format](topology,graphfile,self.settings,self.format):
         print("Created graph file %s in %s format" % (graphfile, output_format))
     else:
       formats = ', '.join(graph_dispatch.keys())
-      common.error('Unknown graph format, use one of %s' % formats,common.IncorrectValue,'graph')
+      log.error('Unknown graph format, use one of %s' % formats,log.IncorrectValue,'d2')
```

### Comparing `networklab-1.5.4.post1/netsim/outputs/d2.yml` & `networklab-1.5.5.dev1/netsim/outputs/d2.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/outputs/devices.py` & `networklab-1.5.5.dev1/netsim/outputs/devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import sys
 from box import Box
 
 from .. import common
 from . import _TopologyOutput,check_writeable
 from .common import adjust_inventory_host
+from ..utils import files as _files
 
 def create(nodes: Box, defaults: Box, addressing: typing.Optional[Box] = None) -> Box:
   inventory = Box({},default_box=True,box_dots=True)
 
   if addressing:
     inventory.all.vars.pools = addressing
     for name,pool in inventory.all.vars.pools.items():
@@ -32,15 +33,15 @@
   return inventory
 
 def write_yaml(data: Box, fname: str, header: str) -> None:
   dirname = os.path.dirname(fname)
   if dirname and not os.path.exists(dirname):
     os.makedirs(dirname)
 
-  with open(fname,"w") as output:
+  with _files.open_output_file(fname) as output:
     output.write(header)
     output.write(common.get_yaml_string(data))
     output.close()
 
 min_inventory_data = [ 'id','ansible_host','ansible_port' ]
 
 def write_devices(data: Box, fname: str, fmt: typing.Optional[str]) -> None:
```

### Comparing `networklab-1.5.4.post1/netsim/outputs/format.py` & `networklab-1.5.5.dev1/netsim/outputs/yaml.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,40 +2,58 @@
 # Create YAML or JSON output
 #
 import typing
 
 import yaml
 import os
 from box import Box,BoxList
-from jinja2 import Environment, BaseLoader, FileSystemLoader, StrictUndefined, make_logging_undefined
 
-from .. import common
 from .. import data
 from ..augment import topology
+from ..utils import files as _files
+from ..utils import log,strings
 
-from . import _TopologyOutput
+from . import _TopologyOutput,check_writeable
 
-class FORMAT(_TopologyOutput):
+class YAML(_TopologyOutput):
 
   def write(self, topo: Box) -> None:
     outfile = self.settings.filename or '-'
     modname = type(self).__name__
 
     if hasattr(self,'filenames'):
       outfile = self.filenames[0]
       if len(self.filenames) > 1:
-        common.error('Extra output filename(s) ignored: %s' % str(self.filenames[1:]),common.IncorrectValue,modname)
+        log.error('Extra output filename(s) ignored: %s' % str(self.filenames[1:]),log.IncorrectValue,modname)
+
+    if outfile == 'netlab.snapshot.yml':
+      check_writeable('netlab.snapshot.yml')
 
     cleantopo: typing.Any = topology.cleanup_topology(topo)
-    output = common.open_output_file(outfile)
+    output = _files.open_output_file(outfile)
 
     for fmt in self.format:
-      if not fmt in self.settings:
-        common.error(f'Unknown template format {fmt}',common.IncorrectValue,modname)
-        print(topo.defaults.outputs.format)
-        continue
-
-      template = Environment(loader=BaseLoader(), \
-              trim_blocks=True,lstrip_blocks=True, \
-              undefined=make_logging_undefined(base=StrictUndefined)).from_string(self.settings[fmt])
-      output.write(template.render(**topo))
+      if fmt == 'nodefault':
+        cleantopo.pop('defaults')
+      elif fmt == 'noaddr':
+        cleantopo.pop('addressing')
+      else:
+        try:
+          result = eval(fmt,cleantopo) if fmt != '.' else cleantopo
+        except Exception as ex:
+          log.fatal(f'Error trying to evaluate {fmt}: {str(ex)}')
+          return
+        cleantopo = result
+        break
+
+    if not isinstance(cleantopo,Box) and not isinstance(cleantopo,BoxList):
+      output.write(f"{str(result)}\n")
+    elif modname == 'YAML':
+      output.write(strings.get_yaml_string(cleantopo))
+    else:
+      output.write(cleantopo.to_json(indent=2,sort_keys=True))
+
+    if outfile != '-':
+      _files.close_output_file(output)
+      print(f"Created transformed topology dump in {modname} format in {outfile}")
+    else:
       output.write("\n")
```

### Comparing `networklab-1.5.4.post1/netsim/outputs/graph.py` & `networklab-1.5.5.dev1/netsim/outputs/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 #
 import typing
 
 import yaml
 import os
 from box import Box
 
-from .. import common
 from ..data.validate import must_be_list
 from . import _TopologyOutput
+from ..utils import files as _files
+from ..utils import log
 
 def node_with_label(f : typing.TextIO, n: Box, settings: Box, indent: typing.Optional[str] = '') -> None:
   f.write('%s  "%s" [\n' % (indent,n.name))
   node_ip_str = ""
   if settings.node_address_label:
     node_ip = n.loopback.ipv4 or n.loopback.ipv6
     if not node_ip and n.interfaces:
@@ -104,25 +105,25 @@
     return
 
   placed_hosts = []
   for g,v in topology.groups.items():
     if g in groups:
       for n in v.members:
         if n in placed_hosts:
-          common.error(
+          log.error(
             f'Cannot create overlapping graph clusters: node {n} is in two groups',
-            common.IncorrectValue,
+            log.IncorrectValue,
             'graph')
           continue
         else:
           maps.groups[g].nodes[n] = topology.nodes[n]
           placed_hosts.append(n)
 
 def graph_topology(topology: Box, fname: str, settings: Box,g_format: typing.Optional[list]) -> bool:
-  f = common.open_output_file(fname)
+  f = _files.open_output_file(fname)
   graph_start(f)
 
   maps = build_maps(topology)
 
   if 'groups' in settings:
     must_be_list(
       parent=settings,
@@ -139,15 +140,15 @@
       node_with_label(f,n,settings)
 
   for l in topology.links:
     if l.type == "p2p":
       edge_p2p(f,l,settings.interface_labels)
     else:
       if not l.bridge:
-        common.error('Found a lan/stub link without a bridge name, skipping',common.IncorrectValue,'graph')
+        log.error('Found a lan/stub link without a bridge name, skipping',log.IncorrectValue,'graph')
         next
       network_with_label(f,l,settings)
       for ifdata in l.interfaces:
         if ifdata.node in maps.nodes:
           edge_node_net(f,l,ifdata,settings.interface_labels)
 
   f.write("}\n")
@@ -171,18 +172,18 @@
   else:
     f.write('    color="%s"\n' % settings.colors.get('ebgp','#b21a1a'))
   f.write(f'    penwidth=2.5 arrowsize=0.7 dir={arrow_dir}\n')
   f.write('  ]\n')
 
 def graph_bgp(topology: Box, fname: str, settings: Box,g_format: typing.Optional[list]) -> bool:
   if not 'bgp' in topology.get('module',{}):
-    common.error('BGP graph format can only be used to draw topologies using BGP')
+    log.error('BGP graph format can only be used to draw topologies using BGP')
     return False
 
-  f = common.open_output_file(fname)
+  f = _files.open_output_file(fname)
   graph_start(f)
 
   rr_session = g_format is not None and len(g_format) > 1 and g_format[1] == 'rr'
 
   maps = build_maps(topology)
   graph_clusters(f,maps.bgp,settings)
 
@@ -206,18 +207,18 @@
   def write(self, topology: Box) -> None:
     graphfile = self.settings.filename or 'graph.dot'
     output_format = 'topology'
 
     if hasattr(self,'filenames'):
       graphfile = self.filenames[0]
       if len(self.filenames) > 1:
-        common.error('Extra output filename(s) ignored: %s' % str(self.filenames[1:]),common.IncorrectValue,'graph')
+        log.error('Extra output filename(s) ignored: %s' % str(self.filenames[1:]),log.IncorrectValue,'graph')
 
     if self.format:
       output_format = self.format[0]
 
     if output_format in graph_dispatch:
       if graph_dispatch[output_format](topology,graphfile,self.settings,self.format):
         print("Created graph file %s in %s format" % (graphfile, output_format))
     else:
       formats = ', '.join(graph_dispatch.keys())
-      common.error('Unknown graph format, use one of %s' % formats,common.IncorrectValue,'graph')
+      log.error('Unknown graph format, use one of %s' % formats,log.IncorrectValue,'graph')
```

### Comparing `networklab-1.5.4.post1/netsim/outputs/graphite.py` & `networklab-1.5.5.dev1/netsim/outputs/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/outputs/provider.py` & `networklab-1.5.5.dev1/netsim/outputs/provider.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/outputs/tools.py` & `networklab-1.5.5.dev1/netsim/outputs/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from box import Box
 from pathlib import Path
 
 from .. import common
 from . import _TopologyOutput,check_writeable
 from ..tools import _ToolOutput
 from .common import adjust_inventory_host
-from ..utils import templates
+from ..utils import templates,strings,log
+from ..utils import files as _files
 
 def render_tool_config(tool: str, fmt: str, topology: Box) -> str:
     output_module = _ToolOutput.load(tool)
     if output_module:
       return output_module.write(topology,fmt)
     else:
       common.error(f'Cannot load tool-specific module tools.{tool}')
@@ -37,28 +38,31 @@
       continue
     fname = f'{tool}/{config.dest}'
     if 'render' in config:
       config_text = render_tool_config(tool,config.render,topology)
       config_src  = f'rendering "{config.render}" format'
     elif 'template' in config:
       template = config.template
-      config_text = templates.template(
-                      j2=config.template,
-                      data=topo_data,
-                      path=f'tools/{tool}',
-                      user_template_path=f'tools/{tool}')
+      try:
+        config_text = templates.render_template(
+                        j2_file=config.template,
+                        data=topo_data,
+                        path=f'tools/{tool}',
+                        extra_path=_files.get_search_path(f'tools/{tool}'))
+      except Exception as ex:
+        log.fatal(
+          text=f"Error rendering {config.template}\n{strings.extra_data_printout(str(ex))}",
+          module='libvirt')
       config_src  = f'from {config.template} template'
     else:
       common.error(f'Unknown tool configuration type\n... tool {tool}\n... config {config}')
       continue
 
     try:
-      with open(fname,"w") as output:
-        output.write(config_text)
-        output.close()
+      _files.create_file_from_text(fname,config_text)
       print(f'Created {fname} {config_src}')
     except Exception as e:
       common.error(f'Error writing tool configuration file {fname}\n... {e}')
 
 class ToolConfigs(_TopologyOutput):
 
   def write(self, topology: Box) -> None:
```

### Comparing `networklab-1.5.4.post1/netsim/providers/__init__.py` & `networklab-1.5.5.dev1/netsim/providers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # Related modules
 from box import Box
 
 from .. import common
 from ..callback import Callback
 from ..augment import devices,links
 from ..data import get_box,get_empty_box,filemaps
+from ..utils import files as _files
+from ..utils import templates,log,strings
 
 class _Provider(Callback):
   def __init__(self, provider: str, data: Box) -> None:
     self.provider = provider
     if 'template' in data:
       self._default_template_name = data.template
 
@@ -34,18 +36,18 @@
     else:
       return _Provider(provider,data)
 
   def get_template_path(self) -> str:
     return 'templates/provider/' + self.provider
 
   def get_full_template_path(self) -> str:
-    return str(common.get_moddir()) + '/' + self.get_template_path()
+    return str(_files.get_moddir()) + '/' + self.get_template_path()
 
   def find_extra_template(self, node: Box, fname: str) -> typing.Optional[str]:
-    return common.find_file(fname+'.j2',[ f'./{node.device}','.',f'{ self.get_full_template_path() }/{node.device}'])
+    return _files.find_file(fname+'.j2',[ f'./{node.device}','.',f'{ self.get_full_template_path() }/{node.device}'])
 
   def get_output_name(self, fname: typing.Optional[str], topology: Box) -> str:
     if fname:
       return fname
 
     fname = topology.defaults.providers[self.provider].config
     if fname:
@@ -119,47 +121,63 @@
       inkey: str = 'config_templates',
       outkey: str = 'binds') -> None:
 
     binds = node.get(f'{self.provider}.{outkey}',None)
     if not binds:
       return
 
-    sys_folder = str(common.get_moddir())+"/"
+    sys_folder = str(_files.get_moddir())+"/"
     out_folder = f"{self.provider}_files/{node.name}"
 
     bind_dict = filemaps.mapping_to_dict(binds)
     for file,mapping in bind_dict.items():
       if not out_folder in file:                  # Skip files that are not mapped into the temporary provider folder
         continue
       file_name = file.replace(out_folder+"/","")
       template_name = self.find_extra_template(node,file_name)
       if template_name:
         node_data = node + { 'hostvars': topology.nodes }
         if '/' in file_name:                      # Create subdirectory in out_folder if needed
           pathlib.Path(f"{out_folder}/{os.path.dirname(file_name)}").mkdir(parents=True,exist_ok=True)
-        common.write_template(
-          in_folder=os.path.dirname(template_name),
-          j2=os.path.basename(template_name),
-          data=node_data.to_dict(),
-          out_folder=out_folder, filename=file_name)
+        try:
+          templates.write_template(
+            in_folder=os.path.dirname(template_name),
+            j2=os.path.basename(template_name),
+            data=node_data.to_dict(),
+            out_folder=out_folder, filename=file_name)
+        except Exception as ex:
+          log.fatal(
+            text=f"Error rendering {template_name} into {file_name}\n{strings.extra_data_printout(str(ex))}",
+            module=self.provider)
+
         print( f"Created {out_folder}/{file_name} from {template_name.replace(sys_folder,'')}, mapped to {node.name}:{mapping}" )
       else:
         common.error(f"Cannot find template for {file_name} on node {node.name}",common.MissingValue,'provider')
 
   def create(self, topology: Box, fname: typing.Optional[str]) -> None:
     self.transform(topology)
     fname = self.get_output_name(fname,topology)
-    output = common.open_output_file(fname)
-    output.write(common.template(self.get_root_template(),topology.to_dict(),self.get_template_path(),self.provider))
+    tname = self.get_root_template()
+    try:
+      r_text = templates.render_template(
+        data=topology.to_dict(),
+        j2_file=tname,
+        path=self.get_template_path(),
+        extra_path=_files.get_search_path(self.provider))
+    except Exception as ex:
+      log.fatal(
+        text=f"Error rendering {fname} from {tname}\n{strings.extra_data_printout(str(ex))}",
+        module=self.provider)
+
+    _files.create_file_from_text(fname,r_text)
     if fname != '-':
-      common.close_output_file(output)
       print("Created provider configuration file: %s" % fname)
       self.post_configuration_create(topology)
     else:
-      output.write("\n")
+      print("\n")
 
   def post_start_lab(self, topology: Box) -> None:
     pass
 
   def pre_start_lab(self, topology: Box) -> None:
     pass
```

### Comparing `networklab-1.5.4.post1/netsim/providers/clab.py` & `networklab-1.5.5.dev1/netsim/providers/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/providers/clab.yml` & `networklab-1.5.5.dev1/netsim/providers/clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/providers/external.py` & `networklab-1.5.5.dev1/netsim/providers/external.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/providers/libvirt.py` & `networklab-1.5.5.dev1/netsim/providers/libvirt.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 import os
 import typing
 from box import Box
 import pathlib
 import tempfile
 import netaddr
 
-from .. import common
 from ..data import types
+from ..utils import log
+from ..utils import files as _files
 from . import _Provider
 from ..augment.links import get_link_by_index
 from ..cli import is_dry_run,external_commands
 
-LIBVIRT_MANAGEMENT_NETWORK_NAME = "vagrant-libvirt"
-LIBVIRT_MANAGEMENT_BRIDGE_NAME  = "libvirt-mgmt"
-LIBVIRT_MANAGEMENT_NETWORK_FILE = "templates/provider/libvirt/vagrant-libvirt.xml"
+LIBVIRT_MANAGEMENT_NETWORK_NAME  = "vagrant-libvirt"
+LIBVIRT_MANAGEMENT_BRIDGE_NAME   = "libvirt-mgmt"
+LIBVIRT_MANAGEMENT_TEMPLATE_PATH = "templates/provider/libvirt"
+LIBVIRT_MANAGEMENT_TEMPLATE_NAME = "vagrant-libvirt.xml"
 LIBVIRT_MANAGEMENT_SUBNET       = "192.168.121.0/24"
 
 """
 Replace management IP subnet in vagrant-libvirt XML template:
 
 * Replace subnet (.1 address) and netmask
 * Replace start (.2) and end (start -1) of dynamic DHCP range
@@ -73,24 +75,32 @@
 * Replace network and bridge name if needed
 * Replace IP subnet/mask and DHCP bindings
 * Create a temporary file with modified XML definitions
 * Return the name of the temporary file
 """
 
 def get_libvirt_mgmt_template() -> str:
-  return str(pathlib.Path(__file__).parent.parent.joinpath(LIBVIRT_MANAGEMENT_NETWORK_FILE).resolve())
+  search_path = _files.get_search_path("libvirt",LIBVIRT_MANAGEMENT_TEMPLATE_PATH)
+  xml_file = _files.find_file(LIBVIRT_MANAGEMENT_TEMPLATE_NAME,search_path)
+  if not xml_file:
+    log.fatal('Internal error: cannot find {LIBVIRT_MANAGEMENT_TEMPLATE_NAME}')
+
+  return xml_file
 
 def create_network_template(topology: Box) -> str:
   net_template_xml = get_libvirt_mgmt_template()
+  if log.debug_active('libvirt'):
+    print(f"Template XML: {net_template_xml}")
+
   mgmt = topology.addressing.mgmt
   try:
     with open(net_template_xml) as xfile:
       xml = xfile.read()
   except Exception as ex:
-    common.fatal(f'Cannot open/read XML definition of vagrant-libvirt network {str(sys.exc_info()[1])}')
+    log.fatal(f'Cannot open/read XML definition of vagrant-libvirt network {str(sys.exc_info()[1])}')
 
   if mgmt._network:
     xml = xml.replace(LIBVIRT_MANAGEMENT_NETWORK_NAME,mgmt._network)
 
   if mgmt._bridge:
     xml = xml.replace(LIBVIRT_MANAGEMENT_BRIDGE_NAME,mgmt._bridge)
 
@@ -100,50 +110,64 @@
     tfile.write(xml)
     tfile.close()
     return tfile.name
 
 def create_vagrant_network(topology: typing.Optional[Box] = None) -> None:
   mgmt_net = topology.addressing.mgmt._network if topology is not None else ''
   mgmt_net = mgmt_net or LIBVIRT_MANAGEMENT_NETWORK_NAME
+  create_net = True
 
-  external_commands.run_command(
-    ['virsh','net-destroy',mgmt_net],check_result=True,ignore_errors=True)    # Remove management network
-  external_commands.run_command(
-    ['virsh','net-undefine',mgmt_net],check_result=True,ignore_errors=True)   # ... if it exists
-  common.print_verbose(f'creating libvirt management network {mgmt_net}')
+  if topology is not None and topology.addressing.mgmt._permanent:
+    net_list = external_commands.run_command(
+      ['virsh','net-list'],check_result=True,return_stdout=True)
+    if isinstance(net_list,str):
+      create_net = not mgmt_net in net_list
+  else:
+    if log.debug_active('libvirt'):
+      print(f"Deleting libvirt management network {mgmt_net}")
+    external_commands.run_command(
+      ['virsh','net-destroy',mgmt_net],check_result=True,ignore_errors=True)    # Remove management network
+    external_commands.run_command(
+      ['virsh','net-undefine',mgmt_net],check_result=True,ignore_errors=True)   # ... if it exists
+
+  if not create_net:
+    return
+
+  if not log.QUIET:
+    print(f'creating libvirt management network {mgmt_net}')
 
   if topology is None:
     net_template = get_libvirt_mgmt_template()                    # When called without topology data use the default template
   else:
     net_template = create_network_template(topology)              # Otherwise create a temporary XML file
+
   external_commands.run_command(
     ['virsh','net-define',net_template],check_result=True)
   if not topology is None:                                        # Remove the temporary XML file if needed
     os.remove(net_template)
 
   return
 
 def get_linux_bridge_name(virsh_bridge: str) -> typing.Optional[str]:
   if is_dry_run():
     print(f"DRY RUN: Assuming Linux bridge name {virsh_bridge} for libvirt network {virsh_bridge}")
     return virsh_bridge
-  try:
-    result = subprocess.run(['virsh','net-info',virsh_bridge],capture_output=True,check=True,text=True)
-  except:
-    common.error('Cannot run net-info for libvirt network %s' % virsh_bridge, module='libvirt')
+  result = external_commands.run_command(
+    ['virsh','net-info',virsh_bridge],check_result=True,return_stdout=True)
+  if not isinstance(result,str):
+    log.error('Cannot run net-info for libvirt network %s' % virsh_bridge, module='libvirt')
     return None
 
   match = None
-  if result and result.returncode == 0:
-    match = re.search("Bridge:\\s+(.*)$",result.stdout,flags=re.MULTILINE)
+  match = re.search("Bridge:\\s+(.*)$",result,flags=re.MULTILINE)
 
   if match:
     return match.group(1)
   else:
-    common.error(f'Cannot get Linux bridge name for libvirt network {virsh_bridge}', module='libvirt')
+    log.error(f'Cannot get Linux bridge name for libvirt network {virsh_bridge}', module='libvirt')
 
   return None
 
 """
 Create batches of 'vagrant up' command to deal with very large topologies
 
 * Split node names into libvirt.batch_size - sized batches
@@ -152,15 +176,15 @@
 def create_vagrant_batches(topology: Box) -> None:
   libvirt_defaults = topology.defaults.providers.libvirt
   if not libvirt_defaults.batch_size:
     return
 
   types.must_be_int(libvirt_defaults,'batch_size','defaults.providers.libvirt',module='libvirt',min_value=1,max_value=50)
   types.must_be_int(libvirt_defaults,'batch_interval','defaults.providers.libvirt',module='libvirt',min_value=1,max_value=1000)
-  common.exit_on_error()
+  log.exit_on_error()
 
   batch_size = libvirt_defaults.batch_size
   start_cmd  = libvirt_defaults.start
   libvirt_defaults.start = []
   node_list = list(topology.nodes.keys())
 
   while True:
@@ -231,55 +255,56 @@
         if intf.libvirt.get('type') != 'tunnel':                    # The current link is not a tunnel link, move on
           continue
 
         link.pop("bridge",None)                                     # And now the real work starts. Pop the bridge attribute first
 
         remote_if_list = [ rif for rif in link.interfaces if rif.node != node.name or rif.ifindex != intf.ifindex ]
         if len(remote_if_list) != 1:                                # There should be only one remote interface attached to this link
-          common.fatal(
+          log.fatal(
             f'Cannot find remote interface for P2P link\n... node {node.name}\n... intf {intf}\n... link {link}\n... iflist {remote_if_list}')
           return
 
         remote_if = remote_if_list[0]                               # Get remote interface
         intf.remote_ifindex = remote_if.ifindex                     # ... and copy its ifindex
         intf.remote_id = topology.nodes[remote_if.node].id          # ... and node ID
         if not intf.remote_id:
-          common.fatal(
+          log.fatal(
             f'Cannot find remote node ID on a P2P link\n... node {node.name}\n... intf {intf}\n... link {link}')
           return
 
   def pre_start_lab(self, topology: Box) -> None:
-    common.print_verbose('pre-start hook for libvirt')
+    log.print_verbose('pre-start hook for libvirt')
     # Starting from vagrant-libvirt 0.7.0, the destroy actions deletes all the networking
     #  including the "vagrant-libvirt" management network.
     #  Let's re-create it if missing!
+    os.environ["LIBVIRT_DEFAULT_URI"] = "qemu:///system"            # Create system-wide libvirt networks
     create_vagrant_network(topology)
     create_vagrant_batches(topology)
 
   def post_start_lab(self, topology: Box) -> None:
-    common.print_verbose('libvirt lab has started, fixing Linux bridges')
+    log.print_verbose('libvirt lab has started, fixing Linux bridges')
     mgmt_bridge = get_linux_bridge_name(topology.addressing.mgmt._network or LIBVIRT_MANAGEMENT_NETWORK_NAME)
     if mgmt_bridge:
       topology.addressing.mgmt._bridge = mgmt_bridge
 
     for l in topology.links:
       brname = l.get('bridge',None)
       if not brname:                                                # Link not using a Linux bridge
         continue
       if not 'libvirt' in l.provider:                               # Not a libvirt link, skip it
         continue
 
-      if common.debug_active('libvirt'):
+      if log.debug_active('libvirt'):
         print('libvirt post_start_lab: fixing Linux bridge for link {l}')
 
       linux_bridge = get_linux_bridge_name(brname)
       if linux_bridge is None:
         continue
 
       l.bridge = linux_bridge
-      common.print_verbose(f"... network {brname} maps into {linux_bridge}")
+      log.print_verbose(f"... network {brname} maps into {linux_bridge}")
       if not external_commands.run_command(
           ['sudo','sh','-c',f'echo 0x4000 >/sys/class/net/{linux_bridge}/bridge/group_fwd_mask']):
-        common.error(f"Cannot set forwarding mask on Linux bridge {linux_bridge}")
+        log.error(f"Cannot set forwarding mask on Linux bridge {linux_bridge}")
         continue
 
-      common.print_verbose(f"... setting LLDP enabled flag on {linux_bridge}")
+      log.print_verbose(f"... setting LLDP enabled flag on {linux_bridge}")
```

### Comparing `networklab-1.5.4.post1/netsim/providers/libvirt.yml` & `networklab-1.5.5.dev1/netsim/providers/libvirt.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/read_topology.py` & `networklab-1.5.5.dev1/netsim/read_topology.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,27 @@
   new_resources = False
   import importlib_resources as resources         # type: ignore
 
 # Related modules
 from . import common
 from . import data
 from .data import types
+from .utils import files as _files
 
 """
 Utility routines for include_yaml functionality
 """
 
 def get_traversable_path(dir_name : str) -> typing.Any:
   if 'package:' in dir_name:
     dir_name = dir_name.replace('package:','')
     pkg_files: typing.Any = None
 
     if not new_resources:
-      pkg_files = pathlib.Path(common.get_moddir())
+      pkg_files = pathlib.Path(_files.get_moddir())
     else:
       package = '.'.join(__name__.split('.')[:-1])
       pkg_files = resources.files(package)        # type: ignore
     if dir_name == '':
       return pkg_files
     else:
       return pkg_files.joinpath(dir_name)
```

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/clab/clab.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/clab/clab.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/clab/frr/daemons.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/clab/frr/daemons.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/clab/linux/hosts.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/clab/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/external/external.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/external/external.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/libvirt/Vagrantfile.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/libvirt/Vagrantfile.j2`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 VAGRANT_COMMAND = ARGV[0]
 
 Vagrant.configure("2") do |config|
   config.vm.provider :libvirt do |libvirt|
 {% if addressing.mgmt._network|default(False) %}
     libvirt.management_network_name = "{{ addressing.mgmt._network }}"
 {% endif %}
+{% if addressing.mgmt._permanent|default(False) %}
+    libvirt.management_network_keep = true
+{% endif %}
     libvirt.management_network_address = "{{ addressing.mgmt.ipv4 }}"
     libvirt.default_prefix = "{{ defaults.name }}_"
   end
 {% for name,n in nodes.items() if not (n.unmanaged|default(False)) %}
 {%   set name = name.split('.')[0] %}
 {%   set box  = n.box %}
 {%   include [ n.device ~ "-raw.j2","define-domain.j2" ] +%}
```

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/libvirt/define-domain.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/libvirt/define-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/libvirt/iosxr-domain.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/libvirt/iosxr-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/libvirt/libvirt-bridge.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/libvirt/libvirt-bridge.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/libvirt/libvirt-tunnel.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/libvirt/libvirt-tunnel.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/libvirt/nxos-domain.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/libvirt/nxos-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/libvirt/vagrant-libvirt.xml` & `networklab-1.5.5.dev1/netsim/templates/provider/libvirt/vagrant-libvirt.xml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/libvirt/vptx-domain.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/libvirt/vptx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/libvirt/vsrx-domain.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/libvirt/vsrx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/templates/provider/virtualbox/Vagrantfile.j2` & `networklab-1.5.5.dev1/netsim/templates/provider/virtualbox/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/tools/__init__.py` & `networklab-1.5.5.dev1/netsim/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/tools/graphite.py` & `networklab-1.5.5.dev1/netsim/tools/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/tools/graphite.yml` & `networklab-1.5.5.dev1/netsim/tools/graphite.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/tools/suzieq.yml` & `networklab-1.5.5.dev1/netsim/tools/suzieq.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/topology-defaults.yml` & `networklab-1.5.5.dev1/netsim/topology-defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/utils/log.py` & `networklab-1.5.5.dev1/netsim/utils/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 class FatalError(Warning):
   pass
 
 class ErrorAbort(Exception):
   pass
 
-def fatal(text: str, module: str = 'netlab') -> None:
+def fatal(text: str, module: str = 'netlab') -> typing.NoReturn:
   global err_count
   err_count = err_count + 1
   if RAISE_ON_ERROR:
     raise ErrorAbort(text)
   else:
     if WARNING:
       warnings.warn_explicit(text,FatalError,filename=module,lineno=err_count)
```

### Comparing `networklab-1.5.4.post1/netsim/utils/status.py` & `networklab-1.5.5.dev1/netsim/utils/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/netsim/utils/strings.py` & `networklab-1.5.5.dev1/netsim/utils/strings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 #
 # Common routines for create-topology script
 #
 import textwrap
-from box import Box
+import typing
+from box import Box,BoxList
+
+ruamel_attrs: typing.Final[dict] = {'version': (1,1)}
+
+def get_yaml_string(x : typing.Any) -> str:
+  global ruamel_attrs
+  if isinstance(x, Box) or isinstance(x,BoxList):
+    return x.to_yaml(ruamel_attrs=ruamel_attrs)
+  if isinstance(x,dict):
+    return Box(x).to_yaml(ruamel_attrs=ruamel_attrs)
+  elif isinstance(x,list):
+    return BoxList(x).to_yaml(ruamel_attrs=ruamel_attrs)
+  else:
+    return str(x)
 
 def extra_data_printout(s : str, width: int = 70) -> str:
   lines = []
   for line in s.split('\n'):
     lines.append(textwrap.TextWrapper(
       initial_indent="... ",
       subsequent_indent="      ",
```

### Comparing `networklab-1.5.4.post1/netsim/utils/templates.py` & `networklab-1.5.5.dev1/netsim/utils/templates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,85 @@
 #
 # Common routines for create-topology script
 #
-import sys
 import typing
 import os
 import pathlib
 
 from jinja2 import Environment, PackageLoader, FileSystemLoader, StrictUndefined, make_logging_undefined
-from box import Box,BoxList
 
-from .log import debug_active
+from .log import debug_active,fatal
+from .files import get_moddir,create_file_from_text
 
 ansible_filter_map: dict = {}
 ANSIBLE_DEBUG = False
 
-#
-# Find path to the module directory (needed for various templates)
-#
-def get_moddir() -> pathlib.Path:
-  return pathlib.Path(__file__).resolve().parent.parent
+def add_ansible_filters(ENV: Environment) -> None:
+  for k,v in ansible_filter_map.items():
+    ENV.filters[k] = v
 
-#
-# Find a file in a search path
-#
-def find_file(path: str, search_path: typing.List[str]) -> typing.Optional[str]:
-  for dirname in search_path:
-    candidate = os.path.join(dirname, path)
-    if os.path.exists(candidate):
-      return candidate
+"""
+Render a Jinja2 template
 
-  return None
+Template parameters:
+* j2_file -- the name of the Jinja2 file
+* j2_text -- the template text (potentially from a topology setting)
+
+Path parameters:
+* template_path -- fully specified template path, overrides any other combo
+* path -- relative path to search in package directory or current/absolute directory
+* user_template_path -- subdirectory of user directories to search (current, home)
+"""
+
+def render_template(
+      data: typing.Dict,
+      j2_file: typing.Optional[str] = None,
+      j2_text: typing.Optional[str] = None,
+      path: typing.Optional[str] = None,
+      extra_path: typing.Optional[list] = None) -> str:
 
-def template(j2: str , data: typing.Dict, path: str, user_template_path: typing.Optional[str] = None) -> str:
   global ansible_filter_map
   load_ansible_filters()
 
-  if path [0] in ('.','/'):                             # Absolute path or path relative to current directory?
-    template_path = [ path ]
-  else:                                                 # Path relative to netsim module, add module path to it
-    template_path = [ str(get_moddir() / path) ]
-  if not user_template_path is None:
-    template_path = [ './' + user_template_path, os.path.expanduser('~/.netlab/'+user_template_path) ] + template_path
+  template_path = []
+  if path is not None:
+    if path [0] in ('.','/'):                             # Absolute path or path relative to current directory?
+      template_path = [ path ]
+    else:                                                 # Path relative to netsim module, add module path to it
+      template_path = [ str(get_moddir() / path) ]
+
+  if extra_path is not None:
+    template_path = extra_path + template_path
   if debug_active('template'):
-    print(f"TEMPLATE PATH for {j2}: {template_path}")
+    print(f"TEMPLATE PATH for {j2_file or 'text'}: {template_path}")
   ENV = Environment(loader=FileSystemLoader(template_path), \
           trim_blocks=True,lstrip_blocks=True, \
           undefined=make_logging_undefined(base=StrictUndefined))
-  for k,v in ansible_filter_map.items():
-    ENV.filters[k] = v
-  template = ENV.get_template(j2)
+  add_ansible_filters(ENV)
+  if j2_file is not None:
+    template = ENV.get_template(j2_file)
+  elif j2_text is not None:
+    template = ENV.from_string(j2_text)
+  else:
+    fatal('Internal error: Call to template function with missing J2 file and J2 text, aborting')
+    return ""
+
   return template.render(**data)
 
 #
 # write_template: Applies a custom template (in_folder/j2) and writes it to the given file path (out_folder/filename)
 #
 def write_template(in_folder: str, j2: str, data: typing.Dict, out_folder: str, filename: str) -> None:
   if debug_active('template'):
     print(f"write_template {in_folder}/{j2} -> {out_folder}/{filename}")
+  r_text = render_template(data=data,j2_file=j2,path=in_folder)       # Make sure we fail before creating any file(s)
+
   pathlib.Path(out_folder).mkdir(parents=True, exist_ok=True)
   out_file = f"{out_folder}/{filename}"
-  with open(out_file,mode='w') as output:
-    output.write(template(j2,data,in_folder))
+  create_file_from_text(out_file,r_text)
 
 """
 get_ansible_filter_map: Get a map of ansible filters to be used in jinja2 templates
 
 Based on the tentative Python module name, this function tries to:
 
 * Load the module
```

### Comparing `networklab-1.5.4.post1/networklab.egg-info/PKG-INFO` & `networklab-1.5.5.dev1/networklab.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.4.post1
+Version: 1.5.5.dev1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -37,32 +37,32 @@
 The latest release is [release 1.5.4](https://github.com/ipspace/netlab/releases/tag/release_1.5.4). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netlab.tools/release/) first.
 
 The latest release before the changes made in release 1.5.0 is [release 1.4.3](https://github.com/ipspace/netlab/releases/tag/release_1.4.3).
 
 ## An overview of tools:
 
 **netlab up**
-: Uses **netlab create** to create configuration files, starts the virtual lab, and uses **netlab initial** to deploy device configurations. [More details](https://netlab.tools/netlab/up/)
+: Uses **[netlab create](https://netlab.tools/netlab/create/)** to create configuration files, starts the virtual lab, and uses **[netlab initial](https://netlab.tools/netlab/initial/)** to deploy device configurations, including IP addressing, LLDP, OSPF, BGP, IS-IS, EIGRP, VRRP, VLANs, VRFs, MPLS, SR-MPLS, VXLAN, EVPN and SRv6. [More details](https://netlab.tools/netlab/up/)
 
 **netlab down**
 : Destroys the virtual lab. [More details](https://netlab.tools/netlab/down/)
 
 **netlab restart**
 : Restart and/or reconfigure the virtual lab. [More details](https://netlab.tools/netlab/restart/)
 
-**netlab create**
-: Creates a full-blown network topology, Vagrantfile and Ansible inventory from a simple list of nodes and links. [More details](https://netlab.tools/netlab/create/)
-
-**netlab initial**
-: Using topology data generated by **netlab create** and default device configuration templates configures common device parameters, protocols that should have been enabled (LLDP, OSPF, IS-IS, BGP, SR-MPLS), enables interfaces, and configures IP addresses on interfaces. [More details](https://netlab.tools/netlab/initial/)
-
 **netlab config**
-: Applies any Jinja2 configuration templates to network devices.
+: Applies additional Jinja2 configuration templates to network devices.
 
 **netlab collect**
 : Using Ansible fact gathering or other device-specific Ansible modules, collects device configurations and saves them in specified directory (default: **config**).
 
 **netlab connect**
 : Use SSH or **docker exec** to [connect to a lab device](https://netlab.tools/netlab/connect/) using device names, management network IP addresses (**ansible_host**), SSH port, and username/passwords specified in lab topology or *netlab* device defaults.
 
+**netlab report**
+: Creates a report from the transformed lab topology data.  [More details](https://netlab.tools/netlab/report/)
+
+**netlab graph**
+: Creates a lab topology graph description in Graphviz or D2 format. [More details](https://netlab.tools/netlab/graph/)
+
 **netlab show**
-: Display system settings in tabular format. [More details](https://netlab.tools/netlab/show/)
+: Display system settings in tabular, text, or YAML format. [More details](https://netlab.tools/netlab/show/)
```

### Comparing `networklab-1.5.4.post1/networklab.egg-info/SOURCES.txt` & `networklab-1.5.5.dev1/networklab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -347,18 +347,21 @@
 netsim/cli/collect.py
 netsim/cli/config.py
 netsim/cli/connect.py
 netsim/cli/create.py
 netsim/cli/down.py
 netsim/cli/empty.yml
 netsim/cli/external_commands.py
+netsim/cli/graph.py
 netsim/cli/initial.py
+netsim/cli/inspect.py
 netsim/cli/install.py
 netsim/cli/libvirt.py
 netsim/cli/read.py
+netsim/cli/report.py
 netsim/cli/restart.py
 netsim/cli/show.py
 netsim/cli/status.py
 netsim/cli/test.py
 netsim/cli/up.py
 netsim/cli/usage.py
 netsim/cli/usage.txt
@@ -403,29 +406,37 @@
 netsim/devices/vmx.py
 netsim/devices/vmx.yml
 netsim/devices/vptx.py
 netsim/devices/vptx.yml
 netsim/devices/vsrx.py
 netsim/devices/vsrx.yml
 netsim/devices/vyos.yml
+netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc
 netsim/extra/ebgp.utils/default-originate.yml
 netsim/extra/ebgp.utils/eos.j2
 netsim/extra/ebgp.utils/frr.j2
 netsim/extra/ebgp.utils/ios.j2
 netsim/extra/ebgp.utils/junos.j2
 netsim/extra/ebgp.utils/plugin.py
 netsim/extra/ebgp.utils/routeros7.j2
 netsim/extra/ebgp.utils/srlinux.j2
 netsim/extra/ebgp.utils/topology.yml
 netsim/extra/ebgp.utils/vyos.j2
+netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc
+netsim/extra/ebgp.utils/__pycache__/plugin.cpython-311.pyc
 netsim/extra/multilab/plugin.py
+netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc
+netsim/extra/multilab/__pycache__/plugin.cpython-311.pyc
 netsim/extra/none/none.j2
 netsim/extra/proxy-arp/plugin.py
 netsim/extra/proxy-arp/srlinux.j2
 netsim/extra/proxy-arp/sros.j2
+netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
+netsim/extra/proxy-arp/__pycache__/plugin.cpython-311.pyc
+netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
 netsim/install/ansible.sh
 netsim/install/containerlab.sh
 netsim/install/grpc.sh
 netsim/install/libvirt.sh
 netsim/install/ubuntu.sh
 netsim/install/libvirt/arubacx.txt
 netsim/install/libvirt/asav.txt
@@ -439,14 +450,15 @@
 netsim/install/libvirt/nxos.txt
 netsim/install/libvirt/nxos.xml.j2
 netsim/install/libvirt/routeros7.txt
 netsim/install/libvirt/vptx.txt
 netsim/install/libvirt/vptx.xml.j2
 netsim/install/libvirt/vsrx.txt
 netsim/install/libvirt/asav/day0-config
+netsim/install/libvirt/iosxr/iosxr_config.txt
 netsim/install/libvirt/vptx/juniper.conf
 netsim/install/libvirt/vptx/make-config.sh
 netsim/install/libvirt/vptx/run.sh
 netsim/install/libvirt/vsrx/juniper.conf
 netsim/modules/__init__.py
 netsim/modules/_dataplane.py
 netsim/modules/_routing.py
@@ -456,14 +468,15 @@
 netsim/modules/bgp.yml
 netsim/modules/eigrp.py
 netsim/modules/eigrp.yml
 netsim/modules/evpn.py
 netsim/modules/evpn.yml
 netsim/modules/gateway.py
 netsim/modules/gateway.yml
+netsim/modules/initial.yml
 netsim/modules/isis.py
 netsim/modules/isis.yml
 netsim/modules/mpls.py
 netsim/modules/mpls.yml
 netsim/modules/ospf.py
 netsim/modules/ospf.yml
 netsim/modules/sr.py
@@ -485,14 +498,15 @@
 netsim/outputs/format.py
 netsim/outputs/graph.py
 netsim/outputs/graph.yml
 netsim/outputs/graphite.py
 netsim/outputs/json.py
 netsim/outputs/none.py
 netsim/outputs/provider.py
+netsim/outputs/report.py
 netsim/outputs/tools.py
 netsim/outputs/yaml.py
 netsim/providers/__init__.py
 netsim/providers/clab.py
 netsim/providers/clab.yml
 netsim/providers/external.py
 netsim/providers/external.yml
@@ -544,14 +558,15 @@
 netsim/templates/tests/virtualbox.yml
 netsim/tools/__init__.py
 netsim/tools/graphite.py
 netsim/tools/graphite.yml
 netsim/tools/suzieq.yml
 netsim/tools/suzieq/suzieq-cfg.yml
 netsim/utils/__init__.py
+netsim/utils/files.py
 netsim/utils/log.py
 netsim/utils/status.py
 netsim/utils/strings.py
 netsim/utils/templates.py
 networklab.egg-info/PKG-INFO
 networklab.egg-info/SOURCES.txt
 networklab.egg-info/dependency_links.txt
```

### Comparing `networklab-1.5.4.post1/setup.py` & `networklab-1.5.5.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4.post1/tests/test_transformation.py` & `networklab-1.5.5.dev1/tests/test_transformation.py`

 * *Files identical despite different names*

