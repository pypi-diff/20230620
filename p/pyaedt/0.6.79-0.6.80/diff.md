# Comparing `tmp/pyaedt-0.6.79.tar.gz` & `tmp/pyaedt-0.6.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.79.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyaedt-0.6.80.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.6.79.tar` & `pyaedt-0.6.80.tar`

### file list

```diff
@@ -1,255 +1,255 @@
--rw-r--r--   0        0        0     1111 2023-05-30 06:59:37.486926 pyaedt-0.6.79/LICENSE
--rw-r--r--   0        0        0     9947 2023-05-30 06:59:37.486926 pyaedt-0.6.79/README.md
--rw-r--r--   0        0        0     2691 2023-06-05 18:57:16.886587 pyaedt-0.6.79/pyaedt/__init__.py
--rw-r--r--   0        0        0    26683 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    88300 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    41317 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17066 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19852 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4431 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4596 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   129320 2023-06-05 14:54:59.781956 pyaedt-0.6.79/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    75524 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12464 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    36749 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    62954 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/circuit.py
--rw-r--r--   0        0        0    10247 2023-06-05 09:04:16.749339 pyaedt-0.6.79/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    64951 2023-06-05 14:54:59.781956 pyaedt-0.6.79/pyaedt/desktop.py
--rw-r--r--   0        0        0    15104 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/dlls/PDFReport/AnsysReport.deps.json
--rw-r--r--   0        0        0    23552 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1092 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0   204800 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
--rw-r--r--   0        0        0   577445 2023-05-30 06:59:39.440208 pyaedt-0.6.79/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
--rw-r--r--   0        0        0     9836 2023-05-30 06:59:39.440208 pyaedt-0.6.79/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   238592 2023-05-30 06:59:39.440208 pyaedt-0.6.79/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
--rw-r--r--   0        0        0   115712 2023-05-30 06:59:39.440208 pyaedt-0.6.79/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
--rw-r--r--   0        0        0   705296 2023-05-30 06:59:39.455836 pyaedt-0.6.79/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   712253 2023-05-30 06:59:39.455836 pyaedt-0.6.79/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0    80384 2023-05-30 06:59:39.455836 pyaedt-0.6.79/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
--rw-r--r--   0        0        0   546816 2023-05-30 06:59:39.471459 pyaedt-0.6.79/pyaedt/dlls/PDFReport/PdfSharpCore.dll
--rw-r--r--   0        0        0   367616 2023-05-30 06:59:39.471459 pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
--rw-r--r--   0        0        0   536367 2023-05-30 06:59:39.471459 pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
--rw-r--r--   0        0        0  1229824 2023-05-30 06:59:39.487088 pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
--rw-r--r--   0        0        0  3285773 2023-05-30 06:59:39.502713 pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
--rw-r--r--   0        0        0   120664 2023-05-30 06:59:39.502713 pyaedt-0.6.79/pyaedt/dlls/PDFReport/System.Runtime.dll
--rw-r--r--   0        0        0  1505294 2023-05-30 06:59:39.518353 pyaedt-0.6.79/pyaedt/dlls/PDFReport/System.Runtime.xml
--rw-r--r--   0        0        0     5632 2023-05-30 06:59:39.518353 pyaedt-0.6.79/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
--rw-r--r--   0        0        0   160754 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
--rw-r--r--   0        0        0    23386 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/downloads.py
--rw-r--r--   0        0        0   136802 2023-06-05 14:54:59.781956 pyaedt-0.6.79/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    92242 2023-06-05 09:36:43.922575 pyaedt-0.6.79/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-06-05 09:36:43.922575 pyaedt-0.6.79/pyaedt/edb_core/dotnet/__init__.py
--rw-r--r--   0        0        0    31497 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/dotnet/database.py
--rw-r--r--   0        0        0     7909 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/dotnet/layout.py
--rw-r--r--   0        0        0    48210 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/dotnet/primitive.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    32946 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0    40100 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/edb_core/edb_data/control_file.py
--rw-r--r--   0        0        0      937 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      867 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    12243 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    65661 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20386 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     4025 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    61171 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    33851 2023-06-05 15:29:29.398358 pyaedt-0.6.79/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0   101786 2023-06-05 14:54:59.781956 pyaedt-0.6.79/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36324 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    33847 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     3923 2023-06-05 14:54:59.781956 pyaedt-0.6.79/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2432 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     3258 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    66975 2023-06-05 14:54:59.797581 pyaedt-0.6.79/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2850 2023-06-05 09:36:43.953828 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7763 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4703 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11390 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21800 2023-06-05 09:36:43.953828 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    47125 2023-06-05 14:54:59.797581 pyaedt-0.6.79/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33310 2023-06-05 09:36:43.953828 pyaedt-0.6.79/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    44030 2023-06-05 14:54:59.797581 pyaedt-0.6.79/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    47600 2023-06-05 14:54:59.797581 pyaedt-0.6.79/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    57553 2023-06-05 14:54:59.797581 pyaedt-0.6.79/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   109207 2023-06-05 09:36:43.953828 pyaedt-0.6.79/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    11363 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/emit.py
--rw-r--r--   0        0        0     3555 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     3291 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/emit_core/EmitConstants.py
--rw-r--r--   0        0        0     1091 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0        2 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7406 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    13338 2023-06-05 14:54:59.797581 pyaedt-0.6.79/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    11758 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3257 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83444 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    21891 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3395 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    69591 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0    25808 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     6989 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0     9795 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    62327 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11301 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/process.py
--rw-r--r--   0        0        0    20326 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3466 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60412 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17095 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   253082 2023-06-05 09:04:16.749339 pyaedt-0.6.79/pyaedt/hfss.py
--rw-r--r--   0        0        0    82916 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   168417 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/icepak.py
--rw-r--r--   0        0        0   118479 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7803 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24316 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3695 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     2380 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10210 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     3731 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     3818 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14107 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    20051 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16840 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120888 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   194639 2023-05-30 14:16:58.540805 pyaedt-0.6.79/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   116607 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11387 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   127894 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    31589 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49057 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59078 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53131 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12645 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    42629 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    32780 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8212 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    63100 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15149 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    32013 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    68135 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6952 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    59936 2023-05-30 14:16:58.540805 pyaedt-0.6.79/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    31327 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    49892 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    65639 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    23689 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    30094 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   114715 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71549 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51967 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40465 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82903 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28363 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53226 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11976 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    26105 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   173007 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64104 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   119432 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33257 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    28709 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103333 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   125079 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    95908 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/q3d.py
--rw-r--r--   0        0        0    10581 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7632 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10410 2023-06-05 09:36:43.953828 pyaedt-0.6.79/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4426 2023-06-01 13:49:54.137333 pyaedt-0.6.79/pyproject.toml
--rw-r--r--   0        0        0    15568 1970-01-01 00:00:00.000000 pyaedt-0.6.79/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-16 06:59:23.102429 pyaedt-0.6.80/LICENSE
+-rw-r--r--   0        0        0     9947 2023-05-16 06:59:23.102429 pyaedt-0.6.80/README.md
+-rw-r--r--   0        0        0     2691 2023-06-13 16:44:32.437795 pyaedt-0.6.80/pyaedt/__init__.py
+-rw-r--r--   0        0        0    26683 2023-05-24 15:53:22.079958 pyaedt-0.6.80/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-05-16 06:59:25.180542 pyaedt-0.6.80/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    88300 2023-05-29 06:50:09.584617 pyaedt-0.6.80/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    41317 2023-05-29 06:50:09.584617 pyaedt-0.6.80/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    17066 2023-05-29 06:50:09.584617 pyaedt-0.6.80/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-05-16 06:59:25.196166 pyaedt-0.6.80/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19852 2023-05-29 06:50:09.584617 pyaedt-0.6.80/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4431 2023-05-29 06:50:09.584617 pyaedt-0.6.80/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4596 2023-05-29 06:50:09.584617 pyaedt-0.6.80/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   129320 2023-06-13 10:43:12.615480 pyaedt-0.6.80/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-05-16 06:59:25.196166 pyaedt-0.6.80/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    75524 2023-05-29 06:50:09.600210 pyaedt-0.6.80/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.196166 pyaedt-0.6.80/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12464 2023-05-29 06:50:09.600210 pyaedt-0.6.80/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    36749 2023-05-29 06:50:09.600210 pyaedt-0.6.80/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    62954 2023-05-23 13:08:30.544249 pyaedt-0.6.80/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10247 2023-06-05 09:41:19.525305 pyaedt-0.6.80/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    64951 2023-06-05 13:38:36.375818 pyaedt-0.6.80/pyaedt/desktop.py
+-rw-r--r--   0        0        0    15104 2023-05-16 06:59:25.196166 pyaedt-0.6.80/pyaedt/dlls/PDFReport/AnsysReport.deps.json
+-rw-r--r--   0        0        0    23552 2023-05-16 06:59:25.196166 pyaedt-0.6.80/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1092 2023-05-16 06:59:25.211792 pyaedt-0.6.80/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0   204800 2023-05-16 06:59:25.211792 pyaedt-0.6.80/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
+-rw-r--r--   0        0        0   577445 2023-05-16 06:59:25.211792 pyaedt-0.6.80/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
+-rw-r--r--   0        0        0     9836 2023-05-16 06:59:25.211792 pyaedt-0.6.80/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   238592 2023-05-16 06:59:25.211792 pyaedt-0.6.80/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
+-rw-r--r--   0        0        0   115712 2023-05-16 06:59:25.211792 pyaedt-0.6.80/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
+-rw-r--r--   0        0        0   705296 2023-05-16 06:59:25.227417 pyaedt-0.6.80/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   712253 2023-05-16 06:59:25.227417 pyaedt-0.6.80/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0    80384 2023-05-16 06:59:25.227417 pyaedt-0.6.80/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
+-rw-r--r--   0        0        0   546816 2023-05-16 06:59:25.243041 pyaedt-0.6.80/pyaedt/dlls/PDFReport/PdfSharpCore.dll
+-rw-r--r--   0        0        0   367616 2023-05-16 06:59:25.243041 pyaedt-0.6.80/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
+-rw-r--r--   0        0        0   536367 2023-05-16 06:59:25.243041 pyaedt-0.6.80/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
+-rw-r--r--   0        0        0  1229824 2023-05-16 06:59:25.258665 pyaedt-0.6.80/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
+-rw-r--r--   0        0        0  3285773 2023-05-16 06:59:25.274293 pyaedt-0.6.80/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
+-rw-r--r--   0        0        0   120664 2023-05-16 06:59:25.289918 pyaedt-0.6.80/pyaedt/dlls/PDFReport/System.Runtime.dll
+-rw-r--r--   0        0        0  1505294 2023-05-16 06:59:25.289918 pyaedt-0.6.80/pyaedt/dlls/PDFReport/System.Runtime.xml
+-rw-r--r--   0        0        0     5632 2023-05-16 06:59:25.289918 pyaedt-0.6.80/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
+-rw-r--r--   0        0        0   160754 2023-05-16 06:59:25.305543 pyaedt-0.6.80/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
+-rw-r--r--   0        0        0    23386 2023-05-25 10:01:32.202746 pyaedt-0.6.80/pyaedt/downloads.py
+-rw-r--r--   0        0        0   136802 2023-06-05 14:38:07.282707 pyaedt-0.6.80/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-05-16 06:59:25.305543 pyaedt-0.6.80/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    92242 2023-06-05 13:38:36.375818 pyaedt-0.6.80/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-06-05 13:38:36.375818 pyaedt-0.6.80/pyaedt/edb_core/dotnet/__init__.py
+-rw-r--r--   0        0        0    31497 2023-06-05 13:38:36.375818 pyaedt-0.6.80/pyaedt/edb_core/dotnet/database.py
+-rw-r--r--   0        0        0     7909 2023-06-05 13:38:36.375818 pyaedt-0.6.80/pyaedt/edb_core/dotnet/layout.py
+-rw-r--r--   0        0        0    48210 2023-06-05 13:38:36.375818 pyaedt-0.6.80/pyaedt/edb_core/dotnet/primitive.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.305543 pyaedt-0.6.80/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    33195 2023-06-12 08:03:23.732504 pyaedt-0.6.80/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0    40100 2023-05-29 06:50:09.600210 pyaedt-0.6.80/pyaedt/edb_core/edb_data/control_file.py
+-rw-r--r--   0        0        0      937 2023-05-16 06:59:25.305543 pyaedt-0.6.80/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      867 2023-05-25 15:57:26.266409 pyaedt-0.6.80/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    12243 2023-06-05 13:38:36.375818 pyaedt-0.6.80/pyaedt/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    65661 2023-06-05 13:38:36.375818 pyaedt-0.6.80/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20386 2023-06-05 13:38:36.375818 pyaedt-0.6.80/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     6441 2023-06-12 08:03:23.732504 pyaedt-0.6.80/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    61171 2023-06-05 13:38:36.391420 pyaedt-0.6.80/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    33851 2023-06-05 18:49:47.519772 pyaedt-0.6.80/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0   101786 2023-06-05 13:38:36.391420 pyaedt-0.6.80/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36324 2023-06-05 13:38:36.391420 pyaedt-0.6.80/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    34198 2023-06-12 08:03:23.732504 pyaedt-0.6.80/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     3923 2023-06-05 15:20:28.578156 pyaedt-0.6.80/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2432 2023-06-05 13:38:36.391420 pyaedt-0.6.80/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     3258 2023-05-16 06:59:25.321165 pyaedt-0.6.80/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    66975 2023-06-05 13:38:36.391420 pyaedt-0.6.80/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.321165 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.321165 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-16 06:59:25.321165 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-05-16 06:59:25.321165 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-05-16 06:59:25.321165 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-05-16 06:59:25.321165 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.321165 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-05-16 06:59:25.321165 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-05-16 06:59:25.321165 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-05-16 06:59:25.321165 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2850 2023-06-05 13:38:36.391420 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7763 2023-05-29 06:50:09.615842 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4703 2023-05-29 06:50:09.615842 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-05-16 06:59:25.336792 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-05-16 06:59:25.352417 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-05-16 06:59:25.352417 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-05-16 06:59:25.352417 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-05-16 06:59:25.352417 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-05-16 06:59:25.352417 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-05-16 06:59:25.352417 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-05-16 06:59:25.352417 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-05-16 06:59:25.352417 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11390 2023-05-29 06:50:09.615842 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-05-16 06:59:25.352417 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-05-16 06:59:25.352417 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-05-16 06:59:25.352417 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-05-16 06:59:25.352417 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21800 2023-06-05 13:38:36.391420 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-05-16 06:59:25.352417 pyaedt-0.6.80/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    47125 2023-06-05 15:20:28.578156 pyaedt-0.6.80/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33310 2023-06-05 13:38:36.391420 pyaedt-0.6.80/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0    44030 2023-06-05 15:20:28.578156 pyaedt-0.6.80/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    47600 2023-06-05 13:38:36.407042 pyaedt-0.6.80/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    57581 2023-06-12 08:03:23.732504 pyaedt-0.6.80/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   109207 2023-06-05 13:38:36.407042 pyaedt-0.6.80/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    11363 2023-06-13 07:50:22.368204 pyaedt-0.6.80/pyaedt/emit.py
+-rw-r--r--   0        0        0     3555 2023-05-16 06:59:25.368043 pyaedt-0.6.80/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3291 2023-06-13 07:50:22.368204 pyaedt-0.6.80/pyaedt/emit_core/EmitConstants.py
+-rw-r--r--   0        0        0     1091 2023-06-13 07:50:22.368204 pyaedt-0.6.80/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0        2 2023-05-16 06:59:25.368043 pyaedt-0.6.80/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-05-19 04:27:23.959058 pyaedt-0.6.80/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    13338 2023-06-13 07:50:22.368204 pyaedt-0.6.80/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-05-16 06:59:25.368043 pyaedt-0.6.80/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    11758 2023-05-16 06:59:25.368043 pyaedt-0.6.80/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.368043 pyaedt-0.6.80/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3257 2023-05-26 11:30:36.599404 pyaedt-0.6.80/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83444 2023-05-29 06:50:09.647120 pyaedt-0.6.80/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-05-16 06:59:25.383677 pyaedt-0.6.80/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    21891 2023-05-24 15:53:22.126810 pyaedt-0.6.80/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3395 2023-05-19 12:41:48.802021 pyaedt-0.6.80/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    69591 2023-05-29 06:50:09.647120 pyaedt-0.6.80/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0    25808 2023-05-16 06:59:25.383677 pyaedt-0.6.80/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     6989 2023-05-16 06:59:25.383677 pyaedt-0.6.80/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0     9795 2023-05-16 06:59:25.383677 pyaedt-0.6.80/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    62327 2023-05-29 06:50:09.647120 pyaedt-0.6.80/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11301 2023-05-16 06:59:25.383677 pyaedt-0.6.80/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    20326 2023-05-16 06:59:25.383677 pyaedt-0.6.80/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3466 2023-05-16 06:59:25.383677 pyaedt-0.6.80/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60412 2023-05-29 06:50:09.647120 pyaedt-0.6.80/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17095 2023-05-16 06:59:25.383677 pyaedt-0.6.80/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-05-16 06:59:25.383677 pyaedt-0.6.80/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   253082 2023-06-05 09:41:19.525305 pyaedt-0.6.80/pyaedt/hfss.py
+-rw-r--r--   0        0        0    82916 2023-05-16 06:59:25.383677 pyaedt-0.6.80/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   168417 2023-06-13 10:43:12.615480 pyaedt-0.6.80/pyaedt/icepak.py
+-rw-r--r--   0        0        0   118479 2023-05-29 06:50:09.662736 pyaedt-0.6.80/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7803 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24316 2023-05-29 06:50:09.662736 pyaedt-0.6.80/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3695 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     2380 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10210 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     3731 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     3818 2023-05-19 12:41:48.802021 pyaedt-0.6.80/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-05-16 06:59:25.399290 pyaedt-0.6.80/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-05-16 06:59:25.414915 pyaedt-0.6.80/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-05-16 06:59:25.414915 pyaedt-0.6.80/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-05-16 06:59:25.414915 pyaedt-0.6.80/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-05-16 06:59:25.414915 pyaedt-0.6.80/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-05-16 06:59:25.414915 pyaedt-0.6.80/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-05-16 06:59:25.414915 pyaedt-0.6.80/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-05-16 06:59:25.414915 pyaedt-0.6.80/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-05-16 06:59:25.430540 pyaedt-0.6.80/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-05-16 06:59:25.430540 pyaedt-0.6.80/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.430540 pyaedt-0.6.80/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.430540 pyaedt-0.6.80/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14107 2023-05-29 06:50:09.662736 pyaedt-0.6.80/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    20051 2023-05-29 06:50:09.662736 pyaedt-0.6.80/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-05-16 06:59:25.430540 pyaedt-0.6.80/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16840 2023-05-29 06:50:09.662736 pyaedt-0.6.80/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120888 2023-05-29 06:50:09.662736 pyaedt-0.6.80/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   198210 2023-06-12 22:10:56.369219 pyaedt-0.6.80/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   116607 2023-05-29 06:50:09.662736 pyaedt-0.6.80/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11387 2023-05-29 06:50:09.662736 pyaedt-0.6.80/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   127857 2023-06-12 22:10:56.369219 pyaedt-0.6.80/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.430540 pyaedt-0.6.80/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    31589 2023-05-29 06:50:09.662736 pyaedt-0.6.80/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49057 2023-05-29 06:50:09.662736 pyaedt-0.6.80/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59078 2023-05-29 06:50:09.678333 pyaedt-0.6.80/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53131 2023-05-29 06:50:09.678333 pyaedt-0.6.80/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12645 2023-05-29 06:50:09.678333 pyaedt-0.6.80/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    42629 2023-05-29 06:50:09.678333 pyaedt-0.6.80/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    32780 2023-06-13 07:50:22.368204 pyaedt-0.6.80/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8212 2023-05-29 06:50:09.678333 pyaedt-0.6.80/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    63100 2023-05-29 06:50:09.678333 pyaedt-0.6.80/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15149 2023-05-29 06:50:09.678333 pyaedt-0.6.80/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.446165 pyaedt-0.6.80/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    32013 2023-05-29 06:50:09.678333 pyaedt-0.6.80/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68135 2023-05-19 10:14:06.395089 pyaedt-0.6.80/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6952 2023-05-29 06:50:09.678333 pyaedt-0.6.80/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    59936 2023-05-30 06:01:48.466176 pyaedt-0.6.80/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    32822 2023-06-12 22:10:56.369219 pyaedt-0.6.80/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    49892 2023-05-29 06:50:09.678333 pyaedt-0.6.80/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.446165 pyaedt-0.6.80/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65639 2023-05-29 06:50:09.693947 pyaedt-0.6.80/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    23689 2023-05-29 06:50:09.693947 pyaedt-0.6.80/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    30094 2023-05-16 06:59:25.461791 pyaedt-0.6.80/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   114715 2023-06-13 10:43:12.615480 pyaedt-0.6.80/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71549 2023-05-16 06:59:25.461791 pyaedt-0.6.80/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-05-16 06:59:25.461791 pyaedt-0.6.80/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51967 2023-05-29 06:50:09.693947 pyaedt-0.6.80/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40465 2023-05-29 06:50:09.693947 pyaedt-0.6.80/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82903 2023-05-29 06:50:09.693947 pyaedt-0.6.80/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28363 2023-05-29 06:50:09.693947 pyaedt-0.6.80/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53226 2023-05-29 06:50:09.693947 pyaedt-0.6.80/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11976 2023-05-29 06:50:09.693947 pyaedt-0.6.80/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    26105 2023-05-29 06:50:09.693947 pyaedt-0.6.80/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-05-16 06:59:25.461791 pyaedt-0.6.80/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   177029 2023-06-12 08:03:23.748124 pyaedt-0.6.80/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64104 2023-05-16 06:59:25.477419 pyaedt-0.6.80/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   121091 2023-06-12 22:10:56.384864 pyaedt-0.6.80/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33257 2023-05-29 06:50:09.709572 pyaedt-0.6.80/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.477419 pyaedt-0.6.80/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    28709 2023-05-29 06:50:09.709572 pyaedt-0.6.80/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103333 2023-05-29 06:50:09.709572 pyaedt-0.6.80/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   125079 2023-05-29 06:50:09.709572 pyaedt-0.6.80/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95908 2023-05-29 06:50:09.709572 pyaedt-0.6.80/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10581 2023-05-29 06:50:09.709572 pyaedt-0.6.80/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.477419 pyaedt-0.6.80/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-05-16 06:59:25.477419 pyaedt-0.6.80/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-05-16 06:59:25.477419 pyaedt-0.6.80/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.477419 pyaedt-0.6.80/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-05-16 06:59:25.477419 pyaedt-0.6.80/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-05-16 06:59:25.477419 pyaedt-0.6.80/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-05-16 06:59:25.477419 pyaedt-0.6.80/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-05-16 06:59:25.477419 pyaedt-0.6.80/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-05-16 06:59:25.477419 pyaedt-0.6.80/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-05-16 06:59:25.493150 pyaedt-0.6.80/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-05-16 06:59:25.493150 pyaedt-0.6.80/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-05-16 06:59:25.493150 pyaedt-0.6.80/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-05-16 06:59:25.493150 pyaedt-0.6.80/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-05-16 06:59:25.493150 pyaedt-0.6.80/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-05-16 06:59:25.493150 pyaedt-0.6.80/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-05-16 06:59:25.493150 pyaedt-0.6.80/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-05-16 06:59:25.493150 pyaedt-0.6.80/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-05-16 06:59:25.493150 pyaedt-0.6.80/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-05-16 06:59:25.493150 pyaedt-0.6.80/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-05-16 06:59:25.493150 pyaedt-0.6.80/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7632 2023-05-29 06:50:09.709572 pyaedt-0.6.80/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10410 2023-06-05 13:38:36.407042 pyaedt-0.6.80/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-05-16 06:59:25.493150 pyaedt-0.6.80/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4410 2023-06-13 13:22:33.125021 pyaedt-0.6.80/pyproject.toml
+-rw-r--r--   0        0        0    15552 1970-01-01 00:00:00.000000 pyaedt-0.6.80/PKG-INFO
```

### Comparing `pyaedt-0.6.79/LICENSE` & `pyaedt-0.6.80/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/README.md` & `pyaedt-0.6.80/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/__init__.py` & `pyaedt-0.6.80/pyaedt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.79"
+__version__ = "0.6.80"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
```

### Comparing `pyaedt-0.6.79/pyaedt/aedt_logger.py` & `pyaedt-0.6.80/pyaedt/aedt_logger.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.80/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/application/Analysis.py` & `pyaedt-0.6.80/pyaedt/application/Analysis.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.80/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.80/pyaedt/application/Analysis3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.80/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.80/pyaedt/application/AnalysisNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.80/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.80/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/application/Design.py` & `pyaedt-0.6.80/pyaedt/application/Design.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/application/JobManager.py` & `pyaedt-0.6.80/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/application/Variables.py` & `pyaedt-0.6.80/pyaedt/application/Variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.80/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/application/design_solutions.py` & `pyaedt-0.6.80/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/circuit.py` & `pyaedt-0.6.80/pyaedt/circuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/common_rpc.py` & `pyaedt-0.6.80/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/desktop.py` & `pyaedt-0.6.80/pyaedt/desktop.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/AnsysReport.deps.json` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/AnsysReport.deps.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/Images/Ansys.png` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/Images/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/PdfSharpCore.dll` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/PdfSharpCore.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/System.Runtime.dll` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/System.Runtime.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/System.Runtime.xml` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/System.Runtime.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml` & `pyaedt-0.6.80/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/downloads.py` & `pyaedt-0.6.80/pyaedt/downloads.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb.py` & `pyaedt-0.6.80/pyaedt/edb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/components.py` & `pyaedt-0.6.80/pyaedt/edb_core/components.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/dotnet/database.py` & `pyaedt-0.6.80/pyaedt/edb_core/dotnet/database.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/dotnet/layout.py` & `pyaedt-0.6.80/pyaedt/edb_core/dotnet/layout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/dotnet/primitive.py` & `pyaedt-0.6.80/pyaedt/edb_core/dotnet/primitive.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/components_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,15 +389,15 @@
         -------
         bool
             ``True`` if current object is enabled, ``False`` otherwise.
         """
         if self.type in ["Resistor", "Capacitor", "Inductor"]:
             return self.component_property.IsEnabled()
         else:  # pragma: no cover
-            return False
+            return True
 
     @is_enabled.setter
     def is_enabled(self, enabled):
         """Enables the current object."""
         if self.type in ["Resistor", "Capacitor", "Inductor"]:
             component_property = self.component_property
             component_property.SetEnabled(enabled)
@@ -440,16 +440,24 @@
         """Retrieve discrete component value.
 
         Returns
         -------
         str
             Value. ``None`` if not an RLC Type.
         """
-        if self.model_type == "RLC" and self._pin_pairs:
-            pin_pair = self._pin_pairs[0]
+        if self.model_type == "RLC":
+            if not self._pin_pairs:
+                if self.type == "Inductor":
+                    return 1e-9
+                elif self.type == "Resistor":
+                    return 1e6
+                else:
+                    return 1
+            else:
+                pin_pair = self._pin_pairs[0]
             if len([i for i in pin_pair.rlc_enable if i]) == 1:
                 return [pin_pair.rlc_values[idx] for idx, val in enumerate(pin_pair.rlc_enable) if val][0]
             else:
                 return pin_pair.rlc_values
         elif self.model_type == "SPICEModel":
             return self.spice_model.file_path
         elif self.model_type == "SParameterModel":
```

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/control_file.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/control_file.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/hfss_extent_info.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/hfss_extent_info.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/nets_data.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/nets_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -119,7 +119,65 @@
         current_value = 1e10
         for prim in self.net_object.Primitives:
             if "GetWidth" in dir(prim):
                 width = prim.GetWidth()
                 if width < current_value:
                     current_value = width
         return current_value
+
+    @pyaedt_function_handler
+    def get_extended_net(self, resistor_below=10, inductor_below=1, capacitor_above=1):
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
+        Returns
+        -------
+        list[
+            dict[str, :class: `pyaedt.edb_core.edb_data.nets_data.EDBNetsData`],
+            dict[str, :class: `pyaedt.edb_core.edb_data.components_data.EDBComponent`],
+            dict[str, :class: `pyaedt.edb_core.edb_data.components_data.EDBComponent`],
+            ]
+        Examples
+        --------
+        >>> from pyaedt import Edb
+        >>> app = Edb()
+        >>> app.nets["BST_V3P3_S5"].get_extended_net()
+        """
+        all_nets = self._app.nets.nets
+        nets = {}
+        rlc_serial = {}
+        comps = {}
+
+        def get_net_list(net_name, _net_list, _rlc_serial, _comp):
+            edb_net = all_nets[net_name]
+            for refdes, val in edb_net.components.items():
+                if not val.is_enabled:
+                    continue
+
+                if val.type == "Inductor" and val.value < inductor_below and val.is_enabled:
+                    pass
+                elif val.type == "Resistor" and val.value < resistor_below and val.is_enabled:
+                    pass
+                elif val.type == "Capacitor" and val.value > capacitor_above and val.is_enabled:
+                    pass
+                else:
+                    _comp[refdes] = val
+                    continue
+
+                _rlc_serial[refdes] = val
+                for net in val.nets:
+                    if net not in _net_list:
+                        _net_list[net] = all_nets[net]
+                        get_net_list(net, _net_list, _rlc_serial, _comp)
+
+        get_net_list(self.name, nets, rlc_serial, comps)
+
+        return [nets, rlc_serial, comps]
```

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,19 +302,20 @@
         terminal = self._create_terminal()
         terminal.SetBoundaryType(self._pedb.edb_api.cell.terminal.BoundaryType.kCurrentSource)
         terminal.SetSourceAmplitude(self._pedb.edb_value(magnitude))
         terminal.SetSourcePhase(self._pedb.edb_api.utility.value(phase))
         return terminal
 
     @pyaedt_function_handler()
-    def create_voltage_source_terminal(self, magnitude=1, phase=0):
+    def create_voltage_source_terminal(self, magnitude=1, phase=0, impedance=0.001):
         terminal = self._create_terminal()
         terminal.SetBoundaryType(self._pedb.edb_api.cell.terminal.BoundaryType.kVoltageSource)
         terminal.SetSourceAmplitude(self._pedb.edb_value(magnitude))
         terminal.SetSourcePhase(self._pedb.edb_api.utility.value(phase))
+        terminal.SetImpedance(self._pedb.edb_value(impedance))
         return terminal
 
     @pyaedt_function_handler()
     def create_port_terminal(self, impedance=50):
         terminal = self._create_terminal()
         terminal.SetBoundaryType(self._pedb.edb_api.cell.terminal.BoundaryType.PortBoundary)
         terminal.SetImpedance(self._pedb.edb_value(impedance))
@@ -539,14 +540,23 @@
         Returns
         -------
         int
         """
         return self._edb_terminal.GetBoundaryType()
 
     @property
+    def impedance(self):
+        """Impedance of the port."""
+        return self._edb_terminal.GetImpedance().ToDouble()
+
+    @impedance.setter
+    def impedance(self, value):
+        self._edb_terminal.SetImpedance(self._pedb.edb_value(value))
+
+    @property
     def reference_object(self):
         """This returns the object assigned as reference. It can be a primitive or a padstack instance.
 
 
         Returns
         -------
         :class:`pyaedt.edb_core.edb_data.padstacks_data.EDBPadstackInstance` or
```

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/edb_data/variables.py` & `pyaedt-0.6.80/pyaedt/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/general.py` & `pyaedt-0.6.80/pyaedt/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.80/pyaedt/edb_core/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.80/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/layout.py` & `pyaedt-0.6.80/pyaedt/edb_core/layout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/materials.py` & `pyaedt-0.6.80/pyaedt/edb_core/materials.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/nets.py` & `pyaedt-0.6.80/pyaedt/edb_core/nets.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.80/pyaedt/edb_core/padstack.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.80/pyaedt/edb_core/siwave.py`

 * *Files 0% similar despite different names*

```diff
@@ -1258,15 +1258,15 @@
         neg_terminal = neg_pin_group_name.create_current_source_terminal()
         neg_terminal.SetName(name + "_ref")
         pos_terminal.SetReferenceTerminal(neg_terminal)
         return True
 
     @pyaedt_function_handler
     def create_voltage_source_on_pin_group(
-        self, pos_pin_group_name, neg_pin_group_name, magnitude=1, phase=0, name=None
+        self, pos_pin_group_name, neg_pin_group_name, magnitude=1, phase=0, name=None, impedance=0.001
     ):
         """Create voltage source between two pin groups.
 
         Parameters
         ----------
         pos_pin_group_name : str
             Name of the positive pin group.
@@ -1279,15 +1279,15 @@
 
         Returns
         -------
         bool
 
         """
         pos_pin_group = self.pin_groups[pos_pin_group_name]
-        pos_terminal = pos_pin_group.create_voltage_source_terminal(magnitude, phase)
+        pos_terminal = pos_pin_group.create_voltage_source_terminal(magnitude, phase, impedance)
         if name:
             pos_terminal.SetName(name)
         else:
             name = generate_unique_name("vsource")
             pos_terminal.SetName(name)
         neg_pin_group_name = self.pin_groups[neg_pin_group_name]
         neg_terminal = neg_pin_group_name.create_voltage_source_terminal(magnitude, phase)
```

### Comparing `pyaedt-0.6.79/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.80/pyaedt/edb_core/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/emit.py` & `pyaedt-0.6.80/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/emit_core/Couplings.py` & `pyaedt-0.6.80/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/emit_core/EmitConstants.py` & `pyaedt-0.6.80/pyaedt/emit_core/EmitConstants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/emit_core/__init__.py` & `pyaedt-0.6.80/pyaedt/emit_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.80/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/emit_core/results/revision.py` & `pyaedt-0.6.80/pyaedt/emit_core/results/revision.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.80/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.80/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/clr_module.py` & `pyaedt-0.6.80/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/configurations.py` & `pyaedt-0.6.80/pyaedt/generic/configurations.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/constants.py` & `pyaedt-0.6.80/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/design_types.py` & `pyaedt-0.6.80/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/filesystem.py` & `pyaedt-0.6.80/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/general_methods.py` & `pyaedt-0.6.80/pyaedt/generic/general_methods.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.80/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.80/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/pdf.py` & `pyaedt-0.6.80/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/plot.py` & `pyaedt-0.6.80/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/process.py` & `pyaedt-0.6.80/pyaedt/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.80/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.80/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/toolkit.py` & `pyaedt-0.6.80/pyaedt/generic/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.80/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/hfss.py` & `pyaedt-0.6.80/pyaedt/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.80/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/icepak.py` & `pyaedt-0.6.80/pyaedt/icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/maxwell.py` & `pyaedt-0.6.80/pyaedt/maxwell.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.80/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/mechanical.py` & `pyaedt-0.6.80/pyaedt/mechanical.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/Console.py_build` & `pyaedt-0.6.80/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.80/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.80/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.80/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.80/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.80/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/amat.xml` & `pyaedt-0.6.80/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/console_setup.py` & `pyaedt-0.6.80/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.80/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.80/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.80/pyaedt/misc/install_extra_toolkits.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.80/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/misc.py` & `pyaedt-0.6.80/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.80/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.80/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.80/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.80/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.80/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.80/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/misc/template.acf` & `pyaedt-0.6.80/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.80/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.80/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.80/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.80/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.80/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.80/pyaedt/modeler/cad/Modeler.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,20 +227,31 @@
         Id of the face where the Face Coordinate System is laying.
 
     """
 
     def __init__(self, modeler, props=None, name=None, face_id=None):
         BaseCoordinateSystem.__init__(self, modeler, name)
         self.face_id = face_id
-        self.props = CsProps(self, props)
-        try:  # pragma: no cover
-            if "KernelVersion" in self.props:
-                del self.props["KernelVersion"]
-        except:
-            pass
+        self._props = None
+        if props:
+            self._props = CsProps(self, props)
+            try:  # pragma: no cover
+                if "KernelVersion" in self.props:
+                    del self.props["KernelVersion"]
+            except:
+                pass
+
+    def props(self):
+        """Coordinate System Properties.
+
+        Returns
+        -------
+        :class:`pyaedt.modeler.Modeler.CSProps`
+        """
+        return self._props
 
     @property
     def _part_name(self):
         """Internally get the part name which the face belongs to"""
         if not self.face_id:
             # face_id has not been defined yet
             return None
@@ -396,15 +407,15 @@
         parameters["ZRotationAngle"] = str(rotation) + "deg"
         parameters["XOffset"] = self._dim_arg((offset[0]), self.model_units)
         parameters["YOffset"] = self._dim_arg((offset[1]), self.model_units)
         parameters["AutoAxis"] = False
 
         self.props = CsProps(self, parameters)
         self._modeler.oeditor.CreateFaceCS(self._face_paramenters, self._attributes)
-        self._modeler.coordinate_systems.insert(0, self)
+        self._modeler._coordinate_systems.insert(0, self)
         return True
 
     @pyaedt_function_handler()
     def _get_type_from_id(self, obj_id):
         """Get the entity type from the id"""
         for obj in self._modeler.objects.values():
             if obj.id == obj_id:
@@ -483,23 +494,102 @@
         The default is ``None``.
 
     """
 
     def __init__(self, modeler, props=None, name=None):
         BaseCoordinateSystem.__init__(self, modeler, name)
         self.model_units = self._modeler.model_units
-        self.props = CsProps(self, props)
-        self.ref_cs = None
+        self._props = None
+        if props:
+            self._props = CsProps(self, props)
+            try:  # pragma: no cover
+                if "KernelVersion" in self.props:
+                    del self.props["KernelVersion"]
+            except:
+                pass
+        self._ref_cs = None
         self._quaternion = None
-        self.mode = None
-        try:  # pragma: no cover
-            if "KernelVersion" in self.props:
-                del self.props["KernelVersion"]
+        self._mode = None
+
+    @property
+    def mode(self):
+        """Coordinate System mode."""
+        if self._mode:
+            return self._mode
+        if "Axis" in self.props.get("Mode", ""):
+            self._mode = "axis"
+        elif "ZXZ" in self.props.get("Mode", ""):
+            self._mode = "zxz"
+        elif "ZYZ" in self.props.get("Mode", ""):
+            self._mode == "zyz"
+        return self._mode
+
+    @mode.setter
+    def mode(self, value):
+        self._mode = value
+
+    @property
+    def props(self):
+        """Coordinate System Properties.
+
+        Returns
+        -------
+        :class:`pyaedt.modeler.Modeler.CSProps`
+        """
+        if self._props or settings.aedt_version <= "2022.2" or self.name is None:
+            return self._props
+        obj1 = self._modeler.oeditor.GetChildObject(self.name)
+        props = {}
+        origin = obj1.GetPropValue("Origin")
+        props["OriginX"] = origin[1]
+        props["OriginY"] = origin[3]
+        props["OriginZ"] = origin[5]
+        axisvec = obj1.GetPropValue("X Axis")
+        props["Mode"] = obj1.GetPropValue("Mode")
+        if props["Mode"] == "Axis/Position":
+            props["XAxisXvec"] = axisvec[1]
+            props["XAxisYvec"] = axisvec[3]
+            props["XAxisZvec"] = axisvec[5]
+            ypoint = obj1.GetPropValue("Y Point")
+
+            props["YAxisXvec"] = ypoint[1]
+            props["YAxisYvec"] = ypoint[3]
+            props["YAxisZvec"] = ypoint[5]
+        else:
+            props["Phi"] = obj1.GetPropValue("Phi")
+            props["Theta"] = obj1.GetPropValue("Theta")
+            props["Psi"] = obj1.GetPropValue("Psi")
+        self._props = CsProps(self, props)
+        return self._props
+
+    @property
+    def ref_cs(self):
+        """Reference coordinate system getter and setter.
+
+        Returns
+        -------
+        str
+        """
+        if self._ref_cs or settings.aedt_version <= "2022.2":
+            return self._ref_cs
+        obj1 = self._modeler.oeditor.GetChildObject(self.name)
+        self._ref_cs = obj1.GetPropValue("Reference CS")
+        return self._ref_cs
+
+    @ref_cs.setter
+    def ref_cs(self, value):
+        if settings.aedt_version <= "2022.2":
+            self._ref_cs = value
+            self.update()
+        obj1 = self._modeler.oeditor.GetChildObject(self.name)
+        try:
+            obj1.SetPropValue("Reference CS", value)
+            self._ref_cs = value
         except:
-            pass
+            self._modeler.logger.error("Failed to set Coordinate CS Reference.")
 
     @pyaedt_function_handler()
     def update(self):
         """Update the coordinate system.
 
         Returns
         -------
@@ -830,19 +920,19 @@
             orientationParameters["Mode"] = "Euler Angle ZYZ"
             orientationParameters["Phi"] = self._dim_arg(phi, "deg")
             orientationParameters["Theta"] = self._dim_arg(theta, "deg")
             orientationParameters["Psi"] = self._dim_arg(psi, "deg")
         else:  # pragma: no cover
             raise ValueError("Specify the mode = 'view', 'axis', 'zxz', 'zyz', 'axisrotation' ")
 
-        self.props = CsProps(self, orientationParameters)
+        self._props = CsProps(self, orientationParameters)
         self._modeler.oeditor.CreateRelativeCS(self._orientation, self._attributes)
-        self._modeler.coordinate_systems.insert(0, self)
+        self._modeler._coordinate_systems.insert(0, self)
         # this workaround is necessary because the reference CS is ignored at creation, it needs to be modified later
-        self.ref_cs = reference_cs
+        self._ref_cs = reference_cs
         return self.update()
 
     @property
     def quaternion(self):
         """Quaternion computed based on specific axis mode.
 
         Returns
@@ -1175,32 +1265,40 @@
 
     def __init__(self, app, is3d=True):
         self._app = app
         self._odefinition_manager = self._app.odefinition_manager
         self._omaterial_manager = self._app.omaterial_manager
         Modeler.__init__(self, app)
         # TODO Refactor this as a dictionary with names as key
-        self._coordinate_systems = None
-        self._user_lists = None
-        self._planes = None
+        self._coordinate_systems = []
+        self._user_lists = []
+        self._planes = []
         self._is3d = is3d
         self._solids = []
         self._sheets = []
         self._lines = []
         self._points = []
         self._unclassified = []
         self._all_object_names = []
         self.objects = {}
         self.user_defined_components = {}
         self._object_names_to_ids = {}
 
     @property
     def coordinate_systems(self):
         """Coordinate Systems."""
-        if self._coordinate_systems is None:
+        if settings.aedt_version > "2022.2":
+            cs_names = [i for i in self.oeditor.GetChildNames("CoordinateSystems") if i != "Global"]
+            for cs_name in cs_names:
+                props = {}
+                local_names = [i.name for i in self._coordinate_systems]
+                if cs_name not in local_names:
+                    self._coordinate_systems.append(CoordinateSystem(self, props, cs_name))
+            return self._coordinate_systems
+        if not self._coordinate_systems:
             self._coordinate_systems = self._get_coordinates_data()
         return self._coordinate_systems
 
     @property
     def user_lists(self):
         """User Lists."""
         if not self._user_lists:
@@ -1343,15 +1441,15 @@
                                                     coord.append(FaceCoordinateSystem(self, props, name))
                                                     break
                 except:
                     pass
             for cs in coord:
                 if isinstance(cs, CoordinateSystem):
                     try:
-                        cs.ref_cs = id2name[name2refid[cs.name]]
+                        cs._ref_cs = id2name[name2refid[cs.name]]
                     except:
                         pass
         coord.reverse()
         return coord
 
     def _get_lists_data(self):
         """Retrieve user object list data.
@@ -3391,62 +3489,64 @@
         >>> oEditor.GetModelBoundingBox
         """
         bb = list(self.oeditor.GetModelBoundingBox())
         bound = [float(b) for b in bb]
         return bound
 
     @pyaedt_function_handler()
-    def unite(self, theList, purge=False):
+    def unite(self, unite_list, purge=False, keep_originals=False):
         """Unite objects from a list.
 
         Parameters
         ----------
-        theList : list
+        unite_list : list
             List of objects.
         purge : bool, optional
-            Purge history after unite.
+            Purge history after unite. Default is False.
+        keep_originals : bool, optional
+            Keep original objects used for the operation. Default is False.
 
         Returns
         -------
         str
             The united object that is the first in the list.
 
         References
         ----------
 
         >>> oEditor.Unite
         """
-        slice = min(100, len(theList))
-        num_objects = len(theList)
+        slice = min(100, len(unite_list))
+        num_objects = len(unite_list)
         remaining = num_objects
         objs_groups = []
         while remaining > 1:
-            objs = theList[:slice]
+            objs = unite_list[:slice]
             szSelections = self.convert_to_selections(objs)
             vArg1 = ["NAME:Selections", "Selections:=", szSelections]
-            vArg2 = ["NAME:UniteParameters", "KeepOriginals:=", False]
+            vArg2 = ["NAME:UniteParameters", "KeepOriginals:=", keep_originals]
             self.oeditor.Unite(vArg1, vArg2)
             if szSelections.split(",")[0] in self.unclassified_names:
                 self.logger.error("Error in uniting objects.")
                 self._odesign.Undo()
                 self.cleanup_objects()
                 return False
             elif purge:
                 self.purge_history(objs[0])
             objs_groups.append(objs[0])
             remaining -= slice
             if remaining > 0:
-                theList = theList[slice:]
+                unite_list = unite_list[slice:]
         if remaining > 0:
-            objs_groups.extend(theList)
+            objs_groups.extend(unite_list)
         self.cleanup_objects()
         if len(objs_groups) > 1:
             return self.unite(objs_groups, purge=purge)
         self.logger.info("Union of {} objects has been executed.".format(num_objects))
-        return self.convert_to_selections(theList[0], False)
+        return self.convert_to_selections(unite_list[0], False)
 
     @pyaedt_function_handler()
     def clone(self, objid):
         """Clone objects from a list of object IDs.
 
         Parameters
         ----------
```

### Comparing `pyaedt-0.6.79/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.80/pyaedt/modeler/cad/Primitives.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.80/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.80/pyaedt/modeler/cad/Primitives3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1319,15 +1319,14 @@
                     self._app.modeler.refresh_all_ids()
                     for udm in set(list(self._app.modeler.user_defined_components)) - old_udm:
                         if self._app.modeler.user_defined_components[udm].target_coordinate_system == "Global":
                             self._app.modeler.user_defined_components[udm].target_coordinate_system = targetCS
                 for cs in set(self._app.modeler.coordinate_systems) - old_cs:
                     if cs.ref_cs == "Global":
                         cs.ref_cs = targetCS
-                        cs.update()
             if aux_dict.get("monitor", None):
                 temp_proj_name = self._app._generate_unique_project_name()
                 ipkapp_temp = Icepak(projectname=os.path.join(self._app.toolkit_directory, temp_proj_name))
                 ipkapp_temp.delete_design(ipkapp_temp.design_name)
                 self._app.oproject.CopyDesign(self._app.design_name)
                 ipkapp_temp.oproject.Paste()
                 temp_proj = ipkapp_temp.project_file
```

### Comparing `pyaedt-0.6.79/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.80/pyaedt/modeler/cad/components_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.80/pyaedt/modeler/cad/elements3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.80/pyaedt/modeler/cad/object3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.80/pyaedt/modeler/cad/polylines.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/calculators.py` & `pyaedt-0.6.80/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.80/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.80/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.80/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.6.80/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.80/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.80/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.80/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.80/pyaedt/modeler/modeler2d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.80/pyaedt/modeler/modeler3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.80/pyaedt/modeler/modelerpcb.py`

 * *Files 1% similar despite different names*

```diff
@@ -960,7 +960,52 @@
         naming convention: "VCP_xxx".
 
         Returns
         -------
         list
         """
         return [i for i in self.oeditor.FindObjects("Name", "VCP*")]
+
+    @pyaedt_function_handler()
+    def geometry_check_and_fix_all(
+        self,
+        min_area=2e-6,
+    ):
+        """Run Geometry Check.
+
+        All checks are used and all auto fix options are enabled.
+
+        min_area : float, optional
+            CutOuts that are smaller than this minimum area will be ignored during validation checks.
+            The default is ``2e-6``.
+
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
+        """
+        try:
+            self.oeditor.GeometryCheckAndAutofix(
+                [
+                    "NAME:checks",
+                    "Self-Intersecting Polygons",
+                    "Disjoint Nets (Floating Nodes)",
+                    "DC-Short Errors",
+                    "Identical/Overlapping Vias",
+                    "Misaligments",
+                ],
+                "minimum_area_meters_squared:=",
+                min_area,
+                [
+                    "NAME:fixes",
+                    "Self-Intersecting Polygons",
+                    "Disjoint Nets",
+                    "Identical/Overlapping Vias",
+                    "Traces-Inside-Traces Errors",
+                    "Misalignments (Planes/Traces/Vias)",
+                ],
+            )
+            self.logger.info("Geometry check succeed")
+            return True
+        except:
+            self.logger.error("Geometry check Failed.")
+            return False
```

### Comparing `pyaedt-0.6.79/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.80/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.80/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modeler/schematic.py` & `pyaedt-0.6.80/pyaedt/modeler/schematic.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.80/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/Boundary.py` & `pyaedt-0.6.80/pyaedt/modules/Boundary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.80/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.80/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.80/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.80/pyaedt/modules/LayerStackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/Material.py` & `pyaedt-0.6.80/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.80/pyaedt/modules/MaterialLib.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/Mesh.py` & `pyaedt-0.6.80/pyaedt/modules/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.80/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.80/pyaedt/modules/MeshIcepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.80/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.80/pyaedt/modules/PostProcessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3342,36 +3342,50 @@
         if plot:
             file_to_add = self.export_field_plot(plot.name, project_path)
             plot.delete()
             return file_to_add
         return None
 
     @pyaedt_function_handler()
-    def power_budget(self, units="W", temperature=22):
+    def power_budget(self, units="W", temperature=22, output_type="component"):
         """Power budget calculation.
 
         Parameters
         ----------
         units : str, optional
             Output power units. The default is ``"W"``.
         temperature : float, optional
             Temperature to calculate the power. The default is ``22``.
+        output_type : str, optional
+            Output data presentation. The default is ``"component"``.
+            The options are ``"component"``, or ``"boundary"``.
+            ``"component"`` will return the power based on each component.
+            ``"boundary"`` will return the power based on each boundary.
 
         Returns
         -------
         dict, float
             Dictionary with the power introduced on each boundary and total power.
 
         References
         ----------
 
         >>> oEditor.ChangeProperty
         """
         available_bcs = self._app.boundaries
         power_dict = {}
+        power_dict_obj = {}
+        group_hierarchy = {}
+
+        groups = self._app.oeditor.GetChildNames("Groups")
+
+        for g in groups:
+            g1 = self._app.oeditor.GetChildObject(g)
+            if g1:
+                group_hierarchy[g] = list(g1.GetChildNames())
 
         def multiplier_from_dataset(expression, valuein):
             multiplier = 0
             if expression in self._app.design_datasets:
                 dataset = self._app.design_datasets[expression]
             elif expression in self._app.project_datasets:
                 dataset = self._app.design_datasets[expression]
@@ -3432,39 +3446,49 @@
                         power_value[0], unit_system="Power", input_units=power_value[1], output_units=units
                     )
 
                 else:
                     power_value, exp = extract_dataset_info(bc_obj, units_input=units, boundary="Power")
                     mult = multiplier_from_dataset(exp, temperature)
 
+                for objs in bc_obj.props["Objects"]:
+                    obj_name = self.modeler[objs].name
+                    power_dict_obj[obj_name] = power_value * mult
+
                 power_dict[bc_obj.name] = power_value * n * mult
-                self.logger.info("The power of {} is {} {}".format(bc_obj.name, str(power_dict[bc_obj.name]), units))
 
             elif bc_obj.type == "SourceIcepak":
                 if bc_obj.props["Thermal Condition"] == "Total Power":
                     n = 0
                     if "Faces" in bc_obj.props:
                         n += len(bc_obj.props["Faces"])
-                    if "Objects" in bc_obj.props:
+                    elif "Objects" in bc_obj.props:
                         n += len(bc_obj.props["Objects"])
 
                     if "Total Power Variation Data" not in bc_obj.props:
                         mult = 1
                         power_value = list(decompose_variable_value(bc_obj.props["Total Power"]))
                         power_value = unit_converter(
                             power_value[0], unit_system="Power", input_units=power_value[1], output_units=units
                         )
                     else:
                         power_value, exp = extract_dataset_info(bc_obj, units_input=units, boundary="Power")
                         mult = multiplier_from_dataset(exp, temperature)
 
+                    if "Objects" in bc_obj.props:
+                        for objs in bc_obj.props["Objects"]:
+                            obj_name = self.modeler[objs].name
+                            power_dict_obj[obj_name] = power_value * mult
+
+                    elif "Faces" in bc_obj.props:
+                        for facs in bc_obj.props["Faces"]:
+                            obj_name = self.modeler.oeditor.GetObjectNameByFaceID(facs) + "_FaceID" + str(facs)
+                            power_dict_obj[obj_name] = power_value * mult
+
                     power_dict[bc_obj.name] = power_value * n * mult
-                    self.logger.info(
-                        "The power of {} is {} {}".format(bc_obj.name, str(power_dict[bc_obj.name]), units)
-                    )
 
                 elif bc_obj.props["Thermal Condition"] == "Surface Flux":
                     if "Surface Heat Variation Data" not in bc_obj.props:
                         mult = 1
                         heat_value = list(decompose_variable_value(bc_obj.props["Surface Heat"]))
                         if isinstance(heat_value[0], str):
                             new_value = self._app[heat_value[0]]
@@ -3472,15 +3496,15 @@
                         heat_value = unit_converter(
                             heat_value[0],
                             unit_system="SurfaceHeat",
                             input_units=heat_value[1],
                             output_units="irrad_W_per_m2",
                         )
                     else:
-                        mult = 0
+                        mult = 1
                         if bc_obj.props["Surface Heat Variation Data"]["Variation Type"] == "Temp Dep":
                             heat_value, exp = extract_dataset_info(bc_obj, boundary="SurfaceHeat")
                             mult = multiplier_from_dataset(exp, temperature)
                         else:
                             heat_value = 0
 
                     power_value = 0.0
@@ -3490,64 +3514,86 @@
                             area = unit_converter(
                                 area,
                                 unit_system="Area",
                                 input_units=self.modeler.model_units + "2",
                                 output_units="m2",
                             )
                             power_value += heat_value * area * mult
-                    if "Objects" in bc_obj.props:
+                    elif "Objects" in bc_obj.props:
                         for component in bc_obj.props["Objects"]:
                             object_assigned = self.modeler[component]
                             for f in object_assigned.faces:
                                 area = unit_converter(
                                     f.area,
                                     unit_system="Area",
                                     input_units=self.modeler.model_units + "2",
                                     output_units="m2",
                                 )
                                 power_value += heat_value * area * mult
 
                     power_value = unit_converter(power_value, unit_system="Power", input_units="W", output_units=units)
+
+                    if "Objects" in bc_obj.props:
+                        for objs in bc_obj.props["Objects"]:
+                            obj_name = self.modeler[objs].name
+                            power_dict_obj[obj_name] = power_value
+
+                    elif "Faces" in bc_obj.props:
+                        for facs in bc_obj.props["Faces"]:
+                            obj_name = self.modeler.oeditor.GetObjectNameByFaceID(facs) + "_FaceID" + str(facs)
+                            power_dict_obj[obj_name] = power_value
+
                     power_dict[bc_obj.name] = power_value
-                    self.logger.info(
-                        "The power of {} is {} {}".format(bc_obj.name, str(power_dict[bc_obj.name]), units)
-                    )
 
             elif bc_obj.type == "Network":
                 nodes = bc_obj.props["Nodes"]
                 power_value = 0
                 for node in nodes:
                     if "Power" in nodes[node]:
                         value = nodes[node]["Power"]
                         value = list(decompose_variable_value(value))
                         value = unit_converter(value[0], unit_system="Power", input_units=value[1], output_units=units)
                         power_value += value
+
+                obj_name = self.modeler.oeditor.GetObjectNameByFaceID(bc_obj.props["Faces"][0])
+                for facs in bc_obj.props["Faces"]:
+                    obj_name += "_FaceID" + str(facs)
+                power_dict_obj[obj_name] = power_value
+
                 power_dict[bc_obj.name] = power_value
-                self.logger.info("The power of {} is {} {}".format(bc_obj.name, str(power_dict[bc_obj.name]), units))
 
             elif bc_obj.type == "Conducting Plate":
                 n = 0
                 if "Faces" in bc_obj.props:
                     n += len(bc_obj.props["Faces"])
-                if "Objects" in bc_obj.props:
+                elif "Objects" in bc_obj.props:
                     n += len(bc_obj.props["Objects"])
 
                 if "Total Power Variation Data" not in bc_obj.props:
                     mult = 1
                     power_value = list(decompose_variable_value(bc_obj.props["Total Power"]))
                     power_value = unit_converter(
                         power_value[0], unit_system="Power", input_units=power_value[1], output_units=units
                     )
 
                 else:
                     power_value, exp = extract_dataset_info(bc_obj, units_input=units, boundary="Power")
                     mult = multiplier_from_dataset(exp, temperature)
 
+                if "Objects" in bc_obj.props:
+                    for objs in bc_obj.props["Objects"]:
+                        obj_name = self.modeler[objs].name
+                        power_dict_obj[obj_name] = power_value * mult
+
+                elif "Faces" in bc_obj.props:
+                    for facs in bc_obj.props["Faces"]:
+                        obj_name = self.modeler.oeditor.GetObjectNameByFaceID(facs) + "_FaceID" + str(facs)
+                        power_dict_obj[obj_name] = power_value * mult
+
                 power_dict[bc_obj.name] = power_value * n * mult
-                self.logger.info("The power of {} is {} {}".format(bc_obj.name, str(power_dict[bc_obj.name]), units))
 
             elif bc_obj.type == "Stationary Wall":
                 if bc_obj.props["External Condition"] == "Heat Flux":
                     mult = 1
                     heat_value = list(decompose_variable_value(bc_obj.props["Heat Flux"]))
                     heat_value = unit_converter(
                         heat_value[0],
@@ -3576,38 +3622,51 @@
                                     unit_system="Area",
                                     input_units=self.modeler.model_units + "2",
                                     output_units="m2",
                                 )
                                 power_value += heat_value * area * mult
 
                     power_value = unit_converter(power_value, unit_system="Power", input_units="W", output_units=units)
+
+                    if "Objects" in bc_obj.props:
+                        for objs in bc_obj.props["Objects"]:
+                            obj_name = self.modeler[objs].name
+                            power_dict_obj[obj_name] = power_value
+
+                    elif "Faces" in bc_obj.props:
+                        for facs in bc_obj.props["Faces"]:
+                            obj_name = self.modeler.oeditor.GetObjectNameByFaceID(facs) + "_FaceID" + str(facs)
+                            power_dict_obj[obj_name] = power_value
+
                     power_dict[bc_obj.name] = power_value
-                    self.logger.info(
-                        "The power of {} is {} {}".format(bc_obj.name, str(power_dict[bc_obj.name]), units)
-                    )
 
             elif bc_obj.type == "Resistance":
                 n = len(bc_obj.props["Objects"])
                 mult = 1
                 power_value = list(decompose_variable_value(bc_obj.props["Thermal Power"]))
                 power_value = unit_converter(
                     power_value[0], unit_system="Power", input_units=power_value[1], output_units=units
                 )
 
+                for objs in bc_obj.props["Objects"]:
+                    obj_name = self.modeler[objs].name
+                    power_dict_obj[obj_name] = power_value * mult
+
                 power_dict[bc_obj.name] = power_value * n * mult
-                self.logger.info("The power of {} is {} {}".format(bc_obj.name, str(power_dict[bc_obj.name]), units))
 
             elif bc_obj.type == "Blower":
                 power_value = list(decompose_variable_value(bc_obj.props["Blower Power"]))
                 power_value = unit_converter(
                     power_value[0], unit_system="Power", input_units=power_value[1], output_units=units
                 )
 
+                obj_name = bc_obj.name
+                power_dict_obj[obj_name] = power_value
+
                 power_dict[bc_obj.name] = power_value
-                self.logger.info("The power of {} is {} {}".format(bc_obj.name, str(power_dict[bc_obj.name]), units))
 
         for native_comps in self.modeler.user_defined_components:
             if hasattr(self.modeler.user_defined_components[native_comps], "native_properties"):
                 native_key = "NativeComponentDefinitionProvider"
                 if native_key in self.modeler.user_defined_components[native_comps].native_properties:
                     power_key = self.modeler.user_defined_components[native_comps].native_properties[native_key]
                 else:
@@ -3619,21 +3678,45 @@
                     power_value = list(decompose_variable_value(power_key["HubPower"]))
 
                 if power_value:
                     power_value = unit_converter(
                         power_value[0], unit_system="Power", input_units=power_value[1], output_units=units
                     )
 
+                    power_dict_obj[native_comps] = power_value
                     power_dict[native_comps] = power_value
-                    self.logger.info(
-                        "The power of {} is {} {}".format(native_comps, str(power_dict[native_comps]), units)
-                    )
 
-        self.logger.info("The total power is {} {}".format(str(sum(power_dict.values())), units))
-        return power_dict, sum(power_dict.values())
+        for group in reversed(list(group_hierarchy.keys())):
+            for comp in group_hierarchy[group]:
+                for power_comp in list(power_dict_obj.keys())[:]:
+                    if power_comp.find(comp) >= 0:
+                        if group not in power_dict_obj.keys():
+                            power_dict_obj[group] = 0.0
+                        power_dict_obj[group] += power_dict_obj[power_comp]
+
+        if output_type == "boundary":
+            for comp in power_dict.keys():
+                self.logger.info("The power of {} is {} {}".format(comp, str(round(power_dict[comp], 3)), units))
+            self.logger.info("The total power is {} {}".format(str(round(sum(power_dict.values()), 3)), units))
+            return power_dict, sum(power_dict.values())
+
+        elif output_type == "component":
+            for comp in power_dict_obj.keys():
+                self.logger.info("The power of {} is {} {}".format(comp, str(round(power_dict_obj[comp], 3)), units))
+            self.logger.info("The total power is {} {}".format(str(round(sum(power_dict_obj.values()), 3)), units))
+            return power_dict_obj, sum(power_dict_obj.values())
+
+        else:
+            for comp in power_dict.keys():
+                self.logger.info("The power of {} is {} {}".format(comp, str(round(power_dict[comp], 3)), units))
+            self.logger.info("The total power is {} {}".format(str(round(sum(power_dict.values()), 3)), units))
+            for comp in power_dict_obj.keys():
+                self.logger.info("The power of {} is {} {}".format(comp, str(round(power_dict_obj[comp], 3)), units))
+            self.logger.info("The total power is {} {}".format(str(round(sum(power_dict_obj.values()), 3)), units))
+            return power_dict_obj, sum(power_dict_obj.values()), power_dict, sum(power_dict.values())
 
     def create_creeping_plane_visual_ray_tracing(
         self,
         max_frequency="1GHz",
         ray_density=1,
         sample_density=10,
         ray_cutoff=40,
```

### Comparing `pyaedt-0.6.79/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.80/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.80/pyaedt/modules/SolveSetup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.constants import AEDT_UNITS
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.SetupTemplates import SetupKeys
 from pyaedt.modules.SolveSweeps import SetupProps
 from pyaedt.modules.SolveSweeps import SweepHFSS
 from pyaedt.modules.SolveSweeps import SweepHFSS3DLayout
 from pyaedt.modules.SolveSweeps import SweepMatrix
 from pyaedt.modules.SolveSweeps import identify_setup
@@ -1346,15 +1347,17 @@
         """
         self.props["Properties"]["Enable"] = "false"
         self.update()
         return True
 
     @pyaedt_function_handler()
     def export_to_hfss(self, file_fullname, keep_net_name=False):
-        """Export the HFSS 3DLayout design to HFSS 3D design.
+        """Export the HFSS 3D Layout design to HFSS 3D design.
+
+        This method is not supported with IronPython.
 
         Parameters
         ----------
         file_fullname : str
             Full path and file name for exporting the project.
 
         keep_net_name : bool
@@ -1376,17 +1379,20 @@
             return False
         file_fullname = os.path.splitext(file_fullname)[0] + ".aedt"
         info_messages = list(self.p_app.odesktop.GetMessages(self.p_app.project_name, self.p_app.design_name, 0))
         error_messages = list(self.p_app.odesktop.GetMessages(self.p_app.project_name, self.p_app.design_name, 2))
         self.omodule.ExportToHfss(self.name, file_fullname)
         succeeded = self._check_export_log(info_messages, error_messages, file_fullname)
         if succeeded and keep_net_name:
-            from pyaedt import Hfss
+            if not is_ironpython:
+                from pyaedt import Hfss
 
-            self._get_net_names(Hfss, file_fullname)
+                self._get_net_names(Hfss, file_fullname)
+            else:
+                self.p_app.logger.error("Exporting layout while keeping net name is not supported with IronPython")
         return succeeded
 
     @pyaedt_function_handler()
     def _get_net_names(self, app, file_fullname):
         primitives_3d_pts_per_nets = self._get_primitives_points_per_net()
         via_per_nets = self._get_via_position_per_net()
         layers_elevation = {
@@ -1446,25 +1452,54 @@
     @pyaedt_function_handler()
     def _get_primitives_points_per_net(self):
         edb = self.p_app.modeler.edb
         net_primitives = edb.modeler.primitives_by_net
         primitive_dict = {}
         for net, primitives in net_primitives.items():
             primitive_dict[net] = []
-            if primitives:
+            n = 0
+            while len(primitive_dict[net]) < len(net_primitives[net]):
+                if n > 1000:  # adding 1000 as maximum value to prevent infinite loop
+                    return
+                n += 10
+                primitive_dict[net] = []
                 for prim in primitives:
                     layer = edb.stackup.signal_layers[prim.layer_name]
                     z = layer.lower_elevation + layer.thickness / 2
-                    for arc in prim.arcs:
-                        pt = self._get_polygon_centroid(arc.points)
+                    pt = self._get_point_inside_primitive(prim, n)
+                    if pt:
                         pt.append(z)
                         primitive_dict[net].append(pt)
         return primitive_dict
 
     @pyaedt_function_handler()
+    def _get_point_inside_primitive(self, primitive, n):
+        from pyaedt.modeler.geometry_operators import GeometryOperators
+
+        if not is_ironpython:
+            import numpy as np
+        else:
+            return False
+        bbox = primitive.bbox
+        primitive_x_points = []
+        primitive_y_points = []
+        for arc in primitive.arcs:
+            if len(arc.points) == 2:
+                primitive_x_points += arc.points[0]
+                primitive_y_points += arc.points[1]
+        dx = (bbox[2] - bbox[0]) / n
+        dy = (bbox[3] - bbox[1]) / n
+        xcoords = [i for i in np.arange(bbox[0], bbox[2], dx)]
+        ycoords = [i for i in np.arange(bbox[1], bbox[3], dy)]
+        for x in xcoords:
+            for y in ycoords:
+                if GeometryOperators.point_in_polygon([x, y], [primitive_x_points, primitive_y_points]) == 1:
+                    return [x, y]
+
+    @pyaedt_function_handler()
     def _get_polygon_centroid(self, arcs=None):
         if arcs:
             k = len(arcs[0])
             x = sum(arcs[0]) / k
             y = sum(arcs[1]) / k
             return [x, y]
 
@@ -1556,17 +1591,20 @@
         if os.path.exists(file_fullname):
             os.unlink(file_fullname)
         info_messages = list(self.p_app.odesktop.GetMessages(self.p_app.project_name, self.p_app.design_name, 0))
         error_messages = list(self.p_app.odesktop.GetMessages(self.p_app.project_name, self.p_app.design_name, 2))
         self.omodule.ExportToQ3d(self.name, file_fullname)
         succeeded = self._check_export_log(info_messages, error_messages, file_fullname)
         if succeeded and keep_net_name:
-            from pyaedt import Q3d
+            if not is_ironpython:
+                from pyaedt import Q3d
 
-            self._get_net_names(Q3d, file_fullname)
+                self._get_net_names(Q3d, file_fullname)
+            else:
+                self.p_app.logger.error("Exporting layout while keeping net name is not supported with IronPython")
         return succeeded
 
     @pyaedt_function_handler()
     def add_sweep(self, sweepname=None, sweeptype="Interpolating"):
         """Add a frequency sweep.
 
         Parameters
```

### Comparing `pyaedt-0.6.79/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.80/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.80/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/report_templates.py` & `pyaedt-0.6.80/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/modules/solutions.py` & `pyaedt-0.6.80/pyaedt/modules/solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/q3d.py` & `pyaedt-0.6.80/pyaedt/q3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/rmxprt.py` & `pyaedt-0.6.80/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.80/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.80/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.80/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.80/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.80/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.80/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.80/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.80/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.80/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.80/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.80/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.80/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.80/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.80/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.80/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/siwave.py` & `pyaedt-0.6.80/pyaedt/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyaedt/twinbuilder.py` & `pyaedt-0.6.80/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.79/pyproject.toml` & `pyaedt-0.6.80/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,43 +32,43 @@
     "psutil",
     "dotnetcore2 ==3.1.23;platform_system=='Linux'",
 ]
 
 [project.optional-dependencies]
 tests = [
     "ipython==8.13.0",
-    "imageio==2.30.0",
+    "imageio==2.31.1",
     "joblib==1.2.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "openpyxl==3.1.2",
     "osmnx",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.2; python_version > '3.7'",
-    "pytest==7.3.1",
-    "pytest-cov==4.0.0",
+    "pytest==7.3.2",
+    "pytest-cov==4.1.0",
     "pytest-xdist==3.3.1",
     "pyvista==0.39.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "scikit-learn==1.2.2",
     "SRTM.py",
     "utm",
     "scikit-rf",
 
 ]
 doc = [
     "ansys-sphinx-theme==0.9.9",
-    "imageio==2.30.0",
+    "imageio==2.31.1",
     "imageio-ffmpeg==0.4.8",
     "ipython==8.13.0",
     "ipywidgets==8.0.6",
     "joblib==1.2.0",
-    "jupyterlab==4.0.1",
+    "jupyterlab==4.0.2",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "nbsphinx==0.9.2",
     "numpydoc==1.5.0",
     "osmnx",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
@@ -85,15 +85,15 @@
     "sphinxcontrib-websupport==1.2.4",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 full = [
-    "imageio==2.30.0",
+    "imageio",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.2; python_version > '3.7'",
     "osmnx",
@@ -101,15 +101,15 @@
     "pyvista==0.38.0; python_version <= '3.7'",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 all = [
-    "imageio==2.30.0",
+    "imageio",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.2; python_version > '3.7'",
     "osmnx",
```

### Comparing `pyaedt-0.6.79/PKG-INFO` & `pyaedt-0.6.80/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.79
+Version: 0.6.80
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -17,35 +17,35 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: cffi == 1.15.1;platform_system=='Linux'
 Requires-Dist: pywin32 >= 303;platform_system=='Windows'
 Requires-Dist: pythonnet == 3.0.1
 Requires-Dist: rpyc==5.3.1
 Requires-Dist: psutil
 Requires-Dist: dotnetcore2 ==3.1.23;platform_system=='Linux'
-Requires-Dist: imageio==2.30.0 ; extra == "all"
+Requires-Dist: imageio ; extra == "all"
 Requires-Dist: matplotlib==3.5.3 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.2 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "all"
 Requires-Dist: pyvista==0.39.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: SRTM.py ; extra == "all"
 Requires-Dist: utm ; extra == "all"
 Requires-Dist: scikit-rf ; extra == "all"
 Requires-Dist: openpyxl==3.1.2 ; extra == "all"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
-Requires-Dist: imageio==2.30.0 ; extra == "doc"
+Requires-Dist: imageio==2.31.1 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
 Requires-Dist: ipython==8.13.0 ; extra == "doc"
 Requires-Dist: ipywidgets==8.0.6 ; extra == "doc"
 Requires-Dist: joblib==1.2.0 ; extra == "doc"
-Requires-Dist: jupyterlab==4.0.1 ; extra == "doc"
+Requires-Dist: jupyterlab==4.0.2 ; extra == "doc"
 Requires-Dist: matplotlib==3.5.3 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: nbsphinx==0.9.2 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: osmnx ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
@@ -60,41 +60,41 @@
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: SRTM.py ; extra == "doc"
 Requires-Dist: utm ; extra == "doc"
 Requires-Dist: scikit-rf ; extra == "doc"
 Requires-Dist: openpyxl==3.1.2 ; extra == "doc"
-Requires-Dist: imageio==2.30.0 ; extra == "full"
+Requires-Dist: imageio ; extra == "full"
 Requires-Dist: matplotlib==3.5.3 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.2 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "full"
 Requires-Dist: pyvista==0.39.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: SRTM.py ; extra == "full"
 Requires-Dist: utm ; extra == "full"
 Requires-Dist: scikit-rf ; extra == "full"
 Requires-Dist: openpyxl==3.1.2 ; extra == "full"
 Requires-Dist: ipython==8.13.0 ; extra == "tests"
-Requires-Dist: imageio==2.30.0 ; extra == "tests"
+Requires-Dist: imageio==2.31.1 ; extra == "tests"
 Requires-Dist: joblib==1.2.0 ; extra == "tests"
 Requires-Dist: matplotlib==3.5.3 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: openpyxl==3.1.2 ; extra == "tests"
 Requires-Dist: osmnx ; extra == "tests"
 Requires-Dist: pandas==1.3.5 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.2 ; extra == "tests" and ( python_version > '3.7')
-Requires-Dist: pytest==7.3.1 ; extra == "tests"
-Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
+Requires-Dist: pytest==7.3.2 ; extra == "tests"
+Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
 Requires-Dist: pytest-xdist==3.3.1 ; extra == "tests"
 Requires-Dist: pyvista==0.39.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: scikit-learn==1.2.2 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
 Requires-Dist: utm ; extra == "tests"
 Requires-Dist: scikit-rf ; extra == "tests"
```

