# Comparing `tmp/pyaedt-0.6.86.tar.gz` & `tmp/pyaedt-0.6.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.86.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyaedt-0.6.87.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.6.86.tar` & `pyaedt-0.6.87.tar`

### file list

```diff
@@ -1,259 +1,259 @@
--rw-r--r--   0        0        0     1111 2023-05-30 06:59:37.486926 pyaedt-0.6.86/LICENSE
--rw-r--r--   0        0        0     9947 2023-05-30 06:59:37.486926 pyaedt-0.6.86/README.md
--rw-r--r--   0        0        0     2629 2023-07-21 14:33:51.388714 pyaedt-0.6.86/pyaedt/__init__.py
--rw-r--r--   0        0        0    26756 2023-07-21 09:35:13.229002 pyaedt-0.6.86/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-05-30 06:59:39.408947 pyaedt-0.6.86/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    88967 2023-07-21 09:35:13.229002 pyaedt-0.6.86/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    50696 2023-07-21 09:35:13.229002 pyaedt-0.6.86/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17066 2023-06-20 15:35:24.349674 pyaedt-0.6.86/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-05-30 06:59:39.408947 pyaedt-0.6.86/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19948 2023-07-19 13:20:21.575376 pyaedt-0.6.86/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4431 2023-05-30 06:59:39.408947 pyaedt-0.6.86/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4596 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   136452 2023-07-21 09:35:13.229002 pyaedt-0.6.86/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    75793 2023-07-20 11:48:09.458225 pyaedt-0.6.86/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12464 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    36750 2023-06-29 09:15:20.741006 pyaedt-0.6.86/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    62949 2023-07-21 09:35:13.229002 pyaedt-0.6.86/pyaedt/circuit.py
--rw-r--r--   0        0        0    10259 2023-07-20 07:33:55.805436 pyaedt-0.6.86/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    84793 2023-07-21 09:35:13.229002 pyaedt-0.6.86/pyaedt/desktop.py
--rw-r--r--   0        0        0    15104 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/dlls/PDFReport/AnsysReport.deps.json
--rw-r--r--   0        0        0    23552 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1086 2023-06-28 08:36:59.983528 pyaedt-0.6.86/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0   204800 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
--rw-r--r--   0        0        0   577445 2023-05-30 06:59:39.440208 pyaedt-0.6.86/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
--rw-r--r--   0        0        0     9836 2023-05-30 06:59:39.440208 pyaedt-0.6.86/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   238592 2023-05-30 06:59:39.440208 pyaedt-0.6.86/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
--rw-r--r--   0        0        0   115712 2023-05-30 06:59:39.440208 pyaedt-0.6.86/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
--rw-r--r--   0        0        0   705296 2023-05-30 06:59:39.455836 pyaedt-0.6.86/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   712253 2023-05-30 06:59:39.455836 pyaedt-0.6.86/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0    80384 2023-05-30 06:59:39.455836 pyaedt-0.6.86/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
--rw-r--r--   0        0        0   546816 2023-05-30 06:59:39.471459 pyaedt-0.6.86/pyaedt/dlls/PDFReport/PdfSharpCore.dll
--rw-r--r--   0        0        0   367616 2023-05-30 06:59:39.471459 pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
--rw-r--r--   0        0        0   536367 2023-05-30 06:59:39.471459 pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
--rw-r--r--   0        0        0  1229824 2023-05-30 06:59:39.487088 pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
--rw-r--r--   0        0        0  3285773 2023-05-30 06:59:39.502713 pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
--rw-r--r--   0        0        0   120664 2023-05-30 06:59:39.502713 pyaedt-0.6.86/pyaedt/dlls/PDFReport/System.Runtime.dll
--rw-r--r--   0        0        0  1505294 2023-05-30 06:59:39.518353 pyaedt-0.6.86/pyaedt/dlls/PDFReport/System.Runtime.xml
--rw-r--r--   0        0        0     5632 2023-05-30 06:59:39.518353 pyaedt-0.6.86/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
--rw-r--r--   0        0        0   160754 2023-05-30 06:59:39.533962 pyaedt-0.6.86/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
--rw-r--r--   0        0        0    24188 2023-07-21 12:41:58.329803 pyaedt-0.6.86/pyaedt/downloads.py
--rw-r--r--   0        0        0   137623 2023-06-29 17:19:45.292504 pyaedt-0.6.86/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-05-30 06:59:39.533962 pyaedt-0.6.86/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    98675 2023-07-13 12:00:19.155166 pyaedt-0.6.86/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-06-05 09:36:43.922575 pyaedt-0.6.86/pyaedt/edb_core/dotnet/__init__.py
--rw-r--r--   0        0        0    31509 2023-07-20 07:33:55.805436 pyaedt-0.6.86/pyaedt/edb_core/dotnet/database.py
--rw-r--r--   0        0        0     7909 2023-06-05 09:36:43.938202 pyaedt-0.6.86/pyaedt/edb_core/dotnet/layout.py
--rw-r--r--   0        0        0    48210 2023-06-05 09:36:43.938202 pyaedt-0.6.86/pyaedt/edb_core/dotnet/primitive.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.533962 pyaedt-0.6.86/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    33195 2023-06-12 08:05:31.703949 pyaedt-0.6.86/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0    40112 2023-07-20 12:55:34.842217 pyaedt-0.6.86/pyaedt/edb_core/edb_data/control_file.py
--rw-r--r--   0        0        0      937 2023-05-30 06:59:39.533962 pyaedt-0.6.86/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      867 2023-05-30 06:59:39.533962 pyaedt-0.6.86/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    12243 2023-06-05 09:36:43.938202 pyaedt-0.6.86/pyaedt/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    65661 2023-06-05 09:36:43.938202 pyaedt-0.6.86/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20820 2023-07-17 10:14:12.806355 pyaedt-0.6.86/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     6880 2023-07-21 11:59:44.723243 pyaedt-0.6.86/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    61171 2023-07-21 12:41:58.329803 pyaedt-0.6.86/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    32590 2023-06-29 16:47:26.445610 pyaedt-0.6.86/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0   102298 2023-06-14 08:50:43.463988 pyaedt-0.6.86/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36324 2023-06-05 09:36:43.938202 pyaedt-0.6.86/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    34944 2023-07-10 08:39:13.777984 pyaedt-0.6.86/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     3923 2023-06-05 14:54:59.781956 pyaedt-0.6.86/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2432 2023-06-05 09:36:43.938202 pyaedt-0.6.86/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     3258 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    68725 2023-06-29 11:46:59.997639 pyaedt-0.6.86/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2850 2023-06-05 09:36:43.953828 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7763 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4703 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11390 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-05-30 06:59:39.580847 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21800 2023-06-05 09:36:43.953828 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-05-30 06:59:39.580847 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    47176 2023-06-22 08:21:07.514633 pyaedt-0.6.86/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33310 2023-06-05 09:36:43.953828 pyaedt-0.6.86/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    44030 2023-07-21 11:59:44.723243 pyaedt-0.6.86/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    49394 2023-07-21 11:24:42.095565 pyaedt-0.6.86/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    58809 2023-06-19 10:47:11.266974 pyaedt-0.6.86/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   111074 2023-07-17 10:14:12.806355 pyaedt-0.6.86/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    11500 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/emit.py
--rw-r--r--   0        0        0     6100 2023-07-06 12:50:33.852654 pyaedt-0.6.86/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     2825 2023-07-20 07:33:55.805436 pyaedt-0.6.86/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0     1621 2023-06-13 17:56:07.965688 pyaedt-0.6.86/pyaedt/emit_core/emit_constants.py
--rw-r--r--   0        0        0    11102 2023-07-21 12:41:58.329803 pyaedt-0.6.86/pyaedt/emit_core/interference_classification.py
--rw-r--r--   0        0        0        2 2023-05-30 06:59:39.580847 pyaedt-0.6.86/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7406 2023-07-06 12:50:33.852654 pyaedt-0.6.86/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    13896 2023-07-06 12:50:33.852654 pyaedt-0.6.86/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-05-30 06:59:39.580847 pyaedt-0.6.86/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    12252 2023-06-21 12:50:18.007016 pyaedt-0.6.86/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.580847 pyaedt-0.6.86/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3257 2023-05-30 06:59:39.580847 pyaedt-0.6.86/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83443 2023-07-20 11:48:09.458225 pyaedt-0.6.86/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    21891 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3442 2023-07-13 12:00:19.155166 pyaedt-0.6.86/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    71208 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0     9410 2023-07-20 12:33:36.682607 pyaedt-0.6.86/pyaedt/generic/grpc_plugin.py
--rw-r--r--   0        0        0     3043 2023-07-11 14:47:17.448018 pyaedt-0.6.86/pyaedt/generic/grpc_plugin_dll.py
--rw-r--r--   0        0        0    25808 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     7029 2023-07-13 12:00:19.155166 pyaedt-0.6.86/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0     9795 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    62327 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11405 2023-06-22 08:21:07.514633 pyaedt-0.6.86/pyaedt/generic/process.py
--rw-r--r--   0        0        0    20326 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3536 2023-06-21 12:50:18.007016 pyaedt-0.6.86/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60412 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17095 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   255506 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/hfss.py
--rw-r--r--   0        0        0    84753 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   200361 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/icepak.py
--rw-r--r--   0        0        0   127831 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7803 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24372 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3972 2023-07-07 09:12:05.234128 pyaedt-0.6.86/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     3311 2023-07-07 09:12:05.234128 pyaedt-0.6.86/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10210 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     2620 2023-07-05 06:36:09.681010 pyaedt-0.6.86/pyaedt/misc/ansys_cloud.areg
--rw-r--r--   0        0        0     3731 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     5611 2023-07-07 06:30:25.350901 pyaedt-0.6.86/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14107 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    20051 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16840 2023-05-30 06:59:39.643351 pyaedt-0.6.86/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120896 2023-07-13 12:00:19.170793 pyaedt-0.6.86/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   199311 2023-07-21 14:10:56.134350 pyaedt-0.6.86/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   116735 2023-07-13 12:00:19.170793 pyaedt-0.6.86/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11407 2023-07-13 12:00:19.170793 pyaedt-0.6.86/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   129702 2023-07-13 12:00:19.170793 pyaedt-0.6.86/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.643351 pyaedt-0.6.86/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    38322 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49140 2023-07-13 12:00:19.170793 pyaedt-0.6.86/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59316 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53078 2023-07-11 14:47:17.463644 pyaedt-0.6.86/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12661 2023-07-19 13:20:21.575376 pyaedt-0.6.86/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    43135 2023-07-14 12:01:50.451661 pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    33551 2023-07-06 12:50:33.852654 pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8236 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    63132 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15185 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.86/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    31781 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    68135 2023-05-30 06:59:39.658979 pyaedt-0.6.86/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6956 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    65138 2023-07-18 12:25:32.970625 pyaedt-0.6.86/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    32782 2023-07-11 14:47:17.463644 pyaedt-0.6.86/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    50049 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.86/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    65191 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    23687 2023-07-11 14:47:17.463644 pyaedt-0.6.86/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    34537 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   159025 2023-07-18 12:25:32.970625 pyaedt-0.6.86/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71535 2023-06-21 12:50:18.022631 pyaedt-0.6.86/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-05-30 06:59:39.658979 pyaedt-0.6.86/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51967 2023-05-30 06:59:39.658979 pyaedt-0.6.86/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40465 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82903 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28440 2023-07-11 14:47:17.463644 pyaedt-0.6.86/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53543 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11976 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    27635 2023-06-26 14:19:11.175189 pyaedt-0.6.86/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   181969 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64120 2023-06-29 09:15:20.756674 pyaedt-0.6.86/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   121445 2023-06-15 12:26:55.582508 pyaedt-0.6.86/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33257 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    30706 2023-06-26 13:01:22.142566 pyaedt-0.6.86/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103333 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   126124 2023-06-23 15:25:31.221272 pyaedt-0.6.86/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    95976 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/q3d.py
--rw-r--r--   0        0        0    10581 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7632 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10410 2023-06-05 09:36:43.953828 pyaedt-0.6.86/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4556 2023-07-21 14:33:51.388714 pyaedt-0.6.86/pyproject.toml
--rw-r--r--   0        0        0    15772 1970-01-01 00:00:00.000000 pyaedt-0.6.86/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-30 06:59:37.486926 pyaedt-0.6.87/LICENSE
+-rw-r--r--   0        0        0     9947 2023-05-30 06:59:37.486926 pyaedt-0.6.87/README.md
+-rw-r--r--   0        0        0     2629 2023-07-27 16:00:23.701424 pyaedt-0.6.87/pyaedt/__init__.py
+-rw-r--r--   0        0        0    26756 2023-07-25 17:51:34.650594 pyaedt-0.6.87/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-05-30 06:59:39.408947 pyaedt-0.6.87/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    88967 2023-07-25 17:51:34.650594 pyaedt-0.6.87/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    50696 2023-07-25 17:51:34.650594 pyaedt-0.6.87/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    17066 2023-06-20 15:35:24.349674 pyaedt-0.6.87/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-05-30 06:59:39.408947 pyaedt-0.6.87/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19948 2023-07-19 13:20:21.575376 pyaedt-0.6.87/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4431 2023-05-30 06:59:39.408947 pyaedt-0.6.87/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4596 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   136452 2023-07-25 17:51:34.650594 pyaedt-0.6.87/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    75793 2023-07-20 11:48:09.458225 pyaedt-0.6.87/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12464 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    36750 2023-06-29 09:15:20.741006 pyaedt-0.6.87/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    62949 2023-07-25 17:51:34.650594 pyaedt-0.6.87/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10259 2023-07-20 07:33:55.805436 pyaedt-0.6.87/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    84793 2023-07-25 17:51:34.650594 pyaedt-0.6.87/pyaedt/desktop.py
+-rw-r--r--   0        0        0    15104 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/dlls/PDFReport/AnsysReport.deps.json
+-rw-r--r--   0        0        0    23552 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1086 2023-06-28 08:36:59.983528 pyaedt-0.6.87/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0   204800 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
+-rw-r--r--   0        0        0   577445 2023-05-30 06:59:39.440208 pyaedt-0.6.87/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
+-rw-r--r--   0        0        0     9836 2023-05-30 06:59:39.440208 pyaedt-0.6.87/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   238592 2023-05-30 06:59:39.440208 pyaedt-0.6.87/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
+-rw-r--r--   0        0        0   115712 2023-05-30 06:59:39.440208 pyaedt-0.6.87/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
+-rw-r--r--   0        0        0   705296 2023-05-30 06:59:39.455836 pyaedt-0.6.87/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   712253 2023-05-30 06:59:39.455836 pyaedt-0.6.87/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0    80384 2023-05-30 06:59:39.455836 pyaedt-0.6.87/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
+-rw-r--r--   0        0        0   546816 2023-05-30 06:59:39.471459 pyaedt-0.6.87/pyaedt/dlls/PDFReport/PdfSharpCore.dll
+-rw-r--r--   0        0        0   367616 2023-05-30 06:59:39.471459 pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
+-rw-r--r--   0        0        0   536367 2023-05-30 06:59:39.471459 pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
+-rw-r--r--   0        0        0  1229824 2023-05-30 06:59:39.487088 pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
+-rw-r--r--   0        0        0  3285773 2023-05-30 06:59:39.502713 pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
+-rw-r--r--   0        0        0   120664 2023-05-30 06:59:39.502713 pyaedt-0.6.87/pyaedt/dlls/PDFReport/System.Runtime.dll
+-rw-r--r--   0        0        0  1505294 2023-05-30 06:59:39.518353 pyaedt-0.6.87/pyaedt/dlls/PDFReport/System.Runtime.xml
+-rw-r--r--   0        0        0     5632 2023-05-30 06:59:39.518353 pyaedt-0.6.87/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
+-rw-r--r--   0        0        0   160754 2023-05-30 06:59:39.533962 pyaedt-0.6.87/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
+-rw-r--r--   0        0        0    24188 2023-07-24 13:10:38.761320 pyaedt-0.6.87/pyaedt/downloads.py
+-rw-r--r--   0        0        0   138814 2023-07-27 13:09:33.142710 pyaedt-0.6.87/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-05-30 06:59:39.533962 pyaedt-0.6.87/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    98725 2023-07-25 16:50:25.973900 pyaedt-0.6.87/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:36:43.922575 pyaedt-0.6.87/pyaedt/edb_core/dotnet/__init__.py
+-rw-r--r--   0        0        0    31509 2023-07-20 07:33:55.805436 pyaedt-0.6.87/pyaedt/edb_core/dotnet/database.py
+-rw-r--r--   0        0        0     7909 2023-06-05 09:36:43.938202 pyaedt-0.6.87/pyaedt/edb_core/dotnet/layout.py
+-rw-r--r--   0        0        0    48515 2023-07-27 16:00:23.701424 pyaedt-0.6.87/pyaedt/edb_core/dotnet/primitive.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.533962 pyaedt-0.6.87/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    33195 2023-06-12 08:05:31.703949 pyaedt-0.6.87/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0    48709 2023-07-25 15:37:16.573778 pyaedt-0.6.87/pyaedt/edb_core/edb_data/control_file.py
+-rw-r--r--   0        0        0      937 2023-05-30 06:59:39.533962 pyaedt-0.6.87/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      867 2023-05-30 06:59:39.533962 pyaedt-0.6.87/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    12243 2023-06-05 09:36:43.938202 pyaedt-0.6.87/pyaedt/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    65661 2023-06-05 09:36:43.938202 pyaedt-0.6.87/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20820 2023-07-17 10:14:12.806355 pyaedt-0.6.87/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     6115 2023-07-24 13:10:38.761320 pyaedt-0.6.87/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    64588 2023-07-25 16:50:25.973900 pyaedt-0.6.87/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    32640 2023-07-27 16:00:23.701424 pyaedt-0.6.87/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0   102353 2023-07-27 07:25:08.069862 pyaedt-0.6.87/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36324 2023-06-05 09:36:43.938202 pyaedt-0.6.87/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    34944 2023-07-10 08:39:13.777984 pyaedt-0.6.87/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     3923 2023-06-05 14:54:59.781956 pyaedt-0.6.87/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2432 2023-06-05 09:36:43.938202 pyaedt-0.6.87/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     3258 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    68725 2023-06-29 11:46:59.997639 pyaedt-0.6.87/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2850 2023-06-05 09:36:43.953828 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7763 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4703 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11390 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-05-30 06:59:39.580847 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21800 2023-06-05 09:36:43.953828 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-05-30 06:59:39.580847 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    47176 2023-06-22 08:21:07.514633 pyaedt-0.6.87/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33310 2023-06-05 09:36:43.953828 pyaedt-0.6.87/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0    47963 2023-07-25 15:36:36.553810 pyaedt-0.6.87/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    50376 2023-07-25 16:50:25.973900 pyaedt-0.6.87/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    58809 2023-06-19 10:47:11.266974 pyaedt-0.6.87/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   111074 2023-07-17 10:14:12.806355 pyaedt-0.6.87/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    11500 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/emit.py
+-rw-r--r--   0        0        0     6100 2023-07-06 12:50:33.852654 pyaedt-0.6.87/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     2825 2023-07-20 07:33:55.805436 pyaedt-0.6.87/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0     1621 2023-06-13 17:56:07.965688 pyaedt-0.6.87/pyaedt/emit_core/emit_constants.py
+-rw-r--r--   0        0        0    11102 2023-07-24 13:10:38.761320 pyaedt-0.6.87/pyaedt/emit_core/interference_classification.py
+-rw-r--r--   0        0        0        2 2023-05-30 06:59:39.580847 pyaedt-0.6.87/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-07-06 12:50:33.852654 pyaedt-0.6.87/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    13896 2023-07-06 12:50:33.852654 pyaedt-0.6.87/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-05-30 06:59:39.580847 pyaedt-0.6.87/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    12252 2023-06-21 12:50:18.007016 pyaedt-0.6.87/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.580847 pyaedt-0.6.87/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3257 2023-05-30 06:59:39.580847 pyaedt-0.6.87/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83443 2023-07-20 11:48:09.458225 pyaedt-0.6.87/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    21891 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3442 2023-07-13 12:00:19.155166 pyaedt-0.6.87/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    71208 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0     9410 2023-07-20 12:33:36.682607 pyaedt-0.6.87/pyaedt/generic/grpc_plugin.py
+-rw-r--r--   0        0        0     3043 2023-07-11 14:47:17.448018 pyaedt-0.6.87/pyaedt/generic/grpc_plugin_dll.py
+-rw-r--r--   0        0        0    25808 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     7029 2023-07-13 12:00:19.155166 pyaedt-0.6.87/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0     9795 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    62327 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11405 2023-06-22 08:21:07.514633 pyaedt-0.6.87/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    20326 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3536 2023-06-21 12:50:18.007016 pyaedt-0.6.87/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60412 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17095 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   255524 2023-07-27 13:09:33.142710 pyaedt-0.6.87/pyaedt/hfss.py
+-rw-r--r--   0        0        0    84753 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   202984 2023-07-26 12:52:26.502860 pyaedt-0.6.87/pyaedt/icepak.py
+-rw-r--r--   0        0        0   127831 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7803 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24372 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3972 2023-07-07 09:12:05.234128 pyaedt-0.6.87/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     3311 2023-07-07 09:12:05.234128 pyaedt-0.6.87/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10210 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     2620 2023-07-05 06:36:09.681010 pyaedt-0.6.87/pyaedt/misc/ansys_cloud.areg
+-rw-r--r--   0        0        0     3731 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     5611 2023-07-07 06:30:25.350901 pyaedt-0.6.87/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14107 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    20051 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16840 2023-05-30 06:59:39.643351 pyaedt-0.6.87/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120896 2023-07-13 12:00:19.170793 pyaedt-0.6.87/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   207873 2023-07-26 13:34:42.288190 pyaedt-0.6.87/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   116735 2023-07-13 12:00:19.170793 pyaedt-0.6.87/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11407 2023-07-13 12:00:19.170793 pyaedt-0.6.87/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   129702 2023-07-13 12:00:19.170793 pyaedt-0.6.87/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.643351 pyaedt-0.6.87/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    39728 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49188 2023-07-26 12:52:26.518490 pyaedt-0.6.87/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59316 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53078 2023-07-11 14:47:17.463644 pyaedt-0.6.87/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12661 2023-07-19 13:20:21.575376 pyaedt-0.6.87/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    43135 2023-07-14 12:01:50.451661 pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    33551 2023-07-06 12:50:33.852654 pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8236 2023-07-13 12:00:19.186418 pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    64284 2023-07-27 13:36:54.705176 pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15185 2023-07-13 12:00:19.186418 pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.87/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    31781 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68135 2023-05-30 06:59:39.658979 pyaedt-0.6.87/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6956 2023-07-13 12:00:19.186418 pyaedt-0.6.87/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    65138 2023-07-18 12:25:32.970625 pyaedt-0.6.87/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    33041 2023-07-26 07:08:37.800116 pyaedt-0.6.87/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    50049 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.87/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65907 2023-07-26 07:08:37.800116 pyaedt-0.6.87/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    23473 2023-07-26 07:08:37.800116 pyaedt-0.6.87/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    34537 2023-07-13 12:00:19.186418 pyaedt-0.6.87/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   159025 2023-07-18 12:25:32.970625 pyaedt-0.6.87/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71535 2023-06-21 12:50:18.022631 pyaedt-0.6.87/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-05-30 06:59:39.658979 pyaedt-0.6.87/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51967 2023-05-30 06:59:39.658979 pyaedt-0.6.87/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40465 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82903 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28440 2023-07-11 14:47:17.463644 pyaedt-0.6.87/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53543 2023-07-13 12:00:19.186418 pyaedt-0.6.87/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11976 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    27635 2023-06-26 14:19:11.175189 pyaedt-0.6.87/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   181969 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64120 2023-06-29 09:15:20.756674 pyaedt-0.6.87/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   121445 2023-06-15 12:26:55.582508 pyaedt-0.6.87/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33257 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    30706 2023-06-26 13:01:22.142566 pyaedt-0.6.87/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103333 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   126124 2023-06-23 15:25:31.221272 pyaedt-0.6.87/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95976 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10581 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7632 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10410 2023-06-05 09:36:43.953828 pyaedt-0.6.87/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4650 2023-07-26 06:46:58.468961 pyaedt-0.6.87/pyproject.toml
+-rw-r--r--   0        0        0    15890 1970-01-01 00:00:00.000000 pyaedt-0.6.87/PKG-INFO
```

### Comparing `pyaedt-0.6.86/LICENSE` & `pyaedt-0.6.87/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/README.md` & `pyaedt-0.6.87/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/__init__.py` & `pyaedt-0.6.87/pyaedt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.86"
+__version__ = "0.6.87"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
```

### Comparing `pyaedt-0.6.86/pyaedt/aedt_logger.py` & `pyaedt-0.6.87/pyaedt/aedt_logger.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.87/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/application/Analysis.py` & `pyaedt-0.6.87/pyaedt/application/Analysis.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.87/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.87/pyaedt/application/Analysis3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.87/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.87/pyaedt/application/AnalysisNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.87/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.87/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/application/Design.py` & `pyaedt-0.6.87/pyaedt/application/Design.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/application/JobManager.py` & `pyaedt-0.6.87/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/application/Variables.py` & `pyaedt-0.6.87/pyaedt/application/Variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.87/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/application/design_solutions.py` & `pyaedt-0.6.87/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/circuit.py` & `pyaedt-0.6.87/pyaedt/circuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/common_rpc.py` & `pyaedt-0.6.87/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/desktop.py` & `pyaedt-0.6.87/pyaedt/desktop.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/AnsysReport.deps.json` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/AnsysReport.deps.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/Images/Ansys.png` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/Images/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/PdfSharpCore.dll` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/PdfSharpCore.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/System.Runtime.dll` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/System.Runtime.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/System.Runtime.xml` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/System.Runtime.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml` & `pyaedt-0.6.87/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/downloads.py` & `pyaedt-0.6.87/pyaedt/downloads.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb.py` & `pyaedt-0.6.87/pyaedt/edb.py`

 * *Files 2% similar despite different names*

```diff
@@ -2868,15 +2868,28 @@
             if simulation_setup.signal_layer_etching_instances:
                 for layer in simulation_setup.signal_layer_etching_instances:
                     if layer in self.stackup.layers:
                         idx = simulation_setup.signal_layer_etching_instances.index(layer)
                         if len(simulation_setup.etching_factor_instances) > idx:
                             self.stackup[layer].etch_factor = float(simulation_setup.etching_factor_instances[idx])
 
+            if not simulation_setup.signal_nets and simulation_setup.components:
+                nets_to_include = []
+                pnets = list(self.nets.power_nets.keys())[:]
+                for el in simulation_setup.components:
+                    nets_to_include.append([i for i in self.components[el].nets if i not in pnets])
+                simulation_setup.signal_nets = [
+                    i
+                    for i in list(set.intersection(*map(set, nets_to_include)))
+                    if i not in simulation_setup.power_nets and i != ""
+                ]
             self.nets.classify_nets(simulation_setup.power_nets, simulation_setup.signal_nets)
+            if not simulation_setup.power_nets or not simulation_setup.signal_nets:
+                self.logger.info("Disabling cutout as no signals or power nets have been defined.")
+                simulation_setup.do_cutout_subdesign = False
             if simulation_setup.do_cutout_subdesign:
                 self.logger.info("Cutting out using method: {0}".format(simulation_setup.cutout_subdesign_type))
                 if simulation_setup.use_default_cutout:
                     old_cell_name = self.active_cell.GetName()
                     if self.cutout(
                         signal_list=simulation_setup.signal_nets,
                         reference_list=simulation_setup.power_nets,
@@ -2916,27 +2929,34 @@
                     self.nets.delete(nets_to_remove)
             self.logger.info("Deleting existing ports.")
             map(lambda port: port.Delete(), self.layout.terminals)
             map(lambda pg: pg.Delete(), self.layout.pin_groups)
             if simulation_setup.solver_type == SolverType.Hfss3dLayout:
                 if simulation_setup.generate_excitations:
                     self.logger.info("Creating HFSS ports for signal nets.")
+                    source_type = SourceType.CoaxPort
+                    if not simulation_setup.generate_solder_balls:
+                        source_type = SourceType.CircPort
                     for cmp in simulation_setup.components:
                         self.components.create_port_on_component(
                             cmp,
                             net_list=simulation_setup.signal_nets,
                             do_pingroup=False,
                             reference_net=simulation_setup.power_nets,
-                            port_type=SourceType.CoaxPort,
+                            port_type=source_type,
                         )
-                    if not self.hfss.set_coax_port_attributes(simulation_setup):  # pragma: no cover
+                    if simulation_setup.generate_solder_balls and not self.hfss.set_coax_port_attributes(
+                        simulation_setup
+                    ):  # pragma: no cover
                         self.logger.error("Failed to configure coaxial port attributes.")
                     self.logger.info("Number of ports: {}".format(self.hfss.get_ports_number()))
                     self.logger.info("Configure HFSS extents.")
-                    if simulation_setup.trim_reference_size:  # pragma: no cover
+                    if (
+                        simulation_setup.generate_solder_balls and simulation_setup.trim_reference_size
+                    ):  # pragma: no cover
                         self.logger.info(
                             "Trimming the reference plane for coaxial ports: {0}".format(
                                 bool(simulation_setup.trim_reference_size)
                             )
                         )
                         self.hfss.trim_component_reference_size(simulation_setup)  # pragma: no cover
                 self.hfss.configure_hfss_extents(simulation_setup)
```

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/components.py` & `pyaedt-0.6.87/pyaedt/edb_core/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -870,19 +870,19 @@
             )
             return False
         pin_layers = cmp_pins[0].GetPadstackDef().GetData().GetLayerNames()
         if port_type == SourceType.CoaxPort:
             pad_params = self._padstack.get_pad_parameters(pin=cmp_pins[0], layername=pin_layers[0], pad_type=0)
             if not pad_params[0] == 7:
                 sball_diam = min([self._pedb.edb_value(val).ToDouble() for val in pad_params[1]])
-                solder_ball_height = sball_diam / 2
+                solder_ball_height = 2 * sball_diam / 3
             else:
                 bbox = pad_params[1]
                 sball_diam = min([abs(bbox[2] - bbox[0]), abs(bbox[3] - bbox[1])]) * 0.8
-                solder_ball_height = sball_diam / 2
+                solder_ball_height = 2 * sball_diam / 3
             self.set_solder_ball(component, solder_ball_height, sball_diam)
             for pin in cmp_pins:
                 self._padstack.create_coax_port(padstackinstance=pin, name=port_name)
 
         elif port_type == SourceType.CircPort:  # pragma no cover
             ref_pins = [
                 p
@@ -892,17 +892,15 @@
             for p in ref_pins:
                 if not p.IsLayoutPin():
                     p.SetIsLayoutPin(True)
             if len(ref_pins) == 0:
                 self._logger.info("No reference pin found on component {}.".format(component.GetName()))
             if do_pingroup:
                 if len(ref_pins) == 1:
-                    self.create_terminal = self._create_terminal(ref_pins[0])
-                    self.terminal = self.create_terminal
-                    ref_pin_group_term = self.terminal
+                    ref_pin_group_term = self._create_terminal(ref_pins[0])
                 else:
                     ref_pin_group = self.create_pingroup_from_pins(ref_pins)
                     if not ref_pin_group:
                         return False
                     ref_pin_group_term = self._create_pin_group_terminal(ref_pin_group, isref=True)
                     if not ref_pin_group_term:
                         return False
@@ -1226,15 +1224,18 @@
 
         isref : bool
 
         Returns
         -------
         Edb pin group terminal.
         """
-        term_name = "{}_T".format(pingroup.GetName())
+        pin = list(pingroup.GetPins())[0]
+        term_name = "{}.{}.{}".format(
+            pin.GetComponent().GetName(), pin.GetComponent().GetName(), pin.GetNet().GetName()
+        )
         for t in list(self._pedb.active_layout.Terminals):
             if t.GetName() == term_name:
                 return t
         pingroup_term = self._edb.cell.terminal.PinGroupTerminal.Create(
             self._active_layout, pingroup.GetNet(), term_name, pingroup, isref
         )
         return pingroup_term
@@ -1818,22 +1819,21 @@
             edb_cmp = self.get_component_by_name(component)
             cmp = self.instances[component]
         else:
             edb_cmp = component
             cmp = self.instances[edb_cmp.GetName()]
         if edb_cmp:
             cmp_type = edb_cmp.GetComponentType()
-            if bool(not sball_diam + sball_height):
+            if not sball_diam:
                 pin1 = list(cmp.pins.values())[0].pin
                 pin_layers = pin1.GetPadstackDef().GetData().GetLayerNames()
                 pad_params = self._padstack.get_pad_parameters(pin=pin1, layername=pin_layers[0], pad_type=0)
                 _sb_diam = min([self._get_edb_value(val).ToDouble() for val in pad_params[1]])
                 sball_diam = _sb_diam
-                sball_height = sball_diam
-
+            sball_height = round(self._edb.utility.Value(sball_diam).ToDouble(), 9) / 2
             if not sball_mid_diam:
                 sball_mid_diam = sball_diam
 
             if shape == "Cylinder":
                 sball_shape = self._edb.definition.SolderballShape.Cylinder
             else:
                 sball_shape = self._edb.definition.SolderballShape.Spheroid
```

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/dotnet/database.py` & `pyaedt-0.6.87/pyaedt/edb_core/dotnet/database.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/dotnet/layout.py` & `pyaedt-0.6.87/pyaedt/edb_core/dotnet/layout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/dotnet/primitive.py` & `pyaedt-0.6.87/pyaedt/edb_core/dotnet/primitive.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,24 @@
     def padstack_instance(self):
         return PadstackInstanceDotNet(self._app)
 
     @property
     def net(self):
         return self.prim_obj.GetNet()
 
+    @net.setter
+    def net(self, value):
+        try:
+            if "net" in dir(value):
+                self.prim_obj.SetNet(value.net_obj)
+            else:
+                self.prim_obj.SetNet(value)
+        except TypeError:
+            self._app.logger.error("Error setting net object")
+
     @property
     def polygon_data(self):
         """:class:`PolygonData <ansys.edb.geometry.PolygonData>`: Outer contour of the Polygon object."""
         return self.prim_obj.GetPolygonData()
 
     @polygon_data.setter
     def polygon_data(self, poly):
```

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/components_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/control_file.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/control_file.py`

 * *Files 18% similar despite different names*

```diff
@@ -99,44 +99,65 @@
     return False
 
 
 class ControlProperty:
     def __init__(self, property_name, value):
         self.name = property_name
         self.value = value
-        try:
-            float(value)
-            self.type = 0
-        except TypeError:
-            if isinstance(value, list):
-                self.type = 2
-            elif isinstance(value, str):
-                self.type = 1
+        if isinstance(value, str):
+            self.type = 1
+        elif isinstance(value, list):
+            self.type = 2
+        else:
+            try:
+                float(value)
+                self.type = 0
+            except TypeError:
+                pass
 
     def _write_xml(self, root):
-        if self.type == 0:
-            content = ET.SubElement(root, self.name)
-            double = ET.SubElement(content, "Double")
-            double.text = str(self.value)
+        try:
+            if self.type == 0:
+                content = ET.SubElement(root, self.name)
+                double = ET.SubElement(content, "Double")
+                double.text = str(self.value)
+            else:
+                pass
+        except:
+            pass
 
 
 class ControlFileMaterial:
     def __init__(self, name, properties):
         self.name = name
         self.properties = {}
         for name, property in properties.items():
             self.properties[name] = ControlProperty(name, property)
 
     def _write_xml(self, root):
         content = ET.SubElement(root, "Material")
         content.set("Name", self.name)
-        for name, property in self.properties.items():
+        for property_name, property in self.properties.items():
             property._write_xml(content)
 
 
+class ControlFileDielectric:
+    def __init__(self, name, properties):
+        self.name = name
+        self.properties = {}
+        for name, prop in properties.items():
+            self.properties[name] = prop
+
+    def _write_xml(self, root):
+        content = ET.SubElement(root, "Layer")
+        for property_name, property in self.properties.items():
+            if not property_name == "Index":
+                content.set(property_name, str(property))
+
+
 class ControlFileLayer:
     def __init__(self, name, properties):
         self.name = name
         self.properties = {}
         for name, prop in properties.items():
             self.properties[name] = prop
 
@@ -260,93 +281,265 @@
         Returns
         -------
         list of :class:`pyaedt.edb_core.edb_data.control_file.ControlFileLayer`
 
         """
         return self._layers
 
-    def add_material(self, material_name, properties):
+    def add_material(
+        self,
+        material_name,
+        permittivity=1.0,
+        dielectric_loss_tg=0.0,
+        permeability=1.0,
+        conductivity=0.0,
+        properties=None,
+    ):
         """Add a new material with specific properties.
 
         Parameters
         ----------
         material_name : str
             Material name.
-        properties : dict
+        permittivity : float, optional
+            Material permittivity. The default is ``1.0``.
+        dielectric_loss_tg : float, optional
+            Material tangent losses. The default is ``0.0``.
+        permeability : float, optional
+            Material permeability. The default is ``1.0``.
+        conductivity : float, optional
+            Material conductivity. The default is ``0.0``.
+        properties : dict, optional
+            Specific material properties. The default is ``None``.
             Dictionary with key and material property value.
 
         Returns
         -------
         :class:`pyaedt.edb_core.edb_data.control_file.ControlFileMaterial`
         """
-        self._materials[material_name] = ControlFileMaterial(material_name, properties)
-        return self._materials[material_name]
+        if isinstance(properties, dict):
+            self._materials[material_name] = ControlFileMaterial(material_name, properties)
+            return self._materials[material_name]
+        else:
+            properties = {
+                "Name": material_name,
+                "Permittivity": permittivity,
+                "Permeability": permeability,
+                "Conductivity": conductivity,
+                "DielectricLossTangent": dielectric_loss_tg,
+            }
+            self._materials[material_name] = ControlFileMaterial(material_name, properties)
+            return self._materials[material_name]
 
-    def add_layer(self, layer_name, properties):
+    def add_layer(
+        self,
+        layer_name,
+        elevation=0.0,
+        material="",
+        gds_type=0,
+        target_layer="",
+        thickness=0.0,
+        layer_type="conductor",
+        solve_inside=True,
+        properties=None,
+    ):
         """Add a new layer.
 
         Parameters
         ----------
         layer_name : str
             Layer name.
+        elevation : float
+            Layer elevation.
+        material : str
+            Material for the layer.
+        gds_type : int
+            GDS type assigned on the layer. The value must be the same as in the GDS file otherwise geometries won't be
+            imported.
+        target_layer : str
+            Layer name assigned in EDB or HFSS 3D layout after import.
+        thickness : float
+            Layer thickness
+        layer_type : str
+            Define the layer type, default value for a layer is ``"conductor"``
+        solve_inside : bool
+            When ``True`` solver will solve inside metal, and not id ``False``. Default value is ``True``.
         properties : dict
             Dictionary with key and  property value.
 
         Returns
         -------
         :class:`pyaedt.edb_core.edb_data.control_file.ControlFileLayer`
         """
-        self._layers.append(ControlFileLayer(layer_name, properties))
+        if isinstance(properties, dict):
+            self._layers.append(ControlFileLayer(layer_name, properties))
+            return self._layers[-1]
+        else:
+            properties = {
+                "Name": layer_name,
+                "GDSDataType": str(gds_type),
+                "TargetLayer": target_layer,
+                "Type": layer_type,
+                "Material": material,
+                "Thickness": str(thickness),
+                "Elevation": str(elevation),
+                "SolveInside": str(solve_inside).lower(),
+            }
+            self._layers.append(ControlFileDielectric(layer_name, properties))
+            return self._layers[-1]
 
-    def add_dielectric(self, layer_name, properties):
+    def add_dielectric(
+        self,
+        layer_name,
+        layer_index=None,
+        material="",
+        thickness=0.0,
+        properties=None,
+        base_layer=None,
+        add_on_top=True,
+    ):
         """Add a new dielectric.
 
         Parameters
         ----------
         layer_name : str
             Layer name.
+        layer_index : int, optional
+            Dielectric layer index as they must be stacked. If not provided the layer index will be incremented.
+        material : str
+            Material name.
+        thickness : float
+            Layer thickness.
         properties : dict
             Dictionary with key and  property value.
+        base_layer : str,  optional
+            Layer name used for layer placement. Default value is ``None``. This option is used for inserting
+            dielectric layer between two existing ones. When no argument is provided the dielectric layer will be placed
+            on top of the stacked ones.
+        method : bool, Optional.
+            Provides the method to use when the argument ``base_layer`` is provided. When ``True`` the layer is added
+            on top on the base layer, when ``False`` it will be added below.
 
         Returns
         -------
-        :class:`pyaedt.edb_core.edb_data.control_file.ControlFileLayer`
+        :class:`pyaedt.edb_core.edb_data.control_file.ControlFileDielectric`
         """
-        self._dielectrics.append(ControlFileLayer(layer_name, properties))
+        if isinstance(properties, dict):
+            self._dielectrics.append(ControlFileDielectric(layer_name, properties))
+            return self._dielectrics[-1]
+        else:
+            if not layer_index and self.dielectrics and not base_layer:
+                layer_index = max([diel.properties["Index"] for diel in self.dielectrics]) + 1
+            elif base_layer and self.dielectrics:
+                if base_layer in [diel.properties["Name"] for diel in self.dielectrics]:
+                    base_layer_index = next(
+                        diel.properties["Index"] for diel in self.dielectrics if diel.properties["Name"] == base_layer
+                    )
+                    if add_on_top:
+                        layer_index = base_layer_index + 1
+                        for diel_layer in self.dielectrics:
+                            if diel_layer.properties["Index"] > base_layer_index:
+                                diel_layer.properties["Index"] += 1
+                    else:
+                        layer_index = base_layer_index
+                        for diel_layer in self.dielectrics:
+                            if diel_layer.properties["Index"] >= base_layer_index:
+                                diel_layer.properties["Index"] += 1
+            elif not layer_index:
+                layer_index = 0
+            properties = {"Index": layer_index, "Material": material, "Name": layer_name, "Thickness": thickness}
+            self._dielectrics.append(ControlFileDielectric(layer_name, properties))
+            return self._dielectrics[-1]
 
-    def add_via(self, layer_name, properties):
+    def add_via(
+        self,
+        layer_name,
+        material="",
+        gds_type=0,
+        target_layer="",
+        start_layer="",
+        stop_layer="",
+        solve_inside=True,
+        via_group_method="proximity",
+        via_group_tol=1e-6,
+        via_group_persistent=True,
+        snap_via_group_method="distance",
+        snap_via_group_tol=10e-9,
+        properties=None,
+    ):
         """Add a new via layer.
 
         Parameters
         ----------
         layer_name : str
             Layer name.
+        material : str
+            Define the material for this layer.
+        gds_type : int
+            Define the gds type.
+        target_layer : str
+            Target layer used after layout import in EDB and HFSS 3D layout.
+        start_layer : str
+            Define the start layer for the via
+        stop_layer : str
+            Define the stop layer for the via.
+        solve_inside : bool
+            When ``True`` solve inside this layer is anbled. Default value is ``True``.
+        via_group_method : str
+            Define the via group method, default value is ``"proximity"``
+        via_group_tol : float
+            Define the via group tolerance.
+        via_group_persistent : bool
+            When ``True`` activated otherwise when ``False``is deactivated. Default value is ``True``.
+        snap_via_group_method : str
+            Define the via group method, default value is ``"distance"``
+        snap_via_group_tol : float
+            Define the via group tolerance, default value is 10e-9.
         properties : dict
             Dictionary with key and  property value.
 
         Returns
         -------
         :class:`pyaedt.edb_core.edb_data.control_file.ControlFileVia`
         """
-        self._vias.append(ControlFileVia(layer_name, properties))
-        return self._vias[-1]
+        if isinstance(properties, dict):
+            self._vias.append(ControlFileVia(layer_name, properties))
+            return self._vias[-1]
+        else:
+            properties = {
+                "Name": layer_name,
+                "GDSDataType": str(gds_type),
+                "TargetLayer": target_layer,
+                "Material": material,
+                "StartLayer": start_layer,
+                "StopLayer": stop_layer,
+                "SolveInside": str(solve_inside).lower(),
+                "ViaGroupMethod": via_group_method,
+                "Persistent": via_group_persistent,
+                "ViaGroupTolerance": via_group_tol,
+                "SnapViaGroupMethod": snap_via_group_method,
+                "SnapViaGroupTolerance": snap_via_group_tol,
+            }
+            self._vias.append(ControlFileVia(layer_name, properties))
+            return self._vias[-1]
 
     def _write_xml(self, root):
         content = ET.SubElement(root, "Stackup")
         content.set("schemaVersion", "1.0")
         materials = ET.SubElement(content, "Materials")
         for materialname, material in self.materials.items():
             material._write_xml(materials)
-
         elayers = ET.SubElement(content, "ELayers")
         elayers.set("LengthUnit", self.units)
         if self.metal_layer_snapping_tolerance:
             elayers.set("MetalLayerSnappingTolerance", str(self.metal_layer_snapping_tolerance))
         dielectrics = ET.SubElement(elayers, "Dielectrics")
         dielectrics.set("BaseElevation", str(self.dielectrics_base_elevation))
+        # sorting dielectric layers
+        self._dielectrics = list(sorted(list(self._dielectrics), key=lambda x: x.properties["Index"], reverse=False))
         for layer in self.dielectrics:
             layer._write_xml(dielectrics)
         layers = ET.SubElement(elayers, "Layers")
 
         for layer in self.layers:
             layer._write_xml(layers)
         vias = ET.SubElement(elayers, "Vias")
@@ -396,15 +589,15 @@
             content.set("MinBondwireWidth", str(self.min_bondwire_width))
         if self.gdsii_scaling_factor != 0.0:
             content.set("GDSIIScalingFactor", str(self.gdsii_scaling_factor))
         content.set("DeleteEmptyNonLaminateSignalLayers", str(self.delte_empty_non_laminate_signal_layers).lower())
 
 
 class ControlExtent:
-    "Extent options."
+    """Extent options."""
 
     def __init__(
         self,
         type="bbox",
         dieltype="bbox",
         diel_hactor=0.25,
         airbox_hfactor=0.25,
@@ -995,25 +1188,31 @@
                                 if prop[0].tag == "Double":
                                     properties[prop.tag] = prop[0].text
                             self.stackup.add_material(mat_name, properties)
                     elif st_el.tag == "ELayers":
                         if st_el.attrib == "LengthUnits":
                             self.stackup.units = st_el.attrib
                         for layers_el in st_el:
+                            if "BaseElevation" in layers_el.attrib:
+                                self.stackup.dielectrics_base_elevation = layers_el.attrib["BaseElevation"]
                             for layer_el in layers_el:
                                 properties = {}
                                 layer_name = layer_el.attrib["Name"]
                                 for propname, prop_val in layer_el.attrib.items():
                                     properties[propname] = prop_val
                                 if layers_el.tag == "Dielectrics":
-                                    self.stackup.add_dielectric(layer_name, properties)
+                                    self.stackup.add_dielectric(
+                                        layer_name=layer_name,
+                                        material=properties["Material"],
+                                        thickness=properties["Thickness"],
+                                    )
                                 elif layers_el.tag == "Layers":
-                                    self.stackup.add_layer(layer_name, properties)
+                                    self.stackup.add_layer(layer_name=layer_name, properties=properties)
                                 elif layers_el.tag == "Vias":
-                                    via = self.stackup.add_via(layer_name, properties)
+                                    via = self.stackup.add_via(layer_name, properties=properties)
                                     for i in layer_el:
                                         if i.tag == "CreateViaGroups":
                                             via.create_via_group = True
                                             if "CheckContainment" in i.attrib:
                                                 via.check_containment = (
                                                     True if i.attrib["CheckContainment"] == "true" else False
                                                 )
@@ -1032,15 +1231,15 @@
                                                 via.remove_unconnected = (
                                                     True if i.attrib["RemoveUnconnected"] == "true" else False
                                                 )
         return True
 
     @pyaedt_function_handler()
     def write_xml(self, xml_output):
-        """Write xml to output file.
+        """Write xml to output file
 
         Parameters
         ----------
         xml_output : str
             Path to the output xml file.
         Returns
         -------
```

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/hfss_extent_info.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/hfss_extent_info.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/nets_data.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/nets_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -142,49 +142,32 @@
         exception_list : list, optional
             List of components which bypass threshold check.
         Returns
         -------
         list[
             dict[str, :class: `pyaedt.edb_core.edb_data.nets_data.EDBNetsData`],
             dict[str, :class: `pyaedt.edb_core.edb_data.components_data.EDBComponent`],
-            dict[str, :class: `pyaedt.edb_core.edb_data.components_data.EDBComponent`],
             ]
         Examples
         --------
         >>> from pyaedt import Edb
         >>> app = Edb()
         >>> app.nets["BST_V3P3_S5"].get_extended_net()
         """
-        if exception_list is None:
-            exception_list = []
-        all_nets = self._app.nets.nets
-        nets = {self.name: all_nets[self.name]}
-        rlc_serial = {}
-        comps = {}
-
-        def get_net_list(net_name, _net_list, _rlc_serial, _comp, exception_list):
-            edb_net = all_nets[net_name]
-            for refdes, val in edb_net.components.items():
-                if not val.is_enabled:
-                    continue
-
-                if refdes in exception_list:
-                    pass
-                elif val.type == "Inductor" and val.rlc_values[1] < inductor_below and val.is_enabled:
-                    pass
-                elif val.type == "Resistor" and val.rlc_values[0] < resistor_below and val.is_enabled:
-                    pass
-                elif val.type == "Capacitor" and val.rlc_values[2] > capacitor_above and val.is_enabled:
-                    pass
-                else:
-                    _comp[refdes] = val
-                    continue
-
-                _rlc_serial[refdes] = val
-                for net in val.nets:
-                    if net not in _net_list:
-                        _net_list[net] = all_nets[net]
-                        get_net_list(net, _net_list, _rlc_serial, _comp, exception_list)
+        exts = self._app.nets.get_extended_nets(resistor_below, inductor_below, capacitor_above, exception_list)
+        for i in exts:
+            if self.name in i:
+                extended = i
+        output_nets = [{i: self._app.nets[i]} for i in extended]
+        comps_common = {}
+        for net in extended:
+            comps_common.update(
+                {
+                    i: v
+                    for i, v in self._app._nets[net].components.items()
+                    if list(set(v.nets).intersection(extended)) != [net]
+                }
+            )
 
-        get_net_list(self.name, nets, rlc_serial, comps, exception_list)
+        rlc_common = {i: v for i, v in comps_common.items() if v.type in ["Resistor", "Inductor", "Capacitor"]}
 
-        return [nets, rlc_serial, comps]
+        return output_nets, rlc_common
```

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -679,14 +679,53 @@
         -------
         dict
         """
         return {
             id: via for id, via in self._ppadstack.padstack_instances.items() if via.padstack_definition == self.name
         }
 
+    @property
+    def hole_range(self):
+        """Get hole range value from padstack definition.
+
+        Returns
+        -------
+        str
+            Possible returned values are ``"through"``, ``"begin_on_upper_pad"``,
+            ``"end_on_lower_pad"``, ``"upper_pad_to_lower_pad"``, and ``"undefined"``.
+        """
+        cloned_padstackdef_data = self._edb.definition.PadstackDefData(self.edb_padstack.GetData())
+        hole_ange_type = int(cloned_padstackdef_data.GetHoleRange())
+        if hole_ange_type == 0:  # pragma no cover
+            return "through"
+        elif hole_ange_type == 1:  # pragma no cover
+            return "begin_on_upper_pad"
+        elif hole_ange_type == 2:  # pragma no cover
+            return "end_on_lower_pad"
+        elif hole_ange_type == 3:  # pragma no cover
+            return "upper_pad_to_lower_pad"
+        else:  # pragma no cover
+            return "undefined"
+
+    @hole_range.setter
+    def hole_range(self, value):
+        if isinstance(value, str):  # pragma no cover
+            cloned_padstackdef_data = self._edb.definition.PadstackDefData(self.edb_padstack.GetData())
+            if value == "through":  # pragma no cover
+                cloned_padstackdef_data.SetHoleRange(self._edb.definition.PadstackHoleRange.Through)
+            elif value == "begin_on_upper_pad":  # pragma no cover
+                cloned_padstackdef_data.SetHoleRange(self._edb.definition.PadstackHoleRange.BeginOnUpperPad)
+            elif value == "end_on_lower_pad":  # pragma no cover
+                cloned_padstackdef_data.SetHoleRange(self._edb.definition.PadstackHoleRange.EndOnLowerPad)
+            elif value == "upper_pad_to_lower_pad":  # pragma no cover
+                cloned_padstackdef_data.SetHoleRange(self._edb.definition.PadstackHoleRange.UpperPadToLowerPad)
+            else:  # pragma no cover
+                return
+            self.edb_padstack.SetData(cloned_padstackdef_data)
+
     @pyaedt_function_handler()
     def convert_to_3d_microvias(self, convert_only_signal_vias=True, hole_wall_angle=15):
         """Convert actual padstack instance to microvias 3D Objects with a given aspect ratio.
 
         Parameters
         ----------
         convert_only_signal_vias : bool, optional
@@ -1058,96 +1097,122 @@
     @property
     def backdrill_top(self):
         """Backdrill layer from top.
 
         Returns
         -------
         tuple
-            Tuple of the layer name and drill diameter.
+            Tuple of the layer name, drill diameter, and offset if it exists.
         """
         layer = self._pedb.edb_api.cell.layer("", self._pedb.edb_api.cell.layer_type.SignalLayer)
         val = self._pedb.edb_value(0)
+        offset = self._pedb.edb_value(0.0)
         if is_ironpython:  # pragma: no cover
             diameter = _clr.StrongBox[type(val)]()
             drill_to_layer = _clr.StrongBox[self._pedb.edb_api.Cell.ILayerReadOnly]()
-            flag = self._edb_padstackinstance.GetBackDrillParametersLayerValue(drill_to_layer, diameter, False)
+            flag = self._edb_padstackinstance.GetBackDrillParametersLayerValue(drill_to_layer, offset, diameter, False)
         else:
             (
                 flag,
                 drill_to_layer,
+                offset,
                 diameter,
-            ) = self._edb_padstackinstance.GetBackDrillParametersLayerValue(layer, val, False)
+            ) = self._edb_padstackinstance.GetBackDrillParametersLayerValue(layer, offset, val, False)
         if flag:
-            return drill_to_layer.GetName(), diameter.ToString()
+            if offset.ToDouble():
+                return drill_to_layer.GetName(), diameter.ToString(), offset.ToString()
+            else:
+                return drill_to_layer.GetName(), diameter.ToString()
         else:
             return
 
-    def set_backdrill_top(self, drill_depth, drill_diameter):
+    def set_backdrill_top(self, drill_depth, drill_diameter, offset=0.0):
         """Set backdrill from top.
 
         Parameters
         ----------
         drill_depth : str
             Name of the drill to layer.
         drill_diameter : float, str
             Diameter of backdrill size.
+        offset : float, str
+            Offset for the backdrill. The default is ``0.0``. If the value is other than the
+            default, the stub does not stop at the layer. In AEDT, this parameter is called
+            "Mfg stub length".
 
         Returns
         -------
         bool
             True if success, False otherwise.
         """
         layer = self._pedb.stackup.layers[drill_depth]._edb_layer
         val = self._pedb.edb_value(drill_diameter)
-        return self._edb_padstackinstance.SetBackDrillParameters(layer, val, False)
+        offset = self._pedb.edb_value(offset)
+        if offset.ToDouble():
+            return self._edb_padstackinstance.SetBackDrillParameters(layer, offset, val, False)
+        else:
+            return self._edb_padstackinstance.SetBackDrillParameters(layer, val, False)
 
     @property
     def backdrill_bottom(self):
         """Backdrill layer from bottom.
 
         Returns
         -------
         tuple
-            Tuple of the layer name and drill diameter.
+            Tuple of the layer name, drill diameter, and drill offset if it exists.
         """
         layer = self._pedb.edb_api.cell.layer("", self._pedb.edb_api.cell.layer_type.SignalLayer)
         val = self._pedb.edb_value(0)
+        offset = self._pedb.edb_value(0.0)
         if is_ironpython:  # pragma: no cover
             diameter = _clr.StrongBox[type(val)]()
             drill_to_layer = _clr.StrongBox[self._pedb.edb_api.Cell.ILayerReadOnly]()
-            flag = self._edb_padstackinstance.GetBackDrillParametersLayerValue(drill_to_layer, diameter, True)
+            flag = self._edb_padstackinstance.GetBackDrillParametersLayerValue(drill_to_layer, offset, diameter, True)
         else:
             (
                 flag,
                 drill_to_layer,
+                offset,
                 diameter,
-            ) = self._edb_padstackinstance.GetBackDrillParametersLayerValue(layer, val, True)
+            ) = self._edb_padstackinstance.GetBackDrillParametersLayerValue(layer, offset, val, True)
         if flag:
-            return drill_to_layer.GetName(), diameter.ToString()
+            if offset.ToDouble():
+                return drill_to_layer.GetName(), diameter.ToString(), offset.ToString()
+            else:
+                return drill_to_layer.GetName(), diameter.ToString()
         else:
             return
 
-    def set_backdrill_bottom(self, drill_depth, drill_diameter):
+    def set_backdrill_bottom(self, drill_depth, drill_diameter, offset=0.0):
         """Set backdrill from bottom.
 
         Parameters
         ----------
         drill_depth : str
             Name of the drill to layer.
         drill_diameter : float, str
-            Diameter of backdrill size.
+            Diameter of the backdrill size.
+        offset : float, str, optional
+            Offset for the backdrill. The default is ``0.0``. If the value is other than the
+            default, the stub does not stop at the layer. In AEDT, this parameter is called
+            "Mfg stub length".
 
         Returns
         -------
         bool
             True if success, False otherwise.
         """
         layer = self._pedb.stackup.layers[drill_depth]._edb_layer
         val = self._pedb.edb_value(drill_diameter)
-        return self._edb_padstackinstance.SetBackDrillParameters(layer, val, True)
+        offset = self._pedb.edb_value(offset)
+        if offset.ToDouble():
+            return self._edb_padstackinstance.SetBackDrillParameters(layer, offset, val, True)
+        else:
+            return self._edb_padstackinstance.SetBackDrillParameters(layer, val, True)
 
     @property
     def start_layer(self):
         """Starting layer.
 
         Returns
         -------
```

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,18 +106,19 @@
         str
         """
         return self.net.GetName()
 
     @net_name.setter
     def net_name(self, name):
         if isinstance(name, str):
-            self.net.SetName(name)
+            net = self._app.nets.nets[name].net_object
+            self.primitive_object.SetNet(net)
         else:
             try:
-                self.net.SetName(name.GetName())
+                self.net = name
             except:
                 self._app.logger.error("Failed to set net name.")
 
     @pyaedt_function_handler()
     def delete(self):
         """Delete this primitive."""
         return self.primitive_object.Delete()
```

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def __init__(self):
         self._signal_nets = []
         self._power_nets = []
         self._components = []
         self._cutout_subdesign_type = CutoutSubdesignType.Conformal  # Conformal
         self._cutout_subdesign_expansion = 0.001
         self._cutout_subdesign_round_corner = True
-        self._use_default_cutout = True
+        self._use_default_cutout = False
         self._generate_excitations = True
         self._add_frequency_sweep = True
         self._include_only_selected_nets = False
         self._generate_solder_balls = True
         self._coax_solder_ball_diameter = []
         self._use_default_coax_port_radial_extension = True
         self._trim_reference_size = False
@@ -257,15 +257,16 @@
 
     @use_pyaedt_cutout.setter
     def use_pyaedt_cutout(self, value):
         self._use_default_cutout = not value
 
     @property
     def use_default_cutout(self):  # pragma: no cover
-        """Whether the default EDB cutout or a new PyAEDT cutout is used.
+        """Whether to use the default EDB cutout. The default is ``False``, in which case
+        a new PyAEDT cutout is used.
 
         Returns
         -------
         bool
         """
 
         return self._use_default_cutout
```

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/sources.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/edb_data/variables.py` & `pyaedt-0.6.87/pyaedt/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/general.py` & `pyaedt-0.6.87/pyaedt/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.87/pyaedt/edb_core/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/layout.py` & `pyaedt-0.6.87/pyaedt/edb_core/layout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/materials.py` & `pyaedt-0.6.87/pyaedt/edb_core/materials.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/nets.py` & `pyaedt-0.6.87/pyaedt/edb_core/nets.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,17 @@
         if name in self.nets:
             return self.nets[name]
         self._pedb.logger.error("Component or definition not found.")
         return
 
     def __init__(self, p_edb):
         self._pedb = p_edb
+        self._nets = {}
+        self._nets_by_comp_dict = {}
+        self._comps_by_nets_dict = {}
 
     @property
     def _edb(self):
         """ """
         return self._pedb.edb_api
 
     @property
@@ -84,18 +87,18 @@
         """Nets.
 
         Returns
         -------
         dict[str, :class:`pyaedt.edb_core.edb_data.nets_data.EDBNetsData`]
             Dictionary of nets.
         """
-        nets = {}
+
         for net in self._layout.nets:
-            nets[net.name] = EDBNetsData(net.api_object, self._pedb)
-        return nets
+            self._nets[net.name] = EDBNetsData(net.api_object, self._pedb)
+        return self._nets
 
     @property
     def netlist(self):
         """Return the cell netlist.
 
         Returns
         -------
@@ -195,14 +198,108 @@
                 pwr_gnd_nets.append(EDBNetsData(net.api_object, self._pedb))
                 continue
             if total_plane_area > 0.0 and total_trace_area > 0.0:
                 if total_plane_area / (total_plane_area + total_trace_area) > threshold:
                     pwr_gnd_nets.append(EDBNetsData(net.api_object, self._pedb))
         return pwr_gnd_nets
 
+    @property
+    def nets_by_components(self):
+        # type: () -> dict
+        """Get all nets for each component instance."""
+        for comp, i in self._pedb.components.instances.items():
+            self._nets_by_comp_dict[comp] = i.nets
+        return self._nets_by_comp_dict
+
+    @property
+    def components_by_nets(self):
+        # type: () -> dict
+        """Get all component instances grouped by nets."""
+        for comp, i in self._pedb.components.instances.items():
+            for n in i.nets:
+                if n in self._comps_by_nets_dict:
+                    self._comps_by_nets_dict[n].append(comp)
+                else:
+                    self._comps_by_nets_dict[n] = [comp]
+        return self._comps_by_nets_dict
+
+    @pyaedt_function_handler()
+    def get_extended_nets(self, resistor_below=10, inductor_below=1, capacitor_above=1, exception_list=None):
+        # type: (int | float, int | float, int |float, list) -> list
+        """Get extended net and associated components.
+
+        Parameters
+        ----------
+        resistor_below : int, float, optional
+            Threshold of resistor value. Search extended net across resistors which has value lower than the threshold.
+        inductor_below : int, float, optional
+            Threshold of inductor value. Search extended net across inductances which has value lower than the
+            threshold.
+        capacitor_above : int, float, optional
+            Threshold of capacitor value. Search extended net across capacitors which has value higher than the
+            threshold.
+        exception_list : list, optional
+            List of components which bypass threshold check. The default is ``None``.
+        Returns
+        -------
+        list
+            List of all extended nets.
+
+        Examples
+        --------
+        >>> from pyaedt import Edb
+        >>> app = Edb()
+        >>> app.nets.get_extended_nets()
+        """
+        if exception_list is None:
+            exception_list = []
+        self._extendend_nets = []
+        all_nets = list(self.nets.keys())[:]
+        net_dicts = self._comps_by_nets_dict if self._comps_by_nets_dict else self.components_by_nets
+        comp_dict = self._nets_by_comp_dict if self._nets_by_comp_dict else self.nets_by_components
+
+        def get_net_list(net_name, _net_list):
+            comps = []
+            if net_name in net_dicts:
+                comps = net_dicts[net_name]
+
+            for vals in comps:
+                refdes = vals
+                cmp = self._pedb.components.instances[refdes]
+                is_enabled = cmp.is_enabled
+                if not is_enabled:
+                    continue
+                val_type = cmp.type
+                if val_type not in ["Inductor", "Resistor", "Capacitor"]:
+                    continue
+                val_value = cmp.rlc_values
+                if refdes in exception_list:
+                    pass
+                elif val_type == "Inductor" and val_value[1] < inductor_below:
+                    pass
+                elif val_type == "Resistor" and val_value[0] < resistor_below:
+                    pass
+                elif val_type == "Capacitor" and val_value[2] > capacitor_above:
+                    pass
+                else:
+                    continue
+
+                for net in comp_dict[refdes]:
+                    if net not in _net_list:
+                        _net_list.append(net)
+                        get_net_list(net, _net_list)
+
+        while len(all_nets) > 0:
+            new_ext = [all_nets[0]]
+            get_net_list(new_ext[0], new_ext)
+            all_nets = [i for i in all_nets if i not in new_ext]
+            self._extendend_nets.append(new_ext)
+
+        return self._extendend_nets
+
     @staticmethod
     def _eval_arc_points(p1, p2, h, n=6, tol=1e-12):
         """Get the points of the arc.
 
         Parameters
         ----------
         p1 : list
```

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.87/pyaedt/edb_core/padstack.py`

 * *Files 2% similar despite different names*

```diff
@@ -828,14 +828,15 @@
         pad_offset_y="0.0",
         pad_rotation="0.0",
         start_layer=None,
         stop_layer=None,
         add_default_layer=False,
         anti_pad_x_size="600um",
         anti_pad_y_size="600um",
+        hole_range="from_upper_to_lower_pad",
     ):
         """Create a padstack.
 
         Parameters
         ----------
         padstackname : str, optional
             Name of the padstack. The default is ``None``.
@@ -876,14 +877,17 @@
             Stop layer of the padstack definition.
         add_default_layer : bool, optional
             Add ``"Default"`` to padstack definition. Default is ``False``.
         anti_pad_x_size : str, optional
             Only applicable to bullet and rectangle shape. The default is ``"600um"``.
         anti_pad_y_size : str, optional
             Only applicable to bullet and rectangle shape. The default is ``"600um"``.
+        hole_range : str, optional
+            Define the padstack hole range. Arguments supported, ``"through"``, ``"begin_on_upper_pad"``,
+            ``"end_on_lower_pad"``, ``"upper_pad_to_lower_pad"``.
 
         Returns
         -------
         str
             Name of the padstack if the operation is successful.
         """
         holediam = self._get_edb_value(holediam)
@@ -908,44 +912,50 @@
         rotation = self._get_edb_value(rotation)
 
         pad_offset_x = self._get_edb_value(pad_offset_x)
         pad_offset_y = self._get_edb_value(pad_offset_y)
         pad_rotation = self._get_edb_value(pad_rotation)
         anti_pad_x_size = self._get_edb_value(anti_pad_x_size)
         anti_pad_y_size = self._get_edb_value(anti_pad_y_size)
-
         padstackData.SetHoleParameters(ptype, holparam, value0, value0, value0)
-
         padstackData.SetHolePlatingPercentage(self._get_edb_value(20.0))
-        padstackData.SetHoleRange(self._edb.definition.PadstackHoleRange.UpperPadToLowerPad)
+        if hole_range == "through":  # pragma no cover
+            padstackData.SetHoleRange(self._edb.definition.PadstackHoleRange.Through)
+        elif hole_range == "begin_on_upper_pad":  # pragma no cover
+            padstackData.SetHoleRange(self._edb.definition.PadstackHoleRange.BeginOnUpperPad)
+        elif hole_range == "end_on_lower_pad":  # pragma no cover
+            padstackData.SetHoleRange(self._edb.definition.PadstackHoleRange.EndOnLowerPad)
+        elif hole_range == "upper_pad_to_lower_pad":  # pragma no cover
+            padstackData.SetHoleRange(self._edb.definition.PadstackHoleRange.UpperPadToLowerPad)
+        else:  # pragma no cover
+            self._logger.error("Unknown padstack hole range")
         padstackData.SetMaterial("copper")
         layers = list(self._pedb.stackup.signal_layers.keys())[:]
-        if start_layer and start_layer in layers:
+        if start_layer and start_layer in layers:  # pragma no cover
             layers = layers[layers.index(start_layer) :]
-        if stop_layer and stop_layer in layers:
+        if stop_layer and stop_layer in layers:  # pragma no cover
             layers = layers[: layers.index(stop_layer) + 1]
         pad_array = Array[type(paddiam)]([paddiam])
-        if pad_shape == "Circle":
+        if pad_shape == "Circle":  # pragma no cover
             pad_shape = self._edb.definition.PadGeometryType.Circle
-        elif pad_shape == "Rectangle":
+        elif pad_shape == "Rectangle":  # pragma no cover
             pad_array = Array[type(x_size)]([x_size, y_size])
             pad_shape = self._edb.definition.PadGeometryType.Rectangle
-        if antipad_shape == "Bullet":
+        if antipad_shape == "Bullet":  # pragma no cover
             antipad_array = Array[type(x_size)]([x_size, y_size, corner_radius])
             antipad_shape = self._edb.definition.PadGeometryType.Bullet
-        elif antipad_shape == "Rectangle":
+        elif antipad_shape == "Rectangle":  # pragma no cover
             antipad_array = Array[type(anti_pad_x_size)]([anti_pad_x_size, anti_pad_y_size])
             antipad_shape = self._edb.definition.PadGeometryType.Rectangle
-        else:
+        else:  # pragma no cover
             antipad_array = Array[type(antipaddiam)]([antipaddiam])
             antipad_shape = self._edb.definition.PadGeometryType.Circle
-        if add_default_layer:
+        if add_default_layer:  # pragma no cover
             layers = layers + ["Default"]
         for layer in layers:
-            # padparam_array = Array[type(paddiam)]([paddiam])
             padstackData.SetPadParameters(
                 layer,
                 self._edb.definition.PadType.RegularPad,
                 pad_shape,
                 pad_array,
                 pad_offset_x,
                 pad_offset_y,
```

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.87/pyaedt/edb_core/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.87/pyaedt/edb_core/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/emit.py` & `pyaedt-0.6.87/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/emit_core/Couplings.py` & `pyaedt-0.6.87/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/emit_core/__init__.py` & `pyaedt-0.6.87/pyaedt/emit_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/emit_core/emit_constants.py` & `pyaedt-0.6.87/pyaedt/emit_core/emit_constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/emit_core/interference_classification.py` & `pyaedt-0.6.87/pyaedt/emit_core/interference_classification.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.87/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/emit_core/results/revision.py` & `pyaedt-0.6.87/pyaedt/emit_core/results/revision.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.87/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.87/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/clr_module.py` & `pyaedt-0.6.87/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/configurations.py` & `pyaedt-0.6.87/pyaedt/generic/configurations.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/constants.py` & `pyaedt-0.6.87/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/design_types.py` & `pyaedt-0.6.87/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/filesystem.py` & `pyaedt-0.6.87/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/general_methods.py` & `pyaedt-0.6.87/pyaedt/generic/general_methods.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/grpc_plugin.py` & `pyaedt-0.6.87/pyaedt/generic/grpc_plugin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/grpc_plugin_dll.py` & `pyaedt-0.6.87/pyaedt/generic/grpc_plugin_dll.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.87/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.87/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/pdf.py` & `pyaedt-0.6.87/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/plot.py` & `pyaedt-0.6.87/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/process.py` & `pyaedt-0.6.87/pyaedt/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.87/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.87/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/toolkit.py` & `pyaedt-0.6.87/pyaedt/generic/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.87/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/hfss.py` & `pyaedt-0.6.87/pyaedt/hfss.py`

 * *Files 0% similar despite different names*

```diff
@@ -2876,15 +2876,15 @@
                 props["UseResist"] = True
                 props["Resistance"] = str(Rvalue) + "ohm"
             if Lvalue:
                 props["UseInduct"] = True
                 props["Inductance"] = str(Lvalue) + "H"
             if Cvalue:
                 props["UseCap"] = True
-                props["Capacitance"] = str(Cvalue) + "F"
+                props["Capacitance"] = str(Cvalue) + "farad"
 
             return self._create_boundary(sourcename, props, "Lumped RLC")
         return False
 
     @pyaedt_function_handler()
     def create_impedance_between_objects(
         self,
@@ -5788,22 +5788,22 @@
 
             props = OrderedDict({"Name": symmetry_name, "Faces": entity_list, "IsPerfectE": is_perfect_e})
             return self._create_boundary(symmetry_name, props, "Symmetry")
         except:
             return False
 
     @pyaedt_function_handler()
-    def set_impedance_multiplier(self, impedance):
+    def set_impedance_multiplier(self, multiplier):
         # type: (float) -> bool
         """Set impedance multiplier.
 
         Parameters
         ----------
-        impedance : float
-            Impedance.
+        multiplier : float
+            Impedance Multiplier.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
@@ -5823,15 +5823,15 @@
         >>> hfss.set_impedance_multiplier(2.0)
 
         """
         try:
             if self.solution_type not in ["Modal"]:
                 self.logger.error("Symmetry is only available with 'Modal' solution type.")
                 return False
-            self.oboundary.ChangeImpedanceMult(impedance)
+            self.oboundary.ChangeImpedanceMult(multiplier)
             return True
         except:
             return False
 
     @pyaedt_function_handler()
     def get_touchstone_data(self, setup_name, sweep_name=None, variation_dict=None):
         """
```

### Comparing `pyaedt-0.6.86/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.87/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/icepak.py` & `pyaedt-0.6.87/pyaedt/icepak.py`

 * *Files 1% similar despite different names*

```diff
@@ -2571,36 +2571,73 @@
         """
         mats = []
         for el in self.materials.gases:
             mats.extend(self.modeler.convert_to_selections(self.modeler.get_objects_by_material(el), True))
         return mats
 
     @pyaedt_function_handler()
-    def generate_fluent_mesh(self, object_lists=None):
+    def generate_fluent_mesh(
+        self,
+        object_lists=None,
+        meshtype="tetrahedral",
+        min_size=None,
+        max_size=None,
+        inflation_layer_number=3,
+        inflation_growth_rate=1.2,
+        mesh_growth_rate=1.2,
+    ):
         """Generate a Fluent mesh for a list of selected objects and assign the mesh automatically to the objects.
 
         Parameters
         ----------
         object_lists : list, optional
             List of objects to compute the Fluent mesh on. The default is ``None``, in which case
             all fluids objects are used to compute the mesh.
+        meshtype : str, optional
+            Mesh type. Options are ``"tethraedral"`` or ``"hexcore"``.
+        min_size : float, optional
+            Minimum mesh size. Default is smallest edge of objects/20.
+        max_size : float, optional
+            Maximum mesh size. Default is smallest edge of objects/5.
+        inflation_layer_number : int, optional
+            Inflation layer number. Default is ``3``.
+        inflation_growth_rate : float, optional
+            Inflation layer size. Default is ``1.2``.
+        mesh_growth_rate : float, optional
+            Growth rate. Default is ``1.2``.
 
         Returns
         -------
         :class:`pyaedt.modules.Mesh.MeshOperation`
         """
         version = self.aedt_version_id[-3:]
         ansys_install_dir = os.environ.get("ANSYS{}_DIR".format(version), "")
         if not ansys_install_dir:
             ansys_install_dir = os.environ.get("AWP_ROOT{}".format(version), "")
         assert ansys_install_dir, "Fluent {} has to be installed on to generate mesh.".format(version)
         assert os.getenv("ANSYS{}_DIR".format(version))
         if not object_lists:
             object_lists = self.get_liquid_objects()
             assert object_lists, "No Fluids objects found."
+        if not min_size or not max_size:
+            dims = []
+            # try:
+            #     dim = self.modeler["Region"].shortest_edge()[0].length
+            # except (AttributeError, KeyError, IndexError):
+            for obj in object_lists:
+                bb = self.modeler[obj].bounding_box
+                dd = [abs(bb[3] - bb[0]), abs(bb[4] - bb[1]), abs(bb[5] - bb[2])]
+                dims.append(min(dd))
+            dim = min(dims)
+            if not max_size:
+                max_size = dim / 5
+            if not min_size:
+                min_size = dim / 20
+            else:
+                min_size = min(min_size, max_size / 4)
         object_lists = self.modeler.convert_to_selections(object_lists, True)
         file_name = self.project_name
         sab_file_pointer = os.path.join(self.working_directory, file_name + ".sab")
         mesh_file_pointer = os.path.join(self.working_directory, file_name + ".msh")
         fl_uscript_file_pointer = os.path.join(self.working_directory, "FLUscript.jou")
         if os.path.exists(mesh_file_pointer):
             os.remove(mesh_file_pointer)
@@ -2623,14 +2660,25 @@
         fluent_script.write("(%py-exec \"workflow.InitializeWorkflow(WorkflowType=r'Watertight Geometry')\")\n")
         cmd = "(%py-exec \"workflow.TaskObject['Import Geometry']."
         cmd += "Arguments.setState({r'FileName': r'" + sab_file_pointer + "',})\")\n"
         fluent_script.write(cmd)
         fluent_script.write("(%py-exec \"workflow.TaskObject['Import Geometry'].Execute()\")\n")
         fluent_script.write("(%py-exec \"workflow.TaskObject['Add Local Sizing'].AddChildToTask()\")\n")
         fluent_script.write("(%py-exec \"workflow.TaskObject['Add Local Sizing'].Execute()\")\n")
+        fluent_script.write("(%py-exec \"meshtype = '{}'\")\n".format(meshtype))
+        fluent_script.write('(%py-exec "gr = {}")\n'.format(mesh_growth_rate))
+        fluent_script.write('(%py-exec "maxsize = {}")\n'.format(max_size))
+        fluent_script.write('(%py-exec "minsize = {}")\n'.format(min_size))
+        fluent_script.write('(%py-exec "nlayers = {}")\n'.format(inflation_layer_number))
+        fluent_script.write('(%py-exec "pgr = {}")\n'.format(inflation_growth_rate))
+        mesh_settings = "(%py-exec \"workflow.TaskObject['Generate the Surface Mesh'].Arguments.setState"
+        mesh_settings += "({r'CFDSurfaceMeshControls': {r'CellsPerGap': 3,r'CurvatureNormalAngle': 18,"
+        mesh_settings += "r'MaxSize': maxsize,r'MinSize': minsize,r'GrowthRate': gr},})\")\n"
+
+        fluent_script.write(mesh_settings)
         fluent_script.write("(%py-exec \"workflow.TaskObject['Generate the Surface Mesh'].Execute()\")\n")
         cmd = "(%py-exec \"workflow.TaskObject['Describe Geometry'].UpdateChildTasks(SetupTypeChanged=False)\")\n"
         fluent_script.write(cmd)
         cmd = "(%py-exec \"workflow.TaskObject['Describe Geometry']."
         cmd += "Arguments.setState({r'SetupType': r'The geometry consists of only fluid regions with no voids',})\")\n"
         fluent_script.write(cmd)
         cmd = "(%py-exec \"workflow.TaskObject['Describe Geometry'].UpdateChildTasks(SetupTypeChanged=True)\")\n"
@@ -2642,40 +2690,46 @@
         cmd = "(%py-exec \"workflow.TaskObject['Describe Geometry'].UpdateChildTasks(SetupTypeChanged=False)\")\n"
         fluent_script.write(cmd)
         fluent_script.write("(%py-exec \"workflow.TaskObject['Describe Geometry'].Execute()\")\n")
         fluent_script.write("(%py-exec \"workflow.TaskObject['Apply Share Topology'].Execute()\")\n")
         fluent_script.write("(%py-exec \"workflow.TaskObject['Update Boundaries'].Execute()\")\n")
         fluent_script.write("(%py-exec \"workflow.TaskObject['Update Regions'].Execute()\")\n")
         fluent_script.write("(%py-exec \"workflow.TaskObject['Add Boundary Layers'].AddChildToTask()\")\n")
+
         fluent_script.write("(%py-exec \"workflow.TaskObject['Add Boundary Layers'].InsertCompoundChildTask()\")\n")
         cmd = "(%py-exec \"workflow.TaskObject['smooth-transition_1']."
-        cmd += "Arguments.setState({r'BLControlName': r'smooth-transition_1',})\")\n"
+        cmd += "Arguments.setState({r'BLControlName': r'smooth-transition_1',"
+        cmd += "r'NumberOfLayers':nlayers, r'Rate':pgr})\")\n"
         fluent_script.write(cmd)
         fluent_script.write("(%py-exec \"workflow.TaskObject['Add Boundary Layers'].Arguments.setState({})\")\n")
         fluent_script.write("(%py-exec \"workflow.TaskObject['smooth-transition_1'].Execute()\")\n")
         # r'VolumeFill': r'hexcore' / r'tetrahedral'
         cmd = "(%py-exec \"workflow.TaskObject['Generate the Volume Mesh'].Arguments.setState({r'VolumeFill': "
-        cmd += "r'hexcore', r'VolumeMeshPreferences': {r'MergeBodyLabels': r'yes',},})\")\n"
+        cmd += "meshtype, r'VolumeMeshPreferences': {r'MergeBodyLabels': r'yes',},})\")\n"
         fluent_script.write(cmd)
         fluent_script.write("(%py-exec \"workflow.TaskObject['Generate the Volume Mesh'].Execute()\")\n")
         fluent_script.write("/file/hdf no\n")
         fluent_script.write('/file/write-mesh "' + mesh_file_pointer + '"\n')
         fluent_script.write("/file/stop-transcript\n")
         fluent_script.write("/exit,\n")
         fluent_script.close()
-
+        cmd = os.path.join(self.desktop_install_dir, "fluent", "ntbin", "win64", "fluent.exe")
+        if is_linux:  # pragma: no cover
+            cmd = os.path.join(ansys_install_dir, "fluent", "bin", "fluent")
         # Fluent command line parameters: -meshing -i <journal> -hidden -tm<x> (# processors for meshing) -wait
         fl_ucommand = [
-            os.path.join(self.desktop_install_dir, "fluent", "ntbin", "win64", "fluent.exe"),
+            cmd,
             "3d",
             "-meshing",
             "-hidden",
-            "-i" + '"' + fl_uscript_file_pointer + '"',
+            "-i",
+            '"' + fl_uscript_file_pointer + '"',
         ]
-        self.logger.info("Fluent is starting in BG.")
+        self.logger.info("Fluent is starting in Background with command line")
+        self.logger.info(" ".join(fl_ucommand))
         subprocess.call(fl_ucommand)
         if os.path.exists(mesh_file_pointer + ".trn"):
             os.remove(mesh_file_pointer + ".trn")
         if os.path.exists(fl_uscript_file_pointer):
             os.remove(fl_uscript_file_pointer)
         if os.path.exists(sab_file_pointer):
             os.remove(sab_file_pointer)
```

### Comparing `pyaedt-0.6.86/pyaedt/maxwell.py` & `pyaedt-0.6.87/pyaedt/maxwell.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.87/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/mechanical.py` & `pyaedt-0.6.87/pyaedt/mechanical.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/Console.py_build` & `pyaedt-0.6.87/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.87/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.87/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.87/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.87/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.87/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/amat.xml` & `pyaedt-0.6.87/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/ansys_cloud.areg` & `pyaedt-0.6.87/pyaedt/misc/ansys_cloud.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/console_setup.py` & `pyaedt-0.6.87/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.87/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.87/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.87/pyaedt/misc/install_extra_toolkits.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.87/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/misc.py` & `pyaedt-0.6.87/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.87/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.87/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.87/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.87/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.87/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.87/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/misc/template.acf` & `pyaedt-0.6.87/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.87/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.87/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.87/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.87/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.87/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.87/pyaedt/modeler/cad/Modeler.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 from collections import OrderedDict
 import copy
 import math
 import os
 import warnings
 
+# from pyaedt.generic.general_methods import property
+from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.constants import AEDT_UNITS
-
-# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import settings
 from pyaedt.modeler.cad.elements3d import EdgePrimitive
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import VertexPrimitive
@@ -94,14 +94,133 @@
 
     def __init__(self, modeler, name=None):
         self.auto_update = True
         self._modeler = modeler
         self.model_units = self._modeler.model_units
         self.name = name
 
+    def _get_coordinates_data(self):
+        self._props = {}
+        id2name = {1: "Global"}
+        name2refid = {}
+        if self._modeler._app.design_properties and "ModelSetup" in self._modeler._app.design_properties:
+            cs = self._modeler._app.design_properties["ModelSetup"]["GeometryCore"]["GeometryOperations"][
+                "CoordinateSystems"
+            ]
+            for ds in cs:
+                try:
+                    if isinstance(cs[ds], (OrderedDict, dict)):
+                        if cs[ds]["OperationType"] == "CreateRelativeCoordinateSystem":
+                            props = cs[ds]["RelativeCSParameters"]
+                            name = cs[ds]["Attributes"]["Name"]
+                            if name != self.name:
+                                continue
+                            cs_id = cs[ds]["ID"]
+                            id2name[cs_id] = name
+                            name2refid[name] = cs[ds]["ReferenceCoordSystemID"]
+                            self._props = CsProps(self, props)
+                            if "ZXZ" in props["Mode"]:
+                                self.mode = "zxz"
+                            elif "ZYZ" in props["Mode"]:
+                                self.mode = "zyz"
+                            else:
+                                self.mode = "axis"
+                        elif cs[ds]["OperationType"] == "CreateFaceCoordinateSystem":
+                            name = cs[ds]["Attributes"]["Name"]
+                            if name != self.name:
+                                continue
+                            cs_id = cs[ds]["ID"]
+                            id2name[cs_id] = name
+                            op_id = cs[ds]["PlaceHolderOperationID"]
+                            geometry_part = self._modeler._app.design_properties["ModelSetup"]["GeometryCore"][
+                                "GeometryOperations"
+                            ]["ToplevelParts"]["GeometryPart"]
+                            if isinstance(geometry_part, (OrderedDict, dict)):
+                                op = geometry_part["Operations"]["FaceCSHolderOperation"]
+                                if isinstance(op, (OrderedDict, dict)):
+                                    if op["ID"] == op_id:
+                                        props = op["FaceCSParameters"]
+                                        self._props = CsProps(self, props)
+                                elif isinstance(op, list):
+                                    for iop in op:
+                                        if iop["ID"] == op_id:
+                                            props = iop["FaceCSParameters"]
+                                            self._props = CsProps(self, props)
+                                            break
+                            elif isinstance(geometry_part, list):
+                                for gp in geometry_part:
+                                    op = gp["Operations"]["FaceCSHolderOperation"]
+                                    if isinstance(op, (OrderedDict, dict)):
+                                        if op["ID"] == op_id:
+                                            props = op["FaceCSParameters"]
+                                            self._props = CsProps(self, props)
+                                    elif isinstance(op, list):
+                                        for iop in op:
+                                            if iop["ID"] == op_id:
+                                                props = iop["FaceCSParameters"]
+                                                self._props = CsProps(self, props)
+                                                break
+                    elif isinstance(cs[ds], list):
+                        for el in cs[ds]:
+                            if el["OperationType"] == "CreateRelativeCoordinateSystem":
+                                props = el["RelativeCSParameters"]
+                                name = el["Attributes"]["Name"]
+                                if name != self.name:
+                                    continue
+                                cs_id = el["ID"]
+                                id2name[cs_id] = name
+                                name2refid[name] = el["ReferenceCoordSystemID"]
+                                self._props = CsProps(self, props)
+                                if "ZXZ" in props["Mode"]:
+                                    self.mode = "zxz"
+                                elif "ZYZ" in props["Mode"]:
+                                    self.mode = "zyz"
+                                else:
+                                    self.mode = "axis"
+                            elif el["OperationType"] == "CreateFaceCoordinateSystem":
+                                name = el["Attributes"]["Name"]
+                                if name != self.name:
+                                    continue
+                                cs_id = el["ID"]
+                                id2name[cs_id] = name
+                                op_id = el["PlaceHolderOperationID"]
+                                geometry_part = self._modeler._app.design_properties["ModelSetup"]["GeometryCore"][
+                                    "GeometryOperations"
+                                ]["ToplevelParts"]["GeometryPart"]
+                                if isinstance(geometry_part, (OrderedDict, dict)):
+                                    op = geometry_part["Operations"]["FaceCSHolderOperation"]
+                                    if isinstance(op, (OrderedDict, dict)):
+                                        if op["ID"] == op_id:
+                                            props = op["FaceCSParameters"]
+                                            self._props = CsProps(self, props)
+                                    elif isinstance(op, list):
+                                        for iop in op:
+                                            if iop["ID"] == op_id:
+                                                props = iop["FaceCSParameters"]
+                                                self._props = CsProps(self, props)
+                                                break
+                                elif isinstance(geometry_part, list):
+                                    for gp in geometry_part:
+                                        try:
+                                            op = gp["Operations"]["FaceCSHolderOperation"]
+                                        except KeyError:
+                                            continue
+                                        if isinstance(op, (OrderedDict, dict)):
+                                            if op["ID"] == op_id:
+                                                props = op["FaceCSParameters"]
+                                                self._props = CsProps(self, props)
+                                        elif isinstance(op, list):
+                                            for iop in op:
+                                                if iop["ID"] == op_id:
+                                                    props = iop["FaceCSParameters"]
+                                                    self._props = CsProps(self, props)
+                                                    break
+                except:
+                    pass
+
     @pyaedt_function_handler()
     def _dim_arg(self, value, units=None):
         """Dimension argument.
 
         Parameters
         ----------
         value :
@@ -245,29 +364,15 @@
 
         Returns
         -------
         :class:`pyaedt.modeler.Modeler.CSProps`
         """
         if self._props or settings.aedt_version <= "2022.2" or self.name is None:
             return self._props
-        obj1 = self._modeler.oeditor.GetChildObject(self.name)
-        props = {}
-        origin = obj1.GetPropValue("Origin")
-        props["Origin"] = origin
-        move_cs_to_end = obj1.GetPropValue("Always Move CS to End")
-        props["MoveToEnd"] = move_cs_to_end
-        move_cs_to_end = obj1.GetPropValue("Axis")
-        props["WhichAxis"] = move_cs_to_end
-        move_cs_to_end = obj1.GetPropValue("Z Rotation Angle")
-        props["ZRotationAngle"] = move_cs_to_end
-        move_cs_to_end = obj1.GetPropValue("Position Offset XY/X")
-        props["XOffset"] = move_cs_to_end
-        move_cs_to_end = obj1.GetPropValue("Position Offset XY/Y")
-        props["YOffset"] = move_cs_to_end
-        self._props = CsProps(self, props)
+        self._get_coordinates_data()
         return self._props
 
     @property
     def _part_name(self):
         """Internally get the part name which the face belongs to"""
         if not self.face_id:
             # face_id has not been defined yet
@@ -528,20 +633,23 @@
         self._mode = None
 
     @property
     def mode(self):
         """Coordinate System mode."""
         if self._mode:
             return self._mode
-        if "Axis" in self.props.get("Mode", ""):
-            self._mode = "axis"
-        elif "ZXZ" in self.props.get("Mode", ""):
-            self._mode = "zxz"
-        elif "ZYZ" in self.props.get("Mode", ""):
-            self._mode == "zyz"
+        try:
+            if "Axis" in self.props["Mode"]:
+                self._mode = "axis"
+            elif "ZXZ" in self.props["Mode"]:
+                self._mode = "zxz"
+            elif "ZYZ" in self.props["Mode"]:
+                self._mode = "zyz"
+        except:
+            pass
         return self._mode
 
     @mode.setter
     def mode(self, value):
         self._mode = value
 
     @property
@@ -550,37 +658,15 @@
 
         Returns
         -------
         :class:`pyaedt.modeler.Modeler.CSProps`
         """
         if self._props or settings.aedt_version <= "2022.2" or self.name is None:
             return self._props
-        obj1 = self._modeler.oeditor.GetChildObject(self.name)
-        props = {}
-        origin = obj1.GetPropValue("Origin")
-        props["OriginX"] = origin[1]
-        props["OriginY"] = origin[3]
-        props["OriginZ"] = origin[5]
-        props["Mode"] = obj1.GetPropValue("Mode")
-        if "X Axis" in obj1.GetPropNames():
-            axisvec = obj1.GetPropValue("X Axis")
-            props["XAxisXvec"] = axisvec[1]
-            props["XAxisYvec"] = axisvec[3]
-            props["XAxisZvec"] = axisvec[5]
-            ypoint = obj1.GetPropValue("Y Point")
-
-            props["YAxisXvec"] = ypoint[1]
-            props["YAxisYvec"] = ypoint[3]
-            props["YAxisZvec"] = ypoint[5]
-        else:
-            props["Phi"] = obj1.GetPropValue("Phi")
-            props["Theta"] = obj1.GetPropValue("Theta")
-            props["Psi"] = obj1.GetPropValue("Psi")
-        self._props = CsProps(self, props)
-        return self._props
+        self._get_coordinates_data()
 
     @property
     def ref_cs(self):
         """Reference coordinate system getter and setter.
 
         Returns
         -------
@@ -1356,15 +1442,15 @@
         Returns
         -------
         :class:`pyaedt.modules.MaterialLib.Materials`
 
         """
         return self._app.materials
 
-    def _get_coordinates_data(self):
+    def _get_coordinates_data(self):  # pragma: no cover
         coord = []
         id2name = {1: "Global"}
         name2refid = {}
         if self._app.design_properties and "ModelSetup" in self._app.design_properties:
             cs = self._app.design_properties["ModelSetup"]["GeometryCore"]["GeometryOperations"]["CoordinateSystems"]
             for ds in cs:
                 try:
@@ -2104,32 +2190,77 @@
             cs = coordinate_system
         elif isinstance(coordinate_system, str):
             if coordinate_system not in cs_names:  # pragma: no cover
                 raise AttributeError("Specified coordinate system does not exist in the design.")
             cs = self.coordinate_systems[cs_names.index(coordinate_system)]
         else:  # pragma: no cover
             raise AttributeError("coordinate_system must either be a string or a CoordinateSystem object.")
-        o, q = self.reference_cs_to_global(coordinate_system)
-        x, y, _ = GeometryOperators.quaternion_to_axis(q)
-        reference_cs = "Global"
-        name = cs.name + "_RefToGlobal"
-        if name in cs_names:
-            name = cs.name + generate_unique_name("_RefToGlobal")
-        cs = CoordinateSystem(self)
-        if cs:
-            result = cs.create(
-                origin=o,
-                reference_cs=reference_cs,
-                name=name,
-                mode="axis",
-                x_pointing=x,
-                y_pointing=y,
-            )
-            if result:
-                return cs
+        if isinstance(cs, CoordinateSystem):
+            o, q = self.reference_cs_to_global(coordinate_system)
+            x, y, _ = GeometryOperators.quaternion_to_axis(q)
+            reference_cs = "Global"
+            name = cs.name + "_RefToGlobal"
+            if name in cs_names:
+                name = cs.name + generate_unique_name("_RefToGlobal")
+            cs = CoordinateSystem(self)
+            if cs:
+                result = cs.create(
+                    origin=o,
+                    reference_cs=reference_cs,
+                    name=name,
+                    mode="axis",
+                    x_pointing=x,
+                    y_pointing=y,
+                )
+                if result:
+                    return cs
+        elif isinstance(cs, FaceCoordinateSystem):
+            name = cs.name + "_RefToGlobal"
+            if name in cs_names:
+                name = cs.name + generate_unique_name("_RefToGlobal")
+            face_cs = FaceCoordinateSystem(self, props=cs.props, name=name, face_id=cs.props["FaceID"])
+            obj = [
+                obj for obj in self._app.modeler.object_list for face in obj.faces if face.id == face_cs.props["FaceID"]
+            ][0]
+            face = [face for face in obj.faces if face.id == face_cs.props["FaceID"]][0]
+            if face_cs.props["Origin"]["PositionType"] == "FaceCenter":
+                origin = face
+            elif face_cs.props["Origin"]["PositionType"] == "EdgeCenter":
+                origin = [edge for edge in face.edges if edge.id == face_cs.props["Origin"]["EntityID"]][0]
+            elif face_cs.props["Origin"]["PositionType"] == "OnVertex":
+                edge = [
+                    edge
+                    for edge in face.edges
+                    for vertex in edge.vertices
+                    if vertex.id == face_cs.props["Origin"]["EntityID"]
+                ][0]
+                origin = [v for v in edge.vertices if v.id == face_cs.props["Origin"]["EntityID"]][0]
+            if face_cs.props["AxisPosn"]["PositionType"] == "EdgeCenter":
+                axis_position = [edge for edge in face.edges if edge.id == face_cs.props["AxisPosn"]["EntityID"]][0]
+            elif face_cs.props["AxisPosn"]["PositionType"] == "OnVertex":
+                edge = [
+                    edge
+                    for edge in face.edges
+                    for vertex in edge.vertices
+                    if vertex.id == face_cs.props["AxisPosn"]["EntityID"]
+                ][0]
+                axis_position = [v for v in edge.vertices if v.id == face_cs.props["AxisPosn"]["EntityID"]][0]
+            if face_cs:
+                result = face_cs.create(
+                    face=face,
+                    origin=origin,
+                    axis_position=axis_position,
+                    axis=face_cs.props["WhichAxis"],
+                    name=name,
+                    offset=[face_cs["XOffset"], face_cs["YOffset"]],
+                    rotation=decompose_variable_value(face_cs["ZRotationAngle"])[0],
+                    always_move_to_end=face_cs["MoveToEnd"],
+                )
+                if result:
+                    return face_cs
         return False
 
     @pyaedt_function_handler()
     def set_objects_deformation(self, objects):
         """Assign deformation objects to a Workbench link.
 
         Parameters
```

### Comparing `pyaedt-0.6.86/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.87/pyaedt/modeler/cad/Primitives.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.87/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.87/pyaedt/modeler/cad/Primitives3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.87/pyaedt/modeler/cad/components_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -801,14 +801,61 @@
             self._group_name,
             self._mesh_assembly,
             self._parameters,
             self._target_coordinate_system,
         )
 
     @pyaedt_function_handler()
+    def get_component_filepath(self):
+        """Get 3d component file path.
+
+        Returns
+        -------
+        str
+            Path of the 3d component file.
+        """
+
+        return self._primitives._app.get_oo_object(self._primitives._app.oeditor, self.definition_name).GetPropValue(
+            "3D Component File Path"
+        )
+
+    @pyaedt_function_handler()
+    def update_definition(self, password="", new_filepath=""):
+        """Update 3d component definition.
+
+        Parameters
+        ----------
+        password : str, optional
+            Password for encrypted models. The default value is ``""``.
+        new_filepath : str, optional
+            New path containing the 3d component file. The default value is ``""``, which means
+            that the 3d component file has not changed.
+
+        Returns
+        -------
+        bool
+            True if successful.
+        """
+
+        self._primitives._app.oeditor.UpdateComponentDefinition(
+            [
+                "NAME:UpdateDefinitionData",
+                "ForLocalEdit:=",
+                False,
+                "DefinitionNames:=",
+                self.definition_name,
+                "Passwords:=",
+                [password],
+                "NewFilePath:=",
+                new_filepath,
+            ]
+        )
+        return True
+
+    @pyaedt_function_handler()
     def edit_definition(self, password=""):
         """Edit 3d Definition. Open AEDT Project and return Pyaedt Object.
 
         Parameters
         ----------
         password : str, optional
             Password for encrypted models. The default value is ``""``.
```

### Comparing `pyaedt-0.6.86/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.87/pyaedt/modeler/cad/elements3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,16 @@
         >>> oEditor.GetVertexPosition
 
         """
         if self._position:
             return self._position
         try:
             vertex_data = list(self.oeditor.GetVertexPosition(self.id))
-            return [float(i) for i in vertex_data]
+            self._position = [float(i) for i in vertex_data]
+            return self._position
         except Exception as e:
             return None
 
     def __repr__(self):
         return "Vertex " + str(self.id)
 
     def __str__(self):
@@ -594,15 +595,15 @@
 
         >>> oEditor.GetFaceCenter
 
         """
         try:
             return [float(i) for i in self.oeditor.GetFaceCenter(self.id)]
         except:  # pragma: no cover
-            vtx = self.vertices
+            vtx = self.vertices[:]
             if len(vtx) > 1:
                 return GeometryOperators.get_polygon_centroid([pos.position for pos in vtx])
             elif len(vtx) <= 1:
                 eval_points = 4
                 try:
                     edge = self.edges[0]
                 except IndexError:
```

### Comparing `pyaedt-0.6.86/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.87/pyaedt/modeler/cad/object3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.87/pyaedt/modeler/cad/polylines.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/calculators.py` & `pyaedt-0.6.87/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1784,44 +1784,71 @@
             for line in f:
                 if ".subckt" in line.lower():
                     pinNames = [i.strip() for i in re.split(" |\t", line) if i]
                     models.append(pinNames[1])
         return models
 
     @pyaedt_function_handler()
-    def create_component_from_spicemodel(self, model_path, model_name=None, create_component=True, location=None):
+    def create_component_from_spicemodel(
+        self,
+        model_path,
+        model_name=None,
+        create_component=True,
+        location=None,
+        symbol_path="Nexxim Circuit Elements\\Nexxim_symbols:",
+        symbol_name="",
+    ):
         """Create and place a new component based on a spice .lib file.
 
         Parameters
         ----------
         model_path : str
             Path to .lib file.
         model_name : str, optional
             Model name to import. If `None` the first subckt in the lib file will be placed.
         create_component : bool, optional
             If set to ``True``, create a spice model component. Otherwise, only import the spice model.
         location : list, optional
             Position in the schematic of the new component.
+        symbol_path : str, optional
+            Path to the symbol library.
+            Default value is ``"Nexxim Circuit Elements\\Nexxim_symbols:"``.
+        symbol_name : str, optional
+            Symbol name to replace the spice model with.
+            Default value is an empty string which means the default symbol for spice is used.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
+
+        Examples
+        --------
+        >>> from pyaedt import Circuit
+        >>> cir = Circuit(specified_version="2023.2")
+        >>> model = os.path.join("Your path", "test.lib")
+        >>> cir.modeler.schematic.create_component_from_spicemodel(model_path=model,
+        >>>                                                        model_name="GRM1234",
+        >>>                                                        symbol_name="nexx_cap")
+        >>> cir.release_desktop(False, False)
         """
         models = self._parse_spice_model(model_path)
         if not model_name and models:
             model_name = models[0]
         elif model_name not in models:
             return False
         arg = ["NAME:Options", "Mode:=", 2, "Overwrite:=", False, "SupportsSimModels:=", False, "LoadOnly:=", False]
         arg2 = ["NAME:Models"]
         for el in models:
             arg2.append(el + ":=")
             if el == model_name:
-                arg2.append([True, "", "", False])
+                if symbol_path and symbol_name:
+                    arg2.append([True, symbol_path + symbol_name, "", False])
+                else:
+                    arg2.append([True, "", "", False])
             else:
                 arg2.append([False, "", "", False])
         arg.append(arg2)
         self.o_component_manager.ImportModelsFromFile(model_path.replace("\\", "/"), arg)
 
         if create_component:
             return self.create_component(
```

### Comparing `pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.87/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.87/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.87/pyaedt/modeler/modeler2d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.87/pyaedt/modeler/modeler3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.87/pyaedt/modeler/modelerpcb.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,24 +181,32 @@
 
         """
         mess = "`primitives` is deprecated.\n"
         mess += " Use `app.modeler` directly to instantiate primitives methods."
         warn(mess, DeprecationWarning)
         return self._primitives
 
-    @property
-    def obounding_box(self):
-        """Bounding box.
+    @pyaedt_function_handler
+    def obounding_box(self, object_name):
+        """Bounding box of a specified object.
+
+        Returns
+        -------
+        list
+            List of [LLx, LLy, URx, URy] coordinates.
 
         References
         ----------
 
-        >>> oEditor.GetModelBoundingBox
+        >>> oEditor.GetBBox
         """
-        return self.oeditor.GetModelBoundingBox()
+        bb = self.oeditor.GetBBox(object_name)
+        pll = bb.BBoxLL()
+        pur = bb.BBoxUR()
+        return [pll.GetX(), pll.GetY(), pur.GetX(), pur.GetY()]
 
     @pyaedt_function_handler()
     def _arg_with_dim(self, value, units=None):
         if units is None:
             units = self.model_units
         if type(value) is str:
             try:
```

### Comparing `pyaedt-0.6.86/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.87/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.87/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files 0% similar despite different names*

```diff
@@ -853,14 +853,30 @@
 
     def __init__(self, primitives, name, prim_type="poly", is_void=False):
         Objec3DLayout.__init__(self, primitives, prim_type)
         self.is_void = is_void
         self._name = name
 
     @property
+    def obounding_box(self):
+        """Bounding box of a specified object.
+
+        Returns
+        -------
+        list
+            List of [LLx, LLy, URx, URy] coordinates.
+
+        References
+        ----------
+
+        >>> oEditor.GetBBox
+        """
+        return self._primitives.obounding_box(self.name)
+
+    @property
     def name(self):
         """Name of Primitive."""
         return self._name
 
     @name.setter
     def name(self, value):
         try:
@@ -1454,34 +1470,43 @@
 
         >>> oEditor.GetPropertyValue
         """
         return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "TotalLength")
 
     @property
     def center_line(self):
-        """Get the center line points.
+        """Get the center line points and arc height.
 
         Returns
         -------
         dict
             Points.
         """
-        props = [i for i in list(self._oeditor.GetProperties("BaseElementTab", self.name)) if i.startswith("Pt")]
+        props = [
+            i
+            for i in list(self._oeditor.GetProperties("BaseElementTab", self.name))
+            if i.startswith("Pt") or i.startswith("ArcHeight")
+        ]
         self._center_line = {}
         for i in props:
             self._center_line[i] = [
                 i.strip() for i in self._oeditor.GetPropertyValue("BaseElementTab", self.name, i).split(",")
             ]
         return self._center_line
 
     @center_line.setter
     def center_line(self, points):
         u = self._primitives.model_units
         for point_name, value in points.items():
-            vpoint = ["NAME:{}".format(point_name), "X:=", _dim_arg(value[0], u), "Y:=", _dim_arg(value[1], u)]
+            if len(value) == 2:
+                vpoint = ["NAME:{}".format(point_name), "X:=", _dim_arg(value[0], u), "Y:=", _dim_arg(value[1], u)]
+            elif isinstance(value, list):
+                vpoint = ["NAME:{}".format(point_name), "Value:=", _dim_arg(value[0], u)]
+            else:
+                vpoint = ["NAME:{}".format(point_name), "Value:=", _dim_arg(value, u)]
             self.change_property(vpoint)
         self._center_line = {}
 
     @pyaedt_function_handler()
     def add(self, point, position=0):
         """Add a new point to the center line.
```

### Comparing `pyaedt-0.6.86/pyaedt/modeler/schematic.py` & `pyaedt-0.6.87/pyaedt/modeler/schematic.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,24 +75,14 @@
 
         References
         ----------
 
         >>> oEditor = oDesign.SetActiveEditor("SchematicEditor")"""
         return self._app.oeditor
 
-    @property
-    def obounding_box(self):
-        """Bounding box.
-
-        References
-        ----------
-
-        >>> oEditor.GetModelBoundingBox()"""
-        return self.oeditor.GetModelBoundingBox()
-
     @pyaedt_function_handler()
     def zoom_to_fit(self):
         """Zoom To Fit.
 
         References
         ----------
```

### Comparing `pyaedt-0.6.86/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.87/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/Boundary.py` & `pyaedt-0.6.87/pyaedt/modules/Boundary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.87/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.87/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.87/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.87/pyaedt/modules/LayerStackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/Material.py` & `pyaedt-0.6.87/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.87/pyaedt/modules/MaterialLib.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/Mesh.py` & `pyaedt-0.6.87/pyaedt/modules/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.87/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.87/pyaedt/modules/MeshIcepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.87/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.87/pyaedt/modules/PostProcessor.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.87/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.87/pyaedt/modules/SolveSetup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.87/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.87/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/report_templates.py` & `pyaedt-0.6.87/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/modules/solutions.py` & `pyaedt-0.6.87/pyaedt/modules/solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/q3d.py` & `pyaedt-0.6.87/pyaedt/q3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/rmxprt.py` & `pyaedt-0.6.87/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.87/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.87/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.87/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.87/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.87/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.87/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.87/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.87/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.87/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.87/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.87/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.87/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.87/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.87/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.87/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/siwave.py` & `pyaedt-0.6.87/pyaedt/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyaedt/twinbuilder.py` & `pyaedt-0.6.87/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.86/pyproject.toml` & `pyaedt-0.6.87/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
     "osmnx",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
     "pyvista==0.40.2; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "recommonmark==0.7.1",
     "scikit-learn==1.3.0",
-    "Sphinx==7.0.1",
+    "Sphinx==7.1.0",
     "sphinx-autobuild==2021.3.14",
-    "sphinx-autodoc-typehints==1.23.3",
+    "sphinx-autodoc-typehints==1.24.0",
     "sphinx-copybutton==0.5.2",
     "sphinx-gallery==0.13.0",
     "sphinx-notfound-page==0.8.3",
     "sphinxcontrib-websupport==1.2.4",
     "SRTM.py",
     "utm",
     "scikit-rf",
@@ -123,17 +123,19 @@
     "openpyxl==3.1.2",
 ]
 
 [tool.flit.module]
 name = "pyaedt"
 
 [project.urls]
-"Bug Tracker" = "https://github.com/pyansys/pyaedt/issues"
-"Documentation" = "https://aedt.docs.pyansys.com"
-"Source Code" = "https://github.com/pyansys/pyaedt"
+Bugs = "https://github.com/ansys/pyaedt/issues"
+Documentation = "https://aedt.docs.pyansys.com"
+Source = "https://github.com/ansys/pyaedt"
+Discussions = "https://github.com/ansys/pyaedt/discussions"
+Releases = "https://github.com/ansys/pyaedt/releases"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
```

### Comparing `pyaedt-0.6.86/PKG-INFO` & `pyaedt-0.6.87/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.86
+Version: 0.6.87
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -50,17 +50,17 @@
 Requires-Dist: osmnx ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
 Requires-Dist: pyvista==0.40.2 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: recommonmark==0.7.1 ; extra == "doc"
 Requires-Dist: scikit-learn==1.3.0 ; extra == "doc"
-Requires-Dist: Sphinx==7.0.1 ; extra == "doc"
+Requires-Dist: Sphinx==7.1.0 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==1.23.3 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==1.24.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: SRTM.py ; extra == "doc"
 Requires-Dist: utm ; extra == "doc"
 Requires-Dist: scikit-rf ; extra == "doc"
@@ -96,17 +96,19 @@
 Requires-Dist: pytest-xdist==3.3.1 ; extra == "tests"
 Requires-Dist: pyvista==0.40.2 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: scikit-learn==1.3.0 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
 Requires-Dist: utm ; extra == "tests"
 Requires-Dist: scikit-rf ; extra == "tests"
-Project-URL: Bug Tracker, https://github.com/pyansys/pyaedt/issues
+Project-URL: Bugs, https://github.com/ansys/pyaedt/issues
+Project-URL: Discussions, https://github.com/ansys/pyaedt/discussions
 Project-URL: Documentation, https://aedt.docs.pyansys.com
-Project-URL: Source Code, https://github.com/pyansys/pyaedt
+Project-URL: Releases, https://github.com/ansys/pyaedt/releases
+Project-URL: Source, https://github.com/ansys/pyaedt
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: full
 Provides-Extra: tests
 
 <!-- -->
 <a name="readme-top"></a>
```

