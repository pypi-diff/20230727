# Comparing `tmp/dtschema-2023.6.1.tar.gz` & `tmp/dtschema-2023.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtschema-2023.6.1.tar", last modified: Tue Jun 27 22:17:29 2023, max compression
+gzip compressed data, was "dtschema-2023.7.tar", last modified: Thu Jul 27 21:39:53 2023, max compression
```

## Comparing `dtschema-2023.6.1.tar` & `dtschema-2023.7.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.187602 dtschema-2023.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.163601 dtschema-2023.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.171601 dtschema-2023.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-27 22:17:17.000000 dtschema-2023.6.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 22:17:17.000000 dtschema-2023.6.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 22:17:17.000000 dtschema-2023.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-27 22:17:17.000000 dtschema-2023.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-27 22:17:29.187602 dtschema-2023.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-27 22:17:17.000000 dtschema-2023.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.171601 dtschema-2023.6.1/dtschema/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15065 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/dtb.py
--rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/fixups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.175602 dtschema-2023.6.1/dtschema/meta-schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/boolean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/cell.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/clocks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/core.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/dma.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/gpios.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/hwlock.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/iio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/interrupts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/iommu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/items.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/keywords.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/mailbox.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/nodes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/nvmem.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/phy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/power-domain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/pwm.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/reset.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/string-array.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/meta-schemas/vendor-props.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.179602 dtschema-2023.6.1/dtschema/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/aliases.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/bootph.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.179602 dtschema-2023.6.1/dtschema/schemas/bus/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/bus/qemu,platform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/cache-controller.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/cache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9188 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/chosen.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.179602 dtschema-2023.6.1/dtschema/schemas/clock/
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/clock/clock.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/cpu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/cpus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.179602 dtschema-2023.6.1/dtschema/schemas/dma/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/dma/dma.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/dt-core.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.179602 dtschema-2023.6.1/dtschema/schemas/gpio/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/gpio/gpio-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/gpio/gpio-hog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/gpio/gpio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/graph.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.179602 dtschema-2023.6.1/dtschema/schemas/hwlock/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/hwlock/hwlock-consumer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.179602 dtschema-2023.6.1/dtschema/schemas/i2c/
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/i2c/i2c-controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.179602 dtschema-2023.6.1/dtschema/schemas/iio/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/iio/iio-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/iio/iio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/interconnects.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/interrupt-controller.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/interrupts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.179602 dtschema-2023.6.1/dtschema/schemas/iommu/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/iommu/iommu.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.179602 dtschema-2023.6.1/dtschema/schemas/isa/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/isa/isa-bridge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/isa/isa-bus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.179602 dtschema-2023.6.1/dtschema/schemas/mbox/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/mbox/mbox-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/memory.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/msi-consumer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.179602 dtschema-2023.6.1/dtschema/schemas/opp/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/opp/opp.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.179602 dtschema-2023.6.1/dtschema/schemas/options/
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/options/u-boot.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/options.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.183602 dtschema-2023.6.1/dtschema/schemas/pci/
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/pci/pci-bus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/pci/pci-iommu.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.183602 dtschema-2023.6.1/dtschema/schemas/phy/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/phy/phy-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/phy/phy-provider.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.183602 dtschema-2023.6.1/dtschema/schemas/pinctrl/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/pinctrl/pinctrl-consumer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.183602 dtschema-2023.6.1/dtschema/schemas/power-domain/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/power-domain/power-domain-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/property-units.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.183602 dtschema-2023.6.1/dtschema/schemas/pwm/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/pwm/pwm-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/reg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.183602 dtschema-2023.6.1/dtschema/schemas/reset/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/reset/reset.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/root-node.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/serial.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/simple-bus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/schemas/types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-06-27 22:17:17.000000 dtschema-2023.6.1/dtschema/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-27 22:17:29.000000 dtschema-2023.6.1/dtschema/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.175602 dtschema-2023.6.1/dtschema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-27 22:17:29.000000 dtschema-2023.6.1/dtschema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-27 22:17:29.000000 dtschema-2023.6.1/dtschema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:17:29.000000 dtschema-2023.6.1/dtschema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 22:17:29.000000 dtschema-2023.6.1/dtschema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 22:17:29.000000 dtschema-2023.6.1/dtschema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-27 22:17:17.000000 dtschema-2023.6.1/example-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:17:29.187602 dtschema-2023.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-06-27 22:17:17.000000 dtschema-2023.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.183602 dtschema-2023.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/bootphases.dts
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/child-node-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/child-node.dts
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/conditionals-allof-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/conditionals-allof-pass.dts
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/conditionals-single-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/conditionals-single-pass.dts
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/device-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/device.dts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.183602 dtschema-2023.6.1/test/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/schemas/bad-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/schemas/child-node-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/schemas/conditionals-allof-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/schemas/conditionals-single-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/schemas/good-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/simple-bus-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/simple-bus-pass.dts
--rwxr-xr-x   0 runner    (1001) docker     (123)     5664 2023-06-27 22:17:17.000000 dtschema-2023.6.1/test/test-dt-validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:17:29.187602 dtschema-2023.6.1/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1333 2023-06-27 22:17:17.000000 dtschema-2023.6.1/tools/dt-check-compatible
--rwxr-xr-x   0 runner    (1001) docker     (123)     2070 2023-06-27 22:17:17.000000 dtschema-2023.6.1/tools/dt-doc-validate
--rwxr-xr-x   0 runner    (1001) docker     (123)     2628 2023-06-27 22:17:17.000000 dtschema-2023.6.1/tools/dt-extract-example
--rwxr-xr-x   0 runner    (1001) docker     (123)     1916 2023-06-27 22:17:17.000000 dtschema-2023.6.1/tools/dt-extract-props
--rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-06-27 22:17:17.000000 dtschema-2023.6.1/tools/dt-mk-schema
--rwxr-xr-x   0 runner    (1001) docker     (123)     6206 2023-06-27 22:17:17.000000 dtschema-2023.6.1/tools/dt-prop-populate
--rwxr-xr-x   0 runner    (1001) docker     (123)     5314 2023-06-27 22:17:17.000000 dtschema-2023.6.1/tools/dt-validate
--rwxr-xr-x   0 runner    (1001) docker     (123)     1321 2023-06-27 22:17:17.000000 dtschema-2023.6.1/tools/dtb2py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-06-27 22:17:17.000000 dtschema-2023.6.1/tools/extract-compatibles
--rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-06-27 22:17:17.000000 dtschema-2023.6.1/tools/yaml-format
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-06-27 22:17:17.000000 dtschema-2023.6.1/tools/yaml2json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.304646 dtschema-2023.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.276646 dtschema-2023.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.284646 dtschema-2023.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-27 21:39:39.000000 dtschema-2023.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-27 21:39:39.000000 dtschema-2023.7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 21:39:39.000000 dtschema-2023.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-27 21:39:39.000000 dtschema-2023.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-27 21:39:53.304646 dtschema-2023.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-27 21:39:39.000000 dtschema-2023.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.284646 dtschema-2023.7/dtschema/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15065 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/dtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/fixups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.288646 dtschema-2023.7/dtschema/meta-schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/boolean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/cell.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/clocks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/core.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/dma.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/gpios.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/hwlock.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/iio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/interrupts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/iommu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/items.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/keywords.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/mailbox.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/nodes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/nvmem.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/phy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/power-domain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/pwm.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/reset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/string-array.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/meta-schemas/vendor-props.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.292646 dtschema-2023.7/dtschema/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/aliases.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/bootph.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.292646 dtschema-2023.7/dtschema/schemas/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/bus/qemu,platform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/cache-controller.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/cache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9188 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/chosen.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.292646 dtschema-2023.7/dtschema/schemas/clock/
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/clock/clock.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/cpus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.292646 dtschema-2023.7/dtschema/schemas/dma/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/dma/dma.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/dt-core.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/gpio/gpio-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/gpio/gpio-hog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/gpio/gpio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/graph.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/hwlock/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/hwlock/hwlock-consumer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/i2c/
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/i2c/i2c-controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/iio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/iio/iio-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/iio/iio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/interconnects.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/interrupt-controller.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/interrupts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/iommu/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/iommu/iommu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/isa/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/isa/isa-bridge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/isa/isa-bus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/mbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/mbox/mbox-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/memory.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/msi-consumer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/opp/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/opp/opp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/options/u-boot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/options.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/pci/
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/pci/pci-bus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/pci/pci-iommu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/phy/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/phy/phy-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/phy/phy-provider.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/pinctrl/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/pinctrl/pinctrl-consumer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/power-domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/power-domain/power-domain-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/property-units.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/pwm/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/pwm/pwm-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/reg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.296646 dtschema-2023.7/dtschema/schemas/reset/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/reset/reset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/root-node.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/serial.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/simple-bus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/schemas/types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-07-27 21:39:39.000000 dtschema-2023.7/dtschema/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 21:39:53.000000 dtschema-2023.7/dtschema/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.284646 dtschema-2023.7/dtschema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-27 21:39:53.000000 dtschema-2023.7/dtschema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-27 21:39:53.000000 dtschema-2023.7/dtschema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:39:53.000000 dtschema-2023.7/dtschema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 21:39:53.000000 dtschema-2023.7/dtschema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 21:39:53.000000 dtschema-2023.7/dtschema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-27 21:39:39.000000 dtschema-2023.7/example-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:39:53.304646 dtschema-2023.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-07-27 21:39:39.000000 dtschema-2023.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.300646 dtschema-2023.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-27 21:39:39.000000 dtschema-2023.7/test/bootphases.dts
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-27 21:39:39.000000 dtschema-2023.7/test/child-node-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-27 21:39:39.000000 dtschema-2023.7/test/child-node.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-27 21:39:39.000000 dtschema-2023.7/test/conditionals-allof-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-27 21:39:39.000000 dtschema-2023.7/test/conditionals-allof-pass.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-27 21:39:39.000000 dtschema-2023.7/test/conditionals-single-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-27 21:39:39.000000 dtschema-2023.7/test/conditionals-single-pass.dts
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-27 21:39:39.000000 dtschema-2023.7/test/device-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-27 21:39:39.000000 dtschema-2023.7/test/device.dts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.300646 dtschema-2023.7/test/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-27 21:39:39.000000 dtschema-2023.7/test/schemas/bad-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-27 21:39:39.000000 dtschema-2023.7/test/schemas/child-node-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-27 21:39:39.000000 dtschema-2023.7/test/schemas/conditionals-allof-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-27 21:39:39.000000 dtschema-2023.7/test/schemas/conditionals-single-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-27 21:39:39.000000 dtschema-2023.7/test/schemas/good-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-27 21:39:39.000000 dtschema-2023.7/test/simple-bus-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-27 21:39:39.000000 dtschema-2023.7/test/simple-bus-pass.dts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5664 2023-07-27 21:39:39.000000 dtschema-2023.7/test/test-dt-validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:53.304646 dtschema-2023.7/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1333 2023-07-27 21:39:39.000000 dtschema-2023.7/tools/dt-check-compatible
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2070 2023-07-27 21:39:39.000000 dtschema-2023.7/tools/dt-doc-validate
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2628 2023-07-27 21:39:39.000000 dtschema-2023.7/tools/dt-extract-example
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1916 2023-07-27 21:39:39.000000 dtschema-2023.7/tools/dt-extract-props
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-07-27 21:39:39.000000 dtschema-2023.7/tools/dt-mk-schema
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6206 2023-07-27 21:39:39.000000 dtschema-2023.7/tools/dt-prop-populate
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5633 2023-07-27 21:39:39.000000 dtschema-2023.7/tools/dt-validate
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1321 2023-07-27 21:39:39.000000 dtschema-2023.7/tools/dtb2py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-07-27 21:39:39.000000 dtschema-2023.7/tools/extract-compatibles
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-07-27 21:39:39.000000 dtschema-2023.7/tools/yaml-format
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-07-27 21:39:39.000000 dtschema-2023.7/tools/yaml2json
```

### Comparing `dtschema-2023.6.1/.github/workflows/ci.yml` & `dtschema-2023.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/.github/workflows/publish.yml` & `dtschema-2023.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/LICENSE.txt` & `dtschema-2023.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/PKG-INFO` & `dtschema-2023.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtschema
-Version: 2023.6.1
+Version: 2023.7
 Summary: DeviceTree validation schema and tools
 Home-page: https://github.com/devicetree-org/dt-schema
 Author: Rob Herring
 Author-email: robh@kernel.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dtschema-2023.6.1/README.md` & `dtschema-2023.7/README.md`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/dtb.py` & `dtschema-2023.7/dtschema/dtb.py`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/fixups.py` & `dtschema-2023.7/dtschema/fixups.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,58 +329,57 @@
 
 known_variable_matrix_props = {
     'fsl,pins',
     'qcom,board-id'
 }
 
 
-def fixup_sub_schema(schema, is_prop):
+def fixup_sub_schema(schema):
     if not isinstance(schema, dict):
         return
 
     schema.pop('description', None)
     fixup_interrupts(schema)
-    if is_prop:
-        fixup_node_props(schema)
+    fixup_node_props(schema)
 
     # 'additionalProperties: true' doesn't work with 'unevaluatedProperties', so
     # remove it. It's in the schemas for common (incomplete) schemas.
     if 'additionalProperties' in schema and schema['additionalProperties'] == True:
         schema.pop('additionalProperties', None)
 
     for k, v in schema.items():
-        if k in ['select', 'if', 'then', 'else', 'additionalProperties', 'not']:
-            fixup_sub_schema(v, False)
+        if k in ['select', 'if', 'then', 'else', 'not', 'additionalProperties']:
+            fixup_sub_schema(v)
 
         if k in ['allOf', 'anyOf', 'oneOf']:
             for subschema in v:
-                fixup_sub_schema(subschema, True)
+                fixup_sub_schema(subschema)
 
         if k not in ['dependentRequired', 'dependentSchemas', 'dependencies', 'properties', 'patternProperties', '$defs']:
             continue
 
         for prop in v:
             if prop in known_variable_matrix_props and isinstance(v[prop], dict):
                 ref = v[prop].pop('$ref', None)
                 schema[k][prop] = {}
                 if ref:
                     schema[k][prop]['$ref'] = ref
                 continue
 
             walk_properties(prop, v[prop])
             # Recurse to check for {properties,patternProperties} in each prop
-            fixup_sub_schema(v[prop], True)
+            fixup_sub_schema(v[prop])
 
     fixup_schema_to_201909(schema)
 
 
 def fixup_node_props(schema):
-    if not {'properties', 'patternProperties', 'unevaluatedProperties', 'additionalProperties'} & schema.keys():
-        return
-    if ('additionalProperties' in schema and schema['additionalProperties'] is True) or \
+    # If no restrictions on undefined properties, then no need to add any implicit properties
+    if (not {'unevaluatedProperties', 'additionalProperties'} & schema.keys()) or \
+       ('additionalProperties' in schema and schema['additionalProperties'] is True) or \
        ('unevaluatedProperties' in schema and schema['unevaluatedProperties'] is True):
         return
 
     schema.setdefault('properties', dict())
     schema['properties'].setdefault('phandle', True)
     schema['properties'].setdefault('status', True)
     schema['properties'].setdefault('secure-status', True)
@@ -477,8 +476,8 @@
 def fixup_schema(schema):
     # Remove parts not necessary for validation
     schema.pop('examples', None)
     schema.pop('maintainers', None)
     schema.pop('historical', None)
 
     add_select_schema(schema)
-    fixup_sub_schema(schema, True)
+    fixup_sub_schema(schema)
```

### Comparing `dtschema-2023.6.1/dtschema/lib.py` & `dtschema-2023.7/dtschema/lib.py`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/meta-schemas/base.yaml` & `dtschema-2023.7/dtschema/meta-schemas/base.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/meta-schemas/cell.yaml` & `dtschema-2023.7/dtschema/meta-schemas/cell.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/meta-schemas/clocks.yaml` & `dtschema-2023.7/dtschema/meta-schemas/clocks.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/meta-schemas/core.yaml` & `dtschema-2023.7/dtschema/meta-schemas/core.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/meta-schemas/gpios.yaml` & `dtschema-2023.7/dtschema/meta-schemas/gpios.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/meta-schemas/interrupts.yaml` & `dtschema-2023.7/dtschema/meta-schemas/interrupts.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/meta-schemas/items.yaml` & `dtschema-2023.7/dtschema/meta-schemas/items.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/meta-schemas/keywords.yaml` & `dtschema-2023.7/dtschema/meta-schemas/keywords.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -83,18 +83,23 @@
     $ref: "#/definitions/scalar-prop-list"
   maxItems:
     $ref: "#/definitions/scalar-prop-list"
   minItems:
     $ref: "#/definitions/scalar-prop-list"
   additionalProperties:
     description: "'additionalProperties' depends on 'properties' or 'patternProperties'"
-    anyOf:
-      - required: [ type ]
-      - required: [ properties ]
-      - required: [ patternProperties ]
+    if:
+      properties:
+        additionalProperties:
+            type: boolean
+    then:
+      anyOf:
+        - required: [ type ]
+        - required: [ properties ]
+        - required: [ patternProperties ]
 
 dependentRequired:
   # Ensure only valid combinations of if/then/else are present
   if:
     - then
   then:
     - if
```

### Comparing `dtschema-2023.6.1/dtschema/meta-schemas/nodes.yaml` & `dtschema-2023.7/dtschema/meta-schemas/nodes.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/meta-schemas/string-array.yaml` & `dtschema-2023.7/dtschema/meta-schemas/string-array.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/meta-schemas/vendor-props.yaml` & `dtschema-2023.7/dtschema/meta-schemas/vendor-props.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schema.py` & `dtschema-2023.7/dtschema/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,32 +97,25 @@
         for e in error.context:
             self.annotate_error(e, schema, path + e.schema_path)
 
         scope = self.validator.ID_OF(schema)
         self.validator.resolver.push_scope(scope)
         ref_depth = 1
 
-        lastp = ''
         for p in path:
-            # json-schema 3.2.0 includes 'if' in schema path
-            if lastp != 'properties' and p == 'if':
-                continue
-            lastp = p
-
             while '$ref' in schema and isinstance(schema['$ref'], str):
                 ref = self.validator.resolver.resolve(schema['$ref'])
                 schema = ref[1]
                 self.validator.resolver.push_scope(ref[0])
                 ref_depth += 1
 
             if '$id' in schema and isinstance(schema['$id'], str):
                 error.schema_file = schema['$id']
 
-            if p in schema:
-                schema = schema[p]
+            schema = schema[p]
 
             if isinstance(schema, dict):
                 if 'description' in schema and isinstance(schema['description'], str):
                     error.note = schema['description']
 
         while ref_depth > 0:
             self.validator.resolver.pop_scope()
```

### Comparing `dtschema-2023.6.1/dtschema/schemas/aliases.yaml` & `dtschema-2023.7/dtschema/schemas/aliases.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/bootph.yaml` & `dtschema-2023.7/dtschema/schemas/bootph.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/bus/qemu,platform.yaml` & `dtschema-2023.7/dtschema/schemas/bus/qemu,platform.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/cache-controller.yaml` & `dtschema-2023.7/dtschema/schemas/cache-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/cache.yaml` & `dtschema-2023.7/dtschema/schemas/cache.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/chosen.yaml` & `dtschema-2023.7/dtschema/schemas/chosen.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/clock/clock.yaml` & `dtschema-2023.7/dtschema/schemas/clock/clock.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/cpu.yaml` & `dtschema-2023.7/dtschema/schemas/cpu.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/cpus.yaml` & `dtschema-2023.7/dtschema/schemas/cpus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/dt-core.yaml` & `dtschema-2023.7/dtschema/schemas/dt-core.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/gpio/gpio-consumer.yaml` & `dtschema-2023.7/dtschema/schemas/gpio/gpio-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/gpio/gpio-hog.yaml` & `dtschema-2023.7/dtschema/schemas/gpio/gpio-hog.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/gpio/gpio.yaml` & `dtschema-2023.7/dtschema/schemas/gpio/gpio.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/graph.yaml` & `dtschema-2023.7/dtschema/schemas/graph.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/hwlock/hwlock-consumer.yaml` & `dtschema-2023.7/dtschema/schemas/hwlock/hwlock-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/i2c/i2c-controller.yaml` & `dtschema-2023.7/dtschema/schemas/i2c/i2c-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/iio/iio-consumer.yaml` & `dtschema-2023.7/dtschema/schemas/iio/iio-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/iio/iio.yaml` & `dtschema-2023.7/dtschema/schemas/iio/iio.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/interrupt-controller.yaml` & `dtschema-2023.7/dtschema/schemas/interrupt-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/interrupts.yaml` & `dtschema-2023.7/dtschema/schemas/interrupts.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/isa/isa-bridge.yaml` & `dtschema-2023.7/dtschema/schemas/isa/isa-bridge.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/isa/isa-bus.yaml` & `dtschema-2023.7/dtschema/schemas/isa/isa-bus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/mbox/mbox-consumer.yaml` & `dtschema-2023.7/dtschema/schemas/mbox/mbox-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/memory.yaml` & `dtschema-2023.7/dtschema/schemas/memory.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/msi-consumer.yaml` & `dtschema-2023.7/dtschema/schemas/msi-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/opp/opp.yaml` & `dtschema-2023.7/dtschema/schemas/opp/opp.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/options/u-boot.yaml` & `dtschema-2023.7/dtschema/schemas/options/u-boot.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/options.yaml` & `dtschema-2023.7/dtschema/schemas/options.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/pci/pci-bus.yaml` & `dtschema-2023.7/dtschema/schemas/pci/pci-bus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/pci/pci-iommu.yaml` & `dtschema-2023.7/dtschema/schemas/pci/pci-iommu.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/phy/phy-consumer.yaml` & `dtschema-2023.7/dtschema/schemas/phy/phy-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/phy/phy-provider.yaml` & `dtschema-2023.7/dtschema/schemas/phy/phy-provider.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/pinctrl/pinctrl-consumer.yaml` & `dtschema-2023.7/dtschema/schemas/pinctrl/pinctrl-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/power-domain/power-domain-consumer.yaml` & `dtschema-2023.7/dtschema/schemas/power-domain/power-domain-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/property-units.yaml` & `dtschema-2023.7/dtschema/schemas/property-units.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -34,19 +34,19 @@
     description: number of bits
 
   "-kBps$":
     $ref: types.yaml#/definitions/uint32-array
     description: kilobytes per second
 
   "-percent$":
-    $ref: types.yaml#/definitions/uint32-array
+    $ref: types.yaml#/definitions/int32-array
     description: percentage
 
   "-bp$":
-    $ref: types.yaml#/definitions/uint32-array
+    $ref: types.yaml#/definitions/int32-array
     description: basis points (1/100 of a percent)
 
   # Time/Frequency
   "-mhz$":
     $ref: types.yaml#/definitions/uint32-array
     description: megahertz
   "(^(?!opp)).*-hz$":
```

### Comparing `dtschema-2023.6.1/dtschema/schemas/pwm/pwm-consumer.yaml` & `dtschema-2023.7/dtschema/schemas/pwm/pwm-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/reg.yaml` & `dtschema-2023.7/dtschema/schemas/reg.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/reset/reset.yaml` & `dtschema-2023.7/dtschema/schemas/reset/reset.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/root-node.yaml` & `dtschema-2023.7/dtschema/schemas/root-node.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/simple-bus.yaml` & `dtschema-2023.7/dtschema/schemas/simple-bus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/schemas/types.yaml` & `dtschema-2023.7/dtschema/schemas/types.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema/validator.py` & `dtschema-2023.7/dtschema/validator.py`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/dtschema.egg-info/PKG-INFO` & `dtschema-2023.7/dtschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtschema
-Version: 2023.6.1
+Version: 2023.7
 Summary: DeviceTree validation schema and tools
 Home-page: https://github.com/devicetree-org/dt-schema
 Author: Rob Herring
 Author-email: robh@kernel.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dtschema-2023.6.1/dtschema.egg-info/SOURCES.txt` & `dtschema-2023.7/dtschema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/example-schema.yaml` & `dtschema-2023.7/example-schema.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/setup.py` & `dtschema-2023.7/setup.py`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/child-node-fail.dts` & `dtschema-2023.7/test/child-node-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/child-node.dts` & `dtschema-2023.7/test/child-node.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/conditionals-allof-fail.dts` & `dtschema-2023.7/test/conditionals-allof-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/conditionals-allof-pass.dts` & `dtschema-2023.7/test/conditionals-allof-pass.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/conditionals-single-fail.dts` & `dtschema-2023.7/test/conditionals-single-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/device-fail.dts` & `dtschema-2023.7/test/device-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/device.dts` & `dtschema-2023.7/test/device.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/schemas/bad-example.yaml` & `dtschema-2023.7/test/schemas/bad-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/schemas/child-node-example.yaml` & `dtschema-2023.7/test/schemas/child-node-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/schemas/conditionals-allof-example.yaml` & `dtschema-2023.7/test/schemas/conditionals-allof-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/schemas/conditionals-single-example.yaml` & `dtschema-2023.7/test/schemas/conditionals-single-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/schemas/good-example.yaml` & `dtschema-2023.7/test/schemas/good-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/simple-bus-pass.dts` & `dtschema-2023.7/test/simple-bus-pass.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/test/test-dt-validate.py` & `dtschema-2023.7/test/test-dt-validate.py`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/tools/dt-check-compatible` & `dtschema-2023.7/tools/dt-check-compatible`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/tools/dt-doc-validate` & `dtschema-2023.7/tools/dt-doc-validate`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/tools/dt-extract-example` & `dtschema-2023.7/tools/dt-extract-example`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/tools/dt-extract-props` & `dtschema-2023.7/tools/dt-extract-props`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/tools/dt-mk-schema` & `dtschema-2023.7/tools/dt-mk-schema`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/tools/dt-prop-populate` & `dtschema-2023.7/tools/dt-prop-populate`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/tools/dt-validate` & `dtschema-2023.7/tools/dt-validate`

 * *Files 5% similar despite different names*

```diff
@@ -98,29 +98,35 @@
 if __name__ == "__main__":
     ap = argparse.ArgumentParser(fromfile_prefix_chars='@',
         epilog='Arguments can also be passed in a file prefixed with a "@" character.')
     ap.add_argument("dtbs", nargs='*',
                     help="Filename or directory of devicetree DTB input file(s)")
     ap.add_argument('-s', '--schema', help="preparsed schema file or path to schema files")
     ap.add_argument('-p', '--preparse', help="preparsed schema file (deprecated, use '-s')")
-    ap.add_argument('-l', '--limit', help="limit validation to schema files matching substring")
+    ap.add_argument('-l', '--limit', help="limit validation to schemas with $id matching LIMIT substring")
     ap.add_argument('-m', '--show-unmatched',
         help="Print out node 'compatible' strings which don't match any schema.",
         action="store_true")
     ap.add_argument('-n', '--line-number', help="Obsolete", action="store_true")
     ap.add_argument('-v', '--verbose', help="verbose mode", action="store_true")
-    ap.add_argument('-u', '--url-path', help="Additional search path for references")
+    ap.add_argument('-u', '--url-path', help="Additional search path for references (deprecated)")
     ap.add_argument('-V', '--version', help="Print version number",
                     action="version", version=dtschema.__version__)
     args = ap.parse_args()
 
     verbose = args.verbose
     show_unmatched = args.show_unmatched
     match_schema_file = args.limit
 
+    # Maintain prior behaviour which accepted file paths by stripping the file path
+    if args.url_path and args.limit:
+        for d in args.url_path.split(os.path.sep):
+            if d and match_schema_file.startswith(d):
+                match_schema_file = match_schema_file[(len(d) + 1):]
+
     if args.preparse:
         sg = schema_group(args.preparse)
     elif args.schema:
         sg = schema_group(args.schema)
     else:
         sg = schema_group()
```

### Comparing `dtschema-2023.6.1/tools/dtb2py` & `dtschema-2023.7/tools/dtb2py`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/tools/extract-compatibles` & `dtschema-2023.7/tools/extract-compatibles`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/tools/yaml-format` & `dtschema-2023.7/tools/yaml-format`

 * *Files identical despite different names*

### Comparing `dtschema-2023.6.1/tools/yaml2json` & `dtschema-2023.7/tools/yaml2json`

 * *Files identical despite different names*

