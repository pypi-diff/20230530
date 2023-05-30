# Comparing `tmp/kivygo-0.0.1.tar.gz` & `tmp/kivygo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivygo-0.0.1.tar", last modified: Tue May 30 12:41:59 2023, max compression
+gzip compressed data, was "kivygo-0.0.2.tar", last modified: Tue May 30 13:32:21 2023, max compression
```

## Comparing `kivygo-0.0.1.tar` & `kivygo-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,153 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 12:41:59.026975 kivygo-0.0.1/
--rw-rw-rw-   0        0        0     1098 2023-04-28 02:03:52.000000 kivygo-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      192 2023-05-30 12:41:59.026975 kivygo-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 12:41:58.970362 kivygo-0.0.1/kivygo/
--rw-rw-rw-   0        0        0       23 2023-05-30 12:40:45.000000 kivygo-0.0.1/kivygo/__init__.py
--rw-rw-rw-   0        0        0    23309 2023-05-13 18:28:10.000000 kivygo-0.0.1/kivygo/animation.py
--rw-rw-rw-   0        0        0     2905 2023-05-13 17:09:56.000000 kivygo-0.0.1/kivygo/app.py
--rw-rw-rw-   0        0        0    16042 2023-05-01 21:00:44.000000 kivygo-0.0.1/kivygo/bounds_math.py
--rw-rw-rw-   0        0        0     2375 2023-05-29 23:31:04.000000 kivygo-0.0.1/kivygo/colors.py
--rw-rw-rw-   0        0        0     2334 2023-04-21 01:53:43.000000 kivygo-0.0.1/kivygo/transformations.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:41:59.025976 kivygo-0.0.1/kivygo/transitions/
--rw-rw-rw-   0        0        0     8072 2023-05-01 19:46:08.000000 kivygo-0.0.1/kivygo/transitions/__init__.py
--rw-rw-rw-   0        0        0     1197 2021-05-13 08:40:19.000000 kivygo-0.0.1/kivygo/transitions/base.py
--rw-rw-rw-   0        0        0     3601 2023-05-04 01:11:32.000000 kivygo-0.0.1/kivygo/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:41:59.009975 kivygo-0.0.1/kivygo.egg-info/
--rw-rw-rw-   0        0        0      192 2023-05-30 12:41:58.000000 kivygo-0.0.1/kivygo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-05-30 12:41:58.000000 kivygo-0.0.1/kivygo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 12:41:58.000000 kivygo-0.0.1/kivygo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-05-30 12:41:58.000000 kivygo-0.0.1/kivygo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-30 12:41:58.000000 kivygo-0.0.1/kivygo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-30 12:41:59.028979 kivygo-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1888 2023-05-30 12:41:52.000000 kivygo-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.546431 kivygo-0.0.2/
+-rw-rw-rw-   0        0        0     1098 2023-04-28 02:03:52.000000 kivygo-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      192 2023-05-30 13:32:21.546431 kivygo-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.356984 kivygo-0.0.2/kivygo/
+-rw-rw-rw-   0        0        0       23 2023-05-30 13:32:16.000000 kivygo-0.0.2/kivygo/__init__.py
+-rw-rw-rw-   0        0        0    23309 2023-05-13 18:28:10.000000 kivygo-0.0.2/kivygo/animation.py
+-rw-rw-rw-   0        0        0     2905 2023-05-13 17:09:56.000000 kivygo-0.0.2/kivygo/app.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.408141 kivygo-0.0.2/kivygo/behaviors/
+-rw-rw-rw-   0        0        0        0 2023-05-30 13:05:00.000000 kivygo-0.0.2/kivygo/behaviors/__init__.py
+-rw-rw-rw-   0        0        0     8273 2023-05-13 17:19:46.000000 kivygo-0.0.2/kivygo/behaviors/button.py
+-rw-rw-rw-   0        0        0     9872 2023-05-13 18:19:31.000000 kivygo-0.0.2/kivygo/behaviors/drag_and_drop.py
+-rw-rw-rw-   0        0        0     5825 2023-05-13 18:20:08.000000 kivygo-0.0.2/kivygo/behaviors/hover.py
+-rw-rw-rw-   0        0        0     3058 2023-05-05 22:06:08.000000 kivygo-0.0.2/kivygo/behaviors/neumorph.py
+-rw-rw-rw-   0        0        0    13342 2023-04-28 02:33:05.000000 kivygo-0.0.2/kivygo/behaviors/resizable.py
+-rw-rw-rw-   0        0        0    15085 2023-05-08 00:20:07.000000 kivygo-0.0.2/kivygo/behaviors/thumb.py
+-rw-rw-rw-   0        0        0     4375 2023-05-07 23:38:10.000000 kivygo-0.0.2/kivygo/behaviors/touch_effecs.py
+-rw-rw-rw-   0        0        0    16042 2023-05-01 21:00:44.000000 kivygo-0.0.2/kivygo/bounds_math.py
+-rw-rw-rw-   0        0        0     2375 2023-05-29 23:31:04.000000 kivygo-0.0.2/kivygo/colors.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.417144 kivygo-0.0.2/kivygo/config/
+-rw-rw-rw-   0        0        0      296 2023-04-30 03:08:38.000000 kivygo-0.0.2/kivygo/config/coins.atlas
+-rw-rw-rw-   0        0        0     4765 2023-04-29 21:48:35.000000 kivygo-0.0.2/kivygo/config/coins.bounds
+-rw-rw-rw-   0        0        0     1490 2013-02-26 10:24:28.000000 kivygo-0.0.2/kivygo/config/drugs.pex
+-rw-rw-rw-   0        0        0     1489 2013-02-26 10:24:28.000000 kivygo-0.0.2/kivygo/config/fire.pex
+-rw-rw-rw-   0        0        0     1496 2013-02-26 10:24:28.000000 kivygo-0.0.2/kivygo/config/jellyfish.pex
+-rw-rw-rw-   0        0        0     1463 2013-02-26 10:24:28.000000 kivygo-0.0.2/kivygo/config/particle.pex
+-rw-rw-rw-   0        0        0      870 2013-02-26 10:24:28.000000 kivygo-0.0.2/kivygo/config/particle.png
+-rw-rw-rw-   0        0        0     1494 2013-02-26 10:24:28.000000 kivygo-0.0.2/kivygo/config/sun.pex
+drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.420145 kivygo-0.0.2/kivygo/elevation/
+-rw-rw-rw-   0        0        0     1630 2023-01-06 02:24:33.000000 kivygo-0.0.2/kivygo/elevation/elevation.frag
+-rw-rw-rw-   0        0        0      198 2023-01-06 02:24:33.000000 kivygo-0.0.2/kivygo/elevation/header.frag
+-rw-rw-rw-   0        0        0      184 2023-01-06 02:24:33.000000 kivygo-0.0.2/kivygo/elevation/main.frag
+drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.448568 kivygo-0.0.2/kivygo/icons/
+-rw-rw-rw-   0        0        0   156742 2023-03-02 15:36:22.000000 kivygo-0.0.2/kivygo/icons/bg_example.png
+-rw-rw-rw-   0        0        0    95465 2022-05-23 02:23:22.000000 kivygo-0.0.2/kivygo/icons/coins.png
+-rw-rw-rw-   0        0        0     1244 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/discord.svg
+-rw-rw-rw-   0        0        0      781 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/discord2.svg
+-rw-rw-rw-   0        0        0      704 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/facebook2.svg
+-rw-rw-rw-   0        0        0     2453 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/github.svg
+-rw-rw-rw-   0        0        0     1864 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/github2.svg
+-rw-rw-rw-   0        0        0      829 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/github3.svg
+-rw-rw-rw-   0        0        0     2451 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/google.svg
+-rw-rw-rw-   0        0        0      990 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/google3.svg
+-rw-rw-rw-   0        0        0     2636 2022-05-23 02:23:22.000000 kivygo-0.0.2/kivygo/icons/kivy.png
+-rw-rw-rw-   0        0        0     1141 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/kivy.svg
+-rw-rw-rw-   0        0        0    16577 2023-03-02 15:36:22.000000 kivygo-0.0.2/kivygo/icons/kivy_logo.png
+-rw-rw-rw-   0        0        0    42074 2021-05-11 19:10:56.000000 kivygo-0.0.2/kivygo/icons/kivymd_logo.png
+-rw-rw-rw-   0        0        0     2919 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/pie_chart.svg
+-rw-rw-rw-   0        0        0     1458 2023-02-14 20:11:52.000000 kivygo-0.0.2/kivygo/icons/pipette.png
+-rw-rw-rw-   0        0        0     1133 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/python2.svg
+-rw-rw-rw-   0        0        0     1621 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/search.svg
+-rw-rw-rw-   0        0        0      851 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/so.svg
+-rw-rw-rw-   0        0        0     1481 2022-05-23 02:23:22.000000 kivygo-0.0.2/kivygo/icons/square.png
+-rw-rw-rw-   0        0        0     1814 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/sublime.svg
+-rw-rw-rw-   0        0        0     3454 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/text.svg
+-rw-rw-rw-   0        0        0     1928 2023-02-14 20:11:52.000000 kivygo-0.0.2/kivygo/icons/transparent.png
+-rw-rw-rw-   0        0        0     1086 2021-06-29 07:37:30.000000 kivygo-0.0.2/kivygo/icons/twitter2.svg
+drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.461541 kivygo-0.0.2/kivygo/images/
+-rw-rw-rw-   0        0        0   709001 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/images/busan.jpg
+-rw-rw-rw-   0        0        0   118790 2018-10-01 10:52:31.000000 kivygo-0.0.2/kivygo/images/demoimage.jpg
+-rw-rw-rw-   0        0        0   190380 2023-04-28 21:56:31.000000 kivygo-0.0.2/kivygo/images/icon-kivygo.png
+-rw-rw-rw-   0        0        0   431598 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/images/iris.jpg
+-rw-rw-rw-   0        0        0   857961 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/images/lion.jpg
+-rw-rw-rw-   0        0        0      879 2019-05-19 13:30:15.000000 kivygo-0.0.2/kivygo/images/navigationdrawer_gradient_ltor.png
+-rw-rw-rw-   0        0        0      874 2019-05-19 13:30:15.000000 kivygo-0.0.2/kivygo/images/navigationdrawer_gradient_rtol.png
+-rw-rw-rw-   0        0        0  1537713 2023-02-14 20:11:52.000000 kivygo-0.0.2/kivygo/images/test.jpg
+-rw-rw-rw-   0        0        0     2334 2023-04-21 01:53:43.000000 kivygo-0.0.2/kivygo/transformations.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.543436 kivygo-0.0.2/kivygo/transitions/
+-rw-rw-rw-   0        0        0      452 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Angular.glsl
+-rw-rw-rw-   0        0        0      719 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Bounce.glsl
+-rw-rw-rw-   0        0        0     2593 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/BowTieHorizontal.glsl
+-rw-rw-rw-   0        0        0     2541 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/BowTieVertical.glsl
+-rw-rw-rw-   0        0        0      231 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Burn.glsl
+-rw-rw-rw-   0        0        0      948 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/ButterflyWaveScrawler.glsl
+-rw-rw-rw-   0        0        0      485 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/CannabisLeaf.glsl
+-rw-rw-rw-   0        0        0      398 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Circle.glsl
+-rw-rw-rw-   0        0        0      386 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/CircleOpen.glsl
+-rw-rw-rw-   0        0        0      370 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/ColorPhase.glsl
+-rw-rw-rw-   0        0        0      353 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/ColourDistance.glsl
+-rw-rw-rw-   0        0        0      586 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/CrazyParametricFun.glsl
+-rw-rw-rw-   0        0        0      590 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/CrossHatch.glsl
+-rw-rw-rw-   0        0        0      228 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/CrossWarp.glsl
+-rw-rw-rw-   0        0        0     2385 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/CrossZoom.glsl
+-rw-rw-rw-   0        0        0     1694 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Cube.glsl
+-rw-rw-rw-   0        0        0      352 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/DirectionalEasing.glsl
+-rw-rw-rw-   0        0        0      489 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/DirectionalWarp.glsl
+-rw-rw-rw-   0        0        0      557 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/DirectionalWipe.glsl
+-rw-rw-rw-   0        0        0      522 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Displacement.glsl
+-rw-rw-rw-   0        0        0     1574 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/DoomScreenTransition.glsl
+-rw-rw-rw-   0        0        0     1189 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Doorway.glsl
+-rw-rw-rw-   0        0        0      378 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Dreamy.glsl
+-rw-rw-rw-   0        0        0     1183 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/DreamyZoom.glsl
+-rw-rw-rw-   0        0        0      136 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Fade.glsl
+-rw-rw-rw-   0        0        0      391 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/FadeColor.glsl
+-rw-rw-rw-   0        0        0      546 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/FadeGrayscale.glsl
+-rw-rw-rw-   0        0        0     2220 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/FilmBurn.glsl
+-rw-rw-rw-   0        0        0      489 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/FlyEye.glsl
+-rw-rw-rw-   0        0        0     2198 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/GlitchDisplace.glsl
+-rw-rw-rw-   0        0        0      607 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/GlitchMemories.glsl
+-rw-rw-rw-   0        0        0     2245 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/GridFlip.glsl
+-rw-rw-rw-   0        0        0      356 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Heart.glsl
+-rw-rw-rw-   0        0        0     1663 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Hexagonalize.glsl
+-rw-rw-rw-   0        0        0      549 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Kaleidoscope.glsl
+-rw-rw-rw-   0        0        0      647 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/LeftRight.glsl
+-rw-rw-rw-   0        0        0      671 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/LinearBlur.glsl
+-rw-rw-rw-   0        0        0      226 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Luma.glsl
+-rw-rw-rw-   0        0        0     3781 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/LuminanceMelt.glsl
+-rw-rw-rw-   0        0        0      379 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Morph.glsl
+-rw-rw-rw-   0        0        0     1105 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Mosaic.glsl
+-rw-rw-rw-   0        0        0      339 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/MultiplyBlend.glsl
+-rw-rw-rw-   0        0        0     1390 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/PageCurl.glsl
+-rw-rw-rw-   0        0        0     1367 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Perlin.glsl
+-rw-rw-rw-   0        0        0      349 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Pinwheel.glsl
+-rw-rw-rw-   0        0        0      562 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Pixelize.glsl
+-rw-rw-rw-   0        0        0      452 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/PolarFunction.glsl
+-rw-rw-rw-   0        0        0      304 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/PolkaDotsCurtain.glsl
+-rw-rw-rw-   0        0        0      353 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Radial.glsl
+-rw-rw-rw-   0        0        0      444 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/RandomNoise.glsl
+-rw-rw-rw-   0        0        0      377 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/RandomSquares.glsl
+-rw-rw-rw-   0        0        0      356 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Ripple.glsl
+-rw-rw-rw-   0        0        0      832 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/RotateScaleFade.glsl
+-rw-rw-rw-   0        0        0      348 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/RotateTransition.glsl
+-rw-rw-rw-   0        0        0      365 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/SimpleZoom.glsl
+-rw-rw-rw-   0        0        0      742 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/SquaresWire.glsl
+-rw-rw-rw-   0        0        0      444 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Squeeze.glsl
+-rw-rw-rw-   0        0        0     8033 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/StereoViewer.glsl
+-rw-rw-rw-   0        0        0     1506 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Swap.glsl
+-rw-rw-rw-   0        0        0      715 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Swirl.glsl
+-rw-rw-rw-   0        0        0     4051 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/TangentMotionBlur.glsl
+-rw-rw-rw-   0        0        0      650 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/TopBottom.glsl
+-rw-rw-rw-   0        0        0     1366 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/UndulatingBurnOut.glsl
+-rw-rw-rw-   0        0        0      409 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WaterDrop.glsl
+-rw-rw-rw-   0        0        0      386 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/Wind.glsl
+-rw-rw-rw-   0        0        0      274 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WindowBlinds.glsl
+-rw-rw-rw-   0        0        0      277 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WindowSlice.glsl
+-rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WipeDown.glsl
+-rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WipeLeft.glsl
+-rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WipeRight.glsl
+-rw-rw-rw-   0        0        0      192 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/WipeUp.glsl
+-rw-rw-rw-   0        0        0     1115 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/ZoomInCircles.glsl
+-rw-rw-rw-   0        0        0     8072 2023-05-01 19:46:08.000000 kivygo-0.0.2/kivygo/transitions/__init__.py
+-rw-rw-rw-   0        0        0     1197 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/base.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.545428 kivygo-0.0.2/kivygo/transitions/extra/
+-rw-rw-rw-   0        0        0      177 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/extra/footer.glsl
+-rw-rw-rw-   0        0        0      403 2021-05-13 08:40:19.000000 kivygo-0.0.2/kivygo/transitions/extra/header.glsl
+-rw-rw-rw-   0        0        0     3601 2023-05-04 01:11:32.000000 kivygo-0.0.2/kivygo/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:32:21.398194 kivygo-0.0.2/kivygo.egg-info/
+-rw-rw-rw-   0        0        0      192 2023-05-30 13:32:21.000000 kivygo-0.0.2/kivygo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4354 2023-05-30 13:32:21.000000 kivygo-0.0.2/kivygo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 13:32:21.000000 kivygo-0.0.2/kivygo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-05-30 13:32:21.000000 kivygo-0.0.2/kivygo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 13:32:21.000000 kivygo-0.0.2/kivygo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-30 13:32:21.550452 kivygo-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2126 2023-05-30 13:06:22.000000 kivygo-0.0.2/setup.py
```

### Comparing `kivygo-0.0.1/LICENSE.txt` & `kivygo-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.1/kivygo/animation.py` & `kivygo-0.0.2/kivygo/animation.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.1/kivygo/app.py` & `kivygo-0.0.2/kivygo/app.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.1/kivygo/bounds_math.py` & `kivygo-0.0.2/kivygo/bounds_math.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.1/kivygo/colors.py` & `kivygo-0.0.2/kivygo/colors.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.1/kivygo/transformations.py` & `kivygo-0.0.2/kivygo/transformations.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.1/kivygo/transitions/__init__.py` & `kivygo-0.0.2/kivygo/transitions/__init__.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.1/kivygo/transitions/base.py` & `kivygo-0.0.2/kivygo/transitions/base.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.1/kivygo/utils.py` & `kivygo-0.0.2/kivygo/utils.py`

 * *Files identical despite different names*

### Comparing `kivygo-0.0.1/setup.py` & `kivygo-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -39,18 +39,24 @@
     setup(
         name="kivygo",
         version = get_version(),
         packages = find_packages(include=["kivygo", "kivygo.*"]),
         package_dir = {"kivygo": "kivygo"},
         package_data={
             "kivygo": [
-                "assets/images/*.png",
-                "assets/icons/*.png",
-                "fonts/*.ttf",
+                *glob_paths(".png"),
+                *glob_paths(".jpg"),
+                *glob_paths(".svg"),
+                *glob_paths(".ttf"),
                 *glob_paths(".kv"),
+                *glob_paths(".frag"),
+                *glob_paths(".glsl"),
+                *glob_paths(".atlas"),
+                *glob_paths(".pex"),
+                *glob_paths(".bounds"),
             ]
         },
         install_requires=[
             "kivy>=2.0.0", "pillow",
             "opencv-python", "camera4kivy",
             "matplotlib", "pyzbar",
             "requests", "svglib"
```

