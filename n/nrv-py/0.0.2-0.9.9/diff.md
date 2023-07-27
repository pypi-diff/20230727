# Comparing `tmp/nrv-py-0.0.2.tar.gz` & `tmp/nrv-py-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/fkolbl/Downloads/NRV-master-2/dist/tmpur2p8o_l/nrv-py-0.0.2.tar", last modified: Thu Dec  9 15:25:50 2021, max compression
+gzip compressed data, was "nrv-py-0.9.9.tar", last modified: Thu Jul 27 11:36:12 2023, max compression
```

## Comparing `nrv-py-0.0.2.tar` & `nrv-py-0.9.9.tar`

### file list

```diff
@@ -1,200 +1,14 @@
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2021-12-09 15:25:50.000000 nrv-py-0.0.2/
--rw-r--r--   0 fkolbl     (501) staff       (20)      234 2021-12-09 01:28:16.000000 nrv-py-0.0.2/MANIFEST.in
--rw-r--r--   0 fkolbl     (501) staff       (20)      361 2021-12-09 15:25:50.000000 nrv-py-0.0.2/PKG-INFO
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv/
--rw-r--r--   0 fkolbl     (501) staff       (20)    32573 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/CL_postprocessing.py
--rw-r--r--   0 fkolbl     (501) staff       (20)    17505 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/CL_simulations.py
--rw-r--r--   0 fkolbl     (501) staff       (20)     7082 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/FEM.py
--rw-r--r--   0 fkolbl     (501) staff       (20)     6518 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/FL_postprocessing.py
--rw-r--r--   0 fkolbl     (501) staff       (20)     6984 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/MCore.py
--rw-r--r--   0 fkolbl     (501) staff       (20)      469 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/NRV.ini
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv/OTF_PP/
--rw-r--r--   0 fkolbl     (501) staff       (20)      569 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/OTF_PP/Raster_plot.py
--rw-r--r--   0 fkolbl     (501) staff       (20)      411 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/OTF_PP/Rmv_keys.py
--rw-r--r--   0 fkolbl     (501) staff       (20)      715 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/OTF_PP/Vmem_plot.py
--rw-r--r--   0 fkolbl     (501) staff       (20)      906 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/__init__.py
--rw-r--r--   0 fkolbl     (501) staff       (20)    30877 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/axons.py
--rw-r--r--   0 fkolbl     (501) staff       (20)      561 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/compileMods.py
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv/comsol_templates/
--rw-r--r--   0 fkolbl     (501) staff       (20)   121400 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/comsol_templates/Nerve_1_Fascicle_1_CUFF.mph
--rw-r--r--   0 fkolbl     (501) staff       (20)    62102 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/comsol_templates/Nerve_1_Fascicle_1_LIFE.mph
--rw-r--r--   0 fkolbl     (501) staff       (20)    66281 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/comsol_templates/Nerve_1_Fascicle_2_LIFE.mph
--rw-r--r--   0 fkolbl     (501) staff       (20)     6153 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/electrodes.py
--rw-r--r--   0 fkolbl     (501) staff       (20)    17795 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/extracellular.py
--rw-r--r--   0 fkolbl     (501) staff       (20)    33224 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/fascicle_generator.py
--rw-r--r--   0 fkolbl     (501) staff       (20)    49873 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/fascicles.py
--rw-r--r--   0 fkolbl     (501) staff       (20)     3226 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/file_handler.py
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv/geom/
--rw-r--r--   0 fkolbl     (501) staff       (20)  1736930 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/geom/smoothed_edges_white.dxf
--rw-r--r--   0 fkolbl     (501) staff       (20)    81236 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/geom/smoothed_edges_white.png
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv/log/
--rw-r--r--   0 fkolbl     (501) staff       (20)        1 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/log/NRV.log
--rw-r--r--   0 fkolbl     (501) staff       (20)     3912 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/log_interface.py
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv/materials/
--rw-r--r--   0 fkolbl     (501) staff       (20)       52 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/bone.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)       64 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/cerebrospinal_fluid.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)       50 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/dura.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)       49 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/endoneurium_bhadra.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)       83 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/endoneurium_ranck.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)       58 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/epidural_space.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)       48 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/epineurium.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)       33 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/material_1.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)       62 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/material_2.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)       50 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/muscle.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)       50 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/perineurium.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)       49 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/platinum.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)       39 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/saline.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)       47 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials/silicone.mat
--rw-r--r--   0 fkolbl     (501) staff       (20)     4186 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/materials.py
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv/mods/
--rw-r--r--   0 fkolbl     (501) staff       (20)     3787 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/AXNODE.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     1806 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/CaPump.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     2056 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/DNav18.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3043 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/KCa.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     2475 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/NaCaPump.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     1505 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/Nakpump.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     2225 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/NakpumpSchild.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     2773 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/Nav11_a.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     2762 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/Nav16_a.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     2747 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/RattayAberham.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     2574 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/caextscale.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     2607 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/caintscale.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     4234 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/can.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3606 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/cat.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)      502 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/extrapump.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3707 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/flut_motor.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3562 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/flut_sensory.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     2102 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/h.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)      994 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/k_ion_dynamics.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3226 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/ka.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     1739 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/kaslow.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3228 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/kd.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     1647 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/kdr.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     1010 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/kdr_Tiger.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3132 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/kds.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     1498 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/kf.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     1123 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/kmtype.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)      719 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/kna.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     1493 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/ks.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)      765 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/leak.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     1715 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/leakSchild.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3569 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/mysa_motor.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3560 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/mysa_sensory.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     2665 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/na3.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     1014 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/na_ion_dynamics.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3825 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/naf.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3072 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/naf97.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3183 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/naf97mean.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     1517 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/nahh.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3252 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/nas.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3128 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/nas97.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3240 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/nas97mean.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     2671 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/nattxs.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3232 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/nav1p9.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     1838 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/nax.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     5217 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/node_motor.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     5330 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/node_sensory.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3569 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/stin_motor.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)     3566 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/mods/stin_sensory.mod
--rw-r--r--   0 fkolbl     (501) staff       (20)    57274 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/myelinated.py
--rw-r--r--   0 fkolbl     (501) staff       (20)     2484 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/nerves.py
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv/pops/
--rw-r--r--   0 fkolbl     (501) staff       (20)    23459 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_1000_axons_A.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    23450 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_1000_axons_B.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    23429 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_1000_axons_C.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    23441 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_1000_axons_D.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    23456 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_1000_axons_E.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    23474 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_1000_axons_F.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)     2348 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_100_axons_A.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)     2346 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_100_axons_B.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)     2355 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_100_axons_C.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)     2349 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_100_axons_D.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)     2352 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_100_axons_E.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)     2346 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_100_axons_F.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    46916 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_2000_axons_A.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    46879 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_2000_axons_B.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    46946 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_2000_axons_C.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    46882 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_2000_axons_D.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    46948 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_2000_axons_E.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    46923 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_2000_axons_F.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)     4694 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_200_axons_A.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)     4681 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_200_axons_B.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)     4702 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_200_axons_C.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)     4699 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_200_axons_D.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)     4685 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_200_axons_E.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)     4673 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_200_axons_F.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)   117300 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_5000_axons_A.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)   117318 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_5000_axons_B.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)   117303 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_5000_axons_C.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)   117297 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_5000_axons_D.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)   117184 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_5000_axons_E.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)   117231 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_5000_axons_F.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    11725 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_500_axons_A.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    11730 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_500_axons_B.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    11732 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_500_axons_C.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    11720 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_500_axons_D.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    11705 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_500_axons_E.pop
--rw-r--r--   0 fkolbl     (501) staff       (20)    11710 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/pops/Population_of_500_axons_F.pop
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv/ppops/
--rw-r--r--   0 fkolbl     (501) staff       (20)    63162 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_1000_axons_A.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    63158 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_1000_axons_B.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    63156 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_1000_axons_C.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    63146 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_1000_axons_D.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    63224 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_1000_axons_E.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    63118 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_1000_axons_F.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)     6335 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_100_axons_A.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)     6345 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_100_axons_B.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)     6367 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_100_axons_C.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)     6337 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_100_axons_D.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)     6350 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_100_axons_E.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)     6346 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_100_axons_F.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)   125839 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_2000_axons_A.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)   125735 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_2000_axons_B.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)   125872 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_2000_axons_C.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)   125804 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_2000_axons_D.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)   125951 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_2000_axons_E.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)   125835 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_2000_axons_F.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    12703 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_200_axons_A.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    12674 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_200_axons_B.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    12705 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_200_axons_C.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    12695 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_200_axons_D.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    12671 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_200_axons_E.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    12677 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_200_axons_F.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)   316552 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_5000_axons_A.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)   316575 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_5000_axons_B.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)   316397 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_5000_axons_C.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)   316442 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_5000_axons_D.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)   316314 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_5000_axons_E.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)   316431 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_5000_axons_F.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    31672 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_500_axons_A.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    31680 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_500_axons_B.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    31643 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_500_axons_C.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    31664 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_500_axons_D.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    31663 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_500_axons_E.ppop
--rw-r--r--   0 fkolbl     (501) staff       (20)    31668 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/ppops/Placed_population_of_500_axons_F.ppop
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv/stats/
--rw-r--r--   0 fkolbl     (501) staff       (20)      219 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/stats/Jacobs_11_A.csv
--rw-r--r--   0 fkolbl     (501) staff       (20)      159 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/stats/Jacobs_11_B.csv
--rw-r--r--   0 fkolbl     (501) staff       (20)      249 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/stats/Jacobs_11_C.csv
--rw-r--r--   0 fkolbl     (501) staff       (20)      270 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/stats/Jacobs_11_D.csv
--rw-r--r--   0 fkolbl     (501) staff       (20)      169 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/stats/Jacobs_9_A.csv
--rw-r--r--   0 fkolbl     (501) staff       (20)      209 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/stats/Jacobs_9_B.csv
--rw-r--r--   0 fkolbl     (501) staff       (20)      269 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/stats/Jacobs_9_C.csv
--rw-r--r--   0 fkolbl     (501) staff       (20)      278 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/stats/Jacobs_9_D.csv
--rw-r--r--   0 fkolbl     (501) staff       (20)      319 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/stats/Ochoa_M.csv
--rw-r--r--   0 fkolbl     (501) staff       (20)      401 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/stats/Ochoa_U.csv
--rw-r--r--   0 fkolbl     (501) staff       (20)     1415 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/stats/Schellens_1.csv
--rw-r--r--   0 fkolbl     (501) staff       (20)     1117 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/stats/Schellens_2.csv
--rwxr-xr-x   0 fkolbl     (501) staff       (20)    15688 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/stimulus.py
--rw-r--r--   0 fkolbl     (501) staff       (20)    43170 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/thin_myelinated.py
--rw-r--r--   0 fkolbl     (501) staff       (20)     1094 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/units.py
--rw-r--r--   0 fkolbl     (501) staff       (20)    44643 2021-12-09 01:28:16.000000 nrv-py-0.0.2/nrv/unmyelinated.py
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv_py.egg-info/
--rw-r--r--   0 fkolbl     (501) staff       (20)      361 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv_py.egg-info/PKG-INFO
--rw-r--r--   0 fkolbl     (501) staff       (20)     5790 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv_py.egg-info/SOURCES.txt
--rw-r--r--   0 fkolbl     (501) staff       (20)        1 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv_py.egg-info/dependency_links.txt
--rw-r--r--   0 fkolbl     (501) staff       (20)       55 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv_py.egg-info/requires.txt
--rw-r--r--   0 fkolbl     (501) staff       (20)        4 2021-12-09 15:25:50.000000 nrv-py-0.0.2/nrv_py.egg-info/top_level.txt
--rw-r--r--   0 fkolbl     (501) staff       (20)     1133 2021-12-09 01:28:16.000000 nrv-py-0.0.2/pyproject.toml
--rw-r--r--   0 fkolbl     (501) staff       (20)       38 2021-12-09 15:25:50.000000 nrv-py-0.0.2/setup.cfg
--rw-r--r--   0 fkolbl     (501) staff       (20)      612 2021-12-09 01:28:16.000000 nrv-py-0.0.2/setup.py
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-27 11:36:12.112702 nrv-py-0.9.9/
+-rw-r--r--   0 fkolbl     (501) staff       (20)      234 2023-07-25 23:18:42.000000 nrv-py-0.9.9/MANIFEST.in
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1300 2023-07-27 11:36:12.112193 nrv-py-0.9.9/PKG-INFO
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-27 11:36:12.108558 nrv-py-0.9.9/nrv/
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3111 2023-07-27 11:19:09.000000 nrv-py-0.9.9/nrv/__init__.py
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-27 11:36:12.111195 nrv-py-0.9.9/nrv_py.egg-info/
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1300 2023-07-27 11:36:12.000000 nrv-py-0.9.9/nrv_py.egg-info/PKG-INFO
+-rw-r--r--   0 fkolbl     (501) staff       (20)      200 2023-07-27 11:36:12.000000 nrv-py-0.9.9/nrv_py.egg-info/SOURCES.txt
+-rw-r--r--   0 fkolbl     (501) staff       (20)        1 2023-07-27 11:36:12.000000 nrv-py-0.9.9/nrv_py.egg-info/dependency_links.txt
+-rw-r--r--   0 fkolbl     (501) staff       (20)       88 2023-07-27 11:36:12.000000 nrv-py-0.9.9/nrv_py.egg-info/requires.txt
+-rw-r--r--   0 fkolbl     (501) staff       (20)        4 2023-07-27 11:36:12.000000 nrv-py-0.9.9/nrv_py.egg-info/top_level.txt
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1424 2023-07-27 11:35:12.000000 nrv-py-0.9.9/pyproject.toml
+-rw-r--r--   0 fkolbl     (501) staff       (20)       38 2023-07-27 11:36:12.112799 nrv-py-0.9.9/setup.cfg
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1335 2023-07-26 08:32:23.000000 nrv-py-0.9.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nrv-py-0.0.2/pyproject.toml` & `nrv-py-0.9.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -3,27 +3,37 @@
 [project]
 name = 'nrv-py'
 authors = [{name='Florian Kolbl - Roland Giraud - Louis Regnacq - Thomas Couppey'}]
 license = {file='License.txt'}
 keywords = ['neuronal simulation', 'computer simulation', 'neurosciences',
             'multiphysics', 'Neuron', 'Comsol']
 classifiers = [
+    'License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)',
     'Development Status :: 5 - Production/Stable',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Operating System :: Microsoft :: Windows',
     'Operating System :: POSIX :: Linux',
     'Operating System :: MacOS :: MacOS X',
-    'Topic :: Scientific/Engineering :: Neuroscience',
+    'Intended Audience :: Education',
     'Intended Audience :: Science/Research',
+    'Topic :: Scientific/Engineering :: Bio-Informatics',
+    'Topic :: Scientific/Engineering :: Medical Science Apps.',
     'Natural Language :: English']
 readme = 'pypi.md'
 requires-python = '>=3.6'
-dependencies = ['mph', 'numpy','scipy','neuron','matplotlib','numba','ezdxf','icecream']
+dependencies = ['mph', 'numpy','scipy','neuron','matplotlib','numba','ezdxf','icecream','pyswarms']
 dynamic = ['version', 'description']
 
 [project.urls]
 Documentation = 'https://nrv.readthedocs.io'
 Source = 'https://github.com/fkolbl/NRV'
+
+
+[project.optional-dependencies]
+dev = [
+    'Sphinx >= 6.1',
+    'Furo',
+]
```

