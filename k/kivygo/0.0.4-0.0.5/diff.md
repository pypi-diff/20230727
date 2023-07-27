# Comparing `tmp/kivygo-0.0.4.tar.gz` & `tmp/kivygo-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivygo-0.0.4.tar", last modified: Mon Jun  5 21:35:12 2023, max compression
+gzip compressed data, was "kivygo-0.0.5.tar", last modified: Thu Jul 27 01:21:17 2023, max compression
```

## Comparing `kivygo-0.0.4.tar` & `kivygo-0.0.5.tar`

### file list

```diff
@@ -1,193 +1,196 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 21:35:12.225710 kivygo-0.0.4/
--rw-rw-rw-   0        0        0     1098 2023-04-28 02:03:52.000000 kivygo-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      192 2023-06-05 21:35:12.224702 kivygo-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 21:35:12.050260 kivygo-0.0.4/kivygo/
--rw-rw-rw-   0        0        0       23 2023-06-05 21:34:14.000000 kivygo-0.0.4/kivygo/__init__.py
--rw-rw-rw-   0        0        0    23309 2023-05-13 18:28:10.000000 kivygo-0.0.4/kivygo/animation.py
--rw-rw-rw-   0        0        0     2905 2023-05-13 17:09:56.000000 kivygo-0.0.4/kivygo/app.py
-drwxrwxrwx   0        0        0        0 2023-06-05 21:35:12.065540 kivygo-0.0.4/kivygo/behaviors/
--rw-rw-rw-   0        0        0        0 2023-05-30 13:05:00.000000 kivygo-0.0.4/kivygo/behaviors/__init__.py
--rw-rw-rw-   0        0        0     8273 2023-05-13 17:19:46.000000 kivygo-0.0.4/kivygo/behaviors/button.py
--rw-rw-rw-   0        0        0     9872 2023-05-13 18:19:31.000000 kivygo-0.0.4/kivygo/behaviors/drag_and_drop.py
--rw-rw-rw-   0        0        0     5868 2023-06-05 21:32:41.000000 kivygo-0.0.4/kivygo/behaviors/hover.py
--rw-rw-rw-   0        0        0     3058 2023-05-05 22:06:08.000000 kivygo-0.0.4/kivygo/behaviors/neumorph.py
--rw-rw-rw-   0        0        0    13342 2023-04-28 02:33:05.000000 kivygo-0.0.4/kivygo/behaviors/resizable.py
--rw-rw-rw-   0        0        0    15085 2023-05-08 00:20:07.000000 kivygo-0.0.4/kivygo/behaviors/thumb.py
--rw-rw-rw-   0        0        0     4375 2023-05-07 23:38:10.000000 kivygo-0.0.4/kivygo/behaviors/touch_effecs.py
--rw-rw-rw-   0        0        0    16042 2023-05-01 21:00:44.000000 kivygo-0.0.4/kivygo/bounds_math.py
--rw-rw-rw-   0        0        0     2375 2023-05-29 23:31:04.000000 kivygo-0.0.4/kivygo/colors.py
-drwxrwxrwx   0        0        0        0 2023-06-05 21:35:12.073738 kivygo-0.0.4/kivygo/config/
--rw-rw-rw-   0        0        0      296 2023-04-30 03:08:38.000000 kivygo-0.0.4/kivygo/config/coins.atlas
--rw-rw-rw-   0        0        0     4765 2023-04-29 21:48:35.000000 kivygo-0.0.4/kivygo/config/coins.bounds
--rw-rw-rw-   0        0        0     1490 2013-02-26 10:24:28.000000 kivygo-0.0.4/kivygo/config/drugs.pex
--rw-rw-rw-   0        0        0     1489 2013-02-26 10:24:28.000000 kivygo-0.0.4/kivygo/config/fire.pex
--rw-rw-rw-   0        0        0     1496 2013-02-26 10:24:28.000000 kivygo-0.0.4/kivygo/config/jellyfish.pex
--rw-rw-rw-   0        0        0     1463 2013-02-26 10:24:28.000000 kivygo-0.0.4/kivygo/config/particle.pex
--rw-rw-rw-   0        0        0      870 2013-02-26 10:24:28.000000 kivygo-0.0.4/kivygo/config/particle.png
--rw-rw-rw-   0        0        0     1494 2013-02-26 10:24:28.000000 kivygo-0.0.4/kivygo/config/sun.pex
-drwxrwxrwx   0        0        0        0 2023-06-05 21:35:12.078844 kivygo-0.0.4/kivygo/elevation/
--rw-rw-rw-   0        0        0     1630 2023-01-06 02:24:33.000000 kivygo-0.0.4/kivygo/elevation/elevation.frag
--rw-rw-rw-   0        0        0      198 2023-01-06 02:24:33.000000 kivygo-0.0.4/kivygo/elevation/header.frag
--rw-rw-rw-   0        0        0      184 2023-01-06 02:24:33.000000 kivygo-0.0.4/kivygo/elevation/main.frag
-drwxrwxrwx   0        0        0        0 2023-06-05 21:35:12.103763 kivygo-0.0.4/kivygo/icons/
--rw-rw-rw-   0        0        0   156742 2023-03-02 15:36:22.000000 kivygo-0.0.4/kivygo/icons/bg_example.png
--rw-rw-rw-   0        0        0    95465 2022-05-23 02:23:22.000000 kivygo-0.0.4/kivygo/icons/coins.png
--rw-rw-rw-   0        0        0     1244 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/discord.svg
--rw-rw-rw-   0        0        0      781 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/discord2.svg
--rw-rw-rw-   0        0        0      704 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/facebook2.svg
--rw-rw-rw-   0        0        0     2453 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/github.svg
--rw-rw-rw-   0        0        0     1864 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/github2.svg
--rw-rw-rw-   0        0        0      829 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/github3.svg
--rw-rw-rw-   0        0        0     2451 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/google.svg
--rw-rw-rw-   0        0        0      990 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/google3.svg
--rw-rw-rw-   0        0        0     2636 2022-05-23 02:23:22.000000 kivygo-0.0.4/kivygo/icons/kivy.png
--rw-rw-rw-   0        0        0     1141 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/kivy.svg
--rw-rw-rw-   0        0        0    16577 2023-03-02 15:36:22.000000 kivygo-0.0.4/kivygo/icons/kivy_logo.png
--rw-rw-rw-   0        0        0    42074 2021-05-11 19:10:56.000000 kivygo-0.0.4/kivygo/icons/kivymd_logo.png
--rw-rw-rw-   0        0        0     2919 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/pie_chart.svg
--rw-rw-rw-   0        0        0     1458 2023-02-14 20:11:52.000000 kivygo-0.0.4/kivygo/icons/pipette.png
--rw-rw-rw-   0        0        0     1133 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/python2.svg
--rw-rw-rw-   0        0        0     1621 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/search.svg
--rw-rw-rw-   0        0        0      851 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/so.svg
--rw-rw-rw-   0        0        0     1481 2022-05-23 02:23:22.000000 kivygo-0.0.4/kivygo/icons/square.png
--rw-rw-rw-   0        0        0     1814 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/sublime.svg
--rw-rw-rw-   0        0        0     3454 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/text.svg
--rw-rw-rw-   0        0        0     1928 2023-02-14 20:11:52.000000 kivygo-0.0.4/kivygo/icons/transparent.png
--rw-rw-rw-   0        0        0     1086 2021-06-29 07:37:30.000000 kivygo-0.0.4/kivygo/icons/twitter2.svg
-drwxrwxrwx   0        0        0        0 2023-06-05 21:35:12.114039 kivygo-0.0.4/kivygo/images/
--rw-rw-rw-   0        0        0   709001 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/images/busan.jpg
--rw-rw-rw-   0        0        0   118790 2018-10-01 10:52:31.000000 kivygo-0.0.4/kivygo/images/demoimage.jpg
--rw-rw-rw-   0        0        0   190380 2023-04-28 21:56:31.000000 kivygo-0.0.4/kivygo/images/icon-kivygo.png
--rw-rw-rw-   0        0        0   431598 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/images/iris.jpg
--rw-rw-rw-   0        0        0   857961 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/images/lion.jpg
--rw-rw-rw-   0        0        0      879 2019-05-19 13:30:15.000000 kivygo-0.0.4/kivygo/images/navigationdrawer_gradient_ltor.png
--rw-rw-rw-   0        0        0      874 2019-05-19 13:30:15.000000 kivygo-0.0.4/kivygo/images/navigationdrawer_gradient_rtol.png
--rw-rw-rw-   0        0        0  1537713 2023-02-14 20:11:52.000000 kivygo-0.0.4/kivygo/images/test.jpg
--rw-rw-rw-   0        0        0     2334 2023-04-21 01:53:43.000000 kivygo-0.0.4/kivygo/transformations.py
-drwxrwxrwx   0        0        0        0 2023-06-05 21:35:12.184450 kivygo-0.0.4/kivygo/transitions/
--rw-rw-rw-   0        0        0      452 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Angular.glsl
--rw-rw-rw-   0        0        0      719 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Bounce.glsl
--rw-rw-rw-   0        0        0     2593 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/BowTieHorizontal.glsl
--rw-rw-rw-   0        0        0     2541 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/BowTieVertical.glsl
--rw-rw-rw-   0        0        0      231 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Burn.glsl
--rw-rw-rw-   0        0        0      948 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/ButterflyWaveScrawler.glsl
--rw-rw-rw-   0        0        0      485 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/CannabisLeaf.glsl
--rw-rw-rw-   0        0        0      398 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Circle.glsl
--rw-rw-rw-   0        0        0      386 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/CircleOpen.glsl
--rw-rw-rw-   0        0        0      370 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/ColorPhase.glsl
--rw-rw-rw-   0        0        0      353 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/ColourDistance.glsl
--rw-rw-rw-   0        0        0      586 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/CrazyParametricFun.glsl
--rw-rw-rw-   0        0        0      590 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/CrossHatch.glsl
--rw-rw-rw-   0        0        0      228 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/CrossWarp.glsl
--rw-rw-rw-   0        0        0     2385 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/CrossZoom.glsl
--rw-rw-rw-   0        0        0     1694 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Cube.glsl
--rw-rw-rw-   0        0        0      352 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/DirectionalEasing.glsl
--rw-rw-rw-   0        0        0      489 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/DirectionalWarp.glsl
--rw-rw-rw-   0        0        0      557 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/DirectionalWipe.glsl
--rw-rw-rw-   0        0        0      522 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Displacement.glsl
--rw-rw-rw-   0        0        0     1574 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/DoomScreenTransition.glsl
--rw-rw-rw-   0        0        0     1189 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Doorway.glsl
--rw-rw-rw-   0        0        0      378 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Dreamy.glsl
--rw-rw-rw-   0        0        0     1183 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/DreamyZoom.glsl
--rw-rw-rw-   0        0        0      136 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Fade.glsl
--rw-rw-rw-   0        0        0      391 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/FadeColor.glsl
--rw-rw-rw-   0        0        0      546 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/FadeGrayscale.glsl
--rw-rw-rw-   0        0        0     2220 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/FilmBurn.glsl
--rw-rw-rw-   0        0        0      489 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/FlyEye.glsl
--rw-rw-rw-   0        0        0     2198 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/GlitchDisplace.glsl
--rw-rw-rw-   0        0        0      607 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/GlitchMemories.glsl
--rw-rw-rw-   0        0        0     2245 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/GridFlip.glsl
--rw-rw-rw-   0        0        0      356 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Heart.glsl
--rw-rw-rw-   0        0        0     1663 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Hexagonalize.glsl
--rw-rw-rw-   0        0        0      549 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Kaleidoscope.glsl
--rw-rw-rw-   0        0        0      647 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/LeftRight.glsl
--rw-rw-rw-   0        0        0      671 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/LinearBlur.glsl
--rw-rw-rw-   0        0        0      226 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Luma.glsl
--rw-rw-rw-   0        0        0     3781 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/LuminanceMelt.glsl
--rw-rw-rw-   0        0        0      379 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Morph.glsl
--rw-rw-rw-   0        0        0     1105 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Mosaic.glsl
--rw-rw-rw-   0        0        0      339 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/MultiplyBlend.glsl
--rw-rw-rw-   0        0        0     1390 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/PageCurl.glsl
--rw-rw-rw-   0        0        0     1367 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Perlin.glsl
--rw-rw-rw-   0        0        0      349 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Pinwheel.glsl
--rw-rw-rw-   0        0        0      562 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Pixelize.glsl
--rw-rw-rw-   0        0        0      452 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/PolarFunction.glsl
--rw-rw-rw-   0        0        0      304 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/PolkaDotsCurtain.glsl
--rw-rw-rw-   0        0        0      353 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Radial.glsl
--rw-rw-rw-   0        0        0      444 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/RandomNoise.glsl
--rw-rw-rw-   0        0        0      377 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/RandomSquares.glsl
--rw-rw-rw-   0        0        0      356 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Ripple.glsl
--rw-rw-rw-   0        0        0      832 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/RotateScaleFade.glsl
--rw-rw-rw-   0        0        0      348 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/RotateTransition.glsl
--rw-rw-rw-   0        0        0      365 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/SimpleZoom.glsl
--rw-rw-rw-   0        0        0      742 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/SquaresWire.glsl
--rw-rw-rw-   0        0        0      444 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Squeeze.glsl
--rw-rw-rw-   0        0        0     8033 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/StereoViewer.glsl
--rw-rw-rw-   0        0        0     1506 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Swap.glsl
--rw-rw-rw-   0        0        0      715 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Swirl.glsl
--rw-rw-rw-   0        0        0     4051 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/TangentMotionBlur.glsl
--rw-rw-rw-   0        0        0      650 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/TopBottom.glsl
--rw-rw-rw-   0        0        0     1366 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/UndulatingBurnOut.glsl
--rw-rw-rw-   0        0        0      409 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/WaterDrop.glsl
--rw-rw-rw-   0        0        0      386 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/Wind.glsl
--rw-rw-rw-   0        0        0      274 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/WindowBlinds.glsl
--rw-rw-rw-   0        0        0      277 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/WindowSlice.glsl
--rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/WipeDown.glsl
--rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/WipeLeft.glsl
--rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/WipeRight.glsl
--rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/WipeUp.glsl
--rw-rw-rw-   0        0        0     1115 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/ZoomInCircles.glsl
--rw-rw-rw-   0        0        0     8072 2023-05-01 19:46:08.000000 kivygo-0.0.4/kivygo/transitions/__init__.py
--rw-rw-rw-   0        0        0     1197 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/base.py
-drwxrwxrwx   0        0        0        0 2023-06-05 21:35:12.186451 kivygo-0.0.4/kivygo/transitions/extra/
--rw-rw-rw-   0        0        0      177 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/extra/footer.glsl
--rw-rw-rw-   0        0        0      403 2021-05-13 08:40:19.000000 kivygo-0.0.4/kivygo/transitions/extra/header.glsl
-drwxrwxrwx   0        0        0        0 2023-06-05 21:35:12.222222 kivygo-0.0.4/kivygo/uix/
--rw-rw-rw-   0        0        0        0 2023-05-10 21:23:48.000000 kivygo-0.0.4/kivygo/uix/__init__.py
--rw-rw-rw-   0        0        0     4809 2023-05-13 16:09:23.000000 kivygo-0.0.4/kivygo/uix/anchorlayout.py
--rw-rw-rw-   0        0        0    13311 2023-06-02 21:48:13.000000 kivygo-0.0.4/kivygo/uix/androidtabs.py
--rw-rw-rw-   0        0        0     3904 2023-05-10 20:13:58.000000 kivygo-0.0.4/kivygo/uix/bezier.py
--rw-rw-rw-   0        0        0     2116 2023-05-03 13:52:13.000000 kivygo-0.0.4/kivygo/uix/boxlayout.py
--rw-rw-rw-   0        0        0     4378 2023-05-13 17:20:58.000000 kivygo-0.0.4/kivygo/uix/button.py
--rw-rw-rw-   0        0        0    12881 2023-04-28 02:33:05.000000 kivygo-0.0.4/kivygo/uix/camera.py
--rw-rw-rw-   0        0        0     7833 2023-05-09 02:19:31.000000 kivygo-0.0.4/kivygo/uix/circular_bar.py
--rw-rw-rw-   0        0        0    20660 2023-04-30 13:59:52.000000 kivygo-0.0.4/kivygo/uix/circulardatetimepicker.py
--rw-rw-rw-   0        0        0     4640 2023-05-13 17:19:53.000000 kivygo-0.0.4/kivygo/uix/circularlayout.py
--rw-rw-rw-   0        0        0    26840 2023-04-03 01:21:22.000000 kivygo-0.0.4/kivygo/uix/codeinput.py
--rw-rw-rw-   0        0        0     4798 2023-04-28 02:33:05.000000 kivygo-0.0.4/kivygo/uix/curvelayout.py
--rw-rw-rw-   0        0        0     1992 2023-04-25 21:55:26.000000 kivygo-0.0.4/kivygo/uix/effect.py
--rw-rw-rw-   0        0        0      781 2023-04-28 02:33:05.000000 kivygo-0.0.4/kivygo/uix/floatlayout.py
--rw-rw-rw-   0        0        0    21770 2023-06-02 01:05:08.000000 kivygo-0.0.4/kivygo/uix/frostedglass.py
--rw-rw-rw-   0        0        0     2380 2023-05-30 13:36:55.000000 kivygo-0.0.4/kivygo/uix/gradient.py
--rw-rw-rw-   0        0        0     2746 2023-05-08 15:57:00.000000 kivygo-0.0.4/kivygo/uix/gridlayout.py
--rw-rw-rw-   0        0        0     4910 2023-04-28 02:33:05.000000 kivygo-0.0.4/kivygo/uix/icon.py
--rw-rw-rw-   0        0        0     2644 2023-03-28 18:29:30.000000 kivygo-0.0.4/kivygo/uix/image.py
--rw-rw-rw-   0        0        0    10992 2023-05-13 17:22:37.000000 kivygo-0.0.4/kivygo/uix/input.py
--rw-rw-rw-   0        0        0     9341 2023-06-03 22:51:05.000000 kivygo-0.0.4/kivygo/uix/joystick.py
--rw-rw-rw-   0        0        0    21810 2023-05-10 20:33:34.000000 kivygo-0.0.4/kivygo/uix/kivyg_icon.py
--rw-rw-rw-   0        0        0     9082 2023-05-13 17:20:07.000000 kivygo-0.0.4/kivygo/uix/label.py
--rw-rw-rw-   0        0        0    14052 2023-05-13 17:20:10.000000 kivygo-0.0.4/kivygo/uix/navigationdrawer.py
--rw-rw-rw-   0        0        0    18174 2023-05-13 18:19:28.000000 kivygo-0.0.4/kivygo/uix/particle.py
--rw-rw-rw-   0        0        0     4457 2023-05-10 20:44:55.000000 kivygo-0.0.4/kivygo/uix/pizza_graph.py
--rw-rw-rw-   0        0        0     2807 2023-04-28 02:33:05.000000 kivygo-0.0.4/kivygo/uix/popup.py
--rw-rw-rw-   0        0        0     6764 2023-05-13 17:20:13.000000 kivygo-0.0.4/kivygo/uix/progressspinner.py
--rw-rw-rw-   0        0        0     6807 2023-05-13 18:19:05.000000 kivygo-0.0.4/kivygo/uix/radialslider.py
--rw-rw-rw-   0        0        0    24325 2023-05-10 20:56:39.000000 kivygo-0.0.4/kivygo/uix/rotabox.py
--rw-rw-rw-   0        0        0     1408 2023-04-06 21:24:34.000000 kivygo-0.0.4/kivygo/uix/screenmanager.py
--rw-rw-rw-   0        0        0     3598 2023-05-13 18:19:11.000000 kivygo-0.0.4/kivygo/uix/scrollview.py
--rw-rw-rw-   0        0        0     4990 2023-05-01 16:18:58.000000 kivygo-0.0.4/kivygo/uix/segment.py
--rw-rw-rw-   0        0        0     2959 2023-05-10 20:57:52.000000 kivygo-0.0.4/kivygo/uix/shader.py
--rw-rw-rw-   0        0        0     2858 2023-05-13 18:19:17.000000 kivygo-0.0.4/kivygo/uix/simpletablelayout.py
--rw-rw-rw-   0        0        0     5517 2023-05-05 22:56:03.000000 kivygo-0.0.4/kivygo/uix/slider.py
--rw-rw-rw-   0        0        0     4389 2023-05-10 21:19:13.000000 kivygo-0.0.4/kivygo/uix/spinner.py
--rw-rw-rw-   0        0        0    12722 2023-03-28 18:29:55.000000 kivygo-0.0.4/kivygo/uix/taptargetview.py
--rw-rw-rw-   0        0        0     6436 2023-05-13 17:20:20.000000 kivygo-0.0.4/kivygo/uix/terminal.py
--rw-rw-rw-   0        0        0     3601 2023-05-04 01:11:32.000000 kivygo-0.0.4/kivygo/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-05 21:35:12.058268 kivygo-0.0.4/kivygo.egg-info/
--rw-rw-rw-   0        0        0      192 2023-06-05 21:35:11.000000 kivygo-0.0.4/kivygo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5300 2023-06-05 21:35:11.000000 kivygo-0.0.4/kivygo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 21:35:11.000000 kivygo-0.0.4/kivygo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-06-05 21:35:11.000000 kivygo-0.0.4/kivygo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 21:35:11.000000 kivygo-0.0.4/kivygo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 21:35:12.225710 kivygo-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2126 2023-05-30 13:06:22.000000 kivygo-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:21:17.850036 kivygo-0.0.5/
+-rw-rw-rw-   0        0        0     1098 2023-04-28 02:03:52.000000 kivygo-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      192 2023-07-27 01:21:17.849043 kivygo-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 01:21:17.675333 kivygo-0.0.5/kivygo/
+-rw-rw-rw-   0        0        0     5006 2023-07-27 01:21:14.000000 kivygo-0.0.5/kivygo/__init__.py
+-rw-rw-rw-   0        0        0    23309 2023-05-13 18:28:10.000000 kivygo-0.0.5/kivygo/animation.py
+-rw-rw-rw-   0        0        0     1154 2023-07-20 20:07:25.000000 kivygo-0.0.5/kivygo/app.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:21:17.702908 kivygo-0.0.5/kivygo/behaviors/
+-rw-rw-rw-   0        0        0        0 2023-05-30 13:05:00.000000 kivygo-0.0.5/kivygo/behaviors/__init__.py
+-rw-rw-rw-   0        0        0     8135 2023-07-24 00:35:16.000000 kivygo-0.0.5/kivygo/behaviors/button.py
+-rw-rw-rw-   0        0        0     9888 2023-07-20 19:12:52.000000 kivygo-0.0.5/kivygo/behaviors/drag_and_drop.py
+-rw-rw-rw-   0        0        0     7318 2023-07-24 00:45:33.000000 kivygo-0.0.5/kivygo/behaviors/effect.py
+-rw-rw-rw-   0        0        0     5964 2023-07-20 20:04:50.000000 kivygo-0.0.5/kivygo/behaviors/hover.py
+-rw-rw-rw-   0        0        0     3065 2023-07-19 01:36:03.000000 kivygo-0.0.5/kivygo/behaviors/neumorph.py
+-rw-rw-rw-   0        0        0    13230 2023-07-19 01:37:31.000000 kivygo-0.0.5/kivygo/behaviors/resizable.py
+-rw-rw-rw-   0        0        0    15093 2023-07-19 01:38:36.000000 kivygo-0.0.5/kivygo/behaviors/thumb.py
+-rw-rw-rw-   0        0        0    16048 2023-07-19 01:58:47.000000 kivygo-0.0.5/kivygo/bounds_math.py
+-rw-rw-rw-   0        0        0    14957 2023-07-25 00:55:45.000000 kivygo-0.0.5/kivygo/colors.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:21:17.709910 kivygo-0.0.5/kivygo/config/
+-rw-rw-rw-   0        0        0      296 2023-04-30 03:08:38.000000 kivygo-0.0.5/kivygo/config/coins.atlas
+-rw-rw-rw-   0        0        0     4765 2023-04-29 21:48:35.000000 kivygo-0.0.5/kivygo/config/coins.bounds
+-rw-rw-rw-   0        0        0     1490 2013-02-26 10:24:28.000000 kivygo-0.0.5/kivygo/config/drugs.pex
+-rw-rw-rw-   0        0        0     1489 2013-02-26 10:24:28.000000 kivygo-0.0.5/kivygo/config/fire.pex
+-rw-rw-rw-   0        0        0     1496 2013-02-26 10:24:28.000000 kivygo-0.0.5/kivygo/config/jellyfish.pex
+-rw-rw-rw-   0        0        0     1463 2013-02-26 10:24:28.000000 kivygo-0.0.5/kivygo/config/particle.pex
+-rw-rw-rw-   0        0        0      870 2013-02-26 10:24:28.000000 kivygo-0.0.5/kivygo/config/particle.png
+-rw-rw-rw-   0        0        0     1494 2013-02-26 10:24:28.000000 kivygo-0.0.5/kivygo/config/sun.pex
+drwxrwxrwx   0        0        0        0 2023-07-27 01:21:17.712420 kivygo-0.0.5/kivygo/elevation/
+-rw-rw-rw-   0        0        0     1630 2023-01-06 02:24:33.000000 kivygo-0.0.5/kivygo/elevation/elevation.frag
+-rw-rw-rw-   0        0        0      198 2023-01-06 02:24:33.000000 kivygo-0.0.5/kivygo/elevation/header.frag
+-rw-rw-rw-   0        0        0      184 2023-01-06 02:24:33.000000 kivygo-0.0.5/kivygo/elevation/main.frag
+drwxrwxrwx   0        0        0        0 2023-07-27 01:21:17.736422 kivygo-0.0.5/kivygo/icons/
+-rw-rw-rw-   0        0        0   156742 2023-03-02 15:36:22.000000 kivygo-0.0.5/kivygo/icons/bg_example.png
+-rw-rw-rw-   0        0        0    95465 2022-05-23 02:23:22.000000 kivygo-0.0.5/kivygo/icons/coins.png
+-rw-rw-rw-   0        0        0     1244 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/discord.svg
+-rw-rw-rw-   0        0        0      781 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/discord2.svg
+-rw-rw-rw-   0        0        0      705 2023-07-15 18:38:14.000000 kivygo-0.0.5/kivygo/icons/facebook2.svg
+-rw-rw-rw-   0        0        0     2453 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/github.svg
+-rw-rw-rw-   0        0        0     1864 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/github2.svg
+-rw-rw-rw-   0        0        0      829 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/github3.svg
+-rw-rw-rw-   0        0        0     2451 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/google.svg
+-rw-rw-rw-   0        0        0      990 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/google3.svg
+-rw-rw-rw-   0        0        0     2636 2022-05-23 02:23:22.000000 kivygo-0.0.5/kivygo/icons/kivy.png
+-rw-rw-rw-   0        0        0     1141 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/kivy.svg
+-rw-rw-rw-   0        0        0    16577 2023-03-02 15:36:22.000000 kivygo-0.0.5/kivygo/icons/kivy_logo.png
+-rw-rw-rw-   0        0        0    42074 2021-05-11 19:10:56.000000 kivygo-0.0.5/kivygo/icons/kivymd_logo.png
+-rw-rw-rw-   0        0        0     2919 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/pie_chart.svg
+-rw-rw-rw-   0        0        0     1458 2023-02-14 20:11:52.000000 kivygo-0.0.5/kivygo/icons/pipette.png
+-rw-rw-rw-   0        0        0     1133 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/python2.svg
+-rw-rw-rw-   0        0        0     1621 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/search.svg
+-rw-rw-rw-   0        0        0      851 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/so.svg
+-rw-rw-rw-   0        0        0     1481 2022-05-23 02:23:22.000000 kivygo-0.0.5/kivygo/icons/square.png
+-rw-rw-rw-   0        0        0     1814 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/sublime.svg
+-rw-rw-rw-   0        0        0     3454 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/text.svg
+-rw-rw-rw-   0        0        0     1928 2023-02-14 20:11:52.000000 kivygo-0.0.5/kivygo/icons/transparent.png
+-rw-rw-rw-   0        0        0     1086 2021-06-29 07:37:30.000000 kivygo-0.0.5/kivygo/icons/twitter2.svg
+drwxrwxrwx   0        0        0        0 2023-07-27 01:21:17.749940 kivygo-0.0.5/kivygo/images/
+-rw-rw-rw-   0        0        0    27298 2023-07-13 23:39:27.000000 kivygo-0.0.5/kivygo/images/6915-green.png
+-rw-rw-rw-   0        0        0     5346 2023-07-14 00:55:12.000000 kivygo-0.0.5/kivygo/images/Path.png
+-rw-rw-rw-   0        0        0   709001 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/images/busan.jpg
+-rw-rw-rw-   0        0        0   118790 2018-10-01 10:52:31.000000 kivygo-0.0.5/kivygo/images/demoimage.jpg
+-rw-rw-rw-   0        0        0   190380 2023-04-28 21:56:31.000000 kivygo-0.0.5/kivygo/images/icon-kivygo.png
+-rw-rw-rw-   0        0        0   431598 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/images/iris.jpg
+-rw-rw-rw-   0        0        0   857961 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/images/lion.jpg
+-rw-rw-rw-   0        0        0      879 2019-05-19 13:30:15.000000 kivygo-0.0.5/kivygo/images/navigationdrawer_gradient_ltor.png
+-rw-rw-rw-   0        0        0      874 2019-05-19 13:30:15.000000 kivygo-0.0.5/kivygo/images/navigationdrawer_gradient_rtol.png
+-rw-rw-rw-   0        0        0  1537713 2023-02-14 20:11:52.000000 kivygo-0.0.5/kivygo/images/test.jpg
+drwxrwxrwx   0        0        0        0 2023-07-27 01:21:17.756933 kivygo-0.0.5/kivygo/layouts/
+-rw-rw-rw-   0        0        0        0 2023-05-10 21:23:48.000000 kivygo-0.0.5/kivygo/layouts/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-07-25 01:03:47.000000 kivygo-0.0.5/kivygo/layouts/anchorlayout.py
+-rw-rw-rw-   0        0        0      975 2023-07-20 20:12:06.000000 kivygo-0.0.5/kivygo/layouts/boxlayout.py
+-rw-rw-rw-   0        0        0     4644 2023-07-07 01:12:57.000000 kivygo-0.0.5/kivygo/layouts/circularlayout.py
+-rw-rw-rw-   0        0        0      747 2023-07-20 20:12:01.000000 kivygo-0.0.5/kivygo/layouts/floatlayout.py
+-rw-rw-rw-   0        0        0     5880 2023-07-24 00:48:06.000000 kivygo-0.0.5/kivygo/layouts/gridlayout.py
+-rw-rw-rw-   0        0        0     2334 2023-04-21 01:53:43.000000 kivygo-0.0.5/kivygo/transformations.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:21:17.814007 kivygo-0.0.5/kivygo/transitions/
+-rw-rw-rw-   0        0        0      452 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Angular.glsl
+-rw-rw-rw-   0        0        0      719 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Bounce.glsl
+-rw-rw-rw-   0        0        0     2593 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/BowTieHorizontal.glsl
+-rw-rw-rw-   0        0        0     2541 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/BowTieVertical.glsl
+-rw-rw-rw-   0        0        0      231 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Burn.glsl
+-rw-rw-rw-   0        0        0      948 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/ButterflyWaveScrawler.glsl
+-rw-rw-rw-   0        0        0      485 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/CannabisLeaf.glsl
+-rw-rw-rw-   0        0        0      398 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Circle.glsl
+-rw-rw-rw-   0        0        0      386 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/CircleOpen.glsl
+-rw-rw-rw-   0        0        0      370 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/ColorPhase.glsl
+-rw-rw-rw-   0        0        0      353 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/ColourDistance.glsl
+-rw-rw-rw-   0        0        0      586 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/CrazyParametricFun.glsl
+-rw-rw-rw-   0        0        0      590 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/CrossHatch.glsl
+-rw-rw-rw-   0        0        0      228 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/CrossWarp.glsl
+-rw-rw-rw-   0        0        0     2385 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/CrossZoom.glsl
+-rw-rw-rw-   0        0        0     1694 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Cube.glsl
+-rw-rw-rw-   0        0        0      352 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/DirectionalEasing.glsl
+-rw-rw-rw-   0        0        0      489 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/DirectionalWarp.glsl
+-rw-rw-rw-   0        0        0      557 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/DirectionalWipe.glsl
+-rw-rw-rw-   0        0        0      522 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Displacement.glsl
+-rw-rw-rw-   0        0        0     1574 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/DoomScreenTransition.glsl
+-rw-rw-rw-   0        0        0     1189 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Doorway.glsl
+-rw-rw-rw-   0        0        0      378 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Dreamy.glsl
+-rw-rw-rw-   0        0        0     1183 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/DreamyZoom.glsl
+-rw-rw-rw-   0        0        0      136 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Fade.glsl
+-rw-rw-rw-   0        0        0      391 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/FadeColor.glsl
+-rw-rw-rw-   0        0        0      546 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/FadeGrayscale.glsl
+-rw-rw-rw-   0        0        0     2220 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/FilmBurn.glsl
+-rw-rw-rw-   0        0        0      489 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/FlyEye.glsl
+-rw-rw-rw-   0        0        0     2198 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/GlitchDisplace.glsl
+-rw-rw-rw-   0        0        0      607 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/GlitchMemories.glsl
+-rw-rw-rw-   0        0        0     2245 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/GridFlip.glsl
+-rw-rw-rw-   0        0        0      356 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Heart.glsl
+-rw-rw-rw-   0        0        0     1663 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Hexagonalize.glsl
+-rw-rw-rw-   0        0        0      549 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Kaleidoscope.glsl
+-rw-rw-rw-   0        0        0      647 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/LeftRight.glsl
+-rw-rw-rw-   0        0        0      671 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/LinearBlur.glsl
+-rw-rw-rw-   0        0        0      226 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Luma.glsl
+-rw-rw-rw-   0        0        0     3781 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/LuminanceMelt.glsl
+-rw-rw-rw-   0        0        0      379 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Morph.glsl
+-rw-rw-rw-   0        0        0     1105 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Mosaic.glsl
+-rw-rw-rw-   0        0        0      339 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/MultiplyBlend.glsl
+-rw-rw-rw-   0        0        0     1390 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/PageCurl.glsl
+-rw-rw-rw-   0        0        0     1367 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Perlin.glsl
+-rw-rw-rw-   0        0        0      349 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Pinwheel.glsl
+-rw-rw-rw-   0        0        0      562 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Pixelize.glsl
+-rw-rw-rw-   0        0        0      452 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/PolarFunction.glsl
+-rw-rw-rw-   0        0        0      304 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/PolkaDotsCurtain.glsl
+-rw-rw-rw-   0        0        0      353 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Radial.glsl
+-rw-rw-rw-   0        0        0      444 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/RandomNoise.glsl
+-rw-rw-rw-   0        0        0      377 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/RandomSquares.glsl
+-rw-rw-rw-   0        0        0      356 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Ripple.glsl
+-rw-rw-rw-   0        0        0      832 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/RotateScaleFade.glsl
+-rw-rw-rw-   0        0        0      348 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/RotateTransition.glsl
+-rw-rw-rw-   0        0        0      365 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/SimpleZoom.glsl
+-rw-rw-rw-   0        0        0      742 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/SquaresWire.glsl
+-rw-rw-rw-   0        0        0      444 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Squeeze.glsl
+-rw-rw-rw-   0        0        0     8033 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/StereoViewer.glsl
+-rw-rw-rw-   0        0        0     1506 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Swap.glsl
+-rw-rw-rw-   0        0        0      715 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Swirl.glsl
+-rw-rw-rw-   0        0        0     4051 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/TangentMotionBlur.glsl
+-rw-rw-rw-   0        0        0      650 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/TopBottom.glsl
+-rw-rw-rw-   0        0        0     1366 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/UndulatingBurnOut.glsl
+-rw-rw-rw-   0        0        0      409 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/WaterDrop.glsl
+-rw-rw-rw-   0        0        0      386 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/Wind.glsl
+-rw-rw-rw-   0        0        0      274 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/WindowBlinds.glsl
+-rw-rw-rw-   0        0        0      277 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/WindowSlice.glsl
+-rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/WipeDown.glsl
+-rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/WipeLeft.glsl
+-rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/WipeRight.glsl
+-rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/WipeUp.glsl
+-rw-rw-rw-   0        0        0     1115 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/ZoomInCircles.glsl
+-rw-rw-rw-   0        0        0     8072 2023-05-01 19:46:08.000000 kivygo-0.0.5/kivygo/transitions/__init__.py
+-rw-rw-rw-   0        0        0     1197 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/base.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:21:17.816011 kivygo-0.0.5/kivygo/transitions/extra/
+-rw-rw-rw-   0        0        0      177 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/extra/footer.glsl
+-rw-rw-rw-   0        0        0      403 2021-05-13 08:40:19.000000 kivygo-0.0.5/kivygo/transitions/extra/header.glsl
+-rw-rw-rw-   0        0        0     3603 2023-07-15 18:15:32.000000 kivygo-0.0.5/kivygo/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:21:17.848035 kivygo-0.0.5/kivygo/widgets/
+-rw-rw-rw-   0        0        0        0 2023-05-10 21:23:48.000000 kivygo-0.0.5/kivygo/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3816 2023-07-20 18:49:32.000000 kivygo-0.0.5/kivygo/widgets/bezier.py
+-rw-rw-rw-   0        0        0     1700 2023-07-24 00:51:12.000000 kivygo-0.0.5/kivygo/widgets/button.py
+-rw-rw-rw-   0        0        0    12947 2023-07-15 18:58:04.000000 kivygo-0.0.5/kivygo/widgets/camera.py
+-rw-rw-rw-   0        0        0     7868 2023-07-19 01:43:26.000000 kivygo-0.0.5/kivygo/widgets/circular_bar.py
+-rw-rw-rw-   0        0        0    20737 2023-07-20 18:53:37.000000 kivygo-0.0.5/kivygo/widgets/circulardatetimepicker.py
+-rw-rw-rw-   0        0        0    26860 2023-07-19 01:47:04.000000 kivygo-0.0.5/kivygo/widgets/codeinput.py
+-rw-rw-rw-   0        0        0     1986 2023-07-20 18:54:42.000000 kivygo-0.0.5/kivygo/widgets/effect.py
+-rw-rw-rw-   0        0        0    21810 2023-07-22 01:27:47.000000 kivygo-0.0.5/kivygo/widgets/frostedglass.py
+-rw-rw-rw-   0        0        0     2392 2023-07-19 01:49:36.000000 kivygo-0.0.5/kivygo/widgets/gradient.py
+-rw-rw-rw-   0        0        0     1766 2023-07-19 01:49:52.000000 kivygo-0.0.5/kivygo/widgets/icon.py
+-rw-rw-rw-   0        0        0     2358 2023-07-19 01:50:31.000000 kivygo-0.0.5/kivygo/widgets/image.py
+-rw-rw-rw-   0        0        0    10988 2023-07-20 19:57:15.000000 kivygo-0.0.5/kivygo/widgets/input.py
+-rw-rw-rw-   0        0        0     9393 2023-07-20 18:57:27.000000 kivygo-0.0.5/kivygo/widgets/joystick.py
+-rw-rw-rw-   0        0        0    21864 2023-07-19 01:53:43.000000 kivygo-0.0.5/kivygo/widgets/kivyg_icon.py
+-rw-rw-rw-   0        0        0     9415 2023-07-25 00:58:12.000000 kivygo-0.0.5/kivygo/widgets/label.py
+-rw-rw-rw-   0        0        0    14049 2023-07-19 01:54:31.000000 kivygo-0.0.5/kivygo/widgets/navigationdrawer.py
+-rw-rw-rw-   0        0        0    18125 2023-07-19 01:55:32.000000 kivygo-0.0.5/kivygo/widgets/particle.py
+-rw-rw-rw-   0        0        0     4459 2023-07-19 01:55:55.000000 kivygo-0.0.5/kivygo/widgets/pizza_graph.py
+-rw-rw-rw-   0        0        0     2877 2023-07-15 18:58:04.000000 kivygo-0.0.5/kivygo/widgets/popup.py
+-rw-rw-rw-   0        0        0     6804 2023-07-19 01:57:08.000000 kivygo-0.0.5/kivygo/widgets/progressspinner.py
+-rw-rw-rw-   0        0        0     6819 2023-07-20 20:12:41.000000 kivygo-0.0.5/kivygo/widgets/radialslider.py
+-rw-rw-rw-   0        0        0    24350 2023-07-19 01:58:47.000000 kivygo-0.0.5/kivygo/widgets/rotabox.py
+-rw-rw-rw-   0        0        0     1952 2023-07-20 20:12:36.000000 kivygo-0.0.5/kivygo/widgets/screenmanager.py
+-rw-rw-rw-   0        0        0     3606 2023-07-19 01:58:09.000000 kivygo-0.0.5/kivygo/widgets/scrollview.py
+-rw-rw-rw-   0        0        0     4994 2023-07-19 01:58:47.000000 kivygo-0.0.5/kivygo/widgets/segment.py
+-rw-rw-rw-   0        0        0     2971 2023-07-20 19:02:44.000000 kivygo-0.0.5/kivygo/widgets/shader.py
+-rw-rw-rw-   0        0        0     5527 2023-07-19 02:02:19.000000 kivygo-0.0.5/kivygo/widgets/slider.py
+-rw-rw-rw-   0        0        0     4401 2023-07-19 02:02:30.000000 kivygo-0.0.5/kivygo/widgets/spinner.py
+-rw-rw-rw-   0        0        0    10556 2023-07-25 01:08:50.000000 kivygo-0.0.5/kivygo/widgets/tab.py
+-rw-rw-rw-   0        0        0    12728 2023-07-20 19:04:27.000000 kivygo-0.0.5/kivygo/widgets/taptargetview.py
+-rw-rw-rw-   0        0        0     6460 2023-07-20 19:05:57.000000 kivygo-0.0.5/kivygo/widgets/terminal.py
+-rw-rw-rw-   0        0        0     3213 2023-07-20 20:13:52.000000 kivygo-0.0.5/kivygo/widgets/widget.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:21:17.693904 kivygo-0.0.5/kivygo.egg-info/
+-rw-rw-rw-   0        0        0      192 2023-07-27 01:21:17.000000 kivygo-0.0.5/kivygo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5480 2023-07-27 01:21:17.000000 kivygo-0.0.5/kivygo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 01:21:17.000000 kivygo-0.0.5/kivygo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-07-27 01:21:17.000000 kivygo-0.0.5/kivygo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 01:21:17.000000 kivygo-0.0.5/kivygo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 01:21:17.850036 kivygo-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2126 2023-05-30 13:06:22.000000 kivygo-0.0.5/setup.py
```

### Comparing `kivygo-0.0.4/LICENSE.txt` & `kivygo-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/animation.py` & `kivygo-0.0.5/kivygo/animation.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/behaviors/button.py` & `kivygo-0.0.5/kivygo/behaviors/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 
 from kivy.properties import (
 	OptionProperty, ObjectProperty,
-	BooleanProperty, NumericProperty,
+	BooleanProperty, NumericProperty
 )
 
 from kivy.uix.widget import Widget
 from kivy.clock import Clock
 from kivy.config import Config
 from weakref import ref
 from time import time
-from kivy.app import App
 
 
-class ButtonBehavior(Widget):
+class GoButtonBehavior(Widget):
 
 	state = OptionProperty('normal', options=('normal', 'down'))
 	'''
 	The state is 'down' only when the button is currently touched/clicked,
 	otherwise its 'normal'.
 	'''
 
@@ -110,36 +109,33 @@
 			self.__state_event.cancel()
 			self.__state_event = None
 
 	def on_touch_down(self, touch):
 		if touch.is_mouse_scrolling:
 			return False
 		
-		if not self.collide_point(touch.x, touch.y):
+		if not self.collide_point(*touch.pos):
 			return False
 		
 		if self in touch.ud:
 			return False
 	
 		if self.collide_point(*touch.pos) and not self.disabled:
 			self.pressed = True
-			self.elev = self.down_elevation
-			self.dispatch("on_press")
+			self.elevation_setter()
+			self.dispatch('on_press')
 
 			if "label" in self.ids and self.do_text_shrink:
 				self.ids.label.font_size -= self.text_shrink_amount
 		
 		touch.grab(self)
 		touch.ud[self] = True
 		self.last_touch = touch
 		self.__touch_time = time()
 		self._do_press()
-
-		if App._running_app:
-			self.dispatch('on_press')
 		
 		return True
 
 	def on_touch_move(self, touch):
 		if touch.grab_current is self:
 			return True
 		
@@ -148,15 +144,15 @@
 		
 		return (self in touch.ud)
 
 	def on_touch_up(self, touch):
 		if touch.grab_current is not self:
 			return super().on_touch_up(touch)
 		
-		assert(self in touch.ud)
+		assert self in touch.ud
 		touch.ungrab(self)
 		self.last_touch = touch
 
 		if (not self.always_release and
 				not self.collide_point(*touch.pos)):
 			self._do_release()
 			return None
@@ -172,16 +168,14 @@
 		touchtime = time() - self.__touch_time
 		if touchtime < self.min_state_time:
 			self.__state_event = Clock.schedule_once(
 				self._do_release, self.min_state_time - touchtime)
 		else:
 			self._do_release()
 		
-		if App._running_app:
-			self.dispatch('on_release')
 		
 		return True
 
 	def trigger_action(self, duration=0.1):
 		'''Trigger whatever action(s) have been bound to the button by calling
 		both the on_press and on_release callbacks.
 
@@ -204,15 +198,15 @@
 		
 		if not duration:
 			trigger_release(0)
 		else:
 			Clock.schedule_once(trigger_release, duration)
 
 
-class ToggleButtonBehavior(ButtonBehavior):
+class GoToggleButtonBehavior(GoButtonBehavior):
 	
 	__groups = {}
 
 	group = ObjectProperty(None, allownone=True)
 	'''
 	Group of the button. If `None`, no group will be used (the button will be
 	independent). `group` must be a hashable object, like a string.
@@ -226,26 +220,26 @@
 	'''
 
 	def __init__(self, **kwargs):
 		self._previous_group = None
 		super().__init__(**kwargs)
 
 	def on_group(self, *largs):
-		groups = ToggleButtonBehavior.__groups
+		groups = GoToggleButtonBehavior.__groups
 		if self._previous_group:
 			group = groups[self._previous_group]
 			for item in group[:]:
 				if item() is self:
 					group.remove(item)
 					break
 		
 		group = self._previous_group = self.group
 		if group not in groups:
 			groups[group] = []
-		r = ref(self, ToggleButtonBehavior._clear_groups)
+		r = ref(self, GoToggleButtonBehavior._clear_groups)
 		groups[group].append(r)
 
 	def _release_group(self, current):
 		if self.group == None:
 			return None
 		
 		group = self.__groups[self.group]
@@ -271,15 +265,15 @@
 
 	def _do_release(self, *args):
 		pass
 
 	@staticmethod
 	def _clear_groups(wk):
 		# auto flush the element when the weak reference have been deleted
-		groups = ToggleButtonBehavior.__groups
+		groups = GoToggleButtonBehavior.__groups
 		for group in list(groups.values()):
 			if wk in group:
 				group.remove(wk)
 				break
 
 	@staticmethod
 	def get_widgets(groupname):
@@ -287,20 +281,20 @@
 		Return a list of the widgets contained in a specific group. If the
 		group doesn't exist, an empty list will be returned.
 		
 		.. note:
 			Always release the result of this method! Holding a reference to
 			any of these widgets can prevent them from being garbage collected.
 			If in doubt, do::
-				l = ToggleButtonBehavior.get_widgets('mygroup')
+				l = GoToggleButtonBehavior.get_widgets('mygroup')
 				# do your job
 				del l
 		
 		.. warning:
 			It's possible that some widgets that you have previously
 			deleted are still in the list. The garbage collector might need
 			to release other objects before flushing them.
 		'''
-		groups = ToggleButtonBehavior.__groups
+		groups = GoToggleButtonBehavior.__groups
 		if groupname not in groups:
 			return []
 		return [x() for x in groups[groupname] if x()][:]
```

### Comparing `kivygo-0.0.4/kivygo/behaviors/drag_and_drop.py` & `kivygo-0.0.5/kivygo/behaviors/drag_and_drop.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 from kivy.core.window import Window
 from kivy.metrics import dp
 from kivy.clock import Clock
 
 
 Builder.load_string("""
 
-<SpacerWidget>:
+<GoSpacerWidget>:
 	size_hint: [None, None]
 	size: [0, 0]
 	canvas:
 		Color:
 			rgba: self.outline_color
 		Line:
 			rectangle: [*self.pos, *self.size]
 			width: root.outline_width
 
-<PreviewWidget>:
+<GoPreviewWidget>:
 	size_hint: [None, None]
 	size: [0, 0]
 	canvas:
 		Color:
 			rgba: self.outline_color
 		Line:
 			rectangle: [\
@@ -49,27 +49,27 @@
 			pos: self.pos
 			size: self.size
 			texture: self.texture
 
 """)
 
 
-class SpacerWidget(Widget):
+class GoSpacerWidget(Widget):
 	outline_width = NumericProperty(dp(2))
 	outline_color = ColorProperty([1, 0, 0, 1])
 
 
-class PreviewWidget(Widget):
+class GoPreviewWidget(Widget):
 	texture = ObjectProperty(None)
 	outline_width = NumericProperty(dp(1.01))
 	outline_color = ColorProperty([1, 0, 0, 1])
 	background_color = ColorProperty([1, 1, 1, 1])
 
 
-class DraggableObjectBehavior(Widget):
+class GoDraggableObjectBehavior(Widget):
 
 	drag_cls = StringProperty('')
 
 	_drag_touch = None
 
 	drag_distance = NumericProperty(dp(10))
 
@@ -85,15 +85,15 @@
 
 	def __init__(self, **kwargs):
 		super().__init__(**kwargs)
 		Clock.schedule_once(self.start)
 	
 	def start(self, *args):
 		if self.preview_widget == None:
-			self.preview_widget = PreviewWidget()
+			self.preview_widget = GoPreviewWidget()
 
 	def _touch_uid(self):
 		return '{}.{}'.format(self.__class__.__name__, self.uid)
 
 	def on_touch_down(self, touch):
 		uid = self._touch_uid()
 		if uid in touch.ud:
@@ -210,24 +210,24 @@
 		"""Removes the drag widget preview.
 		"""
 		self.preview_pixels = None
 		if self.preview_widget.parent:
 			self.preview_widget.parent.remove_widget(self.preview_widget)
 
 
-class DraggableLayoutBehavior(Widget):
+class GoDraggableLayoutBehavior(Widget):
 
 	spacer_widget = ObjectProperty(None)
 
 	drag_classes = ListProperty([])
 
 	drag_append_end = BooleanProperty(False)
 
 	def __init__(self, *args, **kwargs):
-		self.spacer_widget = SpacerWidget()
+		self.spacer_widget = GoSpacerWidget()
 		super().__init__(*args, **kwargs)
 
 	def _touch_uid(self):
 		return '{}.{}'.format(self.__class__.__name__, self.uid)
 
 	def compare_pos_to_widget(self, widget, pos):
 		return 'before'
```

### Comparing `kivygo-0.0.4/kivygo/behaviors/hover.py` & `kivygo-0.0.5/kivygo/behaviors/hover.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """
 To use this class, you must define two methods for it:
-:attr:`HoverBehavior.on_cursor_enter` and :attr:`HoverBehavior.on_cursor_leave`,
+:attr:`GoHoverBehavior.on_cursor_enter` and :attr:`GoHoverBehavior.on_cursor_leave`,
 which will be automatically called when the mouse cursor is over the widget
 and when the mouse cursor goes beyond the widget.
 
 .. note::
 
-	:class:`~HoverBehavior` will by default check to see if the current Widget is visible
+	:class:`~GoHoverBehavior` will by default check to see if the current Widget is visible
 	(i.e. not covered by a modal or popup and not a part of a Relative Layout, MDTab or Carousel
 	that is not currently visible etc) and will only issue events if the widget is visible.
 
 	To get the legacy behavior that the events are always triggered, you can set `detect_visible
 	on the Widget to `False`.
 
 """
+from kivygo.app import GoApp
 from kivy.uix.widget import Widget
 from kivy.core.window import Window
+from kivy.metrics import dp
 from kivy.properties import (
 	BooleanProperty, ObjectProperty,
 	ListProperty
 )
 
 
-class HoverBehavior(Widget):
+class GoHoverBehavior(Widget):
 
 	hovering = BooleanProperty(False)
 	"""
 	`True`, if the mouse cursor is within the borders of the widget.
 
 	Note that this is set and cleared even if the widget is not visible
 	"""
@@ -46,92 +48,86 @@
 	"""
 	Should this widget perform the visibility check?
 	"""
 
 	cursor_pos = ListProperty([0, 0])
 	repeat_callback = BooleanProperty(False)
 
-	_last_parent = ObjectProperty(None)
 	__resizes = []
 
 
 	def on_cursor_enter(self, *args):
 		"""Called when mouse enters the bbox of the widget AND the widget is visible."""
 		pass
 
 	def on_cursor_leave(self, *args):
 		"""Called when the mouse exits the widget AND the widget is visible."""
 		pass
 
+	def on_window_cursor_leave(self, *args):
+		pass
 
 	def __init__(self, **kwargs):
 		super().__init__(**kwargs)
-
+		
 		self.register_event_type("on_cursor_enter")
 		self.register_event_type("on_cursor_leave")
-
-		if not HoverBehavior.__resizes:
+		self.register_event_type("on_window_cursor_leave")
+		
+		if not GoHoverBehavior.__resizes:
 			Window.bind(mouse_pos=self.on_mouse_update)
 			Window.bind(on_cursor_leave=self.window_cursor_leave)
 		
-		HoverBehavior.__resizes.append(self)
+		GoHoverBehavior.__resizes.append(self)
 
 	def on_parent(self, *args):
-		if self.parent != None:
-			self._last_parent = self.parent
 		
-		if self.parent == None and HoverBehavior.__resizes:
-			if HoverBehavior.__resizes[0] is self:
+		if self.parent == None and GoHoverBehavior.__resizes:
+			if GoHoverBehavior.__resizes[0] is self:
 				Window.unbind(mouse_pos=self.on_mouse_update)
 				Window.unbind(on_cursor_leave=self.window_cursor_leave)
-				del HoverBehavior.__resizes[0]
+				del GoHoverBehavior.__resizes[0]
 				
-				if HoverBehavior.__resizes:
-					Window.bind(mouse_pos=HoverBehavior.__resizes[0].on_mouse_pos)
-					Window.bind(on_cursor_leave=HoverBehavior.__resizes[0].window_cursor_leave)
+				if GoHoverBehavior.__resizes:
+					Window.bind(mouse_pos=GoHoverBehavior.__resizes[0].on_mouse_update)
+					Window.bind(on_cursor_leave=GoHoverBehavior.__resizes[0].window_cursor_leave)
 			else:
-				HoverBehavior.__resizes.remove(self)
-
-	def on_mouse_pos(self, *args):
-		pass
+				GoHoverBehavior.__resizes.remove(self)
 
 	def window_cursor_leave(self, *args):
-		for wid in HoverBehavior.__resizes:
+		for wid in GoHoverBehavior.__resizes:
 			if wid.hover_visible or wid.repeat_callback:
 				wid.do_cursor_leave()
 
+	def do_window_cursor_leave(self, *args):
+		self.hovering = False
+		self.enter_point = None
+		if self.hover_visible or self.repeat_callback:
+			self.hover_visible = False
+			self.dispatch("on_window_cursor_leave")
+
 	def do_cursor_leave(self, *args):
 		self.hovering = False
 		self.enter_point = None
 		if self.hover_visible or self.repeat_callback:
 			self.hover_visible = False
 			self.dispatch("on_cursor_leave")
 	
 	def do_cursor_enter(self, *args):
 		if self.hover_visible:
 			self.enter_point = self.cursor_pos
 			self.dispatch("on_cursor_enter")
 
-	def new_dispatch(self, *args):
-		"""
-			ARGS:
-			 `option`: 'leave' or 'enter'
-		"""
-		if not self.hovering:
-			self.dispatch("on_cursor_leave")
-		else:
-			self.dispatch("on_cursor_enter")
-
 	def on_mouse_update(self, *args):
-		if not self.get_root_window():
+		if GoApp.get_root_window() == None:
 			return None
-		
-		for wid in HoverBehavior.__resizes:
+
+		for wid in GoHoverBehavior.__resizes:
 			
-			pos = args[1]
+			pos = list(map(dp, args[1]))
 			wid.cursor_pos = pos
 			#  If widget not in the same position: on_exit event if needed
 			if not wid.collide_point(*wid.to_widget(*pos)):
 				wid.do_cursor_leave()
 				continue
 
 			# | The pointer is in the same position as the widget
```

### Comparing `kivygo-0.0.4/kivygo/behaviors/neumorph.py` & `kivygo-0.0.5/kivygo/behaviors/neumorph.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     ObjectProperty, ColorProperty,
 )
 from kivygo.utils import dec_2_rgb
 from PIL import Image, ImageDraw, ImageFilter
 from kivy.clock import Clock
 
 
-class NeuGlowCircular:
+class GoGlowCircular(Widget):
 
     glow_radius = NumericProperty(0)
     """
     Radius of the glow
 
     attr:`glow_radius` is an :class:`~kivy.properties.NumericProperty`
     and defaults to `0`.
```

### Comparing `kivygo-0.0.4/kivygo/behaviors/resizable.py` & `kivygo-0.0.5/kivygo/behaviors/resizable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,176 +1,175 @@
 
 
 from kivy.lang import Builder
 from kivy.uix.widget import Widget
-from kivygo.uix.image import ImageWithSVG
+from kivygo.widgets.image import GoImage
 
 from kivy.properties import (
 	ColorProperty, ListProperty, 
 	NumericProperty, StringProperty,
 	ObjectProperty
 )
 from kivy.metrics import dp
 from kivy.core.window import Window
 
 
 Builder.load_string("""
 
 
-<ResizableRectangleBord>:
+<GoRectangleResizableBord>:
 	size_hint: None, None
 	size: '8dp', '8dp'
 	radius: [sum(self.size)/2] * 4
 	mipmap: True
-	allow_strech: True
-	keep_ratio: False
+	fit_mode: "fill"
 	
 	canvas:
 		Clear
 		Color:
-			rgba: [0]*4 if self.image_source else root.line_color
+			rgba: [0]*4 if self.source else root.line_color
 		RoundedRectangle:
 			pos: [ ( self.x - self.outline_width ), ( self.y - self.outline_width ) ]
 			size: [ ( self.width + (self.outline_width*2) ), ( self.height + (self.outline_width*2) ) ]
 			radius: root.radius
 		Color:
-			rgba: [0]*4 if self.image_source else root.background_color
+			rgba: [0]*4 if self.source else root.background_color
 		RoundedRectangle:
 			pos: self.pos
 			size: self.size
 			radius: root.radius
 
 	canvas.after:
 		Color:
-			rgba: self.color if self.image_source else [0]*4
+			rgba: self.color if self.source else [0]*4
 		Rectangle:
 			texture: self.texture
 			pos: self.pos
 			size: self.size
 
 
-<ResizableLineBord>:
+<GoLineResizableBord>:
 	canvas:
 		Color:
 			rgba: self.color
 		Line:
 			width: dp(1)
 			points: self.points
 
 
-<ResizeSelectBehavior>:
-	ResizableLineBord: # TOP LINE
+<GoSelectResizableBehavior>:
+	GoLineResizableBord: # TOP LINE
 		id: top_line
 		color: root._top_line_color
 		points: [top_left_rect.right, root.top, top_right_rect.x, root.top]
 
-	ResizableLineBord: # BOTTOM LINE
+	GoLineResizableBord: # BOTTOM LINE
 		id: bottom_line
 		color: root._bottom_line_color
 		points: [bottom_left_rect.right, root.y, bottom_right_rect.x, root.y]
 
-	ResizableLineBord: # LEFT LINE
+	GoLineResizableBord: # LEFT LINE
 		id: left_line
 		color: root._left_line_color
 		points: [root.x, top_left_rect.y, root.x, bottom_left_rect.top]
 	
-	ResizableLineBord: # RIGHT LINE
+	GoLineResizableBord: # RIGHT LINE
 		id: right_line
 		color: root._right_line_color
 		points: [root.right, top_right_rect.y, root.right, bottom_right_rect.y]
 
 	
-	ResizableRectangleBord: # TOP LEFT RECTANGLE
+	GoRectangleResizableBord: # TOP LEFT RECTANGLE
 		id: top_left_rect
 		x: self.parent.x - (self.width/2)
 		y: self.parent.top - (self.height/2)
 		background_color: root._bord_background_color
 		line_color: root._bord_line_color
-		image_source: root.bord_icon_source
+		source: root.bord_icon_source
 		size: root.bord_size
 		
-	ResizableRectangleBord: # BOTTOM LEFT RECTANGLE
+	GoRectangleResizableBord: # BOTTOM LEFT RECTANGLE
 		id: bottom_left_rect
 		x: self.parent.x-(self.width/2)
 		y: self.parent.y-(self.height/2)
 		background_color: root._bord_background_color
 		line_color: root._bord_line_color
-		image_source: root.bord_icon_source
+		source: root.bord_icon_source
 		size: root.bord_size
 	
-	ResizableRectangleBord: # BOTTOM RIGHT RECTANGLE
+	GoRectangleResizableBord: # BOTTOM RIGHT RECTANGLE
 		id: bottom_right_rect
 		x: self.parent.right-(self.width/2)
 		y: self.parent.y-(self.height/2)
 		background_color: root._bord_background_color
 		line_color: root._bord_line_color
-		image_source: root.bord_icon_source
+		source: root.bord_icon_source
 		size: root.bord_size
 	
-	ResizableRectangleBord:  # TOP RIGHT RECTANGLE
+	GoRectangleResizableBord:  # TOP RIGHT RECTANGLE
 		id: top_right_rect
 		x: self.parent.right - (self.width/2)
 		y: self.parent.top - (self.height/2)
 		background_color: root._bord_background_color
 		line_color: root._bord_line_color
-		image_source: root.bord_icon_source
+		source: root.bord_icon_source
 		size: root.bord_size
 
-	ResizableRectangleBord:  # TOP CENTER RECTANGLE
+	GoRectangleResizableBord:  # TOP CENTER RECTANGLE
 		id: top_center_rect
 		x: self.parent.x + (self.parent.width/2) - (self.width/2)
 		y: self.parent.top - (self.height/2)
 		background_color: root._bord_background_color
 		line_color: root._bord_line_color
-		image_source: root.bord_icon_source
+		source: root.bord_icon_source
 		size: root.bord_size
 	
-	ResizableRectangleBord:  # LEFT CENTER RECTANGLE
+	GoRectangleResizableBord:  # LEFT CENTER RECTANGLE
 		id: left_center_rect
 		x: self.parent.x - (self.width/2)
 		y: self.parent.y + (self.parent.height/2) - (self.height/2)
 		background_color: root._bord_background_color
 		line_color: root._bord_line_color
-		image_source: root.bord_icon_source
+		source: root.bord_icon_source
 		size: root.bord_size
 
-	ResizableRectangleBord:  # RIGHT CENTER RECTANGLE
+	GoRectangleResizableBord:  # RIGHT CENTER RECTANGLE
 		id: right_center_rect
 		x: self.parent.right - (self.width/2)
 		y: self.parent.y + (self.parent.height/2) - (self.height/2)
 		background_color: root._bord_background_color
 		line_color: root._bord_line_color
-		image_source: root.bord_icon_source
+		source: root.bord_icon_source
 		size: root.bord_size
 
-	ResizableRectangleBord:  # BOTTOM CENTER RECTANGLE
+	GoRectangleResizableBord:  # BOTTOM CENTER RECTANGLE
 		id: bottom_center_rect
 		x: self.parent.x + (self.parent.width/2) - (self.width/2)
 		y: self.parent.y - (self.height/2)
 		background_color: root._bord_background_color
 		line_color: root._bord_line_color
-		image_source: root.bord_icon_source
+		source: root.bord_icon_source
 		size: root.bord_size
 
 """)
 
 
-class ResizableRectangleBord(ImageWithSVG):
+class GoRectangleResizableBord(GoImage):
 	outline_width = NumericProperty(dp(2))
 	radius = ListProperty([0, 0, 0, 0])
 	background_color = ColorProperty("#FFFFFF")
 	line_color = ColorProperty("#25d2a2")
 
 
-class ResizableLineBord(Widget):
+class GoLineResizableBord(Widget):
 	color = ColorProperty("red")
 	points = ListProperty([0, 0])
 
 
-class ResizeSelectBehavior(Widget):
+class GoSelectResizableBehavior(Widget):
 
 	top_line_color = ColorProperty("#25d2a2")
 	bottom_line_color = ColorProperty("#25d2a2")
 	left_line_color = ColorProperty("#25d2a2")
 	right_line_color = ColorProperty("#25d2a2")
 
 	_top_line_color = ColorProperty("#25d2a2")
@@ -187,53 +186,49 @@
 	bord_size = ListProperty([dp(8), dp(8)])
 	line_color = ColorProperty([0, 0, 0, 0])
 	line_highlight_color = ColorProperty("#12715e")
 
 	last_touch_pos = (0, 0)
 
 	__resizes = []
-	_last_parent = ObjectProperty(None)
 	change_pos_varible = StringProperty("pos")
 	moved = 0
 	touched = 0
 	_in_resize = False
 
 
 	def __init__(self, **kwargs):
 		super().__init__(**kwargs)
 		self.selected_side = None
 
-		if not ResizeSelectBehavior.__resizes:
+		if not GoSelectResizableBehavior.__resizes:
 			Window.bind(mouse_pos=self.on_mouse_pos)
-		ResizeSelectBehavior.__resizes.append(self)
+		GoSelectResizableBehavior.__resizes.append(self)
 
 		self.bind(
 			on_top_line_color=self._set_default_colors,
 			on_bottom_line_color=self._set_default_colors,
 			on_left_line_color=self._set_default_colors,
 			on_right_line_color=self._set_default_colors,
 
 			on_bord_background_color=self._set_default_colors,
 			on_bord_line_color=self._set_default_colors
 		)
 		self._set_default_colors()
 	
 	def on_parent(self, *args):
-		if self.parent != None:
-			self._last_parent = self.parent
-		
-		if self.parent == None and ResizeSelectBehavior.__resizes:
-			if ResizeSelectBehavior.__resizes[0] is self:
+		if self.parent == None and GoSelectResizableBehavior.__resizes:
+			if GoSelectResizableBehavior.__resizes[0] is self:
 				Window.unbind(mouse_pos=self.on_mouse_pos)
-				del ResizeSelectBehavior.__resizes[0]
+				del GoSelectResizableBehavior.__resizes[0]
 				
-				if ResizeSelectBehavior.__resizes:
-					Window.bind(mouse_pos=ResizeSelectBehavior.__resizes[0].on_mouse_pos)
+				if GoSelectResizableBehavior.__resizes:
+					Window.bind(mouse_pos=GoSelectResizableBehavior.__resizes[0].on_mouse_pos)
 			else:
-				ResizeSelectBehavior.__resizes.remove(self)
+				GoSelectResizableBehavior.__resizes.remove(self)
 
 
 	def _set_default_colors(self, *args):
 		if self._in_resize:
 			self._top_line_color = self.top_line_color
 			self._bottom_line_color = self.bottom_line_color
 			self._left_line_color = self.left_line_color
@@ -257,15 +252,15 @@
 		self.right_line_color = self.line_color
 
 	def on_mouse_pos(self, window, touch):
 		"""
 		When the mouse moves, we check the position of the mouse
 		and update the cursor accordingly.
 		"""
-		for wid in ResizeSelectBehavior.__resizes:
+		for wid in GoSelectResizableBehavior.__resizes:
 			if wid.collide_point(*wid.to_widget(*touch)):
 				collision = wid.collides_with_control_points(wid.to_widget(*touch))
 				if collision in ["top left", "bottom right"]:
 					Window.set_system_cursor("size_nwse")
 				elif collision in ["top right", "bottom left"]:
 					Window.set_system_cursor("size_nesw")
 				elif collision in ["top", "bottom"]:
```

### Comparing `kivygo-0.0.4/kivygo/behaviors/thumb.py` & `kivygo-0.0.5/kivygo/behaviors/thumb.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 from kivy.graphics import (
     Color, Ellipse,
     StencilPop, StencilPush,
     StencilUnUse, StencilUse,
 )
 
 from kivygo.utils import root_path, do_correction_path
-from kivygo.behaviors.button import ToggleButtonBehavior
+from kivygo.behaviors.button import GoToggleButtonBehavior
 
 
-class CommonRipple():
+class GoCommonRipple(Widget):
 
     ripple_rad_default = NumericProperty(1)
     """The starting value of the radius of the ripple effect.
     """
 
     ripple_color = ColorProperty(None)
     """Ripple color in (r, g, b, a) format.
@@ -65,15 +65,15 @@
     """Type of animation for ripple out effect.
     """
 
     _ripple_rad = NumericProperty()
     _doing_ripple = BooleanProperty(False)
     _finishing_ripple = BooleanProperty(False)
     _fading_out = BooleanProperty(False)
-    _no_ripple_effect = BooleanProperty(False)
+    _no_effect = BooleanProperty(False)
     _round_rad = ListProperty([0, 0, 0, 0])
 
     def lay_canvas_instructions(self):
         raise NotImplementedError
 
     def start_ripple(self) -> None:
         if not self._doing_ripple:
@@ -131,15 +131,15 @@
             return False
         
         if not self.collide_point(touch.x, touch.y):
             return False
         
         if not self.disabled:
             self.call_ripple_animation_methods(touch)
-            if isinstance(self, ToggleButtonBehavior):
+            if isinstance(self, GoToggleButtonBehavior):
                 return super().on_touch_down(touch)
             else:
                 return True
 
     def call_ripple_animation_methods(self, touch) -> None:
         if self._doing_ripple:
             Animation.cancel_all(
@@ -182,22 +182,22 @@
     def _set_ellipse(self, instance, value):
         self.ellipse.size = (self._ripple_rad, self._ripple_rad)
 
     def _set_color(self, instance, value):
         self.col_instruction.a = value[3]
 
 
-class CircularRippleBehavior(CommonRipple):
+class CircularRippleBehavior(GoCommonRipple):
 
     ripple_scale = NumericProperty(1)
-    """See :class:`~CommonRipple.ripple_scale`.
+    """See :class:`~GoCommonRipple.ripple_scale`.
     """
 
     def lay_canvas_instructions(self) -> None:
-        if self._no_ripple_effect:
+        if self._no_effect:
             return None
 
         with self.canvas.after if self.ripple_canvas_after else self.canvas.before:
             StencilPush(group="circular_ripple_behavior")
             self.stencil = Ellipse(
                 size=[n * self.ripple_scale for n in self.size],
                 pos=(
@@ -234,15 +234,15 @@
 
         self.ellipse.pos = (
             self.center_x - self._ripple_rad / 2.0,
             self.center_y - self._ripple_rad / 2.0,
         )
 
 
-class CommonElevationBehavior(Widget):
+class GoCommonElevationBehavior(Widget):
 
     elevation = BoundedNumericProperty(0, min=0, errorvalue=0)
     """Elevation of the widget.
     """
 
     shadow_radius = VariableListProperty([0], length=4)
     """Radius of the corners of the shadow.
@@ -426,15 +426,15 @@
             self._shadow_color = self.shadow_color[:-1] + [float(self.opacity)]
 
         self.on_shadow_color(self, self._shadow_color)
         self.on_size()
         self.on_pos()
 
 
-class Thumb(CommonElevationBehavior, CircularRippleBehavior, FloatLayout):
+class GoThumb(GoCommonElevationBehavior, CircularRippleBehavior, FloatLayout):
     def _set_ellipse(self, instance, value):
         self.ellipse.size = (self._ripple_rad, self._ripple_rad)
         if self.ellipse.size[0] > self.width * 1.5 and not self._fading_out:
             self.fade_out()
         self.ellipse.pos = (
             self.center_x - self._ripple_rad / 2.0,
             self.center_y - self._ripple_rad / 2.0,
```

### Comparing `kivygo-0.0.4/kivygo/bounds_math.py` & `kivygo-0.0.5/kivygo/bounds_math.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 					j3 = j2 + 1
 
 				v30 = t_pts[j]
 				v31 = t_pts[j1]
 				v40 = t_pts[j2]
 				v41 = t_pts[j3]
 
-				# Segment intersection detection method:
+				# GoSegment intersection detection method:
 				# If the vertices v1 and v2 are not on opposite sides of the
 				# segment v3, v4, or the vertices v3 and v4 are not on
 				# opposite sides of the segment v1, v2, there's no
 				# intersection.
 				if ((v40 - v30) * (v11 - v31) - (v10 - v30) * (v41 - v31) > 0) == \
 						((v40 - v30) * (v21 - v31) - (v20 - v30) * (v41 - v31) > 0):
 					continue
@@ -196,15 +196,15 @@
 						j2 = j - t_off
 						j3 = j2 + 1
 					v30 = t_pts[j]
 					v31 = t_pts[j1]
 					v40 = t_pts[j2]
 					v41 = t_pts[j3]
 
-					# Segment intersection detection method:
+					# GoSegment intersection detection method:
 					# If the vertices v1 and v2 are not on opposite sides of
 					# the segment v3, v4, or the vertices v3 and v4 are not
 					# on opposite sides of the segment v1, v2, there's no
 					# intersection.
 					if ((v40 - v30) * (v11 - v31) - (v10 - v30) * (v41 - v31) > 0) == \
 							((v40 - v30) * (v21 - v31) - (v20 - v30) * (v41 - v31) > 0):
 						continue
@@ -285,15 +285,15 @@
 						j3 = j2 + 1
 
 					v30 = t_pts[j]
 					v31 = t_pts[j1]
 					v40 = t_pts[j2]
 					v41 = t_pts[j3]
 
-					# Segment intersection detection method:
+					# GoSegment intersection detection method:
 					# If the vertices v1 and v2 are not on opposite sides of
 					# the segment v3, v4, or the vertices v3 and v4 are not
 					# on opposite sides of the segment v1, v2, there's no
 					# intersection.
 					if ((v40 - v30) * (v11 - v31) - (v10 - v30) * (v41 - v31) > 0) == \
 							((v40 - v30) * (v21 - v31) - (v20 - v30) * (v41 - v31) > 0):
 						continue
```

### Comparing `kivygo-0.0.4/kivygo/config/coins.bounds` & `kivygo-0.0.5/kivygo/config/coins.bounds`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/config/drugs.pex` & `kivygo-0.0.5/kivygo/config/drugs.pex`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/config/fire.pex` & `kivygo-0.0.5/kivygo/config/fire.pex`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/config/jellyfish.pex` & `kivygo-0.0.5/kivygo/config/jellyfish.pex`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/config/particle.pex` & `kivygo-0.0.5/kivygo/config/particle.pex`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/config/particle.png` & `kivygo-0.0.5/kivygo/config/particle.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/config/sun.pex` & `kivygo-0.0.5/kivygo/config/sun.pex`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/elevation/elevation.frag` & `kivygo-0.0.5/kivygo/elevation/elevation.frag`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/bg_example.png` & `kivygo-0.0.5/kivygo/icons/bg_example.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/coins.png` & `kivygo-0.0.5/kivygo/icons/coins.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/discord.svg` & `kivygo-0.0.5/kivygo/icons/discord.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/discord2.svg` & `kivygo-0.0.5/kivygo/icons/discord2.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/facebook2.svg` & `kivygo-0.0.5/kivygo/icons/facebook2.svg`

 * *Files 0% similar despite different names*

```diff
@@ -20,25 +20,26 @@
 00000130: 6965 6e74 3e0a 3c70 6174 6820 6669 6c6c  ient>.<path fill
 00000140: 3d22 2332 6161 3466 3422 2064 3d22 4d32  ="#2aa4f4" d="M2
 00000150: 342c 3443 3132 2e39 3534 2c34 2c34 2c31  4,4C12.954,4,4,1
 00000160: 322e 3935 342c 342c 3234 7338 2e39 3534  2.954,4,24s8.954
 00000170: 2c32 302c 3230 2c32 3073 3230 2d38 2e39  ,20,20,20s20-8.9
 00000180: 3534 2c32 302d 3230 5333 352e 3034 362c  54,20-20S35.046,
 00000190: 342c 3234 2c34 7a22 2f3e 0a3c 7061 7468  4,24,4z"/>.<path
-000001a0: 2066 696c 6c3d 2223 6666 6666 6622 2064   fill="#fffff" d
-000001b0: 3d22 4d32 362e 3730 372c 3239 2e33 3031  ="M26.707,29.301
-000001c0: 6835 2e31 3736 6c30 2e38 3133 2d35 2e32  h5.176l0.813-5.2
-000001d0: 3538 682d 352e 3938 3976 2d32 2e38 3734  58h-5.989v-2.874
-000001e0: 6330 2d32 2e31 3834 2c30 2e37 3134 2d34  c0-2.184,0.714-4
-000001f0: 2e31 3231 2c32 2e37 3537 2d34 2e31 3231  .121,2.757-4.121
-00000200: 6833 2e32 3833 5631 322e 3436 2063 2d30  h3.283V12.46 c-0
-00000210: 2e35 3737 2d30 2e30 3738 2d31 2e37 3937  .577-0.078-1.797
-00000220: 2d30 2e32 3438 2d34 2e31 3032 2d30 2e32  -0.248-4.102-0.2
-00000230: 3438 632d 342e 3831 342c 302d 372e 3633  48c-4.814,0-7.63
-00000240: 362c 322e 3534 322d 372e 3633 362c 382e  6,2.542-7.636,8.
-00000250: 3333 3476 332e 3439 3848 3136 2e30 3676  334v3.498H16.06v
-00000260: 352e 3235 3868 342e 3934 3876 3134 2e34  5.258h4.948v14.4
-00000270: 3532 2043 3231 2e39 3838 2c34 332e 392c  52 C21.988,43.9,
-00000280: 3232 2e39 3831 2c34 342c 3234 2c34 3463  22.981,44,24,44c
-00000290: 302e 3932 312c 302c 312e 3832 2d30 2e30  0.921,0,1.82-0.0
-000002a0: 3834 2c32 2e37 3037 2d30 2e32 3034 5632  84,2.707-0.204V2
-000002b0: 392e 3330 317a 222f 3e0a 3c2f 7376 673e  9.301z"/>.</svg>
+000001a0: 2066 696c 6c3d 2223 6666 6666 6666 2220   fill="#ffffff" 
+000001b0: 643d 224d 3236 2e37 3037 2c32 392e 3330  d="M26.707,29.30
+000001c0: 3168 352e 3137 366c 302e 3831 332d 352e  1h5.176l0.813-5.
+000001d0: 3235 3868 2d35 2e39 3839 762d 322e 3837  258h-5.989v-2.87
+000001e0: 3463 302d 322e 3138 342c 302e 3731 342d  4c0-2.184,0.714-
+000001f0: 342e 3132 312c 322e 3735 372d 342e 3132  4.121,2.757-4.12
+00000200: 3168 332e 3238 3356 3132 2e34 3620 632d  1h3.283V12.46 c-
+00000210: 302e 3537 372d 302e 3037 382d 312e 3739  0.577-0.078-1.79
+00000220: 372d 302e 3234 382d 342e 3130 322d 302e  7-0.248-4.102-0.
+00000230: 3234 3863 2d34 2e38 3134 2c30 2d37 2e36  248c-4.814,0-7.6
+00000240: 3336 2c32 2e35 3432 2d37 2e36 3336 2c38  36,2.542-7.636,8
+00000250: 2e33 3334 7633 2e34 3938 4831 362e 3036  .334v3.498H16.06
+00000260: 7635 2e32 3538 6834 2e39 3438 7631 342e  v5.258h4.948v14.
+00000270: 3435 3220 4332 312e 3938 382c 3433 2e39  452 C21.988,43.9
+00000280: 2c32 322e 3938 312c 3434 2c32 342c 3434  ,22.981,44,24,44
+00000290: 6330 2e39 3231 2c30 2c31 2e38 322d 302e  c0.921,0,1.82-0.
+000002a0: 3038 342c 322e 3730 372d 302e 3230 3456  084,2.707-0.204V
+000002b0: 3239 2e33 3031 7a22 2f3e 0a3c 2f73 7667  29.301z"/>.</svg
+000002c0: 3e                                       >
```

### Comparing `kivygo-0.0.4/kivygo/icons/github.svg` & `kivygo-0.0.5/kivygo/icons/github.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/github2.svg` & `kivygo-0.0.5/kivygo/icons/github2.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/github3.svg` & `kivygo-0.0.5/kivygo/icons/github3.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/google.svg` & `kivygo-0.0.5/kivygo/icons/google.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/google3.svg` & `kivygo-0.0.5/kivygo/icons/google3.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/kivy.png` & `kivygo-0.0.5/kivygo/icons/kivy.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/kivy.svg` & `kivygo-0.0.5/kivygo/icons/kivy.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/kivy_logo.png` & `kivygo-0.0.5/kivygo/icons/kivy_logo.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/kivymd_logo.png` & `kivygo-0.0.5/kivygo/icons/kivymd_logo.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/pie_chart.svg` & `kivygo-0.0.5/kivygo/icons/pie_chart.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/pipette.png` & `kivygo-0.0.5/kivygo/icons/pipette.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/python2.svg` & `kivygo-0.0.5/kivygo/icons/python2.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/search.svg` & `kivygo-0.0.5/kivygo/icons/search.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/so.svg` & `kivygo-0.0.5/kivygo/icons/so.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/square.png` & `kivygo-0.0.5/kivygo/icons/square.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/sublime.svg` & `kivygo-0.0.5/kivygo/icons/sublime.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/text.svg` & `kivygo-0.0.5/kivygo/icons/text.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/transparent.png` & `kivygo-0.0.5/kivygo/icons/transparent.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/icons/twitter2.svg` & `kivygo-0.0.5/kivygo/icons/twitter2.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/images/busan.jpg` & `kivygo-0.0.5/kivygo/images/busan.jpg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/images/demoimage.jpg` & `kivygo-0.0.5/kivygo/images/demoimage.jpg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/images/icon-kivygo.png` & `kivygo-0.0.5/kivygo/images/icon-kivygo.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/images/iris.jpg` & `kivygo-0.0.5/kivygo/images/iris.jpg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/images/lion.jpg` & `kivygo-0.0.5/kivygo/images/lion.jpg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/images/navigationdrawer_gradient_ltor.png` & `kivygo-0.0.5/kivygo/images/navigationdrawer_gradient_ltor.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/images/navigationdrawer_gradient_rtol.png` & `kivygo-0.0.5/kivygo/images/navigationdrawer_gradient_rtol.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/images/test.jpg` & `kivygo-0.0.5/kivygo/images/test.jpg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transformations.py` & `kivygo-0.0.5/kivygo/transformations.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/Bounce.glsl` & `kivygo-0.0.5/kivygo/transitions/Bounce.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/BowTieHorizontal.glsl` & `kivygo-0.0.5/kivygo/transitions/BowTieHorizontal.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/BowTieVertical.glsl` & `kivygo-0.0.5/kivygo/transitions/BowTieVertical.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/ButterflyWaveScrawler.glsl` & `kivygo-0.0.5/kivygo/transitions/ButterflyWaveScrawler.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/CrazyParametricFun.glsl` & `kivygo-0.0.5/kivygo/transitions/CrazyParametricFun.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/CrossHatch.glsl` & `kivygo-0.0.5/kivygo/transitions/CrossHatch.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/CrossZoom.glsl` & `kivygo-0.0.5/kivygo/transitions/CrossZoom.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/Cube.glsl` & `kivygo-0.0.5/kivygo/transitions/Cube.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/DirectionalWipe.glsl` & `kivygo-0.0.5/kivygo/transitions/DirectionalWipe.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/Displacement.glsl` & `kivygo-0.0.5/kivygo/transitions/Displacement.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/DoomScreenTransition.glsl` & `kivygo-0.0.5/kivygo/transitions/DoomScreenTransition.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/Doorway.glsl` & `kivygo-0.0.5/kivygo/transitions/Doorway.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/DreamyZoom.glsl` & `kivygo-0.0.5/kivygo/transitions/DreamyZoom.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/FadeGrayscale.glsl` & `kivygo-0.0.5/kivygo/transitions/FadeGrayscale.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/FilmBurn.glsl` & `kivygo-0.0.5/kivygo/transitions/FilmBurn.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/GlitchDisplace.glsl` & `kivygo-0.0.5/kivygo/transitions/GlitchDisplace.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/GlitchMemories.glsl` & `kivygo-0.0.5/kivygo/transitions/GlitchMemories.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/GridFlip.glsl` & `kivygo-0.0.5/kivygo/transitions/GridFlip.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/Hexagonalize.glsl` & `kivygo-0.0.5/kivygo/transitions/Hexagonalize.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/Kaleidoscope.glsl` & `kivygo-0.0.5/kivygo/transitions/Kaleidoscope.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/LeftRight.glsl` & `kivygo-0.0.5/kivygo/transitions/LeftRight.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/LinearBlur.glsl` & `kivygo-0.0.5/kivygo/transitions/LinearBlur.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/LuminanceMelt.glsl` & `kivygo-0.0.5/kivygo/transitions/LuminanceMelt.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/Mosaic.glsl` & `kivygo-0.0.5/kivygo/transitions/Mosaic.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/PageCurl.glsl` & `kivygo-0.0.5/kivygo/transitions/PageCurl.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/Perlin.glsl` & `kivygo-0.0.5/kivygo/transitions/Perlin.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/Pixelize.glsl` & `kivygo-0.0.5/kivygo/transitions/Pixelize.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/RotateScaleFade.glsl` & `kivygo-0.0.5/kivygo/transitions/RotateScaleFade.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/SquaresWire.glsl` & `kivygo-0.0.5/kivygo/transitions/SquaresWire.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/StereoViewer.glsl` & `kivygo-0.0.5/kivygo/transitions/StereoViewer.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/Swap.glsl` & `kivygo-0.0.5/kivygo/transitions/Swap.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/Swirl.glsl` & `kivygo-0.0.5/kivygo/transitions/Swirl.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/TangentMotionBlur.glsl` & `kivygo-0.0.5/kivygo/transitions/TangentMotionBlur.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/TopBottom.glsl` & `kivygo-0.0.5/kivygo/transitions/TopBottom.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/UndulatingBurnOut.glsl` & `kivygo-0.0.5/kivygo/transitions/UndulatingBurnOut.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/ZoomInCircles.glsl` & `kivygo-0.0.5/kivygo/transitions/ZoomInCircles.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/__init__.py` & `kivygo-0.0.5/kivygo/transitions/__init__.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/transitions/base.py` & `kivygo-0.0.5/kivygo/transitions/base.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.4/kivygo/uix/androidtabs.py` & `kivygo-0.0.5/kivygo/widgets/tab.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,76 @@
 
 from kivy.lang import Builder
 from kivy.clock import Clock
 from kivy.uix.label import Label
-from kivy.uix.behaviors import ToggleButtonBehavior
-from kivy.uix.boxlayout import BoxLayout
-from kivy.uix.anchorlayout import AnchorLayout
-from kivy.uix.carousel import Carousel
-from kivy.uix.widget import Widget
+from kivygo.behaviors.button import GoToggleButtonBehavior
+from kivygo.layouts.boxlayout import GoBoxLayout
+from kivygo.layouts.anchorlayout import GoAnchorLayout
+from kivygo.widgets.widget import GoWidget
 from kivy.uix.scrollview import ScrollView
 from kivy.graphics import Rectangle
 from kivy.utils import boundary
 from kivy.properties import (
 	ObjectProperty, NumericProperty,
 	VariableListProperty, StringProperty,
 	AliasProperty, BooleanProperty,
-	BoundedNumericProperty, ListProperty
+	BoundedNumericProperty
 )
 
-from kivygo.behaviors.touch_effecs import EffectBehavior
-from kivygo.behaviors.hover import HoverBehavior
-
-
 Builder.load_string('''
 
 #:import DampedScrollEffect kivy.effects.dampedscroll.DampedScrollEffect
 
-<AndroidTabsBar>:
-	canvas.before: 
-		Color:
-			rgba: self._background_color
-		RoundedRectangle:
-			pos: self.pos
-			size: self.size
-			radius: self.radius
-	canvas.after:
-		Color:
-			rgba: self.stroke_color
-		Line:
-			rounded_rectangle: [*self.pos, *self.size, *self.radius]
-			width: self.stroke_width
+<GoTabBar>:
 
-<AndroidTabsLabel>:
+<GoTabLabel>:
 	size_hint: None, 1
 	halign: 'center'
-	padding: '12dp', 0
+	padding: ['12dp', 0]
 	group: 'tabs'
 	allow_no_selection: False
-	text_color_normal: 1, 1, 1, .6
-	text_color_active: 1, 1, 1, 1
-	color: self.text_color_active if self.state is 'down' \
-								else self.text_color_normal
+	text_color_normal: GoColors.text_default
+	text_color_active: GoColors.text_pressed
+	color: self.text_color_active if self.state == 'down' else self.text_color_normal
 	on_x: self._trigger_update_tab_indicator()
 	on_width: self._trigger_update_tab_indicator()
 
-<AndroidTabsScrollView>:
-	size_hint: 1, 1
+<GoTabScrollView>:
+	size_hint: [1, 1]
 	do_scroll_y: False
-	bar_color: 0, 0, 0, 0
-	bar_inactive_color: 0, 0, 0, 0
+	bar_color: GoColors.no_color
+	bar_inactive_color: GoColors.no_color
 	bar_width: 0
 	effect_cls: DampedScrollEffect
 
-<AndroidTabs>:
+<GoTab>:
 	carousel: carousel
 	tab_bar: tab_bar
 	anchor_y: 'top'
 
-	AndroidTabsMain:
-		padding: 0, tab_bar.height, 0, 0
+	GoBoxLayout:
+		padding: [0, tab_bar.height, 0, 0]
 
-		AndroidTabsCarousel:
+		Carousel:
 			id: carousel
 			anim_move_duration: root.anim_duration
 			on_index: root.on_carousel_index(*args)
 			on__offset: tab_bar.android_animation(*args)
 			on_slides: self.index = root.default_tab
 			on_slides: root.on_carousel_index(self, 0)
 
-	AndroidTabsBar:
+	GoTabBar:
 		id: tab_bar
 		carousel: carousel
 		scrollview: scrollview
 		layout: layout
 		size_hint: 1, None
 		height: root.tab_bar_height
 
-		AndroidTabsScrollView:
+		GoTabScrollView:
 			id: scrollview
 			on_width: tab_bar._trigger_update_tab_bar()
 
 			GridLayout:
 				id: layout
 				rows: 1
 				size_hint: None, 1
@@ -101,25 +82,25 @@
 						rgba: root.tab_indicator_color
 					Rectangle:
 						pos: self.pos
 						size: 0, root.tab_indicator_height
 ''')
 
 
-class AndroidTabsException(Exception):
+class GoTabException(Exception):
 	pass
 
 
-class AndroidTabsLabel(ToggleButtonBehavior, Label):
+class GoTabLabel(GoToggleButtonBehavior, Label):
 
-	text_color_normal = VariableListProperty([1, 1, 1, .6])
+	text_color_normal = VariableListProperty([0]*4)
 	'''Text color of the label when it is not selected.
 	'''
 
-	text_color_active = VariableListProperty([1])
+	text_color_active = VariableListProperty([0]*4)
 	'''Text color of the label when it is selected.
 	'''
 
 	tab = ObjectProperty(None)
 	tab_bar = ObjectProperty(None)
 
 	def __init__(self, **kwargs):
@@ -142,58 +123,46 @@
 	def _trigger_update_tab_indicator(self):
 		# update the position and size of the indicator
 		# when the label changes size or position
 		if self.state == 'down':
 			self.tab_bar.update_indicator(self.x, self.width)
 
 
-class AndroidTabsBase(Widget):
+class GoTabBase(GoWidget):
 
 	'''
-	AndroidTabsBase allow you to create a tab.
+	GoTabBase allow you to create a tab.
 	You must create a new class that inherits
-	from AndroidTabsBase.
+	from GoTabBase.
 	In this way you have total control over the
 	views of your tabbed panel.
 	'''
 
 	text = StringProperty('')
 	'''It will be the label text of the tab.
 	'''
 
 	tab_label = ObjectProperty(None)
 	'''It is the label object reference of the tab.
 	'''
 
 	def __init__(self, **kwargs):
 
-		self.tab_label = AndroidTabsLabel(tab=self)
+		self.tab_label = GoTabLabel(tab=self)
 		super().__init__(**kwargs)
 
 	def on_text(self, widget, text):
 		# set the label text
 		self.tab_label.text = self.text
 
 
-class AndroidTabsMain(BoxLayout):
-	'''
-	AndroidTabsMain is just a boxlayout that contain
-	the carousel. It allows you to have control over the carousel.
-	'''
-	pass
-
-
-class AndroidTabsCarousel(Carousel):
-	pass
-
-
-class AndroidTabsScrollView(ScrollView):
-	'''
-	AndroidTabsScrollView hacked version to fix scroll_x manual setting.
+class GoTabScrollView(ScrollView):
+	'''GoTabScrollView hacked version to fix scroll_x manual setting.
 	'''
+	
 	def goto(self, scroll_x, scroll_y):
 		''' Update event value along with scroll_*
 		'''
 		def _update(e, x):
 			if e:
 				e.value = (e.max + e.min) * x
 
@@ -202,32 +171,21 @@
 			_update(self.effect_x, scroll_x)
 
 		if not (scroll_y == None):
 			self.scroll_y = scroll_y
 			_update(self.effect_y, scroll_y)
 
 
-class AndroidTabsBar(BoxLayout, HoverBehavior, EffectBehavior):
+class GoTabBar(GoBoxLayout):
 	'''
-	AndroidTabsBar is just a boxlayout that contain
+	GoTabBar is just a boxlayout that contain
 	the scrollview for the tabs.
 	It is also responsible to resize the tab label when it needed.
 	'''
 
-	stroke_color = ListProperty([0, 0 ,0 ,0])
-	stroke_width = NumericProperty(2)
-
-	background_color = ListProperty([0, 0, 0, 0])
-	background_color_pos = ListProperty([0, 0, 0, 0])
-	
-	_background_color = ListProperty([0, 0, 0, 0])
-
-	radius = ListProperty([0, 0, 0, 0])
-	effect_color = ListProperty([0, 0, 0, 0])
-
 	target = ObjectProperty(None, allownone=True)
 	'''
 	Is the carousel reference of the next tab / slide.
 	When you go from "Tab A" to "Tab B", "Tab B" will be the
 	target tab / slide of the carousel.
 	'''
 
@@ -250,66 +208,15 @@
 	When you go from "Tab A" to "Tab B", "Tab B" will be the
 	target tab / slide of the carousel.
 	'''
 
 	def __init__(self, **kwargs):
 		self._trigger_update_tab_bar = Clock.schedule_once(self._update_tab_bar, 0)
 		super().__init__(**kwargs)
-		self.type_button = 'rounded'
-		Clock.schedule_once(self.set_color)
-	
-	def set_color(self, *args):
-		if isinstance(self.background_color[0], (int, float)):
-
-			if self.background_color != [0, 0, 0, 0]:
-				self._background_color = self.background_color
-
-		elif self.background_color[0] != [0, 0, 0, 0]:
-			self._background_color = self.background_color[0]
-		
-		if isinstance(self.background_color_pos[0], (int, float)):
-
-			if self.background_color_pos != [0, 0, 0, 0]:
-				self._background_color = self.background_color_pos
-				
-		elif self.background_color_pos[0] != [0, 0, 0, 0]:
-			self._background_color = self.background_color_pos[0]
-
-	def on_cursor_enter(self, *args):
-		if not isinstance(self.background_color_pos[0], (int, float)):
-			self._background_color = self.background_color_pos[1]
-
-		return super().on_cursor_enter(*args)
-
-	def on_cursor_leave(self, *args):
-		if not isinstance(self.background_color_pos[0], (int, float)):
-			self._background_color = self.background_color_pos[0]
-			
-		return super().on_cursor_leave(*args)
-
-	def on_touch_down(self, touch):
-		if not self.collide_point(*touch.pos):
-			return False
 		
-		if len(self.background_color) == 2 and isinstance(self.background_color, (list, tuple)):
-			self._background_color = self.background_color[1]
-		
-		self.ripple_show(touch)        
-		return super().on_touch_down(touch)
-
-	def on_touch_up(self, touch):
-		if not self.collide_point(*touch.pos):
-			return False
-		
-		if len(self.background_color) == 2 and isinstance(self.background_color, (list, tuple)):
-			self._background_color = self.background_color[0]
-
-		self.ripple_fade()
-		return super().on_touch_up(touch)
-
 	def _update_tab_bar(self, *args):
 		# update width of the labels when it is needed
 		width, tabs = self.scrollview.width, self.layout.children
 		tabs_widths = [t.min_space for t in tabs if t.min_space]
 		tabs_space = float(sum(tabs_widths))
 
 		if not tabs_space:
@@ -416,17 +323,17 @@
 					gap_w = ind_width - b.width
 					w_step = ind_width - (gap_w * break_step)
 					w_step = w_step if w_step + x_step <= a.x + a.width else ind_width
 
 			self.update_indicator(x_step, w_step)
 
 
-class AndroidTabs(AnchorLayout):
+class GoTab(GoAnchorLayout):
 	'''
-	The AndroidTabs class.
+	The GoTab class.
 	You can use it to create your own custom tabbed panel.
 	'''
 
 	default_tab = NumericProperty(0)
 	'''Index of the default tab. Default to 0.
 	'''
 
@@ -468,29 +375,30 @@
 			current_tab_label._do_press()
 		
 		self.tab_bar.update_indicator(
 			current_tab_label.x,
 			current_tab_label.width)
 
 	def add_widget(self, widget):
-		# You can add only subclass of AndroidTabsBase.
+		# You can add only subclass of GoTabBase.
 		if len(self.children) >= 2:
 
-			if not issubclass(widget.__class__, AndroidTabsBase):
-				raise AndroidTabsException('AndroidTabs accept only subclass of AndroidTabsBase')
+			if not issubclass(widget.__class__, GoTabBase):
+				raise GoTabException('GoTab accept only subclass of GoTabBase')
 
 			widget.tab_label.tab_bar = self.tab_bar
 			self.tab_bar.layout.add_widget(widget.tab_label)
 			self.carousel.add_widget(widget)
 			return None
 
 		return super().add_widget(widget)
 
 	def remove_widget(self, widget):
-		# You can remove only subclass of AndroidTabsBase.
-		if not issubclass(widget.__class__, AndroidTabsBase):
+		# You can remove only subclass of GoTabBase.
+		if not issubclass(widget.__class__, GoTabBase):
 
-			raise AndroidTabsException('AndroidTabs can remove only subclass of AndroidTabBase')
+			raise GoTabException('GoTab can remove only subclass of AndroidTabBase')
 
 		if widget.parent.parent == self.carousel:
 			self.tab_bar.layout.remove_widget(widget.tab_label)
 			self.carousel.remove_widget(widget)
+
```

### Comparing `kivygo-0.0.4/kivygo/uix/bezier.py` & `kivygo-0.0.5/kivygo/widgets/bezier.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 from kivy.lang import Builder
-from kivy.uix.widget import Widget
+from kivygo.widgets.widget import GoWidget
 from kivy.properties import ListProperty, NumericProperty
 from kivy.metrics import dp
 import numpy as np
 
 
 Builder.load_string('''
 
 #:import chain itertools.chain
 
 
-<BezierLine>:
+<GoBezierLine>:
 	_points: list(chain(*self.points))
 
 	canvas:
 		Color:
 			rgba: [1, 1, 1, 0.2]
 		SmoothLine:
 			points: self._points
@@ -31,19 +31,96 @@
 		Point:
 			points: self._points
 			pointsize: 5
 
 ''')
 
 
+def TwoPoints(t, P1, P2):
+	"""
+	Returns a point between P1 and P2, parametised by t.
+	INPUTS:
+		t     float/int; a parameterisation.
+		P1    numpy array; a point.
+		P2    numpy array; a point.
+	OUTPUTS:
+			numpy array; a point.
+	"""
+
+	if not isinstance(P1, np.ndarray) or not isinstance(P2, np.ndarray):
+		raise TypeError("Points must be an instance of the numpy.ndarray!")
+	
+	if not isinstance(t, (int, float)):
+		raise TypeError("Parameter t must be an int or float!")
+
+	return ( (1 - t) * P1 + t * P2 )
+
+def Points(t, points):
+	"""
+	Returns a list of points interpolated by the Bezier process
+	INPUTS:
+		t            float/int; a parameterisation.
+		points       list of numpy arrays; points.
+	OUTPUTS:
+		newpoints    list of numpy arrays; points.
+	"""
+
+	newpoints = []
+	for i1 in range(len(points) - 1):
+		newpoints += [TwoPoints(t, points[i1], points[i1 + 1])]
+
+	return newpoints
+
+def Point(t, points):
+	"""
+	Returns a point interpolated by the Bezier process
+	INPUTS:
+		t            float/int; a parameterisation.
+		points       list of numpy arrays; points.
+	OUTPUTS:
+		newpoint     numpy array; a point.
+	"""
+
+	newpoints = points
+	while len(newpoints) > 1:
+		newpoints = Points(t, newpoints)
+
+	return newpoints[0]
+
+def Curve(t_values, points):
+	"""
+	Returns a point interpolated by the Bezier process
+	INPUTS:
+		t_values     list of floats/ints; a parameterisation.
+		points       list of numpy arrays; points.
+	OUTPUTS:
+		curve        list of numpy arrays; points.
+	"""
+
+	if not hasattr(t_values, "__iter__") \
+		or not isinstance(t_values[0], (int, float)) \
+		or len(t_values) < 1:
+		
+		raise TypeError("`t_values` Must be an iterable of integers or floats, of length greater than 0 .")
+	
+	
+	curve = np.array([[0.0] * len(points[0])])
+	for t in t_values:
+		curve = np.append(curve, [Point(t, points)], axis=0)
+
+	curve = np.delete(curve, 0, 0)
+	return curve
+
+
+
 def dist(a, b):
 	return ( ((a[0] - b[0]) ** 2 + (a[1] - b[1]) ** 2) ** 0.5 )
 
 
-class BezierLine(Widget):
+class GoBezierLine(GoWidget):
 
 	_points = ListProperty([])
 	points = ListProperty([])
 	select_dist = NumericProperty(10)
 	delete_dist = NumericProperty(5)
 
 	def on_touch_down(self, touch):
@@ -88,84 +165,7 @@
 				self.parent.remove_widget(self)
 			elif i <= 0:
 				self.points = self.points[i + 1::]
 			else:
 				self.points = self.points[::i] + self.points[i + 1::]
 
 
-class Bezier():
-
-	def TwoPoints(t, P1, P2):
-		"""
-		Returns a point between P1 and P2, parametised by t.
-		INPUTS:
-			t     float/int; a parameterisation.
-			P1    numpy array; a point.
-			P2    numpy array; a point.
-		OUTPUTS:
-			    numpy array; a point.
-		"""
-
-		if not isinstance(P1, np.ndarray) or not isinstance(P2, np.ndarray):
-			raise TypeError("Points must be an instance of the numpy.ndarray!")
-		
-		if not isinstance(t, (int, float)):
-			raise TypeError("Parameter t must be an int or float!")
-
-		return ( (1 - t) * P1 + t * P2 )
-
-	def Points(t, points):
-		"""
-		Returns a list of points interpolated by the Bezier process
-		INPUTS:
-			t            float/int; a parameterisation.
-			points       list of numpy arrays; points.
-		OUTPUTS:
-			newpoints    list of numpy arrays; points.
-		"""
-
-		newpoints = []
-		for i1 in range(len(points) - 1):
-			newpoints += [Bezier.TwoPoints(t, points[i1], points[i1 + 1])]
-
-		return newpoints
-
-	def Point(t, points):
-		"""
-		Returns a point interpolated by the Bezier process
-		INPUTS:
-			t            float/int; a parameterisation.
-			points       list of numpy arrays; points.
-		OUTPUTS:
-			newpoint     numpy array; a point.
-		"""
-
-		newpoints = points
-		while len(newpoints) > 1:
-			newpoints = Bezier.Points(t, newpoints)
-
-		return newpoints[0]
-
-	def Curve(t_values, points):
-		"""
-		Returns a point interpolated by the Bezier process
-		INPUTS:
-			t_values     list of floats/ints; a parameterisation.
-			points       list of numpy arrays; points.
-		OUTPUTS:
-			curve        list of numpy arrays; points.
-		"""
-
-		if not hasattr(t_values, "__iter__") \
-			or not isinstance(t_values[0], (int, float)) \
-			or len(t_values) < 1:
-			
-			raise TypeError("`t_values` Must be an iterable of integers or floats, of length greater than 0 .")
-		
-		
-		curve = np.array([[0.0] * len(points[0])])
-		for t in t_values:
-			curve = np.append(curve, [Bezier.Point(t, points)], axis=0)
-
-		curve = np.delete(curve, 0, 0)
-		return curve
-
```

### Comparing `kivygo-0.0.4/kivygo/uix/camera.py` & `kivygo-0.0.5/kivygo/widgets/camera.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from kivy.lang import Builder
 from kivy.clock import Clock
 from kivy.properties import ObjectProperty, ListProperty
 from kivy.core.window import Window
-from kivygo.uix.popup import BoxPopup
+from kivygo.widgets.popup import BoxPopup
 from kivy.animation import Animation
 import time, random, os
 from camera4kivy import Preview
 
 from pyzbar import pyzbar
 from PIL import Image as PILImage
 
@@ -25,18 +25,18 @@
 
 	return founded[index]
 
 
 Builder.load_string("""
 
 
-#:import IconInput kivygo.uix.input.IconInput
-#:import ButtonEffect kivygo.uix.button.ButtonEffect
-#:import ButtonIcon kivygo.uix.icon.ButtonIcon
-#:import AnchorLayoutButton kivygo.uix.anchorlayout.AnchorLayoutButton
+#:import GoInputIcon kivygo.widgets.input.GoInputIcon
+#:import GoButtonRipple kivygo.widgets.button.GoButtonRipple
+#:import GoIconButton kivygo.widgets.icon.GoIconButton
+#:import GoAnchorLayoutColor kivygo.layouts.anchorlayout.GoAnchorLayoutColor
 #:import hex kivy.utils.get_color_from_hex
 
 
 <PreviewVCamera>:
 	v_size: [0, 0]
 	v_pos: [0, 0]
 
@@ -77,45 +77,45 @@
 							size: self.size
 					BoxLayout:
 						size_hint_y: None
 						height: '30dp'
 						BoxLayout:
 							size_hint: [None, None]
 							size: ['110dp', '30dp']
-							AnchorLayoutButton:
+							GoAnchorLayoutColor:
 								radius: [self.width / 1.7] * 4
 								size_hint_y: None
 								size: ['60dp', '30dp']
-								ButtonIcon:
+								GoIconButton:
 									size: ['25dp', '25dp']
 									# source: icon('flash')
 									on_release: root.start_scann()
 							Label:
 								text: 'Auto'
 								bold: True
 								color: [0, 0, 0, 1]
 								halign: 'left'
 								valign: 'center'
 								text_size: self.size
 
 						Widget:
-						AnchorLayoutButton:
+						GoAnchorLayoutColor:
 							radius: [self.width / 1.7] * 4
 							size_hint_y: None
 							size: ['80dp', '30dp']
-							ButtonIcon:
+							GoIconButton:
 								size: ['25dp', '25dp']
 								# source: icon('settings')
 								on_release: root.start_scann()
 				
-				AnchorLayoutButton:
+				GoAnchorLayoutColor:
 					size_hint_y: None
 					height: '40dp'
 					width: self.parent.width
-					ButtonIcon:
+					GoIconButton:
 						size: ['25dp', '25dp']
 						# source: icon('return')
 						on_release: root.dismiss()
 
 				AnchorLayout:
 					anchor_x: 'center'
 					anchor_y: 'center'
@@ -151,28 +151,28 @@
 							rgba: hex('#fefefe')[0:-1] + [0.8]
 						Rectangle:
 							pos: self.pos
 							size: self.size
 					BoxLayout:
 						size_hint_y: None
 						height: '25dp'
-						AnchorLayoutButton:
+						GoAnchorLayoutColor:
 							radius: [self.width / 1.7] * 4
 							size_hint_y: None
 							size: ['80dp', '25dp']
-							ButtonIcon:
+							GoIconButton:
 								size: ['25dp', '25dp']
 								# source: icon('aspect_ratio')
 								on_release: root.start_scann()
 						Widget:
-						AnchorLayoutButton:
+						GoAnchorLayoutColor:
 							radius: [self.width / 1.7] * 4
 							size_hint_y: None
 							size: ['80dp', '25dp']
-							ButtonIcon:
+							GoIconButton:
 								size: ['25dp', '25dp']
 								# source: icon('dark_theme')
 								on_release: root.start_scann()
 				AnchorLayout:
 					size_hint_y: None
 					height: '100dp'
 					anchor_y: 'center'
@@ -182,35 +182,35 @@
 						Rectangle:
 							pos: self.pos
 							size: self.size
 					BoxLayout:
 						size_hint_y: None
 						height: '70dp'
 						Widget:
-						AnchorLayoutButton:
+						GoAnchorLayoutColor:
 							radius: [self.width / 1.7] * 4
 							size_hint_y: None
 							size: ['100dp', '70dp']
-							ButtonIcon:
+							GoIconButton:
 								size: ['60dp', '60dp']
 								# source: icon('img')
 								on_release: root.start_scann()
-						AnchorLayoutButton:
+						GoAnchorLayoutColor:
 							radius: [self.width / 1.7] * 4
 							size_hint_y: None
 							size: ['100dp', '70dp']
-							ButtonIcon:
+							GoIconButton:
 								size: ['70dp', '70dp']
 								# source: icon('btn_camera')
 								on_release: root.start_scann()
-						AnchorLayoutButton:
+						GoAnchorLayoutColor:
 							radius: [self.width / 1.7] * 4
 							size_hint_y: None
 							size: ['100dp', '70dp']
-							ButtonIcon:
+							GoIconButton:
 								size: ['60dp', '60dp']
 								# source: icon('btn_photos')
 								on_release: root.start_scann()
 						Widget:
 
 
 <QRCode>:
@@ -276,15 +276,15 @@
 							Line:
 								points: [(self.x + self.width), (self.y + self.height - dp(60)), (self.x + self.width), (self.y + self.height), (self.x + self.width -dp(60)), (self.y + self.height)]
 								width: dp(3)
 							Line:
 								points: [(self.x + self.width), (self.y + dp(60)), (self.x + self.width), self.y, (self.x + self.width - dp(60)), self.y]
 								width: dp(3)
 
-						Icon:
+						GoIcon:
 							pos: [(self.parent.x + self.parent.width - self.width - dp(7)), (self.parent.y + dp(7))]
 							background_color: [1, 1, 1, 1]
 							radius: [self.width / 2] * 4
 							size_hint_y: None
 							size: ['35dp', '35dp']
 							icon_size: ['30dp', '30dp']
 							
@@ -303,37 +303,37 @@
 								if self.touch_in: scanner.height += (args[1].x - self.last_touch)
 								if self.touch_in: self.last_touch = args[1].x
 				BoxLayout:
 					size_hint_y: None
 					height: '70dp'
 					padding: ['0dp', '0dp', '0dp', '15dp']
 					Widget:
-					AnchorLayoutButton:
+					GoAnchorLayoutColor:
 						background_color: hex('#333333')
 						radius: [self.width / 2] * 4
 						size_hint_y: None
 						size: ['70dp', '70dp']
-						ButtonIcon:
+						GoIconButton:
 							size: ['45dp', '45dp']
 							# source: icon('qrcode')
 							on_release: root.start_scann()
 							color: hex('#313131')
 							canvas:
 								Color:
 									rgba: [1, 1, 1, 1]
 								RoundedRectangle:
 									pos: self.pos
 									size: self.size
 									radius: [self.width / 6] * 4
 					Widget:
-				AnchorLayoutButton:
+				GoAnchorLayoutColor:
 					size_hint_y: None
 					height: '50dp'
 					width: self.parent.width
-					ButtonIcon:
+					GoIconButton:
 						size: ['25dp', '25dp']
 						# source: icon('return')
 						on_release: root.dismiss()
 
 """)
```

### Comparing `kivygo-0.0.4/kivygo/uix/circular_bar.py` & `kivygo-0.0.5/kivygo/widgets/circular_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,30 +10,31 @@
 	ListProperty, StringProperty,
 	BooleanProperty
 )
 
 from kivy.metrics import dp
 from kivy.lang.builder import Builder
 from math import ceil
+from kivygo.app import GoApp
 
 
 Builder.load_string("""
 
-<CircularProgressBar>:
+<GoCircularProgressBar>:
 	anchor_x: "center"
 	anchor_y: "center"
 	Widget:
 		id: circular_widget
 		size_hint: None, None
 		size: [root.widget_size] * 2
 
 """)
 
 
-class CircularProgressBar(AnchorLayout):
+class GoCircularProgressBar(AnchorLayout):
 
 	started  = BooleanProperty(False)
 
 	# This constant enforces the cap argument to be one of the caps accepted by the kivy.graphics.Line class
 	cap_style = OptionProperty("round", options=["round", "none", "square"])
 	""" cap / edge of the bar, check the cap keyword argument in kivy.graphics.Line
 	"""
@@ -158,15 +159,15 @@
 
 		Clock.schedule_once(self.start)
 
 	def on_kv_post(self, *args):
 		self.ids.circular_widget.bind(size=self.start)
 	
 	def start(self, *args):
-		if self.get_root_window() != None:
+		if GoApp.get_root_window() != None:
 			self.ids.circular_widget.unbind(size=self.start)
 			if not self.started:
 				Clock.schedule_once(self.start)
 				self.started = True
 				return None
 		else:
 			return None
```

### Comparing `kivygo-0.0.4/kivygo/uix/circulardatetimepicker.py` & `kivygo-0.0.5/kivygo/widgets/circulardatetimepicker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 from kivy.animation import Animation
 from kivy.clock import Clock
-from kivygo.uix.circularlayout import CircularLayout
+from kivygo.layouts.circularlayout import GoCircularLayout
 from kivy.graphics import Line, Color, Ellipse
 from kivy.lang import Builder
 from kivy.properties import (
     NumericProperty, BoundedNumericProperty,
     ObjectProperty, StringProperty, AliasProperty,
     ListProperty, ReferenceListProperty,
     OptionProperty, BooleanProperty,
     DictProperty
 )
-from kivy.uix.boxlayout import BoxLayout
+from kivygo.layouts.boxlayout import GoBoxLayout
 from kivy.uix.label import Label
 
 from math import atan, pi, radians, sin, cos
 import datetime
 
 
 def map_number(x, in_min, in_max, out_min, out_max):
@@ -26,41 +26,39 @@
     for c in color:
         tor += "{:>02}".format(hex(int(c*255))[2:])
     return tor
 
 
 Builder.load_string("""
 
-<Number>:
+<GoNumber>:
     text_size: self.size
     valign: "middle"
     halign: "center"
     font_size: self.height * self.size_factor
 
-<CircularNumberPicker>:
+<GoCircularNumberPicker>:
     canvas.before:
         PushMatrix
         Scale:
             origin: self.center_x + self.padding[0] - self.padding[2], self.center_y + self.padding[3] - self.padding[1]
             x: self.scale
             y: self.scale
 
     canvas.after:
         PopMatrix            
 
-<CircularTimePicker>:
+<GoCircularTimePicker>:
     orientation: "vertical"
     spacing: "20dp"
 
-    AnchorLayout:
-        anchor_x: "center"
-        anchor_y: "center"
+    GoAnchorLayout:
         size_hint_y: 1.0 / 3
 
-        GridLayout:
+        GoGridLayout:
             cols: 2
             spacing: "10dp"
             size_hint_x: None
             width: self.minimum_width
            
             Label:
                 id: timelabel
@@ -78,31 +76,36 @@
                 markup: True
                 halign: "left"
                 valign: "middle"
                 size_hint_x: None
                 width: self.texture_size[0]
                 font_size: self.height * 0.3
 
-    FloatLayout:
+    GoFloatLayout:
         id: picker_container
         _bound: {}
+                
+<GoCircularTimePicker>:
+
+<GoCircularHourPicker>:    
+
 """)
 
 
-class Number(Label):
+class GoNumber(Label):
     """The class used to show the numbers in the selector.
     """
 
     size_factor = NumericProperty(.5)
     """Font size scale.
     """
 
 
-class CircularNumberPicker(CircularLayout):
-    """A circular number picker based on CircularLayout. A selector will
+class GoCircularNumberPicker(GoCircularLayout):
+    """A circular number picker based on GoCircularLayout. A selector will
     help you pick a number. You can also set :attr:`multiples_of` to make
     it show only some numbers and use the space in between for the other
     numbers.
     """
 
     min = NumericProperty(0)
     """The first value of the range.
@@ -136,24 +139,24 @@
     """
 
     selected = NumericProperty(None)
     """Currently selected number. defaults to :attr:`min`.
     """
 
     number_size_factor = NumericProperty(0.5)
-    """Font size scale factor fot the :class:`Number`s.
+    """Font size scale factor fot the :class:`GoNumber`s.
     """
 
     number_format_string = StringProperty("{}")
     """String that will be formatted with the selected number as the first argument.
     Can be anything supported by :meth:`str.format` (es. "{:02d}").
     """
 
     scale = NumericProperty(1)
-    """Canvas scale factor. Used in :class:`CircularTimePicker` transitions.
+    """Canvas scale factor. Used in :class:`GoCircularTimePicker` transitions.
     """
 
     _selection_circle = ObjectProperty(None)
     _selection_line = ObjectProperty(None)
     _selection_dot = ObjectProperty(None)
     _selection_dot_color = ObjectProperty(None)
     _selection_color = ObjectProperty(None)
@@ -220,15 +223,15 @@
         Clock.schedule_once(self.on_selected) # Just to make sure pos/size are set
 
     def _genitems(self, *a):
         self.clear_widgets()
         for i in range(*self.range):
             if i % self.multiples_of != 0:
                 continue
-            n = Number(text=self.number_format_string.format(i), size_factor=self.number_size_factor, color=self.color)
+            n = GoNumber(text=self.number_format_string.format(i), size_factor=self.number_size_factor, color=self.color)
             self.bind(color=n.setter("color"))
             self.add_widget(n)
 
     def on_touch_down(self, touch):
         if not self.collide_point(*touch.pos):
             return None
         
@@ -341,15 +344,15 @@
             angle += 2*pi
         elif angle > 2*pi:
             angle -= 2*pi
 
         return min(int(angle / quota) + self.min, self.max-1)
 
 
-class CircularMinutePicker(CircularNumberPicker):
+class GoCircularMinutePicker(GoCircularNumberPicker):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.min = 0
         self.max = 60
         self.multiples_of = 5
         self.number_format_string = "{:02d}"
@@ -358,15 +361,15 @@
         Clock.schedule_once(self._update_start_angle)
         Clock.schedule_once(self.on_selected)
 
     def _update_start_angle(self, *a):
         self.start_angle = -(360. / self.shown_items / 2) - 90
 
 
-class CircularHourPicker(CircularNumberPicker):
+class GoCircularHourPicker(GoCircularNumberPicker):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.min = 1
         self.max = 13
         self.multiples_of = 1
         self.number_format_string = "{}"
         self.direction = "cw"
@@ -374,17 +377,17 @@
         Clock.schedule_once(self._update_start_angle)
         Clock.schedule_once(self.on_selected)
 
     def _update_start_angle(self, *a):
         self.start_angle = (360.0 / self.shown_items / 2) - 90
 
 
-class CircularTimePicker(BoxLayout):
-    """Widget that makes use of :class:`CircularHourPicker` and
-    :class:`CircularMinutePicker` to create a user-friendly, animated
+class GoCircularTimePicker(GoBoxLayout):
+    """Widget that makes use of :class:`GoCircularHourPicker` and
+    :class:`GoCircularMinutePicker` to create a user-friendly, animated
     time picker like the one seen on Android.
 
     See module documentation for more details.
     """
 
     hours = NumericProperty(0)
     """The hours, in military format (0-23).
@@ -480,16 +483,16 @@
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         if self.hours >= 12:
             self._am = False
         
         self.bind(time_list=self.on_time_list, picker=self._switch_picker, _am=self.on_ampm)
-        self._h_picker = CircularHourPicker()
-        self._m_picker = CircularMinutePicker()
+        self._h_picker = GoCircularHourPicker()
+        self._m_picker = GoCircularMinutePicker()
         Clock.schedule_once(self.on_selected)
         Clock.schedule_once(self.on_time_list)
         Clock.schedule_once(self._init_later)
         Clock.schedule_once(lambda *a: self._switch_picker(noanim=True))
         
     def _init_later(self, *args):
         self.ids.timelabel.bind(on_ref_press=self.on_ref_press)
```

### Comparing `kivygo-0.0.4/kivygo/uix/circularlayout.py` & `kivygo-0.0.5/kivygo/layouts/circularlayout.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     NumericProperty, ReferenceListProperty,
     OptionProperty, BoundedNumericProperty,
     VariableListProperty, AliasProperty,
 )
 from math import sin, cos, pi, radians
 
 
-class CircularLayout(Layout):
+class GoCircularLayout(Layout):
 
     padding = VariableListProperty([0, 0, 0, 0])
     '''Padding between the layout box and it's children: [padding_left,
     padding_top, padding_right, padding_bottom].
 
     padding also accepts a two argument form [padding_horizontal,
     padding_vertical] and a one argument form [padding].
@@ -98,15 +98,15 @@
         delta_r = outer_r - inner_r
 
         # calculate maximum space used by size_hint
         stretch_weight_angle = 0.
         for w in self.children:
             sha = w.size_hint_x
             if sha == None:
-                raise ValueError("size_hint_x cannot be None in a CircularLayout")
+                raise ValueError("size_hint_x cannot be None in a GoCircularLayout")
             else:
                 stretch_weight_angle += sha
 
         sign = 1.0
         angle_offset = start_angle_r
         if direction == 'cw':
             angle_offset = 2 * pi - start_angle_r
```

### Comparing `kivygo-0.0.4/kivygo/uix/codeinput.py` & `kivygo-0.0.5/kivygo/widgets/codeinput.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [ BUGS ] Rolagem | Seleção | Canvas ViewPort |
 
 '''
 
 from kivy.app import runTouchApp
 from kivy.core.text.markup import MarkupLabel as CoreLabel
 from kivy.core.text import DEFAULT_FONT
-from kivy.uix.widget import Widget
+from kivygo.widgets.widget import GoWidget
 from kivy.core.window import Window
 from kivy.properties import (
 	ListProperty, NumericProperty,
 	StringProperty, AliasProperty,
 	BooleanProperty, ColorProperty
 )
 from kivy.clock import Clock
@@ -55,15 +55,15 @@
 	308 : 'lalt',
 }
 
 
 Builder.load_string("""
 
 
-<CodeInput>:
+<GoCodeInput>:
 	canvas.before:
 		Color:
 			rgba: self.background
 		Rectangle:
 			pos: self.pos
 			size: self.size
 		Color:
@@ -78,15 +78,15 @@
 		
 		Color:
 			rgba: self.selection_color[:-1] + [0.4]
 
 """)
 
 
-class CodeInput(Widget):
+class GoCodeInput(GoWidget):
 	
 	cursor_color = ListProperty([[1, 0, 0, 1], [0, 1, 0, 1]])
 	_cursor_color = ColorProperty([0, 0, 0, 0])
 	
 	cursor_size = ListProperty([sp(1), sp(18)])
 
 	_cursor_pos = ListProperty([0, 0])
@@ -107,18 +107,18 @@
 	focus = BooleanProperty(False)
 
 
 	# Index of the `end` & `init` visible labels on the viewport
 	label_init = 0
 	label_end = 0
 
-	# Number of lines in all text -> len(lines)
+	# GoNumber of lines in all text -> len(lines)
 	_n_labels = 0
 
-	# Number of lines in the viewport -> viewport_height / line_height
+	# GoNumber of lines in the viewport -> viewport_height / line_height
 	max_lines = 0
 	
 	# True if the key is pressed and False if not
 	shift_pressed = False
 	ctrl_pressed = False
 	capslock_pressed = False
 	alt_pressed = False
@@ -979,10 +979,10 @@
 	path = r'C:\Users\heito\AppData\Local\Programs\Python\Python39\Lib\site-packages\kivy\uix\textinput.py'
 	from kivy.uix.textinput import TextInput
 
 	with open(path, 'r') as file:
 		text = ""
 		text = file.read()
 		# inp = TextInput()
-		inp = CodeInput()
+		inp = GoCodeInput()
 		inp.text = text
 		runTouchApp(inp)
```

### Comparing `kivygo-0.0.4/kivygo/uix/effect.py` & `kivygo-0.0.5/kivygo/widgets/effect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 
 from kivy.lang import global_idmap
 from kivy.properties import (
     ObjectProperty,
     OptionProperty,
     StringProperty,
 )
-from kivy.uix.effectwidget import AdvancedEffectBase, EffectWidget
+from kivy.uix.effectwidget import AdvancedEffectBase
 from kivy.graphics import BindTexture
 
+
 GLSL = """
 
 uniform sampler2D mask;
 uniform vec2 mask_pos;
 uniform vec2 mask_size;
 
 // 0: the mask pixel multiply the texture
@@ -34,15 +35,15 @@
         return color * texture2D(mask, pos);
     else
         return color - texture2D(mask, pos);
 }
 """
 
 
-class MaskEffect(AdvancedEffectBase):
+class GoMaskEffect(AdvancedEffectBase):
     mask = ObjectProperty(None)
     glsl = StringProperty(GLSL)
     mode = OptionProperty("multiply", options=["multiply", "substract"])
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         assert self.mask
@@ -65,8 +66,8 @@
                 "mask_pos": list(self.mask.pos),
                 "mask_size": list(self.mask.size),
                 "mode": 0 if self.mode == "multiply" else 1,
             }
         )
 
 
-global_idmap["MaskEffect"] = MaskEffect
+global_idmap["GoMaskEffect"] = GoMaskEffect
```

### Comparing `kivygo-0.0.4/kivygo/uix/frostedglass.py` & `kivygo-0.0.5/kivygo/widgets/frostedglass.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     SmoothLine, Translate,
 )
 from kivy.metrics import dp
 from kivy.properties import (
     ColorProperty, ListProperty,
     NumericProperty, ObjectProperty,
 )
-from kivy.uix.floatlayout import FloatLayout
+from kivygo.layouts.floatlayout import GoFloatLayout
 from kivy.uix.image import Image
 from kivy.uix.modalview import ModalView
 from kivy.uix.screenmanager import Screen
 from kivy.uix.scrollview import ScrollView
 from kivy.uix.video import Video
 
 MEAN_RES = (Window.width + Window.height) / 2
@@ -205,48 +205,48 @@
     );
 
     gl_FragColor = vec4(effect_texture.rgb, opacity);
 }
 """
 
 
-class VerticalBlur(Fbo):
+class GoVerticalBlur(Fbo):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, fs=vertical_blur_shader, **kwargs)
         self["mean_res"] = MEAN_RES
         self["blur_size"] = dp(25)
 
 
-class HorizontalBlur(Fbo):
+class GoHorizontalBlur(Fbo):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, fs=horizontal_blur_shader, **kwargs)
         self.rect = Rectangle()
         self["mean_res"] = MEAN_RES
         self["blur_size"] = dp(25)
 
 
-class Noise(Fbo):
+class GoNoise(Fbo):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, fs=noise_shader, **kwargs)
         self.rect = Rectangle()
 
 
-class FrostedGlass(FloatLayout):
+class GoFrostedGlass(GoFloatLayout):
 
     background = ObjectProperty(None, allownone=True)
     """
-    Target widget/layout that will be used as a background to FrostedGlass.
+    Target widget/layout that will be used as a background to GoFrostedGlass.
     The recomended way to pass the widget is through the id.
     """
 
     blur_size = NumericProperty(25)
     """
     Size of the gaussian blur aplied to the background.
 
-    Note: Do not pass relative values such as dp or sp. FrostedGlass already
+    Note: Do not pass relative values such as dp or sp. GoFrostedGlass already
     manages this automatically, according to the device's screen density.
     """
 
     noise_opacity = NumericProperty(0.1)
     """Opacity of the noise layer.
     """
 
@@ -264,19 +264,19 @@
 
     border_radius = ListProperty([0, 0, 0, 0])
     """Specifies the radius used for the rounded corners clockwise:
     top-left, top-right, bottom-right, bottom-left.
     """
 
     outline_color = ColorProperty([1.0, 1.0, 1.0, 1.0])
-    """FrostedGlass outline color.
+    """GoFrostedGlass outline color.
     """
 
     outline_width = NumericProperty(1)
-    """FrostedGlass outline width.
+    """GoFrostedGlass outline width.
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         fbind = self.fbind
         fbind("outline_width", self._update_canvas)
         fbind("outline_color", self._update_canvas)
@@ -313,17 +313,17 @@
                 rounded_rectangle=(
                     self.x, self.y,
                     self.width, self.height,
                     1, 1, 1, 1, 45,
                 ),
             )
 
-        self.noise = Noise(size=(100, 100))
-        self.h_blur = HorizontalBlur(size=(100, 100))
-        self.v_blur = VerticalBlur(size=(100, 100))
+        self.noise = GoNoise(size=(100, 100))
+        self.h_blur = GoHorizontalBlur(size=(100, 100))
+        self.v_blur = GoVerticalBlur(size=(100, 100))
 
         with self.h_blur:
             ClearColor(0, 0, 0, 0)
             ClearBuffers()
             self.h_blur_scale = Scale(1, 1, 1)
             self.h_blur_translate = Translate(0, 0)
 
@@ -478,15 +478,15 @@
         blur_size = int(blur_size)
         if blur_size != self.last_blur_size_value:
             self.v_blur["blur_size"] = dp(blur_size)
             self.h_blur["blur_size"] = dp(blur_size)
             self.update_effect()
             self.last_blur_size_value = blur_size
 
-    def on_background(self, *args):
+    def on_background_default(self, *args):
         if not self.background:
             return None
         
         self.background_parents_list = self._get_all_parents(self.background)
         self.background_children_list = self._get_all_children(self.background)
         self._bind_parent_properties(self.background_parents_list)
         self._bind_children_properties(self.background_children_list)
```

### Comparing `kivygo-0.0.4/kivygo/uix/gradient.py` & `kivygo-0.0.5/kivygo/widgets/gradient.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from kivy.clock import Clock
 from kivy.graphics import (
 	RenderContext, Fbo, Color,
 	ClearColor, ClearBuffers,
 	Rectangle,
 )
-from kivy.uix.boxlayout import BoxLayout
+from kivygo.layouts.boxlayout import GoBoxLayout
 from kivy.properties import StringProperty, ObjectProperty
 
 
 shader_gradient = '''
 
 #ifdef GL_ES
 precision mediump float;
@@ -33,15 +33,15 @@
 
 	gl_FragColor = vec4(col, 1.0);
 }
 '''
 
 
 
-class GradientWidget(BoxLayout):
+class GoGradientWidget(GoBoxLayout):
 
 	fs = StringProperty(None)
 
 	texture = ObjectProperty(None)
 
 	def __init__(self, **kwargs):
```

### Comparing `kivygo-0.0.4/kivygo/uix/image.py` & `kivygo-0.0.5/kivygo/widgets/image.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,110 +1,95 @@
 
-from kivy.properties import ObjectProperty, ListProperty, StringProperty
+from kivy.properties import ListProperty, ColorProperty
 from kivy.lang.builder import Builder
 from kivy.clock import Clock
-from kivy.metrics import dp
-
-from kivy.uix.widget import Widget
 from kivy.uix.image import Image
 
 from kivy.core.image import Image as CoreImage
 import tempfile
 
 from svglib import svglib
 from reportlab.graphics import renderPM
 from reportlab.lib.colors import red, green
 from PIL import ImageChops
 from PIL import Image as PILImage
 import io
 
 
-def get_kivy_image_from_bytes(image_bytes, file_extension, image_widget=None):
-	# Return a Kivy image set from a bytes variable
-	buf = io.BytesIO(image_bytes)
-	kw = dict()
-
-	if image_widget != None:
-		kw = {
-			"mipmap": image_widget.mipmap,
-			"anim_delay": image_widget.anim_delay,
-			"keep_data": image_widget.keep_data,
-			"nocache": image_widget.nocache
-		}
-	cim = CoreImage(buf, ext=file_extension, **kw)
-	return cim
-
-
-def drawing2png(path, fp):
-	draw = svglib.svg2rlg(path)
-	if draw == None:
-		return None
-	
-	red_img = renderPM.drawToPIL(draw, bg=green, configPIL={'transparent': green})
-	green_img = renderPM.drawToPIL(draw, bg=red, configPIL={'transparent': red})
-	bg_mask = ImageChops.difference(red_img, green_img).convert('1', dither=PILImage.NONE)
-	bg_mask = ImageChops.invert(bg_mask)
-	red_img.putalpha(bg_mask)
-	red_img.save(fp, fmt='png')
-
-
 Builder.load_string("""
 
-<RoudedImage>:
-	size_hint_x: None
-	width: '70dp'
+<GoImage>:
 	canvas:
+		Clear:
 		Color:
-			rgba:[1, 1, 1, 1]
+			rgba: self._color
 		RoundedRectangle:
 			pos: self.pos
 			size: self.size
 			radius: root.radius
 			texture: root.texture
 
+	fit_mode: "fill"
 
 """)
 
 
-class RoudedImage(Widget):
+class GoImage(Image):
+
+	radius = ListProperty([0]*4)
+	_color = ColorProperty([0]*4)
 
-	texture = ObjectProperty(None)
-	source = StringProperty('')
-	radius = ListProperty([dp(5), 0, 0, dp(5)])
-	
 	def __init__(self, **kwargs):
 		super().__init__(**kwargs)
-		Clock.schedule_once(self.create_texture, 1)
+		self._color = self.color
+		Clock.schedule_once(self.texture_update)
 
-	def create_texture(self, *args):
-		image = Image(
-			source=self.source, allow_stretch=True, keep_ratio=False, 
-			size_hint=(None, None), size=self.size,
-		)
-		self.texture = image.texture
-
-
-class ImageWithSVG(Image):
-	
-	image_source = ObjectProperty('')
-	
-	def on_image_source(self, *args):
+	def on_color(self, *args):
+		self._color = self.color
 
-		if isinstance(self.image_source, str):
-			self.set_source(self.image_source)
-
-	def set_source(self, source:str):
-
-		if not source.endswith(".svg"):
-			self.source = source
+	def set_texture_from_resource(self, resource):
+		if not resource:
+			self._clear_core_image()
 			return None
 		
+		if not resource.endswith(".svg"):
+			return super().set_texture_from_resource(resource)
+	
+		if self._coreimage:
+			self._coreimage.unbind(on_texture=self._on_tex_change)
+
 		file = tempfile.NamedTemporaryFile(mode='+wb', suffix=".png")
 		try:
-			drawing2png(source, file)
+			self.svg_to_png(self.source, file)
 		except ValueError:
 			pass
 
 		file.seek(0)
-		img = get_kivy_image_from_bytes(file.read(), 'png', self)
-		self.texture = img.texture
+		self._coreimage = image = self.get_kivy_image_from_bytes(file.read(), 'png')
+		image.bind(on_texture=self._on_tex_change)
+		self.texture = image.texture
 
+	
+	def get_kivy_image_from_bytes(self, image_bytes, file_extension):
+		# Return a Kivy image set from a bytes variable
+		buf = io.BytesIO(image_bytes)
+	
+		image = CoreImage(
+			buf, ext=file_extension,
+			mipmap=self.mipmap,
+			anim_delay=self.anim_delay,
+			keep_data=self.keep_data,
+			nocache=self.nocache
+		)
+		return image
+
+	def svg_to_png(self, path, fp):
+		draw = svglib.svg2rlg(path)
+		if draw == None:
+			return None
+		
+		red_img = renderPM.drawToPIL(draw, bg=green, configPIL={'transparent': green})
+		green_img = renderPM.drawToPIL(draw, bg=red, configPIL={'transparent': red})
+		bg_mask = ImageChops.difference(red_img, green_img).convert('1', dither=PILImage.NONE)
+		bg_mask = ImageChops.invert(bg_mask)
+		red_img.putalpha(bg_mask)
+		red_img.save(fp, fmt='png')
```

### Comparing `kivygo-0.0.4/kivygo/uix/input.py` & `kivygo-0.0.5/kivygo/widgets/input.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,24 +11,27 @@
 )
 from kivy.uix.anchorlayout import AnchorLayout
 from kivy.uix.textinput import TextInput
 
 
 Builder.load_string("""
 
-#:import ToggleButtonIcon kivygo.uix.icon.ToggleButtonIcon
-#:import InputEditor kivygo.uix.terminal.InputEditor
 
-
-<IconInput>:
+<GoInputIcon>:
 	hide: False
 	padding: [dp(10), dp(10), dp(10), dp(10)]
 	size_hint_y: None
 	height: '60dp'
 	input: input
+		    
+	line_color: GoColors.primary_border
+	background_color: GoColors.primary_default
+	label_defaut_color: GoColors.title_default
+	label_pos_color: GoColors.title_hover
+	text_input_color: GoColors.text_default
 
 	BoxLayout:
 		id: box
 		canvas:
 			Color:
 				rgba: root.color_line
 			Line:
@@ -45,39 +48,38 @@
 		AnchorLayout:
 			id: anchor_left
 			padding: [1, 1, 1, 1]
 			size_hint_x: None
 			width: ( root.icon_left_size[0] + dp(15) )
 			anchor_y: 'center'
 			
-			ToggleButtonIcon:
+			GoIconToggleButton:
 				id: button_left
-				allow_stretch: True
+				fit_mode: "fill"
 				name: 'icon_left'
-				keep_ratio: False
 				mipmap: True
 				size_hint_y: None
 				size: root.icon_left_size
 				pos_source: root.icon_left_pos_source
-				icon_source: root.icon_left_source
+				source: root.icon_left_source
 				icon_color: root.icon_left_color
 				pos_color: root.icon_left_color_pos
 				icon_state_source: root.icon_left_state_sources
 				effect_color: root.icon_left_effect_color
 				state_button: root.icon_left_state
 
 		AnchorLayout:
 			id: anchor_input
 
 			AnchorLayout:
 				anchor_y: 'center'
 				anchor_x: 'center'
 				padding: root.padding
 				MyTextInput:
-				# InputEditor:
+				# GoInputEditor:
 					id: input
 					size_hint_y: None
 					height: self.minimum_height			
 					id: input
 					text: root.input_text
 					on_text: root.input_text = self.text
 					window_root: root
@@ -94,25 +96,24 @@
 		AnchorLayout:
 			padding: [dp(-1), dp(1), dp(10), dp(1)]
 			size_hint_x: None
 			width: ( root.icon_right_size[0] + dp(15) )
 			anchor_y: 'center'
 			id: anchor_right
 
-			ToggleButtonIcon:
+			GoIconToggleButton:
 				id: button_right
 				name: 'icon_right'
 				window_root: root
-				allow_stretch: True
-				keep_ratio: False
+				fit_mode: "fill"
 				mipmap: True
 				size_hint_y: None
 				size: root.icon_right_size
 				pos_source: root.icon_right_pos_source
-				image_source: root.icon_right_source
+				source: root.icon_right_source
 				icon_state_source: root.icon_right_state_sources
 				icon_color: root.icon_right_color
 				pos_color: root.icon_right_color_pos
 				effect_color: root.icon_right_effect_color
 				state_button: root.icon_right_state
 	
 	FloatLayout:
@@ -136,22 +137,22 @@
 		r =  super().insert_text(substring, from_undo=from_undo)
 
 		if self.window_root != None:
 			self.window_root.dispatch('on_input_text', substring, from_undo)
 		return r
 
 
-class IconInput(AnchorLayout):
+class GoInputIcon(AnchorLayout):
 
-	line_color = ListProperty([1,1,1,1])
-	line_color_pos = ListProperty([0, 0, 0, 0])
-	color_line = ListProperty([0, 0, 0, 0])
+	line_color = ListProperty([0]*4)
+	line_color_pos = ListProperty([0]*4)
+	color_line = ListProperty([0]*4)
 	outline_width = NumericProperty(1.01)
 
-	background_color = ListProperty([0,0,0,0])
+	background_color = ListProperty([0]*4)
 	multiline = BooleanProperty(False)
 	radius = ListProperty([dp(15), dp(15), dp(15), dp(15)])
 
 	icon_left = ObjectProperty(None)
 	icon_left_state = StringProperty('toggle')#'toggle' or 'button'
 	icon_left_color = ListProperty([1, 1, 1, 1])
 	icon_left_pos_source = StringProperty('')
@@ -169,21 +170,21 @@
 	icon_right_source = StringProperty('')
 	icon_right_color_pos = ListProperty([-1, -1, -1, -1])
 	icon_right_size = ListProperty([dp(30), dp(23)])
 	icon_right_effect_color = ListProperty([0, 0, 0, 0])
 
 	label_text = StringProperty('')
 	label_font_size = NumericProperty(dp(16))
-	label_defaut_color = ListProperty([1, 1, 1, 1])
-	label_pos_color = ListProperty([1, 1, 1, 1])
+	label_defaut_color = ListProperty([0]*4)
+	label_pos_color = ListProperty([0]*4)
 	state_label = StringProperty('')
 
 	input = ObjectProperty(None)
 	hide = ObjectProperty(False)
-	text_input_color = ListProperty([1, 1, 1, 1])
+	text_input_color = ListProperty([0]*4)
 	input_text = StringProperty("")
 
 	__events__ = ('on_icon_right_press', 'on_icon_right_release', 'on_icon_left_press',
 				  'on_icon_left_release', 'on_input_press', 'on_input_release', 
 				  'on_input_text', 'on_init_input', 'on_icon_right_pos',
 				  'on_icon_right_pos_release', 'on_enter')
 
@@ -217,23 +218,23 @@
 
 	def icon_down(self, button, *args):
 		if button.state_button == 'toggle':
 			button.num += 1
 			if button.pos_source and button.num == 1:
 				button.source = button.pos_source
 			elif button.num == 2:
-				button.source = button.icon_source
+				button.source = button.source
 				button.num = 0
 		elif button.state_button == 'button':
 			if button.pos_source:
 				button.source = button.pos_source
 	
 	def icon_up(self, button, *args):
 		if button.state_button == 'button':
-			button.source = button.icon_source
+			button.source = button.source
 
 	def config(self, *args):
 		self.pads()
 		self.color_line = self.line_color
 		self.icon_right = self.ids.button_right
 		self.icon_left = self.ids.button_left
 		self.input = self.ids.input
```

### Comparing `kivygo-0.0.4/kivygo/uix/joystick.py` & `kivygo-0.0.5/kivygo/widgets/joystick.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import math
 from kivy.lang.builder import Builder
-from kivy.uix.widget import Widget
+from kivygo.widgets.widget import GoWidget
 from kivy.properties import (
 	BooleanProperty, NumericProperty,
 	ListProperty, ReferenceListProperty,
 )
 
 OUTLINE_ZERO = 0.00000000001
 # replaces user's 0 value for outlines, avoids invalid width exception
 
 
 Builder.load_string("""
 
-<JoystickPad>:
+<GoTouchData>:
+
+<GoJoystickPad>:
 	id: pad
 	canvas:
 		Color:
 			rgba: self._background_color
 		Ellipse:
 			pos: (self.center_x - self._radius), (self.center_y - self._radius)
 			size: (self._diameter, self._diameter)
@@ -24,15 +26,15 @@
 		Color:
 			rgba: self._line_color
 		Line:
 			circle: (self.center_x, self.center_y, (self._diameter - (self._line_width * 2)) / 2)
 			width: self._line_width
 
 			
-<JoyStick>:
+<GoJoyStick>:
 	canvas:
 		Color:
 			rgba: self.outer_background_color
 		Ellipse:
 			pos: (self.center_x - self._outer_radius), (self.center_y - self._outer_radius)
 			size: (self._outer_diameter, self._outer_diameter)
 
@@ -50,22 +52,22 @@
 
 		Color:
 			rgba: self.inner_line_color
 		Line:
 			circle: (self.center_x, self.center_y, self._inner_radius)
 			width: self._inner_line_width
 
-	JoystickPad:
+	GoJoystickPad:
 		id: pad
 
 
 """)
 
 
-class TouchData:
+class GoTouchData(GoWidget):
 	x_distance = None
 	y_distance = None
 	x_offset = None
 	y_offset = None
 	relative_distance = None
 	is_external = None
 	in_range = None
@@ -95,23 +97,23 @@
 		self.x_offset = x_offset
 		self.y_offset = y_offset
 		self.relative_distance = relative_distance
 		self.is_external = is_external
 		self.in_range = in_range
 
 
-class JoystickPad(Widget):
+class GoJoystickPad(GoWidget):
 	_diameter = NumericProperty(1)
 	_radius = NumericProperty(1)
 	_background_color = ListProperty([0, 0, 0, 1])
 	_line_color = ListProperty([1, 1, 1, 1])
 	_line_width = NumericProperty(1)
 
 
-class Joystick(Widget):
+class GoJoystick(GoWidget):
 	'''The joystick base is comprised of an outer circle & an inner circle.
 	   The joystick pad is another circle,
 		   which the user can move within the base.
 	   All 3 of these elements can be styled independently
 		   to create different effects.
 	   All coordinate properties are based on the
 		   position of the joystick pad.'''
@@ -215,15 +217,15 @@
 		self.bind(
 			pos=self.do_layout,
 			size=self.do_layout,
 			children=self.do_layout
 		)
 
 	def move_pad(self, touch, from_touch_down):
-		td = TouchData(self, touch)
+		td = GoTouchData(self, touch)
 		if td.is_external and from_touch_down:
 			touch.ud['joystick'] = None
 			return False
 		elif td.in_range:
 			self._update_coordinates_from_internal_touch(touch, td)
 			return True
 		elif not (td.in_range):
```

### Comparing `kivygo-0.0.4/kivygo/uix/kivyg_icon.py` & `kivygo-0.0.5/kivygo/widgets/kivyg_icon.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 from kivygo.utils import (
     line_points, bezier_points,
     get_all_points, parse_svg,
     find_center,
 )
 
 from kivygo.animation import Animation
+from kivygo.widgets.widget import GoWidget
 from svg.path import parse_path
 from collections import OrderedDict
 
 
-class Kivg():
+class GoKivg(GoWidget):
     def __init__(self, widget, *args):
         """
         widget: widget to draw svg upon
         """
         self.b = widget
         self._fill = True  # Fill path with color after drawing
         self._LINE_WIDTH = 2
```

### Comparing `kivygo-0.0.4/kivygo/uix/label.py` & `kivygo-0.0.5/kivygo/widgets/label.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,68 @@
 
-from kivygo.behaviors.button import ButtonBehavior
+from kivygo.behaviors.button import GoButtonBehavior
 
 from kivy.core.text.markup import MarkupLabel as CoreLabel
 from kivy.lang import Builder
 from kivy.graphics.texture import Texture
 
 from kivy.uix.label import Label
 from kivy.properties import (
 	NumericProperty, DictProperty,
 	StringProperty, ObjectProperty,
 	ListProperty, AliasProperty,
+	ColorProperty
 )
 
 from kivy.clock import Clock
 from kivy.graphics.vertex_instructions import Quad
 from kivy.animation import AnimationTransition
 from kivy.compat import string_types
 from math import pi, cos, sin, radians
 from kivy.vector import Vector
 from kivygo.transformations import Transformations
 
 
 Builder.load_string("""
 
-<LabelGradient>:
+<GoLabel>:
+	color: GoColors.text_default
+		    
+<GoLabelGradient>:
 	canvas.before:
 		# draw the gradient below the normal Label Texture
 		Color:
 			rgba: [1, 1, 1, 1]
 		Rectangle:
 			texture: self.gradient
 			size: self.texture_size
 			pos: [ \
 			int(self.center_x - self.texture_size[0] / 2.0), \
 			int(self.center_y - self.texture_size[1] / 2.0)]
 			
-<LabelButton>:
-	color: [1, 1, 1, 1]
+<GoLabelButton>:
+	normal_color: GoColors.text_default
+	down_color: GoColors.text_pressed
+	color: self.normal_color if self.state == "normal" and GoColors.palette else self.down_color
 
-<LabelToScroll>:
+<GoLabelScroll>:
 	text: 'Section Option'
-	padding_x: '15dp'
 	size_hint_y: None
 	on_size: self.update_content()
 	text_size: self.size
 	valign: 'center'
 	halign: 'center'
 	multiline: True
 
 """)
 
+class GoLabel(Label):
+	pass
 
-class LabelGradient(Label):
+class GoLabelGradient(GoLabel):
 
 	gradient = ObjectProperty(None)
 	bg_color = ListProperty([0, 0, 0, 255])
 
 	def __init__(self, **kwargs):
 		super().__init__(**kwargs)
 
@@ -67,15 +74,15 @@
 			return None
 
 		# unbind, so we don't loop
 		self.unbind(texture=self.fix_texture)
 
 		# The normal Label texture is transparent except for the text itself
 		# This code changes the texture to make the text transparent, and everything else
-		# gets set to self.bg_color (a property of LabelGradient)
+		# gets set to self.bg_color (a property of GoLabelGradient)
 		pixels = list(self.texture.pixels)
 		
 		for index in range(3, len(pixels)-4, 4):
 
 			if pixels[index] == 0:
 				# change transparent pixels to the bg_color
 				pixels[index-3:index+1] = self.bg_color
@@ -86,19 +93,20 @@
 		# create a new texture, blit the new pixels, and apply the new texture
 		new_texture = Texture.create(size=self.texture.size, colorfmt='rgba')
 		new_texture.blit_buffer(bytes(pixels), colorfmt='rgba', bufferfmt='ubyte')
 		new_texture.flip_vertical()
 		self.texture = new_texture
 
 	
-class LabelButton(ButtonBehavior, Label):
-	pass
+class GoLabelButton(GoButtonBehavior, GoLabel):
+	normal_color = ColorProperty([0, 0, 0, 0])
+	down_color = ColorProperty([0, 0, 0, 0])
 
 
-class LabelToScroll(Label):
+class GoLabelScroll(GoLabel):
 
 	n_lines = NumericProperty(0)
 	d_height = NumericProperty(0)
 
 	def __init__(self, **kwargs):
 		super().__init__(**kwargs)
 		Clock.schedule_once(self.update_content, 3)
@@ -108,15 +116,15 @@
 		kw['text'] = self.text
 		kw['text_size'] = [self.text_size[0], None]
 		lb = CoreLabel(**kw)
 		lb.refresh()
 		self.height = lb.texture.size[1]
 
 
-class AnimatedLabel(Label):
+class GoLabelAnimated(GoLabel):
 	'''duration of the animation of each letter'''
 	letter_duration = NumericProperty()
 
 	'''time to wait before starting to animate each letter'''
 	letter_offset = NumericProperty()
 
 	'''target text to set to animate'''
@@ -237,15 +245,15 @@
 			return None
 		
 		self._time = 0
 		Clock.unschedule(self.tick)
 		Clock.schedule_interval(self.tick, 0)
 
 
-class AnimatedBezierLabel(AnimatedLabel):
+class GoLabelBezierAnimated(GoLabelAnimated):
 
 	def compute_bezier(self, points, n):
 		'''compute nth segment point among segments of the bezier line
 		defined by points
 
 		Beware, complexity is quadratic to the number of points
 		'''
```

### Comparing `kivygo-0.0.4/kivygo/uix/navigationdrawer.py` & `kivygo-0.0.5/kivygo/widgets/navigationdrawer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 	StringProperty,
 )
 from kivy.lang import Builder
 
 
 Builder.load_string('''
 
-<NavigationDrawer>:
+<GoNavigationDrawer>:
 	size_hint: [1, 1]
 	_side_panel: sidepanel
 	_main_panel: mainpanel
 	_join_image: joinimage
 	side_panel_width: min(dp(250), 0.5*self.width)
-	BoxLayout:
+	GoBoxLayout:
 		id: sidepanel
 		y: root.y
 		x: root.x - \
 		   (1-root._anim_progress)* \
 		   root.side_panel_init_offset*root.side_panel_width
 		height: root.height
 		width: root.side_panel_width
@@ -37,15 +37,15 @@
 				size: self.size
 		canvas.after:
 			Color:
 				rgba: [0, 0, 0, (1-root._anim_progress)*root.side_panel_darkness]
 			Rectangle:
 				size: self.size
 				pos: self.pos
-	BoxLayout:
+	GoBoxLayout:
 		id: mainpanel
 		x: root.x + \
 		   root._anim_progress * \
 		   root.side_panel_width * \
 		   root.main_panel_final_offset
 		y: root.y
 		size: root.size
@@ -57,38 +57,37 @@
 				size: self.size
 		canvas.after:
 			Color:
 				rgba: [0, 0,0 , root._anim_progress*root.main_panel_darkness]
 			Rectangle:
 				size: self.size
 				pos: self.pos
-	Image:
+	GoImage:
 		id: joinimage
 		opacity: min(sidepanel.opacity, 0 if root._anim_progress < 0.00001 \
 				 else min(root._anim_progress*40, 1))
 		source: root._choose_image(root._main_above, root.separator_image)
 		mipmap: False
 		width: root.separator_image_width
 		height: root._side_panel.height
 		x: (mainpanel.x - self.width + 1) if root._main_above \
 		   else (sidepanel.x + sidepanel.width - 1)
 		y: root.y
-		allow_stretch: True
-		keep_ratio: False
+		fit_mode: "fill"
 ''')
 
 
 class NavigationDrawerException(Exception):
 	'''Raised when add_widget or remove_widget called incorrectly on a
-	NavigationDrawer.
+	GoNavigationDrawer.
 
 	'''
 
 
-class NavigationDrawer(StencilView):
+class GoNavigationDrawer(StencilView):
 	'''Widget taking two children, a side panel and a main panel,
 	displaying them in a way that replicates the popular Android
 	functionality. See module documentation for more info.
 
 	'''
 
 	# Internal references for side, main and image widgets
@@ -100,41 +99,41 @@
 	'''Automatically bound to whatever widget is added as the hidden panel.'''
 	main_panel = ObjectProperty(None, allownone=True)
 	'''Automatically bound to whatever widget is added as the main panel.'''
 
 	# Appearance properties
 	side_panel_width = NumericProperty()
 	'''The width of the hidden side panel. Defaults to the minimum of
-	250dp or half the NavigationDrawer width.'''
+	250dp or half the GoNavigationDrawer width.'''
 	separator_image = StringProperty('')
 	'''The path to an image that will be placed between the side and main
 	panels. If set to `''`, defaults to a gradient from black to
 	transparent in an appropriate direction (left->right if side panel
 	above main, right->left if main panel on top).'''
 	separator_image_width = NumericProperty(dp(10))
 	'''The width of the separator image. Defaults to 10dp'''
 
 	# Touch properties
 	touch_accept_width = NumericProperty('14dp')
-	'''Distance from the left of the NavigationDrawer in which to grab the
+	'''Distance from the left of the GoNavigationDrawer in which to grab the
 	touch and allow revealing of the hidden panel.'''
 	_touch = ObjectProperty(None, allownone=True)  # The currently active touch
 
 	# Animation properties
 	state = OptionProperty('closed', options=('open', 'closed'))
 	'''Specifies the state of the widget. Must be one of 'open' or
 	'closed'. Setting its value automatically jumps to the relevant state,
 	or users may use the anim_to_state() method to animate the
 	transition.'''
 	anim_time = NumericProperty(0.3)
 	'''The time taken for the panel to slide to the open/closed state when
 	released or manually animated with anim_to_state.'''
 	min_dist_to_open = NumericProperty(0.7)
 	'''Must be between 0 and 1. Specifies the fraction of the hidden panel
-	width beyond which the NavigationDrawer will relax to open state when
+	width beyond which the GoNavigationDrawer will relax to open state when
 	released. Defaults to 0.7.'''
 	_anim_progress = NumericProperty(0)  # Internal state controlling
 										 # widget positions
 	_anim_init_progress = NumericProperty(0)
 
 	# Animation controls
 	top_panel = OptionProperty('main', options=['main', 'side'])
@@ -274,15 +273,15 @@
 
 		elif self.main_panel == None:
 			self._main_panel.add_widget(widget)
 			self.main_panel = widget
 		else:
 			raise NavigationDrawerException(
 				'Can\'t add more than two widgets'
-				'directly to NavigationDrawer')
+				'directly to GoNavigationDrawer')
 
 	def remove_widget(self, widget):
 		if widget is self.side_panel:
 			self._side_panel.remove_widget(widget)
 			self.side_panel = None
 		elif widget is self.main_panel:
 			self._main_panel.remove_widget(widget)
```

### Comparing `kivygo-0.0.4/kivygo/uix/particle.py` & `kivygo-0.0.5/kivygo/widgets/particle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from kivy.uix.widget import Widget
+from kivygo.widgets.widget import GoWidget
 from kivy.clock import Clock
 from kivy.graphics import (
     Color, Callback, Rotate,
     PushMatrix, PopMatrix,
     Translate, Quad
 )
 
@@ -34,40 +34,41 @@
 def random_color_variance(base, variance):
     return [min(max(0.0, (random_variance(base[i], variance[i]))), 1.0) for i in range(4)]
 
 
 EMITTER_TYPE_GRAVITY = 0
 EMITTER_TYPE_RADIAL = 1
 
-BLEND_FUNC = {0: GL_ZERO,
-            1: GL_ONE,
-            0x300: GL_SRC_COLOR,
-            0x301: GL_ONE_MINUS_SRC_COLOR,
-            0x302: GL_SRC_ALPHA,
-            0x303: GL_ONE_MINUS_SRC_ALPHA,
-            0x304: GL_DST_ALPHA,
-            0x305: GL_ONE_MINUS_DST_ALPHA,
-            0x306: GL_DST_COLOR,
-            0x307: GL_ONE_MINUS_DST_COLOR
+BLEND_FUNC = {
+    0: GL_ZERO,
+    1: GL_ONE,
+    0x300: GL_SRC_COLOR,
+    0x301: GL_ONE_MINUS_SRC_COLOR,
+    0x302: GL_SRC_ALPHA,
+    0x303: GL_ONE_MINUS_SRC_ALPHA,
+    0x304: GL_DST_ALPHA,
+    0x305: GL_ONE_MINUS_DST_ALPHA,
+    0x306: GL_DST_COLOR,
+    0x307: GL_ONE_MINUS_DST_COLOR
 }
 
 
-class Particle(object):
+class GoParticle(object):
     x, y, rotation, current_time = -256, -256, 0, 0
     scale, total_time = 1.0, 0.
     color = [1.0, 1.0, 1.0, 1.0]
     color_delta = [0.0, 0.0, 0.0, 0.0]
     start_x, start_y, velocity_x, velocity_y = 0, 0, 0, 0
     radial_acceleration, tangent_acceleration = 0, 0
     emit_radius, emit_radius_delta = 0, 0
     emit_rotation, emit_rotation_delta = 0, 0
     rotation_delta, scale_delta = 0, 0
 
 
-class ParticleSystem(Widget):
+class GoParticleSystem(GoWidget):
     max_num_particles = NumericProperty(200)
     life_span = NumericProperty(2)
     texture = ObjectProperty(None)
     texture_path = StringProperty(None)
     life_span_variance = NumericProperty(0)
     start_size = NumericProperty(16)
     start_size_variance = NumericProperty(0)
@@ -234,15 +235,15 @@
     def _update(self, dt):
         self._advance_time(dt)
         self._render()
         if not self._is_paused:
             Clock.schedule_once(self._update, self.update_interval)
 
     def _create_particle(self):
-        return Particle()
+        return GoParticle()
 
     def _init_particle(self, particle):
         life_span = random_variance(self.life_span, self.life_span_variance)
         if life_span <= 0.0:
             return
 
         particle.current_time = 0.0
@@ -367,15 +368,15 @@
             else:
                 if particle_index != self.num_particles - 1:
                     next_particle = self.particles[self.num_particles - 1]
                     self.particles[self.num_particles - 1] = particle
                     self.particles[particle_index] = next_particle
                 self.num_particles -= 1
                 if self.num_particles == 0:
-                    Logger.debug('Particle: COMPLETE')
+                    Logger.debug('GoParticle: COMPLETE')
 
         # create and advance new particles
         if self.emission_time > 0:
             time_between_particles = 1.0 / self.emission_rate
             self.frame_time += passed_time
 
             while self.frame_time > 0:
```

### Comparing `kivygo-0.0.4/kivygo/uix/pizza_graph.py` & `kivygo-0.0.5/kivygo/widgets/pizza_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from kivy.graphics import Color
 from kivy.graphics import Ellipse
 from kivy.graphics import Line
 from kivy.uix.label import Label
 from kivy.utils import get_color_from_hex
 
 
-class Pizza(RelativeLayout):
+class GoPizza(RelativeLayout):
     serie = ListProperty([])
     chart_size = NumericProperty(256)
     legend_color = StringProperty('ffffcc')
     legend_value_rayon = NumericProperty(100)
     legend_title_rayon = NumericProperty(160)
     chart_border = NumericProperty(2)
```

### Comparing `kivygo-0.0.4/kivygo/uix/popup.py` & `kivygo-0.0.5/kivygo/widgets/popup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 from kivy.uix.modalview import ModalView
-from kivygo.uix.boxlayout import ColoredBoxLayout
+from kivygo.layouts.boxlayout import GoBoxLayoutColor
 from kivy.lang.builder import Builder
 from kivy.properties import StringProperty
-from kivygo.uix.label import LabelToScroll
-from kivygo.uix.icon import ButtonIcon
-from kivygo.uix.button import ButtonEffect
-from kivygo.uix.anchorlayout import AnchorLayoutButton
+from kivygo.widgets.label import GoLabelScroll
+from kivygo.widgets.icon import GoIconButton
+from kivygo.widgets.button import GoButtonRipple
+from kivygo.layouts.anchorlayout import GoAnchorLayoutColor
 
 
 Builder.load_string("""
 
 #:import hex kivy.utils.get_color_from_hex
 
 <BoxPopup>:
@@ -18,15 +18,15 @@
 	box_radius:  [dp(20), dp(20), dp(20), dp(20)]
 	box_padding: ['0dp', '15dp', '0dp', '0dp']
 	border: [0, 0, 0, 0]
 	auto_dismiss: False
 	overlay_color: [0, 0, 0, 0]
 	background_color: [0, 0, 0, 0]
 
-	ColoredBoxLayout:
+	GoBoxLayoutColor:
 		orientation: 'vertical'
 		padding: root.box_padding
 		background_color: root.box_background_color
 		radius: root.box_radius
 		id: _colored_box
 
 
@@ -41,58 +41,58 @@
 	box_padding: [0, 0, 0, 0]
 	overlay_color: [0, 0, 0, 0.7]
 
 	BoxLayout:
 		size_hint_y: None
 		height: self.minimum_height
 
-		ColoredBoxLayout:
+		GoBoxLayoutColor:
 			size_hint_y: None
 			height: self.minimum_height
 			background_color: hex('#ebeef2')
 			radius: [dp(20), dp(20), 0, 0]
 
 			AnchorLayout:
 				anchor_y: 'center'
 				size_hint_y: None
 				height: lb_t.height + dp(10)
 				padding: [dp(10), 0, 0, 0]
-
-				LabelToScroll:
+				padding_x: "15dp"
+				GoLabelScroll:
 					text: root.title
 					font_size: "30sp"
 					bold: True
 					halign: 'left'
 					valign: 'center'
 					color: hex('#e06031')
 					id: lb_t
 
-			AnchorLayoutButton:
+			GoAnchorLayoutColor:
 				size_hint_y: None
 				height: lb_t.parent.height
 
-				ButtonIcon:
+				GoIconButton:
 					size: ['35dp', '35dp']
 					source: app.get_icon('close')
 					on_release: root.dismiss()
 
 	AnchorLayout:
 		anchor_y: 'center'
-
-		LabelToScroll:
+		padding_x: "15dp"
+		GoLabelScroll:
 			text: root.msg
 			font_size: "20sp"
 
 	AnchorLayout:
 		anchor_y: 'center'
 		anchor_x: 'center'
 		size_hint_y: None
 		height: 0 if not self.children else self.children[0].height + dp(30)
 
-		ButtonEffect:
+		GoButtonRipple:
 			text: "Continuar"
 			size_hint: None, None
 			size: '120dp', '55dp'
 			radius: [dp(15)]
 			background_color: hex('#2c2c2c')
 			bold: True
 			font_size: '17sp'
@@ -100,15 +100,15 @@
 
 """)
 
 
 class BoxPopup(ModalView):
 
 	def add_widget(self, widget, *args, **kwargs):
-		if isinstance(widget, ColoredBoxLayout):
+		if isinstance(widget, GoBoxLayoutColor):
 			return super().add_widget(widget, *args, **kwargs)
 		return self.ids._colored_box.add_widget(widget, *args, **kwargs)
 
 
 class ConfirmPopup(BoxPopup):
 	
 	msg = StringProperty("É necessário aceitar os termos de uso!")
```

### Comparing `kivygo-0.0.4/kivygo/uix/progressspinner.py` & `kivygo-0.0.5/kivygo/widgets/progressspinner.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,37 +5,37 @@
     NumericProperty, ListProperty,
     BoundedNumericProperty, StringProperty,
     ObjectProperty,
 )
 from kivy.animation import Animation
 from kivy.clock import Clock
 from kivy.properties import BooleanProperty
-from kivy.uix.widget import Widget
+from kivygo.widgets.widget import GoWidget
 
 Builder.load_string('''
 
-<ProgressSpinnerBase>:
+<GoProgressSpinnerBase>:
 	_size: min(self.height, self.width)
 	_rsize: self._size / 2.0
 	_stroke: max(0.1, self._rsize / 20.0 if self.stroke_width == None else self.stroke_width)
 	_radius: self._rsize - self._stroke * 2.0
 
-<ProgressSpinner>:
+<GoProgressSpinner>:
 	canvas:
 		Color:
 			rgba: self.color
 		Line:
 			circle:
 				(self.center_x, self.center_y, self._radius,
 				self._angle_center + self._angle_start,
 				self._angle_center + self._angle_end)
 			width: self._stroke
 			cap: 'none'
 
-<TextureProgressSpinner>:
+<GoTextureProgressSpinner>:
 	canvas:
 		StencilPush
 		Color:
 			rgba: [1, 1, 1, 1]
 		Line:
 			circle:
 				(self.center_x, self.center_y, self._radius,
@@ -60,15 +60,15 @@
 				(self.center_x, self.center_y, self._radius,
 				self._angle_center + self._angle_start,
 				self._angle_center + self._angle_end)
 			width: self._stroke
 			cap: 'none'
 		StencilPop
 
-<RotatingTextureProgressSpinner>:
+<GoRotatingTextureProgressSpinner>:
 	canvas:
 		PushMatrix
 		Rotate:
 			angle: -(self._angle_center)
 			origin: self.center
 		
 		StencilPush
@@ -101,15 +101,15 @@
 		StencilPop
 		
 		PopMatrix
 
 ''')
 
 
-class ProgressSpinnerBase(Widget):
+class GoProgressSpinnerBase(GoWidget):
 
     color = ListProperty([1, 1, 1, 1])
     '''Color to render the spinner.
     '''
 
     speed = BoundedNumericProperty(1, min=0.1)
     '''Speed coefficient of the spinner. This value is multiplied by the
@@ -215,36 +215,36 @@
             self._state = 'wait1'
             self._next = Clock.schedule_once(self._rotate, wait_speed)
             while self._angle_end > 720.:
                 self._angle_start -= 360.
                 self._angle_end -= 360.
 
 
-class ProgressSpinner(ProgressSpinnerBase):
+class GoProgressSpinner(GoProgressSpinnerBase):
     pass
 
 
-class TextureProgressSpinnerBase(ProgressSpinnerBase):
+class GoTextureProgressSpinnerBase(GoProgressSpinnerBase):
     texture = ObjectProperty(None)
     '''Texture to render for the spinner.
     '''
 
     source = StringProperty('')
     '''Source image to render for the spinner.
     '''
 
     def on_source(self, inst, value):
         if value:
             self.texture = CoreImage(value).texture
 
 
-class TextureProgressSpinner(TextureProgressSpinnerBase):
-    '''Same as ProgressSpinner, but with a texture/image instead of a solid color.
+class GoTextureProgressSpinner(GoTextureProgressSpinnerBase):
+    '''Same as GoProgressSpinner, but with a texture/image instead of a solid color.
     '''
     pass
 
 
-class RotatingTextureProgressSpinner(TextureProgressSpinnerBase):
-    '''Same as TextureProgressSpinner, but the texture/image rotates along with the spinner.
+class GoRotatingTextureProgressSpinner(GoTextureProgressSpinnerBase):
+    '''Same as GoTextureProgressSpinner, but the texture/image rotates along with the spinner.
     '''
     pass
```

### Comparing `kivygo-0.0.4/kivygo/uix/radialslider.py` & `kivygo-0.0.5/kivygo/widgets/radialslider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from math import sin, cos, atan2, radians
-from kivy.uix.widget import Widget
+from kivygo.widgets.widget import GoWidget
 from kivy.graphics import Color, SmoothLine, Ellipse
 from kivy.properties import NumericProperty, ColorProperty, AliasProperty
 
 
-class RadialSlider(Widget):
+class GoRadialSlider(GoWidget):
     '''A :class:`~kivy.uix.widget.Widget` that provides a radial slider.
     '''
 
     angle = NumericProperty(0)
     '''
     Current angle used for the Radial Slider.
     You can use it for setting the angle of the thumb in the track in range
```

### Comparing `kivygo-0.0.4/kivygo/uix/rotabox.py` & `kivygo-0.0.5/kivygo/widgets/rotabox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,1521 +1,1522 @@
-00000000: 0d0a 6672 6f6d 206b 6976 792e 7569 782e  ..from kivy.uix.
-00000010: 7769 6467 6574 2069 6d70 6f72 7420 5769  widget import Wi
-00000020: 6467 6574 0d0a 6672 6f6d 206b 6976 792e  dget..from kivy.
-00000030: 7569 782e 696d 6167 6520 696d 706f 7274  uix.image import
-00000040: 2049 6d61 6765 0d0a 6672 6f6d 206b 6976   Image..from kiv
-00000050: 792e 636c 6f63 6b20 696d 706f 7274 2043  y.clock import C
-00000060: 6c6f 636b 0d0a 6672 6f6d 206b 6976 792e  lock..from kivy.
-00000070: 7665 6374 6f72 2069 6d70 6f72 7420 5665  vector import Ve
-00000080: 6374 6f72 0d0a 6672 6f6d 206b 6976 792e  ctor..from kivy.
-00000090: 6772 6170 6869 6373 2069 6d70 6f72 7420  graphics import 
-000000a0: 5075 7368 4d61 7472 6978 2c20 526f 7461  PushMatrix, Rota
-000000b0: 7465 2c20 506f 704d 6174 7269 780d 0a66  te, PopMatrix..f
-000000c0: 726f 6d20 6b69 7679 2e67 7261 7068 6963  rom kivy.graphic
-000000d0: 732e 636f 6e74 6578 745f 696e 7374 7275  s.context_instru
-000000e0: 6374 696f 6e73 2069 6d70 6f72 7420 436f  ctions import Co
-000000f0: 6c6f 720d 0a66 726f 6d20 6b69 7679 2e67  lor..from kivy.g
-00000100: 7261 7068 6963 732e 7665 7274 6578 5f69  raphics.vertex_i
-00000110: 6e73 7472 7563 7469 6f6e 7320 696d 706f  nstructions impo
-00000120: 7274 204c 696e 650d 0a66 726f 6d20 6b69  rt Line..from ki
-00000130: 7679 2e61 746c 6173 2069 6d70 6f72 7420  vy.atlas import 
-00000140: 4174 6c61 730d 0a0d 0a66 726f 6d20 6b69  Atlas....from ki
-00000150: 7679 2e70 726f 7065 7274 6965 7320 696d  vy.properties im
-00000160: 706f 7274 2028 0d0a 094e 756d 6572 6963  port (...Numeric
-00000170: 5072 6f70 6572 7479 2c20 5265 6665 7265  Property, Refere
-00000180: 6e63 654c 6973 7450 726f 7065 7274 792c  nceListProperty,
-00000190: 0d0a 0941 6c69 6173 5072 6f70 6572 7479  ...AliasProperty
-000001a0: 2c20 4f62 6a65 6374 5072 6f70 6572 7479  , ObjectProperty
-000001b0: 2c20 426f 6f6c 6561 6e50 726f 7065 7274  , BooleanPropert
-000001c0: 792c 0d0a 094c 6973 7450 726f 7065 7274  y,...ListPropert
-000001d0: 792c 2042 6f75 6e64 6564 4e75 6d65 7269  y, BoundedNumeri
-000001e0: 6350 726f 7065 7274 792c 0d0a 0953 7472  cProperty,...Str
-000001f0: 696e 6750 726f 7065 7274 790d 0a29 0d0a  ingProperty..)..
-00000200: 0d0a 6672 6f6d 206d 6174 6820 696d 706f  ..from math impo
-00000210: 7274 2072 6164 6961 6e73 2c20 7369 6e2c  rt radians, sin,
-00000220: 2063 6f73 0d0a 696d 706f 7274 206a 736f   cos..import jso
-00000230: 6e0d 0a0d 0a66 726f 6d20 6b69 7679 676f  n....from kivygo
-00000240: 2e62 6f75 6e64 735f 6d61 7468 2069 6d70  .bounds_math imp
-00000250: 6f72 7420 280d 0a09 7065 6572 732c 2064  ort (...peers, d
-00000260: 6566 696e 655f 626f 756e 6473 2c20 7265  efine_bounds, re
-00000270: 7369 7a65 2c0d 0a09 7570 6461 7465 5f62  size,...update_b
-00000280: 6f75 6e64 732c 2061 6e69 7265 7369 7a65  ounds, aniresize
-00000290: 2c20 616e 6975 7064 6174 655f 626f 756e  , aniupdate_boun
-000002a0: 6473 2c0d 0a09 706f 696e 745f 696e 5f62  ds,...point_in_b
-000002b0: 6f75 6e64 732c 2063 6f6c 6c69 6465 5f62  ounds, collide_b
-000002c0: 6f75 6e64 730d 0a29 0d0a 0d0a 0d0a 636c  ounds..)......cl
-000002d0: 6173 7320 526f 7461 626f 7828 5769 6467  ass Rotabox(Widg
-000002e0: 6574 293a 0d0a 0d0a 0973 6f75 7263 655f  et):.....source_
-000002f0: 6372 6f70 203d 2053 7472 696e 6750 726f  crop = StringPro
-00000300: 7065 7274 7928 2222 290d 0a0d 0a09 6375  perty("").....cu
-00000310: 7272 656e 745f 696d 6167 6520 3d20 5374  rrent_image = St
-00000320: 7269 6e67 5072 6f70 6572 7479 2822 626f  ringProperty("bo
-00000330: 756e 6473 2229 0d0a 0d0a 0973 6f75 7263  unds").....sourc
-00000340: 655f 626f 756e 6473 203d 2053 7472 696e  e_bounds = Strin
-00000350: 6750 726f 7065 7274 7928 2222 290d 0a0d  gProperty("")...
-00000360: 0a09 6174 6c61 7320 3d20 4f62 6a65 6374  ..atlas = Object
-00000370: 5072 6f70 6572 7479 284e 6f6e 6529 0d0a  Property(None)..
-00000380: 090d 0a0d 0a09 696d 6167 6520 3d20 4f62  ......image = Ob
-00000390: 6a65 6374 5072 6f70 6572 7479 284e 6f6e  jectProperty(Non
-000003a0: 6529 0d0a 0927 2727 5468 6973 2073 686f  e)...'''This sho
-000003b0: 756c 6420 6265 2074 6865 2069 6d61 6765  uld be the image
-000003c0: 2074 6861 7420 616e 7920 6375 7374 6f6d   that any custom
-000003d0: 2062 6f75 6e64 7320 6172 6520 6d65 616e   bounds are mean
-000003e0: 7420 666f 722e 0d0a 0949 6620 6e6f 7420  t for....If not 
-000003f0: 6465 6669 6e65 642c 2077 6964 6765 7420  defined, widget 
-00000400: 7769 6c6c 2074 7279 2074 6f20 6c6f 6361  will try to loca
-00000410: 7465 2074 6865 2074 6f70 6d6f 7374 2069  te the topmost i
-00000420: 6d61 6765 2069 6e20 6974 7320 7472 6565  mage in its tree
-00000430: 2e0d 0a09 2727 270d 0a0d 0a09 6173 7065  ....'''.....aspe
-00000440: 6374 5f72 6174 696f 203d 204e 756d 6572  ct_ratio = Numer
-00000450: 6963 5072 6f70 6572 7479 2830 2e30 290d  icProperty(0.0).
-00000460: 0a09 2727 2754 6865 2077 6964 6765 7427  ..'''The widget'
-00000470: 7320 6173 7065 6374 2072 6174 696f 2e20  s aspect ratio. 
-00000480: 4966 206e 6f74 2064 6566 696e 6564 2c20  If not defined, 
-00000490: 696d 6167 6527 7320 7261 7469 6f20 7769  image's ratio wi
-000004a0: 6c6c 2062 6520 7573 6564 2e0d 0a09 2727  ll be used....''
-000004b0: 270d 0a0d 0a09 616e 676c 6520 3d20 4e75  '.....angle = Nu
-000004c0: 6d65 7269 6350 726f 7065 7274 7928 3029  mericProperty(0)
-000004d0: 0d0a 0927 2727 416e 676c 6520 6f66 2052  ...'''Angle of R
-000004e0: 6f74 6174 696f 6e2e 0d0a 0927 2727 0d0a  otation....'''..
-000004f0: 0d0a 0d0a 0964 6566 2067 6574 5f6f 7269  .....def get_ori
-00000500: 6769 6e28 7365 6c66 293a 0d0a 0909 7265  gin(self):....re
-00000510: 7475 726e 2073 656c 662e 7069 766f 740d  turn self.pivot.
-00000520: 0a0d 0a09 6465 6620 7365 745f 6f72 6967  ....def set_orig
-00000530: 696e 2873 656c 662c 2070 6f69 6e74 293a  in(self, point):
-00000540: 0d0a 0909 616e 676c 6520 3d20 2d72 6164  ....angle = -rad
-00000550: 6961 6e73 2873 656c 662e 6c61 7374 5f61  ians(self.last_a
-00000560: 6e67 6c65 290d 0a09 096f 7269 6720 3d20  ngle)....orig = 
-00000570: 7365 6c66 2e6f 7269 6769 6e0d 0a09 0973  self.origin....s
-00000580: 203d 2073 696e 2861 6e67 6c65 290d 0a09   = sin(angle)...
-00000590: 0963 203d 2063 6f73 2861 6e67 6c65 290d  .c = cos(angle).
-000005a0: 0a0d 0a09 0923 206e 6f72 6d61 6c69 7a65  .....# normalize
-000005b0: 2028 7472 616e 736c 6174 6520 706f 696e   (translate poin
-000005c0: 7420 736f 206f 7269 6769 6e20 7769 6c6c  t so origin will
-000005d0: 2062 6520 302c 3029 0d0a 0909 6478 203d   be 0,0)....dx =
-000005e0: 2070 6f69 6e74 5b30 5d20 2d20 6f72 6967   point[0] - orig
-000005f0: 5b30 5d0d 0a09 0964 7920 3d20 706f 696e  [0]....dy = poin
-00000600: 745b 315d 202d 206f 7269 675b 315d 0d0a  t[1] - orig[1]..
-00000610: 0d0a 0909 2320 756e 2d72 6f74 6174 6520  ....# un-rotate 
-00000620: 706f 696e 740d 0a09 0978 6e65 7720 3d20  point....xnew = 
-00000630: 6478 202a 2063 202d 2064 7920 2a20 730d  dx * c - dy * s.
-00000640: 0a09 0979 6e65 7720 3d20 6478 202a 2073  ...ynew = dx * s
-00000650: 202b 2064 7920 2a20 630d 0a0d 0a09 0923   + dy * c......#
-00000660: 2074 7261 6e73 6c61 7465 2070 6f69 6e74   translate point
-00000670: 2062 6163 6b3a 0d0a 0909 7069 766f 7420   back:....pivot 
-00000680: 3d20 786e 6577 202b 206f 7269 675b 305d  = xnew + orig[0]
-00000690: 2c20 796e 6577 202b 206f 7269 675b 315d  , ynew + orig[1]
-000006a0: 0d0a 0d0a 0909 2320 6c6f 636b 2070 6f73  ......# lock pos
-000006b0: 2d70 6976 6f74 2072 656c 6174 696f 6e0d  -pivot relation.
-000006c0: 0a09 0973 656c 662e 7069 766f 745f 626f  ...self.pivot_bo
-000006d0: 6e64 203d 205b 2870 6976 6f74 5b30 5d20  nd = [(pivot[0] 
-000006e0: 2d20 7365 6c66 2e78 2920 2f20 666c 6f61  - self.x) / floa
-000006f0: 7428 7365 6c66 2e77 6964 7468 292c 0d0a  t(self.width),..
-00000700: 0909 0909 0909 2020 2028 7069 766f 745b  ......   (pivot[
-00000710: 315d 202d 2073 656c 662e 7929 202f 2066  1] - self.y) / f
-00000720: 6c6f 6174 2873 656c 662e 6865 6967 6874  loat(self.height
-00000730: 295d 0d0a 0d0a 0909 2320 5369 6e63 6520  )]......# Since 
-00000740: 7468 6520 696d 6167 6520 286f 6e20 6361  the image (on ca
-00000750: 6e76 6173 2920 616c 7761 7973 2073 7461  nvas) always sta
-00000760: 7274 7320 6561 6368 2066 7261 6d65 2069  rts each frame i
-00000770: 6e20 7a65 726f 2061 6e67 6c65 2c0d 0a09  n zero angle,...
-00000780: 0923 2061 6e20 5b6f 7269 6769 6e5d 2063  .# an [origin] c
-00000790: 6861 6e67 6520 696e 2061 6e79 206e 6f6e  hange in any non
-000007a0: 2d7a 6572 6f20 616e 676c 6520 6272 6561  -zero angle brea
-000007b0: 6b73 2074 6865 2063 6f6e 7469 6e75 6974  ks the continuit
-000007c0: 7920 6f66 0d0a 0909 2320 6d6f 7469 6f6e  y of....# motion
-000007d0: 2f72 6f74 6174 696f 6e2c 2069 6e74 726f  /rotation, intro
-000007e0: 6475 6369 6e67 2061 6e20 696d 6167 6520  ducing an image 
-000007f0: 7472 616e 736c 6174 696f 6e20 286a 756d  translation (jum
-00000800: 7029 2e0d 0a09 0923 2063 6f6d 7065 6e73  p).....# compens
-00000810: 6174 696e 6720 6279 2063 6861 6e67 696e  ating by changin
-00000820: 6720 7468 6520 7769 6467 6574 2773 2070  g the widget's p
-00000830: 6f73 6974 696f 6e2e 0d0a 0d0a 0909 2320  osition.......# 
-00000840: 7072 6576 656e 7420 6120 626f 756e 6473  prevent a bounds
-00000850: 2720 7570 6461 7465 2074 6f20 5b70 6f73  ' update to [pos
-00000860: 5d20 6368 616e 6765 2062 656c 6f77 2e0d  ] change below..
-00000870: 0a09 0973 656c 662e 616c 6c6f 7720 3d20  ...self.allow = 
-00000880: 300d 0a0d 0a09 0923 2063 6f6d 7065 6e73  0......# compens
-00000890: 6174 696e 6720 666f 7220 696d 6167 6520  ating for image 
-000008a0: 7472 616e 736c 6174 696f 6e0d 0a09 0973  translation....s
-000008b0: 656c 662e 706f 7320 3d20 2873 656c 662e  elf.pos = (self.
-000008c0: 7820 2d20 2870 6976 6f74 5b30 5d20 2d20  x - (pivot[0] - 
-000008d0: 706f 696e 745b 305d 292c 0d0a 0909 0909  point[0]),......
-000008e0: 0973 656c 662e 7920 2d20 2870 6976 6f74  .self.y - (pivot
-000008f0: 5b31 5d20 2d20 706f 696e 745b 315d 2929  [1] - point[1]))
-00000900: 0d0a 0d0a 0909 2320 6361 6e6e 6f74 2077  ......# cannot w
-00000910: 6169 7420 666f 7220 7468 6520 7472 6967  ait for the trig
-00000920: 6765 7265 6420 5b75 7064 6174 655d 2c20  gered [update], 
-00000930: 6174 2074 6865 2065 6e64 206f 6620 7468  at the end of th
-00000940: 6973 2066 7261 6d65 2c0d 0a09 0923 2073  is frame,....# s
-00000950: 696e 6365 2069 7420 6d69 6768 7420 636f  ince it might co
-00000960: 6e63 6572 6e20 6f74 6865 7220 6368 616e  ncern other chan
-00000970: 6765 7320 7468 6174 2072 6571 7569 7265  ges that require
-00000980: 2061 2062 6f75 6e64 7327 2075 7064 6174   a bounds' updat
-00000990: 652e 0d0a 0909 2320 7365 6c66 2e75 7064  e.....# self.upd
-000009a0: 6174 6528 290d 0a09 0973 656c 662e 7472  ate()....self.tr
-000009b0: 6967 6765 725f 7570 6461 7465 2829 0d0a  igger_update()..
-000009c0: 0d0a 096f 7269 6769 6e20 3d20 416c 6961  ...origin = Alia
-000009d0: 7350 726f 7065 7274 7928 6765 745f 6f72  sProperty(get_or
-000009e0: 6967 696e 2c20 7365 745f 6f72 6967 696e  igin, set_origin
-000009f0: 290d 0a09 2727 2753 6574 7320 7468 6520  )...'''Sets the 
-00000a00: 706f 696e 7420 6f66 2072 6f74 6174 696f  point of rotatio
-00000a10: 6e2e 2044 6566 6175 6c74 2076 616c 7565  n. Default value
-00000a20: 2069 7320 7468 6520 7769 6467 6574 2773   is the widget's
-00000a30: 2063 656e 7465 722e 0d0a 0957 6f72 6b73   center....Works
-00000a40: 206e 6963 656c 7920 7769 7468 2074 6865   nicely with the
-00000a50: 205b 6765 745f 706f 696e 745d 206d 6574   [get_point] met
-00000a60: 686f 6420 6265 6c6f 7720 616e 6420 706f  hod below and po
-00000a70: 696e 7473 2061 6c72 6561 6479 2064 6566  ints already def
-00000a80: 696e 6564 2069 6e0d 0a09 5b63 7573 746f  ined in...[custo
-00000a90: 6d5f 626f 756e 6473 5d2e 0d0a 0927 2727  m_bounds]....'''
-00000aa0: 0d0a 0d0a 0d0a 0961 6c6c 6f77 5f72 6f74  .......allow_rot
-00000ab0: 6162 6f78 203d 2042 6f6f 6c65 616e 5072  abox = BooleanPr
-00000ac0: 6f70 6572 7479 2854 7275 6529 0d0a 0927  operty(True)...'
-00000ad0: 2727 456e 6162 6c65 7320 7769 6467 6574  ''Enables widget
-00000ae0: 2773 2061 6476 616e 6365 6420 636f 6c6c  's advanced coll
-00000af0: 6973 696f 6e20 6465 7465 6374 696f 6e2e  ision detection.
-00000b00: 2049 6620 4661 6c73 652c 2077 6964 6765   If False, widge
-00000b10: 7420 7769 6c6c 0d0a 0963 6f6c 6c69 6465  t will...collide
-00000b20: 2061 7320 6120 6e6f 726d 616c 2028 6e6f   as a normal (no
-00000b30: 6e2d 526f 7461 626f 7829 2077 6964 6765  n-Rotabox) widge
-00000b40: 742e 0d0a 0927 2727 0d0a 0d0a 0963 7573  t....'''.....cus
-00000b50: 746f 6d5f 626f 756e 6473 203d 204f 626a  tom_bounds = Obj
-00000b60: 6563 7450 726f 7065 7274 7928 5b5b 2830  ectProperty([[(0
-00000b70: 2e2c 2030 2e29 2c20 2831 2e2c 2030 2e29  ., 0.), (1., 0.)
-00000b80: 2c20 2831 2e2c 2031 2e29 2c20 2830 2e2c  , (1., 1.), (0.,
-00000b90: 2031 2e29 5d5d 290d 0a09 2727 2743 7573   1.)]])...'''Cus
-00000ba0: 746f 6d20 626f 756e 6473 2720 6465 6669  tom bounds' defi
-00000bb0: 6e69 7469 6f6e 2069 6e74 6572 6661 6365  nition interface
-00000bc0: 2e20 2853 6565 206d 6f64 756c 6527 7320  . (See module's 
-00000bd0: 646f 6375 6d65 6e74 6174 696f 6e29 2e0d  documentation)..
-00000be0: 0a09 2727 270d 0a0d 0a09 7365 676d 656e  ..'''.....segmen
-00000bf0: 745f 6d6f 6465 203d 2042 6f6f 6c65 616e  t_mode = Boolean
-00000c00: 5072 6f70 6572 7479 2854 7275 6529 0d0a  Property(True)..
-00000c10: 0927 2727 436f 6c6c 6973 696f 6e20 6465  .'''Collision de
-00000c20: 7465 6374 696f 6e20 6d65 7468 6f64 2073  tection method s
-00000c30: 7769 7463 6820 2873 6565 2064 6f63 756d  witch (see docum
-00000c40: 656e 7461 7469 6f6e 2061 626f 7665 292e  entation above).
-00000c50: 0d0a 0927 2727 0d0a 0d0a 096f 7065 6e5f  ...'''.....open_
-00000c60: 626f 756e 6473 203d 204c 6973 7450 726f  bounds = ListPro
-00000c70: 7065 7274 7928 5b5d 290d 0a09 2727 2728  perty([])...'''(
-00000c80: 7365 676d 656e 745f 6d6f 6465 2920 4966  segment_mode) If
-00000c90: 2061 2070 6f6c 7967 6f6e 2773 2069 6e64   a polygon's ind
-00000ca0: 6578 2069 7320 696e 2074 6869 7320 6c69  ex is in this li
-00000cb0: 7374 2c20 7468 6520 7365 676d 656e 740d  st, the segment.
-00000cc0: 0a09 6265 7477 6565 6e20 7468 6520 6c61  ..between the la
-00000cd0: 7374 2061 6e64 2066 6972 7374 2070 6f69  st and first poi
-00000ce0: 6e74 7320 6f66 2074 6865 2070 6f6c 7967  nts of the polyg
-00000cf0: 6f6e 2069 7320 6e6f 7420 636f 6e73 6964  on is not consid
-00000d00: 6572 6564 2069 6e20 7468 650d 0a09 636f  ered in the...co
-00000d10: 6c6c 6973 696f 6e20 6368 6563 6b73 2e0d  llision checks..
-00000d20: 0a09 2727 270d 0a0d 0a09 7072 655f 6368  ..'''.....pre_ch
-00000d30: 6563 6b20 3d20 426f 6f6c 6561 6e50 726f  eck = BooleanPro
-00000d40: 7065 7274 7928 4661 6c73 6529 0d0a 0927  perty(False)...'
-00000d50: 2727 2843 7974 686f 6e29 2041 2063 6f6c  ''(Cython) A col
-00000d60: 6c69 7369 6f6e 206f 7074 696d 697a 6174  lision optimizat
-00000d70: 696f 6e20 7377 6974 6368 2066 6f72 206c  ion switch for l
-00000d80: 6172 6765 7220 7769 6467 6574 7320 2834  arger widgets (4
-00000d90: 352b 2070 6f69 6e74 7329 2e0d 0a09 4974  5+ points)....It
-00000da0: 2773 2061 6c77 6179 7320 5472 7565 2069  's always True i
-00000db0: 6e20 5079 7468 6f6e 2062 7574 2069 6e20  n Python but in 
-00000dc0: 4379 7468 6f6e 2c20 666f 7220 736d 616c  Cython, for smal
-00000dd0: 6c20 7769 6467 6574 732c 2074 6865 2073  l widgets, the s
-00000de0: 6c69 6768 7420 7461 7820 0d0a 0969 6e20  light tax ...in 
-00000df0: 7570 6461 7469 6e67 2074 6865 2062 6f75  updating the bou
-00000e00: 6e64 7320 6f75 7477 6569 6768 7320 7468  nds outweighs th
-00000e10: 6520 6265 6e65 6669 7420 696e 2063 6f6c  e benefit in col
-00000e20: 6c69 7369 6f6e 2e0d 0a09 2727 270d 0a0d  lision....'''...
-00000e30: 0a0d 0a09 6465 6620 6765 745f 616c 6c6f  ....def get_allo
-00000e40: 775f 6472 6167 2873 656c 6629 3a0d 0a09  w_drag(self):...
-00000e50: 0972 6574 7572 6e20 7365 6c66 2e61 6c6c  .return self.all
-00000e60: 6f77 5f64 7261 675f 782c 2073 656c 662e  ow_drag_x, self.
-00000e70: 616c 6c6f 775f 6472 6167 5f79 0d0a 0d0a  allow_drag_y....
-00000e80: 0964 6566 2073 6574 5f61 6c6c 6f77 5f64  .def set_allow_d
-00000e90: 7261 6728 7365 6c66 2c20 7661 6c75 6529  rag(self, value)
-00000ea0: 3a0d 0a09 0969 6620 7479 7065 2876 616c  :....if type(val
-00000eb0: 7565 2920 696e 2028 6c69 7374 2c20 7475  ue) in (list, tu
-00000ec0: 706c 6529 3a0d 0a09 0909 7365 6c66 2e61  ple):.....self.a
-00000ed0: 6c6c 6f77 5f64 7261 675f 782c 2073 656c  llow_drag_x, sel
-00000ee0: 662e 616c 6c6f 775f 6472 6167 5f79 203d  f.allow_drag_y =
-00000ef0: 2076 616c 7565 0d0a 0909 656c 7365 3a0d   value....else:.
-00000f00: 0a09 0909 7365 6c66 2e61 6c6c 6f77 5f64  ....self.allow_d
-00000f10: 7261 675f 7820 3d20 7365 6c66 2e61 6c6c  rag_x = self.all
-00000f20: 6f77 5f64 7261 675f 7920 3d20 626f 6f6c  ow_drag_y = bool
-00000f30: 2876 616c 7565 290d 0a0d 0a09 616c 6c6f  (value).....allo
-00000f40: 775f 6472 6167 203d 2041 6c69 6173 5072  w_drag = AliasPr
-00000f50: 6f70 6572 7479 2867 6574 5f61 6c6c 6f77  operty(get_allow
-00000f60: 5f64 7261 672c 2073 6574 5f61 6c6c 6f77  _drag, set_allow
-00000f70: 5f64 7261 672c 2062 696e 643d 2827 616c  _drag, bind=('al
-00000f80: 6c6f 775f 6472 6167 5f78 272c 2027 616c  low_drag_x', 'al
-00000f90: 6c6f 775f 6472 6167 5f79 2729 290d 0a09  low_drag_y'))...
-00000fa0: 2727 2741 6c6c 6f77 2074 6f75 6368 2074  '''Allow touch t
-00000fb0: 7261 6e73 6c61 7469 6f6e 206f 6e20 7468  ranslation on th
-00000fc0: 6520 5820 6f72 2059 2061 7869 732e 0d0a  e X or Y axis...
-00000fd0: 0927 2727 0d0a 0d0a 0961 6c6c 6f77 5f64  .'''.....allow_d
-00000fe0: 7261 675f 7820 3d20 426f 6f6c 6561 6e50  rag_x = BooleanP
-00000ff0: 726f 7065 7274 7928 4661 6c73 6529 0d0a  roperty(False)..
-00001000: 0927 2727 416c 6c6f 7720 746f 7563 6820  .'''Allow touch 
-00001010: 7472 616e 736c 6174 696f 6e20 6f6e 2074  translation on t
-00001020: 6865 2058 2061 7869 732e 0d0a 0927 2727  he X axis....'''
-00001030: 0d0a 0d0a 0961 6c6c 6f77 5f64 7261 675f  .....allow_drag_
-00001040: 7920 3d20 426f 6f6c 6561 6e50 726f 7065  y = BooleanPrope
-00001050: 7274 7928 4661 6c73 6529 0d0a 0927 2727  rty(False)...'''
-00001060: 416c 6c6f 7720 746f 7563 6820 7472 616e  Allow touch tran
-00001070: 736c 6174 696f 6e20 6f6e 2074 6865 2059  slation on the Y
-00001080: 2061 7869 732e 0d0a 0927 2727 0d0a 0d0a   axis....'''....
-00001090: 0d0a 0973 696e 676c 655f 746f 7563 685f  ...single_touch_
-000010a0: 726f 7461 7469 6f6e 203d 2042 6f6f 6c65  rotation = Boole
-000010b0: 616e 5072 6f70 6572 7479 2846 616c 7365  anProperty(False
-000010c0: 290d 0a09 2727 2741 6c6c 6f77 2072 6f74  )...'''Allow rot
-000010d0: 6174 696f 6e20 6172 6f75 6e64 205b 6f72  ation around [or
-000010e0: 6967 696e 5d2e 0d0a 0927 2727 0d0a 0d0a  igin]....'''....
-000010f0: 0973 696e 676c 655f 746f 7563 685f 7363  .single_touch_sc
-00001100: 616c 696e 6720 3d20 426f 6f6c 6561 6e50  aling = BooleanP
-00001110: 726f 7065 7274 7928 4661 6c73 6529 0d0a  roperty(False)..
-00001120: 0927 2727 416c 6c6f 7720 7363 616c 696e  .'''Allow scalin
-00001130: 6720 6172 6f75 6e64 205b 6f72 6967 696e  g around [origin
-00001140: 5d2e 0d0a 0927 2727 0d0a 0d0a 096d 756c  ]....'''.....mul
-00001150: 7469 5f74 6f75 6368 5f72 6f74 6174 696f  ti_touch_rotatio
-00001160: 6e20 3d20 426f 6f6c 6561 6e50 726f 7065  n = BooleanPrope
-00001170: 7274 7928 4661 6c73 6529 0d0a 0927 2727  rty(False)...'''
-00001180: 416c 6c6f 7720 6d75 6c74 6974 6f75 6368  Allow multitouch
-00001190: 2072 6f74 6174 696f 6e2e 205b 6f72 6967   rotation. [orig
-000011a0: 696e 5d20 6973 2064 6566 696e 6564 2065  in] is defined e
-000011b0: 6163 6820 7469 6d65 2062 7920 7468 6520  ach time by the 
-000011c0: 746f 7563 682e 0d0a 0927 2727 0d0a 0d0a  touch....'''....
-000011d0: 096d 756c 7469 5f74 6f75 6368 5f73 6361  .multi_touch_sca
-000011e0: 6c69 6e67 203d 2042 6f6f 6c65 616e 5072  ling = BooleanPr
-000011f0: 6f70 6572 7479 2846 616c 7365 290d 0a09  operty(False)...
-00001200: 2727 2741 6c6c 6f77 206d 756c 7469 746f  '''Allow multito
-00001210: 7563 6820 7363 616c 696e 672e 205b 6f72  uch scaling. [or
-00001220: 6967 696e 5d20 6973 2064 6566 696e 6564  igin] is defined
-00001230: 2065 6163 6820 7469 6d65 2062 7920 7468   each time by th
-00001240: 6520 746f 7563 682e 0d0a 0927 2727 0d0a  e touch....'''..
-00001250: 0d0a 0973 696e 676c 655f 6472 6167 5f74  ...single_drag_t
-00001260: 6f75 6368 203d 2042 6f75 6e64 6564 4e75  ouch = BoundedNu
-00001270: 6d65 7269 6350 726f 7065 7274 7928 312c  mericProperty(1,
-00001280: 206d 696e 3d31 290d 0a09 2727 2748 6f77   min=1)...'''How
-00001290: 206d 616e 7920 746f 7563 6865 7320 7769   many touches wi
-000012a0: 6c6c 2062 6520 7472 6561 7465 6420 6173  ll be treated as
-000012b0: 206f 6e65 2073 696e 676c 6520 6472 6167   one single drag
-000012c0: 2074 6f75 6368 2e0d 0a09 2727 270d 0a0d   touch....'''...
-000012d0: 0a09 7369 6e67 6c65 5f74 7261 6e73 5f74  ..single_trans_t
-000012e0: 6f75 6368 203d 2042 6f75 6e64 6564 4e75  ouch = BoundedNu
-000012f0: 6d65 7269 6350 726f 7065 7274 7928 312c  mericProperty(1,
-00001300: 206d 696e 3d31 290d 0a09 2727 2748 6f77   min=1)...'''How
-00001310: 206d 616e 7920 746f 7563 6865 7320 7769   many touches wi
-00001320: 6c6c 2062 6520 7472 6561 7465 6420 6173  ll be treated as
-00001330: 206f 6e65 2073 696e 676c 6520 726f 7461   one single rota
-00001340: 7469 6f6e 2f73 6361 6c69 6e67 2074 6f75  tion/scaling tou
-00001350: 6368 2e0d 0a09 2727 270d 0a0d 0a09 746f  ch....'''.....to
-00001360: 7563 6865 645f 746f 5f66 726f 6e74 203d  uched_to_front =
-00001370: 2042 6f6f 6c65 616e 5072 6f70 6572 7479   BooleanProperty
-00001380: 2846 616c 7365 290d 0a09 2727 2749 6620  (False)...'''If 
-00001390: 746f 7563 6865 642c 2077 6964 6765 7420  touched, widget 
-000013a0: 7769 6c6c 2062 6520 7075 7368 6564 2074  will be pushed t
-000013b0: 6f20 7468 6520 746f 7020 6f66 2070 6172  o the top of par
-000013c0: 656e 7420 7769 6467 6574 2074 7265 652e  ent widget tree.
-000013d0: 0d0a 0927 2727 0d0a 0d0a 0963 6f6c 6c69  ...'''.....colli
-000013e0: 6465 5f61 6674 6572 5f63 6869 6c64 7265  de_after_childre
-000013f0: 6e20 3d20 426f 6f6c 6561 6e50 726f 7065  n = BooleanPrope
-00001400: 7274 7928 4661 6c73 6529 0d0a 0927 2727  rty(False)...'''
-00001410: 4966 2054 7275 652c 206c 696d 6974 696e  If True, limitin
-00001420: 6720 7468 6520 746f 7563 6820 696e 7369  g the touch insi
-00001430: 6465 2074 6865 2062 6f75 6e64 7320 7769  de the bounds wi
-00001440: 6c6c 2062 6520 646f 6e65 2061 6674 6572  ll be done after
-00001450: 0d0a 0964 6973 7061 6368 696e 6720 7468  ...dispaching th
-00001460: 6520 746f 7563 6820 746f 2074 6865 2063  e touch to the c
-00001470: 6869 6c64 2061 6e64 2067 7261 6e64 6368  hild and grandch
-00001480: 696c 6472 656e 2c20 736f 2065 7665 6e20  ildren, so even 
-00001490: 6f75 7473 6964 6520 7468 650d 0a09 626f  outside the...bo
-000014a0: 756e 6473 2074 6865 7920 6361 6e20 7374  unds they can st
-000014b0: 696c 6c20 6265 2074 6f75 6368 6564 2e0d  ill be touched..
-000014c0: 0a09 494d 504f 5254 414e 5420 4e4f 5445  ..IMPORTANT NOTE
-000014d0: 3a20 4772 616e 6463 6869 6c64 7265 6e2c  : Grandchildren,
-000014e0: 2069 6e73 6964 6520 6f72 206f 7574 7369   inside or outsi
-000014f0: 6465 2074 6865 2062 6f75 6e64 732c 2063  de the bounds, c
-00001500: 616e 2063 6f6c 6c69 6465 0d0a 0909 696e  an collide....in
-00001510: 6465 7065 6e64 656e 746c 7920 4f4e 4c59  dependently ONLY
-00001520: 2069 6620 7769 6467 6574 2069 7320 4e4f   if widget is NO
-00001530: 5420 524f 5441 5445 4420 285b 616e 676c  T ROTATED ([angl
-00001540: 655d 206d 7573 7420 6265 2030 292e 0d0a  e] must be 0)...
-00001550: 0927 2727 0d0a 0d0a 0d0a 0964 6566 2067  .'''.......def g
-00001560: 6574 5f73 6361 6c65 2873 656c 6629 3a0d  et_scale(self):.
-00001570: 0a09 0972 6574 7572 6e20 666c 6f61 7428  ...return float(
-00001580: 7365 6c66 2e77 6964 7468 2920 2f20 7365  self.width) / se
-00001590: 6c66 2e6f 7269 6769 6e61 6c5f 7369 7a65  lf.original_size
-000015a0: 5b30 5d0d 0a0d 0a09 6465 6620 7365 745f  [0].....def set_
-000015b0: 7363 616c 6528 7365 6c66 2c20 616d 6f75  scale(self, amou
-000015c0: 6e74 293a 0d0a 0909 6966 2061 6d6f 756e  nt):....if amoun
-000015d0: 7420 3c20 7365 6c66 2e73 6361 6c65 5f6d  t < self.scale_m
-000015e0: 696e 3a0d 0a09 0909 616d 6f75 6e74 203d  in:.....amount =
-000015f0: 2073 656c 662e 7363 616c 655f 6d69 6e0d   self.scale_min.
-00001600: 0a09 0965 6c69 6620 616d 6f75 6e74 203e  ...elif amount >
-00001610: 2073 656c 662e 7363 616c 655f 6d61 783a   self.scale_max:
-00001620: 0d0a 0909 0961 6d6f 756e 7420 3d20 7365  .....amount = se
-00001630: 6c66 2e73 6361 6c65 5f6d 6178 0d0a 0d0a  lf.scale_max....
-00001640: 0909 7069 766f 7420 3d20 7365 6c66 2e70  ..pivot = self.p
-00001650: 6976 6f74 5b3a 5d0d 0a09 0973 656c 662e  ivot[:]....self.
-00001660: 7369 7a65 203d 2028 616d 6f75 6e74 202a  size = (amount *
-00001670: 2073 656c 662e 6f72 6967 696e 616c 5f73   self.original_s
-00001680: 697a 655b 305d 2c0d 0a09 0909 0909 2061  ize[0],....... a
-00001690: 6d6f 756e 7420 2a20 7365 6c66 2e6f 7269  mount * self.ori
-000016a0: 6769 6e61 6c5f 7369 7a65 5b31 5d29 0d0a  ginal_size[1])..
-000016b0: 0909 7365 6c66 2e70 6976 6f74 203d 2070  ..self.pivot = p
-000016c0: 6976 6f74 0d0a 0909 6966 2073 656c 662e  ivot....if self.
-000016d0: 696e 6974 6961 6c5f 7363 616c 653a 0d0a  initial_scale:..
-000016e0: 0909 0972 6574 7572 6e0d 0a09 0973 656c  ...return....sel
-000016f0: 662e 696e 6974 6961 6c5f 7363 616c 6520  f.initial_scale 
-00001700: 3d20 7365 6c66 2e73 6361 6c65 0d0a 090d  = self.scale....
-00001710: 0a09 7363 616c 6520 3d20 416c 6961 7350  ..scale = AliasP
-00001720: 726f 7065 7274 7928 6765 745f 7363 616c  roperty(get_scal
-00001730: 652c 2073 6574 5f73 6361 6c65 2c20 6269  e, set_scale, bi
-00001740: 6e64 3d28 2777 6964 7468 272c 2027 6865  nd=('width', 'he
-00001750: 6967 6874 272c 2027 6f72 6967 696e 616c  ight', 'original
-00001760: 5f73 697a 6527 2929 0d0a 0927 2727 0d0a  _size'))...'''..
-00001770: 0957 6964 6765 7427 7320 6375 7272 656e  .Widget's curren
-00001780: 7420 7363 616c 652e 2043 616c 6375 6c61  t scale. Calcula
-00001790: 7465 6420 6672 6f6d 205b 6f72 6967 696e  ted from [origin
-000017a0: 616c 5f73 697a 655d 2028 7573 6572 2773  al_size] (user's
-000017b0: 2069 6e70 7574 0d0a 095b 7369 7a65 5d20   input...[size] 
-000017c0: 6f72 205b 696d 6167 655d 2773 205b 7465  or [image]'s [te
-000017d0: 7874 7572 655f 7369 7a65 5d29 2e20 5573  xture_size]). Us
-000017e0: 6564 2066 6f72 2074 6f75 6368 2073 6361  ed for touch sca
-000017f0: 6c69 6e67 2062 7574 2069 7420 6361 6e20  ling but it can 
-00001800: 6265 2061 6e0d 0a09 616c 7465 726e 6174  be an...alternat
-00001810: 6976 6520 746f 205b 7369 7a65 5d2e 0d0a  ive to [size]...
-00001820: 0927 2727 0d0a 0d0a 0973 6361 6c65 5f6d  .'''.....scale_m
-00001830: 696e 203d 204e 756d 6572 6963 5072 6f70  in = NumericProp
-00001840: 6572 7479 2830 2e30 3129 0d0a 0927 2727  erty(0.01)...'''
-00001850: 4d69 6e69 6d75 6d20 7363 616c 6520 616c  Minimum scale al
-00001860: 6c6f 7765 642e 0d0a 0927 2727 0d0a 0d0a  lowed....'''....
-00001870: 0973 6361 6c65 5f6d 6178 203d 204e 756d  .scale_max = Num
-00001880: 6572 6963 5072 6f70 6572 7479 2831 6532  ericProperty(1e2
-00001890: 3029 0d0a 0927 2727 4d61 7869 6d75 6d20  0)...'''Maximum 
-000018a0: 7363 616c 6520 616c 6c6f 7765 642e 0d0a  scale allowed...
-000018b0: 0927 2727 0d0a 0d0a 0d0a 0964 6566 2067  .'''.......def g
-000018c0: 6574 5f70 6976 6f74 5f78 2873 656c 6629  et_pivot_x(self)
-000018d0: 3a0d 0a09 0972 6574 7572 6e20 7365 6c66  :....return self
-000018e0: 2e78 202b 2073 656c 662e 7769 6474 6820  .x + self.width 
-000018f0: 2a20 7365 6c66 2e70 6976 6f74 5f62 6f6e  * self.pivot_bon
-00001900: 645b 305d 0d0a 0d0a 0964 6566 2073 6574  d[0].....def set
-00001910: 5f70 6976 6f74 5f78 2873 656c 662c 2076  _pivot_x(self, v
-00001920: 616c 7565 293a 0d0a 0909 6966 2073 656c  alue):....if sel
-00001930: 662e 7769 6474 6820 3e20 313a 0d0a 0909  f.width > 1:....
-00001940: 0973 656c 662e 7820 3d20 7661 6c75 6520  .self.x = value 
-00001950: 2d20 7365 6c66 2e77 6964 7468 202a 2073  - self.width * s
-00001960: 656c 662e 7069 766f 745f 626f 6e64 5b30  elf.pivot_bond[0
-00001970: 5d0d 0a09 0965 6c69 6620 7661 6c75 6520  ]....elif value 
-00001980: 3e20 313a 0d0a 0909 0973 656c 662e 7465  > 1:.....self.te
-00001990: 6d70 5f70 6976 5f78 203d 2076 616c 7565  mp_piv_x = value
-000019a0: 0d0a 0d0a 0964 6566 2067 6574 5f70 6976  .....def get_piv
-000019b0: 6f74 5f79 2873 656c 6629 3a0d 0a09 0972  ot_y(self):....r
-000019c0: 6574 7572 6e20 7365 6c66 2e79 202b 2073  eturn self.y + s
-000019d0: 656c 662e 6865 6967 6874 202a 2073 656c  elf.height * sel
-000019e0: 662e 7069 766f 745f 626f 6e64 5b31 5d0d  f.pivot_bond[1].
-000019f0: 0a0d 0a09 6465 6620 7365 745f 7069 766f  ....def set_pivo
-00001a00: 745f 7928 7365 6c66 2c20 7661 6c75 6529  t_y(self, value)
-00001a10: 3a0d 0a09 0969 6620 7365 6c66 2e68 6569  :....if self.hei
-00001a20: 6768 7420 3e20 313a 0d0a 0909 0973 656c  ght > 1:.....sel
-00001a30: 662e 7920 3d20 7661 6c75 6520 2d20 7365  f.y = value - se
-00001a40: 6c66 2e68 6569 6768 7420 2a20 7365 6c66  lf.height * self
-00001a50: 2e70 6976 6f74 5f62 6f6e 645b 315d 0d0a  .pivot_bond[1]..
-00001a60: 0909 656c 6966 2076 616c 7565 203e 2031  ..elif value > 1
-00001a70: 3a0d 0a09 0909 7365 6c66 2e74 656d 705f  :.....self.temp_
-00001a80: 7069 765f 7920 3d20 7661 6c75 650d 0a0d  piv_y = value...
-00001a90: 0a09 7069 766f 745f 7820 3d20 416c 6961  ..pivot_x = Alia
-00001aa0: 7350 726f 7065 7274 7928 6765 745f 7069  sProperty(get_pi
-00001ab0: 766f 745f 782c 2073 6574 5f70 6976 6f74  vot_x, set_pivot
-00001ac0: 5f78 2c20 6269 6e64 3d28 2778 272c 2027  _x, bind=('x', '
-00001ad0: 7769 6474 6827 2c20 2770 6976 6f74 5f62  width', 'pivot_b
-00001ae0: 6f6e 6427 2929 0d0a 0970 6976 6f74 5f79  ond'))...pivot_y
-00001af0: 203d 2041 6c69 6173 5072 6f70 6572 7479   = AliasProperty
-00001b00: 2867 6574 5f70 6976 6f74 5f79 2c20 7365  (get_pivot_y, se
-00001b10: 745f 7069 766f 745f 792c 2062 696e 643d  t_pivot_y, bind=
-00001b20: 2827 7927 2c20 2768 6569 6768 7427 2c20  ('y', 'height', 
-00001b30: 2770 6976 6f74 5f62 6f6e 6427 2929 0d0a  'pivot_bond'))..
-00001b40: 0970 6976 6f74 203d 2052 6566 6572 656e  .pivot = Referen
-00001b50: 6365 4c69 7374 5072 6f70 6572 7479 2870  ceListProperty(p
-00001b60: 6976 6f74 5f78 2c20 7069 766f 745f 7929  ivot_x, pivot_y)
-00001b70: 0d0a 0927 2727 0d0a 0950 6f69 6e74 206f  ...'''...Point o
-00001b80: 6620 726f 7461 7469 6f6e 2061 6e64 2073  f rotation and s
-00001b90: 6361 6c69 6e67 2e0d 0a09 5768 696c 6520  caling....While 
-00001ba0: 5b6f 7269 6769 6e5d 2070 726f 7065 7274  [origin] propert
-00001bb0: 7920 7365 7473 205b 7069 766f 745d 2773  y sets [pivot]'s
-00001bc0: 2072 656c 6174 696f 6e20 746f 2077 6964   relation to wid
-00001bd0: 6765 742c 205b 7069 766f 745d 0d0a 0969  get, [pivot]...i
-00001be0: 7473 656c 6620 6361 6e20 6265 2075 7365  tself can be use
-00001bf0: 6420 746f 2070 6f73 6974 696f 6e20 7468  d to position th
-00001c00: 6520 7769 6467 6574 2c20 6d75 6368 206c  e widget, much l
-00001c10: 696b 6520 5b70 6f73 5d20 6f72 205b 6365  ike [pos] or [ce
-00001c20: 6e74 6572 5d2e 0d0a 0927 2727 0d0a 0d0a  nter]....'''....
-00001c30: 0970 7265 7061 7265 6420 3d20 426f 6f6c  .prepared = Bool
-00001c40: 6561 6e50 726f 7065 7274 7928 4661 6c73  eanProperty(Fals
-00001c50: 6529 0d0a 0927 2727 0d0a 0949 7473 2073  e)...'''...Its s
-00001c60: 7461 7465 2063 6861 6e67 6520 7369 676e  tate change sign
-00001c70: 6966 6965 7320 6120 7265 7365 742e 2054  ifies a reset. T
-00001c80: 6865 2072 6573 6574 2063 6f6d 706c 6574  he reset complet
-00001c90: 696f 6e20 7369 676e 616c 2c20 686f 7765  ion signal, howe
-00001ca0: 7665 722c 0d0a 0969 7320 7468 6520 636f  ver,...is the co
-00001cb0: 6e73 6571 7565 6e74 205b 7265 6164 795d  nsequent [ready]
-00001cc0: 2073 7461 7465 2063 6861 6e67 6520 746f   state change to
-00001cd0: 2054 7275 652e 0d0a 0927 2727 0d0a 0d0a   True....'''....
-00001ce0: 0964 7261 775f 626f 756e 6473 203d 2042  .draw_bounds = B
-00001cf0: 6f6f 6c65 616e 5072 6f70 6572 7479 2846  ooleanProperty(F
-00001d00: 616c 7365 290d 0a09 2727 2745 6e61 626c  alse)...'''Enabl
-00001d10: 6573 2062 6f75 6e64 7320 7669 7375 616c  es bounds visual
-00001d20: 697a 6174 696f 6e20 2866 6f72 2074 6573  ization (for tes
-00001d30: 7469 6e67 292e 0d0a 0927 2727 0d0a 0d0a  ting)....'''....
-00001d40: 0d0a 095f 5f65 7665 6e74 735f 5f20 3d20  ...__events__ = 
-00001d50: 2827 6f6e 5f74 7261 6e73 666f 726d 5f77  ('on_transform_w
-00001d60: 6974 685f 746f 7563 6827 2c20 276f 6e5f  ith_touch', 'on_
-00001d70: 746f 7563 6865 645f 746f 5f66 726f 6e74  touched_to_front
-00001d80: 2729 0d0a 0d0a 0964 6566 206f 6e5f 7472  ').....def on_tr
-00001d90: 616e 7366 6f72 6d5f 7769 7468 5f74 6f75  ansform_with_tou
-00001da0: 6368 2873 656c 662c 2074 6f75 6368 293a  ch(self, touch):
-00001db0: 0d0a 0909 2727 270d 0a09 0943 616c 6c65  ....'''....Calle
-00001dc0: 6420 7768 656e 2061 2074 6f75 6368 2065  d when a touch e
-00001dd0: 7665 6e74 2068 6173 2074 7261 6e73 666f  vent has transfo
-00001de0: 726d 6564 2074 6865 2077 6964 6765 742e  rmed the widget.
-00001df0: 0d0a 0909 4279 2064 6566 6175 6c74 2074  ....By default t
-00001e00: 6869 7320 646f 6573 206e 6f74 6869 6e67  his does nothing
-00001e10: 2c20 6275 7420 6361 6e20 6265 206f 7665  , but can be ove
-00001e20: 7272 6964 656e 2062 7920 6465 7269 7665  rriden by derive
-00001e30: 640d 0a09 0963 6c61 7373 6573 2074 6861  d....classes tha
-00001e40: 7420 6e65 6564 2074 6f20 7265 6163 7420  t need to react 
-00001e50: 746f 2074 7261 6e73 666f 726d 6174 696f  to transformatio
-00001e60: 6e73 2063 6175 7365 6420 6279 2075 7365  ns caused by use
-00001e70: 720d 0a09 0969 6e70 7574 2e0d 0a09 0927  r....input.....'
-00001e80: 2727 0d0a 0909 7061 7373 0d0a 0d0a 0964  ''....pass.....d
-00001e90: 6566 206f 6e5f 746f 7563 6865 645f 746f  ef on_touched_to
-00001ea0: 5f66 726f 6e74 2873 656c 662c 2074 6f75  _front(self, tou
-00001eb0: 6368 293a 0d0a 0909 2727 270d 0a09 0943  ch):....'''....C
-00001ec0: 616c 6c65 6420 7768 656e 2061 2074 6f75  alled when a tou
-00001ed0: 6368 2065 7665 6e74 2063 6175 7365 7320  ch event causes 
-00001ee0: 7468 6520 7769 6467 6574 2074 6f20 6265  the widget to be
-00001ef0: 2062 726f 7567 6874 2074 6f20 7468 650d   brought to the.
-00001f00: 0a09 0966 726f 6e74 206f 6620 7468 6520  ...front of the 
-00001f10: 7061 7265 6e74 2028 6f6e 6c79 2069 6620  parent (only if 
-00001f20: 3a61 7474 723a 6074 6f75 6368 6564 5f74  :attr:`touched_t
-00001f30: 6f5f 6672 6f6e 7460 2069 7320 5472 7565  o_front` is True
-00001f40: 290d 0a09 0927 2727 0d0a 0909 7061 7373  )....'''....pass
-00001f50: 0d0a 0d0a 0d0a 0964 6566 205f 5f69 6e69  .......def __ini
-00001f60: 745f 5f28 7365 6c66 2c20 2a2a 6b77 6172  t__(self, **kwar
-00001f70: 6773 293a 0d0a 0909 7365 6c66 2e73 697a  gs):....self.siz
-00001f80: 6520 3d20 5b31 2c20 315d 0d0a 0909 7365  e = [1, 1]....se
-00001f90: 6c66 2e74 656d 705f 7069 765f 7820 3d20  lf.temp_piv_x = 
-00001fa0: 7365 6c66 2e74 656d 705f 7069 765f 7920  self.temp_piv_y 
-00001fb0: 3d20 300d 0a09 0973 656c 662e 696e 6974  = 0....self.init
-00001fc0: 6961 6c5f 7363 616c 6520 3d20 300d 0a09  ial_scale = 0...
-00001fd0: 0973 656c 662e 746f 7563 6865 7320 3d20  .self.touches = 
-00001fe0: 5b5d 0d0a 0909 7365 6c66 2e6c 6173 745f  []....self.last_
-00001ff0: 746f 7563 685f 706f 7320 3d20 7b7d 0d0a  touch_pos = {}..
-00002000: 0909 0d0a 0909 7375 7065 7228 292e 5f5f  ......super().__
-00002010: 696e 6974 5f5f 282a 2a6b 7761 7267 7329  init__(**kwargs)
-00002020: 0d0a 0909 0d0a 0909 7365 6c66 2e69 6d61  ........self.ima
-00002030: 6765 203d 2049 6d61 6765 2829 0d0a 0909  ge = Image()....
-00002040: 7365 6c66 2e73 697a 6564 5f62 795f 696d  self.sized_by_im
-00002050: 6720 3d20 4661 6c73 650d 0a09 0973 656c  g = False....sel
-00002060: 662e 7261 7469 6f20 3d20 310d 0a09 0973  f.ratio = 1....s
-00002070: 656c 662e 6c61 7374 5f70 6f73 203d 205b  elf.last_pos = [
-00002080: 302c 2030 5d0d 0a09 0973 656c 662e 6c61  0, 0]....self.la
-00002090: 7374 5f73 697a 6520 3d20 7365 6c66 2e73  st_size = self.s
-000020a0: 697a 655b 3a5d 0d0a 0909 7365 6c66 2e6c  ize[:]....self.l
-000020b0: 6173 745f 616e 676c 6520 3d20 300d 0a09  ast_angle = 0...
-000020c0: 0973 656c 662e 616e 696d 203d 2046 616c  .self.anim = Fal
-000020d0: 7365 0d0a 0909 7365 6c66 2e72 6964 203d  se....self.rid =
-000020e0: 2030 0d0a 0909 7365 6c66 2e63 7572 725f   0....self.curr_
-000020f0: 6b65 7920 3d20 2762 6f75 6e64 7327 0d0a  key = 'bounds'..
-00002100: 0909 7365 6c66 2e64 7261 775f 636f 6c6f  ..self.draw_colo
-00002110: 7220 3d20 436f 6c6f 7228 7267 6261 3d5b  r = Color(rgba=[
-00002120: 302e 3239 2c20 302e 3531 382c 2031 2c20  0.29, 0.518, 1, 
-00002130: 315d 290d 0a09 0973 656c 662e 626f 785f  1])....self.box_
-00002140: 636f 6c6f 7220 3d20 436f 6c6f 7228 7267  color = Color(rg
-00002150: 6261 3d5b 302e 3335 2c20 302e 3135 2c20  ba=[0.35, 0.15, 
-00002160: 302c 2031 5d29 0d0a 0909 7365 6c66 2e64  0, 1])....self.d
-00002170: 7261 775f 6c69 6e65 7320 3d20 5b5d 0d0a  raw_lines = []..
-00002180: 0909 7365 6c66 2e62 6f78 5f6c 696e 6573  ..self.box_lines
-00002190: 203d 205b 5d0d 0a09 0973 656c 662e 726f   = []....self.ro
-000021a0: 7461 7469 6f6e 203d 2052 6f74 6174 6528  tation = Rotate(
-000021b0: 616e 676c 653d 302c 206f 7269 6769 6e3d  angle=0, origin=
-000021c0: 7365 6c66 2e63 656e 7465 7229 0d0a 0909  self.center)....
-000021d0: 7365 6c66 2e63 616e 7661 732e 6265 666f  self.canvas.befo
-000021e0: 7265 2e61 6464 2850 7573 684d 6174 7269  re.add(PushMatri
-000021f0: 7828 2929 0d0a 0909 7365 6c66 2e63 616e  x())....self.can
-00002200: 7661 732e 6265 666f 7265 2e61 6464 2873  vas.before.add(s
-00002210: 656c 662e 726f 7461 7469 6f6e 290d 0a09  elf.rotation)...
-00002220: 0973 656c 662e 6361 6e76 6173 2e61 6674  .self.canvas.aft
-00002230: 6572 2e61 6464 2850 6f70 4d61 7472 6978  er.add(PopMatrix
-00002240: 2829 290d 0a0d 0a09 0973 656c 662e 7472  ())......self.tr
-00002250: 6967 6765 725f 7570 6461 7465 203d 2043  igger_update = C
-00002260: 6c6f 636b 2e63 7265 6174 655f 7472 6967  lock.create_trig
-00002270: 6765 7228 7365 6c66 2e75 7064 6174 652c  ger(self.update,
-00002280: 202d 3129 0d0a 0909 7365 6c66 2e74 7269   -1)....self.tri
-00002290: 6767 6572 5f64 7261 7720 3d20 436c 6f63  gger_draw = Cloc
-000022a0: 6b2e 6372 6561 7465 5f74 7269 6767 6572  k.create_trigger
-000022b0: 2873 656c 662e 6472 6177 2c20 2d31 290d  (self.draw, -1).
-000022c0: 0a0d 0a09 0973 656c 662e 6269 6e64 280d  .....self.bind(.
-000022d0: 0a09 0909 6368 696c 6472 656e 3d73 656c  ....children=sel
-000022e0: 662e 7472 6967 6765 725f 7570 6461 7465  f.trigger_update
-000022f0: 2c0d 0a09 0909 7061 7265 6e74 3d73 656c  ,.....parent=sel
-00002300: 662e 7472 6967 6765 725f 7570 6461 7465  f.trigger_update
-00002310: 2c0d 0a09 0909 706f 733d 7365 6c66 2e74  ,.....pos=self.t
-00002320: 7269 6767 6572 5f75 7064 6174 652c 0d0a  rigger_update,..
-00002330: 0909 0970 6f73 5f68 696e 743d 7365 6c66  ...pos_hint=self
-00002340: 2e74 7269 6767 6572 5f75 7064 6174 652c  .trigger_update,
-00002350: 0d0a 0909 0961 6e67 6c65 3d73 656c 662e  .....angle=self.
-00002360: 7472 6967 6765 725f 7570 6461 7465 2c0d  trigger_update,.
-00002370: 0a09 0909 696d 6167 653d 7365 6c66 2e6f  ....image=self.o
-00002380: 6e5f 7265 7365 742c 0d0a 0909 0961 7370  n_reset,.....asp
-00002390: 6563 745f 7261 7469 6f3d 7365 6c66 2e6f  ect_ratio=self.o
-000023a0: 6e5f 7265 7365 742c 0d0a 0909 0963 7573  n_reset,.....cus
-000023b0: 746f 6d5f 626f 756e 6473 3d73 656c 662e  tom_bounds=self.
-000023c0: 6f6e 5f72 6573 6574 2c0d 0a09 0909 616c  on_reset,.....al
-000023d0: 6c6f 775f 726f 7461 626f 783d 7365 6c66  low_rotabox=self
-000023e0: 2e6f 6e5f 7265 7365 742c 0d0a 0909 0964  .on_reset,.....d
-000023f0: 7261 775f 626f 756e 6473 3d73 656c 662e  raw_bounds=self.
-00002400: 6f6e 5f72 6573 6574 0d0a 0909 290d 0a09  on_reset....)...
-00002410: 0d0a 0964 6566 2061 6464 5f77 6964 6765  ...def add_widge
-00002420: 7428 7365 6c66 2c20 7769 6467 6574 2c20  t(self, widget, 
-00002430: 2a2a 6b77 6172 6773 293a 0d0a 0909 6966  **kwargs):....if
-00002440: 2073 656c 662e 6368 696c 6472 656e 3a0d   self.children:.
-00002450: 0a09 0909 7261 6973 6520 4578 6365 7074  ....raise Except
-00002460: 696f 6e28 2752 6f74 6162 6f78 2063 616e  ion('Rotabox can
-00002470: 206f 6e6c 7920 6861 7665 206f 6e65 2063   only have one c
-00002480: 6869 6c64 2e27 290d 0a09 0973 7570 6572  hild.')....super
-00002490: 2829 2e61 6464 5f77 6964 6765 7428 7769  ().add_widget(wi
-000024a0: 6467 6574 290d 0a0d 0a09 6465 6620 6f6e  dget).....def on
-000024b0: 5f6f 7065 6e5f 626f 756e 6473 2873 656c  _open_bounds(sel
-000024c0: 662c 202a 6172 6773 293a 0d0a 0909 6966  f, *args):....if
-000024d0: 2073 656c 662e 6f70 656e 5f62 6f75 6e64   self.open_bound
-000024e0: 7320 616e 6420 6e6f 7420 7365 6c66 2e73  s and not self.s
-000024f0: 6567 6d65 6e74 5f6d 6f64 653a 0d0a 0909  egment_mode:....
-00002500: 0972 6169 7365 2045 7863 6570 7469 6f6e  .raise Exception
-00002510: 2827 4f70 656e 2062 6f75 6e64 7320 6172  ('Open bounds ar
-00002520: 6520 6f6e 6c79 2061 7070 6c69 6361 626c  e only applicabl
-00002530: 6520 696e 2053 6567 6d65 6e74 206d 6f64  e in Segment mod
-00002540: 652e 2729 0d0a 0d0a 0964 6566 206f 6e5f  e.').....def on_
-00002550: 736f 7572 6365 5f62 6f75 6e64 7328 7365  source_bounds(se
-00002560: 6c66 2c20 2a61 7267 7329 3a0d 0a09 0973  lf, *args):....s
-00002570: 656c 662e 6375 7374 6f6d 5f62 6f75 6e64  elf.custom_bound
-00002580: 7320 3d20 7365 6c66 2e72 6561 645f 626f  s = self.read_bo
-00002590: 756e 6473 2873 656c 662e 736f 7572 6365  unds(self.source
-000025a0: 5f62 6f75 6e64 7329 0d0a 0d0a 0964 6566  _bounds).....def
-000025b0: 206f 6e5f 6375 7272 656e 745f 696d 6167   on_current_imag
-000025c0: 6528 7365 6c66 2c20 2a61 7267 7329 3a0d  e(self, *args):.
-000025d0: 0a09 0969 6620 7365 6c66 2e61 746c 6173  ...if self.atlas
-000025e0: 203d 3d20 4e6f 6e65 3a0d 0a09 0909 7265   == None:.....re
-000025f0: 7475 726e 204e 6f6e 650d 0a09 090d 0a09  turn None.......
-00002600: 0973 656c 662e 696d 6167 652e 7465 7874  .self.image.text
-00002610: 7572 6520 3d20 7365 6c66 2e61 746c 6173  ure = self.atlas
-00002620: 2e74 6578 7475 7265 735b 7365 6c66 2e63  .textures[self.c
-00002630: 7572 7265 6e74 5f69 6d61 6765 5d0d 0a09  urrent_image]...
-00002640: 0973 656c 662e 7072 6570 6172 6564 203d  .self.prepared =
-00002650: 2046 616c 7365 0d0a 0909 7365 6c66 2e74   False....self.t
-00002660: 7269 6767 6572 5f75 7064 6174 6528 290d  rigger_update().
-00002670: 0a0d 0a09 6465 6620 6f6e 5f73 6f75 7263  ....def on_sourc
-00002680: 655f 6372 6f70 2873 656c 662c 202a 6172  e_crop(self, *ar
-00002690: 6773 293a 0d0a 0909 6966 2073 656c 662e  gs):....if self.
-000026a0: 736f 7572 6365 5f63 726f 7020 3d3d 2022  source_crop == "
-000026b0: 223a 0d0a 0909 0973 656c 662e 6174 6c61  ":.....self.atla
-000026c0: 7320 3d20 4e6f 6e65 0d0a 0909 0973 656c  s = None.....sel
-000026d0: 662e 696d 6167 6520 3d20 4e6f 6e65 0d0a  f.image = None..
-000026e0: 0909 0973 656c 662e 636c 6561 725f 7769  ...self.clear_wi
-000026f0: 6467 6574 7328 290d 0a09 0909 7265 7475  dgets().....retu
-00002700: 726e 204e 6f6e 650d 0a09 090d 0a09 0969  rn None........i
-00002710: 6620 7365 6c66 2e69 6d61 6765 2021 3d20  f self.image != 
-00002720: 4e6f 6e65 2061 6e64 206e 6f74 2073 656c  None and not sel
-00002730: 662e 696d 6167 6520 696e 2073 656c 662e  f.image in self.
-00002740: 6368 696c 6472 656e 3a0d 0a09 0909 7365  children:.....se
-00002750: 6c66 2e61 6464 5f77 6964 6765 7428 7365  lf.add_widget(se
-00002760: 6c66 2e69 6d61 6765 290d 0a09 090d 0a09  lf.image).......
-00002770: 0973 656c 662e 6174 6c61 7320 3d20 4174  .self.atlas = At
-00002780: 6c61 7328 7365 6c66 2e73 6f75 7263 655f  las(self.source_
-00002790: 6372 6f70 290d 0a09 0973 656c 662e 696d  crop)....self.im
-000027a0: 6167 652e 7465 7874 7572 6520 3d20 7475  age.texture = tu
-000027b0: 706c 6528 7365 6c66 2e61 746c 6173 2e74  ple(self.atlas.t
-000027c0: 6578 7475 7265 732e 7661 6c75 6573 2829  extures.values()
-000027d0: 295b 305d 0d0a 0909 0d0a 0964 6566 206f  )[0].......def o
-000027e0: 6e5f 7369 7a65 2873 656c 662c 202a 6172  n_size(self, *ar
-000027f0: 6773 293a 0d0a 0909 7365 6c66 2e74 7269  gs):....self.tri
-00002800: 6767 6572 5f75 7064 6174 6528 290d 0a0d  gger_update()...
-00002810: 0a09 6465 6620 6f6e 5f72 6573 6574 2873  ..def on_reset(s
-00002820: 656c 662c 202a 6172 6773 293a 0d0a 0909  elf, *args):....
-00002830: 7365 6c66 2e74 7269 6767 6572 5f75 7064  self.trigger_upd
-00002840: 6174 6528 290d 0a0d 0a09 6465 6620 7265  ate().....def re
-00002850: 7365 745f 6472 6177 5f62 6f75 6e64 7328  set_draw_bounds(
-00002860: 7365 6c66 2c20 2a61 7267 7329 3a0d 0a09  self, *args):...
-00002870: 0966 6f72 206c 696e 6520 696e 2073 656c  .for line in sel
-00002880: 662e 6472 6177 5f6c 696e 6573 3a0d 0a09  f.draw_lines:...
-00002890: 0909 7365 6c66 2e63 616e 7661 732e 6166  ..self.canvas.af
-000028a0: 7465 722e 7265 6d6f 7665 286c 696e 6529  ter.remove(line)
-000028b0: 0d0a 0909 7365 6c66 2e64 7261 775f 6c69  ....self.draw_li
-000028c0: 6e65 7320 3d20 5b5d 0d0a 0d0a 0909 666f  nes = []......fo
-000028d0: 7220 6c69 6e65 2069 6e20 7365 6c66 2e62  r line in self.b
-000028e0: 6f78 5f6c 696e 6573 3a0d 0a09 0909 7365  ox_lines:.....se
-000028f0: 6c66 2e63 616e 7661 732e 6166 7465 722e  lf.canvas.after.
-00002900: 7265 6d6f 7665 286c 696e 6529 0d0a 0909  remove(line)....
-00002910: 7365 6c66 2e62 6f78 5f6c 696e 6573 203d  self.box_lines =
-00002920: 205b 5d0d 0a0d 0a09 6465 6620 7072 6570   [].....def prep
-00002930: 6172 6528 7365 6c66 2c20 6e3d 4e6f 6e65  are(self, n=None
-00002940: 2c20 2a61 7267 7329 3a0d 0a09 0973 656c  , *args):....sel
-00002950: 662e 7072 6570 6172 6564 203d 2054 7275  f.prepared = Tru
-00002960: 650d 0a09 0974 656d 7073 6361 6c65 203d  e....tempscale =
-00002970: 2073 656c 662e 696e 6974 6961 6c5f 7363   self.initial_sc
-00002980: 616c 650d 0a0d 0a09 0969 6620 7365 6c66  ale......if self
-00002990: 2e73 6f75 7263 655f 6372 6f70 206f 7220  .source_crop or 
-000029a0: 7365 6c66 2e69 6d61 6765 3a0d 0a09 0909  self.image:.....
-000029b0: 7472 793a 0d0a 0909 0909 7365 6c66 2e69  try:......self.i
-000029c0: 6d61 6765 2e74 6578 7475 7265 2e6d 6167  mage.texture.mag
-000029d0: 5f66 696c 7465 7220 3d20 276e 6561 7265  _filter = 'neare
-000029e0: 7374 270d 0a09 0909 6578 6365 7074 2041  st'.....except A
-000029f0: 7474 7269 6275 7465 4572 726f 723a 0d0a  ttributeError:..
-00002a00: 0909 0909 7061 7373 0d0a 0d0a 0909 0973  ....pass.......s
-00002a10: 656c 662e 696d 6167 652e 616c 6c6f 775f  elf.image.allow_
-00002a20: 7374 7265 7463 6820 3d20 5472 7565 0d0a  stretch = True..
-00002a30: 0d0a 0909 0923 2043 616c 6375 6c61 7469  .....# Calculati
-00002a40: 6e67 2077 6964 6765 7427 7320 7369 7a65  ng widget's size
-00002a50: 2066 726f 6d20 6176 6169 6c61 626c 6520   from available 
-00002a60: 696e 7075 7473 2e0d 0a09 0909 6966 2028  inputs......if (
-00002a70: 6e6f 7420 2873 656c 662e 7769 6474 6820  not (self.width 
-00002a80: 2d20 7465 6d70 7363 616c 6520 3e20 3120  - tempscale > 1 
-00002a90: 6f72 2073 656c 662e 6865 6967 6874 202d  or self.height -
-00002aa0: 2074 656d 7073 6361 6c65 203e 2031 2920   tempscale > 1) 
-00002ab0: 6f72 2073 656c 662e 7369 7a65 645f 6279  or self.sized_by
-00002ac0: 5f69 6d67 293a 0d0a 0909 0909 7472 793a  _img):......try:
-00002ad0: 0d0a 0909 0909 0973 656c 662e 6f72 6967  .......self.orig
-00002ae0: 696e 616c 5f73 697a 6520 3d20 7365 6c66  inal_size = self
-00002af0: 2e69 6d61 6765 2e74 6578 7475 7265 2e73  .image.texture.s
-00002b00: 697a 650d 0a09 0909 0965 7863 6570 7420  ize......except 
-00002b10: 4174 7472 6962 7574 6545 7272 6f72 3a0d  AttributeError:.
-00002b20: 0a09 0909 0909 2320 4966 2061 6e69 6d61  ......# If anima
-00002b30: 7469 6f6e 2c20 7465 7874 7572 6520 6e6f  tion, texture no
-00002b40: 7420 7265 6164 7920 283f 290d 0a09 0909  t ready (?).....
-00002b50: 0909 7365 6c66 2e6f 7269 6769 6e61 6c5f  ..self.original_
-00002b60: 7369 7a65 203d 2073 656c 662e 696d 6167  size = self.imag
-00002b70: 652e 7369 7a65 0d0a 0d0a 0909 0909 6966  e.size........if
-00002b80: 206e 6f74 2074 656d 7073 6361 6c65 3a0d   not tempscale:.
-00002b90: 0a09 0909 0909 7465 6d70 7363 616c 6520  ......tempscale 
-00002ba0: 3d20 310d 0a09 0909 0973 656c 662e 7369  = 1......self.si
-00002bb0: 7a65 203d 206c 6973 7428 6d61 7028 6c61  ze = list(map(la
-00002bc0: 6d62 6461 206e 3a20 286e 202a 2074 656d  mbda n: (n * tem
-00002bd0: 7073 6361 6c65 292c 2073 656c 662e 6f72  pscale), self.or
-00002be0: 6967 696e 616c 5f73 697a 6529 290d 0a0d  iginal_size))...
-00002bf0: 0a09 0909 0969 6620 7365 6c66 2e73 697a  .....if self.siz
-00002c00: 6564 5f62 795f 696d 673a 0d0a 0909 0909  ed_by_img:......
-00002c10: 0964 7720 3d20 7365 6c66 2e77 6964 7468  .dw = self.width
-00002c20: 202d 2073 656c 662e 6c61 7374 5f73 697a   - self.last_siz
-00002c30: 655b 305d 0d0a 0909 0909 0964 6820 3d20  e[0].......dh = 
-00002c40: 7365 6c66 2e68 6569 6768 7420 2d20 7365  self.height - se
-00002c50: 6c66 2e6c 6173 745f 7369 7a65 5b31 5d0d  lf.last_size[1].
-00002c60: 0a09 0909 0909 7365 6c66 2e70 6976 6f74  ......self.pivot
-00002c70: 203d 2028 2028 7365 6c66 2e70 6976 6f74   = ( (self.pivot
-00002c80: 5f78 202d 2064 7720 2a20 302e 3529 2c20  _x - dw * 0.5), 
-00002c90: 2873 656c 662e 7069 766f 745f 7920 2d20  (self.pivot_y - 
-00002ca0: 6468 202a 2030 2e35 2920 290d 0a09 0909  dh * 0.5) ).....
-00002cb0: 656c 7365 3a0d 0a09 0909 0973 656c 662e  else:......self.
-00002cc0: 6f72 6967 696e 616c 5f73 697a 6520 3d20  original_size = 
-00002cd0: 7365 6c66 2e73 697a 655b 3a5d 0d0a 0909  self.size[:]....
-00002ce0: 0909 6966 2074 656d 7073 6361 6c65 3a0d  ..if tempscale:.
-00002cf0: 0a09 0909 0909 7365 6c66 2e73 697a 6520  ......self.size 
-00002d00: 3d20 6c69 7374 286d 6170 286c 616d 6264  = list(map(lambd
-00002d10: 6120 6e3a 2028 6e20 2a20 7465 6d70 7363  a n: (n * tempsc
-00002d20: 616c 6529 2c20 7365 6c66 2e73 697a 6529  ale), self.size)
-00002d30: 290d 0a09 0965 6c73 653a 0d0a 0909 0973  )....else:.....s
-00002d40: 656c 662e 6f72 6967 696e 616c 5f73 697a  elf.original_siz
-00002d50: 6520 3d20 7365 6c66 2e73 697a 655b 3a5d  e = self.size[:]
-00002d60: 0d0a 0909 0969 6620 6e6f 7420 7465 6d70  .....if not temp
-00002d70: 7363 616c 653a 0d0a 0909 0909 7465 6d70  scale:......temp
-00002d80: 7363 616c 6520 3d20 310d 0a09 0909 7365  scale = 1.....se
-00002d90: 6c66 2e73 697a 6520 3d20 6c69 7374 286d  lf.size = list(m
-00002da0: 6170 286c 616d 6264 6120 6e3a 2028 6e20  ap(lambda n: (n 
-00002db0: 2a20 7465 6d70 7363 616c 6529 2c20 7365  * tempscale), se
-00002dc0: 6c66 2e73 697a 6529 290d 0a0d 0a09 0923  lf.size))......#
-00002dd0: 2053 6574 7469 6e67 2074 6865 2077 6964   Setting the wid
-00002de0: 6765 7427 7320 7261 7469 6f2e 0d0a 0909  get's ratio.....
-00002df0: 6966 206e 6f74 2073 656c 662e 6173 7065  if not self.aspe
-00002e00: 6374 5f72 6174 696f 3a0d 0a09 0909 6966  ct_ratio:.....if
-00002e10: 2073 656c 662e 736f 7572 6365 5f63 726f   self.source_cro
-00002e20: 7020 616e 6420 7365 6c66 2e73 697a 6564  p and self.sized
-00002e30: 5f62 795f 696d 673a 0d0a 0909 0909 7365  _by_img:......se
-00002e40: 6c66 2e72 6174 696f 203d 2073 656c 662e  lf.ratio = self.
-00002e50: 696d 6167 652e 696d 6167 655f 7261 7469  image.image_rati
-00002e60: 6f0d 0a09 0909 656c 7365 3a0d 0a09 0909  o.....else:.....
-00002e70: 0973 656c 662e 7261 7469 6f20 3d20 2873  .self.ratio = (s
-00002e80: 656c 662e 7769 6474 6820 2f20 666c 6f61  elf.width / floa
-00002e90: 7428 7365 6c66 2e68 6569 6768 7429 290d  t(self.height)).
-00002ea0: 0a09 0965 6c73 653a 0d0a 0909 0973 656c  ...else:.....sel
-00002eb0: 662e 7261 7469 6f20 3d20 7365 6c66 2e61  f.ratio = self.a
-00002ec0: 7370 6563 745f 7261 7469 6f0d 0a0d 0a09  spect_ratio.....
-00002ed0: 0923 2049 6620 5b73 697a 655d 2069 7320  .# If [size] is 
-00002ee0: 6e6f 7420 7370 6563 6966 6965 6420 6578  not specified ex
-00002ef0: 706c 6963 6974 6c79 2062 7920 7468 6520  plicitly by the 
-00002f00: 7573 6572 2c20 616e 7920 696e 7075 7420  user, any input 
-00002f10: 7661 6c75 6573 0d0a 0909 2320 666f 7220  values....# for 
-00002f20: 5b70 6976 6f74 5d20 6172 6520 7769 7468  [pivot] are with
-00002f30: 6865 6c64 2069 6e20 5b74 656d 705f 7069  held in [temp_pi
-00002f40: 765f 785d 2061 6e64 205b 7465 6d70 5f70  v_x] and [temp_p
-00002f50: 6976 5f79 5d2c 2075 6e74 696c 0d0a 0909  iv_y], until....
-00002f60: 2320 5b73 697a 655d 2067 6574 7320 6974  # [size] gets it
-00002f70: 7320 7661 6c75 6573 2066 726f 6d20 5b69  s values from [i
-00002f80: 6d61 6765 5d2e 2054 6865 6e2c 205b 7069  mage]. Then, [pi
-00002f90: 766f 745d 2067 6574 7320 7468 6520 7769  vot] gets the wi
-00002fa0: 7468 6865 6c64 0d0a 0909 2320 7661 6c75  thheld....# valu
-00002fb0: 6573 2c20 6865 7265 2e0d 0a09 0969 6620  es, here.....if 
-00002fc0: 7365 6c66 2e74 656d 705f 7069 765f 7820  self.temp_piv_x 
-00002fd0: 6f72 2073 656c 662e 7465 6d70 5f70 6976  or self.temp_piv
-00002fe0: 5f79 3a0d 0a09 0909 7365 6c66 2e70 6976  _y:.....self.piv
-00002ff0: 6f74 203d 2073 656c 662e 7465 6d70 5f70  ot = self.temp_p
-00003000: 6976 5f78 2c20 7365 6c66 2e74 656d 705f  iv_x, self.temp_
-00003010: 7069 765f 790d 0a09 0909 7365 6c66 2e74  piv_y.....self.t
-00003020: 656d 705f 7069 765f 7820 3d20 7365 6c66  emp_piv_x = self
-00003030: 2e74 656d 705f 7069 765f 7920 3d20 300d  .temp_piv_y = 0.
-00003040: 0a0d 0a09 0969 6620 7365 6c66 2e61 6c6c  .....if self.all
-00003050: 6f77 5f72 6f74 6162 6f78 3a0d 0a09 0909  ow_rotabox:.....
-00003060: 2320 4765 6e65 7261 7469 6e67 2061 2075  # Generating a u
-00003070: 6e69 7175 6520 6b65 7920 666f 7220 6561  nique key for ea
-00003080: 6368 2069 6e73 7461 6e63 650d 0a09 0909  ch instance.....
-00003090: 7472 793a 0d0a 0909 0909 7365 6c66 2e72  try:......self.r
-000030a0: 6964 203d 2073 6f72 7465 6428 7065 6572  id = sorted(peer
-000030b0: 732e 6b65 7973 2829 295b 2d31 5d20 2b20  s.keys())[-1] + 
-000030c0: 310d 0a09 0909 6578 6365 7074 2049 6e64  1.....except Ind
-000030d0: 6578 4572 726f 723a 0d0a 0909 0909 7061  exError:......pa
-000030e0: 7373 0d0a 0d0a 0909 0969 6620 6973 696e  ss.......if isin
-000030f0: 7374 616e 6365 2873 656c 662e 6375 7374  stance(self.cust
-00003100: 6f6d 5f62 6f75 6e64 732c 2064 6963 7429  om_bounds, dict)
-00003110: 3a0d 0a09 0909 0973 656c 662e 6375 7272  :......self.curr
-00003120: 5f6b 6579 203d 2073 656c 662e 6375 7272  _key = self.curr
-00003130: 656e 745f 696d 6167 650d 0a09 0909 0973  ent_image......s
-00003140: 656c 662e 616e 696d 203d 2054 7275 650d  elf.anim = True.
-00003150: 0a09 0909 0d0a 0909 0964 6566 696e 655f  .........define_
-00003160: 626f 756e 6473 2873 656c 662e 6375 7374  bounds(self.cust
-00003170: 6f6d 5f62 6f75 6e64 732c 2073 656c 662e  om_bounds, self.
-00003180: 6f70 656e 5f62 6f75 6e64 732c 2073 656c  open_bounds, sel
-00003190: 662e 7365 676d 656e 745f 6d6f 6465 2c20  f.segment_mode, 
-000031a0: 7365 6c66 2e72 6964 2c20 7365 6c66 2e70  self.rid, self.p
-000031b0: 7265 5f63 6865 636b 290d 0a09 0909 0d0a  re_check).......
-000031c0: 0909 0969 6620 7365 6c66 2e64 7261 775f  ...if self.draw_
-000031d0: 626f 756e 6473 3a0d 0a09 0909 0973 656c  bounds:......sel
-000031e0: 662e 7365 745f 6472 6177 2829 0d0a 0909  f.set_draw()....
-000031f0: 0909 7365 6c66 2e62 696e 6428 0d0a 0909  ..self.bind(....
-00003200: 0909 0963 6869 6c64 7265 6e3d 7365 6c66  ...children=self
-00003210: 2e74 7269 6767 6572 5f64 7261 772c 0d0a  .trigger_draw,..
-00003220: 0909 0909 0970 6172 656e 743d 7365 6c66  .....parent=self
-00003230: 2e74 7269 6767 6572 5f64 7261 772c 0d0a  .trigger_draw,..
-00003240: 0909 0909 0970 6f73 3d73 656c 662e 7472  .....pos=self.tr
-00003250: 6967 6765 725f 6472 6177 2c0d 0a09 0909  igger_draw,.....
-00003260: 0909 706f 735f 6869 6e74 3d73 656c 662e  ..pos_hint=self.
-00003270: 7472 6967 6765 725f 6472 6177 2c0d 0a09  trigger_draw,...
-00003280: 0909 0909 616e 676c 653d 7365 6c66 2e74  ....angle=self.t
-00003290: 7269 6767 6572 5f64 7261 772c 0d0a 0909  rigger_draw,....
-000032a0: 0909 290d 0a0d 0a09 0973 656c 662e 7472  ..)......self.tr
-000032b0: 6967 6765 725f 7570 6461 7465 2829 0d0a  igger_update()..
-000032c0: 0d0a 0964 6566 2067 6574 5f70 6f69 6e74  ...def get_point
-000032d0: 2873 656c 662c 2070 6f6c 5f69 6e64 6578  (self, pol_index
-000032e0: 2c20 706f 696e 745f 696e 6465 7829 3a0d  , point_index):.
-000032f0: 0a09 0927 2727 4163 6365 7373 2061 2070  ...'''Access a p
-00003300: 6f69 6e74 2773 2063 7572 7265 6e74 2070  oint's current p
-00003310: 6f73 6974 696f 6e2c 2062 6173 6564 206f  osition, based o
-00003320: 6e20 5b63 7573 746f 6d5f 626f 756e 6473  n [custom_bounds
-00003330: 5d20 7374 7275 6374 7572 652e 2727 270d  ] structure.'''.
-00003340: 0a09 0962 6f75 6e64 7320 3d20 7065 6572  ...bounds = peer
-00003350: 735b 7365 6c66 2e72 6964 5d5b 7365 6c66  s[self.rid][self
-00003360: 2e63 7572 725f 6b65 795d 0d0a 0909 696e  .curr_key]....in
-00003370: 6465 7820 3d20 2873 756d 2862 6f75 6e64  dex = (sum(bound
-00003380: 735b 2770 6f6c 5f6c 656e 7327 5d5b 3a70  s['pol_lens'][:p
-00003390: 6f6c 5f69 6e64 6578 5d29 202b 2070 6f69  ol_index]) + poi
-000033a0: 6e74 5f69 6e64 6578 2920 2a20 320d 0a09  nt_index) * 2...
-000033b0: 0972 6574 7572 6e20 6c69 7374 2862 6f75  .return list(bou
-000033c0: 6e64 735b 2770 6f69 6e74 7327 5d5b 696e  nds['points'][in
-000033d0: 6465 783a 696e 6465 7820 2b20 325d 290d  dex:index + 2]).
-000033e0: 0a0d 0a09 6465 6620 7265 6164 5f62 6f75  ....def read_bou
-000033f0: 6e64 7328 7365 6c66 2c20 6669 6c65 6e61  nds(self, filena
-00003400: 6d65 2c20 6465 6c61 7965 643d 4661 6c73  me, delayed=Fals
-00003410: 652c 202a 6172 6773 293a 0d0a 0909 2727  e, *args):....''
-00003420: 270d 0a09 0944 6566 696e 6520 5b63 7573  '....Define [cus
-00003430: 746f 6d5f 626f 756e 6473 5d20 7573 696e  tom_bounds] usin
-00003440: 6720 6120 726f 7461 626f 7865 7227 7320  g a rotaboxer's 
-00003450: 7072 6f6a 6563 7420 6669 6c65 2e0d 0a09  project file....
-00003460: 0954 6f20 776f 726b 2c20 5b73 697a 655d  .To work, [size]
-00003470: 2073 686f 756c 6420 6265 2061 6c72 6561   should be alrea
-00003480: 6479 2064 6566 696e 6564 2e0d 0a09 0927  dy defined.....'
-00003490: 2727 0d0a 0909 7072 6f6a 6563 7420 3d20  ''....project = 
-000034a0: 4e6f 6e65 0d0a 090d 0a09 0974 7279 3a0d  None.......try:.
-000034b0: 0a09 0909 7769 7468 206f 7065 6e28 6669  ....with open(fi
-000034c0: 6c65 6e61 6d65 2c20 2772 272c 2065 6e63  lename, 'r', enc
-000034d0: 6f64 696e 673d 2255 5446 3822 2920 6173  oding="UTF8") as
-000034e0: 2070 726f 6a3a 0d0a 0909 0909 7072 6f6a   proj:......proj
-000034f0: 6563 7420 3d20 6a73 6f6e 2e6c 6f61 6428  ect = json.load(
-00003500: 7072 6f6a 290d 0a09 0965 7863 6570 7420  proj)....except 
-00003510: 2849 4f45 7272 6f72 2c20 4b65 7945 7272  (IOError, KeyErr
-00003520: 6f72 2920 6173 2065 723a 0d0a 0909 0970  or) as er:.....p
-00003530: 7269 6e74 2827 4f6e 2072 6561 645f 626f  rint('On read_bo
-00003540: 756e 6473 3a20 272c 2065 7229 0d0a 0909  unds: ', er)....
-00003550: 0972 6574 7572 6e20 4e6f 6e65 0d0a 0909  .return None....
-00003560: 0d0a 0909 626f 756e 6473 203d 207b 7d0d  ....bounds = {}.
-00003570: 0a09 096f 7065 6e73 203d 205b 5d0d 0a09  ...opens = []...
-00003580: 0966 6f72 2066 2c20 6672 616d 6520 696e  .for f, frame in
-00003590: 2070 726f 6a65 6374 2e69 7465 6d73 2829   project.items()
-000035a0: 3a0d 0a09 0909 6966 2066 2069 6e20 2827  :.....if f in ('
-000035b0: 696d 6167 6527 2c20 2776 6572 7369 6f6e  image', 'version
-000035c0: 2729 3a0d 0a09 0909 0963 6f6e 7469 6e75  '):......continu
-000035d0: 650d 0a0d 0a09 0909 706f 6c73 203d 205b  e.......pols = [
-000035e0: 5d0d 0a09 0909 6920 3d20 300d 0a09 0909  ].....i = 0.....
-000035f0: 7768 696c 6520 6920 3c20 6c65 6e28 6672  while i < len(fr
-00003600: 616d 6529 3a0d 0a09 0909 0966 6f72 2070  ame):......for p
-00003610: 6f6c 2069 6e20 6672 616d 652e 7661 6c75  ol in frame.valu
-00003620: 6573 2829 3a0d 0a09 0909 0909 6966 2070  es():.......if p
-00003630: 6f6c 5b27 6e75 6d62 6572 275d 203d 3d20  ol['number'] == 
-00003640: 693a 0d0a 0909 0909 0909 706f 6c73 2e61  i:........pols.a
-00003650: 7070 656e 6428 706f 6c29 0d0a 0909 0909  ppend(pol)......
-00003660: 0909 6272 6561 6b0d 0a09 0909 0969 202b  ..break......i +
-00003670: 3d20 310d 0a09 0909 626f 756e 6473 5b66  = 1.....bounds[f
-00003680: 5d20 3d20 5b5d 0d0a 0909 0966 6f72 2070  ] = [].....for p
-00003690: 2c20 706f 6c20 696e 2065 6e75 6d65 7261  , pol in enumera
-000036a0: 7465 2870 6f6c 7329 3a0d 0a09 0909 0974  te(pols):......t
-000036b0: 7279 3a0d 0a09 0909 0909 6966 2070 6f6c  ry:.......if pol
-000036c0: 5b27 6f70 656e 275d 3a0d 0a09 0909 0909  ['open']:.......
-000036d0: 096f 7065 6e73 2e61 7070 656e 6428 7029  .opens.append(p)
-000036e0: 0d0a 0909 0909 6578 6365 7074 204b 6579  ......except Key
-000036f0: 4572 726f 723a 0d0a 0909 0909 0970 6173  Error:.......pas
-00003700: 730d 0a09 0909 090d 0a09 0909 0962 6f75  s............bou
-00003710: 6e64 735b 665d 2e61 7070 656e 6428 5b28  nds[f].append([(
-00003720: 726f 756e 6428 666c 6f61 7428 706f 696e  round(float(poin
-00003730: 745b 305d 2920 2f20 7365 6c66 2e77 6964  t[0]) / self.wid
-00003740: 7468 2c20 3329 2c0d 0a09 0909 0909 0909  th, 3),.........
-00003750: 0909 726f 756e 6428 666c 6f61 7428 706f  ..round(float(po
-00003760: 696e 745b 315d 2920 2f20 7365 6c66 2e68  int[1]) / self.h
-00003770: 6569 6768 742c 2033 2929 0d0a 0909 0909  eight, 3))......
-00003780: 0909 0909 0966 6f72 2070 6f69 6e74 2069  .....for point i
-00003790: 6e20 706f 6c5b 2770 6f69 6e74 7327 5d5d  n pol['points']]
-000037a0: 290d 0a0d 0a09 0962 6c65 6e20 3d20 6c65  )......blen = le
-000037b0: 6e28 626f 756e 6473 290d 0a09 0969 6620  n(bounds)....if 
-000037c0: 626c 656e 3a0d 0a09 0909 6966 206f 7065  blen:.....if ope
-000037d0: 6e73 3a0d 0a09 0909 0973 656c 662e 6f70  ns:......self.op
-000037e0: 656e 5f62 6f75 6e64 7320 3d20 6f70 656e  en_bounds = open
-000037f0: 730d 0a0d 0a09 0909 6966 2062 6c65 6e20  s.......if blen 
-00003800: 3d3d 2031 3a0d 0a09 0909 0962 6f75 6e64  == 1:......bound
-00003810: 7320 3d20 626f 756e 6473 5b6c 6973 7428  s = bounds[list(
-00003820: 626f 756e 6473 2e6b 6579 7328 2929 5b30  bounds.keys())[0
-00003830: 5d5d 0d0a 0d0a 0909 0969 6620 6465 6c61  ]].......if dela
-00003840: 7965 643a 0d0a 0909 0909 7365 6c66 2e63  yed:......self.c
-00003850: 7573 746f 6d5f 626f 756e 6473 203d 2062  ustom_bounds = b
-00003860: 6f75 6e64 730d 0a09 0909 0972 6574 7572  ounds......retur
-00003870: 6e20 4e6f 6e65 0d0a 0d0a 0909 0972 6574  n None.......ret
-00003880: 7572 6e20 626f 756e 6473 0d0a 0d0a 0909  urn bounds......
-00003890: 7265 7475 726e 2073 656c 662e 6375 7374  return self.cust
-000038a0: 6f6d 5f62 6f75 6e64 730d 0a0d 0a0d 0a09  om_bounds.......
-000038b0: 6465 6620 7570 6461 7465 5f73 697a 6528  def update_size(
-000038c0: 7365 6c66 2c20 2a61 7267 7329 3a0d 0a09  self, *args):...
-000038d0: 090d 0a09 0977 6964 7468 2c20 6865 6967  .....width, heig
-000038e0: 6874 203d 2073 656c 662e 7369 7a65 0d0a  ht = self.size..
-000038f0: 0909 6966 2072 6f75 6e64 2873 656c 662e  ..if round(self.
-00003900: 7261 7469 6f2c 2033 2920 213d 2072 6f75  ratio, 3) != rou
-00003910: 6e64 2877 6964 7468 202f 2066 6c6f 6174  nd(width / float
-00003920: 2868 6569 6768 7429 2c20 3329 3a0d 0a09  (height), 3):...
-00003930: 0909 2320 4164 6a75 7374 696e 6720 7369  ..# Adjusting si
-00003940: 7a65 2074 6f20 6669 7420 7261 7469 6f0d  ze to fit ratio.
-00003950: 0a09 0909 6c61 7374 5f73 697a 6520 3d20  ....last_size = 
-00003960: 7365 6c66 2e6c 6173 745f 7369 7a65 0d0a  self.last_size..
-00003970: 0909 0969 6620 6162 7328 7769 6474 6820  ...if abs(width 
-00003980: 2d20 6c61 7374 5f73 697a 655b 305d 2920  - last_size[0]) 
-00003990: 3e20 6162 7328 6865 6967 6874 202d 206c  > abs(height - l
-000039a0: 6173 745f 7369 7a65 5b31 5d29 3a0d 0a09  ast_size[1]):...
-000039b0: 0909 0973 656c 662e 7369 7a65 203d 205b  ...self.size = [
-000039c0: 7769 6474 682c 2028 666c 6f61 7428 7769  width, (float(wi
-000039d0: 6474 6829 202f 2073 656c 662e 7261 7469  dth) / self.rati
-000039e0: 6f29 5d0d 0a09 0909 656c 7365 3a0d 0a09  o)].....else:...
-000039f0: 0909 0973 656c 662e 7369 7a65 203d 205b  ...self.size = [
-00003a00: 2868 6569 6768 7420 2a20 7365 6c66 2e72  (height * self.r
-00003a10: 6174 696f 292c 2068 6569 6768 745d 0d0a  atio), height]..
-00003a20: 0909 090d 0a09 0909 6966 206c 6173 745f  ........if last_
-00003a30: 7369 7a65 2021 3d20 5b31 2c20 315d 3a0d  size != [1, 1]:.
-00003a40: 0a09 0909 0964 7720 3d20 7365 6c66 2e77  .....dw = self.w
-00003a50: 6964 7468 202d 206c 6173 745f 7369 7a65  idth - last_size
-00003a60: 5b30 5d0d 0a09 0909 0964 6820 3d20 7365  [0]......dh = se
-00003a70: 6c66 2e68 6569 6768 7420 2d20 6c61 7374  lf.height - last
-00003a80: 5f73 697a 655b 315d 0d0a 0909 0909 2320  _size[1]......# 
-00003a90: 4d6f 7669 6e67 2077 6964 6765 7420 746f  Moving widget to
-00003aa0: 206b 6565 7020 7069 766f 7427 7320 706f   keep pivot's po
-00003ab0: 7369 7469 6f6e 2074 6865 2073 616d 652c  sition the same,
-00003ac0: 2074 6f20 6f72 6967 696e 6174 6520 7468   to originate th
-00003ad0: 6520 7265 7369 7a69 6e67 2066 726f 6d20  e resizing from 
-00003ae0: 7069 766f 742e 0d0a 0909 0909 7365 6c66  pivot.......self
-00003af0: 2e70 6976 6f74 203d 2028 2028 7365 6c66  .pivot = ( (self
-00003b00: 2e70 6976 6f74 5f78 202d 2064 7720 2a20  .pivot_x - dw * 
-00003b10: 302e 3529 2c20 2873 656c 662e 7069 766f  0.5), (self.pivo
-00003b20: 745f 7920 2d20 6468 202a 2030 2e35 2920  t_y - dh * 0.5) 
-00003b30: 290d 0a0d 0a09 0969 6620 7365 6c66 2e61  )......if self.a
-00003b40: 6c6c 6f77 5f72 6f74 6162 6f78 3a0d 0a09  llow_rotabox:...
-00003b50: 0909 2320 5363 616c 696e 6720 7769 6467  ..# Scaling widg
-00003b60: 6574 2773 2062 6f75 6e64 730d 0a09 0909  et's bounds.....
-00003b70: 6966 206e 6f74 2073 656c 662e 616e 696d  if not self.anim
-00003b80: 3a0d 0a09 0909 0972 6573 697a 6528 7365  :......resize(se
-00003b90: 6c66 2e77 6964 7468 2c20 7365 6c66 2e68  lf.width, self.h
-00003ba0: 6569 6768 742c 2073 656c 662e 7269 6429  eight, self.rid)
-00003bb0: 0d0a 0909 0909 7570 6461 7465 5f62 6f75  ......update_bou
-00003bc0: 6e64 7328 7365 6c66 2e70 6f73 2c20 7261  nds(self.pos, ra
-00003bd0: 6469 616e 7328 7365 6c66 2e61 6e67 6c65  dians(self.angle
-00003be0: 292c 2073 656c 662e 6f72 6967 696e 2c20  ), self.origin, 
-00003bf0: 7365 6c66 2e72 6964 2c20 7365 6c66 2e63  self.rid, self.c
-00003c00: 7572 725f 6b65 7929 0d0a 0909 0909 7365  urr_key)......se
-00003c10: 6c66 2e61 6c6c 6f77 203d 2030 0d0a 0909  lf.allow = 0....
-00003c20: 0965 6c73 653a 0d0a 0909 0909 616e 6972  .else:......anir
-00003c30: 6573 697a 6528 7365 6c66 2e77 6964 7468  esize(self.width
-00003c40: 2c20 7365 6c66 2e68 6569 6768 742c 2073  , self.height, s
-00003c50: 656c 662e 7269 6429 0d0a 0d0a 0909 6966  elf.rid)......if
-00003c60: 2073 656c 662e 6368 696c 6472 656e 3a0d   self.children:.
-00003c70: 0a09 0909 7365 6c66 2e63 6869 6c64 7265  ....self.childre
-00003c80: 6e5b 305d 2e73 697a 6520 3d20 7365 6c66  n[0].size = self
-00003c90: 2e73 697a 650d 0a0d 0a09 0973 656c 662e  .size......self.
-00003ca0: 6c61 7374 5f73 697a 6520 3d20 7365 6c66  last_size = self
-00003cb0: 2e73 697a 655b 3a5d 0d0a 0909 7365 6c66  .size[:]....self
-00003cc0: 2e74 7269 6767 6572 5f75 7064 6174 6528  .trigger_update(
-00003cd0: 290d 0a0d 0a09 6465 6620 7570 6461 7465  ).....def update
-00003ce0: 2873 656c 662c 202a 6172 6773 293a 0d0a  (self, *args):..
-00003cf0: 0909 2727 2755 7064 6174 6573 2074 6865  ..'''Updates the
-00003d00: 2077 6964 6765 7427 7320 616e 676c 652c   widget's angle,
-00003d10: 2070 6f69 6e74 206f 6620 726f 7461 7469   point of rotati
-00003d20: 6f6e 2c20 626f 756e 6473 2061 6e64 2063  on, bounds and c
-00003d30: 6869 6c64 2773 0d0a 0909 706f 7369 7469  hild's....positi
-00003d40: 6f6e 2e0d 0a09 0941 6c73 6f20 7275 6e73  on.....Also runs
-00003d50: 2074 6865 205b 7570 6461 7465 5f73 697a   the [update_siz
-00003d60: 655d 206d 6574 686f 6420 6f6e 2073 697a  e] method on siz
-00003d70: 6520 6368 616e 6765 2061 6e64 2074 6865  e change and the
-00003d80: 205b 7072 6570 6172 655d 0d0a 0909 6d65   [prepare]....me
-00003d90: 7468 6f64 2069 6e69 7469 616c 6c79 2061  thod initially a
-00003da0: 6e64 206f 6e20 7265 7365 742e 0d0a 0909  nd on reset.....
-00003db0: 2727 270d 0a09 0969 6620 6e6f 7420 7365  '''....if not se
-00003dc0: 6c66 2e70 7265 7061 7265 643a 0d0a 0909  lf.prepared:....
-00003dd0: 0973 656c 662e 7072 6570 6172 6528 290d  .self.prepare().
-00003de0: 0a09 0909 7365 6c66 2e75 7064 6174 655f  ....self.update_
-00003df0: 7369 7a65 2829 0d0a 0909 0972 6574 7572  size().....retur
-00003e00: 6e20 4e6f 6e65 0d0a 0d0a 0909 7365 6c66  n None......self
-00003e10: 2e61 6e67 6c65 2025 3d20 3336 300d 0a09  .angle %= 360...
-00003e20: 0961 6e67 6c65 203d 2073 656c 662e 616e  .angle = self.an
-00003e30: 676c 650d 0a09 0970 6f73 203d 2073 656c  gle....pos = sel
-00003e40: 662e 706f 730d 0a0d 0a09 0923 2055 7064  f.pos......# Upd
-00003e50: 6174 696e 6720 7468 6520 726f 7461 7469  ating the rotati
-00003e60: 6f6e 2069 6e73 7472 7563 7469 6f6e 2c20  on instruction, 
-00003e70: 696e 2063 616e 7661 732e 6265 666f 7265  in canvas.before
-00003e80: 0d0a 0909 7365 6c66 2e72 6f74 6174 696f  ....self.rotatio
-00003e90: 6e2e 6f72 6967 696e 203d 2073 656c 662e  n.origin = self.
-00003ea0: 6f72 6967 696e 0d0a 0909 7365 6c66 2e72  origin....self.r
-00003eb0: 6f74 6174 696f 6e2e 616e 676c 6520 3d20  otation.angle = 
-00003ec0: 616e 676c 650d 0a0d 0a09 0923 2055 7064  angle......# Upd
-00003ed0: 6174 696e 6720 7468 6520 6368 696c 6427  ating the child'
-00003ee0: 7320 706f 7369 7469 6f6e 0d0a 0909 6966  s position....if
-00003ef0: 2073 656c 662e 6368 696c 6472 656e 3a0d   self.children:.
-00003f00: 0a09 0909 7365 6c66 2e63 6869 6c64 7265  ....self.childre
-00003f10: 6e5b 305d 2e70 6f73 203d 2070 6f73 0d0a  n[0].pos = pos..
-00003f20: 0d0a 0909 6d6f 7469 6f6e 203d 205b 706f  ....motion = [po
-00003f30: 735b 305d 202d 2073 656c 662e 6c61 7374  s[0] - self.last
-00003f40: 5f70 6f73 5b30 5d2c 2070 6f73 5b31 5d20  _pos[0], pos[1] 
-00003f50: 2d20 7365 6c66 2e6c 6173 745f 706f 735b  - self.last_pos[
-00003f60: 315d 5d0d 0a09 0969 6620 6162 7328 6d6f  1]]....if abs(mo
-00003f70: 7469 6f6e 5b30 5d29 203c 202e 3031 2061  tion[0]) < .01 a
-00003f80: 6e64 2061 6273 286d 6f74 696f 6e5b 315d  nd abs(motion[1]
-00003f90: 2920 3c20 302e 3031 3a0d 0a09 0909 6d6f  ) < 0.01:.....mo
-00003fa0: 7469 6f6e 203d 205b 5d0d 0a09 0973 656c  tion = []....sel
-00003fb0: 662e 6c61 7374 5f70 6f73 203d 2070 6f73  f.last_pos = pos
-00003fc0: 5b3a 5d0d 0a0d 0a09 0961 6e67 6c65 5f64  [:]......angle_d
-00003fd0: 6966 6620 3d20 616e 676c 6520 2d20 7365  iff = angle - se
-00003fe0: 6c66 2e6c 6173 745f 616e 676c 650d 0a09  lf.last_angle...
-00003ff0: 0969 6620 6162 7328 616e 676c 655f 6469  .if abs(angle_di
-00004000: 6666 2920 3c20 302e 3031 3a0d 0a09 0909  ff) < 0.01:.....
-00004010: 616e 676c 655f 6469 6666 203d 2030 0d0a  angle_diff = 0..
-00004020: 0d0a 0909 7365 6c66 2e6c 6173 745f 616e  ....self.last_an
-00004030: 676c 6520 3d20 616e 676c 650d 0a09 0969  gle = angle....i
-00004040: 6620 6e6f 7420 7365 6c66 2e61 6c6c 6f77  f not self.allow
-00004050: 3a0d 0a09 0909 7365 6c66 2e61 6c6c 6f77  :.....self.allow
-00004060: 203d 2031 0d0a 0909 0972 6574 7572 6e20   = 1.....return 
-00004070: 4e6f 6e65 0d0a 0d0a 0909 6966 2073 656c  None......if sel
-00004080: 662e 616c 6c6f 775f 726f 7461 626f 783a  f.allow_rotabox:
-00004090: 0d0a 0909 0923 2055 7064 6174 696e 6720  .....# Updating 
-000040a0: 7468 6520 6375 7374 6f6d 2062 6f75 6e64  the custom bound
-000040b0: 730d 0a09 0909 6966 2073 656c 662e 616e  s.....if self.an
-000040c0: 696d 3a0d 0a09 0909 0923 2041 6e20 6964  im:......# An id
-000040d0: 656e 7469 6361 6c6c 7920 6b65 7965 6420  entically keyed 
-000040e0: 6174 6c61 7320 6669 6c65 2069 7320 6173  atlas file is as
-000040f0: 7375 6d65 642e 0d0a 0909 0909 7365 6c66  sumed.......self
-00004100: 2e63 7572 725f 6b65 7920 3d20 7365 6c66  .curr_key = self
-00004110: 2e63 7572 7265 6e74 5f69 6d61 6765 0d0a  .current_image..
-00004120: 0909 0909 616e 6975 7064 6174 655f 626f  ....aniupdate_bo
-00004130: 756e 6473 2854 7275 652c 2070 6f73 2c20  unds(True, pos, 
-00004140: 7261 6469 616e 7328 616e 676c 6529 2c20  radians(angle), 
-00004150: 7365 6c66 2e6f 7269 6769 6e2c 2073 656c  self.origin, sel
-00004160: 662e 7269 642c 2073 656c 662e 6375 7272  f.rid, self.curr
-00004170: 5f6b 6579 290d 0a09 0909 0972 6574 7572  _key)......retur
-00004180: 6e20 4e6f 6e65 0d0a 0d0a 0909 0969 6620  n None.......if 
-00004190: 6d6f 7469 6f6e 206f 7220 616e 676c 655f  motion or angle_
-000041a0: 6469 6666 3a0d 0a09 0909 0975 7064 6174  diff:......updat
-000041b0: 655f 626f 756e 6473 286d 6f74 696f 6e2c  e_bounds(motion,
-000041c0: 2072 6164 6961 6e73 2861 6e67 6c65 5f64   radians(angle_d
-000041d0: 6966 6629 2c20 7365 6c66 2e6f 7269 6769  iff), self.origi
-000041e0: 6e2c 2073 656c 662e 7269 642c 2073 656c  n, self.rid, sel
-000041f0: 662e 6375 7272 5f6b 6579 290d 0a09 0d0a  f.curr_key).....
-00004200: 0d0a 0964 6566 2063 6f6c 6c69 6465 5f70  ...def collide_p
-00004210: 6f69 6e74 2873 656c 662c 2078 3d30 2c20  oint(self, x=0, 
-00004220: 793d 3029 3a0d 0a09 0969 6620 7365 6c66  y=0):....if self
-00004230: 2e61 6c6c 6f77 5f72 6f74 6162 6f78 3a0d  .allow_rotabox:.
-00004240: 0a09 0909 7265 7475 726e 2070 6f69 6e74  ....return point
-00004250: 5f69 6e5f 626f 756e 6473 2878 2c20 792c  _in_bounds(x, y,
-00004260: 2073 656c 662e 7269 642c 2066 7261 6d65   self.rid, frame
-00004270: 3d73 656c 662e 6375 7272 5f6b 6579 290d  =self.curr_key).
-00004280: 0a09 0965 6c73 653a 0d0a 0909 0972 6574  ...else:.....ret
-00004290: 7572 6e20 7375 7065 7228 292e 636f 6c6c  urn super().coll
-000042a0: 6964 655f 706f 696e 7428 782c 2079 290d  ide_point(x, y).
-000042b0: 0a0d 0a09 6465 6620 636f 6c6c 6964 655f  ....def collide_
-000042c0: 7769 6467 6574 2873 656c 662c 2077 6964  widget(self, wid
-000042d0: 293a 0d0a 0909 7472 793a 0d0a 0909 0974  ):....try:.....t
-000042e0: 7279 3a0d 0a09 0909 0972 6574 7572 6e20  ry:......return 
-000042f0: 636f 6c6c 6964 655f 626f 756e 6473 2873  collide_bounds(s
-00004300: 656c 662e 7269 642c 2077 6964 2e72 6964  elf.rid, wid.rid
-00004310: 2c20 6672 616d 653d 7365 6c66 2e63 7572  , frame=self.cur
-00004320: 725f 6b65 792c 2074 6672 616d 653d 7769  r_key, tframe=wi
-00004330: 642e 6375 7272 5f6b 6579 290d 0a09 0909  d.curr_key).....
-00004340: 6578 6365 7074 2041 7474 7269 6275 7465  except Attribute
-00004350: 4572 726f 723a 0d0a 0909 0909 6966 2073  Error:......if s
-00004360: 656c 662e 7365 676d 656e 745f 6d6f 6465  elf.segment_mode
-00004370: 3a0d 0a09 0909 0909 7265 7475 726e 2063  :.......return c
-00004380: 6f6c 6c69 6465 5f62 6f75 6e64 7328 7365  ollide_bounds(se
-00004390: 6c66 2e72 6964 2c20 5b77 6964 2e78 2c20  lf.rid, [wid.x, 
-000043a0: 7769 642e 792c 2077 6964 2e72 6967 6874  wid.y, wid.right
-000043b0: 2c20 7769 642e 746f 705d 2c20 6672 616d  , wid.top], fram
-000043c0: 653d 7365 6c66 2e63 7572 725f 6b65 7929  e=self.curr_key)
-000043d0: 0d0a 0909 0909 7265 7475 726e 2073 7570  ......return sup
-000043e0: 6572 2829 2e63 6f6c 6c69 6465 5f77 6964  er().collide_wid
-000043f0: 6765 7428 7769 6429 0d0a 0909 6578 6365  get(wid)....exce
-00004400: 7074 204b 6579 4572 726f 723a 0d0a 0909  pt KeyError:....
-00004410: 0972 6574 7572 6e20 4661 6c73 650d 0a0d  .return False...
-00004420: 0a09 6465 6620 6f6e 5f74 6f75 6368 5f64  ..def on_touch_d
-00004430: 6f77 6e28 7365 6c66 2c20 746f 7563 6829  own(self, touch)
-00004440: 3a0d 0a09 0978 2c20 7920 3d20 746f 7563  :....x, y = touc
-00004450: 682e 782c 2074 6f75 6368 2e79 0d0a 0d0a  h.x, touch.y....
-00004460: 0909 2320 6966 2074 6865 2074 6f75 6368  ..# if the touch
-00004470: 2069 736e 7420 6f6e 2074 6865 2077 6964   isnt on the wid
-00004480: 6765 7420 7765 2064 6f20 6e6f 7468 696e  get we do nothin
-00004490: 670d 0a09 0969 6620 6e6f 7420 7365 6c66  g....if not self
-000044a0: 2e63 6f6c 6c69 6465 5f61 6674 6572 5f63  .collide_after_c
-000044b0: 6869 6c64 7265 6e3a 0d0a 0909 0969 6620  hildren:.....if 
-000044c0: 6e6f 7420 7365 6c66 2e63 6f6c 6c69 6465  not self.collide
-000044d0: 5f70 6f69 6e74 2878 2c20 7929 3a0d 0a09  _point(x, y):...
-000044e0: 0909 0972 6574 7572 6e20 4661 6c73 650d  ...return False.
-000044f0: 0a0d 0a09 0923 206c 6574 2074 6865 2063  .....# let the c
-00004500: 6869 6c64 2077 6964 6765 7473 2068 616e  hild widgets han
-00004510: 646c 6520 7468 6520 6576 656e 7420 6966  dle the event if
-00004520: 2074 6865 7920 7761 6e74 0d0a 0909 6966   they want....if
-00004530: 2073 7570 6572 2829 2e6f 6e5f 746f 7563   super().on_touc
-00004540: 685f 646f 776e 2874 6f75 6368 293a 0d0a  h_down(touch):..
-00004550: 0909 0923 2065 6e73 7572 6520 6368 696c  ...# ensure chil
-00004560: 6472 656e 2064 6f6e 2774 2068 6176 6520  dren don't have 
-00004570: 746f 2064 6f20 6974 2074 6865 6d73 656c  to do it themsel
-00004580: 7665 730d 0a09 0909 6966 2027 6d75 6c74  ves.....if 'mult
-00004590: 6974 6f75 6368 5f73 696d 2720 696e 2074  itouch_sim' in t
-000045a0: 6f75 6368 2e70 726f 6669 6c65 3a0d 0a09  ouch.profile:...
-000045b0: 0909 0974 6f75 6368 2e6d 756c 7469 746f  ...touch.multito
-000045c0: 7563 685f 7369 6d20 3d20 5472 7565 0d0a  uch_sim = True..
-000045d0: 0909 090d 0a09 0909 7365 6c66 2e62 7269  ........self.bri
-000045e0: 6e67 5f74 6f5f 6672 6f6e 7428 746f 7563  ng_to_front(touc
-000045f0: 6829 0d0a 0909 0972 6574 7572 6e20 5472  h).....return Tr
-00004600: 7565 0d0a 0d0a 0909 2320 6966 2077 6520  ue......# if we 
-00004610: 646f 6e27 7420 6861 7665 2061 6e79 2061  don't have any a
-00004620: 6374 6976 650d 0a09 0923 2069 6e74 6572  ctive....# inter
-00004630: 6163 7469 6f6e 2063 6f6e 7472 6f6c 2c20  action control, 
-00004640: 7468 656e 2064 6f6e 2774 2061 6363 6570  then don't accep
-00004650: 7420 7468 6520 746f 7563 682e 0d0a 0909  t the touch.....
-00004660: 6966 206e 6f74 2028 7365 6c66 2e61 6c6c  if not (self.all
-00004670: 6f77 5f64 7261 675f 780d 0a09 0909 096f  ow_drag_x......o
-00004680: 7220 7365 6c66 2e61 6c6c 6f77 5f64 7261  r self.allow_dra
-00004690: 675f 790d 0a09 0909 096f 7220 7365 6c66  g_y......or self
-000046a0: 2e6d 756c 7469 5f74 6f75 6368 5f72 6f74  .multi_touch_rot
-000046b0: 6174 696f 6e0d 0a09 0909 096f 7220 7365  ation......or se
-000046c0: 6c66 2e6d 756c 7469 5f74 6f75 6368 5f73  lf.multi_touch_s
-000046d0: 6361 6c69 6e67 0d0a 0909 0909 6f72 2073  caling......or s
-000046e0: 656c 662e 7369 6e67 6c65 5f74 6f75 6368  elf.single_touch
-000046f0: 5f72 6f74 6174 696f 6e0d 0a09 0909 096f  _rotation......o
-00004700: 7220 7365 6c66 2e73 696e 676c 655f 746f  r self.single_to
-00004710: 7563 685f 7363 616c 696e 6729 3a0d 0a09  uch_scaling):...
-00004720: 0909 7265 7475 726e 2046 616c 7365 0d0a  ..return False..
-00004730: 0d0a 0909 6966 2073 656c 662e 636f 6c6c  ....if self.coll
-00004740: 6964 655f 6166 7465 725f 6368 696c 6472  ide_after_childr
-00004750: 656e 3a0d 0a09 0909 6966 206e 6f74 2073  en:.....if not s
-00004760: 656c 662e 636f 6c6c 6964 655f 706f 696e  elf.collide_poin
-00004770: 7428 782c 2079 293a 0d0a 0909 0909 7265  t(x, y):......re
-00004780: 7475 726e 2046 616c 7365 0d0a 0d0a 0909  turn False......
-00004790: 6966 2027 6d75 6c74 6974 6f75 6368 5f73  if 'multitouch_s
-000047a0: 696d 2720 696e 2074 6f75 6368 2e70 726f  im' in touch.pro
-000047b0: 6669 6c65 3a0d 0a09 0909 746f 7563 682e  file:.....touch.
-000047c0: 6d75 6c74 6974 6f75 6368 5f73 696d 203d  multitouch_sim =
-000047d0: 2054 7275 650d 0a0d 0a09 0923 2067 7261   True......# gra
-000047e0: 6220 7468 6520 746f 7563 6820 736f 2077  b the touch so w
-000047f0: 6520 6765 7420 616c 6c20 6974 206c 6174  e get all it lat
-00004800: 6572 206d 6f76 6520 6576 656e 7473 2066  er move events f
-00004810: 6f72 2073 7572 650d 0a09 0973 656c 662e  or sure....self.
-00004820: 6272 696e 675f 746f 5f66 726f 6e74 2874  bring_to_front(t
-00004830: 6f75 6368 290d 0a09 0974 6f75 6368 2e67  ouch)....touch.g
-00004840: 7261 6228 7365 6c66 290d 0a09 0973 656c  rab(self)....sel
-00004850: 662e 746f 7563 6865 732e 6170 7065 6e64  f.touches.append
-00004860: 2874 6f75 6368 290d 0a09 0973 656c 662e  (touch)....self.
-00004870: 6c61 7374 5f74 6f75 6368 5f70 6f73 5b74  last_touch_pos[t
-00004880: 6f75 6368 5d20 3d20 782c 2079 0d0a 0909  ouch] = x, y....
-00004890: 7265 7475 726e 2054 7275 650d 0a0d 0a09  return True.....
-000048a0: 6465 6620 6272 696e 675f 746f 5f66 726f  def bring_to_fro
-000048b0: 6e74 2873 656c 662c 2074 6f75 6368 293a  nt(self, touch):
-000048c0: 0d0a 0909 6966 2073 656c 662e 746f 7563  ....if self.touc
-000048d0: 6865 645f 746f 5f66 726f 6e74 2061 6e64  hed_to_front and
-000048e0: 2073 656c 662e 7061 7265 6e74 3a0d 0a09   self.parent:...
-000048f0: 0909 7061 7265 6e74 203d 2073 656c 662e  ..parent = self.
-00004900: 7061 7265 6e74 0d0a 0909 0969 6620 7061  parent.....if pa
-00004910: 7265 6e74 2e63 6869 6c64 7265 6e5b 305d  rent.children[0]
-00004920: 2069 7320 7365 6c66 3a0d 0a09 0909 0972   is self:......r
-00004930: 6574 7572 6e20 4e6f 6e65 0d0a 0909 090d  eturn None......
-00004940: 0a09 0909 7061 7265 6e74 2e72 656d 6f76  ....parent.remov
-00004950: 655f 7769 6467 6574 2873 656c 6629 0d0a  e_widget(self)..
-00004960: 0909 0970 6172 656e 742e 6164 645f 7769  ...parent.add_wi
-00004970: 6467 6574 2873 656c 6629 0d0a 0909 0973  dget(self).....s
-00004980: 656c 662e 6469 7370 6174 6368 2827 6f6e  elf.dispatch('on
-00004990: 5f74 6f75 6368 6564 5f74 6f5f 6672 6f6e  _touched_to_fron
-000049a0: 7427 2c20 746f 7563 6829 0d0a 0d0a 0964  t', touch).....d
-000049b0: 6566 206f 6e5f 746f 7563 685f 6d6f 7665  ef on_touch_move
-000049c0: 2873 656c 662c 2074 6f75 6368 293a 0d0a  (self, touch):..
-000049d0: 0909 782c 2079 203d 2074 6f75 6368 2e78  ..x, y = touch.x
-000049e0: 2c20 746f 7563 682e 790d 0a0d 0a09 0923  , touch.y......#
-000049f0: 206c 6574 2074 6865 2063 6869 6c64 2077   let the child w
-00004a00: 6964 6765 7473 2068 616e 646c 6520 7468  idgets handle th
-00004a10: 6520 6576 656e 7420 6966 2074 6865 7920  e event if they 
-00004a20: 7761 6e74 0d0a 0909 6966 2073 656c 662e  want....if self.
-00004a30: 636f 6c6c 6964 655f 706f 696e 7428 782c  collide_point(x,
-00004a40: 2079 2920 616e 6420 6e6f 7420 746f 7563   y) and not touc
-00004a50: 682e 6772 6162 5f63 7572 7265 6e74 203d  h.grab_current =
-00004a60: 3d20 7365 6c66 3a0d 0a09 0909 6966 2073  = self:.....if s
-00004a70: 7570 6572 2829 2e6f 6e5f 746f 7563 685f  uper().on_touch_
-00004a80: 6d6f 7665 2874 6f75 6368 293a 0d0a 0909  move(touch):....
-00004a90: 0909 7265 7475 726e 2054 7275 650d 0a0d  ..return True...
-00004aa0: 0a09 0969 6620 746f 7563 6820 696e 2073  ...if touch in s
-00004ab0: 656c 662e 746f 7563 6865 7320 616e 6420  elf.touches and 
-00004ac0: 746f 7563 682e 6772 6162 5f63 7572 7265  touch.grab_curre
-00004ad0: 6e74 203d 3d20 7365 6c66 3a0d 0a09 0909  nt == self:.....
-00004ae0: 6966 2073 656c 662e 7472 616e 7366 6f72  if self.transfor
-00004af0: 6d5f 7769 7468 5f74 6f75 6368 2874 6f75  m_with_touch(tou
-00004b00: 6368 293a 0d0a 0909 0909 7365 6c66 2e64  ch):......self.d
-00004b10: 6973 7061 7463 6828 276f 6e5f 7472 616e  ispatch('on_tran
-00004b20: 7366 6f72 6d5f 7769 7468 5f74 6f75 6368  sform_with_touch
-00004b30: 272c 2074 6f75 6368 290d 0a09 0909 7365  ', touch).....se
-00004b40: 6c66 2e6c 6173 745f 746f 7563 685f 706f  lf.last_touch_po
-00004b50: 735b 746f 7563 685d 203d 2078 2c20 790d  s[touch] = x, y.
-00004b60: 0a0d 0a09 0969 6620 7365 6c66 2e63 6f6c  .....if self.col
-00004b70: 6c69 6465 5f70 6f69 6e74 2878 2c20 7929  lide_point(x, y)
-00004b80: 3a0d 0a09 0909 7265 7475 726e 2054 7275  :.....return Tru
-00004b90: 650d 0a0d 0a09 6465 6620 7472 616e 7366  e.....def transf
-00004ba0: 6f72 6d5f 7769 7468 5f74 6f75 6368 2873  orm_with_touch(s
-00004bb0: 656c 662c 2074 6f75 6368 293a 0d0a 0909  elf, touch):....
-00004bc0: 6368 616e 6765 6420 3d20 4661 6c73 650d  changed = False.
-00004bd0: 0a09 0974 6f75 6368 6573 203d 206c 656e  ...touches = len
-00004be0: 2873 656c 662e 746f 7563 6865 7329 0d0a  (self.touches)..
-00004bf0: 0d0a 0909 6966 2028 746f 7563 6865 7320  ....if (touches 
-00004c00: 3d3d 2073 656c 662e 7369 6e67 6c65 5f64  == self.single_d
-00004c10: 7261 675f 746f 7563 6820 616e 6420 2873  rag_touch and (s
-00004c20: 656c 662e 616c 6c6f 775f 6472 6167 5f78  elf.allow_drag_x
-00004c30: 206f 7220 7365 6c66 2e61 6c6c 6f77 5f64   or self.allow_d
-00004c40: 7261 675f 7929 293a 0d0a 0909 0964 7820  rag_y)):.....dx 
-00004c50: 3d20 2874 6f75 6368 2e78 202d 2073 656c  = (touch.x - sel
-00004c60: 662e 6c61 7374 5f74 6f75 6368 5f70 6f73  f.last_touch_pos
-00004c70: 5b74 6f75 6368 5d5b 305d 2920 2a20 7365  [touch][0]) * se
-00004c80: 6c66 2e61 6c6c 6f77 5f64 7261 675f 780d  lf.allow_drag_x.
-00004c90: 0a09 0909 6479 203d 2028 746f 7563 682e  ....dy = (touch.
-00004ca0: 7920 2d20 7365 6c66 2e6c 6173 745f 746f  y - self.last_to
-00004cb0: 7563 685f 706f 735b 746f 7563 685d 5b31  uch_pos[touch][1
-00004cc0: 5d29 202a 2073 656c 662e 616c 6c6f 775f  ]) * self.allow_
-00004cd0: 6472 6167 5f79 0d0a 0909 090d 0a09 0909  drag_y..........
-00004ce0: 7365 6c66 2e78 202b 3d20 666c 6f61 7428  self.x += float(
-00004cf0: 6478 2920 2f20 7365 6c66 2e73 696e 676c  dx) / self.singl
-00004d00: 655f 6472 6167 5f74 6f75 6368 0d0a 0909  e_drag_touch....
-00004d10: 0973 656c 662e 7920 2b3d 2066 6c6f 6174  .self.y += float
-00004d20: 2864 7929 202f 2073 656c 662e 7369 6e67  (dy) / self.sing
-00004d30: 6c65 5f64 7261 675f 746f 7563 680d 0a09  le_drag_touch...
-00004d40: 0909 6368 616e 6765 6420 3d20 5472 7565  ..changed = True
-00004d50: 0d0a 0d0a 0909 6966 2028 746f 7563 6865  ......if (touche
-00004d60: 7320 3d3d 2073 656c 662e 7369 6e67 6c65  s == self.single
-00004d70: 5f74 7261 6e73 5f74 6f75 6368 2061 6e64  _trans_touch and
-00004d80: 2028 7365 6c66 2e73 696e 676c 655f 746f   (self.single_to
-00004d90: 7563 685f 726f 7461 7469 6f6e 206f 7220  uch_rotation or 
-00004da0: 7365 6c66 2e73 696e 676c 655f 746f 7563  self.single_touc
-00004db0: 685f 7363 616c 696e 6729 293a 0d0a 0909  h_scaling)):....
-00004dc0: 0961 6e63 686f 7220 3d20 7365 6c66 2e70  .anchor = self.p
-00004dd0: 6976 6f74 0d0a 0909 096f 6c64 5f6c 696e  ivot.....old_lin
-00004de0: 6520 3d20 5665 6374 6f72 282a 746f 7563  e = Vector(*touc
-00004df0: 682e 7070 6f73 2920 2d20 616e 6368 6f72  h.ppos) - anchor
-00004e00: 0d0a 0909 096e 6577 5f6c 696e 6520 3d20  .....new_line = 
-00004e10: 5665 6374 6f72 282a 746f 7563 682e 706f  Vector(*touch.po
-00004e20: 7329 202d 2061 6e63 686f 720d 0a09 0909  s) - anchor.....
-00004e30: 6966 206e 6f74 206f 6c64 5f6c 696e 652e  if not old_line.
-00004e40: 6c65 6e67 7468 2829 3a0d 0a09 0909 0972  length():......r
-00004e50: 6574 7572 6e20 6368 616e 6765 640d 0a09  eturn changed...
-00004e60: 0909 0d0a 0909 0969 6620 7365 6c66 2e73  .......if self.s
-00004e70: 696e 676c 655f 746f 7563 685f 726f 7461  ingle_touch_rota
-00004e80: 7469 6f6e 3a0d 0a09 0909 0961 6e67 6c65  tion:......angle
-00004e90: 203d 206e 6577 5f6c 696e 652e 616e 676c   = new_line.angl
-00004ea0: 6528 6f6c 645f 6c69 6e65 290d 0a09 0909  e(old_line).....
-00004eb0: 0973 656c 662e 616e 676c 6520 2b3d 2061  .self.angle += a
-00004ec0: 6e67 6c65 0d0a 0d0a 0909 0969 6620 7365  ngle.......if se
-00004ed0: 6c66 2e73 696e 676c 655f 746f 7563 685f  lf.single_touch_
-00004ee0: 7363 616c 696e 673a 0d0a 0909 0909 5f73  scaling:......_s
-00004ef0: 6361 6c65 203d 206e 6577 5f6c 696e 652e  cale = new_line.
-00004f00: 6c65 6e67 7468 2829 202f 206f 6c64 5f6c  length() / old_l
-00004f10: 696e 652e 6c65 6e67 7468 2829 0d0a 0909  ine.length()....
-00004f20: 0909 7365 6c66 2e73 6361 6c65 202a 3d20  ..self.scale *= 
-00004f30: 5f73 6361 6c65 0d0a 0909 090d 0a09 0909  _scale..........
-00004f40: 6368 616e 6765 6420 3d20 5472 7565 0d0a  changed = True..
-00004f50: 0d0a 0909 6966 2074 6f75 6368 6573 203d  ....if touches =
-00004f60: 3d20 313a 0d0a 0909 0972 6574 7572 6e20  = 1:.....return 
-00004f70: 6368 616e 6765 640d 0a0d 0a09 0923 2077  changed......# w
-00004f80: 6520 6861 7665 206d 6f72 6520 7468 616e  e have more than
-00004f90: 206f 6e65 2074 6f75 6368 2e2e 2e20 6c69   one touch... li
-00004fa0: 7374 206f 6620 6c61 7374 206b 6e6f 776e  st of last known
-00004fb0: 2070 6f73 0d0a 0909 706f 696e 7473 203d   pos....points =
-00004fc0: 205b 5665 6374 6f72 2873 656c 662e 6c61   [Vector(self.la
-00004fd0: 7374 5f74 6f75 6368 5f70 6f73 5b74 5d29  st_touch_pos[t])
-00004fe0: 2066 6f72 2074 2069 6e20 7365 6c66 2e74   for t in self.t
-00004ff0: 6f75 6368 6573 2069 6620 7420 6973 206e  ouches if t is n
-00005000: 6f74 2074 6f75 6368 5d0d 0a09 0970 6f69  ot touch]....poi
-00005010: 6e74 732e 6170 7065 6e64 2856 6563 746f  nts.append(Vecto
-00005020: 7228 746f 7563 682e 706f 7329 290d 0a0d  r(touch.pos))...
-00005030: 0a09 0923 2077 6520 6f6e 6c79 2077 616e  ...# we only wan
-00005040: 7420 746f 2074 7261 6e73 666f 726d 2069  t to transform i
-00005050: 6620 7468 6520 746f 7563 6820 6973 2070  f the touch is p
-00005060: 6172 7420 6f66 2074 6865 2074 776f 2074  art of the two t
-00005070: 6f75 6368 6573 0d0a 0909 2320 6661 7274  ouches....# fart
-00005080: 6865 7374 2061 7061 7274 2120 536f 2066  hest apart! So f
-00005090: 6972 7374 2077 6520 6669 6e64 2061 6e63  irst we find anc
-000050a0: 686f 722c 2074 6865 2070 6f69 6e74 2074  hor, the point t
-000050b0: 6f20 7472 616e 7366 6f72 6d0d 0a09 0923  o transform....#
-000050c0: 2061 726f 756e 6420 6173 2061 6e6f 7468   around as anoth
-000050d0: 6572 2074 6f75 6368 2066 6172 7468 6573  er touch farthes
-000050e0: 7420 6177 6179 2066 726f 6d20 6375 7272  t away from curr
-000050f0: 656e 7420 746f 7563 6827 7320 706f 730d  ent touch's pos.
-00005100: 0a09 0961 6e63 686f 7220 3d20 6d61 7828  ...anchor = max(
-00005110: 706f 696e 7473 5b3a 2d31 5d2c 206b 6579  points[:-1], key
-00005120: 3d6c 616d 6264 6120 703a 2070 2e64 6973  =lambda p: p.dis
-00005130: 7461 6e63 6528 746f 7563 682e 706f 7329  tance(touch.pos)
-00005140: 290d 0a0d 0a09 0973 656c 662e 6f72 6967  )......self.orig
-00005150: 696e 203d 2061 6e63 686f 720d 0a0d 0a09  in = anchor.....
-00005160: 0923 206e 6f77 2077 6520 6669 6e64 2074  .# now we find t
-00005170: 6865 2074 6f75 6368 2066 6172 7468 6573  he touch farthes
-00005180: 7420 6177 6179 2066 726f 6d20 616e 6368  t away from anch
-00005190: 6f72 2c20 6966 2069 7473 206e 6f74 2074  or, if its not t
-000051a0: 6865 0d0a 0909 2320 7361 6d65 2061 7320  he....# same as 
-000051b0: 746f 7563 682e 2054 6f75 6368 2069 7320  touch. Touch is 
-000051c0: 6e6f 7420 6f6e 6520 6f66 2074 6865 2074  not one of the t
-000051d0: 776f 2074 6f75 6368 6573 2075 7365 6420  wo touches used 
-000051e0: 746f 2074 7261 6e73 666f 726d 0d0a 0909  to transform....
-000051f0: 6661 7274 6865 7374 203d 206d 6178 2870  farthest = max(p
-00005200: 6f69 6e74 732c 206b 6579 3d61 6e63 686f  oints, key=ancho
-00005210: 722e 6469 7374 616e 6365 290d 0a09 0969  r.distance)....i
-00005220: 6620 6661 7274 6865 7374 2069 7320 6e6f  f farthest is no
-00005230: 7420 706f 696e 7473 5b2d 315d 3a0d 0a09  t points[-1]:...
-00005240: 0909 7265 7475 726e 2063 6861 6e67 6564  ..return changed
-00005250: 0d0a 0d0a 0909 2320 6f6b 2c20 736f 2077  ......# ok, so w
-00005260: 6520 6861 7665 2074 6f75 6368 2c20 616e  e have touch, an
-00005270: 6420 616e 6368 6f72 2c20 736f 2077 6520  d anchor, so we 
-00005280: 6361 6e20 6163 7475 616c 6c79 2063 6f6d  can actually com
-00005290: 7075 7465 2074 6865 2074 7261 6e73 666f  pute the transfo
-000052a0: 726d 6174 696f 6e0d 0a09 096f 6c64 5f6c  rmation....old_l
-000052b0: 696e 6520 3d20 5665 6374 6f72 282a 746f  ine = Vector(*to
-000052c0: 7563 682e 7070 6f73 2920 2d20 616e 6368  uch.ppos) - anch
-000052d0: 6f72 0d0a 0909 6e65 775f 6c69 6e65 203d  or....new_line =
-000052e0: 2056 6563 746f 7228 2a74 6f75 6368 2e70   Vector(*touch.p
-000052f0: 6f73 2920 2d20 616e 6368 6f72 0d0a 0909  os) - anchor....
-00005300: 6966 206e 6f74 206f 6c64 5f6c 696e 652e  if not old_line.
-00005310: 6c65 6e67 7468 2829 3a0d 0a09 0909 7265  length():.....re
-00005320: 7475 726e 2063 6861 6e67 6564 0d0a 0d0a  turn changed....
-00005330: 0909 616e 676c 6520 3d20 6e65 775f 6c69  ..angle = new_li
-00005340: 6e65 2e61 6e67 6c65 286f 6c64 5f6c 696e  ne.angle(old_lin
-00005350: 6529 202a 2073 656c 662e 6d75 6c74 695f  e) * self.multi_
-00005360: 746f 7563 685f 726f 7461 7469 6f6e 0d0a  touch_rotation..
-00005370: 0909 7365 6c66 2e61 6e67 6c65 202b 3d20  ..self.angle += 
-00005380: 616e 676c 650d 0a0d 0a09 0969 6620 7365  angle......if se
-00005390: 6c66 2e6d 756c 7469 5f74 6f75 6368 5f73  lf.multi_touch_s
-000053a0: 6361 6c69 6e67 3a0d 0a09 0909 5f73 6361  caling:....._sca
-000053b0: 6c65 203d 206e 6577 5f6c 696e 652e 6c65  le = new_line.le
-000053c0: 6e67 7468 2829 202f 206f 6c64 5f6c 696e  ngth() / old_lin
-000053d0: 652e 6c65 6e67 7468 2829 0d0a 0909 0973  e.length().....s
-000053e0: 656c 662e 7363 616c 6520 2a3d 205f 7363  elf.scale *= _sc
-000053f0: 616c 650d 0a09 0909 6368 616e 6765 6420  ale.....changed 
-00005400: 3d20 5472 7565 0d0a 0909 0d0a 0909 7265  = True........re
-00005410: 7475 726e 2063 6861 6e67 6564 0d0a 0d0a  turn changed....
-00005420: 0964 6566 206f 6e5f 746f 7563 685f 7570  .def on_touch_up
-00005430: 2873 656c 662c 2074 6f75 6368 293a 0d0a  (self, touch):..
-00005440: 0909 2320 6966 2074 6865 2074 6f75 6368  ..# if the touch
-00005450: 2069 736e 7420 6f6e 2074 6865 2077 6964   isnt on the wid
-00005460: 6765 7420 7765 2064 6f20 6e6f 7468 696e  get we do nothin
-00005470: 672c 206a 7573 7420 7472 7920 6368 696c  g, just try chil
-00005480: 6472 656e 0d0a 0909 6966 206e 6f74 2074  dren....if not t
-00005490: 6f75 6368 2e67 7261 625f 6375 7272 656e  ouch.grab_curren
-000054a0: 7420 3d3d 2073 656c 663a 0d0a 0909 0969  t == self:.....i
-000054b0: 6620 7375 7065 7228 292e 6f6e 5f74 6f75  f super().on_tou
-000054c0: 6368 5f75 7028 746f 7563 6829 3a0d 0a09  ch_up(touch):...
-000054d0: 0909 0972 6574 7572 6e20 5472 7565 0d0a  ...return True..
-000054e0: 0d0a 0909 2320 7265 6d6f 7665 2069 7420  ....# remove it 
-000054f0: 6672 6f6d 206f 7572 2073 6176 6564 2074  from our saved t
-00005500: 6f75 6368 6573 0d0a 0909 6966 2074 6f75  ouches....if tou
-00005510: 6368 2069 6e20 7365 6c66 2e74 6f75 6368  ch in self.touch
-00005520: 6573 2061 6e64 2074 6f75 6368 2e67 7261  es and touch.gra
-00005530: 625f 7374 6174 653a 0d0a 0909 0974 6f75  b_state:.....tou
-00005540: 6368 2e75 6e67 7261 6228 7365 6c66 290d  ch.ungrab(self).
-00005550: 0a09 0909 6465 6c20 7365 6c66 2e6c 6173  ....del self.las
-00005560: 745f 746f 7563 685f 706f 735b 746f 7563  t_touch_pos[touc
-00005570: 685d 0d0a 0909 0973 656c 662e 746f 7563  h].....self.touc
-00005580: 6865 732e 7265 6d6f 7665 2874 6f75 6368  hes.remove(touch
-00005590: 290d 0a0d 0a09 0923 2073 746f 7020 7072  )......# stop pr
-000055a0: 6f70 6167 6174 696e 6720 6966 2069 7473  opagating if its
-000055b0: 2077 6974 6869 6e20 6f75 7220 626f 756e   within our boun
-000055c0: 6473 0d0a 0909 6966 2073 656c 662e 636f  ds....if self.co
-000055d0: 6c6c 6964 655f 706f 696e 7428 2a74 6f75  llide_point(*tou
-000055e0: 6368 2e70 6f73 293a 0d0a 0909 0972 6574  ch.pos):.....ret
-000055f0: 7572 6e20 5472 7565 0d0a 0d0a 0964 6566  urn True.....def
-00005600: 2073 6574 5f64 7261 7728 7365 6c66 2c20   set_draw(self, 
-00005610: 2a61 7267 7329 3a0d 0a09 0927 2727 5365  *args):....'''Se
-00005620: 7474 696e 6720 7570 2063 616e 7661 7320  tting up canvas 
-00005630: 666f 7220 7465 7374 2d64 7261 7769 6e67  for test-drawing
-00005640: 2074 6865 2062 6f75 6e64 732e 2727 270d   the bounds.'''.
-00005650: 0a09 0973 656c 662e 7265 7365 745f 6472  ...self.reset_dr
-00005660: 6177 5f62 6f75 6e64 7328 290d 0a09 090d  aw_bounds().....
-00005670: 0a09 0969 6620 7365 6c66 2e61 6e69 6d3a  ...if self.anim:
-00005680: 0d0a 0909 0970 6f6c 7320 3d20 6d61 7828  .....pols = max(
-00005690: 5b6c 656e 2866 7261 6d65 2920 666f 7220  [len(frame) for 
-000056a0: 6672 616d 6520 696e 2073 656c 662e 6375  frame in self.cu
-000056b0: 7374 6f6d 5f62 6f75 6e64 732e 7661 6c75  stom_bounds.valu
-000056c0: 6573 2829 5d29 0d0a 0909 090d 0a09 0909  es()])..........
-000056d0: 6c65 6e67 7468 203d 206d 6178 285b 6c65  length = max([le
-000056e0: 6e28 706f 6c29 2066 6f72 2070 6f6c 2069  n(pol) for pol i
-000056f0: 6e20 7365 6c66 2e63 7573 746f 6d5f 626f  n self.custom_bo
-00005700: 756e 6473 2e76 616c 7565 7328 295d 290d  unds.values()]).
-00005710: 0a09 0965 6c73 653a 0d0a 0909 0970 6f6c  ...else:.....pol
-00005720: 7320 3d20 6c65 6e28 7365 6c66 2e63 7573  s = len(self.cus
-00005730: 746f 6d5f 626f 756e 6473 290d 0a09 0909  tom_bounds).....
-00005740: 6c65 6e67 7468 203d 2070 6565 7273 5b73  length = peers[s
-00005750: 656c 662e 7269 645d 5b73 656c 662e 6375  elf.rid][self.cu
-00005760: 7272 5f6b 6579 5d5b 276c 656e 6774 6827  rr_key]['length'
-00005770: 5d0d 0a0d 0a09 0966 6f72 2069 2069 6e20  ]......for i in 
-00005780: 7261 6e67 6528 706f 6c73 293a 0d0a 0909  range(pols):....
-00005790: 0969 6620 6920 6e6f 7420 696e 2073 656c  .if i not in sel
-000057a0: 662e 6f70 656e 5f62 6f75 6e64 7320 6f72  f.open_bounds or
-000057b0: 206e 6f74 2073 656c 662e 7365 676d 656e   not self.segmen
-000057c0: 745f 6d6f 6465 3a0d 0a09 0909 0973 656c  t_mode:......sel
-000057d0: 662e 6472 6177 5f6c 696e 6573 2e61 7070  f.draw_lines.app
-000057e0: 656e 6428 4c69 6e65 2863 6c6f 7365 3d54  end(Line(close=T
-000057f0: 7275 652c 2064 6173 685f 6f66 6673 6574  rue, dash_offset
-00005800: 3d33 2c20 6461 7368 5f6c 656e 6774 683d  =3, dash_length=
-00005810: 3529 290d 0a09 0909 656c 7365 3a0d 0a09  5)).....else:...
-00005820: 0909 0973 656c 662e 6472 6177 5f6c 696e  ...self.draw_lin
-00005830: 6573 2e61 7070 656e 6428 4c69 6e65 2863  es.append(Line(c
-00005840: 6c6f 7365 3d46 616c 7365 2c20 6461 7368  lose=False, dash
-00005850: 5f6f 6666 7365 743d 332c 2064 6173 685f  _offset=3, dash_
-00005860: 6c65 6e67 7468 3d35 2929 0d0a 0d0a 0909  length=5))......
-00005870: 7365 6c66 2e63 616e 7661 732e 6166 7465  self.canvas.afte
-00005880: 722e 6164 6428 7365 6c66 2e64 7261 775f  r.add(self.draw_
-00005890: 636f 6c6f 7229 0d0a 0909 666f 7220 6c69  color)....for li
-000058a0: 6e65 2069 6e20 7365 6c66 2e64 7261 775f  ne in self.draw_
-000058b0: 6c69 6e65 733a 0d0a 0909 0973 656c 662e  lines:.....self.
-000058c0: 6361 6e76 6173 2e61 6674 6572 2e61 6464  canvas.after.add
-000058d0: 286c 696e 6529 0d0a 0d0a 0909 2320 5365  (line)......# Se
-000058e0: 6375 7269 6e67 2064 7261 7720 6f6e 2061  curing draw on a
-000058f0: 2073 7461 7469 6f6e 6172 7920 7769 6467   stationary widg
-00005900: 6574 2e0d 0a09 0973 656c 662e 7820 2b3d  et.....self.x +=
-00005910: 2030 2e30 3031 0d0a 0909 7365 6c66 2e74   0.001....self.t
-00005920: 7269 6767 6572 5f64 7261 7728 290d 0a0d  rigger_draw()...
-00005930: 0a09 6465 6620 6472 6177 2873 656c 662c  ..def draw(self,
-00005940: 202a 6172 6773 293a 0d0a 0909 2727 2720   *args):....''' 
-00005950: 4966 205b 6472 6177 5f62 6f75 6e64 735d  If [draw_bounds]
-00005960: 2069 7320 5472 7565 2c20 7669 7375 616c   is True, visual
-00005970: 6973 6573 2074 6865 2077 6964 6765 7427  ises the widget'
-00005980: 7320 626f 756e 6473 2e20 466f 7220 7465  s bounds. For te
-00005990: 7374 696e 672e 0d0a 0909 2727 2720 0d0a  sting.....''' ..
-000059a0: 0909 6966 206e 6f74 2073 656c 662e 7072  ..if not self.pr
-000059b0: 6570 6172 6564 3a0d 0a09 0909 7265 7475  epared:.....retu
-000059c0: 726e 204e 6f6e 650d 0a09 090d 0a09 0974  rn None........t
-000059d0: 7279 3a0d 0a09 0909 626f 756e 6473 203d  ry:.....bounds =
-000059e0: 2070 6565 7273 5b73 656c 662e 7269 645d   peers[self.rid]
-000059f0: 5b73 656c 662e 6375 7272 5f6b 6579 5d0d  [self.curr_key].
-00005a00: 0a09 0965 7863 6570 7420 4b65 7945 7272  ...except KeyErr
-00005a10: 6f72 3a0d 0a09 0909 7265 7475 726e 204e  or:.....return N
-00005a20: 6f6e 650d 0a0d 0a09 0973 7461 7274 203d  one......start =
-00005a30: 2030 0d0a 0909 666f 7220 692c 206c 656e   0....for i, len
-00005a40: 6720 696e 2065 6e75 6d65 7261 7465 2862  g in enumerate(b
-00005a50: 6f75 6e64 735b 2770 6f6c 5f6c 656e 7327  ounds['pol_lens'
-00005a60: 5d29 3a0d 0a09 0909 7365 6c66 2e64 7261  ]):.....self.dra
-00005a70: 775f 6c69 6e65 735b 695d 2e70 6f69 6e74  w_lines[i].point
-00005a80: 7320 3d20 5b62 6f75 6e64 735b 2770 6f69  s = [bounds['poi
-00005a90: 6e74 7327 5d5b 6a5d 2066 6f72 206a 2069  nts'][j] for j i
-00005aa0: 6e20 7261 6e67 6528 7374 6172 742c 2073  n range(start, s
-00005ab0: 7461 7274 202b 206c 656e 6720 2a20 3229  tart + leng * 2)
-00005ac0: 5d0d 0a09 0909 7374 6172 7420 2b3d 206c  ].....start += l
-00005ad0: 656e 6720 2a20 320d 0a0d 0a0d 0a09 6465  eng * 2.......de
-00005ae0: 6620 6765 745f 7369 7a65 5f68 696e 745f  f get_size_hint_
-00005af0: 7828 7365 6c66 293a 0d0a 0909 2320 4c6f  x(self):....# Lo
-00005b00: 636b 696e 6720 7369 7a65 5f68 696e 7420  cking size_hint 
-00005b10: 7072 6f70 6572 7479 2074 6f20 4e6f 6e65  property to None
-00005b20: 2c20 4e6f 6e65 2c0d 0a09 0923 2069 6e20  , None,....# in 
-00005b30: 6f72 6465 7220 746f 206b 6565 7020 696e  order to keep in
-00005b40: 7465 6e64 6564 2061 7370 6563 7420 7261  tended aspect ra
-00005b50: 7469 6f20 2863 7269 7469 6361 6c20 666f  tio (critical fo
-00005b60: 7220 6375 7374 6f6d 2062 6f75 6e64 7329  r custom bounds)
-00005b70: 2e0d 0a09 0972 6574 7572 6e20 4e6f 6e65  .....return None
-00005b80: 0d0a 0d0a 0964 6566 2073 6574 5f73 697a  .....def set_siz
-00005b90: 655f 6869 6e74 5f78 2873 656c 662c 2076  e_hint_x(self, v
-00005ba0: 616c 7565 293a 0d0a 0909 7261 6973 6520  alue):....raise 
-00005bb0: 4578 6365 7074 696f 6e28 2252 6f74 6162  Exception("Rotab
-00005bc0: 6f78 2063 616e 2774 2075 7365 2073 697a  ox can't use siz
-00005bd0: 655f 6869 6e74 2e22 290d 0a09 0d0a 0973  e_hint.")......s
-00005be0: 697a 655f 6869 6e74 5f78 203d 2041 6c69  ize_hint_x = Ali
-00005bf0: 6173 5072 6f70 6572 7479 2867 6574 5f73  asProperty(get_s
-00005c00: 697a 655f 6869 6e74 5f78 2c20 7365 745f  ize_hint_x, set_
-00005c10: 7369 7a65 5f68 696e 745f 7829 0d0a 0d0a  size_hint_x)....
-00005c20: 0d0a 0964 6566 2067 6574 5f73 697a 655f  ...def get_size_
-00005c30: 6869 6e74 5f79 2873 656c 6629 3a0d 0a09  hint_y(self):...
-00005c40: 0972 6574 7572 6e20 4e6f 6e65 0d0a 0d0a  .return None....
-00005c50: 0964 6566 2073 6574 5f73 697a 655f 6869  .def set_size_hi
-00005c60: 6e74 5f79 2873 656c 662c 2076 616c 7565  nt_y(self, value
-00005c70: 293a 0d0a 0909 7261 6973 6520 4578 6365  ):....raise Exce
-00005c80: 7074 696f 6e28 2252 6f74 6162 6f78 2063  ption("Rotabox c
-00005c90: 616e 2774 2075 7365 2073 697a 655f 6869  an't use size_hi
-00005ca0: 6e74 2e22 290d 0a0d 0a09 7369 7a65 5f68  nt.").....size_h
-00005cb0: 696e 745f 7920 3d20 416c 6961 7350 726f  int_y = AliasPro
-00005cc0: 7065 7274 7928 6765 745f 7369 7a65 5f68  perty(get_size_h
-00005cd0: 696e 745f 792c 2073 6574 5f73 697a 655f  int_y, set_size_
-00005ce0: 6869 6e74 5f79 290d 0a09 7369 7a65 5f68  hint_y)...size_h
-00005cf0: 696e 7420 3d20 5265 6665 7265 6e63 654c  int = ReferenceL
-00005d00: 6973 7450 726f 7065 7274 7928 7369 7a65  istProperty(size
-00005d10: 5f68 696e 745f 782c 2073 697a 655f 6869  _hint_x, size_hi
-00005d20: 6e74 5f79 290d 0a0d 0a0d 0a09 6f72 6967  nt_y).......orig
-00005d30: 696e 616c 5f73 697a 6520 3d20 4c69 7374  inal_size = List
-00005d40: 5072 6f70 6572 7479 285b 312c 2031 5d29  Property([1, 1])
-00005d50: 0d0a 0922 2222 0d0a 0955 7365 6420 666f  ..."""...Used fo
-00005d60: 7220 6361 6c63 756c 6174 696e 6720 7468  r calculating th
-00005d70: 6520 7769 6467 6574 2773 2073 6361 6c65  e widget's scale
-00005d80: 2e20 4974 2773 2074 6865 2075 7365 7227  . It's the user'
-00005d90: 7320 696e 7075 7420 7369 7a65 0d0a 096f  s input size...o
-00005da0: 7220 7468 6520 5b74 6578 7475 7265 5f73  r the [texture_s
-00005db0: 697a 655d 206f 6620 7468 6520 7769 6467  ize] of the widg
-00005dc0: 6574 2773 205b 696d 6167 655d 2e0d 0a09  et's [image]....
-00005dd0: 2222 220d 0a0d 0a09 7069 766f 745f 626f  """.....pivot_bo
-00005de0: 6e64 203d 204c 6973 7450 726f 7065 7274  nd = ListPropert
-00005df0: 7928 5b2e 352c 202e 355d 290d 0a09 2222  y([.5, .5])...""
-00005e00: 220d 0a09 4120 6672 6163 7469 6f6e 616c  "...A fractional
-00005e10: 2076 616c 7565 2074 6861 7420 6b65 6570   value that keep
-00005e20: 7320 5b70 6976 6f74 5d20 7265 6c61 7469  s [pivot] relati
-00005e30: 7665 2074 6f20 7468 6520 7769 6467 6574  ve to the widget
-00005e40: 2773 2073 697a 650d 0a09 616e 6420 706f  's size...and po
-00005e50: 7369 7469 6f6e 2e20 5b6f 7269 6769 6e5d  sition. [origin]
-00005e60: 2073 6574 7320 616e 6420 6368 616e 6765   sets and change
-00005e70: 7320 6974 2e0d 0a09 2222 220d 0a0d 0a09  s it....""".....
-00005e80: 616c 6c6f 7720 3d20 426f 6f6c 6561 6e50  allow = BooleanP
-00005e90: 726f 7065 7274 7928 3129 0d0a 0922 2222  roperty(1)..."""
-00005ea0: 2053 7769 7463 6820 746f 2073 7573 7065   Switch to suspe
-00005eb0: 6e64 2062 6f75 6e64 7327 2075 7064 6174  nd bounds' updat
-00005ec0: 6520 7768 696c 6520 7265 706f 7369 7469  e while repositi
-00005ed0: 6f6e 696e 672c 2064 7572 696e 6720 616e  oning, during an
-00005ee0: 205b 6f72 6967 696e 5d20 6368 616e 6765   [origin] change
-00005ef0: 206f 7220 6120 7265 7369 7a65 2e0d 0a09   or a resize....
-00005f00: 2222 220d 0a                             """..
+00000000: 0d0a 6672 6f6d 206b 6976 7967 6f2e 7769  ..from kivygo.wi
+00000010: 6467 6574 732e 7769 6467 6574 2069 6d70  dgets.widget imp
+00000020: 6f72 7420 476f 5769 6467 6574 0d0a 6672  ort GoWidget..fr
+00000030: 6f6d 206b 6976 792e 7569 782e 696d 6167  om kivy.uix.imag
+00000040: 6520 696d 706f 7274 2049 6d61 6765 0d0a  e import Image..
+00000050: 6672 6f6d 206b 6976 792e 636c 6f63 6b20  from kivy.clock 
+00000060: 696d 706f 7274 2043 6c6f 636b 0d0a 6672  import Clock..fr
+00000070: 6f6d 206b 6976 792e 7665 6374 6f72 2069  om kivy.vector i
+00000080: 6d70 6f72 7420 5665 6374 6f72 0d0a 6672  mport Vector..fr
+00000090: 6f6d 206b 6976 792e 6772 6170 6869 6373  om kivy.graphics
+000000a0: 2069 6d70 6f72 7420 5075 7368 4d61 7472   import PushMatr
+000000b0: 6978 2c20 526f 7461 7465 2c20 506f 704d  ix, Rotate, PopM
+000000c0: 6174 7269 780d 0a66 726f 6d20 6b69 7679  atrix..from kivy
+000000d0: 2e67 7261 7068 6963 732e 636f 6e74 6578  .graphics.contex
+000000e0: 745f 696e 7374 7275 6374 696f 6e73 2069  t_instructions i
+000000f0: 6d70 6f72 7420 436f 6c6f 720d 0a66 726f  mport Color..fro
+00000100: 6d20 6b69 7679 2e67 7261 7068 6963 732e  m kivy.graphics.
+00000110: 7665 7274 6578 5f69 6e73 7472 7563 7469  vertex_instructi
+00000120: 6f6e 7320 696d 706f 7274 204c 696e 650d  ons import Line.
+00000130: 0a66 726f 6d20 6b69 7679 2e61 746c 6173  .from kivy.atlas
+00000140: 2069 6d70 6f72 7420 4174 6c61 730d 0a0d   import Atlas...
+00000150: 0a66 726f 6d20 6b69 7679 2e70 726f 7065  .from kivy.prope
+00000160: 7274 6965 7320 696d 706f 7274 2028 0d0a  rties import (..
+00000170: 094e 756d 6572 6963 5072 6f70 6572 7479  .NumericProperty
+00000180: 2c20 5265 6665 7265 6e63 654c 6973 7450  , ReferenceListP
+00000190: 726f 7065 7274 792c 0d0a 0941 6c69 6173  roperty,...Alias
+000001a0: 5072 6f70 6572 7479 2c20 4f62 6a65 6374  Property, Object
+000001b0: 5072 6f70 6572 7479 2c20 426f 6f6c 6561  Property, Boolea
+000001c0: 6e50 726f 7065 7274 792c 0d0a 094c 6973  nProperty,...Lis
+000001d0: 7450 726f 7065 7274 792c 2042 6f75 6e64  tProperty, Bound
+000001e0: 6564 4e75 6d65 7269 6350 726f 7065 7274  edNumericPropert
+000001f0: 792c 0d0a 0953 7472 696e 6750 726f 7065  y,...StringPrope
+00000200: 7274 790d 0a29 0d0a 0d0a 6672 6f6d 206d  rty..)....from m
+00000210: 6174 6820 696d 706f 7274 2072 6164 6961  ath import radia
+00000220: 6e73 2c20 7369 6e2c 2063 6f73 0d0a 696d  ns, sin, cos..im
+00000230: 706f 7274 206a 736f 6e0d 0a0d 0a66 726f  port json....fro
+00000240: 6d20 6b69 7679 676f 2e62 6f75 6e64 735f  m kivygo.bounds_
+00000250: 6d61 7468 2069 6d70 6f72 7420 280d 0a09  math import (...
+00000260: 7065 6572 732c 2064 6566 696e 655f 626f  peers, define_bo
+00000270: 756e 6473 2c20 7265 7369 7a65 2c0d 0a09  unds, resize,...
+00000280: 7570 6461 7465 5f62 6f75 6e64 732c 2061  update_bounds, a
+00000290: 6e69 7265 7369 7a65 2c20 616e 6975 7064  niresize, aniupd
+000002a0: 6174 655f 626f 756e 6473 2c0d 0a09 706f  ate_bounds,...po
+000002b0: 696e 745f 696e 5f62 6f75 6e64 732c 2063  int_in_bounds, c
+000002c0: 6f6c 6c69 6465 5f62 6f75 6e64 730d 0a29  ollide_bounds..)
+000002d0: 0d0a 0d0a 0d0a 636c 6173 7320 476f 526f  ......class GoRo
+000002e0: 7461 626f 7828 476f 5769 6467 6574 293a  tabox(GoWidget):
+000002f0: 0d0a 0d0a 0973 6f75 7263 655f 6372 6f70  .....source_crop
+00000300: 203d 2053 7472 696e 6750 726f 7065 7274   = StringPropert
+00000310: 7928 2222 290d 0a0d 0a09 6375 7272 656e  y("").....curren
+00000320: 745f 696d 6167 6520 3d20 5374 7269 6e67  t_image = String
+00000330: 5072 6f70 6572 7479 2822 626f 756e 6473  Property("bounds
+00000340: 2229 0d0a 0d0a 0973 6f75 7263 655f 626f  ").....source_bo
+00000350: 756e 6473 203d 2053 7472 696e 6750 726f  unds = StringPro
+00000360: 7065 7274 7928 2222 290d 0a0d 0a09 6174  perty("").....at
+00000370: 6c61 7320 3d20 4f62 6a65 6374 5072 6f70  las = ObjectProp
+00000380: 6572 7479 284e 6f6e 6529 0d0a 090d 0a0d  erty(None)......
+00000390: 0a09 696d 6167 6520 3d20 4f62 6a65 6374  ..image = Object
+000003a0: 5072 6f70 6572 7479 284e 6f6e 6529 0d0a  Property(None)..
+000003b0: 0927 2727 5468 6973 2073 686f 756c 6420  .'''This should 
+000003c0: 6265 2074 6865 2069 6d61 6765 2074 6861  be the image tha
+000003d0: 7420 616e 7920 6375 7374 6f6d 2062 6f75  t any custom bou
+000003e0: 6e64 7320 6172 6520 6d65 616e 7420 666f  nds are meant fo
+000003f0: 722e 0d0a 0949 6620 6e6f 7420 6465 6669  r....If not defi
+00000400: 6e65 642c 2077 6964 6765 7420 7769 6c6c  ned, widget will
+00000410: 2074 7279 2074 6f20 6c6f 6361 7465 2074   try to locate t
+00000420: 6865 2074 6f70 6d6f 7374 2069 6d61 6765  he topmost image
+00000430: 2069 6e20 6974 7320 7472 6565 2e0d 0a09   in its tree....
+00000440: 2727 270d 0a0d 0a09 6173 7065 6374 5f72  '''.....aspect_r
+00000450: 6174 696f 203d 204e 756d 6572 6963 5072  atio = NumericPr
+00000460: 6f70 6572 7479 2830 2e30 290d 0a09 2727  operty(0.0)...''
+00000470: 2754 6865 2077 6964 6765 7427 7320 6173  'The widget's as
+00000480: 7065 6374 2072 6174 696f 2e20 4966 206e  pect ratio. If n
+00000490: 6f74 2064 6566 696e 6564 2c20 696d 6167  ot defined, imag
+000004a0: 6527 7320 7261 7469 6f20 7769 6c6c 2062  e's ratio will b
+000004b0: 6520 7573 6564 2e0d 0a09 2727 270d 0a0d  e used....'''...
+000004c0: 0a09 616e 676c 6520 3d20 4e75 6d65 7269  ..angle = Numeri
+000004d0: 6350 726f 7065 7274 7928 3029 0d0a 0927  cProperty(0)...'
+000004e0: 2727 416e 676c 6520 6f66 2052 6f74 6174  ''Angle of Rotat
+000004f0: 696f 6e2e 0d0a 0927 2727 0d0a 0d0a 0d0a  ion....'''......
+00000500: 0964 6566 2067 6574 5f6f 7269 6769 6e28  .def get_origin(
+00000510: 7365 6c66 293a 0d0a 0909 7265 7475 726e  self):....return
+00000520: 2073 656c 662e 7069 766f 740d 0a0d 0a09   self.pivot.....
+00000530: 6465 6620 7365 745f 6f72 6967 696e 2873  def set_origin(s
+00000540: 656c 662c 2070 6f69 6e74 293a 0d0a 0909  elf, point):....
+00000550: 616e 676c 6520 3d20 2d72 6164 6961 6e73  angle = -radians
+00000560: 2873 656c 662e 6c61 7374 5f61 6e67 6c65  (self.last_angle
+00000570: 290d 0a09 096f 7269 6720 3d20 7365 6c66  )....orig = self
+00000580: 2e6f 7269 6769 6e0d 0a09 0973 203d 2073  .origin....s = s
+00000590: 696e 2861 6e67 6c65 290d 0a09 0963 203d  in(angle)....c =
+000005a0: 2063 6f73 2861 6e67 6c65 290d 0a0d 0a09   cos(angle).....
+000005b0: 0923 206e 6f72 6d61 6c69 7a65 2028 7472  .# normalize (tr
+000005c0: 616e 736c 6174 6520 706f 696e 7420 736f  anslate point so
+000005d0: 206f 7269 6769 6e20 7769 6c6c 2062 6520   origin will be 
+000005e0: 302c 3029 0d0a 0909 6478 203d 2070 6f69  0,0)....dx = poi
+000005f0: 6e74 5b30 5d20 2d20 6f72 6967 5b30 5d0d  nt[0] - orig[0].
+00000600: 0a09 0964 7920 3d20 706f 696e 745b 315d  ...dy = point[1]
+00000610: 202d 206f 7269 675b 315d 0d0a 0d0a 0909   - orig[1]......
+00000620: 2320 756e 2d72 6f74 6174 6520 706f 696e  # un-rotate poin
+00000630: 740d 0a09 0978 6e65 7720 3d20 6478 202a  t....xnew = dx *
+00000640: 2063 202d 2064 7920 2a20 730d 0a09 0979   c - dy * s....y
+00000650: 6e65 7720 3d20 6478 202a 2073 202b 2064  new = dx * s + d
+00000660: 7920 2a20 630d 0a0d 0a09 0923 2074 7261  y * c......# tra
+00000670: 6e73 6c61 7465 2070 6f69 6e74 2062 6163  nslate point bac
+00000680: 6b3a 0d0a 0909 7069 766f 7420 3d20 786e  k:....pivot = xn
+00000690: 6577 202b 206f 7269 675b 305d 2c20 796e  ew + orig[0], yn
+000006a0: 6577 202b 206f 7269 675b 315d 0d0a 0d0a  ew + orig[1]....
+000006b0: 0909 2320 6c6f 636b 2070 6f73 2d70 6976  ..# lock pos-piv
+000006c0: 6f74 2072 656c 6174 696f 6e0d 0a09 0973  ot relation....s
+000006d0: 656c 662e 7069 766f 745f 626f 6e64 203d  elf.pivot_bond =
+000006e0: 205b 2870 6976 6f74 5b30 5d20 2d20 7365   [(pivot[0] - se
+000006f0: 6c66 2e78 2920 2f20 666c 6f61 7428 7365  lf.x) / float(se
+00000700: 6c66 2e77 6964 7468 292c 0d0a 0909 0909  lf.width),......
+00000710: 0909 2020 2028 7069 766f 745b 315d 202d  ..   (pivot[1] -
+00000720: 2073 656c 662e 7929 202f 2066 6c6f 6174   self.y) / float
+00000730: 2873 656c 662e 6865 6967 6874 295d 0d0a  (self.height)]..
+00000740: 0d0a 0909 2320 5369 6e63 6520 7468 6520  ....# Since the 
+00000750: 696d 6167 6520 286f 6e20 6361 6e76 6173  image (on canvas
+00000760: 2920 616c 7761 7973 2073 7461 7274 7320  ) always starts 
+00000770: 6561 6368 2066 7261 6d65 2069 6e20 7a65  each frame in ze
+00000780: 726f 2061 6e67 6c65 2c0d 0a09 0923 2061  ro angle,....# a
+00000790: 6e20 5b6f 7269 6769 6e5d 2063 6861 6e67  n [origin] chang
+000007a0: 6520 696e 2061 6e79 206e 6f6e 2d7a 6572  e in any non-zer
+000007b0: 6f20 616e 676c 6520 6272 6561 6b73 2074  o angle breaks t
+000007c0: 6865 2063 6f6e 7469 6e75 6974 7920 6f66  he continuity of
+000007d0: 0d0a 0909 2320 6d6f 7469 6f6e 2f72 6f74  ....# motion/rot
+000007e0: 6174 696f 6e2c 2069 6e74 726f 6475 6369  ation, introduci
+000007f0: 6e67 2061 6e20 696d 6167 6520 7472 616e  ng an image tran
+00000800: 736c 6174 696f 6e20 286a 756d 7029 2e0d  slation (jump)..
+00000810: 0a09 0923 2063 6f6d 7065 6e73 6174 696e  ...# compensatin
+00000820: 6720 6279 2063 6861 6e67 696e 6720 7468  g by changing th
+00000830: 6520 7769 6467 6574 2773 2070 6f73 6974  e widget's posit
+00000840: 696f 6e2e 0d0a 0d0a 0909 2320 7072 6576  ion.......# prev
+00000850: 656e 7420 6120 626f 756e 6473 2720 7570  ent a bounds' up
+00000860: 6461 7465 2074 6f20 5b70 6f73 5d20 6368  date to [pos] ch
+00000870: 616e 6765 2062 656c 6f77 2e0d 0a09 0973  ange below.....s
+00000880: 656c 662e 616c 6c6f 7720 3d20 300d 0a0d  elf.allow = 0...
+00000890: 0a09 0923 2063 6f6d 7065 6e73 6174 696e  ...# compensatin
+000008a0: 6720 666f 7220 696d 6167 6520 7472 616e  g for image tran
+000008b0: 736c 6174 696f 6e0d 0a09 0973 656c 662e  slation....self.
+000008c0: 706f 7320 3d20 2873 656c 662e 7820 2d20  pos = (self.x - 
+000008d0: 2870 6976 6f74 5b30 5d20 2d20 706f 696e  (pivot[0] - poin
+000008e0: 745b 305d 292c 0d0a 0909 0909 0973 656c  t[0]),.......sel
+000008f0: 662e 7920 2d20 2870 6976 6f74 5b31 5d20  f.y - (pivot[1] 
+00000900: 2d20 706f 696e 745b 315d 2929 0d0a 0d0a  - point[1]))....
+00000910: 0909 2320 6361 6e6e 6f74 2077 6169 7420  ..# cannot wait 
+00000920: 666f 7220 7468 6520 7472 6967 6765 7265  for the triggere
+00000930: 6420 5b75 7064 6174 655d 2c20 6174 2074  d [update], at t
+00000940: 6865 2065 6e64 206f 6620 7468 6973 2066  he end of this f
+00000950: 7261 6d65 2c0d 0a09 0923 2073 696e 6365  rame,....# since
+00000960: 2069 7420 6d69 6768 7420 636f 6e63 6572   it might concer
+00000970: 6e20 6f74 6865 7220 6368 616e 6765 7320  n other changes 
+00000980: 7468 6174 2072 6571 7569 7265 2061 2062  that require a b
+00000990: 6f75 6e64 7327 2075 7064 6174 652e 0d0a  ounds' update...
+000009a0: 0909 2320 7365 6c66 2e75 7064 6174 6528  ..# self.update(
+000009b0: 290d 0a09 0973 656c 662e 7472 6967 6765  )....self.trigge
+000009c0: 725f 7570 6461 7465 2829 0d0a 0d0a 096f  r_update().....o
+000009d0: 7269 6769 6e20 3d20 416c 6961 7350 726f  rigin = AliasPro
+000009e0: 7065 7274 7928 6765 745f 6f72 6967 696e  perty(get_origin
+000009f0: 2c20 7365 745f 6f72 6967 696e 290d 0a09  , set_origin)...
+00000a00: 2727 2753 6574 7320 7468 6520 706f 696e  '''Sets the poin
+00000a10: 7420 6f66 2072 6f74 6174 696f 6e2e 2044  t of rotation. D
+00000a20: 6566 6175 6c74 2076 616c 7565 2069 7320  efault value is 
+00000a30: 7468 6520 7769 6467 6574 2773 2063 656e  the widget's cen
+00000a40: 7465 722e 0d0a 0957 6f72 6b73 206e 6963  ter....Works nic
+00000a50: 656c 7920 7769 7468 2074 6865 205b 6765  ely with the [ge
+00000a60: 745f 706f 696e 745d 206d 6574 686f 6420  t_point] method 
+00000a70: 6265 6c6f 7720 616e 6420 706f 696e 7473  below and points
+00000a80: 2061 6c72 6561 6479 2064 6566 696e 6564   already defined
+00000a90: 2069 6e0d 0a09 5b63 7573 746f 6d5f 626f   in...[custom_bo
+00000aa0: 756e 6473 5d2e 0d0a 0927 2727 0d0a 0d0a  unds]....'''....
+00000ab0: 0d0a 0961 6c6c 6f77 5f72 6f74 6162 6f78  ...allow_rotabox
+00000ac0: 203d 2042 6f6f 6c65 616e 5072 6f70 6572   = BooleanProper
+00000ad0: 7479 2854 7275 6529 0d0a 0927 2727 456e  ty(True)...'''En
+00000ae0: 6162 6c65 7320 7769 6467 6574 2773 2061  ables widget's a
+00000af0: 6476 616e 6365 6420 636f 6c6c 6973 696f  dvanced collisio
+00000b00: 6e20 6465 7465 6374 696f 6e2e 2049 6620  n detection. If 
+00000b10: 4661 6c73 652c 2077 6964 6765 7420 7769  False, widget wi
+00000b20: 6c6c 0d0a 0963 6f6c 6c69 6465 2061 7320  ll...collide as 
+00000b30: 6120 6e6f 726d 616c 2028 6e6f 6e2d 476f  a normal (non-Go
+00000b40: 526f 7461 626f 7829 2077 6964 6765 742e  Rotabox) widget.
+00000b50: 0d0a 0927 2727 0d0a 0d0a 0963 7573 746f  ...'''.....custo
+00000b60: 6d5f 626f 756e 6473 203d 204f 626a 6563  m_bounds = Objec
+00000b70: 7450 726f 7065 7274 7928 5b5b 2830 2e2c  tProperty([[(0.,
+00000b80: 2030 2e29 2c20 2831 2e2c 2030 2e29 2c20   0.), (1., 0.), 
+00000b90: 2831 2e2c 2031 2e29 2c20 2830 2e2c 2031  (1., 1.), (0., 1
+00000ba0: 2e29 5d5d 290d 0a09 2727 2743 7573 746f  .)]])...'''Custo
+00000bb0: 6d20 626f 756e 6473 2720 6465 6669 6e69  m bounds' defini
+00000bc0: 7469 6f6e 2069 6e74 6572 6661 6365 2e20  tion interface. 
+00000bd0: 2853 6565 206d 6f64 756c 6527 7320 646f  (See module's do
+00000be0: 6375 6d65 6e74 6174 696f 6e29 2e0d 0a09  cumentation)....
+00000bf0: 2727 270d 0a0d 0a09 7365 676d 656e 745f  '''.....segment_
+00000c00: 6d6f 6465 203d 2042 6f6f 6c65 616e 5072  mode = BooleanPr
+00000c10: 6f70 6572 7479 2854 7275 6529 0d0a 0927  operty(True)...'
+00000c20: 2727 436f 6c6c 6973 696f 6e20 6465 7465  ''Collision dete
+00000c30: 6374 696f 6e20 6d65 7468 6f64 2073 7769  ction method swi
+00000c40: 7463 6820 2873 6565 2064 6f63 756d 656e  tch (see documen
+00000c50: 7461 7469 6f6e 2061 626f 7665 292e 0d0a  tation above)...
+00000c60: 0927 2727 0d0a 0d0a 096f 7065 6e5f 626f  .'''.....open_bo
+00000c70: 756e 6473 203d 204c 6973 7450 726f 7065  unds = ListPrope
+00000c80: 7274 7928 5b5d 290d 0a09 2727 2728 7365  rty([])...'''(se
+00000c90: 676d 656e 745f 6d6f 6465 2920 4966 2061  gment_mode) If a
+00000ca0: 2070 6f6c 7967 6f6e 2773 2069 6e64 6578   polygon's index
+00000cb0: 2069 7320 696e 2074 6869 7320 6c69 7374   is in this list
+00000cc0: 2c20 7468 6520 7365 676d 656e 740d 0a09  , the segment...
+00000cd0: 6265 7477 6565 6e20 7468 6520 6c61 7374  between the last
+00000ce0: 2061 6e64 2066 6972 7374 2070 6f69 6e74   and first point
+00000cf0: 7320 6f66 2074 6865 2070 6f6c 7967 6f6e  s of the polygon
+00000d00: 2069 7320 6e6f 7420 636f 6e73 6964 6572   is not consider
+00000d10: 6564 2069 6e20 7468 650d 0a09 636f 6c6c  ed in the...coll
+00000d20: 6973 696f 6e20 6368 6563 6b73 2e0d 0a09  ision checks....
+00000d30: 2727 270d 0a0d 0a09 7072 655f 6368 6563  '''.....pre_chec
+00000d40: 6b20 3d20 426f 6f6c 6561 6e50 726f 7065  k = BooleanPrope
+00000d50: 7274 7928 4661 6c73 6529 0d0a 0927 2727  rty(False)...'''
+00000d60: 2843 7974 686f 6e29 2041 2063 6f6c 6c69  (Cython) A colli
+00000d70: 7369 6f6e 206f 7074 696d 697a 6174 696f  sion optimizatio
+00000d80: 6e20 7377 6974 6368 2066 6f72 206c 6172  n switch for lar
+00000d90: 6765 7220 7769 6467 6574 7320 2834 352b  ger widgets (45+
+00000da0: 2070 6f69 6e74 7329 2e0d 0a09 4974 2773   points)....It's
+00000db0: 2061 6c77 6179 7320 5472 7565 2069 6e20   always True in 
+00000dc0: 5079 7468 6f6e 2062 7574 2069 6e20 4379  Python but in Cy
+00000dd0: 7468 6f6e 2c20 666f 7220 736d 616c 6c20  thon, for small 
+00000de0: 7769 6467 6574 732c 2074 6865 2073 6c69  widgets, the sli
+00000df0: 6768 7420 7461 7820 0d0a 0969 6e20 7570  ght tax ...in up
+00000e00: 6461 7469 6e67 2074 6865 2062 6f75 6e64  dating the bound
+00000e10: 7320 6f75 7477 6569 6768 7320 7468 6520  s outweighs the 
+00000e20: 6265 6e65 6669 7420 696e 2063 6f6c 6c69  benefit in colli
+00000e30: 7369 6f6e 2e0d 0a09 2727 270d 0a0d 0a0d  sion....'''.....
+00000e40: 0a09 6465 6620 6765 745f 616c 6c6f 775f  ..def get_allow_
+00000e50: 6472 6167 2873 656c 6629 3a0d 0a09 0972  drag(self):....r
+00000e60: 6574 7572 6e20 7365 6c66 2e61 6c6c 6f77  eturn self.allow
+00000e70: 5f64 7261 675f 782c 2073 656c 662e 616c  _drag_x, self.al
+00000e80: 6c6f 775f 6472 6167 5f79 0d0a 0d0a 0964  low_drag_y.....d
+00000e90: 6566 2073 6574 5f61 6c6c 6f77 5f64 7261  ef set_allow_dra
+00000ea0: 6728 7365 6c66 2c20 7661 6c75 6529 3a0d  g(self, value):.
+00000eb0: 0a09 0969 6620 7479 7065 2876 616c 7565  ...if type(value
+00000ec0: 2920 696e 2028 6c69 7374 2c20 7475 706c  ) in (list, tupl
+00000ed0: 6529 3a0d 0a09 0909 7365 6c66 2e61 6c6c  e):.....self.all
+00000ee0: 6f77 5f64 7261 675f 782c 2073 656c 662e  ow_drag_x, self.
+00000ef0: 616c 6c6f 775f 6472 6167 5f79 203d 2076  allow_drag_y = v
+00000f00: 616c 7565 0d0a 0909 656c 7365 3a0d 0a09  alue....else:...
+00000f10: 0909 7365 6c66 2e61 6c6c 6f77 5f64 7261  ..self.allow_dra
+00000f20: 675f 7820 3d20 7365 6c66 2e61 6c6c 6f77  g_x = self.allow
+00000f30: 5f64 7261 675f 7920 3d20 626f 6f6c 2876  _drag_y = bool(v
+00000f40: 616c 7565 290d 0a0d 0a09 616c 6c6f 775f  alue).....allow_
+00000f50: 6472 6167 203d 2041 6c69 6173 5072 6f70  drag = AliasProp
+00000f60: 6572 7479 2867 6574 5f61 6c6c 6f77 5f64  erty(get_allow_d
+00000f70: 7261 672c 2073 6574 5f61 6c6c 6f77 5f64  rag, set_allow_d
+00000f80: 7261 672c 2062 696e 643d 2827 616c 6c6f  rag, bind=('allo
+00000f90: 775f 6472 6167 5f78 272c 2027 616c 6c6f  w_drag_x', 'allo
+00000fa0: 775f 6472 6167 5f79 2729 290d 0a09 2727  w_drag_y'))...''
+00000fb0: 2741 6c6c 6f77 2074 6f75 6368 2074 7261  'Allow touch tra
+00000fc0: 6e73 6c61 7469 6f6e 206f 6e20 7468 6520  nslation on the 
+00000fd0: 5820 6f72 2059 2061 7869 732e 0d0a 0927  X or Y axis....'
+00000fe0: 2727 0d0a 0d0a 0961 6c6c 6f77 5f64 7261  ''.....allow_dra
+00000ff0: 675f 7820 3d20 426f 6f6c 6561 6e50 726f  g_x = BooleanPro
+00001000: 7065 7274 7928 4661 6c73 6529 0d0a 0927  perty(False)...'
+00001010: 2727 416c 6c6f 7720 746f 7563 6820 7472  ''Allow touch tr
+00001020: 616e 736c 6174 696f 6e20 6f6e 2074 6865  anslation on the
+00001030: 2058 2061 7869 732e 0d0a 0927 2727 0d0a   X axis....'''..
+00001040: 0d0a 0961 6c6c 6f77 5f64 7261 675f 7920  ...allow_drag_y 
+00001050: 3d20 426f 6f6c 6561 6e50 726f 7065 7274  = BooleanPropert
+00001060: 7928 4661 6c73 6529 0d0a 0927 2727 416c  y(False)...'''Al
+00001070: 6c6f 7720 746f 7563 6820 7472 616e 736c  low touch transl
+00001080: 6174 696f 6e20 6f6e 2074 6865 2059 2061  ation on the Y a
+00001090: 7869 732e 0d0a 0927 2727 0d0a 0d0a 0d0a  xis....'''......
+000010a0: 0973 696e 676c 655f 746f 7563 685f 726f  .single_touch_ro
+000010b0: 7461 7469 6f6e 203d 2042 6f6f 6c65 616e  tation = Boolean
+000010c0: 5072 6f70 6572 7479 2846 616c 7365 290d  Property(False).
+000010d0: 0a09 2727 2741 6c6c 6f77 2072 6f74 6174  ..'''Allow rotat
+000010e0: 696f 6e20 6172 6f75 6e64 205b 6f72 6967  ion around [orig
+000010f0: 696e 5d2e 0d0a 0927 2727 0d0a 0d0a 0973  in]....'''.....s
+00001100: 696e 676c 655f 746f 7563 685f 7363 616c  ingle_touch_scal
+00001110: 696e 6720 3d20 426f 6f6c 6561 6e50 726f  ing = BooleanPro
+00001120: 7065 7274 7928 4661 6c73 6529 0d0a 0927  perty(False)...'
+00001130: 2727 416c 6c6f 7720 7363 616c 696e 6720  ''Allow scaling 
+00001140: 6172 6f75 6e64 205b 6f72 6967 696e 5d2e  around [origin].
+00001150: 0d0a 0927 2727 0d0a 0d0a 096d 756c 7469  ...'''.....multi
+00001160: 5f74 6f75 6368 5f72 6f74 6174 696f 6e20  _touch_rotation 
+00001170: 3d20 426f 6f6c 6561 6e50 726f 7065 7274  = BooleanPropert
+00001180: 7928 4661 6c73 6529 0d0a 0927 2727 416c  y(False)...'''Al
+00001190: 6c6f 7720 6d75 6c74 6974 6f75 6368 2072  low multitouch r
+000011a0: 6f74 6174 696f 6e2e 205b 6f72 6967 696e  otation. [origin
+000011b0: 5d20 6973 2064 6566 696e 6564 2065 6163  ] is defined eac
+000011c0: 6820 7469 6d65 2062 7920 7468 6520 746f  h time by the to
+000011d0: 7563 682e 0d0a 0927 2727 0d0a 0d0a 096d  uch....'''.....m
+000011e0: 756c 7469 5f74 6f75 6368 5f73 6361 6c69  ulti_touch_scali
+000011f0: 6e67 203d 2042 6f6f 6c65 616e 5072 6f70  ng = BooleanProp
+00001200: 6572 7479 2846 616c 7365 290d 0a09 2727  erty(False)...''
+00001210: 2741 6c6c 6f77 206d 756c 7469 746f 7563  'Allow multitouc
+00001220: 6820 7363 616c 696e 672e 205b 6f72 6967  h scaling. [orig
+00001230: 696e 5d20 6973 2064 6566 696e 6564 2065  in] is defined e
+00001240: 6163 6820 7469 6d65 2062 7920 7468 6520  ach time by the 
+00001250: 746f 7563 682e 0d0a 0927 2727 0d0a 0d0a  touch....'''....
+00001260: 0973 696e 676c 655f 6472 6167 5f74 6f75  .single_drag_tou
+00001270: 6368 203d 2042 6f75 6e64 6564 4e75 6d65  ch = BoundedNume
+00001280: 7269 6350 726f 7065 7274 7928 312c 206d  ricProperty(1, m
+00001290: 696e 3d31 290d 0a09 2727 2748 6f77 206d  in=1)...'''How m
+000012a0: 616e 7920 746f 7563 6865 7320 7769 6c6c  any touches will
+000012b0: 2062 6520 7472 6561 7465 6420 6173 206f   be treated as o
+000012c0: 6e65 2073 696e 676c 6520 6472 6167 2074  ne single drag t
+000012d0: 6f75 6368 2e0d 0a09 2727 270d 0a0d 0a09  ouch....'''.....
+000012e0: 7369 6e67 6c65 5f74 7261 6e73 5f74 6f75  single_trans_tou
+000012f0: 6368 203d 2042 6f75 6e64 6564 4e75 6d65  ch = BoundedNume
+00001300: 7269 6350 726f 7065 7274 7928 312c 206d  ricProperty(1, m
+00001310: 696e 3d31 290d 0a09 2727 2748 6f77 206d  in=1)...'''How m
+00001320: 616e 7920 746f 7563 6865 7320 7769 6c6c  any touches will
+00001330: 2062 6520 7472 6561 7465 6420 6173 206f   be treated as o
+00001340: 6e65 2073 696e 676c 6520 726f 7461 7469  ne single rotati
+00001350: 6f6e 2f73 6361 6c69 6e67 2074 6f75 6368  on/scaling touch
+00001360: 2e0d 0a09 2727 270d 0a0d 0a09 746f 7563  ....'''.....touc
+00001370: 6865 645f 746f 5f66 726f 6e74 203d 2042  hed_to_front = B
+00001380: 6f6f 6c65 616e 5072 6f70 6572 7479 2846  ooleanProperty(F
+00001390: 616c 7365 290d 0a09 2727 2749 6620 746f  alse)...'''If to
+000013a0: 7563 6865 642c 2077 6964 6765 7420 7769  uched, widget wi
+000013b0: 6c6c 2062 6520 7075 7368 6564 2074 6f20  ll be pushed to 
+000013c0: 7468 6520 746f 7020 6f66 2070 6172 656e  the top of paren
+000013d0: 7420 7769 6467 6574 2074 7265 652e 0d0a  t widget tree...
+000013e0: 0927 2727 0d0a 0d0a 0963 6f6c 6c69 6465  .'''.....collide
+000013f0: 5f61 6674 6572 5f63 6869 6c64 7265 6e20  _after_children 
+00001400: 3d20 426f 6f6c 6561 6e50 726f 7065 7274  = BooleanPropert
+00001410: 7928 4661 6c73 6529 0d0a 0927 2727 4966  y(False)...'''If
+00001420: 2054 7275 652c 206c 696d 6974 696e 6720   True, limiting 
+00001430: 7468 6520 746f 7563 6820 696e 7369 6465  the touch inside
+00001440: 2074 6865 2062 6f75 6e64 7320 7769 6c6c   the bounds will
+00001450: 2062 6520 646f 6e65 2061 6674 6572 0d0a   be done after..
+00001460: 0964 6973 7061 6368 696e 6720 7468 6520  .dispaching the 
+00001470: 746f 7563 6820 746f 2074 6865 2063 6869  touch to the chi
+00001480: 6c64 2061 6e64 2067 7261 6e64 6368 696c  ld and grandchil
+00001490: 6472 656e 2c20 736f 2065 7665 6e20 6f75  dren, so even ou
+000014a0: 7473 6964 6520 7468 650d 0a09 626f 756e  tside the...boun
+000014b0: 6473 2074 6865 7920 6361 6e20 7374 696c  ds they can stil
+000014c0: 6c20 6265 2074 6f75 6368 6564 2e0d 0a09  l be touched....
+000014d0: 494d 504f 5254 414e 5420 4e4f 5445 3a20  IMPORTANT NOTE: 
+000014e0: 4772 616e 6463 6869 6c64 7265 6e2c 2069  Grandchildren, i
+000014f0: 6e73 6964 6520 6f72 206f 7574 7369 6465  nside or outside
+00001500: 2074 6865 2062 6f75 6e64 732c 2063 616e   the bounds, can
+00001510: 2063 6f6c 6c69 6465 0d0a 0909 696e 6465   collide....inde
+00001520: 7065 6e64 656e 746c 7920 4f4e 4c59 2069  pendently ONLY i
+00001530: 6620 7769 6467 6574 2069 7320 4e4f 5420  f widget is NOT 
+00001540: 524f 5441 5445 4420 285b 616e 676c 655d  ROTATED ([angle]
+00001550: 206d 7573 7420 6265 2030 292e 0d0a 0927   must be 0)....'
+00001560: 2727 0d0a 0d0a 0d0a 0964 6566 2067 6574  ''.......def get
+00001570: 5f73 6361 6c65 2873 656c 6629 3a0d 0a09  _scale(self):...
+00001580: 0972 6574 7572 6e20 666c 6f61 7428 7365  .return float(se
+00001590: 6c66 2e77 6964 7468 2920 2f20 7365 6c66  lf.width) / self
+000015a0: 2e6f 7269 6769 6e61 6c5f 7369 7a65 5b30  .original_size[0
+000015b0: 5d0d 0a0d 0a09 6465 6620 7365 745f 7363  ].....def set_sc
+000015c0: 616c 6528 7365 6c66 2c20 616d 6f75 6e74  ale(self, amount
+000015d0: 293a 0d0a 0909 6966 2061 6d6f 756e 7420  ):....if amount 
+000015e0: 3c20 7365 6c66 2e73 6361 6c65 5f6d 696e  < self.scale_min
+000015f0: 3a0d 0a09 0909 616d 6f75 6e74 203d 2073  :.....amount = s
+00001600: 656c 662e 7363 616c 655f 6d69 6e0d 0a09  elf.scale_min...
+00001610: 0965 6c69 6620 616d 6f75 6e74 203e 2073  .elif amount > s
+00001620: 656c 662e 7363 616c 655f 6d61 783a 0d0a  elf.scale_max:..
+00001630: 0909 0961 6d6f 756e 7420 3d20 7365 6c66  ...amount = self
+00001640: 2e73 6361 6c65 5f6d 6178 0d0a 0d0a 0909  .scale_max......
+00001650: 7069 766f 7420 3d20 7365 6c66 2e70 6976  pivot = self.piv
+00001660: 6f74 5b3a 5d0d 0a09 0973 656c 662e 7369  ot[:]....self.si
+00001670: 7a65 203d 2028 616d 6f75 6e74 202a 2073  ze = (amount * s
+00001680: 656c 662e 6f72 6967 696e 616c 5f73 697a  elf.original_siz
+00001690: 655b 305d 2c0d 0a09 0909 0909 2061 6d6f  e[0],....... amo
+000016a0: 756e 7420 2a20 7365 6c66 2e6f 7269 6769  unt * self.origi
+000016b0: 6e61 6c5f 7369 7a65 5b31 5d29 0d0a 0909  nal_size[1])....
+000016c0: 7365 6c66 2e70 6976 6f74 203d 2070 6976  self.pivot = piv
+000016d0: 6f74 0d0a 0909 6966 2073 656c 662e 696e  ot....if self.in
+000016e0: 6974 6961 6c5f 7363 616c 653a 0d0a 0909  itial_scale:....
+000016f0: 0972 6574 7572 6e0d 0a09 0973 656c 662e  .return....self.
+00001700: 696e 6974 6961 6c5f 7363 616c 6520 3d20  initial_scale = 
+00001710: 7365 6c66 2e73 6361 6c65 0d0a 090d 0a09  self.scale......
+00001720: 7363 616c 6520 3d20 416c 6961 7350 726f  scale = AliasPro
+00001730: 7065 7274 7928 6765 745f 7363 616c 652c  perty(get_scale,
+00001740: 2073 6574 5f73 6361 6c65 2c20 6269 6e64   set_scale, bind
+00001750: 3d28 2777 6964 7468 272c 2027 6865 6967  =('width', 'heig
+00001760: 6874 272c 2027 6f72 6967 696e 616c 5f73  ht', 'original_s
+00001770: 697a 6527 2929 0d0a 0927 2727 0d0a 0957  ize'))...'''...W
+00001780: 6964 6765 7427 7320 6375 7272 656e 7420  idget's current 
+00001790: 7363 616c 652e 2043 616c 6375 6c61 7465  scale. Calculate
+000017a0: 6420 6672 6f6d 205b 6f72 6967 696e 616c  d from [original
+000017b0: 5f73 697a 655d 2028 7573 6572 2773 2069  _size] (user's i
+000017c0: 6e70 7574 0d0a 095b 7369 7a65 5d20 6f72  nput...[size] or
+000017d0: 205b 696d 6167 655d 2773 205b 7465 7874   [image]'s [text
+000017e0: 7572 655f 7369 7a65 5d29 2e20 5573 6564  ure_size]). Used
+000017f0: 2066 6f72 2074 6f75 6368 2073 6361 6c69   for touch scali
+00001800: 6e67 2062 7574 2069 7420 6361 6e20 6265  ng but it can be
+00001810: 2061 6e0d 0a09 616c 7465 726e 6174 6976   an...alternativ
+00001820: 6520 746f 205b 7369 7a65 5d2e 0d0a 0927  e to [size]....'
+00001830: 2727 0d0a 0d0a 0973 6361 6c65 5f6d 696e  ''.....scale_min
+00001840: 203d 204e 756d 6572 6963 5072 6f70 6572   = NumericProper
+00001850: 7479 2830 2e30 3129 0d0a 0927 2727 4d69  ty(0.01)...'''Mi
+00001860: 6e69 6d75 6d20 7363 616c 6520 616c 6c6f  nimum scale allo
+00001870: 7765 642e 0d0a 0927 2727 0d0a 0d0a 0973  wed....'''.....s
+00001880: 6361 6c65 5f6d 6178 203d 204e 756d 6572  cale_max = Numer
+00001890: 6963 5072 6f70 6572 7479 2831 6532 3029  icProperty(1e20)
+000018a0: 0d0a 0927 2727 4d61 7869 6d75 6d20 7363  ...'''Maximum sc
+000018b0: 616c 6520 616c 6c6f 7765 642e 0d0a 0927  ale allowed....'
+000018c0: 2727 0d0a 0d0a 0d0a 0964 6566 2067 6574  ''.......def get
+000018d0: 5f70 6976 6f74 5f78 2873 656c 6629 3a0d  _pivot_x(self):.
+000018e0: 0a09 0972 6574 7572 6e20 7365 6c66 2e78  ...return self.x
+000018f0: 202b 2073 656c 662e 7769 6474 6820 2a20   + self.width * 
+00001900: 7365 6c66 2e70 6976 6f74 5f62 6f6e 645b  self.pivot_bond[
+00001910: 305d 0d0a 0d0a 0964 6566 2073 6574 5f70  0].....def set_p
+00001920: 6976 6f74 5f78 2873 656c 662c 2076 616c  ivot_x(self, val
+00001930: 7565 293a 0d0a 0909 6966 2073 656c 662e  ue):....if self.
+00001940: 7769 6474 6820 3e20 313a 0d0a 0909 0973  width > 1:.....s
+00001950: 656c 662e 7820 3d20 7661 6c75 6520 2d20  elf.x = value - 
+00001960: 7365 6c66 2e77 6964 7468 202a 2073 656c  self.width * sel
+00001970: 662e 7069 766f 745f 626f 6e64 5b30 5d0d  f.pivot_bond[0].
+00001980: 0a09 0965 6c69 6620 7661 6c75 6520 3e20  ...elif value > 
+00001990: 313a 0d0a 0909 0973 656c 662e 7465 6d70  1:.....self.temp
+000019a0: 5f70 6976 5f78 203d 2076 616c 7565 0d0a  _piv_x = value..
+000019b0: 0d0a 0964 6566 2067 6574 5f70 6976 6f74  ...def get_pivot
+000019c0: 5f79 2873 656c 6629 3a0d 0a09 0972 6574  _y(self):....ret
+000019d0: 7572 6e20 7365 6c66 2e79 202b 2073 656c  urn self.y + sel
+000019e0: 662e 6865 6967 6874 202a 2073 656c 662e  f.height * self.
+000019f0: 7069 766f 745f 626f 6e64 5b31 5d0d 0a0d  pivot_bond[1]...
+00001a00: 0a09 6465 6620 7365 745f 7069 766f 745f  ..def set_pivot_
+00001a10: 7928 7365 6c66 2c20 7661 6c75 6529 3a0d  y(self, value):.
+00001a20: 0a09 0969 6620 7365 6c66 2e68 6569 6768  ...if self.heigh
+00001a30: 7420 3e20 313a 0d0a 0909 0973 656c 662e  t > 1:.....self.
+00001a40: 7920 3d20 7661 6c75 6520 2d20 7365 6c66  y = value - self
+00001a50: 2e68 6569 6768 7420 2a20 7365 6c66 2e70  .height * self.p
+00001a60: 6976 6f74 5f62 6f6e 645b 315d 0d0a 0909  ivot_bond[1]....
+00001a70: 656c 6966 2076 616c 7565 203e 2031 3a0d  elif value > 1:.
+00001a80: 0a09 0909 7365 6c66 2e74 656d 705f 7069  ....self.temp_pi
+00001a90: 765f 7920 3d20 7661 6c75 650d 0a0d 0a09  v_y = value.....
+00001aa0: 7069 766f 745f 7820 3d20 416c 6961 7350  pivot_x = AliasP
+00001ab0: 726f 7065 7274 7928 6765 745f 7069 766f  roperty(get_pivo
+00001ac0: 745f 782c 2073 6574 5f70 6976 6f74 5f78  t_x, set_pivot_x
+00001ad0: 2c20 6269 6e64 3d28 2778 272c 2027 7769  , bind=('x', 'wi
+00001ae0: 6474 6827 2c20 2770 6976 6f74 5f62 6f6e  dth', 'pivot_bon
+00001af0: 6427 2929 0d0a 0970 6976 6f74 5f79 203d  d'))...pivot_y =
+00001b00: 2041 6c69 6173 5072 6f70 6572 7479 2867   AliasProperty(g
+00001b10: 6574 5f70 6976 6f74 5f79 2c20 7365 745f  et_pivot_y, set_
+00001b20: 7069 766f 745f 792c 2062 696e 643d 2827  pivot_y, bind=('
+00001b30: 7927 2c20 2768 6569 6768 7427 2c20 2770  y', 'height', 'p
+00001b40: 6976 6f74 5f62 6f6e 6427 2929 0d0a 0970  ivot_bond'))...p
+00001b50: 6976 6f74 203d 2052 6566 6572 656e 6365  ivot = Reference
+00001b60: 4c69 7374 5072 6f70 6572 7479 2870 6976  ListProperty(piv
+00001b70: 6f74 5f78 2c20 7069 766f 745f 7929 0d0a  ot_x, pivot_y)..
+00001b80: 0927 2727 0d0a 0950 6f69 6e74 206f 6620  .'''...Point of 
+00001b90: 726f 7461 7469 6f6e 2061 6e64 2073 6361  rotation and sca
+00001ba0: 6c69 6e67 2e0d 0a09 5768 696c 6520 5b6f  ling....While [o
+00001bb0: 7269 6769 6e5d 2070 726f 7065 7274 7920  rigin] property 
+00001bc0: 7365 7473 205b 7069 766f 745d 2773 2072  sets [pivot]'s r
+00001bd0: 656c 6174 696f 6e20 746f 2077 6964 6765  elation to widge
+00001be0: 742c 205b 7069 766f 745d 0d0a 0969 7473  t, [pivot]...its
+00001bf0: 656c 6620 6361 6e20 6265 2075 7365 6420  elf can be used 
+00001c00: 746f 2070 6f73 6974 696f 6e20 7468 6520  to position the 
+00001c10: 7769 6467 6574 2c20 6d75 6368 206c 696b  widget, much lik
+00001c20: 6520 5b70 6f73 5d20 6f72 205b 6365 6e74  e [pos] or [cent
+00001c30: 6572 5d2e 0d0a 0927 2727 0d0a 0d0a 0970  er]....'''.....p
+00001c40: 7265 7061 7265 6420 3d20 426f 6f6c 6561  repared = Boolea
+00001c50: 6e50 726f 7065 7274 7928 4661 6c73 6529  nProperty(False)
+00001c60: 0d0a 0927 2727 0d0a 0949 7473 2073 7461  ...'''...Its sta
+00001c70: 7465 2063 6861 6e67 6520 7369 676e 6966  te change signif
+00001c80: 6965 7320 6120 7265 7365 742e 2054 6865  ies a reset. The
+00001c90: 2072 6573 6574 2063 6f6d 706c 6574 696f   reset completio
+00001ca0: 6e20 7369 676e 616c 2c20 686f 7765 7665  n signal, howeve
+00001cb0: 722c 0d0a 0969 7320 7468 6520 636f 6e73  r,...is the cons
+00001cc0: 6571 7565 6e74 205b 7265 6164 795d 2073  equent [ready] s
+00001cd0: 7461 7465 2063 6861 6e67 6520 746f 2054  tate change to T
+00001ce0: 7275 652e 0d0a 0927 2727 0d0a 0d0a 0964  rue....'''.....d
+00001cf0: 7261 775f 626f 756e 6473 203d 2042 6f6f  raw_bounds = Boo
+00001d00: 6c65 616e 5072 6f70 6572 7479 2846 616c  leanProperty(Fal
+00001d10: 7365 290d 0a09 2727 2745 6e61 626c 6573  se)...'''Enables
+00001d20: 2062 6f75 6e64 7320 7669 7375 616c 697a   bounds visualiz
+00001d30: 6174 696f 6e20 2866 6f72 2074 6573 7469  ation (for testi
+00001d40: 6e67 292e 0d0a 0927 2727 0d0a 0d0a 0d0a  ng)....'''......
+00001d50: 095f 5f65 7665 6e74 735f 5f20 3d20 2827  .__events__ = ('
+00001d60: 6f6e 5f74 7261 6e73 666f 726d 5f77 6974  on_transform_wit
+00001d70: 685f 746f 7563 6827 2c20 276f 6e5f 746f  h_touch', 'on_to
+00001d80: 7563 6865 645f 746f 5f66 726f 6e74 2729  uched_to_front')
+00001d90: 0d0a 0d0a 0964 6566 206f 6e5f 7472 616e  .....def on_tran
+00001da0: 7366 6f72 6d5f 7769 7468 5f74 6f75 6368  sform_with_touch
+00001db0: 2873 656c 662c 2074 6f75 6368 293a 0d0a  (self, touch):..
+00001dc0: 0909 2727 270d 0a09 0943 616c 6c65 6420  ..'''....Called 
+00001dd0: 7768 656e 2061 2074 6f75 6368 2065 7665  when a touch eve
+00001de0: 6e74 2068 6173 2074 7261 6e73 666f 726d  nt has transform
+00001df0: 6564 2074 6865 2077 6964 6765 742e 0d0a  ed the widget...
+00001e00: 0909 4279 2064 6566 6175 6c74 2074 6869  ..By default thi
+00001e10: 7320 646f 6573 206e 6f74 6869 6e67 2c20  s does nothing, 
+00001e20: 6275 7420 6361 6e20 6265 206f 7665 7272  but can be overr
+00001e30: 6964 656e 2062 7920 6465 7269 7665 640d  iden by derived.
+00001e40: 0a09 0963 6c61 7373 6573 2074 6861 7420  ...classes that 
+00001e50: 6e65 6564 2074 6f20 7265 6163 7420 746f  need to react to
+00001e60: 2074 7261 6e73 666f 726d 6174 696f 6e73   transformations
+00001e70: 2063 6175 7365 6420 6279 2075 7365 720d   caused by user.
+00001e80: 0a09 0969 6e70 7574 2e0d 0a09 0927 2727  ...input.....'''
+00001e90: 0d0a 0909 7061 7373 0d0a 0d0a 0964 6566  ....pass.....def
+00001ea0: 206f 6e5f 746f 7563 6865 645f 746f 5f66   on_touched_to_f
+00001eb0: 726f 6e74 2873 656c 662c 2074 6f75 6368  ront(self, touch
+00001ec0: 293a 0d0a 0909 2727 270d 0a09 0943 616c  ):....'''....Cal
+00001ed0: 6c65 6420 7768 656e 2061 2074 6f75 6368  led when a touch
+00001ee0: 2065 7665 6e74 2063 6175 7365 7320 7468   event causes th
+00001ef0: 6520 7769 6467 6574 2074 6f20 6265 2062  e widget to be b
+00001f00: 726f 7567 6874 2074 6f20 7468 650d 0a09  rought to the...
+00001f10: 0966 726f 6e74 206f 6620 7468 6520 7061  .front of the pa
+00001f20: 7265 6e74 2028 6f6e 6c79 2069 6620 3a61  rent (only if :a
+00001f30: 7474 723a 6074 6f75 6368 6564 5f74 6f5f  ttr:`touched_to_
+00001f40: 6672 6f6e 7460 2069 7320 5472 7565 290d  front` is True).
+00001f50: 0a09 0927 2727 0d0a 0909 7061 7373 0d0a  ...'''....pass..
+00001f60: 0d0a 0d0a 0964 6566 205f 5f69 6e69 745f  .....def __init_
+00001f70: 5f28 7365 6c66 2c20 2a2a 6b77 6172 6773  _(self, **kwargs
+00001f80: 293a 0d0a 0909 7365 6c66 2e73 697a 6520  ):....self.size 
+00001f90: 3d20 5b31 2c20 315d 0d0a 0909 7365 6c66  = [1, 1]....self
+00001fa0: 2e74 656d 705f 7069 765f 7820 3d20 7365  .temp_piv_x = se
+00001fb0: 6c66 2e74 656d 705f 7069 765f 7920 3d20  lf.temp_piv_y = 
+00001fc0: 300d 0a09 0973 656c 662e 696e 6974 6961  0....self.initia
+00001fd0: 6c5f 7363 616c 6520 3d20 300d 0a09 0973  l_scale = 0....s
+00001fe0: 656c 662e 746f 7563 6865 7320 3d20 5b5d  elf.touches = []
+00001ff0: 0d0a 0909 7365 6c66 2e6c 6173 745f 746f  ....self.last_to
+00002000: 7563 685f 706f 7320 3d20 7b7d 0d0a 0909  uch_pos = {}....
+00002010: 0d0a 0909 7375 7065 7228 292e 5f5f 696e  ....super().__in
+00002020: 6974 5f5f 282a 2a6b 7761 7267 7329 0d0a  it__(**kwargs)..
+00002030: 0909 0d0a 0909 7365 6c66 2e69 6d61 6765  ......self.image
+00002040: 203d 2049 6d61 6765 2829 0d0a 0909 7365   = Image()....se
+00002050: 6c66 2e73 697a 6564 5f62 795f 696d 6720  lf.sized_by_img 
+00002060: 3d20 4661 6c73 650d 0a09 0973 656c 662e  = False....self.
+00002070: 7261 7469 6f20 3d20 310d 0a09 0973 656c  ratio = 1....sel
+00002080: 662e 6c61 7374 5f70 6f73 203d 205b 302c  f.last_pos = [0,
+00002090: 2030 5d0d 0a09 0973 656c 662e 6c61 7374   0]....self.last
+000020a0: 5f73 697a 6520 3d20 7365 6c66 2e73 697a  _size = self.siz
+000020b0: 655b 3a5d 0d0a 0909 7365 6c66 2e6c 6173  e[:]....self.las
+000020c0: 745f 616e 676c 6520 3d20 300d 0a09 0973  t_angle = 0....s
+000020d0: 656c 662e 616e 696d 203d 2046 616c 7365  elf.anim = False
+000020e0: 0d0a 0909 7365 6c66 2e72 6964 203d 2030  ....self.rid = 0
+000020f0: 0d0a 0909 7365 6c66 2e63 7572 725f 6b65  ....self.curr_ke
+00002100: 7920 3d20 2762 6f75 6e64 7327 0d0a 0909  y = 'bounds'....
+00002110: 7365 6c66 2e64 7261 775f 636f 6c6f 7220  self.draw_color 
+00002120: 3d20 436f 6c6f 7228 7267 6261 3d5b 302e  = Color(rgba=[0.
+00002130: 3239 2c20 302e 3531 382c 2031 2c20 315d  29, 0.518, 1, 1]
+00002140: 290d 0a09 0973 656c 662e 626f 785f 636f  )....self.box_co
+00002150: 6c6f 7220 3d20 436f 6c6f 7228 7267 6261  lor = Color(rgba
+00002160: 3d5b 302e 3335 2c20 302e 3135 2c20 302c  =[0.35, 0.15, 0,
+00002170: 2031 5d29 0d0a 0909 7365 6c66 2e64 7261   1])....self.dra
+00002180: 775f 6c69 6e65 7320 3d20 5b5d 0d0a 0909  w_lines = []....
+00002190: 7365 6c66 2e62 6f78 5f6c 696e 6573 203d  self.box_lines =
+000021a0: 205b 5d0d 0a09 0973 656c 662e 726f 7461   []....self.rota
+000021b0: 7469 6f6e 203d 2052 6f74 6174 6528 616e  tion = Rotate(an
+000021c0: 676c 653d 302c 206f 7269 6769 6e3d 7365  gle=0, origin=se
+000021d0: 6c66 2e63 656e 7465 7229 0d0a 0909 7365  lf.center)....se
+000021e0: 6c66 2e63 616e 7661 732e 6265 666f 7265  lf.canvas.before
+000021f0: 2e61 6464 2850 7573 684d 6174 7269 7828  .add(PushMatrix(
+00002200: 2929 0d0a 0909 7365 6c66 2e63 616e 7661  ))....self.canva
+00002210: 732e 6265 666f 7265 2e61 6464 2873 656c  s.before.add(sel
+00002220: 662e 726f 7461 7469 6f6e 290d 0a09 0973  f.rotation)....s
+00002230: 656c 662e 6361 6e76 6173 2e61 6674 6572  elf.canvas.after
+00002240: 2e61 6464 2850 6f70 4d61 7472 6978 2829  .add(PopMatrix()
+00002250: 290d 0a0d 0a09 0973 656c 662e 7472 6967  )......self.trig
+00002260: 6765 725f 7570 6461 7465 203d 2043 6c6f  ger_update = Clo
+00002270: 636b 2e63 7265 6174 655f 7472 6967 6765  ck.create_trigge
+00002280: 7228 7365 6c66 2e75 7064 6174 652c 202d  r(self.update, -
+00002290: 3129 0d0a 0909 7365 6c66 2e74 7269 6767  1)....self.trigg
+000022a0: 6572 5f64 7261 7720 3d20 436c 6f63 6b2e  er_draw = Clock.
+000022b0: 6372 6561 7465 5f74 7269 6767 6572 2873  create_trigger(s
+000022c0: 656c 662e 6472 6177 2c20 2d31 290d 0a0d  elf.draw, -1)...
+000022d0: 0a09 0973 656c 662e 6269 6e64 280d 0a09  ...self.bind(...
+000022e0: 0909 6368 696c 6472 656e 3d73 656c 662e  ..children=self.
+000022f0: 7472 6967 6765 725f 7570 6461 7465 2c0d  trigger_update,.
+00002300: 0a09 0909 7061 7265 6e74 3d73 656c 662e  ....parent=self.
+00002310: 7472 6967 6765 725f 7570 6461 7465 2c0d  trigger_update,.
+00002320: 0a09 0909 706f 733d 7365 6c66 2e74 7269  ....pos=self.tri
+00002330: 6767 6572 5f75 7064 6174 652c 0d0a 0909  gger_update,....
+00002340: 0970 6f73 5f68 696e 743d 7365 6c66 2e74  .pos_hint=self.t
+00002350: 7269 6767 6572 5f75 7064 6174 652c 0d0a  rigger_update,..
+00002360: 0909 0961 6e67 6c65 3d73 656c 662e 7472  ...angle=self.tr
+00002370: 6967 6765 725f 7570 6461 7465 2c0d 0a09  igger_update,...
+00002380: 0909 696d 6167 653d 7365 6c66 2e6f 6e5f  ..image=self.on_
+00002390: 7265 7365 742c 0d0a 0909 0961 7370 6563  reset,.....aspec
+000023a0: 745f 7261 7469 6f3d 7365 6c66 2e6f 6e5f  t_ratio=self.on_
+000023b0: 7265 7365 742c 0d0a 0909 0963 7573 746f  reset,.....custo
+000023c0: 6d5f 626f 756e 6473 3d73 656c 662e 6f6e  m_bounds=self.on
+000023d0: 5f72 6573 6574 2c0d 0a09 0909 616c 6c6f  _reset,.....allo
+000023e0: 775f 726f 7461 626f 783d 7365 6c66 2e6f  w_rotabox=self.o
+000023f0: 6e5f 7265 7365 742c 0d0a 0909 0964 7261  n_reset,.....dra
+00002400: 775f 626f 756e 6473 3d73 656c 662e 6f6e  w_bounds=self.on
+00002410: 5f72 6573 6574 0d0a 0909 290d 0a09 0d0a  _reset....).....
+00002420: 0964 6566 2061 6464 5f77 6964 6765 7428  .def add_widget(
+00002430: 7365 6c66 2c20 7769 6467 6574 2c20 2a2a  self, widget, **
+00002440: 6b77 6172 6773 293a 0d0a 0909 6966 2073  kwargs):....if s
+00002450: 656c 662e 6368 696c 6472 656e 3a0d 0a09  elf.children:...
+00002460: 0909 7261 6973 6520 4578 6365 7074 696f  ..raise Exceptio
+00002470: 6e28 2747 6f52 6f74 6162 6f78 2063 616e  n('GoRotabox can
+00002480: 206f 6e6c 7920 6861 7665 206f 6e65 2063   only have one c
+00002490: 6869 6c64 2e27 290d 0a09 0973 7570 6572  hild.')....super
+000024a0: 2829 2e61 6464 5f77 6964 6765 7428 7769  ().add_widget(wi
+000024b0: 6467 6574 290d 0a0d 0a09 6465 6620 6f6e  dget).....def on
+000024c0: 5f6f 7065 6e5f 626f 756e 6473 2873 656c  _open_bounds(sel
+000024d0: 662c 202a 6172 6773 293a 0d0a 0909 6966  f, *args):....if
+000024e0: 2073 656c 662e 6f70 656e 5f62 6f75 6e64   self.open_bound
+000024f0: 7320 616e 6420 6e6f 7420 7365 6c66 2e73  s and not self.s
+00002500: 6567 6d65 6e74 5f6d 6f64 653a 0d0a 0909  egment_mode:....
+00002510: 0972 6169 7365 2045 7863 6570 7469 6f6e  .raise Exception
+00002520: 2827 4f70 656e 2062 6f75 6e64 7320 6172  ('Open bounds ar
+00002530: 6520 6f6e 6c79 2061 7070 6c69 6361 626c  e only applicabl
+00002540: 6520 696e 2047 6f53 6567 6d65 6e74 206d  e in GoSegment m
+00002550: 6f64 652e 2729 0d0a 0d0a 0964 6566 206f  ode.').....def o
+00002560: 6e5f 736f 7572 6365 5f62 6f75 6e64 7328  n_source_bounds(
+00002570: 7365 6c66 2c20 2a61 7267 7329 3a0d 0a09  self, *args):...
+00002580: 0973 656c 662e 6375 7374 6f6d 5f62 6f75  .self.custom_bou
+00002590: 6e64 7320 3d20 7365 6c66 2e72 6561 645f  nds = self.read_
+000025a0: 626f 756e 6473 2873 656c 662e 736f 7572  bounds(self.sour
+000025b0: 6365 5f62 6f75 6e64 7329 0d0a 0d0a 0964  ce_bounds).....d
+000025c0: 6566 206f 6e5f 6375 7272 656e 745f 696d  ef on_current_im
+000025d0: 6167 6528 7365 6c66 2c20 2a61 7267 7329  age(self, *args)
+000025e0: 3a0d 0a09 0969 6620 7365 6c66 2e61 746c  :....if self.atl
+000025f0: 6173 203d 3d20 4e6f 6e65 3a0d 0a09 0909  as == None:.....
+00002600: 7265 7475 726e 204e 6f6e 650d 0a09 090d  return None.....
+00002610: 0a09 0973 656c 662e 696d 6167 652e 7465  ...self.image.te
+00002620: 7874 7572 6520 3d20 7365 6c66 2e61 746c  xture = self.atl
+00002630: 6173 2e74 6578 7475 7265 735b 7365 6c66  as.textures[self
+00002640: 2e63 7572 7265 6e74 5f69 6d61 6765 5d0d  .current_image].
+00002650: 0a09 0973 656c 662e 7072 6570 6172 6564  ...self.prepared
+00002660: 203d 2046 616c 7365 0d0a 0909 7365 6c66   = False....self
+00002670: 2e74 7269 6767 6572 5f75 7064 6174 6528  .trigger_update(
+00002680: 290d 0a0d 0a09 6465 6620 6f6e 5f73 6f75  ).....def on_sou
+00002690: 7263 655f 6372 6f70 2873 656c 662c 202a  rce_crop(self, *
+000026a0: 6172 6773 293a 0d0a 0909 6966 2073 656c  args):....if sel
+000026b0: 662e 736f 7572 6365 5f63 726f 7020 3d3d  f.source_crop ==
+000026c0: 2022 223a 0d0a 0909 0973 656c 662e 6174   "":.....self.at
+000026d0: 6c61 7320 3d20 4e6f 6e65 0d0a 0909 0973  las = None.....s
+000026e0: 656c 662e 696d 6167 6520 3d20 4e6f 6e65  elf.image = None
+000026f0: 0d0a 0909 0973 656c 662e 636c 6561 725f  .....self.clear_
+00002700: 7769 6467 6574 7328 290d 0a09 0909 7265  widgets().....re
+00002710: 7475 726e 204e 6f6e 650d 0a09 090d 0a09  turn None.......
+00002720: 0969 6620 7365 6c66 2e69 6d61 6765 2021  .if self.image !
+00002730: 3d20 4e6f 6e65 2061 6e64 206e 6f74 2073  = None and not s
+00002740: 656c 662e 696d 6167 6520 696e 2073 656c  elf.image in sel
+00002750: 662e 6368 696c 6472 656e 3a0d 0a09 0909  f.children:.....
+00002760: 7365 6c66 2e61 6464 5f77 6964 6765 7428  self.add_widget(
+00002770: 7365 6c66 2e69 6d61 6765 290d 0a09 090d  self.image).....
+00002780: 0a09 0973 656c 662e 6174 6c61 7320 3d20  ...self.atlas = 
+00002790: 4174 6c61 7328 7365 6c66 2e73 6f75 7263  Atlas(self.sourc
+000027a0: 655f 6372 6f70 290d 0a09 0973 656c 662e  e_crop)....self.
+000027b0: 696d 6167 652e 7465 7874 7572 6520 3d20  image.texture = 
+000027c0: 7475 706c 6528 7365 6c66 2e61 746c 6173  tuple(self.atlas
+000027d0: 2e74 6578 7475 7265 732e 7661 6c75 6573  .textures.values
+000027e0: 2829 295b 305d 0d0a 0909 0d0a 0964 6566  ())[0].......def
+000027f0: 206f 6e5f 7369 7a65 2873 656c 662c 202a   on_size(self, *
+00002800: 6172 6773 293a 0d0a 0909 7365 6c66 2e74  args):....self.t
+00002810: 7269 6767 6572 5f75 7064 6174 6528 290d  rigger_update().
+00002820: 0a0d 0a09 6465 6620 6f6e 5f72 6573 6574  ....def on_reset
+00002830: 2873 656c 662c 202a 6172 6773 293a 0d0a  (self, *args):..
+00002840: 0909 7365 6c66 2e74 7269 6767 6572 5f75  ..self.trigger_u
+00002850: 7064 6174 6528 290d 0a0d 0a09 6465 6620  pdate().....def 
+00002860: 7265 7365 745f 6472 6177 5f62 6f75 6e64  reset_draw_bound
+00002870: 7328 7365 6c66 2c20 2a61 7267 7329 3a0d  s(self, *args):.
+00002880: 0a09 0966 6f72 206c 696e 6520 696e 2073  ...for line in s
+00002890: 656c 662e 6472 6177 5f6c 696e 6573 3a0d  elf.draw_lines:.
+000028a0: 0a09 0909 7365 6c66 2e63 616e 7661 732e  ....self.canvas.
+000028b0: 6166 7465 722e 7265 6d6f 7665 286c 696e  after.remove(lin
+000028c0: 6529 0d0a 0909 7365 6c66 2e64 7261 775f  e)....self.draw_
+000028d0: 6c69 6e65 7320 3d20 5b5d 0d0a 0d0a 0909  lines = []......
+000028e0: 666f 7220 6c69 6e65 2069 6e20 7365 6c66  for line in self
+000028f0: 2e62 6f78 5f6c 696e 6573 3a0d 0a09 0909  .box_lines:.....
+00002900: 7365 6c66 2e63 616e 7661 732e 6166 7465  self.canvas.afte
+00002910: 722e 7265 6d6f 7665 286c 696e 6529 0d0a  r.remove(line)..
+00002920: 0909 7365 6c66 2e62 6f78 5f6c 696e 6573  ..self.box_lines
+00002930: 203d 205b 5d0d 0a0d 0a09 6465 6620 7072   = [].....def pr
+00002940: 6570 6172 6528 7365 6c66 2c20 6e3d 4e6f  epare(self, n=No
+00002950: 6e65 2c20 2a61 7267 7329 3a0d 0a09 0973  ne, *args):....s
+00002960: 656c 662e 7072 6570 6172 6564 203d 2054  elf.prepared = T
+00002970: 7275 650d 0a09 0974 656d 7073 6361 6c65  rue....tempscale
+00002980: 203d 2073 656c 662e 696e 6974 6961 6c5f   = self.initial_
+00002990: 7363 616c 650d 0a0d 0a09 0969 6620 7365  scale......if se
+000029a0: 6c66 2e73 6f75 7263 655f 6372 6f70 206f  lf.source_crop o
+000029b0: 7220 7365 6c66 2e69 6d61 6765 3a0d 0a09  r self.image:...
+000029c0: 0909 7472 793a 0d0a 0909 0909 7365 6c66  ..try:......self
+000029d0: 2e69 6d61 6765 2e74 6578 7475 7265 2e6d  .image.texture.m
+000029e0: 6167 5f66 696c 7465 7220 3d20 276e 6561  ag_filter = 'nea
+000029f0: 7265 7374 270d 0a09 0909 6578 6365 7074  rest'.....except
+00002a00: 2041 7474 7269 6275 7465 4572 726f 723a   AttributeError:
+00002a10: 0d0a 0909 0909 7061 7373 0d0a 0d0a 0909  ......pass......
+00002a20: 0973 656c 662e 696d 6167 652e 6669 745f  .self.image.fit_
+00002a30: 6d6f 6465 203d 2022 7363 616c 652d 646f  mode = "scale-do
+00002a40: 776e 220d 0a0d 0a09 0909 2320 4361 6c63  wn".......# Calc
+00002a50: 756c 6174 696e 6720 7769 6467 6574 2773  ulating widget's
+00002a60: 2073 697a 6520 6672 6f6d 2061 7661 696c   size from avail
+00002a70: 6162 6c65 2069 6e70 7574 732e 0d0a 0909  able inputs.....
+00002a80: 0969 6620 286e 6f74 2028 7365 6c66 2e77  .if (not (self.w
+00002a90: 6964 7468 202d 2074 656d 7073 6361 6c65  idth - tempscale
+00002aa0: 203e 2031 206f 7220 7365 6c66 2e68 6569   > 1 or self.hei
+00002ab0: 6768 7420 2d20 7465 6d70 7363 616c 6520  ght - tempscale 
+00002ac0: 3e20 3129 206f 7220 7365 6c66 2e73 697a  > 1) or self.siz
+00002ad0: 6564 5f62 795f 696d 6729 3a0d 0a09 0909  ed_by_img):.....
+00002ae0: 0974 7279 3a0d 0a09 0909 0909 7365 6c66  .try:.......self
+00002af0: 2e6f 7269 6769 6e61 6c5f 7369 7a65 203d  .original_size =
+00002b00: 2073 656c 662e 696d 6167 652e 7465 7874   self.image.text
+00002b10: 7572 652e 7369 7a65 0d0a 0909 0909 6578  ure.size......ex
+00002b20: 6365 7074 2041 7474 7269 6275 7465 4572  cept AttributeEr
+00002b30: 726f 723a 0d0a 0909 0909 0923 2049 6620  ror:.......# If 
+00002b40: 616e 696d 6174 696f 6e2c 2074 6578 7475  animation, textu
+00002b50: 7265 206e 6f74 2072 6561 6479 2028 3f29  re not ready (?)
+00002b60: 0d0a 0909 0909 0973 656c 662e 6f72 6967  .......self.orig
+00002b70: 696e 616c 5f73 697a 6520 3d20 7365 6c66  inal_size = self
+00002b80: 2e69 6d61 6765 2e73 697a 650d 0a0d 0a09  .image.size.....
+00002b90: 0909 0969 6620 6e6f 7420 7465 6d70 7363  ...if not tempsc
+00002ba0: 616c 653a 0d0a 0909 0909 0974 656d 7073  ale:.......temps
+00002bb0: 6361 6c65 203d 2031 0d0a 0909 0909 7365  cale = 1......se
+00002bc0: 6c66 2e73 697a 6520 3d20 6c69 7374 286d  lf.size = list(m
+00002bd0: 6170 286c 616d 6264 6120 6e3a 2028 6e20  ap(lambda n: (n 
+00002be0: 2a20 7465 6d70 7363 616c 6529 2c20 7365  * tempscale), se
+00002bf0: 6c66 2e6f 7269 6769 6e61 6c5f 7369 7a65  lf.original_size
+00002c00: 2929 0d0a 0d0a 0909 0909 6966 2073 656c  ))........if sel
+00002c10: 662e 7369 7a65 645f 6279 5f69 6d67 3a0d  f.sized_by_img:.
+00002c20: 0a09 0909 0909 6477 203d 2073 656c 662e  ......dw = self.
+00002c30: 7769 6474 6820 2d20 7365 6c66 2e6c 6173  width - self.las
+00002c40: 745f 7369 7a65 5b30 5d0d 0a09 0909 0909  t_size[0].......
+00002c50: 6468 203d 2073 656c 662e 6865 6967 6874  dh = self.height
+00002c60: 202d 2073 656c 662e 6c61 7374 5f73 697a   - self.last_siz
+00002c70: 655b 315d 0d0a 0909 0909 0973 656c 662e  e[1].......self.
+00002c80: 7069 766f 7420 3d20 2820 2873 656c 662e  pivot = ( (self.
+00002c90: 7069 766f 745f 7820 2d20 6477 202a 2030  pivot_x - dw * 0
+00002ca0: 2e35 292c 2028 7365 6c66 2e70 6976 6f74  .5), (self.pivot
+00002cb0: 5f79 202d 2064 6820 2a20 302e 3529 2029  _y - dh * 0.5) )
+00002cc0: 0d0a 0909 0965 6c73 653a 0d0a 0909 0909  .....else:......
+00002cd0: 7365 6c66 2e6f 7269 6769 6e61 6c5f 7369  self.original_si
+00002ce0: 7a65 203d 2073 656c 662e 7369 7a65 5b3a  ze = self.size[:
+00002cf0: 5d0d 0a09 0909 0969 6620 7465 6d70 7363  ]......if tempsc
+00002d00: 616c 653a 0d0a 0909 0909 0973 656c 662e  ale:.......self.
+00002d10: 7369 7a65 203d 206c 6973 7428 6d61 7028  size = list(map(
+00002d20: 6c61 6d62 6461 206e 3a20 286e 202a 2074  lambda n: (n * t
+00002d30: 656d 7073 6361 6c65 292c 2073 656c 662e  empscale), self.
+00002d40: 7369 7a65 2929 0d0a 0909 656c 7365 3a0d  size))....else:.
+00002d50: 0a09 0909 7365 6c66 2e6f 7269 6769 6e61  ....self.origina
+00002d60: 6c5f 7369 7a65 203d 2073 656c 662e 7369  l_size = self.si
+00002d70: 7a65 5b3a 5d0d 0a09 0909 6966 206e 6f74  ze[:].....if not
+00002d80: 2074 656d 7073 6361 6c65 3a0d 0a09 0909   tempscale:.....
+00002d90: 0974 656d 7073 6361 6c65 203d 2031 0d0a  .tempscale = 1..
+00002da0: 0909 0973 656c 662e 7369 7a65 203d 206c  ...self.size = l
+00002db0: 6973 7428 6d61 7028 6c61 6d62 6461 206e  ist(map(lambda n
+00002dc0: 3a20 286e 202a 2074 656d 7073 6361 6c65  : (n * tempscale
+00002dd0: 292c 2073 656c 662e 7369 7a65 2929 0d0a  ), self.size))..
+00002de0: 0d0a 0909 2320 5365 7474 696e 6720 7468  ....# Setting th
+00002df0: 6520 7769 6467 6574 2773 2072 6174 696f  e widget's ratio
+00002e00: 2e0d 0a09 0969 6620 6e6f 7420 7365 6c66  .....if not self
+00002e10: 2e61 7370 6563 745f 7261 7469 6f3a 0d0a  .aspect_ratio:..
+00002e20: 0909 0969 6620 7365 6c66 2e73 6f75 7263  ...if self.sourc
+00002e30: 655f 6372 6f70 2061 6e64 2073 656c 662e  e_crop and self.
+00002e40: 7369 7a65 645f 6279 5f69 6d67 3a0d 0a09  sized_by_img:...
+00002e50: 0909 0973 656c 662e 7261 7469 6f20 3d20  ...self.ratio = 
+00002e60: 7365 6c66 2e69 6d61 6765 2e69 6d61 6765  self.image.image
+00002e70: 5f72 6174 696f 0d0a 0909 0965 6c73 653a  _ratio.....else:
+00002e80: 0d0a 0909 0909 7365 6c66 2e72 6174 696f  ......self.ratio
+00002e90: 203d 2028 7365 6c66 2e77 6964 7468 202f   = (self.width /
+00002ea0: 2066 6c6f 6174 2873 656c 662e 6865 6967   float(self.heig
+00002eb0: 6874 2929 0d0a 0909 656c 7365 3a0d 0a09  ht))....else:...
+00002ec0: 0909 7365 6c66 2e72 6174 696f 203d 2073  ..self.ratio = s
+00002ed0: 656c 662e 6173 7065 6374 5f72 6174 696f  elf.aspect_ratio
+00002ee0: 0d0a 0d0a 0909 2320 4966 205b 7369 7a65  ......# If [size
+00002ef0: 5d20 6973 206e 6f74 2073 7065 6369 6669  ] is not specifi
+00002f00: 6564 2065 7870 6c69 6369 746c 7920 6279  ed explicitly by
+00002f10: 2074 6865 2075 7365 722c 2061 6e79 2069   the user, any i
+00002f20: 6e70 7574 2076 616c 7565 730d 0a09 0923  nput values....#
+00002f30: 2066 6f72 205b 7069 766f 745d 2061 7265   for [pivot] are
+00002f40: 2077 6974 6868 656c 6420 696e 205b 7465   withheld in [te
+00002f50: 6d70 5f70 6976 5f78 5d20 616e 6420 5b74  mp_piv_x] and [t
+00002f60: 656d 705f 7069 765f 795d 2c20 756e 7469  emp_piv_y], unti
+00002f70: 6c0d 0a09 0923 205b 7369 7a65 5d20 6765  l....# [size] ge
+00002f80: 7473 2069 7473 2076 616c 7565 7320 6672  ts its values fr
+00002f90: 6f6d 205b 696d 6167 655d 2e20 5468 656e  om [image]. Then
+00002fa0: 2c20 5b70 6976 6f74 5d20 6765 7473 2074  , [pivot] gets t
+00002fb0: 6865 2077 6974 6868 656c 640d 0a09 0923  he withheld....#
+00002fc0: 2076 616c 7565 732c 2068 6572 652e 0d0a   values, here...
+00002fd0: 0909 6966 2073 656c 662e 7465 6d70 5f70  ..if self.temp_p
+00002fe0: 6976 5f78 206f 7220 7365 6c66 2e74 656d  iv_x or self.tem
+00002ff0: 705f 7069 765f 793a 0d0a 0909 0973 656c  p_piv_y:.....sel
+00003000: 662e 7069 766f 7420 3d20 7365 6c66 2e74  f.pivot = self.t
+00003010: 656d 705f 7069 765f 782c 2073 656c 662e  emp_piv_x, self.
+00003020: 7465 6d70 5f70 6976 5f79 0d0a 0909 0973  temp_piv_y.....s
+00003030: 656c 662e 7465 6d70 5f70 6976 5f78 203d  elf.temp_piv_x =
+00003040: 2073 656c 662e 7465 6d70 5f70 6976 5f79   self.temp_piv_y
+00003050: 203d 2030 0d0a 0d0a 0909 6966 2073 656c   = 0......if sel
+00003060: 662e 616c 6c6f 775f 726f 7461 626f 783a  f.allow_rotabox:
+00003070: 0d0a 0909 0923 2047 656e 6572 6174 696e  .....# Generatin
+00003080: 6720 6120 756e 6971 7565 206b 6579 2066  g a unique key f
+00003090: 6f72 2065 6163 6820 696e 7374 616e 6365  or each instance
+000030a0: 0d0a 0909 0974 7279 3a0d 0a09 0909 0973  .....try:......s
+000030b0: 656c 662e 7269 6420 3d20 736f 7274 6564  elf.rid = sorted
+000030c0: 2870 6565 7273 2e6b 6579 7328 2929 5b2d  (peers.keys())[-
+000030d0: 315d 202b 2031 0d0a 0909 0965 7863 6570  1] + 1.....excep
+000030e0: 7420 496e 6465 7845 7272 6f72 3a0d 0a09  t IndexError:...
+000030f0: 0909 0970 6173 730d 0a0d 0a09 0909 6966  ...pass.......if
+00003100: 2069 7369 6e73 7461 6e63 6528 7365 6c66   isinstance(self
+00003110: 2e63 7573 746f 6d5f 626f 756e 6473 2c20  .custom_bounds, 
+00003120: 6469 6374 293a 0d0a 0909 0909 7365 6c66  dict):......self
+00003130: 2e63 7572 725f 6b65 7920 3d20 7365 6c66  .curr_key = self
+00003140: 2e63 7572 7265 6e74 5f69 6d61 6765 0d0a  .current_image..
+00003150: 0909 0909 7365 6c66 2e61 6e69 6d20 3d20  ....self.anim = 
+00003160: 5472 7565 0d0a 0909 090d 0a09 0909 6465  True..........de
+00003170: 6669 6e65 5f62 6f75 6e64 7328 7365 6c66  fine_bounds(self
+00003180: 2e63 7573 746f 6d5f 626f 756e 6473 2c20  .custom_bounds, 
+00003190: 7365 6c66 2e6f 7065 6e5f 626f 756e 6473  self.open_bounds
+000031a0: 2c20 7365 6c66 2e73 6567 6d65 6e74 5f6d  , self.segment_m
+000031b0: 6f64 652c 2073 656c 662e 7269 642c 2073  ode, self.rid, s
+000031c0: 656c 662e 7072 655f 6368 6563 6b29 0d0a  elf.pre_check)..
+000031d0: 0909 090d 0a09 0909 6966 2073 656c 662e  ........if self.
+000031e0: 6472 6177 5f62 6f75 6e64 733a 0d0a 0909  draw_bounds:....
+000031f0: 0909 7365 6c66 2e73 6574 5f64 7261 7728  ..self.set_draw(
+00003200: 290d 0a09 0909 0973 656c 662e 6269 6e64  )......self.bind
+00003210: 280d 0a09 0909 0909 6368 696c 6472 656e  (.......children
+00003220: 3d73 656c 662e 7472 6967 6765 725f 6472  =self.trigger_dr
+00003230: 6177 2c0d 0a09 0909 0909 7061 7265 6e74  aw,.......parent
+00003240: 3d73 656c 662e 7472 6967 6765 725f 6472  =self.trigger_dr
+00003250: 6177 2c0d 0a09 0909 0909 706f 733d 7365  aw,.......pos=se
+00003260: 6c66 2e74 7269 6767 6572 5f64 7261 772c  lf.trigger_draw,
+00003270: 0d0a 0909 0909 0970 6f73 5f68 696e 743d  .......pos_hint=
+00003280: 7365 6c66 2e74 7269 6767 6572 5f64 7261  self.trigger_dra
+00003290: 772c 0d0a 0909 0909 0961 6e67 6c65 3d73  w,.......angle=s
+000032a0: 656c 662e 7472 6967 6765 725f 6472 6177  elf.trigger_draw
+000032b0: 2c0d 0a09 0909 0929 0d0a 0d0a 0909 7365  ,......)......se
+000032c0: 6c66 2e74 7269 6767 6572 5f75 7064 6174  lf.trigger_updat
+000032d0: 6528 290d 0a0d 0a09 6465 6620 6765 745f  e().....def get_
+000032e0: 706f 696e 7428 7365 6c66 2c20 706f 6c5f  point(self, pol_
+000032f0: 696e 6465 782c 2070 6f69 6e74 5f69 6e64  index, point_ind
+00003300: 6578 293a 0d0a 0909 2727 2741 6363 6573  ex):....'''Acces
+00003310: 7320 6120 706f 696e 7427 7320 6375 7272  s a point's curr
+00003320: 656e 7420 706f 7369 7469 6f6e 2c20 6261  ent position, ba
+00003330: 7365 6420 6f6e 205b 6375 7374 6f6d 5f62  sed on [custom_b
+00003340: 6f75 6e64 735d 2073 7472 7563 7475 7265  ounds] structure
+00003350: 2e27 2727 0d0a 0909 626f 756e 6473 203d  .'''....bounds =
+00003360: 2070 6565 7273 5b73 656c 662e 7269 645d   peers[self.rid]
+00003370: 5b73 656c 662e 6375 7272 5f6b 6579 5d0d  [self.curr_key].
+00003380: 0a09 0969 6e64 6578 203d 2028 7375 6d28  ...index = (sum(
+00003390: 626f 756e 6473 5b27 706f 6c5f 6c65 6e73  bounds['pol_lens
+000033a0: 275d 5b3a 706f 6c5f 696e 6465 785d 2920  '][:pol_index]) 
+000033b0: 2b20 706f 696e 745f 696e 6465 7829 202a  + point_index) *
+000033c0: 2032 0d0a 0909 7265 7475 726e 206c 6973   2....return lis
+000033d0: 7428 626f 756e 6473 5b27 706f 696e 7473  t(bounds['points
+000033e0: 275d 5b69 6e64 6578 3a69 6e64 6578 202b  '][index:index +
+000033f0: 2032 5d29 0d0a 0d0a 0964 6566 2072 6561   2]).....def rea
+00003400: 645f 626f 756e 6473 2873 656c 662c 2066  d_bounds(self, f
+00003410: 696c 656e 616d 652c 2064 656c 6179 6564  ilename, delayed
+00003420: 3d46 616c 7365 2c20 2a61 7267 7329 3a0d  =False, *args):.
+00003430: 0a09 0927 2727 0d0a 0909 4465 6669 6e65  ...'''....Define
+00003440: 205b 6375 7374 6f6d 5f62 6f75 6e64 735d   [custom_bounds]
+00003450: 2075 7369 6e67 2061 2072 6f74 6162 6f78   using a rotabox
+00003460: 6572 2773 2070 726f 6a65 6374 2066 696c  er's project fil
+00003470: 652e 0d0a 0909 546f 2077 6f72 6b2c 205b  e.....To work, [
+00003480: 7369 7a65 5d20 7368 6f75 6c64 2062 6520  size] should be 
+00003490: 616c 7265 6164 7920 6465 6669 6e65 642e  already defined.
+000034a0: 0d0a 0909 2727 270d 0a09 0970 726f 6a65  ....'''....proje
+000034b0: 6374 203d 204e 6f6e 650d 0a09 0d0a 0909  ct = None.......
+000034c0: 7472 793a 0d0a 0909 0977 6974 6820 6f70  try:.....with op
+000034d0: 656e 2866 696c 656e 616d 652c 2027 7227  en(filename, 'r'
+000034e0: 2c20 656e 636f 6469 6e67 3d22 5554 4638  , encoding="UTF8
+000034f0: 2229 2061 7320 7072 6f6a 3a0d 0a09 0909  ") as proj:.....
+00003500: 0970 726f 6a65 6374 203d 206a 736f 6e2e  .project = json.
+00003510: 6c6f 6164 2870 726f 6a29 0d0a 0909 6578  load(proj)....ex
+00003520: 6365 7074 2028 494f 4572 726f 722c 204b  cept (IOError, K
+00003530: 6579 4572 726f 7229 2061 7320 6572 3a0d  eyError) as er:.
+00003540: 0a09 0909 7072 696e 7428 274f 6e20 7265  ....print('On re
+00003550: 6164 5f62 6f75 6e64 733a 2027 2c20 6572  ad_bounds: ', er
+00003560: 290d 0a09 0909 7265 7475 726e 204e 6f6e  ).....return Non
+00003570: 650d 0a09 090d 0a09 0962 6f75 6e64 7320  e........bounds 
+00003580: 3d20 7b7d 0d0a 0909 6f70 656e 7320 3d20  = {}....opens = 
+00003590: 5b5d 0d0a 0909 666f 7220 662c 2066 7261  []....for f, fra
+000035a0: 6d65 2069 6e20 7072 6f6a 6563 742e 6974  me in project.it
+000035b0: 656d 7328 293a 0d0a 0909 0969 6620 6620  ems():.....if f 
+000035c0: 696e 2028 2769 6d61 6765 272c 2027 7665  in ('image', 've
+000035d0: 7273 696f 6e27 293a 0d0a 0909 0909 636f  rsion'):......co
+000035e0: 6e74 696e 7565 0d0a 0d0a 0909 0970 6f6c  ntinue.......pol
+000035f0: 7320 3d20 5b5d 0d0a 0909 0969 203d 2030  s = [].....i = 0
+00003600: 0d0a 0909 0977 6869 6c65 2069 203c 206c  .....while i < l
+00003610: 656e 2866 7261 6d65 293a 0d0a 0909 0909  en(frame):......
+00003620: 666f 7220 706f 6c20 696e 2066 7261 6d65  for pol in frame
+00003630: 2e76 616c 7565 7328 293a 0d0a 0909 0909  .values():......
+00003640: 0969 6620 706f 6c5b 276e 756d 6265 7227  .if pol['number'
+00003650: 5d20 3d3d 2069 3a0d 0a09 0909 0909 0970  ] == i:........p
+00003660: 6f6c 732e 6170 7065 6e64 2870 6f6c 290d  ols.append(pol).
+00003670: 0a09 0909 0909 0962 7265 616b 0d0a 0909  .......break....
+00003680: 0909 6920 2b3d 2031 0d0a 0909 0962 6f75  ..i += 1.....bou
+00003690: 6e64 735b 665d 203d 205b 5d0d 0a09 0909  nds[f] = [].....
+000036a0: 666f 7220 702c 2070 6f6c 2069 6e20 656e  for p, pol in en
+000036b0: 756d 6572 6174 6528 706f 6c73 293a 0d0a  umerate(pols):..
+000036c0: 0909 0909 7472 793a 0d0a 0909 0909 0969  ....try:.......i
+000036d0: 6620 706f 6c5b 276f 7065 6e27 5d3a 0d0a  f pol['open']:..
+000036e0: 0909 0909 0909 6f70 656e 732e 6170 7065  ......opens.appe
+000036f0: 6e64 2870 290d 0a09 0909 0965 7863 6570  nd(p)......excep
+00003700: 7420 4b65 7945 7272 6f72 3a0d 0a09 0909  t KeyError:.....
+00003710: 0909 7061 7373 0d0a 0909 0909 0d0a 0909  ..pass..........
+00003720: 0909 626f 756e 6473 5b66 5d2e 6170 7065  ..bounds[f].appe
+00003730: 6e64 285b 2872 6f75 6e64 2866 6c6f 6174  nd([(round(float
+00003740: 2870 6f69 6e74 5b30 5d29 202f 2073 656c  (point[0]) / sel
+00003750: 662e 7769 6474 682c 2033 292c 0d0a 0909  f.width, 3),....
+00003760: 0909 0909 0909 0972 6f75 6e64 2866 6c6f  .......round(flo
+00003770: 6174 2870 6f69 6e74 5b31 5d29 202f 2073  at(point[1]) / s
+00003780: 656c 662e 6865 6967 6874 2c20 3329 290d  elf.height, 3)).
+00003790: 0a09 0909 0909 0909 0909 666f 7220 706f  ..........for po
+000037a0: 696e 7420 696e 2070 6f6c 5b27 706f 696e  int in pol['poin
+000037b0: 7473 275d 5d29 0d0a 0d0a 0909 626c 656e  ts']])......blen
+000037c0: 203d 206c 656e 2862 6f75 6e64 7329 0d0a   = len(bounds)..
+000037d0: 0909 6966 2062 6c65 6e3a 0d0a 0909 0969  ..if blen:.....i
+000037e0: 6620 6f70 656e 733a 0d0a 0909 0909 7365  f opens:......se
+000037f0: 6c66 2e6f 7065 6e5f 626f 756e 6473 203d  lf.open_bounds =
+00003800: 206f 7065 6e73 0d0a 0d0a 0909 0969 6620   opens.......if 
+00003810: 626c 656e 203d 3d20 313a 0d0a 0909 0909  blen == 1:......
+00003820: 626f 756e 6473 203d 2062 6f75 6e64 735b  bounds = bounds[
+00003830: 6c69 7374 2862 6f75 6e64 732e 6b65 7973  list(bounds.keys
+00003840: 2829 295b 305d 5d0d 0a0d 0a09 0909 6966  ())[0]].......if
+00003850: 2064 656c 6179 6564 3a0d 0a09 0909 0973   delayed:......s
+00003860: 656c 662e 6375 7374 6f6d 5f62 6f75 6e64  elf.custom_bound
+00003870: 7320 3d20 626f 756e 6473 0d0a 0909 0909  s = bounds......
+00003880: 7265 7475 726e 204e 6f6e 650d 0a0d 0a09  return None.....
+00003890: 0909 7265 7475 726e 2062 6f75 6e64 730d  ..return bounds.
+000038a0: 0a0d 0a09 0972 6574 7572 6e20 7365 6c66  .....return self
+000038b0: 2e63 7573 746f 6d5f 626f 756e 6473 0d0a  .custom_bounds..
+000038c0: 0d0a 0d0a 0964 6566 2075 7064 6174 655f  .....def update_
+000038d0: 7369 7a65 2873 656c 662c 202a 6172 6773  size(self, *args
+000038e0: 293a 0d0a 0909 0d0a 0909 7769 6474 682c  ):........width,
+000038f0: 2068 6569 6768 7420 3d20 7365 6c66 2e73   height = self.s
+00003900: 697a 650d 0a09 0969 6620 726f 756e 6428  ize....if round(
+00003910: 7365 6c66 2e72 6174 696f 2c20 3329 2021  self.ratio, 3) !
+00003920: 3d20 726f 756e 6428 7769 6474 6820 2f20  = round(width / 
+00003930: 666c 6f61 7428 6865 6967 6874 292c 2033  float(height), 3
+00003940: 293a 0d0a 0909 0923 2041 646a 7573 7469  ):.....# Adjusti
+00003950: 6e67 2073 697a 6520 746f 2066 6974 2072  ng size to fit r
+00003960: 6174 696f 0d0a 0909 096c 6173 745f 7369  atio.....last_si
+00003970: 7a65 203d 2073 656c 662e 6c61 7374 5f73  ze = self.last_s
+00003980: 697a 650d 0a09 0909 6966 2061 6273 2877  ize.....if abs(w
+00003990: 6964 7468 202d 206c 6173 745f 7369 7a65  idth - last_size
+000039a0: 5b30 5d29 203e 2061 6273 2868 6569 6768  [0]) > abs(heigh
+000039b0: 7420 2d20 6c61 7374 5f73 697a 655b 315d  t - last_size[1]
+000039c0: 293a 0d0a 0909 0909 7365 6c66 2e73 697a  ):......self.siz
+000039d0: 6520 3d20 5b77 6964 7468 2c20 2866 6c6f  e = [width, (flo
+000039e0: 6174 2877 6964 7468 2920 2f20 7365 6c66  at(width) / self
+000039f0: 2e72 6174 696f 295d 0d0a 0909 0965 6c73  .ratio)].....els
+00003a00: 653a 0d0a 0909 0909 7365 6c66 2e73 697a  e:......self.siz
+00003a10: 6520 3d20 5b28 6865 6967 6874 202a 2073  e = [(height * s
+00003a20: 656c 662e 7261 7469 6f29 2c20 6865 6967  elf.ratio), heig
+00003a30: 6874 5d0d 0a09 0909 0d0a 0909 0969 6620  ht]..........if 
+00003a40: 6c61 7374 5f73 697a 6520 213d 205b 312c  last_size != [1,
+00003a50: 2031 5d3a 0d0a 0909 0909 6477 203d 2073   1]:......dw = s
+00003a60: 656c 662e 7769 6474 6820 2d20 6c61 7374  elf.width - last
+00003a70: 5f73 697a 655b 305d 0d0a 0909 0909 6468  _size[0]......dh
+00003a80: 203d 2073 656c 662e 6865 6967 6874 202d   = self.height -
+00003a90: 206c 6173 745f 7369 7a65 5b31 5d0d 0a09   last_size[1]...
+00003aa0: 0909 0923 204d 6f76 696e 6720 7769 6467  ...# Moving widg
+00003ab0: 6574 2074 6f20 6b65 6570 2070 6976 6f74  et to keep pivot
+00003ac0: 2773 2070 6f73 6974 696f 6e20 7468 6520  's position the 
+00003ad0: 7361 6d65 2c20 746f 206f 7269 6769 6e61  same, to origina
+00003ae0: 7465 2074 6865 2072 6573 697a 696e 6720  te the resizing 
+00003af0: 6672 6f6d 2070 6976 6f74 2e0d 0a09 0909  from pivot......
+00003b00: 0973 656c 662e 7069 766f 7420 3d20 2820  .self.pivot = ( 
+00003b10: 2873 656c 662e 7069 766f 745f 7820 2d20  (self.pivot_x - 
+00003b20: 6477 202a 2030 2e35 292c 2028 7365 6c66  dw * 0.5), (self
+00003b30: 2e70 6976 6f74 5f79 202d 2064 6820 2a20  .pivot_y - dh * 
+00003b40: 302e 3529 2029 0d0a 0d0a 0909 6966 2073  0.5) )......if s
+00003b50: 656c 662e 616c 6c6f 775f 726f 7461 626f  elf.allow_rotabo
+00003b60: 783a 0d0a 0909 0923 2053 6361 6c69 6e67  x:.....# Scaling
+00003b70: 2077 6964 6765 7427 7320 626f 756e 6473   widget's bounds
+00003b80: 0d0a 0909 0969 6620 6e6f 7420 7365 6c66  .....if not self
+00003b90: 2e61 6e69 6d3a 0d0a 0909 0909 7265 7369  .anim:......resi
+00003ba0: 7a65 2873 656c 662e 7769 6474 682c 2073  ze(self.width, s
+00003bb0: 656c 662e 6865 6967 6874 2c20 7365 6c66  elf.height, self
+00003bc0: 2e72 6964 290d 0a09 0909 0975 7064 6174  .rid)......updat
+00003bd0: 655f 626f 756e 6473 2873 656c 662e 706f  e_bounds(self.po
+00003be0: 732c 2072 6164 6961 6e73 2873 656c 662e  s, radians(self.
+00003bf0: 616e 676c 6529 2c20 7365 6c66 2e6f 7269  angle), self.ori
+00003c00: 6769 6e2c 2073 656c 662e 7269 642c 2073  gin, self.rid, s
+00003c10: 656c 662e 6375 7272 5f6b 6579 290d 0a09  elf.curr_key)...
+00003c20: 0909 0973 656c 662e 616c 6c6f 7720 3d20  ...self.allow = 
+00003c30: 300d 0a09 0909 656c 7365 3a0d 0a09 0909  0.....else:.....
+00003c40: 0961 6e69 7265 7369 7a65 2873 656c 662e  .aniresize(self.
+00003c50: 7769 6474 682c 2073 656c 662e 6865 6967  width, self.heig
+00003c60: 6874 2c20 7365 6c66 2e72 6964 290d 0a0d  ht, self.rid)...
+00003c70: 0a09 0969 6620 7365 6c66 2e63 6869 6c64  ...if self.child
+00003c80: 7265 6e3a 0d0a 0909 0973 656c 662e 6368  ren:.....self.ch
+00003c90: 696c 6472 656e 5b30 5d2e 7369 7a65 203d  ildren[0].size =
+00003ca0: 2073 656c 662e 7369 7a65 0d0a 0d0a 0909   self.size......
+00003cb0: 7365 6c66 2e6c 6173 745f 7369 7a65 203d  self.last_size =
+00003cc0: 2073 656c 662e 7369 7a65 5b3a 5d0d 0a09   self.size[:]...
+00003cd0: 0973 656c 662e 7472 6967 6765 725f 7570  .self.trigger_up
+00003ce0: 6461 7465 2829 0d0a 0d0a 0964 6566 2075  date().....def u
+00003cf0: 7064 6174 6528 7365 6c66 2c20 2a61 7267  pdate(self, *arg
+00003d00: 7329 3a0d 0a09 0927 2727 5570 6461 7465  s):....'''Update
+00003d10: 7320 7468 6520 7769 6467 6574 2773 2061  s the widget's a
+00003d20: 6e67 6c65 2c20 706f 696e 7420 6f66 2072  ngle, point of r
+00003d30: 6f74 6174 696f 6e2c 2062 6f75 6e64 7320  otation, bounds 
+00003d40: 616e 6420 6368 696c 6427 730d 0a09 0970  and child's....p
+00003d50: 6f73 6974 696f 6e2e 0d0a 0909 416c 736f  osition.....Also
+00003d60: 2072 756e 7320 7468 6520 5b75 7064 6174   runs the [updat
+00003d70: 655f 7369 7a65 5d20 6d65 7468 6f64 206f  e_size] method o
+00003d80: 6e20 7369 7a65 2063 6861 6e67 6520 616e  n size change an
+00003d90: 6420 7468 6520 5b70 7265 7061 7265 5d0d  d the [prepare].
+00003da0: 0a09 096d 6574 686f 6420 696e 6974 6961  ...method initia
+00003db0: 6c6c 7920 616e 6420 6f6e 2072 6573 6574  lly and on reset
+00003dc0: 2e0d 0a09 0927 2727 0d0a 0909 6966 206e  .....'''....if n
+00003dd0: 6f74 2073 656c 662e 7072 6570 6172 6564  ot self.prepared
+00003de0: 3a0d 0a09 0909 7365 6c66 2e70 7265 7061  :.....self.prepa
+00003df0: 7265 2829 0d0a 0909 0973 656c 662e 7570  re().....self.up
+00003e00: 6461 7465 5f73 697a 6528 290d 0a09 0909  date_size().....
+00003e10: 7265 7475 726e 204e 6f6e 650d 0a0d 0a09  return None.....
+00003e20: 0973 656c 662e 616e 676c 6520 253d 2033  .self.angle %= 3
+00003e30: 3630 0d0a 0909 616e 676c 6520 3d20 7365  60....angle = se
+00003e40: 6c66 2e61 6e67 6c65 0d0a 0909 706f 7320  lf.angle....pos 
+00003e50: 3d20 7365 6c66 2e70 6f73 0d0a 0d0a 0909  = self.pos......
+00003e60: 2320 5570 6461 7469 6e67 2074 6865 2072  # Updating the r
+00003e70: 6f74 6174 696f 6e20 696e 7374 7275 6374  otation instruct
+00003e80: 696f 6e2c 2069 6e20 6361 6e76 6173 2e62  ion, in canvas.b
+00003e90: 6566 6f72 650d 0a09 0973 656c 662e 726f  efore....self.ro
+00003ea0: 7461 7469 6f6e 2e6f 7269 6769 6e20 3d20  tation.origin = 
+00003eb0: 7365 6c66 2e6f 7269 6769 6e0d 0a09 0973  self.origin....s
+00003ec0: 656c 662e 726f 7461 7469 6f6e 2e61 6e67  elf.rotation.ang
+00003ed0: 6c65 203d 2061 6e67 6c65 0d0a 0d0a 0909  le = angle......
+00003ee0: 2320 5570 6461 7469 6e67 2074 6865 2063  # Updating the c
+00003ef0: 6869 6c64 2773 2070 6f73 6974 696f 6e0d  hild's position.
+00003f00: 0a09 0969 6620 7365 6c66 2e63 6869 6c64  ...if self.child
+00003f10: 7265 6e3a 0d0a 0909 0973 656c 662e 6368  ren:.....self.ch
+00003f20: 696c 6472 656e 5b30 5d2e 706f 7320 3d20  ildren[0].pos = 
+00003f30: 706f 730d 0a0d 0a09 096d 6f74 696f 6e20  pos......motion 
+00003f40: 3d20 5b70 6f73 5b30 5d20 2d20 7365 6c66  = [pos[0] - self
+00003f50: 2e6c 6173 745f 706f 735b 305d 2c20 706f  .last_pos[0], po
+00003f60: 735b 315d 202d 2073 656c 662e 6c61 7374  s[1] - self.last
+00003f70: 5f70 6f73 5b31 5d5d 0d0a 0909 6966 2061  _pos[1]]....if a
+00003f80: 6273 286d 6f74 696f 6e5b 305d 2920 3c20  bs(motion[0]) < 
+00003f90: 2e30 3120 616e 6420 6162 7328 6d6f 7469  .01 and abs(moti
+00003fa0: 6f6e 5b31 5d29 203c 2030 2e30 313a 0d0a  on[1]) < 0.01:..
+00003fb0: 0909 096d 6f74 696f 6e20 3d20 5b5d 0d0a  ...motion = []..
+00003fc0: 0909 7365 6c66 2e6c 6173 745f 706f 7320  ..self.last_pos 
+00003fd0: 3d20 706f 735b 3a5d 0d0a 0d0a 0909 616e  = pos[:]......an
+00003fe0: 676c 655f 6469 6666 203d 2061 6e67 6c65  gle_diff = angle
+00003ff0: 202d 2073 656c 662e 6c61 7374 5f61 6e67   - self.last_ang
+00004000: 6c65 0d0a 0909 6966 2061 6273 2861 6e67  le....if abs(ang
+00004010: 6c65 5f64 6966 6629 203c 2030 2e30 313a  le_diff) < 0.01:
+00004020: 0d0a 0909 0961 6e67 6c65 5f64 6966 6620  .....angle_diff 
+00004030: 3d20 300d 0a0d 0a09 0973 656c 662e 6c61  = 0......self.la
+00004040: 7374 5f61 6e67 6c65 203d 2061 6e67 6c65  st_angle = angle
+00004050: 0d0a 0909 6966 206e 6f74 2073 656c 662e  ....if not self.
+00004060: 616c 6c6f 773a 0d0a 0909 0973 656c 662e  allow:.....self.
+00004070: 616c 6c6f 7720 3d20 310d 0a09 0909 7265  allow = 1.....re
+00004080: 7475 726e 204e 6f6e 650d 0a0d 0a09 0969  turn None......i
+00004090: 6620 7365 6c66 2e61 6c6c 6f77 5f72 6f74  f self.allow_rot
+000040a0: 6162 6f78 3a0d 0a09 0909 2320 5570 6461  abox:.....# Upda
+000040b0: 7469 6e67 2074 6865 2063 7573 746f 6d20  ting the custom 
+000040c0: 626f 756e 6473 0d0a 0909 0969 6620 7365  bounds.....if se
+000040d0: 6c66 2e61 6e69 6d3a 0d0a 0909 0909 2320  lf.anim:......# 
+000040e0: 416e 2069 6465 6e74 6963 616c 6c79 206b  An identically k
+000040f0: 6579 6564 2061 746c 6173 2066 696c 6520  eyed atlas file 
+00004100: 6973 2061 7373 756d 6564 2e0d 0a09 0909  is assumed......
+00004110: 0973 656c 662e 6375 7272 5f6b 6579 203d  .self.curr_key =
+00004120: 2073 656c 662e 6375 7272 656e 745f 696d   self.current_im
+00004130: 6167 650d 0a09 0909 0961 6e69 7570 6461  age......aniupda
+00004140: 7465 5f62 6f75 6e64 7328 5472 7565 2c20  te_bounds(True, 
+00004150: 706f 732c 2072 6164 6961 6e73 2861 6e67  pos, radians(ang
+00004160: 6c65 292c 2073 656c 662e 6f72 6967 696e  le), self.origin
+00004170: 2c20 7365 6c66 2e72 6964 2c20 7365 6c66  , self.rid, self
+00004180: 2e63 7572 725f 6b65 7929 0d0a 0909 0909  .curr_key)......
+00004190: 7265 7475 726e 204e 6f6e 650d 0a0d 0a09  return None.....
+000041a0: 0909 6966 206d 6f74 696f 6e20 6f72 2061  ..if motion or a
+000041b0: 6e67 6c65 5f64 6966 663a 0d0a 0909 0909  ngle_diff:......
+000041c0: 7570 6461 7465 5f62 6f75 6e64 7328 6d6f  update_bounds(mo
+000041d0: 7469 6f6e 2c20 7261 6469 616e 7328 616e  tion, radians(an
+000041e0: 676c 655f 6469 6666 292c 2073 656c 662e  gle_diff), self.
+000041f0: 6f72 6967 696e 2c20 7365 6c66 2e72 6964  origin, self.rid
+00004200: 2c20 7365 6c66 2e63 7572 725f 6b65 7929  , self.curr_key)
+00004210: 0d0a 090d 0a0d 0a09 6465 6620 636f 6c6c  ........def coll
+00004220: 6964 655f 706f 696e 7428 7365 6c66 2c20  ide_point(self, 
+00004230: 783d 302c 2079 3d30 293a 0d0a 0909 6966  x=0, y=0):....if
+00004240: 2073 656c 662e 616c 6c6f 775f 726f 7461   self.allow_rota
+00004250: 626f 783a 0d0a 0909 0972 6574 7572 6e20  box:.....return 
+00004260: 706f 696e 745f 696e 5f62 6f75 6e64 7328  point_in_bounds(
+00004270: 782c 2079 2c20 7365 6c66 2e72 6964 2c20  x, y, self.rid, 
+00004280: 6672 616d 653d 7365 6c66 2e63 7572 725f  frame=self.curr_
+00004290: 6b65 7929 0d0a 0909 656c 7365 3a0d 0a09  key)....else:...
+000042a0: 0909 7265 7475 726e 2073 7570 6572 2829  ..return super()
+000042b0: 2e63 6f6c 6c69 6465 5f70 6f69 6e74 2878  .collide_point(x
+000042c0: 2c20 7929 0d0a 0d0a 0964 6566 2063 6f6c  , y).....def col
+000042d0: 6c69 6465 5f77 6964 6765 7428 7365 6c66  lide_widget(self
+000042e0: 2c20 7769 6429 3a0d 0a09 0974 7279 3a0d  , wid):....try:.
+000042f0: 0a09 0909 7472 793a 0d0a 0909 0909 7265  ....try:......re
+00004300: 7475 726e 2063 6f6c 6c69 6465 5f62 6f75  turn collide_bou
+00004310: 6e64 7328 7365 6c66 2e72 6964 2c20 7769  nds(self.rid, wi
+00004320: 642e 7269 642c 2066 7261 6d65 3d73 656c  d.rid, frame=sel
+00004330: 662e 6375 7272 5f6b 6579 2c20 7466 7261  f.curr_key, tfra
+00004340: 6d65 3d77 6964 2e63 7572 725f 6b65 7929  me=wid.curr_key)
+00004350: 0d0a 0909 0965 7863 6570 7420 4174 7472  .....except Attr
+00004360: 6962 7574 6545 7272 6f72 3a0d 0a09 0909  ibuteError:.....
+00004370: 0969 6620 7365 6c66 2e73 6567 6d65 6e74  .if self.segment
+00004380: 5f6d 6f64 653a 0d0a 0909 0909 0972 6574  _mode:.......ret
+00004390: 7572 6e20 636f 6c6c 6964 655f 626f 756e  urn collide_boun
+000043a0: 6473 2873 656c 662e 7269 642c 205b 7769  ds(self.rid, [wi
+000043b0: 642e 782c 2077 6964 2e79 2c20 7769 642e  d.x, wid.y, wid.
+000043c0: 7269 6768 742c 2077 6964 2e74 6f70 5d2c  right, wid.top],
+000043d0: 2066 7261 6d65 3d73 656c 662e 6375 7272   frame=self.curr
+000043e0: 5f6b 6579 290d 0a09 0909 0972 6574 7572  _key)......retur
+000043f0: 6e20 7375 7065 7228 292e 636f 6c6c 6964  n super().collid
+00004400: 655f 7769 6467 6574 2877 6964 290d 0a09  e_widget(wid)...
+00004410: 0965 7863 6570 7420 4b65 7945 7272 6f72  .except KeyError
+00004420: 3a0d 0a09 0909 7265 7475 726e 2046 616c  :.....return Fal
+00004430: 7365 0d0a 0d0a 0964 6566 206f 6e5f 746f  se.....def on_to
+00004440: 7563 685f 646f 776e 2873 656c 662c 2074  uch_down(self, t
+00004450: 6f75 6368 293a 0d0a 0909 782c 2079 203d  ouch):....x, y =
+00004460: 2074 6f75 6368 2e78 2c20 746f 7563 682e   touch.x, touch.
+00004470: 790d 0a0d 0a09 0923 2069 6620 7468 6520  y......# if the 
+00004480: 746f 7563 6820 6973 6e74 206f 6e20 7468  touch isnt on th
+00004490: 6520 7769 6467 6574 2077 6520 646f 206e  e widget we do n
+000044a0: 6f74 6869 6e67 0d0a 0909 6966 206e 6f74  othing....if not
+000044b0: 2073 656c 662e 636f 6c6c 6964 655f 6166   self.collide_af
+000044c0: 7465 725f 6368 696c 6472 656e 3a0d 0a09  ter_children:...
+000044d0: 0909 6966 206e 6f74 2073 656c 662e 636f  ..if not self.co
+000044e0: 6c6c 6964 655f 706f 696e 7428 782c 2079  llide_point(x, y
+000044f0: 293a 0d0a 0909 0909 7265 7475 726e 2046  ):......return F
+00004500: 616c 7365 0d0a 0d0a 0909 2320 6c65 7420  alse......# let 
+00004510: 7468 6520 6368 696c 6420 7769 6467 6574  the child widget
+00004520: 7320 6861 6e64 6c65 2074 6865 2065 7665  s handle the eve
+00004530: 6e74 2069 6620 7468 6579 2077 616e 740d  nt if they want.
+00004540: 0a09 0969 6620 7375 7065 7228 292e 6f6e  ...if super().on
+00004550: 5f74 6f75 6368 5f64 6f77 6e28 746f 7563  _touch_down(touc
+00004560: 6829 3a0d 0a09 0909 2320 656e 7375 7265  h):.....# ensure
+00004570: 2063 6869 6c64 7265 6e20 646f 6e27 7420   children don't 
+00004580: 6861 7665 2074 6f20 646f 2069 7420 7468  have to do it th
+00004590: 656d 7365 6c76 6573 0d0a 0909 0969 6620  emselves.....if 
+000045a0: 276d 756c 7469 746f 7563 685f 7369 6d27  'multitouch_sim'
+000045b0: 2069 6e20 746f 7563 682e 7072 6f66 696c   in touch.profil
+000045c0: 653a 0d0a 0909 0909 746f 7563 682e 6d75  e:......touch.mu
+000045d0: 6c74 6974 6f75 6368 5f73 696d 203d 2054  ltitouch_sim = T
+000045e0: 7275 650d 0a09 0909 0d0a 0909 0973 656c  rue..........sel
+000045f0: 662e 6272 696e 675f 746f 5f66 726f 6e74  f.bring_to_front
+00004600: 2874 6f75 6368 290d 0a09 0909 7265 7475  (touch).....retu
+00004610: 726e 2054 7275 650d 0a0d 0a09 0923 2069  rn True......# i
+00004620: 6620 7765 2064 6f6e 2774 2068 6176 6520  f we don't have 
+00004630: 616e 7920 6163 7469 7665 0d0a 0909 2320  any active....# 
+00004640: 696e 7465 7261 6374 696f 6e20 636f 6e74  interaction cont
+00004650: 726f 6c2c 2074 6865 6e20 646f 6e27 7420  rol, then don't 
+00004660: 6163 6365 7074 2074 6865 2074 6f75 6368  accept the touch
+00004670: 2e0d 0a09 0969 6620 6e6f 7420 2873 656c  .....if not (sel
+00004680: 662e 616c 6c6f 775f 6472 6167 5f78 0d0a  f.allow_drag_x..
+00004690: 0909 0909 6f72 2073 656c 662e 616c 6c6f  ....or self.allo
+000046a0: 775f 6472 6167 5f79 0d0a 0909 0909 6f72  w_drag_y......or
+000046b0: 2073 656c 662e 6d75 6c74 695f 746f 7563   self.multi_touc
+000046c0: 685f 726f 7461 7469 6f6e 0d0a 0909 0909  h_rotation......
+000046d0: 6f72 2073 656c 662e 6d75 6c74 695f 746f  or self.multi_to
+000046e0: 7563 685f 7363 616c 696e 670d 0a09 0909  uch_scaling.....
+000046f0: 096f 7220 7365 6c66 2e73 696e 676c 655f  .or self.single_
+00004700: 746f 7563 685f 726f 7461 7469 6f6e 0d0a  touch_rotation..
+00004710: 0909 0909 6f72 2073 656c 662e 7369 6e67  ....or self.sing
+00004720: 6c65 5f74 6f75 6368 5f73 6361 6c69 6e67  le_touch_scaling
+00004730: 293a 0d0a 0909 0972 6574 7572 6e20 4661  ):.....return Fa
+00004740: 6c73 650d 0a0d 0a09 0969 6620 7365 6c66  lse......if self
+00004750: 2e63 6f6c 6c69 6465 5f61 6674 6572 5f63  .collide_after_c
+00004760: 6869 6c64 7265 6e3a 0d0a 0909 0969 6620  hildren:.....if 
+00004770: 6e6f 7420 7365 6c66 2e63 6f6c 6c69 6465  not self.collide
+00004780: 5f70 6f69 6e74 2878 2c20 7929 3a0d 0a09  _point(x, y):...
+00004790: 0909 0972 6574 7572 6e20 4661 6c73 650d  ...return False.
+000047a0: 0a0d 0a09 0969 6620 276d 756c 7469 746f  .....if 'multito
+000047b0: 7563 685f 7369 6d27 2069 6e20 746f 7563  uch_sim' in touc
+000047c0: 682e 7072 6f66 696c 653a 0d0a 0909 0974  h.profile:.....t
+000047d0: 6f75 6368 2e6d 756c 7469 746f 7563 685f  ouch.multitouch_
+000047e0: 7369 6d20 3d20 5472 7565 0d0a 0d0a 0909  sim = True......
+000047f0: 2320 6772 6162 2074 6865 2074 6f75 6368  # grab the touch
+00004800: 2073 6f20 7765 2067 6574 2061 6c6c 2069   so we get all i
+00004810: 7420 6c61 7465 7220 6d6f 7665 2065 7665  t later move eve
+00004820: 6e74 7320 666f 7220 7375 7265 0d0a 0909  nts for sure....
+00004830: 7365 6c66 2e62 7269 6e67 5f74 6f5f 6672  self.bring_to_fr
+00004840: 6f6e 7428 746f 7563 6829 0d0a 0909 746f  ont(touch)....to
+00004850: 7563 682e 6772 6162 2873 656c 6629 0d0a  uch.grab(self)..
+00004860: 0909 7365 6c66 2e74 6f75 6368 6573 2e61  ..self.touches.a
+00004870: 7070 656e 6428 746f 7563 6829 0d0a 0909  ppend(touch)....
+00004880: 7365 6c66 2e6c 6173 745f 746f 7563 685f  self.last_touch_
+00004890: 706f 735b 746f 7563 685d 203d 2078 2c20  pos[touch] = x, 
+000048a0: 790d 0a09 0972 6574 7572 6e20 5472 7565  y....return True
+000048b0: 0d0a 0d0a 0964 6566 2062 7269 6e67 5f74  .....def bring_t
+000048c0: 6f5f 6672 6f6e 7428 7365 6c66 2c20 746f  o_front(self, to
+000048d0: 7563 6829 3a0d 0a09 0969 6620 7365 6c66  uch):....if self
+000048e0: 2e74 6f75 6368 6564 5f74 6f5f 6672 6f6e  .touched_to_fron
+000048f0: 7420 616e 6420 7365 6c66 2e70 6172 656e  t and self.paren
+00004900: 743a 0d0a 0909 0970 6172 656e 7420 3d20  t:.....parent = 
+00004910: 7365 6c66 2e70 6172 656e 740d 0a09 0909  self.parent.....
+00004920: 6966 2070 6172 656e 742e 6368 696c 6472  if parent.childr
+00004930: 656e 5b30 5d20 6973 2073 656c 663a 0d0a  en[0] is self:..
+00004940: 0909 0909 7265 7475 726e 204e 6f6e 650d  ....return None.
+00004950: 0a09 0909 0d0a 0909 0970 6172 656e 742e  .........parent.
+00004960: 7265 6d6f 7665 5f77 6964 6765 7428 7365  remove_widget(se
+00004970: 6c66 290d 0a09 0909 7061 7265 6e74 2e61  lf).....parent.a
+00004980: 6464 5f77 6964 6765 7428 7365 6c66 290d  dd_widget(self).
+00004990: 0a09 0909 7365 6c66 2e64 6973 7061 7463  ....self.dispatc
+000049a0: 6828 276f 6e5f 746f 7563 6865 645f 746f  h('on_touched_to
+000049b0: 5f66 726f 6e74 272c 2074 6f75 6368 290d  _front', touch).
+000049c0: 0a0d 0a09 6465 6620 6f6e 5f74 6f75 6368  ....def on_touch
+000049d0: 5f6d 6f76 6528 7365 6c66 2c20 746f 7563  _move(self, touc
+000049e0: 6829 3a0d 0a09 0978 2c20 7920 3d20 746f  h):....x, y = to
+000049f0: 7563 682e 782c 2074 6f75 6368 2e79 0d0a  uch.x, touch.y..
+00004a00: 0d0a 0909 2320 6c65 7420 7468 6520 6368  ....# let the ch
+00004a10: 696c 6420 7769 6467 6574 7320 6861 6e64  ild widgets hand
+00004a20: 6c65 2074 6865 2065 7665 6e74 2069 6620  le the event if 
+00004a30: 7468 6579 2077 616e 740d 0a09 0969 6620  they want....if 
+00004a40: 7365 6c66 2e63 6f6c 6c69 6465 5f70 6f69  self.collide_poi
+00004a50: 6e74 2878 2c20 7929 2061 6e64 206e 6f74  nt(x, y) and not
+00004a60: 2074 6f75 6368 2e67 7261 625f 6375 7272   touch.grab_curr
+00004a70: 656e 7420 3d3d 2073 656c 663a 0d0a 0909  ent == self:....
+00004a80: 0969 6620 7375 7065 7228 292e 6f6e 5f74  .if super().on_t
+00004a90: 6f75 6368 5f6d 6f76 6528 746f 7563 6829  ouch_move(touch)
+00004aa0: 3a0d 0a09 0909 0972 6574 7572 6e20 5472  :......return Tr
+00004ab0: 7565 0d0a 0d0a 0909 6966 2074 6f75 6368  ue......if touch
+00004ac0: 2069 6e20 7365 6c66 2e74 6f75 6368 6573   in self.touches
+00004ad0: 2061 6e64 2074 6f75 6368 2e67 7261 625f   and touch.grab_
+00004ae0: 6375 7272 656e 7420 3d3d 2073 656c 663a  current == self:
+00004af0: 0d0a 0909 0969 6620 7365 6c66 2e74 7261  .....if self.tra
+00004b00: 6e73 666f 726d 5f77 6974 685f 746f 7563  nsform_with_touc
+00004b10: 6828 746f 7563 6829 3a0d 0a09 0909 0973  h(touch):......s
+00004b20: 656c 662e 6469 7370 6174 6368 2827 6f6e  elf.dispatch('on
+00004b30: 5f74 7261 6e73 666f 726d 5f77 6974 685f  _transform_with_
+00004b40: 746f 7563 6827 2c20 746f 7563 6829 0d0a  touch', touch)..
+00004b50: 0909 0973 656c 662e 6c61 7374 5f74 6f75  ...self.last_tou
+00004b60: 6368 5f70 6f73 5b74 6f75 6368 5d20 3d20  ch_pos[touch] = 
+00004b70: 782c 2079 0d0a 0d0a 0909 6966 2073 656c  x, y......if sel
+00004b80: 662e 636f 6c6c 6964 655f 706f 696e 7428  f.collide_point(
+00004b90: 782c 2079 293a 0d0a 0909 0972 6574 7572  x, y):.....retur
+00004ba0: 6e20 5472 7565 0d0a 0d0a 0964 6566 2074  n True.....def t
+00004bb0: 7261 6e73 666f 726d 5f77 6974 685f 746f  ransform_with_to
+00004bc0: 7563 6828 7365 6c66 2c20 746f 7563 6829  uch(self, touch)
+00004bd0: 3a0d 0a09 0963 6861 6e67 6564 203d 2046  :....changed = F
+00004be0: 616c 7365 0d0a 0909 746f 7563 6865 7320  alse....touches 
+00004bf0: 3d20 6c65 6e28 7365 6c66 2e74 6f75 6368  = len(self.touch
+00004c00: 6573 290d 0a0d 0a09 0969 6620 2874 6f75  es)......if (tou
+00004c10: 6368 6573 203d 3d20 7365 6c66 2e73 696e  ches == self.sin
+00004c20: 676c 655f 6472 6167 5f74 6f75 6368 2061  gle_drag_touch a
+00004c30: 6e64 2028 7365 6c66 2e61 6c6c 6f77 5f64  nd (self.allow_d
+00004c40: 7261 675f 7820 6f72 2073 656c 662e 616c  rag_x or self.al
+00004c50: 6c6f 775f 6472 6167 5f79 2929 3a0d 0a09  low_drag_y)):...
+00004c60: 0909 6478 203d 2028 746f 7563 682e 7820  ..dx = (touch.x 
+00004c70: 2d20 7365 6c66 2e6c 6173 745f 746f 7563  - self.last_touc
+00004c80: 685f 706f 735b 746f 7563 685d 5b30 5d29  h_pos[touch][0])
+00004c90: 202a 2073 656c 662e 616c 6c6f 775f 6472   * self.allow_dr
+00004ca0: 6167 5f78 0d0a 0909 0964 7920 3d20 2874  ag_x.....dy = (t
+00004cb0: 6f75 6368 2e79 202d 2073 656c 662e 6c61  ouch.y - self.la
+00004cc0: 7374 5f74 6f75 6368 5f70 6f73 5b74 6f75  st_touch_pos[tou
+00004cd0: 6368 5d5b 315d 2920 2a20 7365 6c66 2e61  ch][1]) * self.a
+00004ce0: 6c6c 6f77 5f64 7261 675f 790d 0a09 0909  llow_drag_y.....
+00004cf0: 0d0a 0909 0973 656c 662e 7820 2b3d 2066  .....self.x += f
+00004d00: 6c6f 6174 2864 7829 202f 2073 656c 662e  loat(dx) / self.
+00004d10: 7369 6e67 6c65 5f64 7261 675f 746f 7563  single_drag_touc
+00004d20: 680d 0a09 0909 7365 6c66 2e79 202b 3d20  h.....self.y += 
+00004d30: 666c 6f61 7428 6479 2920 2f20 7365 6c66  float(dy) / self
+00004d40: 2e73 696e 676c 655f 6472 6167 5f74 6f75  .single_drag_tou
+00004d50: 6368 0d0a 0909 0963 6861 6e67 6564 203d  ch.....changed =
+00004d60: 2054 7275 650d 0a0d 0a09 0969 6620 2874   True......if (t
+00004d70: 6f75 6368 6573 203d 3d20 7365 6c66 2e73  ouches == self.s
+00004d80: 696e 676c 655f 7472 616e 735f 746f 7563  ingle_trans_touc
+00004d90: 6820 616e 6420 2873 656c 662e 7369 6e67  h and (self.sing
+00004da0: 6c65 5f74 6f75 6368 5f72 6f74 6174 696f  le_touch_rotatio
+00004db0: 6e20 6f72 2073 656c 662e 7369 6e67 6c65  n or self.single
+00004dc0: 5f74 6f75 6368 5f73 6361 6c69 6e67 2929  _touch_scaling))
+00004dd0: 3a0d 0a09 0909 616e 6368 6f72 203d 2073  :.....anchor = s
+00004de0: 656c 662e 7069 766f 740d 0a09 0909 6f6c  elf.pivot.....ol
+00004df0: 645f 6c69 6e65 203d 2056 6563 746f 7228  d_line = Vector(
+00004e00: 2a74 6f75 6368 2e70 706f 7329 202d 2061  *touch.ppos) - a
+00004e10: 6e63 686f 720d 0a09 0909 6e65 775f 6c69  nchor.....new_li
+00004e20: 6e65 203d 2056 6563 746f 7228 2a74 6f75  ne = Vector(*tou
+00004e30: 6368 2e70 6f73 2920 2d20 616e 6368 6f72  ch.pos) - anchor
+00004e40: 0d0a 0909 0969 6620 6e6f 7420 6f6c 645f  .....if not old_
+00004e50: 6c69 6e65 2e6c 656e 6774 6828 293a 0d0a  line.length():..
+00004e60: 0909 0909 7265 7475 726e 2063 6861 6e67  ....return chang
+00004e70: 6564 0d0a 0909 090d 0a09 0909 6966 2073  ed..........if s
+00004e80: 656c 662e 7369 6e67 6c65 5f74 6f75 6368  elf.single_touch
+00004e90: 5f72 6f74 6174 696f 6e3a 0d0a 0909 0909  _rotation:......
+00004ea0: 616e 676c 6520 3d20 6e65 775f 6c69 6e65  angle = new_line
+00004eb0: 2e61 6e67 6c65 286f 6c64 5f6c 696e 6529  .angle(old_line)
+00004ec0: 0d0a 0909 0909 7365 6c66 2e61 6e67 6c65  ......self.angle
+00004ed0: 202b 3d20 616e 676c 650d 0a0d 0a09 0909   += angle.......
+00004ee0: 6966 2073 656c 662e 7369 6e67 6c65 5f74  if self.single_t
+00004ef0: 6f75 6368 5f73 6361 6c69 6e67 3a0d 0a09  ouch_scaling:...
+00004f00: 0909 095f 7363 616c 6520 3d20 6e65 775f  ..._scale = new_
+00004f10: 6c69 6e65 2e6c 656e 6774 6828 2920 2f20  line.length() / 
+00004f20: 6f6c 645f 6c69 6e65 2e6c 656e 6774 6828  old_line.length(
+00004f30: 290d 0a09 0909 0973 656c 662e 7363 616c  )......self.scal
+00004f40: 6520 2a3d 205f 7363 616c 650d 0a09 0909  e *= _scale.....
+00004f50: 0d0a 0909 0963 6861 6e67 6564 203d 2054  .....changed = T
+00004f60: 7275 650d 0a0d 0a09 0969 6620 746f 7563  rue......if touc
+00004f70: 6865 7320 3d3d 2031 3a0d 0a09 0909 7265  hes == 1:.....re
+00004f80: 7475 726e 2063 6861 6e67 6564 0d0a 0d0a  turn changed....
+00004f90: 0909 2320 7765 2068 6176 6520 6d6f 7265  ..# we have more
+00004fa0: 2074 6861 6e20 6f6e 6520 746f 7563 682e   than one touch.
+00004fb0: 2e2e 206c 6973 7420 6f66 206c 6173 7420  .. list of last 
+00004fc0: 6b6e 6f77 6e20 706f 730d 0a09 0970 6f69  known pos....poi
+00004fd0: 6e74 7320 3d20 5b56 6563 746f 7228 7365  nts = [Vector(se
+00004fe0: 6c66 2e6c 6173 745f 746f 7563 685f 706f  lf.last_touch_po
+00004ff0: 735b 745d 2920 666f 7220 7420 696e 2073  s[t]) for t in s
+00005000: 656c 662e 746f 7563 6865 7320 6966 2074  elf.touches if t
+00005010: 2069 7320 6e6f 7420 746f 7563 685d 0d0a   is not touch]..
+00005020: 0909 706f 696e 7473 2e61 7070 656e 6428  ..points.append(
+00005030: 5665 6374 6f72 2874 6f75 6368 2e70 6f73  Vector(touch.pos
+00005040: 2929 0d0a 0d0a 0909 2320 7765 206f 6e6c  ))......# we onl
+00005050: 7920 7761 6e74 2074 6f20 7472 616e 7366  y want to transf
+00005060: 6f72 6d20 6966 2074 6865 2074 6f75 6368  orm if the touch
+00005070: 2069 7320 7061 7274 206f 6620 7468 6520   is part of the 
+00005080: 7477 6f20 746f 7563 6865 730d 0a09 0923  two touches....#
+00005090: 2066 6172 7468 6573 7420 6170 6172 7421   farthest apart!
+000050a0: 2053 6f20 6669 7273 7420 7765 2066 696e   So first we fin
+000050b0: 6420 616e 6368 6f72 2c20 7468 6520 706f  d anchor, the po
+000050c0: 696e 7420 746f 2074 7261 6e73 666f 726d  int to transform
+000050d0: 0d0a 0909 2320 6172 6f75 6e64 2061 7320  ....# around as 
+000050e0: 616e 6f74 6865 7220 746f 7563 6820 6661  another touch fa
+000050f0: 7274 6865 7374 2061 7761 7920 6672 6f6d  rthest away from
+00005100: 2063 7572 7265 6e74 2074 6f75 6368 2773   current touch's
+00005110: 2070 6f73 0d0a 0909 616e 6368 6f72 203d   pos....anchor =
+00005120: 206d 6178 2870 6f69 6e74 735b 3a2d 315d   max(points[:-1]
+00005130: 2c20 6b65 793d 6c61 6d62 6461 2070 3a20  , key=lambda p: 
+00005140: 702e 6469 7374 616e 6365 2874 6f75 6368  p.distance(touch
+00005150: 2e70 6f73 2929 0d0a 0d0a 0909 7365 6c66  .pos))......self
+00005160: 2e6f 7269 6769 6e20 3d20 616e 6368 6f72  .origin = anchor
+00005170: 0d0a 0d0a 0909 2320 6e6f 7720 7765 2066  ......# now we f
+00005180: 696e 6420 7468 6520 746f 7563 6820 6661  ind the touch fa
+00005190: 7274 6865 7374 2061 7761 7920 6672 6f6d  rthest away from
+000051a0: 2061 6e63 686f 722c 2069 6620 6974 7320   anchor, if its 
+000051b0: 6e6f 7420 7468 650d 0a09 0923 2073 616d  not the....# sam
+000051c0: 6520 6173 2074 6f75 6368 2e20 546f 7563  e as touch. Touc
+000051d0: 6820 6973 206e 6f74 206f 6e65 206f 6620  h is not one of 
+000051e0: 7468 6520 7477 6f20 746f 7563 6865 7320  the two touches 
+000051f0: 7573 6564 2074 6f20 7472 616e 7366 6f72  used to transfor
+00005200: 6d0d 0a09 0966 6172 7468 6573 7420 3d20  m....farthest = 
+00005210: 6d61 7828 706f 696e 7473 2c20 6b65 793d  max(points, key=
+00005220: 616e 6368 6f72 2e64 6973 7461 6e63 6529  anchor.distance)
+00005230: 0d0a 0909 6966 2066 6172 7468 6573 7420  ....if farthest 
+00005240: 6973 206e 6f74 2070 6f69 6e74 735b 2d31  is not points[-1
+00005250: 5d3a 0d0a 0909 0972 6574 7572 6e20 6368  ]:.....return ch
+00005260: 616e 6765 640d 0a0d 0a09 0923 206f 6b2c  anged......# ok,
+00005270: 2073 6f20 7765 2068 6176 6520 746f 7563   so we have touc
+00005280: 682c 2061 6e64 2061 6e63 686f 722c 2073  h, and anchor, s
+00005290: 6f20 7765 2063 616e 2061 6374 7561 6c6c  o we can actuall
+000052a0: 7920 636f 6d70 7574 6520 7468 6520 7472  y compute the tr
+000052b0: 616e 7366 6f72 6d61 7469 6f6e 0d0a 0909  ansformation....
+000052c0: 6f6c 645f 6c69 6e65 203d 2056 6563 746f  old_line = Vecto
+000052d0: 7228 2a74 6f75 6368 2e70 706f 7329 202d  r(*touch.ppos) -
+000052e0: 2061 6e63 686f 720d 0a09 096e 6577 5f6c   anchor....new_l
+000052f0: 696e 6520 3d20 5665 6374 6f72 282a 746f  ine = Vector(*to
+00005300: 7563 682e 706f 7329 202d 2061 6e63 686f  uch.pos) - ancho
+00005310: 720d 0a09 0969 6620 6e6f 7420 6f6c 645f  r....if not old_
+00005320: 6c69 6e65 2e6c 656e 6774 6828 293a 0d0a  line.length():..
+00005330: 0909 0972 6574 7572 6e20 6368 616e 6765  ...return change
+00005340: 640d 0a0d 0a09 0961 6e67 6c65 203d 206e  d......angle = n
+00005350: 6577 5f6c 696e 652e 616e 676c 6528 6f6c  ew_line.angle(ol
+00005360: 645f 6c69 6e65 2920 2a20 7365 6c66 2e6d  d_line) * self.m
+00005370: 756c 7469 5f74 6f75 6368 5f72 6f74 6174  ulti_touch_rotat
+00005380: 696f 6e0d 0a09 0973 656c 662e 616e 676c  ion....self.angl
+00005390: 6520 2b3d 2061 6e67 6c65 0d0a 0d0a 0909  e += angle......
+000053a0: 6966 2073 656c 662e 6d75 6c74 695f 746f  if self.multi_to
+000053b0: 7563 685f 7363 616c 696e 673a 0d0a 0909  uch_scaling:....
+000053c0: 095f 7363 616c 6520 3d20 6e65 775f 6c69  ._scale = new_li
+000053d0: 6e65 2e6c 656e 6774 6828 2920 2f20 6f6c  ne.length() / ol
+000053e0: 645f 6c69 6e65 2e6c 656e 6774 6828 290d  d_line.length().
+000053f0: 0a09 0909 7365 6c66 2e73 6361 6c65 202a  ....self.scale *
+00005400: 3d20 5f73 6361 6c65 0d0a 0909 0963 6861  = _scale.....cha
+00005410: 6e67 6564 203d 2054 7275 650d 0a09 090d  nged = True.....
+00005420: 0a09 0972 6574 7572 6e20 6368 616e 6765  ...return change
+00005430: 640d 0a0d 0a09 6465 6620 6f6e 5f74 6f75  d.....def on_tou
+00005440: 6368 5f75 7028 7365 6c66 2c20 746f 7563  ch_up(self, touc
+00005450: 6829 3a0d 0a09 0923 2069 6620 7468 6520  h):....# if the 
+00005460: 746f 7563 6820 6973 6e74 206f 6e20 7468  touch isnt on th
+00005470: 6520 7769 6467 6574 2077 6520 646f 206e  e widget we do n
+00005480: 6f74 6869 6e67 2c20 6a75 7374 2074 7279  othing, just try
+00005490: 2063 6869 6c64 7265 6e0d 0a09 0969 6620   children....if 
+000054a0: 6e6f 7420 746f 7563 682e 6772 6162 5f63  not touch.grab_c
+000054b0: 7572 7265 6e74 203d 3d20 7365 6c66 3a0d  urrent == self:.
+000054c0: 0a09 0909 6966 2073 7570 6572 2829 2e6f  ....if super().o
+000054d0: 6e5f 746f 7563 685f 7570 2874 6f75 6368  n_touch_up(touch
+000054e0: 293a 0d0a 0909 0909 7265 7475 726e 2054  ):......return T
+000054f0: 7275 650d 0a0d 0a09 0923 2072 656d 6f76  rue......# remov
+00005500: 6520 6974 2066 726f 6d20 6f75 7220 7361  e it from our sa
+00005510: 7665 6420 746f 7563 6865 730d 0a09 0969  ved touches....i
+00005520: 6620 746f 7563 6820 696e 2073 656c 662e  f touch in self.
+00005530: 746f 7563 6865 7320 616e 6420 746f 7563  touches and touc
+00005540: 682e 6772 6162 5f73 7461 7465 3a0d 0a09  h.grab_state:...
+00005550: 0909 746f 7563 682e 756e 6772 6162 2873  ..touch.ungrab(s
+00005560: 656c 6629 0d0a 0909 0964 656c 2073 656c  elf).....del sel
+00005570: 662e 6c61 7374 5f74 6f75 6368 5f70 6f73  f.last_touch_pos
+00005580: 5b74 6f75 6368 5d0d 0a09 0909 7365 6c66  [touch].....self
+00005590: 2e74 6f75 6368 6573 2e72 656d 6f76 6528  .touches.remove(
+000055a0: 746f 7563 6829 0d0a 0d0a 0909 2320 7374  touch)......# st
+000055b0: 6f70 2070 726f 7061 6761 7469 6e67 2069  op propagating i
+000055c0: 6620 6974 7320 7769 7468 696e 206f 7572  f its within our
+000055d0: 2062 6f75 6e64 730d 0a09 0969 6620 7365   bounds....if se
+000055e0: 6c66 2e63 6f6c 6c69 6465 5f70 6f69 6e74  lf.collide_point
+000055f0: 282a 746f 7563 682e 706f 7329 3a0d 0a09  (*touch.pos):...
+00005600: 0909 7265 7475 726e 2054 7275 650d 0a0d  ..return True...
+00005610: 0a09 6465 6620 7365 745f 6472 6177 2873  ..def set_draw(s
+00005620: 656c 662c 202a 6172 6773 293a 0d0a 0909  elf, *args):....
+00005630: 2727 2753 6574 7469 6e67 2075 7020 6361  '''Setting up ca
+00005640: 6e76 6173 2066 6f72 2074 6573 742d 6472  nvas for test-dr
+00005650: 6177 696e 6720 7468 6520 626f 756e 6473  awing the bounds
+00005660: 2e27 2727 0d0a 0909 7365 6c66 2e72 6573  .'''....self.res
+00005670: 6574 5f64 7261 775f 626f 756e 6473 2829  et_draw_bounds()
+00005680: 0d0a 0909 0d0a 0909 6966 2073 656c 662e  ........if self.
+00005690: 616e 696d 3a0d 0a09 0909 706f 6c73 203d  anim:.....pols =
+000056a0: 206d 6178 285b 6c65 6e28 6672 616d 6529   max([len(frame)
+000056b0: 2066 6f72 2066 7261 6d65 2069 6e20 7365   for frame in se
+000056c0: 6c66 2e63 7573 746f 6d5f 626f 756e 6473  lf.custom_bounds
+000056d0: 2e76 616c 7565 7328 295d 290d 0a09 0909  .values()]).....
+000056e0: 0d0a 0909 096c 656e 6774 6820 3d20 6d61  .....length = ma
+000056f0: 7828 5b6c 656e 2870 6f6c 2920 666f 7220  x([len(pol) for 
+00005700: 706f 6c20 696e 2073 656c 662e 6375 7374  pol in self.cust
+00005710: 6f6d 5f62 6f75 6e64 732e 7661 6c75 6573  om_bounds.values
+00005720: 2829 5d29 0d0a 0909 656c 7365 3a0d 0a09  ()])....else:...
+00005730: 0909 706f 6c73 203d 206c 656e 2873 656c  ..pols = len(sel
+00005740: 662e 6375 7374 6f6d 5f62 6f75 6e64 7329  f.custom_bounds)
+00005750: 0d0a 0909 096c 656e 6774 6820 3d20 7065  .....length = pe
+00005760: 6572 735b 7365 6c66 2e72 6964 5d5b 7365  ers[self.rid][se
+00005770: 6c66 2e63 7572 725f 6b65 795d 5b27 6c65  lf.curr_key]['le
+00005780: 6e67 7468 275d 0d0a 0d0a 0909 666f 7220  ngth']......for 
+00005790: 6920 696e 2072 616e 6765 2870 6f6c 7329  i in range(pols)
+000057a0: 3a0d 0a09 0909 6966 2069 206e 6f74 2069  :.....if i not i
+000057b0: 6e20 7365 6c66 2e6f 7065 6e5f 626f 756e  n self.open_boun
+000057c0: 6473 206f 7220 6e6f 7420 7365 6c66 2e73  ds or not self.s
+000057d0: 6567 6d65 6e74 5f6d 6f64 653a 0d0a 0909  egment_mode:....
+000057e0: 0909 7365 6c66 2e64 7261 775f 6c69 6e65  ..self.draw_line
+000057f0: 732e 6170 7065 6e64 284c 696e 6528 636c  s.append(Line(cl
+00005800: 6f73 653d 5472 7565 2c20 6461 7368 5f6f  ose=True, dash_o
+00005810: 6666 7365 743d 332c 2064 6173 685f 6c65  ffset=3, dash_le
+00005820: 6e67 7468 3d35 2929 0d0a 0909 0965 6c73  ngth=5)).....els
+00005830: 653a 0d0a 0909 0909 7365 6c66 2e64 7261  e:......self.dra
+00005840: 775f 6c69 6e65 732e 6170 7065 6e64 284c  w_lines.append(L
+00005850: 696e 6528 636c 6f73 653d 4661 6c73 652c  ine(close=False,
+00005860: 2064 6173 685f 6f66 6673 6574 3d33 2c20   dash_offset=3, 
+00005870: 6461 7368 5f6c 656e 6774 683d 3529 290d  dash_length=5)).
+00005880: 0a0d 0a09 0973 656c 662e 6361 6e76 6173  .....self.canvas
+00005890: 2e61 6674 6572 2e61 6464 2873 656c 662e  .after.add(self.
+000058a0: 6472 6177 5f63 6f6c 6f72 290d 0a09 0966  draw_color)....f
+000058b0: 6f72 206c 696e 6520 696e 2073 656c 662e  or line in self.
+000058c0: 6472 6177 5f6c 696e 6573 3a0d 0a09 0909  draw_lines:.....
+000058d0: 7365 6c66 2e63 616e 7661 732e 6166 7465  self.canvas.afte
+000058e0: 722e 6164 6428 6c69 6e65 290d 0a0d 0a09  r.add(line).....
+000058f0: 0923 2053 6563 7572 696e 6720 6472 6177  .# Securing draw
+00005900: 206f 6e20 6120 7374 6174 696f 6e61 7279   on a stationary
+00005910: 2077 6964 6765 742e 0d0a 0909 7365 6c66   widget.....self
+00005920: 2e78 202b 3d20 302e 3030 310d 0a09 0973  .x += 0.001....s
+00005930: 656c 662e 7472 6967 6765 725f 6472 6177  elf.trigger_draw
+00005940: 2829 0d0a 0d0a 0964 6566 2064 7261 7728  ().....def draw(
+00005950: 7365 6c66 2c20 2a61 7267 7329 3a0d 0a09  self, *args):...
+00005960: 0927 2727 2049 6620 5b64 7261 775f 626f  .''' If [draw_bo
+00005970: 756e 6473 5d20 6973 2054 7275 652c 2076  unds] is True, v
+00005980: 6973 7561 6c69 7365 7320 7468 6520 7769  isualises the wi
+00005990: 6467 6574 2773 2062 6f75 6e64 732e 2046  dget's bounds. F
+000059a0: 6f72 2074 6573 7469 6e67 2e0d 0a09 0927  or testing.....'
+000059b0: 2727 200d 0a09 0969 6620 6e6f 7420 7365  '' ....if not se
+000059c0: 6c66 2e70 7265 7061 7265 643a 0d0a 0909  lf.prepared:....
+000059d0: 0972 6574 7572 6e20 4e6f 6e65 0d0a 0909  .return None....
+000059e0: 0d0a 0909 7472 793a 0d0a 0909 0962 6f75  ....try:.....bou
+000059f0: 6e64 7320 3d20 7065 6572 735b 7365 6c66  nds = peers[self
+00005a00: 2e72 6964 5d5b 7365 6c66 2e63 7572 725f  .rid][self.curr_
+00005a10: 6b65 795d 0d0a 0909 6578 6365 7074 204b  key]....except K
+00005a20: 6579 4572 726f 723a 0d0a 0909 0972 6574  eyError:.....ret
+00005a30: 7572 6e20 4e6f 6e65 0d0a 0d0a 0909 7374  urn None......st
+00005a40: 6172 7420 3d20 300d 0a09 0966 6f72 2069  art = 0....for i
+00005a50: 2c20 6c65 6e67 2069 6e20 656e 756d 6572  , leng in enumer
+00005a60: 6174 6528 626f 756e 6473 5b27 706f 6c5f  ate(bounds['pol_
+00005a70: 6c65 6e73 275d 293a 0d0a 0909 0973 656c  lens']):.....sel
+00005a80: 662e 6472 6177 5f6c 696e 6573 5b69 5d2e  f.draw_lines[i].
+00005a90: 706f 696e 7473 203d 205b 626f 756e 6473  points = [bounds
+00005aa0: 5b27 706f 696e 7473 275d 5b6a 5d20 666f  ['points'][j] fo
+00005ab0: 7220 6a20 696e 2072 616e 6765 2873 7461  r j in range(sta
+00005ac0: 7274 2c20 7374 6172 7420 2b20 6c65 6e67  rt, start + leng
+00005ad0: 202a 2032 295d 0d0a 0909 0973 7461 7274   * 2)].....start
+00005ae0: 202b 3d20 6c65 6e67 202a 2032 0d0a 0d0a   += leng * 2....
+00005af0: 0d0a 0964 6566 2067 6574 5f73 697a 655f  ...def get_size_
+00005b00: 6869 6e74 5f78 2873 656c 6629 3a0d 0a09  hint_x(self):...
+00005b10: 0923 204c 6f63 6b69 6e67 2073 697a 655f  .# Locking size_
+00005b20: 6869 6e74 2070 726f 7065 7274 7920 746f  hint property to
+00005b30: 204e 6f6e 652c 204e 6f6e 652c 0d0a 0909   None, None,....
+00005b40: 2320 696e 206f 7264 6572 2074 6f20 6b65  # in order to ke
+00005b50: 6570 2069 6e74 656e 6465 6420 6173 7065  ep intended aspe
+00005b60: 6374 2072 6174 696f 2028 6372 6974 6963  ct ratio (critic
+00005b70: 616c 2066 6f72 2063 7573 746f 6d20 626f  al for custom bo
+00005b80: 756e 6473 292e 0d0a 0909 7265 7475 726e  unds).....return
+00005b90: 204e 6f6e 650d 0a0d 0a09 6465 6620 7365   None.....def se
+00005ba0: 745f 7369 7a65 5f68 696e 745f 7828 7365  t_size_hint_x(se
+00005bb0: 6c66 2c20 7661 6c75 6529 3a0d 0a09 0972  lf, value):....r
+00005bc0: 6169 7365 2045 7863 6570 7469 6f6e 2822  aise Exception("
+00005bd0: 476f 526f 7461 626f 7820 6361 6e27 7420  GoRotabox can't 
+00005be0: 7573 6520 7369 7a65 5f68 696e 742e 2229  use size_hint.")
+00005bf0: 0d0a 090d 0a09 7369 7a65 5f68 696e 745f  ......size_hint_
+00005c00: 7820 3d20 416c 6961 7350 726f 7065 7274  x = AliasPropert
+00005c10: 7928 6765 745f 7369 7a65 5f68 696e 745f  y(get_size_hint_
+00005c20: 782c 2073 6574 5f73 697a 655f 6869 6e74  x, set_size_hint
+00005c30: 5f78 290d 0a0d 0a0d 0a09 6465 6620 6765  _x).......def ge
+00005c40: 745f 7369 7a65 5f68 696e 745f 7928 7365  t_size_hint_y(se
+00005c50: 6c66 293a 0d0a 0909 7265 7475 726e 204e  lf):....return N
+00005c60: 6f6e 650d 0a0d 0a09 6465 6620 7365 745f  one.....def set_
+00005c70: 7369 7a65 5f68 696e 745f 7928 7365 6c66  size_hint_y(self
+00005c80: 2c20 7661 6c75 6529 3a0d 0a09 0972 6169  , value):....rai
+00005c90: 7365 2045 7863 6570 7469 6f6e 2822 476f  se Exception("Go
+00005ca0: 526f 7461 626f 7820 6361 6e27 7420 7573  Rotabox can't us
+00005cb0: 6520 7369 7a65 5f68 696e 742e 2229 0d0a  e size_hint.")..
+00005cc0: 0d0a 0973 697a 655f 6869 6e74 5f79 203d  ...size_hint_y =
+00005cd0: 2041 6c69 6173 5072 6f70 6572 7479 2867   AliasProperty(g
+00005ce0: 6574 5f73 697a 655f 6869 6e74 5f79 2c20  et_size_hint_y, 
+00005cf0: 7365 745f 7369 7a65 5f68 696e 745f 7929  set_size_hint_y)
+00005d00: 0d0a 0973 697a 655f 6869 6e74 203d 2052  ...size_hint = R
+00005d10: 6566 6572 656e 6365 4c69 7374 5072 6f70  eferenceListProp
+00005d20: 6572 7479 2873 697a 655f 6869 6e74 5f78  erty(size_hint_x
+00005d30: 2c20 7369 7a65 5f68 696e 745f 7929 0d0a  , size_hint_y)..
+00005d40: 0d0a 0d0a 096f 7269 6769 6e61 6c5f 7369  .....original_si
+00005d50: 7a65 203d 204c 6973 7450 726f 7065 7274  ze = ListPropert
+00005d60: 7928 5b31 2c20 315d 290d 0a09 2222 220d  y([1, 1])...""".
+00005d70: 0a09 5573 6564 2066 6f72 2063 616c 6375  ..Used for calcu
+00005d80: 6c61 7469 6e67 2074 6865 2077 6964 6765  lating the widge
+00005d90: 7427 7320 7363 616c 652e 2049 7427 7320  t's scale. It's 
+00005da0: 7468 6520 7573 6572 2773 2069 6e70 7574  the user's input
+00005db0: 2073 697a 650d 0a09 6f72 2074 6865 205b   size...or the [
+00005dc0: 7465 7874 7572 655f 7369 7a65 5d20 6f66  texture_size] of
+00005dd0: 2074 6865 2077 6964 6765 7427 7320 5b69   the widget's [i
+00005de0: 6d61 6765 5d2e 0d0a 0922 2222 0d0a 0d0a  mage]...."""....
+00005df0: 0970 6976 6f74 5f62 6f6e 6420 3d20 4c69  .pivot_bond = Li
+00005e00: 7374 5072 6f70 6572 7479 285b 2e35 2c20  stProperty([.5, 
+00005e10: 2e35 5d29 0d0a 0922 2222 0d0a 0941 2066  .5])..."""...A f
+00005e20: 7261 6374 696f 6e61 6c20 7661 6c75 6520  ractional value 
+00005e30: 7468 6174 206b 6565 7073 205b 7069 766f  that keeps [pivo
+00005e40: 745d 2072 656c 6174 6976 6520 746f 2074  t] relative to t
+00005e50: 6865 2077 6964 6765 7427 7320 7369 7a65  he widget's size
+00005e60: 0d0a 0961 6e64 2070 6f73 6974 696f 6e2e  ...and position.
+00005e70: 205b 6f72 6967 696e 5d20 7365 7473 2061   [origin] sets a
+00005e80: 6e64 2063 6861 6e67 6573 2069 742e 0d0a  nd changes it...
+00005e90: 0922 2222 0d0a 0d0a 0961 6c6c 6f77 203d  .""".....allow =
+00005ea0: 2042 6f6f 6c65 616e 5072 6f70 6572 7479   BooleanProperty
+00005eb0: 2831 290d 0a09 2222 2220 5377 6974 6368  (1)...""" Switch
+00005ec0: 2074 6f20 7375 7370 656e 6420 626f 756e   to suspend boun
+00005ed0: 6473 2720 7570 6461 7465 2077 6869 6c65  ds' update while
+00005ee0: 2072 6570 6f73 6974 696f 6e69 6e67 2c20   repositioning, 
+00005ef0: 6475 7269 6e67 2061 6e20 5b6f 7269 6769  during an [origi
+00005f00: 6e5d 2063 6861 6e67 6520 6f72 2061 2072  n] change or a r
+00005f10: 6573 697a 652e 0d0a 0922 2222 0d0a       esize...."""..
```

### Comparing `kivygo-0.0.4/kivygo/uix/scrollview.py` & `kivygo-0.0.5/kivygo/widgets/scrollview.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 Builder.load_string("""
 
 #:import hex kivy.utils.get_color_from_hex
 
 
-<BarScroll>:
+<GoBarScroll>:
 	size_hint_x: None
 	width: '40dp'
 	canvas.after:
 		Color:
 			rgba: self._background_color
 		RoundedRectangle:
 			size: [ ( self.bar_width * 2 ), self.height ]
@@ -27,28 +27,28 @@
 		Color:
 			rgba: self._bar_color
 		RoundedRectangle:
 			size: [self.bar_width, self.bar_height]
 			pos: [ ( self.x + ( self.width / 2 ) - (self.bar_width / 2 ) ), self.bar_y ]
 			radius: self.bar_radius
 
-<ScrollViewBar>:
+<GoScrollViewBar>:
 	bar_color: [0, 0, 0, 0]
 	bar_inactive_color: [0, 0, 0, 0]
 	effect_cls: 'ScrollEffect'
 
 	
 """)
 
 
-class ScrollViewBar(ScrollView):
+class GoScrollViewBar(ScrollView):
 	pass
 
 
-class BarScroll(AnchorLayout):
+class GoBarScroll(AnchorLayout):
 
 	scroll_view = ObjectProperty(None)
 	_last_scroll_view = None
 	bar_width = NumericProperty(dp(4))
 	bar_height = NumericProperty(0)
 	bar_y = NumericProperty(0)
```

### Comparing `kivygo-0.0.4/kivygo/uix/segment.py` & `kivygo-0.0.5/kivygo/widgets/segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 
 from kivy.properties import StringProperty, BoundedNumericProperty
 from kivy.uix.relativelayout import RelativeLayout
 from kivy.graphics import Color, Ellipse, Mesh, Scale
 from kivy.utils import get_color_from_hex
 
 
-class Segment(RelativeLayout):
+class GoSegment(RelativeLayout):
   
     scale = BoundedNumericProperty(0.1, min=0.1, max=1, errorvalue=0.2)
     color = StringProperty('2fc827')
     value = StringProperty('A.')
 
     def __init__(self, **kwargs):     
         super().__init__(**kwargs)
 
         # Drawing meshes configuration, indices range meshes and mode
         self.indice = range(0, 6)
         self.xmode = 'triangle_fan'
         
-        # Segment matrix configuration
+        # GoSegment matrix configuration
         seg_1 = [
             20, 215, 0, 0,
             35, 230, 0, 0,
             95, 230, 0, 0,
             110, 215, 0, 0,
             95, 200, 0, 0,
             35, 200, 0, 0,
```

### Comparing `kivygo-0.0.4/kivygo/uix/shader.py` & `kivygo-0.0.5/kivygo/widgets/shader.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from kivy.core.window import Window
 from kivy.clock import Clock
 from kivy.graphics import (
     RenderContext, Fbo, Color,
     ClearColor, ClearBuffers,
     Rectangle
 )
-from kivy.uix.floatlayout import FloatLayout
+from kivygo.layouts.floatlayout import GoFloatLayout
 from kivy.properties import (
     StringProperty, ListProperty,
     ObjectProperty
 )
 
 
 header = '''
@@ -49,15 +49,15 @@
 }
 
 ''')
 
 
 
 
-class ShaderWidget(FloatLayout):
+class GoShaderWidget(GoFloatLayout):
 
     mouse_pos = ListProperty([100, 100])
 
     fs = StringProperty(None)
 
     texture = ObjectProperty(None)
```

### Comparing `kivygo-0.0.4/kivygo/uix/slider.py` & `kivygo-0.0.5/kivygo/widgets/slider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from kivy.clock import Clock
 from kivy.lang import Builder
 from kivy.properties import (
 	ColorProperty, ListProperty,
 	NumericProperty, ObjectProperty
 )
 from kivy.uix.slider import Slider
-from kivygo.behaviors.neumorph import NeuGlowCircular
-from kivygo.behaviors.thumb import Thumb
+from kivygo.behaviors.neumorph import GoGlowCircular
+from kivygo.behaviors.thumb import GoThumb
 from kivy.metrics import dp
 from kivy.graphics.texture import Texture
 from kivygo.utils import dec_2_rgb
 from PIL import Image, ImageDraw, ImageFilter
 
 
 Builder.load_string("""
 
-<NeuSlider>
+<GoSlider>
 	canvas:
 		Clear
 		Color:
 			rgba: self.background_color
 		RoundedRectangle:
 			size: self.size
 			pos: self.pos
 			radius: self.radius
 
 	background_width: 0
 	cursor_size: [0, 0]
 	padding: (self.height / 2)
 
-	NeuThumb:
+	GoSliderThumb:
 		canvas.before:
 			Color:
 			Rectangle:
 				size:self.glow_size
 				pos:self.glow_pos
 				texture:self.glow_texture
 		canvas:
@@ -49,15 +49,15 @@
 		pos: [ ( root.value_pos[0] - self.width / 2), ( root.center_y - self.height / 2) ]
 		behind_color: ( root.comp_color[0:3] + [0] ) if root.thumb_bg_color == [0, 0, 0, 0] else root.thumb_bg_color
 		glow_color: root.thumb_color if root.glow_color == [0, 0, 0, 0] else root.glow_color
 
 """)
 
 
-class NeuSlider(Slider):
+class GoSlider(Slider):
 
 	comp_color = ColorProperty("#333333")
 
 	shadow_behind_color = ColorProperty("#333333")
 
 	background_color = ListProperty([0.6, 0.1, 0.4, 1])
 
@@ -114,15 +114,15 @@
 	def elevation_set(self, *args):
 		self.elev = self.elevation
 
 	def radius_set(self, *args):
 		self.radius = [(self.height / 2)] * 4
 
 
-class NeuThumb(Thumb, NeuGlowCircular):
+class GoSliderThumb(GoThumb, GoGlowCircular):
 
 	glow_color = ColorProperty([0.8, 0.7, 0.5, 1])
 
 	elevation = NumericProperty(0)
 
 	glow_radius = NumericProperty(dp(20))
 	"""
```

### Comparing `kivygo-0.0.4/kivygo/uix/spinner.py` & `kivygo-0.0.5/kivygo/widgets/spinner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 
 
 from kivy.compat import string_types
 from kivy.factory import Factory
 from kivy.properties import ListProperty, ObjectProperty, BooleanProperty
-from kivygo.uix.button import ButtonEffect
+from kivygo.widgets.button import GoButtonRipple
 from kivy.uix.dropdown import DropDown
 
 
-class EffectSpinner(ButtonEffect):
+class GoEffectSpinner(GoButtonRipple):
 
     values = ListProperty([])
     '''Values that can be selected by the user. It must be a list of strings.
     '''
 
     text_autoupdate = BooleanProperty(False)
     '''Indicates if the spinner's :attr:`text` should be automatically
     updated with the first value of the :attr:`values` property.
     Setting it to True will cause the spinner to update its :attr:`text`
     property every time attr:`values` are changed.
     '''
 
-    option_cls = ObjectProperty(ButtonEffect)
+    option_cls = ObjectProperty(GoButtonRipple)
     '''Class used to display the options within the dropdown list displayed
     under the Spinner. The `text` property of the class will be used to
     represent the value.
 
     The option class requires:
 
     - a `text` property, used to display the value.
```

### Comparing `kivygo-0.0.4/kivygo/uix/taptargetview.py` & `kivygo-0.0.5/kivygo/widgets/taptargetview.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 	ObjectProperty, NumericProperty,
 	ListProperty, StringProperty,
 	BooleanProperty, OptionProperty
 )
 from kivy.uix.label import Label
 
 
-class TapTargetView(EventDispatcher):
-	"""Rough try to mimic the working of Android's TapTargetView."""
+class GoTapTargetView(EventDispatcher):
+	"""Rough try to mimic the working of Android's GoTapTargetView."""
 
 	widget = ObjectProperty(None)
 	"""
-	Widget to add ``TapTargetView`` upon.
+	Widget to add ``GoTapTargetView`` upon.
 	"""
 
 	outer_radius = NumericProperty(dp(300))
 	"""
 	Radius for outer circle.
 	"""
```

### Comparing `kivygo-0.0.4/kivygo/uix/terminal.py` & `kivygo-0.0.5/kivygo/widgets/terminal.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,53 +11,53 @@
 from kivy.clock import Clock
 from kivy.metrics import dp
 from pygments.styles import get_style_by_name
 
 
 Builder.load_string("""
 
-<CodeEditor>:
+<GoCodeEditor>:
 	id: scroller
 	code: text_code
 	effect_cls: 'ScrollEffect'
 	bar_width: '15dp'
 	input_minimum_height: text_code.minimum_height
-	TextCode:
+	GoTextCode:
 		id: text_code
 		size_hint: [None, None]
 		on_text: scroller.update_width_code()
 		height: max(self.minimum_height, scroller.height)
 		font_size: root.font_size
 		style: root.style
 		background_color: [1, 1, 1, 0]
 		text: root.text
 
 
-<InputEditor>:
+<GoInputEditor>:
 	id: scroller
 	code: text_code
 	effect_cls: 'ScrollEffect'
 	bar_width: '15dp'
 	input_minimum_height: text_code.minimum_height
-	InputTerminal:
+	GoInputTerminal:
 		id: text_code
 		size_hint: None, None
 		on_text: scroller.update_width_code()
 		height: max(self.minimum_height, scroller.height)
 		font_size: root.font_size
 		style: root.style
 		background_color: [1, 1, 1, 0]
 		text: root.text
 		foreground_color: root.text_color
 
 		
 """)
 
 
-class InputTerminal(TextInput):
+class GoInputTerminal(TextInput):
 
 	can_scroll = True
 
 	def on_touch_down(self, touch):
 		if not self.can_scroll:
 			# Não posso rolar
 			return False
@@ -66,19 +66,19 @@
 	def on_touch_move(self, touch):
 		if not self.can_scroll:
 			# Não posso rolar
 			return False
 		return super().on_touch_move(touch)
 
 
-class TextCode(CodeInput, InputTerminal):
+class GoTextCode(CodeInput, GoInputTerminal):
 	pass
 
 
-class CodeEditorBase(ScrollView):
+class GoCodeEditorBase(ScrollView):
 	
 	code = ObjectProperty(None)
 	bar_move = ''
 	change_width = ObjectProperty(True)
 	touch_pos = [0, 0]
 	style = ObjectProperty(get_style_by_name('monokai'))
 	text = StringProperty("")
@@ -248,14 +248,14 @@
 
 		# if not self.clickable:
 		#     return None
 	
 		return super().on_touch_move(touch)
 
 
-class InputEditor(CodeEditorBase):
+class GoInputEditor(GoCodeEditorBase):
 	pass
 
 
-class CodeEditor(CodeEditorBase):
+class GoCodeEditor(GoCodeEditorBase):
 	pass
```

### Comparing `kivygo-0.0.4/kivygo/utils.py` & `kivygo-0.0.5/kivygo/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,177 +50,177 @@
 00000310: 706f 730d 0a77 2c20 683a 2077 6964 6765  pos..w, h: widge
 00000320: 7420 7369 7a65 0d0a 7377 2c20 7368 3a20  t size..sw, sh: 
 00000330: 7376 6720 7369 7a65 0d0a 7366 3a20 7376  svg size..sf: sv
 00000340: 675f 6669 6c65 2c20 6f6e 6c79 206e 6565  g_file, only nee
 00000350: 6465 6420 666f 7220 6b69 7679 2069 636f  ded for kivy ico
 00000360: 6e20 7375 7070 6f72 740d 0a22 2222 0d0a  n support.."""..
 00000370: 2320 5370 6563 6961 6c20 7375 7070 6f72  # Special suppor
-00000380: 7420 666f 7220 4b69 7679 2073 7667 2049  t for Kivy svg I
-00000390: 636f 6e20 3a29 0d0a 0d0a 6465 6620 7828  con :)....def x(
-000003a0: 785f 706f 732c 2077 782c 2077 2c20 7377  x_pos, wx, w, sw
-000003b0: 2c20 7366 293a 0d0a 0d0a 2020 2020 6966  , sf):....    if
-000003c0: 2022 6b69 7679 2220 696e 2073 663a 0d0a   "kivy" in sf:..
-000003d0: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-000003e0: 2077 7820 2b20 2820 7720 2a20 2878 5f70   wx + ( w * (x_p
-000003f0: 6f73 202f 2031 3029 202f 2073 7729 2029  os / 10) / sw) )
-00000400: 0d0a 2020 2020 0d0a 2020 2020 7265 7475  ..    ..    retu
-00000410: 726e 2028 2077 7820 2b20 2877 202a 2078  rn ( wx + (w * x
-00000420: 5f70 6f73 202f 2073 7729 2029 0d0a 0d0a  _pos / sw) )....
-00000430: 0d0a 6465 6620 7928 795f 706f 732c 2077  ..def y(y_pos, w
-00000440: 792c 2068 2c20 7368 2c20 7366 293a 0d0a  y, h, sh, sf):..
-00000450: 2020 2020 0d0a 2020 2020 6966 2022 6b69      ..    if "ki
-00000460: 7679 2220 696e 2073 663a 0d0a 2020 2020  vy" in sf:..    
-00000470: 2020 2020 7265 7475 726e 2028 2077 7920      return ( wy 
-00000480: 2b20 2868 202a 2028 2879 5f70 6f73 202f  + (h * ((y_pos /
-00000490: 2031 3029 2920 2f20 7368 2920 290d 0a20   10)) / sh) ).. 
-000004a0: 2020 200d 0a20 2020 2072 6574 7572 6e20     ..    return 
-000004b0: 2820 7779 202b 2028 6820 2a20 2873 6820  ( wy + (h * (sh 
-000004c0: 2d20 795f 706f 7329 202f 2073 6829 2029  - y_pos) / sh) )
-000004d0: 0d0a 0d0a 0d0a 6465 6620 706f 696e 7428  ......def point(
-000004e0: 636f 6d70 6c65 785f 706f 696e 743a 2063  complex_point: c
-000004f0: 6f6d 706c 6578 2c20 772c 2068 2c20 7778  omplex, w, h, wx
-00000500: 2c20 7779 2c20 7377 2c20 7368 2c20 7366  , wy, sw, sh, sf
-00000510: 293a 200d 0a20 2020 2072 6574 7572 6e20  ): ..    return 
-00000520: 5b0d 0a20 2020 2020 2020 2078 2863 6f6d  [..        x(com
-00000530: 706c 6578 5f70 6f69 6e74 2e72 6561 6c2c  plex_point.real,
-00000540: 2077 782c 2077 2c20 7377 2c20 7366 292c   wx, w, sw, sf),
-00000550: 0d0a 2020 2020 2020 2020 7928 636f 6d70  ..        y(comp
-00000560: 6c65 785f 706f 696e 742e 696d 6167 2c20  lex_point.imag, 
-00000570: 7779 2c20 682c 2073 682c 2073 6629 0d0a  wy, h, sh, sf)..
-00000580: 2020 2020 5d0d 0a0d 0a0d 0a64 6566 2062      ]......def b
-00000590: 657a 6965 725f 706f 696e 7473 2865 3a20  ezier_points(e: 
-000005a0: 4375 6269 6342 657a 6965 722c 2077 2c20  CubicBezier, w, 
-000005b0: 682c 2077 782c 2077 792c 2073 772c 2073  h, wx, wy, sw, s
-000005c0: 682c 2073 6629 3a0d 0a20 2020 2072 6574  h, sf):..    ret
-000005d0: 7572 6e20 5b0d 0a20 2020 2020 2020 202a  urn [..        *
-000005e0: 706f 696e 7428 652e 7374 6172 742c 2077  point(e.start, w
-000005f0: 2c20 682c 2077 782c 2077 792c 2073 772c  , h, wx, wy, sw,
-00000600: 2073 682c 2073 6629 2c0d 0a20 2020 2020   sh, sf),..     
-00000610: 2020 202a 706f 696e 7428 652e 636f 6e74     *point(e.cont
-00000620: 726f 6c31 2c20 772c 2068 2c20 7778 2c20  rol1, w, h, wx, 
-00000630: 7779 2c20 7377 2c20 7368 2c20 7366 292c  wy, sw, sh, sf),
-00000640: 0d0a 2020 2020 2020 2020 2a70 6f69 6e74  ..        *point
-00000650: 2865 2e63 6f6e 7472 6f6c 322c 2077 2c20  (e.control2, w, 
-00000660: 682c 2077 782c 2077 792c 2073 772c 2073  h, wx, wy, sw, s
-00000670: 682c 2073 6629 2c0d 0a20 2020 2020 2020  h, sf),..       
-00000680: 202a 706f 696e 7428 652e 656e 642c 2077   *point(e.end, w
-00000690: 2c20 682c 2077 782c 2077 792c 2073 772c  , h, wx, wy, sw,
-000006a0: 2073 682c 2073 6629 2c0d 0a20 2020 205d   sh, sf),..    ]
-000006b0: 0d0a 0d0a 0d0a 6465 6620 6c69 6e65 5f70  ......def line_p
-000006c0: 6f69 6e74 7328 653a 204c 696e 652c 2077  oints(e: Line, w
-000006d0: 2c20 682c 2077 782c 2077 792c 2073 772c  , h, wx, wy, sw,
-000006e0: 2073 682c 2073 6629 3a0d 0a20 2020 2072   sh, sf):..    r
-000006f0: 6574 7572 6e20 5b0d 0a20 2020 2020 2020  eturn [..       
-00000700: 202a 706f 696e 7428 652e 7374 6172 742c   *point(e.start,
-00000710: 2077 2c20 682c 2077 782c 2077 792c 2073   w, h, wx, wy, s
-00000720: 772c 2073 682c 2073 6629 2c0d 0a20 2020  w, sh, sf),..   
-00000730: 2020 2020 202a 706f 696e 7428 652e 656e       *point(e.en
-00000740: 642c 2077 2c20 682c 2077 782c 2077 792c  d, w, h, wx, wy,
-00000750: 2073 772c 2073 682c 2073 6629 2c0d 0a20   sw, sh, sf),.. 
-00000760: 2020 205d 0d0a 0d0a 0d0a 2320 6874 7470     ]......# http
-00000770: 733a 2f2f 7374 6163 6b6f 7665 7266 6c6f  s://stackoverflo
-00000780: 772e 636f 6d2f 612f 3135 3339 3931 3733  w.com/a/15399173
-00000790: 2f38 3837 3139 3534 0d0a 6465 6620 4230  /8871954..def B0
-000007a0: 5f74 2874 293a 0d0a 2020 2020 7265 7475  _t(t):..    retu
-000007b0: 726e 2028 3120 2d20 7429 202a 2a20 330d  rn (1 - t) ** 3.
-000007c0: 0a0d 0a64 6566 2042 315f 7428 7429 3a0d  ...def B1_t(t):.
-000007d0: 0a20 2020 2072 6574 7572 6e20 3320 2a20  .    return 3 * 
-000007e0: 7420 2a20 2831 202d 2074 2920 2a2a 2032  t * (1 - t) ** 2
-000007f0: 0d0a 0d0a 6465 6620 4232 5f74 2874 293a  ....def B2_t(t):
-00000800: 0d0a 2020 2020 7265 7475 726e 2033 202a  ..    return 3 *
-00000810: 2074 202a 2a20 3220 2a20 2831 202d 2074   t ** 2 * (1 - t
-00000820: 290d 0a0d 0a64 6566 2042 335f 7428 7429  )....def B3_t(t)
-00000830: 3a0d 0a20 2020 2072 6574 7572 6e20 7420  :..    return t 
-00000840: 2a2a 2033 0d0a 0d0a 0d0a 6465 6620 6765  ** 3......def ge
-00000850: 745f 616c 6c5f 706f 696e 7473 2873 7461  t_all_points(sta
-00000860: 7274 2c20 6331 2c20 6332 2c20 656e 6429  rt, c1, c2, end)
-00000870: 3a0d 0a20 2020 2070 6f69 6e74 7320 3d20  :..    points = 
-00000880: 5b5d 0d0a 2020 2020 6178 2c20 6179 203d  []..    ax, ay =
-00000890: 2073 7461 7274 0d0a 2020 2020 6478 2c20   start..    dx, 
-000008a0: 6479 203d 2065 6e64 0d0a 2020 2020 6278  dy = end..    bx
-000008b0: 2c20 6279 203d 2063 310d 0a20 2020 2063  , by = c1..    c
-000008c0: 782c 2063 7920 3d20 6332 0d0a 0d0a 2020  x, cy = c2....  
-000008d0: 2020 7365 6720 3d20 3120 2f20 3430 0d0a    seg = 1 / 40..
-000008e0: 2020 2020 7420 3d20 300d 0a0d 0a20 2020      t = 0....   
-000008f0: 2077 6869 6c65 2074 203c 3d20 313a 0d0a   while t <= 1:..
-00000900: 2020 2020 2020 2020 706f 696e 7473 2e65          points.e
-00000910: 7874 656e 6428 0d0a 2020 2020 2020 2020  xtend(..        
-00000920: 2020 2020 5b0d 0a20 2020 2020 2020 2020      [..         
-00000930: 2020 2020 2020 2028 4230 5f74 2874 2920         (B0_t(t) 
-00000940: 2a20 6178 2920 2b20 2842 315f 7428 7429  * ax) + (B1_t(t)
-00000950: 202a 2062 7829 202b 2028 4232 5f74 2874   * bx) + (B2_t(t
-00000960: 2920 2a20 6378 2920 2b20 2842 335f 7428  ) * cx) + (B3_t(
-00000970: 7429 202a 2064 7829 2c0d 0a20 2020 2020  t) * dx),..     
-00000980: 2020 2020 2020 2020 2020 2028 4230 5f74             (B0_t
-00000990: 2874 2920 2a20 6179 2920 2b20 2842 315f  (t) * ay) + (B1_
-000009a0: 7428 7429 202a 2062 7929 202b 2028 4232  t(t) * by) + (B2
-000009b0: 5f74 2874 2920 2a20 6379 2920 2b20 2842  _t(t) * cy) + (B
-000009c0: 335f 7428 7429 202a 2064 7929 2c0d 0a20  3_t(t) * dy),.. 
-000009d0: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
-000009e0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-000009f0: 2074 202b 3d20 7365 670d 0a0d 0a20 2020   t += seg....   
-00000a00: 2072 6574 7572 6e20 706f 696e 7473 0d0a   return points..
-00000a10: 0d0a 6465 6620 7061 7273 655f 7376 6728  ..def parse_svg(
-00000a20: 7376 675f 6669 6c65 293a 0d0a 2020 2020  svg_file):..    
-00000a30: 646f 6320 3d20 6d69 6e69 646f 6d2e 7061  doc = minidom.pa
-00000a40: 7273 6528 7376 675f 6669 6c65 290d 0a0d  rse(svg_file)...
-00000a50: 0a20 2020 2076 6965 7762 6f78 5f73 7472  .    viewbox_str
-00000a60: 696e 6720 3d20 646f 632e 6765 7445 6c65  ing = doc.getEle
-00000a70: 6d65 6e74 7342 7954 6167 4e61 6d65 2822  mentsByTagName("
-00000a80: 7376 6722 295b 305d 2e67 6574 4174 7472  svg")[0].getAttr
-00000a90: 6962 7574 6528 2276 6965 7742 6f78 2229  ibute("viewBox")
-00000aa0: 0d0a 0d0a 2020 2020 7365 7020 3d20 222c  ....    sep = ",
-00000ab0: 2220 6966 2022 2c22 2069 6e20 7669 6577  " if "," in view
-00000ac0: 626f 785f 7374 7269 6e67 2065 6c73 6520  box_string else 
-00000ad0: 2220 220d 0a20 2020 2073 775f 7369 7a65  " "..    sw_size
-00000ae0: 203d 206c 6973 7428 206d 6170 2869 6e74   = list( map(int
-00000af0: 2c20 7669 6577 626f 785f 7374 7269 6e67  , viewbox_string
-00000b00: 2e73 706c 6974 2873 6570 295b 323a 5d29  .split(sep)[2:])
-00000b10: 2029 0d0a 2020 2020 0d0a 2020 2020 7061   )..    ..    pa
-00000b20: 7468 5f63 6f75 6e74 203d 2030 0d0a 2020  th_count = 0..  
-00000b30: 2020 7061 7468 5f73 7472 696e 6773 203d    path_strings =
-00000b40: 205b 5d0d 0a0d 0a20 2020 2066 6f72 2070   []....    for p
-00000b50: 6174 6820 696e 2064 6f63 2e67 6574 456c  ath in doc.getEl
-00000b60: 656d 656e 7473 4279 5461 674e 616d 6528  ementsByTagName(
-00000b70: 2270 6174 6822 293a 0d0a 2020 2020 2020  "path"):..      
-00000b80: 2020 6964 5f20 3d20 7061 7468 2e67 6574    id_ = path.get
-00000b90: 4174 7472 6962 7574 6528 2269 6422 2920  Attribute("id") 
-00000ba0: 6f72 2066 2270 6174 685f 7b70 6174 685f  or f"path_{path_
-00000bb0: 636f 756e 747d 220d 0a20 2020 2020 2020  count}"..       
-00000bc0: 2064 203d 2070 6174 682e 6765 7441 7474   d = path.getAtt
-00000bd0: 7269 6275 7465 2822 6422 290d 0a20 2020  ribute("d")..   
-00000be0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00000bf0: 2020 2020 2020 2063 6c72 203d 2067 6574         clr = get
-00000c00: 5f63 6f6c 6f72 5f66 726f 6d5f 6865 7828  _color_from_hex(
-00000c10: 7061 7468 2e67 6574 4174 7472 6962 7574  path.getAttribut
-00000c20: 6528 2266 696c 6c22 2929 206f 7220 5b31  e("fill")) or [1
-00000c30: 2c20 312c 2031 2c20 305d 0d0a 2020 2020  , 1, 1, 0]..    
-00000c40: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
-00000c50: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
-00000c60: 2020 2020 2320 6966 2063 6f6c 6f72 2066      # if color f
-00000c70: 6f72 6d61 7420 6973 2064 6966 6665 7265  ormat is differe
-00000c80: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-00000c90: 636c 7220 3d20 5b31 2c20 312c 2031 2c20  clr = [1, 1, 1, 
-00000ca0: 305d 0d0a 0d0a 2020 2020 2020 2020 7061  0]....        pa
-00000cb0: 7468 5f73 7472 696e 6773 2e61 7070 656e  th_strings.appen
-00000cc0: 6428 2864 2c20 6964 5f2c 2063 6c72 2929  d((d, id_, clr))
-00000cd0: 0d0a 2020 2020 2020 2020 7061 7468 5f63  ..        path_c
-00000ce0: 6f75 6e74 202b 3d20 310d 0a20 2020 200d  ount += 1..    .
-00000cf0: 0a20 2020 2064 6f63 2e75 6e6c 696e 6b28  .    doc.unlink(
-00000d00: 290d 0a20 2020 2072 6574 7572 6e20 5b73  )..    return [s
-00000d10: 775f 7369 7a65 2c20 7061 7468 5f73 7472  w_size, path_str
-00000d20: 696e 6773 5d0d 0a0d 0a64 6566 2066 696e  ings]....def fin
-00000d30: 645f 6365 6e74 6572 2869 6e70 7574 5f6c  d_center(input_l
-00000d40: 6973 7429 3a0d 0a20 2020 206d 6964 646c  ist):..    middl
-00000d50: 6520 3d20 666c 6f61 7428 6c65 6e28 696e  e = float(len(in
-00000d60: 7075 745f 6c69 7374 2929 202f 2032 0d0a  put_list)) / 2..
-00000d70: 2020 2020 0d0a 2020 2020 6966 206d 6964      ..    if mid
-00000d80: 646c 6520 2520 3220 213d 2030 3a0d 0a20  dle % 2 != 0:.. 
-00000d90: 2020 2020 2020 2072 6574 7572 6e20 696e         return in
-00000da0: 7075 745f 6c69 7374 5b69 6e74 286d 6964  put_list[int(mid
-00000db0: 646c 6520 2d20 302e 3529 5d0d 0a20 2020  dle - 0.5)]..   
-00000dc0: 200d 0a20 2020 2072 6574 7572 6e20 2820   ..    return ( 
-00000dd0: 2869 6e70 7574 5f6c 6973 745b 696e 7428  (input_list[int(
-00000de0: 6d69 6464 6c65 295d 202b 2069 6e70 7574  middle)] + input
-00000df0: 5f6c 6973 745b 696e 7428 6d69 6464 6c65  _list[int(middle
-00000e00: 2d31 295d 2920 2f20 3220 290d 0a0d 0a0d  -1)]) / 2 ).....
-00000e10: 0a                                       .
+00000380: 7420 666f 7220 4b69 7679 2073 7667 2047  t for Kivy svg G
+00000390: 6f49 636f 6e20 3a29 0d0a 0d0a 6465 6620  oIcon :)....def 
+000003a0: 7828 785f 706f 732c 2077 782c 2077 2c20  x(x_pos, wx, w, 
+000003b0: 7377 2c20 7366 293a 0d0a 0d0a 2020 2020  sw, sf):....    
+000003c0: 6966 2022 6b69 7679 2220 696e 2073 663a  if "kivy" in sf:
+000003d0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000003e0: 2028 2077 7820 2b20 2820 7720 2a20 2878   ( wx + ( w * (x
+000003f0: 5f70 6f73 202f 2031 3029 202f 2073 7729  _pos / 10) / sw)
+00000400: 2029 0d0a 2020 2020 0d0a 2020 2020 7265   )..    ..    re
+00000410: 7475 726e 2028 2077 7820 2b20 2877 202a  turn ( wx + (w *
+00000420: 2078 5f70 6f73 202f 2073 7729 2029 0d0a   x_pos / sw) )..
+00000430: 0d0a 0d0a 6465 6620 7928 795f 706f 732c  ....def y(y_pos,
+00000440: 2077 792c 2068 2c20 7368 2c20 7366 293a   wy, h, sh, sf):
+00000450: 0d0a 2020 2020 0d0a 2020 2020 6966 2022  ..    ..    if "
+00000460: 6b69 7679 2220 696e 2073 663a 0d0a 2020  kivy" in sf:..  
+00000470: 2020 2020 2020 7265 7475 726e 2028 2077        return ( w
+00000480: 7920 2b20 2868 202a 2028 2879 5f70 6f73  y + (h * ((y_pos
+00000490: 202f 2031 3029 2920 2f20 7368 2920 290d   / 10)) / sh) ).
+000004a0: 0a20 2020 200d 0a20 2020 2072 6574 7572  .    ..    retur
+000004b0: 6e20 2820 7779 202b 2028 6820 2a20 2873  n ( wy + (h * (s
+000004c0: 6820 2d20 795f 706f 7329 202f 2073 6829  h - y_pos) / sh)
+000004d0: 2029 0d0a 0d0a 0d0a 6465 6620 706f 696e   )......def poin
+000004e0: 7428 636f 6d70 6c65 785f 706f 696e 743a  t(complex_point:
+000004f0: 2063 6f6d 706c 6578 2c20 772c 2068 2c20   complex, w, h, 
+00000500: 7778 2c20 7779 2c20 7377 2c20 7368 2c20  wx, wy, sw, sh, 
+00000510: 7366 293a 200d 0a20 2020 2072 6574 7572  sf): ..    retur
+00000520: 6e20 5b0d 0a20 2020 2020 2020 2078 2863  n [..        x(c
+00000530: 6f6d 706c 6578 5f70 6f69 6e74 2e72 6561  omplex_point.rea
+00000540: 6c2c 2077 782c 2077 2c20 7377 2c20 7366  l, wx, w, sw, sf
+00000550: 292c 0d0a 2020 2020 2020 2020 7928 636f  ),..        y(co
+00000560: 6d70 6c65 785f 706f 696e 742e 696d 6167  mplex_point.imag
+00000570: 2c20 7779 2c20 682c 2073 682c 2073 6629  , wy, h, sh, sf)
+00000580: 0d0a 2020 2020 5d0d 0a0d 0a0d 0a64 6566  ..    ]......def
+00000590: 2062 657a 6965 725f 706f 696e 7473 2865   bezier_points(e
+000005a0: 3a20 4375 6269 6342 657a 6965 722c 2077  : CubicBezier, w
+000005b0: 2c20 682c 2077 782c 2077 792c 2073 772c  , h, wx, wy, sw,
+000005c0: 2073 682c 2073 6629 3a0d 0a20 2020 2072   sh, sf):..    r
+000005d0: 6574 7572 6e20 5b0d 0a20 2020 2020 2020  eturn [..       
+000005e0: 202a 706f 696e 7428 652e 7374 6172 742c   *point(e.start,
+000005f0: 2077 2c20 682c 2077 782c 2077 792c 2073   w, h, wx, wy, s
+00000600: 772c 2073 682c 2073 6629 2c0d 0a20 2020  w, sh, sf),..   
+00000610: 2020 2020 202a 706f 696e 7428 652e 636f       *point(e.co
+00000620: 6e74 726f 6c31 2c20 772c 2068 2c20 7778  ntrol1, w, h, wx
+00000630: 2c20 7779 2c20 7377 2c20 7368 2c20 7366  , wy, sw, sh, sf
+00000640: 292c 0d0a 2020 2020 2020 2020 2a70 6f69  ),..        *poi
+00000650: 6e74 2865 2e63 6f6e 7472 6f6c 322c 2077  nt(e.control2, w
+00000660: 2c20 682c 2077 782c 2077 792c 2073 772c  , h, wx, wy, sw,
+00000670: 2073 682c 2073 6629 2c0d 0a20 2020 2020   sh, sf),..     
+00000680: 2020 202a 706f 696e 7428 652e 656e 642c     *point(e.end,
+00000690: 2077 2c20 682c 2077 782c 2077 792c 2073   w, h, wx, wy, s
+000006a0: 772c 2073 682c 2073 6629 2c0d 0a20 2020  w, sh, sf),..   
+000006b0: 205d 0d0a 0d0a 0d0a 6465 6620 6c69 6e65   ]......def line
+000006c0: 5f70 6f69 6e74 7328 653a 204c 696e 652c  _points(e: Line,
+000006d0: 2077 2c20 682c 2077 782c 2077 792c 2073   w, h, wx, wy, s
+000006e0: 772c 2073 682c 2073 6629 3a0d 0a20 2020  w, sh, sf):..   
+000006f0: 2072 6574 7572 6e20 5b0d 0a20 2020 2020   return [..     
+00000700: 2020 202a 706f 696e 7428 652e 7374 6172     *point(e.star
+00000710: 742c 2077 2c20 682c 2077 782c 2077 792c  t, w, h, wx, wy,
+00000720: 2073 772c 2073 682c 2073 6629 2c0d 0a20   sw, sh, sf),.. 
+00000730: 2020 2020 2020 202a 706f 696e 7428 652e         *point(e.
+00000740: 656e 642c 2077 2c20 682c 2077 782c 2077  end, w, h, wx, w
+00000750: 792c 2073 772c 2073 682c 2073 6629 2c0d  y, sw, sh, sf),.
+00000760: 0a20 2020 205d 0d0a 0d0a 0d0a 2320 6874  .    ]......# ht
+00000770: 7470 733a 2f2f 7374 6163 6b6f 7665 7266  tps://stackoverf
+00000780: 6c6f 772e 636f 6d2f 612f 3135 3339 3931  low.com/a/153991
+00000790: 3733 2f38 3837 3139 3534 0d0a 6465 6620  73/8871954..def 
+000007a0: 4230 5f74 2874 293a 0d0a 2020 2020 7265  B0_t(t):..    re
+000007b0: 7475 726e 2028 3120 2d20 7429 202a 2a20  turn (1 - t) ** 
+000007c0: 330d 0a0d 0a64 6566 2042 315f 7428 7429  3....def B1_t(t)
+000007d0: 3a0d 0a20 2020 2072 6574 7572 6e20 3320  :..    return 3 
+000007e0: 2a20 7420 2a20 2831 202d 2074 2920 2a2a  * t * (1 - t) **
+000007f0: 2032 0d0a 0d0a 6465 6620 4232 5f74 2874   2....def B2_t(t
+00000800: 293a 0d0a 2020 2020 7265 7475 726e 2033  ):..    return 3
+00000810: 202a 2074 202a 2a20 3220 2a20 2831 202d   * t ** 2 * (1 -
+00000820: 2074 290d 0a0d 0a64 6566 2042 335f 7428   t)....def B3_t(
+00000830: 7429 3a0d 0a20 2020 2072 6574 7572 6e20  t):..    return 
+00000840: 7420 2a2a 2033 0d0a 0d0a 0d0a 6465 6620  t ** 3......def 
+00000850: 6765 745f 616c 6c5f 706f 696e 7473 2873  get_all_points(s
+00000860: 7461 7274 2c20 6331 2c20 6332 2c20 656e  tart, c1, c2, en
+00000870: 6429 3a0d 0a20 2020 2070 6f69 6e74 7320  d):..    points 
+00000880: 3d20 5b5d 0d0a 2020 2020 6178 2c20 6179  = []..    ax, ay
+00000890: 203d 2073 7461 7274 0d0a 2020 2020 6478   = start..    dx
+000008a0: 2c20 6479 203d 2065 6e64 0d0a 2020 2020  , dy = end..    
+000008b0: 6278 2c20 6279 203d 2063 310d 0a20 2020  bx, by = c1..   
+000008c0: 2063 782c 2063 7920 3d20 6332 0d0a 0d0a   cx, cy = c2....
+000008d0: 2020 2020 7365 6720 3d20 3120 2f20 3430      seg = 1 / 40
+000008e0: 0d0a 2020 2020 7420 3d20 300d 0a0d 0a20  ..    t = 0.... 
+000008f0: 2020 2077 6869 6c65 2074 203c 3d20 313a     while t <= 1:
+00000900: 0d0a 2020 2020 2020 2020 706f 696e 7473  ..        points
+00000910: 2e65 7874 656e 6428 0d0a 2020 2020 2020  .extend(..      
+00000920: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
+00000930: 2020 2020 2020 2020 2028 4230 5f74 2874           (B0_t(t
+00000940: 2920 2a20 6178 2920 2b20 2842 315f 7428  ) * ax) + (B1_t(
+00000950: 7429 202a 2062 7829 202b 2028 4232 5f74  t) * bx) + (B2_t
+00000960: 2874 2920 2a20 6378 2920 2b20 2842 335f  (t) * cx) + (B3_
+00000970: 7428 7429 202a 2064 7829 2c0d 0a20 2020  t(t) * dx),..   
+00000980: 2020 2020 2020 2020 2020 2020 2028 4230               (B0
+00000990: 5f74 2874 2920 2a20 6179 2920 2b20 2842  _t(t) * ay) + (B
+000009a0: 315f 7428 7429 202a 2062 7929 202b 2028  1_t(t) * by) + (
+000009b0: 4232 5f74 2874 2920 2a20 6379 2920 2b20  B2_t(t) * cy) + 
+000009c0: 2842 335f 7428 7429 202a 2064 7929 2c0d  (B3_t(t) * dy),.
+000009d0: 0a20 2020 2020 2020 2020 2020 205d 0d0a  .            ]..
+000009e0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+000009f0: 2020 2074 202b 3d20 7365 670d 0a0d 0a20     t += seg.... 
+00000a00: 2020 2072 6574 7572 6e20 706f 696e 7473     return points
+00000a10: 0d0a 0d0a 6465 6620 7061 7273 655f 7376  ....def parse_sv
+00000a20: 6728 7376 675f 6669 6c65 293a 0d0a 2020  g(svg_file):..  
+00000a30: 2020 646f 6320 3d20 6d69 6e69 646f 6d2e    doc = minidom.
+00000a40: 7061 7273 6528 7376 675f 6669 6c65 290d  parse(svg_file).
+00000a50: 0a0d 0a20 2020 2076 6965 7762 6f78 5f73  ...    viewbox_s
+00000a60: 7472 696e 6720 3d20 646f 632e 6765 7445  tring = doc.getE
+00000a70: 6c65 6d65 6e74 7342 7954 6167 4e61 6d65  lementsByTagName
+00000a80: 2822 7376 6722 295b 305d 2e67 6574 4174  ("svg")[0].getAt
+00000a90: 7472 6962 7574 6528 2276 6965 7742 6f78  tribute("viewBox
+00000aa0: 2229 0d0a 0d0a 2020 2020 7365 7020 3d20  ")....    sep = 
+00000ab0: 222c 2220 6966 2022 2c22 2069 6e20 7669  "," if "," in vi
+00000ac0: 6577 626f 785f 7374 7269 6e67 2065 6c73  ewbox_string els
+00000ad0: 6520 2220 220d 0a20 2020 2073 775f 7369  e " "..    sw_si
+00000ae0: 7a65 203d 206c 6973 7428 206d 6170 2869  ze = list( map(i
+00000af0: 6e74 2c20 7669 6577 626f 785f 7374 7269  nt, viewbox_stri
+00000b00: 6e67 2e73 706c 6974 2873 6570 295b 323a  ng.split(sep)[2:
+00000b10: 5d29 2029 0d0a 2020 2020 0d0a 2020 2020  ]) )..    ..    
+00000b20: 7061 7468 5f63 6f75 6e74 203d 2030 0d0a  path_count = 0..
+00000b30: 2020 2020 7061 7468 5f73 7472 696e 6773      path_strings
+00000b40: 203d 205b 5d0d 0a0d 0a20 2020 2066 6f72   = []....    for
+00000b50: 2070 6174 6820 696e 2064 6f63 2e67 6574   path in doc.get
+00000b60: 456c 656d 656e 7473 4279 5461 674e 616d  ElementsByTagNam
+00000b70: 6528 2270 6174 6822 293a 0d0a 2020 2020  e("path"):..    
+00000b80: 2020 2020 6964 5f20 3d20 7061 7468 2e67      id_ = path.g
+00000b90: 6574 4174 7472 6962 7574 6528 2269 6422  etAttribute("id"
+00000ba0: 2920 6f72 2066 2270 6174 685f 7b70 6174  ) or f"path_{pat
+00000bb0: 685f 636f 756e 747d 220d 0a20 2020 2020  h_count}"..     
+00000bc0: 2020 2064 203d 2070 6174 682e 6765 7441     d = path.getA
+00000bd0: 7474 7269 6275 7465 2822 6422 290d 0a20  ttribute("d").. 
+00000be0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00000bf0: 2020 2020 2020 2020 2063 6c72 203d 2067           clr = g
+00000c00: 6574 5f63 6f6c 6f72 5f66 726f 6d5f 6865  et_color_from_he
+00000c10: 7828 7061 7468 2e67 6574 4174 7472 6962  x(path.getAttrib
+00000c20: 7574 6528 2266 696c 6c22 2929 206f 7220  ute("fill")) or 
+00000c30: 5b31 2c20 312c 2031 2c20 305d 0d0a 2020  [1, 1, 1, 0]..  
+00000c40: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
+00000c50: 7565 4572 726f 723a 0d0a 2020 2020 2020  ueError:..      
+00000c60: 2020 2020 2020 2320 6966 2063 6f6c 6f72        # if color
+00000c70: 2066 6f72 6d61 7420 6973 2064 6966 6665   format is diffe
+00000c80: 7265 6e74 0d0a 2020 2020 2020 2020 2020  rent..          
+00000c90: 2020 636c 7220 3d20 5b31 2c20 312c 2031    clr = [1, 1, 1
+00000ca0: 2c20 305d 0d0a 0d0a 2020 2020 2020 2020  , 0]....        
+00000cb0: 7061 7468 5f73 7472 696e 6773 2e61 7070  path_strings.app
+00000cc0: 656e 6428 2864 2c20 6964 5f2c 2063 6c72  end((d, id_, clr
+00000cd0: 2929 0d0a 2020 2020 2020 2020 7061 7468  ))..        path
+00000ce0: 5f63 6f75 6e74 202b 3d20 310d 0a20 2020  _count += 1..   
+00000cf0: 200d 0a20 2020 2064 6f63 2e75 6e6c 696e   ..    doc.unlin
+00000d00: 6b28 290d 0a20 2020 2072 6574 7572 6e20  k()..    return 
+00000d10: 5b73 775f 7369 7a65 2c20 7061 7468 5f73  [sw_size, path_s
+00000d20: 7472 696e 6773 5d0d 0a0d 0a64 6566 2066  trings]....def f
+00000d30: 696e 645f 6365 6e74 6572 2869 6e70 7574  ind_center(input
+00000d40: 5f6c 6973 7429 3a0d 0a20 2020 206d 6964  _list):..    mid
+00000d50: 646c 6520 3d20 666c 6f61 7428 6c65 6e28  dle = float(len(
+00000d60: 696e 7075 745f 6c69 7374 2929 202f 2032  input_list)) / 2
+00000d70: 0d0a 2020 2020 0d0a 2020 2020 6966 206d  ..    ..    if m
+00000d80: 6964 646c 6520 2520 3220 213d 2030 3a0d  iddle % 2 != 0:.
+00000d90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000da0: 696e 7075 745f 6c69 7374 5b69 6e74 286d  input_list[int(m
+00000db0: 6964 646c 6520 2d20 302e 3529 5d0d 0a20  iddle - 0.5)].. 
+00000dc0: 2020 200d 0a20 2020 2072 6574 7572 6e20     ..    return 
+00000dd0: 2820 2869 6e70 7574 5f6c 6973 745b 696e  ( (input_list[in
+00000de0: 7428 6d69 6464 6c65 295d 202b 2069 6e70  t(middle)] + inp
+00000df0: 7574 5f6c 6973 745b 696e 7428 6d69 6464  ut_list[int(midd
+00000e00: 6c65 2d31 295d 2920 2f20 3220 290d 0a0d  le-1)]) / 2 )...
+00000e10: 0a0d 0a                                  ...
```

### Comparing `kivygo-0.0.4/kivygo.egg-info/SOURCES.txt` & `kivygo-0.0.5/kivygo.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 kivygo.egg-info/SOURCES.txt
 kivygo.egg-info/dependency_links.txt
 kivygo.egg-info/requires.txt
 kivygo.egg-info/top_level.txt
 kivygo/behaviors/__init__.py
 kivygo/behaviors/button.py
 kivygo/behaviors/drag_and_drop.py
+kivygo/behaviors/effect.py
 kivygo/behaviors/hover.py
 kivygo/behaviors/neumorph.py
 kivygo/behaviors/resizable.py
 kivygo/behaviors/thumb.py
-kivygo/behaviors/touch_effecs.py
 kivygo/config/coins.atlas
 kivygo/config/coins.bounds
 kivygo/config/drugs.pex
 kivygo/config/fire.pex
 kivygo/config/jellyfish.pex
 kivygo/config/particle.pex
 kivygo/config/particle.png
@@ -51,22 +51,30 @@
 kivygo/icons/search.svg
 kivygo/icons/so.svg
 kivygo/icons/square.png
 kivygo/icons/sublime.svg
 kivygo/icons/text.svg
 kivygo/icons/transparent.png
 kivygo/icons/twitter2.svg
+kivygo/images/6915-green.png
+kivygo/images/Path.png
 kivygo/images/busan.jpg
 kivygo/images/demoimage.jpg
 kivygo/images/icon-kivygo.png
 kivygo/images/iris.jpg
 kivygo/images/lion.jpg
 kivygo/images/navigationdrawer_gradient_ltor.png
 kivygo/images/navigationdrawer_gradient_rtol.png
 kivygo/images/test.jpg
+kivygo/layouts/__init__.py
+kivygo/layouts/anchorlayout.py
+kivygo/layouts/boxlayout.py
+kivygo/layouts/circularlayout.py
+kivygo/layouts/floatlayout.py
+kivygo/layouts/gridlayout.py
 kivygo/transitions/Angular.glsl
 kivygo/transitions/Bounce.glsl
 kivygo/transitions/BowTieHorizontal.glsl
 kivygo/transitions/BowTieVertical.glsl
 kivygo/transitions/Burn.glsl
 kivygo/transitions/ButterflyWaveScrawler.glsl
 kivygo/transitions/CannabisLeaf.glsl
@@ -135,46 +143,40 @@
 kivygo/transitions/WipeRight.glsl
 kivygo/transitions/WipeUp.glsl
 kivygo/transitions/ZoomInCircles.glsl
 kivygo/transitions/__init__.py
 kivygo/transitions/base.py
 kivygo/transitions/extra/footer.glsl
 kivygo/transitions/extra/header.glsl
-kivygo/uix/__init__.py
-kivygo/uix/anchorlayout.py
-kivygo/uix/androidtabs.py
-kivygo/uix/bezier.py
-kivygo/uix/boxlayout.py
-kivygo/uix/button.py
-kivygo/uix/camera.py
-kivygo/uix/circular_bar.py
-kivygo/uix/circulardatetimepicker.py
-kivygo/uix/circularlayout.py
-kivygo/uix/codeinput.py
-kivygo/uix/curvelayout.py
-kivygo/uix/effect.py
-kivygo/uix/floatlayout.py
-kivygo/uix/frostedglass.py
-kivygo/uix/gradient.py
-kivygo/uix/gridlayout.py
-kivygo/uix/icon.py
-kivygo/uix/image.py
-kivygo/uix/input.py
-kivygo/uix/joystick.py
-kivygo/uix/kivyg_icon.py
-kivygo/uix/label.py
-kivygo/uix/navigationdrawer.py
-kivygo/uix/particle.py
-kivygo/uix/pizza_graph.py
-kivygo/uix/popup.py
-kivygo/uix/progressspinner.py
-kivygo/uix/radialslider.py
-kivygo/uix/rotabox.py
-kivygo/uix/screenmanager.py
-kivygo/uix/scrollview.py
-kivygo/uix/segment.py
-kivygo/uix/shader.py
-kivygo/uix/simpletablelayout.py
-kivygo/uix/slider.py
-kivygo/uix/spinner.py
-kivygo/uix/taptargetview.py
-kivygo/uix/terminal.py
+kivygo/widgets/__init__.py
+kivygo/widgets/bezier.py
+kivygo/widgets/button.py
+kivygo/widgets/camera.py
+kivygo/widgets/circular_bar.py
+kivygo/widgets/circulardatetimepicker.py
+kivygo/widgets/codeinput.py
+kivygo/widgets/effect.py
+kivygo/widgets/frostedglass.py
+kivygo/widgets/gradient.py
+kivygo/widgets/icon.py
+kivygo/widgets/image.py
+kivygo/widgets/input.py
+kivygo/widgets/joystick.py
+kivygo/widgets/kivyg_icon.py
+kivygo/widgets/label.py
+kivygo/widgets/navigationdrawer.py
+kivygo/widgets/particle.py
+kivygo/widgets/pizza_graph.py
+kivygo/widgets/popup.py
+kivygo/widgets/progressspinner.py
+kivygo/widgets/radialslider.py
+kivygo/widgets/rotabox.py
+kivygo/widgets/screenmanager.py
+kivygo/widgets/scrollview.py
+kivygo/widgets/segment.py
+kivygo/widgets/shader.py
+kivygo/widgets/slider.py
+kivygo/widgets/spinner.py
+kivygo/widgets/tab.py
+kivygo/widgets/taptargetview.py
+kivygo/widgets/terminal.py
+kivygo/widgets/widget.py
```

### Comparing `kivygo-0.0.4/setup.py` & `kivygo-0.0.5/setup.py`

 * *Files identical despite different names*

