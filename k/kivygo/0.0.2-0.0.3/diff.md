# Comparing `tmp/kivygo-0.0.2.tar.gz` & `tmp/kivygo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivygo-0.0.2.tar", last modified: Tue May 30 13:32:21 2023, max compression
+gzip compressed data, was "kivygo-0.0.3.tar", last modified: Tue May 30 13:34:44 2023, max compression
```

## Comparing `kivygo-0.0.2.tar` & `kivygo-0.0.3.tar`

### file list

```diff
@@ -1,153 +1,193 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.546431 kivygo-0.0.2/
--rw-rw-rw-   0        0        0     1098 2023-04-28 02:03:52.000000 kivygo-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      192 2023-05-30 13:32:21.546431 kivygo-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.356984 kivygo-0.0.2/kivygo/
--rw-rw-rw-   0        0        0       23 2023-05-30 13:32:16.000000 kivygo-0.0.2/kivygo/__init__.py
--rw-rw-rw-   0        0        0    23309 2023-05-13 18:28:10.000000 kivygo-0.0.2/kivygo/animation.py
--rw-rw-rw-   0        0        0     2905 2023-05-13 17:09:56.000000 kivygo-0.0.2/kivygo/app.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.408141 kivygo-0.0.2/kivygo/behaviors/
--rw-rw-rw-   0        0        0        0 2023-05-30 13:05:00.000000 kivygo-0.0.2/kivygo/behaviors/__init__.py
--rw-rw-rw-   0        0        0     8273 2023-05-13 17:19:46.000000 kivygo-0.0.2/kivygo/behaviors/button.py
--rw-rw-rw-   0        0        0     9872 2023-05-13 18:19:31.000000 kivygo-0.0.2/kivygo/behaviors/drag_and_drop.py
--rw-rw-rw-   0        0        0     5825 2023-05-13 18:20:08.000000 kivygo-0.0.2/kivygo/behaviors/hover.py
--rw-rw-rw-   0        0        0     3058 2023-05-05 22:06:08.000000 kivygo-0.0.2/kivygo/behaviors/neumorph.py
--rw-rw-rw-   0        0        0    13342 2023-04-28 02:33:05.000000 kivygo-0.0.2/kivygo/behaviors/resizable.py
--rw-rw-rw-   0        0        0    15085 2023-05-08 00:20:07.000000 kivygo-0.0.2/kivygo/behaviors/thumb.py
--rw-rw-rw-   0        0        0     4375 2023-05-07 23:38:10.000000 kivygo-0.0.2/kivygo/behaviors/touch_effecs.py
--rw-rw-rw-   0        0        0    16042 2023-05-01 21:00:44.000000 kivygo-0.0.2/kivygo/bounds_math.py
--rw-rw-rw-   0        0        0     2375 2023-05-29 23:31:04.000000 kivygo-0.0.2/kivygo/colors.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.417144 kivygo-0.0.2/kivygo/config/
--rw-rw-rw-   0        0        0      296 2023-04-30 03:08:38.000000 kivygo-0.0.2/kivygo/config/coins.atlas
--rw-rw-rw-   0        0        0     4765 2023-04-29 21:48:35.000000 kivygo-0.0.2/kivygo/config/coins.bounds
--rw-rw-rw-   0        0        0     1490 2013-02-26 10:24:28.000000 kivygo-0.0.2/kivygo/config/drugs.pex
--rw-rw-rw-   0        0        0     1489 2013-02-26 10:24:28.000000 kivygo-0.0.2/kivygo/config/fire.pex
--rw-rw-rw-   0        0        0     1496 2013-02-26 10:24:28.000000 kivygo-0.0.2/kivygo/config/jellyfish.pex
--rw-rw-rw-   0        0        0     1463 2013-02-26 10:24:28.000000 kivygo-0.0.2/kivygo/config/particle.pex
--rw-rw-rw-   0        0        0      870 2013-02-26 10:24:28.000000 kivygo-0.0.2/kivygo/config/particle.png
--rw-rw-rw-   0        0        0     1494 2013-02-26 10:24:28.000000 kivygo-0.0.2/kivygo/config/sun.pex
-drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.420145 kivygo-0.0.2/kivygo/elevation/
--rw-rw-rw-   0        0        0     1630 2023-01-06 02:24:33.000000 kivygo-0.0.2/kivygo/elevation/elevation.frag
--rw-rw-rw-   0        0        0      198 2023-01-06 02:24:33.000000 kivygo-0.0.2/kivygo/elevation/header.frag
--rw-rw-rw-   0        0        0      184 2023-01-06 02:24:33.000000 kivygo-0.0.2/kivygo/elevation/main.frag
-drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.448568 kivygo-0.0.2/kivygo/icons/
--rw-rw-rw-   0        0        0   156742 2023-03-02 15:36:22.000000 kivygo-0.0.2/kivygo/icons/bg_example.png
--rw-rw-rw-   0        0        0    95465 2022-05-23 02:23:22.000000 kivygo-0.0.2/kivygo/icons/coins.png
--rw-rw-rw-   0        0        0     1244 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/discord.svg
--rw-rw-rw-   0        0        0      781 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/discord2.svg
--rw-rw-rw-   0        0        0      704 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/facebook2.svg
--rw-rw-rw-   0        0        0     2453 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/github.svg
--rw-rw-rw-   0        0        0     1864 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/github2.svg
--rw-rw-rw-   0        0        0      829 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/github3.svg
--rw-rw-rw-   0        0        0     2451 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/google.svg
--rw-rw-rw-   0        0        0      990 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/google3.svg
--rw-rw-rw-   0        0        0     2636 2022-05-23 02:23:22.000000 kivygo-0.0.2/kivygo/icons/kivy.png
--rw-rw-rw-   0        0        0     1141 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/kivy.svg
--rw-rw-rw-   0        0        0    16577 2023-03-02 15:36:22.000000 kivygo-0.0.2/kivygo/icons/kivy_logo.png
--rw-rw-rw-   0        0        0    42074 2021-05-11 19:10:56.000000 kivygo-0.0.2/kivygo/icons/kivymd_logo.png
--rw-rw-rw-   0        0        0     2919 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/pie_chart.svg
--rw-rw-rw-   0        0        0     1458 2023-02-14 20:11:52.000000 kivygo-0.0.2/kivygo/icons/pipette.png
--rw-rw-rw-   0        0        0     1133 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/python2.svg
--rw-rw-rw-   0        0        0     1621 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/search.svg
--rw-rw-rw-   0        0        0      851 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/so.svg
--rw-rw-rw-   0        0        0     1481 2022-05-23 02:23:22.000000 kivygo-0.0.2/kivygo/icons/square.png
--rw-rw-rw-   0        0        0     1814 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/sublime.svg
--rw-rw-rw-   0        0        0     3454 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/text.svg
--rw-rw-rw-   0        0        0     1928 2023-02-14 20:11:52.000000 kivygo-0.0.2/kivygo/icons/transparent.png
--rw-rw-rw-   0        0        0     1086 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/twitter2.svg
-drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.461541 kivygo-0.0.2/kivygo/images/
--rw-rw-rw-   0        0        0   709001 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/images/busan.jpg
--rw-rw-rw-   0        0        0   118790 2018-10-01 10:52:31.000000 kivygo-0.0.2/kivygo/images/demoimage.jpg
--rw-rw-rw-   0        0        0   190380 2023-04-28 21:56:31.000000 kivygo-0.0.2/kivygo/images/icon-kivygo.png
--rw-rw-rw-   0        0        0   431598 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/images/iris.jpg
--rw-rw-rw-   0        0        0   857961 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/images/lion.jpg
--rw-rw-rw-   0        0        0      879 2019-05-19 13:30:15.000000 kivygo-0.0.2/kivygo/images/navigationdrawer_gradient_ltor.png
--rw-rw-rw-   0        0        0      874 2019-05-19 13:30:15.000000 kivygo-0.0.2/kivygo/images/navigationdrawer_gradient_rtol.png
--rw-rw-rw-   0        0        0  1537713 2023-02-14 20:11:52.000000 kivygo-0.0.2/kivygo/images/test.jpg
--rw-rw-rw-   0        0        0     2334 2023-04-21 01:53:43.000000 kivygo-0.0.2/kivygo/transformations.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.543436 kivygo-0.0.2/kivygo/transitions/
--rw-rw-rw-   0        0        0      452 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Angular.glsl
--rw-rw-rw-   0        0        0      719 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Bounce.glsl
--rw-rw-rw-   0        0        0     2593 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/BowTieHorizontal.glsl
--rw-rw-rw-   0        0        0     2541 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/BowTieVertical.glsl
--rw-rw-rw-   0        0        0      231 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Burn.glsl
--rw-rw-rw-   0        0        0      948 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/ButterflyWaveScrawler.glsl
--rw-rw-rw-   0        0        0      485 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/CannabisLeaf.glsl
--rw-rw-rw-   0        0        0      398 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Circle.glsl
--rw-rw-rw-   0        0        0      386 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/CircleOpen.glsl
--rw-rw-rw-   0        0        0      370 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/ColorPhase.glsl
--rw-rw-rw-   0        0        0      353 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/ColourDistance.glsl
--rw-rw-rw-   0        0        0      586 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/CrazyParametricFun.glsl
--rw-rw-rw-   0        0        0      590 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/CrossHatch.glsl
--rw-rw-rw-   0        0        0      228 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/CrossWarp.glsl
--rw-rw-rw-   0        0        0     2385 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/CrossZoom.glsl
--rw-rw-rw-   0        0        0     1694 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Cube.glsl
--rw-rw-rw-   0        0        0      352 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/DirectionalEasing.glsl
--rw-rw-rw-   0        0        0      489 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/DirectionalWarp.glsl
--rw-rw-rw-   0        0        0      557 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/DirectionalWipe.glsl
--rw-rw-rw-   0        0        0      522 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Displacement.glsl
--rw-rw-rw-   0        0        0     1574 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/DoomScreenTransition.glsl
--rw-rw-rw-   0        0        0     1189 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Doorway.glsl
--rw-rw-rw-   0        0        0      378 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Dreamy.glsl
--rw-rw-rw-   0        0        0     1183 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/DreamyZoom.glsl
--rw-rw-rw-   0        0        0      136 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Fade.glsl
--rw-rw-rw-   0        0        0      391 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/FadeColor.glsl
--rw-rw-rw-   0        0        0      546 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/FadeGrayscale.glsl
--rw-rw-rw-   0        0        0     2220 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/FilmBurn.glsl
--rw-rw-rw-   0        0        0      489 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/FlyEye.glsl
--rw-rw-rw-   0        0        0     2198 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/GlitchDisplace.glsl
--rw-rw-rw-   0        0        0      607 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/GlitchMemories.glsl
--rw-rw-rw-   0        0        0     2245 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/GridFlip.glsl
--rw-rw-rw-   0        0        0      356 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Heart.glsl
--rw-rw-rw-   0        0        0     1663 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Hexagonalize.glsl
--rw-rw-rw-   0        0        0      549 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Kaleidoscope.glsl
--rw-rw-rw-   0        0        0      647 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/LeftRight.glsl
--rw-rw-rw-   0        0        0      671 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/LinearBlur.glsl
--rw-rw-rw-   0        0        0      226 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Luma.glsl
--rw-rw-rw-   0        0        0     3781 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/LuminanceMelt.glsl
--rw-rw-rw-   0        0        0      379 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Morph.glsl
--rw-rw-rw-   0        0        0     1105 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Mosaic.glsl
--rw-rw-rw-   0        0        0      339 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/MultiplyBlend.glsl
--rw-rw-rw-   0        0        0     1390 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/PageCurl.glsl
--rw-rw-rw-   0        0        0     1367 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Perlin.glsl
--rw-rw-rw-   0        0        0      349 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Pinwheel.glsl
--rw-rw-rw-   0        0        0      562 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Pixelize.glsl
--rw-rw-rw-   0        0        0      452 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/PolarFunction.glsl
--rw-rw-rw-   0        0        0      304 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/PolkaDotsCurtain.glsl
--rw-rw-rw-   0        0        0      353 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Radial.glsl
--rw-rw-rw-   0        0        0      444 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/RandomNoise.glsl
--rw-rw-rw-   0        0        0      377 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/RandomSquares.glsl
--rw-rw-rw-   0        0        0      356 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Ripple.glsl
--rw-rw-rw-   0        0        0      832 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/RotateScaleFade.glsl
--rw-rw-rw-   0        0        0      348 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/RotateTransition.glsl
--rw-rw-rw-   0        0        0      365 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/SimpleZoom.glsl
--rw-rw-rw-   0        0        0      742 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/SquaresWire.glsl
--rw-rw-rw-   0        0        0      444 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Squeeze.glsl
--rw-rw-rw-   0        0        0     8033 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/StereoViewer.glsl
--rw-rw-rw-   0        0        0     1506 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Swap.glsl
--rw-rw-rw-   0        0        0      715 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Swirl.glsl
--rw-rw-rw-   0        0        0     4051 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/TangentMotionBlur.glsl
--rw-rw-rw-   0        0        0      650 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/TopBottom.glsl
--rw-rw-rw-   0        0        0     1366 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/UndulatingBurnOut.glsl
--rw-rw-rw-   0        0        0      409 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WaterDrop.glsl
--rw-rw-rw-   0        0        0      386 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Wind.glsl
--rw-rw-rw-   0        0        0      274 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WindowBlinds.glsl
--rw-rw-rw-   0        0        0      277 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WindowSlice.glsl
--rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WipeDown.glsl
--rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WipeLeft.glsl
--rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WipeRight.glsl
--rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WipeUp.glsl
--rw-rw-rw-   0        0        0     1115 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/ZoomInCircles.glsl
--rw-rw-rw-   0        0        0     8072 2023-05-01 19:46:08.000000 kivygo-0.0.2/kivygo/transitions/__init__.py
--rw-rw-rw-   0        0        0     1197 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/base.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.545428 kivygo-0.0.2/kivygo/transitions/extra/
--rw-rw-rw-   0        0        0      177 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/extra/footer.glsl
--rw-rw-rw-   0        0        0      403 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/extra/header.glsl
--rw-rw-rw-   0        0        0     3601 2023-05-04 01:11:32.000000 kivygo-0.0.2/kivygo/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.398194 kivygo-0.0.2/kivygo.egg-info/
--rw-rw-rw-   0        0        0      192 2023-05-30 13:32:21.000000 kivygo-0.0.2/kivygo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4354 2023-05-30 13:32:21.000000 kivygo-0.0.2/kivygo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 13:32:21.000000 kivygo-0.0.2/kivygo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-05-30 13:32:21.000000 kivygo-0.0.2/kivygo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-30 13:32:21.000000 kivygo-0.0.2/kivygo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-30 13:32:21.550452 kivygo-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2126 2023-05-30 13:06:22.000000 kivygo-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:34:44.618241 kivygo-0.0.3/
+-rw-rw-rw-   0        0        0     1098 2023-04-28 02:03:52.000000 kivygo-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      192 2023-05-30 13:34:44.618241 kivygo-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 13:34:44.394789 kivygo-0.0.3/kivygo/
+-rw-rw-rw-   0        0        0       23 2023-05-30 13:34:29.000000 kivygo-0.0.3/kivygo/__init__.py
+-rw-rw-rw-   0        0        0    23309 2023-05-13 18:28:10.000000 kivygo-0.0.3/kivygo/animation.py
+-rw-rw-rw-   0        0        0     2905 2023-05-13 17:09:56.000000 kivygo-0.0.3/kivygo/app.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:34:44.442788 kivygo-0.0.3/kivygo/behaviors/
+-rw-rw-rw-   0        0        0        0 2023-05-30 13:05:00.000000 kivygo-0.0.3/kivygo/behaviors/__init__.py
+-rw-rw-rw-   0        0        0     8273 2023-05-13 17:19:46.000000 kivygo-0.0.3/kivygo/behaviors/button.py
+-rw-rw-rw-   0        0        0     9872 2023-05-13 18:19:31.000000 kivygo-0.0.3/kivygo/behaviors/drag_and_drop.py
+-rw-rw-rw-   0        0        0     5825 2023-05-13 18:20:08.000000 kivygo-0.0.3/kivygo/behaviors/hover.py
+-rw-rw-rw-   0        0        0     3058 2023-05-05 22:06:08.000000 kivygo-0.0.3/kivygo/behaviors/neumorph.py
+-rw-rw-rw-   0        0        0    13342 2023-04-28 02:33:05.000000 kivygo-0.0.3/kivygo/behaviors/resizable.py
+-rw-rw-rw-   0        0        0    15085 2023-05-08 00:20:07.000000 kivygo-0.0.3/kivygo/behaviors/thumb.py
+-rw-rw-rw-   0        0        0     4375 2023-05-07 23:38:10.000000 kivygo-0.0.3/kivygo/behaviors/touch_effecs.py
+-rw-rw-rw-   0        0        0    16042 2023-05-01 21:00:44.000000 kivygo-0.0.3/kivygo/bounds_math.py
+-rw-rw-rw-   0        0        0     2375 2023-05-29 23:31:04.000000 kivygo-0.0.3/kivygo/colors.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:34:44.451799 kivygo-0.0.3/kivygo/config/
+-rw-rw-rw-   0        0        0      296 2023-04-30 03:08:38.000000 kivygo-0.0.3/kivygo/config/coins.atlas
+-rw-rw-rw-   0        0        0     4765 2023-04-29 21:48:35.000000 kivygo-0.0.3/kivygo/config/coins.bounds
+-rw-rw-rw-   0        0        0     1490 2013-02-26 10:24:28.000000 kivygo-0.0.3/kivygo/config/drugs.pex
+-rw-rw-rw-   0        0        0     1489 2013-02-26 10:24:28.000000 kivygo-0.0.3/kivygo/config/fire.pex
+-rw-rw-rw-   0        0        0     1496 2013-02-26 10:24:28.000000 kivygo-0.0.3/kivygo/config/jellyfish.pex
+-rw-rw-rw-   0        0        0     1463 2013-02-26 10:24:28.000000 kivygo-0.0.3/kivygo/config/particle.pex
+-rw-rw-rw-   0        0        0      870 2013-02-26 10:24:28.000000 kivygo-0.0.3/kivygo/config/particle.png
+-rw-rw-rw-   0        0        0     1494 2013-02-26 10:24:28.000000 kivygo-0.0.3/kivygo/config/sun.pex
+drwxrwxrwx   0        0        0        0 2023-05-30 13:34:44.454788 kivygo-0.0.3/kivygo/elevation/
+-rw-rw-rw-   0        0        0     1630 2023-01-06 02:24:33.000000 kivygo-0.0.3/kivygo/elevation/elevation.frag
+-rw-rw-rw-   0        0        0      198 2023-01-06 02:24:33.000000 kivygo-0.0.3/kivygo/elevation/header.frag
+-rw-rw-rw-   0        0        0      184 2023-01-06 02:24:33.000000 kivygo-0.0.3/kivygo/elevation/main.frag
+drwxrwxrwx   0        0        0        0 2023-05-30 13:34:44.479016 kivygo-0.0.3/kivygo/icons/
+-rw-rw-rw-   0        0        0   156742 2023-03-02 15:36:22.000000 kivygo-0.0.3/kivygo/icons/bg_example.png
+-rw-rw-rw-   0        0        0    95465 2022-05-23 02:23:22.000000 kivygo-0.0.3/kivygo/icons/coins.png
+-rw-rw-rw-   0        0        0     1244 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/discord.svg
+-rw-rw-rw-   0        0        0      781 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/discord2.svg
+-rw-rw-rw-   0        0        0      704 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/facebook2.svg
+-rw-rw-rw-   0        0        0     2453 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/github.svg
+-rw-rw-rw-   0        0        0     1864 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/github2.svg
+-rw-rw-rw-   0        0        0      829 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/github3.svg
+-rw-rw-rw-   0        0        0     2451 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/google.svg
+-rw-rw-rw-   0        0        0      990 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/google3.svg
+-rw-rw-rw-   0        0        0     2636 2022-05-23 02:23:22.000000 kivygo-0.0.3/kivygo/icons/kivy.png
+-rw-rw-rw-   0        0        0     1141 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/kivy.svg
+-rw-rw-rw-   0        0        0    16577 2023-03-02 15:36:22.000000 kivygo-0.0.3/kivygo/icons/kivy_logo.png
+-rw-rw-rw-   0        0        0    42074 2021-05-11 19:10:56.000000 kivygo-0.0.3/kivygo/icons/kivymd_logo.png
+-rw-rw-rw-   0        0        0     2919 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/pie_chart.svg
+-rw-rw-rw-   0        0        0     1458 2023-02-14 20:11:52.000000 kivygo-0.0.3/kivygo/icons/pipette.png
+-rw-rw-rw-   0        0        0     1133 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/python2.svg
+-rw-rw-rw-   0        0        0     1621 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/search.svg
+-rw-rw-rw-   0        0        0      851 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/so.svg
+-rw-rw-rw-   0        0        0     1481 2022-05-23 02:23:22.000000 kivygo-0.0.3/kivygo/icons/square.png
+-rw-rw-rw-   0        0        0     1814 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/sublime.svg
+-rw-rw-rw-   0        0        0     3454 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/text.svg
+-rw-rw-rw-   0        0        0     1928 2023-02-14 20:11:52.000000 kivygo-0.0.3/kivygo/icons/transparent.png
+-rw-rw-rw-   0        0        0     1086 2021-06-29 07:37:30.000000 kivygo-0.0.3/kivygo/icons/twitter2.svg
+drwxrwxrwx   0        0        0        0 2023-05-30 13:34:44.491015 kivygo-0.0.3/kivygo/images/
+-rw-rw-rw-   0        0        0   709001 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/images/busan.jpg
+-rw-rw-rw-   0        0        0   118790 2018-10-01 10:52:31.000000 kivygo-0.0.3/kivygo/images/demoimage.jpg
+-rw-rw-rw-   0        0        0   190380 2023-04-28 21:56:31.000000 kivygo-0.0.3/kivygo/images/icon-kivygo.png
+-rw-rw-rw-   0        0        0   431598 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/images/iris.jpg
+-rw-rw-rw-   0        0        0   857961 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/images/lion.jpg
+-rw-rw-rw-   0        0        0      879 2019-05-19 13:30:15.000000 kivygo-0.0.3/kivygo/images/navigationdrawer_gradient_ltor.png
+-rw-rw-rw-   0        0        0      874 2019-05-19 13:30:15.000000 kivygo-0.0.3/kivygo/images/navigationdrawer_gradient_rtol.png
+-rw-rw-rw-   0        0        0  1537713 2023-02-14 20:11:52.000000 kivygo-0.0.3/kivygo/images/test.jpg
+-rw-rw-rw-   0        0        0     2334 2023-04-21 01:53:43.000000 kivygo-0.0.3/kivygo/transformations.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:34:44.571773 kivygo-0.0.3/kivygo/transitions/
+-rw-rw-rw-   0        0        0      452 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Angular.glsl
+-rw-rw-rw-   0        0        0      719 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Bounce.glsl
+-rw-rw-rw-   0        0        0     2593 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/BowTieHorizontal.glsl
+-rw-rw-rw-   0        0        0     2541 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/BowTieVertical.glsl
+-rw-rw-rw-   0        0        0      231 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Burn.glsl
+-rw-rw-rw-   0        0        0      948 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/ButterflyWaveScrawler.glsl
+-rw-rw-rw-   0        0        0      485 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/CannabisLeaf.glsl
+-rw-rw-rw-   0        0        0      398 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Circle.glsl
+-rw-rw-rw-   0        0        0      386 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/CircleOpen.glsl
+-rw-rw-rw-   0        0        0      370 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/ColorPhase.glsl
+-rw-rw-rw-   0        0        0      353 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/ColourDistance.glsl
+-rw-rw-rw-   0        0        0      586 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/CrazyParametricFun.glsl
+-rw-rw-rw-   0        0        0      590 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/CrossHatch.glsl
+-rw-rw-rw-   0        0        0      228 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/CrossWarp.glsl
+-rw-rw-rw-   0        0        0     2385 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/CrossZoom.glsl
+-rw-rw-rw-   0        0        0     1694 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Cube.glsl
+-rw-rw-rw-   0        0        0      352 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/DirectionalEasing.glsl
+-rw-rw-rw-   0        0        0      489 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/DirectionalWarp.glsl
+-rw-rw-rw-   0        0        0      557 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/DirectionalWipe.glsl
+-rw-rw-rw-   0        0        0      522 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Displacement.glsl
+-rw-rw-rw-   0        0        0     1574 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/DoomScreenTransition.glsl
+-rw-rw-rw-   0        0        0     1189 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Doorway.glsl
+-rw-rw-rw-   0        0        0      378 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Dreamy.glsl
+-rw-rw-rw-   0        0        0     1183 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/DreamyZoom.glsl
+-rw-rw-rw-   0        0        0      136 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Fade.glsl
+-rw-rw-rw-   0        0        0      391 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/FadeColor.glsl
+-rw-rw-rw-   0        0        0      546 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/FadeGrayscale.glsl
+-rw-rw-rw-   0        0        0     2220 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/FilmBurn.glsl
+-rw-rw-rw-   0        0        0      489 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/FlyEye.glsl
+-rw-rw-rw-   0        0        0     2198 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/GlitchDisplace.glsl
+-rw-rw-rw-   0        0        0      607 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/GlitchMemories.glsl
+-rw-rw-rw-   0        0        0     2245 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/GridFlip.glsl
+-rw-rw-rw-   0        0        0      356 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Heart.glsl
+-rw-rw-rw-   0        0        0     1663 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Hexagonalize.glsl
+-rw-rw-rw-   0        0        0      549 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Kaleidoscope.glsl
+-rw-rw-rw-   0        0        0      647 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/LeftRight.glsl
+-rw-rw-rw-   0        0        0      671 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/LinearBlur.glsl
+-rw-rw-rw-   0        0        0      226 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Luma.glsl
+-rw-rw-rw-   0        0        0     3781 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/LuminanceMelt.glsl
+-rw-rw-rw-   0        0        0      379 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Morph.glsl
+-rw-rw-rw-   0        0        0     1105 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Mosaic.glsl
+-rw-rw-rw-   0        0        0      339 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/MultiplyBlend.glsl
+-rw-rw-rw-   0        0        0     1390 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/PageCurl.glsl
+-rw-rw-rw-   0        0        0     1367 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Perlin.glsl
+-rw-rw-rw-   0        0        0      349 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Pinwheel.glsl
+-rw-rw-rw-   0        0        0      562 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Pixelize.glsl
+-rw-rw-rw-   0        0        0      452 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/PolarFunction.glsl
+-rw-rw-rw-   0        0        0      304 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/PolkaDotsCurtain.glsl
+-rw-rw-rw-   0        0        0      353 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Radial.glsl
+-rw-rw-rw-   0        0        0      444 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/RandomNoise.glsl
+-rw-rw-rw-   0        0        0      377 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/RandomSquares.glsl
+-rw-rw-rw-   0        0        0      356 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Ripple.glsl
+-rw-rw-rw-   0        0        0      832 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/RotateScaleFade.glsl
+-rw-rw-rw-   0        0        0      348 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/RotateTransition.glsl
+-rw-rw-rw-   0        0        0      365 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/SimpleZoom.glsl
+-rw-rw-rw-   0        0        0      742 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/SquaresWire.glsl
+-rw-rw-rw-   0        0        0      444 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Squeeze.glsl
+-rw-rw-rw-   0        0        0     8033 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/StereoViewer.glsl
+-rw-rw-rw-   0        0        0     1506 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Swap.glsl
+-rw-rw-rw-   0        0        0      715 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Swirl.glsl
+-rw-rw-rw-   0        0        0     4051 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/TangentMotionBlur.glsl
+-rw-rw-rw-   0        0        0      650 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/TopBottom.glsl
+-rw-rw-rw-   0        0        0     1366 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/UndulatingBurnOut.glsl
+-rw-rw-rw-   0        0        0      409 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/WaterDrop.glsl
+-rw-rw-rw-   0        0        0      386 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/Wind.glsl
+-rw-rw-rw-   0        0        0      274 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/WindowBlinds.glsl
+-rw-rw-rw-   0        0        0      277 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/WindowSlice.glsl
+-rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/WipeDown.glsl
+-rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/WipeLeft.glsl
+-rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/WipeRight.glsl
+-rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/WipeUp.glsl
+-rw-rw-rw-   0        0        0     1115 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/ZoomInCircles.glsl
+-rw-rw-rw-   0        0        0     8072 2023-05-01 19:46:08.000000 kivygo-0.0.3/kivygo/transitions/__init__.py
+-rw-rw-rw-   0        0        0     1197 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/base.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:34:44.573751 kivygo-0.0.3/kivygo/transitions/extra/
+-rw-rw-rw-   0        0        0      177 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/extra/footer.glsl
+-rw-rw-rw-   0        0        0      403 2021-05-13 08:40:19.000000 kivygo-0.0.3/kivygo/transitions/extra/header.glsl
+drwxrwxrwx   0        0        0        0 2023-05-30 13:34:44.617243 kivygo-0.0.3/kivygo/uix/
+-rw-rw-rw-   0        0        0        0 2023-05-10 21:23:48.000000 kivygo-0.0.3/kivygo/uix/__init__.py
+-rw-rw-rw-   0        0        0     4809 2023-05-13 16:09:23.000000 kivygo-0.0.3/kivygo/uix/anchorlayout.py
+-rw-rw-rw-   0        0        0    13311 2023-05-13 18:19:00.000000 kivygo-0.0.3/kivygo/uix/androidtabs.py
+-rw-rw-rw-   0        0        0     3904 2023-05-10 20:13:58.000000 kivygo-0.0.3/kivygo/uix/bezier.py
+-rw-rw-rw-   0        0        0     2116 2023-05-03 13:52:13.000000 kivygo-0.0.3/kivygo/uix/boxlayout.py
+-rw-rw-rw-   0        0        0     4378 2023-05-13 17:20:58.000000 kivygo-0.0.3/kivygo/uix/button.py
+-rw-rw-rw-   0        0        0    12881 2023-04-28 02:33:05.000000 kivygo-0.0.3/kivygo/uix/camera.py
+-rw-rw-rw-   0        0        0     7833 2023-05-09 02:19:31.000000 kivygo-0.0.3/kivygo/uix/circular_bar.py
+-rw-rw-rw-   0        0        0    20660 2023-04-30 13:59:52.000000 kivygo-0.0.3/kivygo/uix/circulardatetimepicker.py
+-rw-rw-rw-   0        0        0     4640 2023-05-13 17:19:53.000000 kivygo-0.0.3/kivygo/uix/circularlayout.py
+-rw-rw-rw-   0        0        0    26840 2023-04-03 01:21:22.000000 kivygo-0.0.3/kivygo/uix/codeinput.py
+-rw-rw-rw-   0        0        0     4798 2023-04-28 02:33:05.000000 kivygo-0.0.3/kivygo/uix/curvelayout.py
+-rw-rw-rw-   0        0        0     1992 2023-04-25 21:55:26.000000 kivygo-0.0.3/kivygo/uix/effect.py
+-rw-rw-rw-   0        0        0      781 2023-04-28 02:33:05.000000 kivygo-0.0.3/kivygo/uix/floatlayout.py
+-rw-rw-rw-   0        0        0    21770 2023-05-13 17:19:58.000000 kivygo-0.0.3/kivygo/uix/frostedglass.py
+-rw-rw-rw-   0        0        0     2380 2023-05-10 20:29:00.000000 kivygo-0.0.3/kivygo/uix/gradient.py
+-rw-rw-rw-   0        0        0     2746 2023-05-08 15:57:00.000000 kivygo-0.0.3/kivygo/uix/gridlayout.py
+-rw-rw-rw-   0        0        0     4910 2023-04-28 02:33:05.000000 kivygo-0.0.3/kivygo/uix/icon.py
+-rw-rw-rw-   0        0        0     2644 2023-03-28 18:29:30.000000 kivygo-0.0.3/kivygo/uix/image.py
+-rw-rw-rw-   0        0        0    10992 2023-05-13 17:22:37.000000 kivygo-0.0.3/kivygo/uix/input.py
+-rw-rw-rw-   0        0        0     9444 2023-05-13 17:22:37.000000 kivygo-0.0.3/kivygo/uix/joystick.py
+-rw-rw-rw-   0        0        0    21810 2023-05-10 20:33:34.000000 kivygo-0.0.3/kivygo/uix/kivyg_icon.py
+-rw-rw-rw-   0        0        0     9082 2023-05-13 17:20:07.000000 kivygo-0.0.3/kivygo/uix/label.py
+-rw-rw-rw-   0        0        0    14052 2023-05-13 17:20:10.000000 kivygo-0.0.3/kivygo/uix/navigationdrawer.py
+-rw-rw-rw-   0        0        0    18174 2023-05-13 18:19:28.000000 kivygo-0.0.3/kivygo/uix/particle.py
+-rw-rw-rw-   0        0        0     4457 2023-05-10 20:44:55.000000 kivygo-0.0.3/kivygo/uix/pizza_graph.py
+-rw-rw-rw-   0        0        0     2807 2023-04-28 02:33:05.000000 kivygo-0.0.3/kivygo/uix/popup.py
+-rw-rw-rw-   0        0        0     6764 2023-05-13 17:20:13.000000 kivygo-0.0.3/kivygo/uix/progressspinner.py
+-rw-rw-rw-   0        0        0     6807 2023-05-13 18:19:05.000000 kivygo-0.0.3/kivygo/uix/radialslider.py
+-rw-rw-rw-   0        0        0    24325 2023-05-10 20:56:39.000000 kivygo-0.0.3/kivygo/uix/rotabox.py
+-rw-rw-rw-   0        0        0     1408 2023-04-06 21:24:34.000000 kivygo-0.0.3/kivygo/uix/screenmanager.py
+-rw-rw-rw-   0        0        0     3598 2023-05-13 18:19:11.000000 kivygo-0.0.3/kivygo/uix/scrollview.py
+-rw-rw-rw-   0        0        0     4990 2023-05-01 16:18:58.000000 kivygo-0.0.3/kivygo/uix/segment.py
+-rw-rw-rw-   0        0        0     2959 2023-05-10 20:57:52.000000 kivygo-0.0.3/kivygo/uix/shader.py
+-rw-rw-rw-   0        0        0     2858 2023-05-13 18:19:17.000000 kivygo-0.0.3/kivygo/uix/simpletablelayout.py
+-rw-rw-rw-   0        0        0     5517 2023-05-05 22:56:03.000000 kivygo-0.0.3/kivygo/uix/slider.py
+-rw-rw-rw-   0        0        0     4389 2023-05-10 21:19:13.000000 kivygo-0.0.3/kivygo/uix/spinner.py
+-rw-rw-rw-   0        0        0    12722 2023-03-28 18:29:55.000000 kivygo-0.0.3/kivygo/uix/taptargetview.py
+-rw-rw-rw-   0        0        0     6436 2023-05-13 17:20:20.000000 kivygo-0.0.3/kivygo/uix/terminal.py
+-rw-rw-rw-   0        0        0     3601 2023-05-04 01:11:32.000000 kivygo-0.0.3/kivygo/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:34:44.431789 kivygo-0.0.3/kivygo.egg-info/
+-rw-rw-rw-   0        0        0      192 2023-05-30 13:34:44.000000 kivygo-0.0.3/kivygo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5310 2023-05-30 13:34:44.000000 kivygo-0.0.3/kivygo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 13:34:44.000000 kivygo-0.0.3/kivygo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-05-30 13:34:44.000000 kivygo-0.0.3/kivygo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 13:34:44.000000 kivygo-0.0.3/kivygo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-30 13:34:44.619240 kivygo-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2126 2023-05-30 13:06:22.000000 kivygo-0.0.3/setup.py
```

### Comparing `kivygo-0.0.2/LICENSE.txt` & `kivygo-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/animation.py` & `kivygo-0.0.3/kivygo/animation.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/app.py` & `kivygo-0.0.3/kivygo/app.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/behaviors/button.py` & `kivygo-0.0.3/kivygo/behaviors/button.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/behaviors/drag_and_drop.py` & `kivygo-0.0.3/kivygo/behaviors/drag_and_drop.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/behaviors/hover.py` & `kivygo-0.0.3/kivygo/behaviors/hover.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/behaviors/neumorph.py` & `kivygo-0.0.3/kivygo/behaviors/neumorph.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/behaviors/resizable.py` & `kivygo-0.0.3/kivygo/behaviors/resizable.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/behaviors/thumb.py` & `kivygo-0.0.3/kivygo/behaviors/thumb.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/behaviors/touch_effecs.py` & `kivygo-0.0.3/kivygo/behaviors/touch_effecs.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/bounds_math.py` & `kivygo-0.0.3/kivygo/bounds_math.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/colors.py` & `kivygo-0.0.3/kivygo/colors.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/config/coins.bounds` & `kivygo-0.0.3/kivygo/config/coins.bounds`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/config/drugs.pex` & `kivygo-0.0.3/kivygo/config/drugs.pex`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/config/fire.pex` & `kivygo-0.0.3/kivygo/config/fire.pex`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/config/jellyfish.pex` & `kivygo-0.0.3/kivygo/config/jellyfish.pex`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/config/particle.pex` & `kivygo-0.0.3/kivygo/config/particle.pex`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/config/particle.png` & `kivygo-0.0.3/kivygo/config/particle.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/config/sun.pex` & `kivygo-0.0.3/kivygo/config/sun.pex`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/elevation/elevation.frag` & `kivygo-0.0.3/kivygo/elevation/elevation.frag`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/bg_example.png` & `kivygo-0.0.3/kivygo/icons/bg_example.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/coins.png` & `kivygo-0.0.3/kivygo/icons/coins.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/discord.svg` & `kivygo-0.0.3/kivygo/icons/discord.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/discord2.svg` & `kivygo-0.0.3/kivygo/icons/discord2.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/facebook2.svg` & `kivygo-0.0.3/kivygo/icons/facebook2.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/github.svg` & `kivygo-0.0.3/kivygo/icons/github.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/github2.svg` & `kivygo-0.0.3/kivygo/icons/github2.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/github3.svg` & `kivygo-0.0.3/kivygo/icons/github3.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/google.svg` & `kivygo-0.0.3/kivygo/icons/google.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/google3.svg` & `kivygo-0.0.3/kivygo/icons/google3.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/kivy.png` & `kivygo-0.0.3/kivygo/icons/kivy.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/kivy.svg` & `kivygo-0.0.3/kivygo/icons/kivy.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/kivy_logo.png` & `kivygo-0.0.3/kivygo/icons/kivy_logo.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/kivymd_logo.png` & `kivygo-0.0.3/kivygo/icons/kivymd_logo.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/pie_chart.svg` & `kivygo-0.0.3/kivygo/icons/pie_chart.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/pipette.png` & `kivygo-0.0.3/kivygo/icons/pipette.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/python2.svg` & `kivygo-0.0.3/kivygo/icons/python2.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/search.svg` & `kivygo-0.0.3/kivygo/icons/search.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/so.svg` & `kivygo-0.0.3/kivygo/icons/so.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/square.png` & `kivygo-0.0.3/kivygo/icons/square.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/sublime.svg` & `kivygo-0.0.3/kivygo/icons/sublime.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/text.svg` & `kivygo-0.0.3/kivygo/icons/text.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/transparent.png` & `kivygo-0.0.3/kivygo/icons/transparent.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/icons/twitter2.svg` & `kivygo-0.0.3/kivygo/icons/twitter2.svg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/images/busan.jpg` & `kivygo-0.0.3/kivygo/images/busan.jpg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/images/demoimage.jpg` & `kivygo-0.0.3/kivygo/images/demoimage.jpg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/images/icon-kivygo.png` & `kivygo-0.0.3/kivygo/images/icon-kivygo.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/images/iris.jpg` & `kivygo-0.0.3/kivygo/images/iris.jpg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/images/lion.jpg` & `kivygo-0.0.3/kivygo/images/lion.jpg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/images/navigationdrawer_gradient_ltor.png` & `kivygo-0.0.3/kivygo/images/navigationdrawer_gradient_ltor.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/images/navigationdrawer_gradient_rtol.png` & `kivygo-0.0.3/kivygo/images/navigationdrawer_gradient_rtol.png`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/images/test.jpg` & `kivygo-0.0.3/kivygo/images/test.jpg`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transformations.py` & `kivygo-0.0.3/kivygo/transformations.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/Bounce.glsl` & `kivygo-0.0.3/kivygo/transitions/Bounce.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/BowTieHorizontal.glsl` & `kivygo-0.0.3/kivygo/transitions/BowTieHorizontal.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/BowTieVertical.glsl` & `kivygo-0.0.3/kivygo/transitions/BowTieVertical.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/ButterflyWaveScrawler.glsl` & `kivygo-0.0.3/kivygo/transitions/ButterflyWaveScrawler.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/CrazyParametricFun.glsl` & `kivygo-0.0.3/kivygo/transitions/CrazyParametricFun.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/CrossHatch.glsl` & `kivygo-0.0.3/kivygo/transitions/CrossHatch.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/CrossZoom.glsl` & `kivygo-0.0.3/kivygo/transitions/CrossZoom.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/Cube.glsl` & `kivygo-0.0.3/kivygo/transitions/Cube.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/DirectionalWipe.glsl` & `kivygo-0.0.3/kivygo/transitions/DirectionalWipe.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/Displacement.glsl` & `kivygo-0.0.3/kivygo/transitions/Displacement.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/DoomScreenTransition.glsl` & `kivygo-0.0.3/kivygo/transitions/DoomScreenTransition.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/Doorway.glsl` & `kivygo-0.0.3/kivygo/transitions/Doorway.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/DreamyZoom.glsl` & `kivygo-0.0.3/kivygo/transitions/DreamyZoom.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/FadeGrayscale.glsl` & `kivygo-0.0.3/kivygo/transitions/FadeGrayscale.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/FilmBurn.glsl` & `kivygo-0.0.3/kivygo/transitions/FilmBurn.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/GlitchDisplace.glsl` & `kivygo-0.0.3/kivygo/transitions/GlitchDisplace.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/GlitchMemories.glsl` & `kivygo-0.0.3/kivygo/transitions/GlitchMemories.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/GridFlip.glsl` & `kivygo-0.0.3/kivygo/transitions/GridFlip.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/Hexagonalize.glsl` & `kivygo-0.0.3/kivygo/transitions/Hexagonalize.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/Kaleidoscope.glsl` & `kivygo-0.0.3/kivygo/transitions/Kaleidoscope.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/LeftRight.glsl` & `kivygo-0.0.3/kivygo/transitions/LeftRight.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/LinearBlur.glsl` & `kivygo-0.0.3/kivygo/transitions/LinearBlur.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/LuminanceMelt.glsl` & `kivygo-0.0.3/kivygo/transitions/LuminanceMelt.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/Mosaic.glsl` & `kivygo-0.0.3/kivygo/transitions/Mosaic.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/PageCurl.glsl` & `kivygo-0.0.3/kivygo/transitions/PageCurl.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/Perlin.glsl` & `kivygo-0.0.3/kivygo/transitions/Perlin.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/Pixelize.glsl` & `kivygo-0.0.3/kivygo/transitions/Pixelize.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/RotateScaleFade.glsl` & `kivygo-0.0.3/kivygo/transitions/RotateScaleFade.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/SquaresWire.glsl` & `kivygo-0.0.3/kivygo/transitions/SquaresWire.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/StereoViewer.glsl` & `kivygo-0.0.3/kivygo/transitions/StereoViewer.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/Swap.glsl` & `kivygo-0.0.3/kivygo/transitions/Swap.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/Swirl.glsl` & `kivygo-0.0.3/kivygo/transitions/Swirl.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/TangentMotionBlur.glsl` & `kivygo-0.0.3/kivygo/transitions/TangentMotionBlur.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/TopBottom.glsl` & `kivygo-0.0.3/kivygo/transitions/TopBottom.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/UndulatingBurnOut.glsl` & `kivygo-0.0.3/kivygo/transitions/UndulatingBurnOut.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/ZoomInCircles.glsl` & `kivygo-0.0.3/kivygo/transitions/ZoomInCircles.glsl`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/__init__.py` & `kivygo-0.0.3/kivygo/transitions/__init__.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/transitions/base.py` & `kivygo-0.0.3/kivygo/transitions/base.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/kivygo/utils.py` & `kivygo-0.0.3/kivygo/utils.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.2/setup.py` & `kivygo-0.0.3/setup.py`

 * *Files identical despite different names*

