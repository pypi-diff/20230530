# Comparing `tmp/rtc-tools-channel-flow-1.1.1rc1.tar.gz` & `tmp/rtc-tools-channel-flow-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rtc-tools-channel-flow-1.1.1rc1.tar", last modified: Tue Feb 21 10:29:18 2023, max compression
+gzip compressed data, was "dist/rtc-tools-channel-flow-1.1.2.tar", last modified: Tue May 30 09:09:09 2023, max compression
```

## Comparing `rtc-tools-channel-flow-1.1.1rc1.tar` & `rtc-tools-channel-flow-1.1.2.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/
--rw-r--r--   0 root         (0) root         (0)      985 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtc_tools_channel_flow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      985 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtc_tools_channel_flow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10350 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtc_tools_channel_flow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtc_tools_channel_flow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtc_tools_channel_flow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtc_tools_channel_flow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtc_tools_channel_flow.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/
--rw-r--r--   0 root         (0) root         (0)      500 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/_version.py
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/Constants.mo
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/package.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/HQToQOut.mo
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/QInToHQ.mo
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/package.order
--rw-rw-rw-   0 root         (0) root         (0)      671 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/HQPort.mo
--rw-rw-rw-   0 root         (0) root         (0)      736 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/HQCMPort.mo
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/QOutPort.mo
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/package.mo
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/QInPort.mo
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/package.order
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/SmoothMax.mo
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/SmoothSwitch.mo
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/SmoothAbs.mo
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/package.order
--rw-rw-rw-   0 root         (0) root         (0)      362 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/SmoothMin.mo
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QForcing.mo
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/HQOnePort.mo
--rw-rw-rw-   0 root         (0) root         (0)     1215 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/HQTwoPort.mo
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QSI.mo
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QLateral.mo
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Reservoir.mo
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QSISO.mo
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/package.mo
--rw-rw-rw-   0 root         (0) root         (0)      315 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Volume.mo
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/package.order
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QSO.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Media/
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Media/SalineWater.mo
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Media/FreshWater.mo
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Media/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Media/package.order
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/
--rw-rw-rw-   0 root         (0) root         (0)      606 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/Level.mo
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/Discharge.mo
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/package.order
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/HomotopicLinear.mo
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Linear.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Internal/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Internal/package.mo
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Internal/BottomFrictionCoefficient.mo
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Internal/package.order
--rw-rw-rw-   0 root         (0) root         (0)    11063 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Internal/PartialHomotopic.mo
--rw-rw-rw-   0 root         (0) root         (0)     3175 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/HomotopicTrapezoidal.mo
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/package.order
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/Linear.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/Internal/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/Internal/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/Internal/package.order
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/Internal/PartialStorage.mo
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/package.order
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Structures/
--rw-rw-rw-   0 root         (0) root         (0)     1448 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Structures/DischargeControlledStructure.mo
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Structures/Pump.mo
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Structures/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Structures/package.order
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/package.order
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/Linear.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/Internal/
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/Internal/PartialReservoir.mo
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/Internal/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/Internal/package.order
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/package.order
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/package.order
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/BoundaryConditions/
--rw-rw-rw-   0 root         (0) root         (0)      542 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/BoundaryConditions/Inflow.mo
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/BoundaryConditions/Terminal.mo
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/BoundaryConditions/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/BoundaryConditions/package.order
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/KLag.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/KLagAlpha.mo
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/KLagNonlinearityParameterDenominator.mo
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/KLagNonlinearityParameter.mo
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/KLagNonlinearityParameterNumerator.mo
--rw-rw-rw-   0 root         (0) root         (0)     1262 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/PartialKLag.mo
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/package.mo
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/MuskingumWeightingFactor.mo
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/package.order
--rw-rw-rw-   0 root         (0) root         (0)     1409 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/PartialMuskingum.mo
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Steady.mo
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/package.mo
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/EmptyBranch.mo
--rw-rw-rw-   0 root         (0) root         (0)      367 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Delay.mo
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/package.order
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Integrator.mo
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Muskingum.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/QSI.mo
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/package.order
--rw-rw-rw-   0 root         (0) root         (0)      414 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/QSO.mo
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/Storage.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/DischargeControlledStructure.mo
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/Pump.mo
--rw-rw-rw-   0 root         (0) root         (0)      775 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/RunOfRiverHydropowerComplexFixedHead.mo
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/package.order
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/package.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Internal/
--rw-rw-rw-   0 root         (0) root         (0)     1325 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Internal/PartialNode.mo
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Internal/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Internal/package.order
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/NodeHQPort.mo
--rw-rw-rw-   0 root         (0) root         (0)     1246 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Node.mo
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/package.order
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/package.order
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Reservoir/
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Reservoir/Reservoir_turbine_out.mo
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Reservoir/Reservoir.mo
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Reservoir/package.mo
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Reservoir/package.order
--rw-rw-rw-   0 root         (0) root         (0)      288 2023-02-21 10:29:18.000000 rtc-tools-channel-flow-1.1.1rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/versioneer.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-02-21 10:29:17.000000 rtc-tools-channel-flow-1.1.1rc1/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)      982 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtc_tools_channel_flow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      982 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtc_tools_channel_flow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10350 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtc_tools_channel_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtc_tools_channel_flow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtc_tools_channel_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtc_tools_channel_flow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtc_tools_channel_flow.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/Constants.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/package.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/HQToQOut.mo
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/QInToHQ.mo
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/package.order
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/HQPort.mo
+-rw-rw-rw-   0 root         (0) root         (0)      736 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/HQCMPort.mo
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/QOutPort.mo
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/QInPort.mo
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/package.order
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/SmoothMax.mo
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/SmoothSwitch.mo
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/SmoothAbs.mo
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/package.order
+-rw-rw-rw-   0 root         (0) root         (0)      362 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Functions/SmoothMin.mo
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QForcing.mo
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/HQOnePort.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/HQTwoPort.mo
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QSI.mo
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QLateral.mo
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Reservoir.mo
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QSISO.mo
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)      315 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Volume.mo
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/package.order
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QSO.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Media/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Media/SalineWater.mo
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Media/FreshWater.mo
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Media/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Media/package.order
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/
+-rw-rw-rw-   0 root         (0) root         (0)      606 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/Level.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/Discharge.mo
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/package.order
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/HomotopicLinear.mo
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Linear.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Internal/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Internal/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Internal/BottomFrictionCoefficient.mo
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Internal/package.order
+-rw-rw-rw-   0 root         (0) root         (0)    11063 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Internal/PartialHomotopic.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3175 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/HomotopicTrapezoidal.mo
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/package.order
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/Linear.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/Internal/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/Internal/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/Internal/package.order
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/Internal/PartialStorage.mo
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/package.order
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Structures/
+-rw-rw-rw-   0 root         (0) root         (0)     1448 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Structures/DischargeControlledStructure.mo
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Structures/Pump.mo
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Structures/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Structures/package.order
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/package.order
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/Linear.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/Internal/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/Internal/PartialReservoir.mo
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/Internal/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/Internal/package.order
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/package.order
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/package.order
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/BoundaryConditions/
+-rw-rw-rw-   0 root         (0) root         (0)      542 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/BoundaryConditions/Inflow.mo
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/BoundaryConditions/Terminal.mo
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/BoundaryConditions/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/BoundaryConditions/package.order
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/KLag.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/KLagAlpha.mo
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/KLagNonlinearityParameterDenominator.mo
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/KLagNonlinearityParameter.mo
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/KLagNonlinearityParameterNumerator.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/PartialKLag.mo
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/MuskingumWeightingFactor.mo
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/package.order
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/PartialMuskingum.mo
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Steady.mo
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/EmptyBranch.mo
+-rw-rw-rw-   0 root         (0) root         (0)      367 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Delay.mo
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/package.order
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Integrator.mo
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Muskingum.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/QSI.mo
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/package.order
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/QSO.mo
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/Storage.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/DischargeControlledStructure.mo
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/Pump.mo
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/RunOfRiverHydropowerComplexFixedHead.mo
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/package.order
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/package.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Internal/
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Internal/PartialNode.mo
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Internal/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Internal/package.order
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/NodeHQPort.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Node.mo
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/package.order
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/package.order
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Reservoir/
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Reservoir/Reservoir_turbine_out.mo
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Reservoir/Reservoir.mo
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Reservoir/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Reservoir/package.order
+-rw-rw-rw-   0 root         (0) root         (0)      288 2023-05-30 09:09:09.000000 rtc-tools-channel-flow-1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/versioneer.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-05-30 09:09:08.000000 rtc-tools-channel-flow-1.1.2/README
```

### Comparing `rtc-tools-channel-flow-1.1.1rc1/PKG-INFO` & `rtc-tools-channel-flow-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtc-tools-channel-flow
-Version: 1.1.1rc1
+Version: 1.1.2
 Summary: Simple and hydraulic Modelica routing models for RTC-Tools 2.
 Home-page: http://www.deltares.nl/en/software/rtc-tools/
 Author: Deltares
 Maintainer: Deltares
 License: LGPL
 Download-URL: http://gitlab.com/deltares/rtc-tools-channel-flow/
 Platform: Windows
```

### Comparing `rtc-tools-channel-flow-1.1.1rc1/COPYING.LESSER` & `rtc-tools-channel-flow-1.1.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/setup.py` & `rtc-tools-channel-flow-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     url='http://www.deltares.nl/en/software/rtc-tools/',
     download_url='http://gitlab.com/deltares/rtc-tools-channel-flow/',
     classifiers=[_f for _f in CLASSIFIERS.split('\n') if _f],
     platforms=['Windows', 'Linux', 'Mac OS-X', 'Unix'],
     license="LGPL",
     packages=find_packages("src"),
     package_dir={"": "src"},
-    install_requires=["rtc-tools>=2.0.0",
-                      "pymoca >= 0.4.2"],
+    install_requires=["pymoca >= 0.4.2"],
     include_package_data=True,
     cmdclass=versioneer.get_cmdclass(),
     entry_points={
         'rtctools.libraries.modelica': [
             'library_folder = rtctools_channel_flow:modelica',
         ]
     }
```

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtc_tools_channel_flow.egg-info/PKG-INFO` & `rtc-tools-channel-flow-1.1.2/src/rtc_tools_channel_flow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtc-tools-channel-flow
-Version: 1.1.1rc1
+Version: 1.1.2
 Summary: Simple and hydraulic Modelica routing models for RTC-Tools 2.
 Home-page: http://www.deltares.nl/en/software/rtc-tools/
 Author: Deltares
 Maintainer: Deltares
 License: LGPL
 Download-URL: http://gitlab.com/deltares/rtc-tools-channel-flow/
 Platform: Windows
```

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtc_tools_channel_flow.egg-info/SOURCES.txt` & `rtc-tools-channel-flow-1.1.2/src/rtc_tools_channel_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/Constants.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/Constants.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/package.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/package.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/HQToQOut.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/HQToQOut.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/QInToHQ.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/Adaptors/QInToHQ.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/HQPort.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/HQPort.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/HQCMPort.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/HQCMPort.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/QOutPort.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Interfaces/QOutPort.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/HQTwoPort.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/HQTwoPort.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QLateral.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QLateral.mo`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 within Deltares.ChannelFlow.Internal;
 
 partial class QLateral
   parameter Integer n_QLateral(min = 0) = 0;
   Deltares.ChannelFlow.Interfaces.QInPort QLateral[n_QLateral] annotation(Placement(visible = true, transformation(origin = {40, 80}, extent = {{20, -20}, {-20, 20}}, rotation = 90), iconTransformation(origin = {40, 80}, extent = {{20, -20}, {-20, 20}}, rotation = 90)));
-  annotation(Icon(graphics = {Text(extent = {{50, 100}, {90, 80}}, textString = "%n_QLateral", fontSize = 80, fontName = "Arial")}, coordinateSystem(initialScale = 0.1)));
+  annotation(Icon(graphics = {Text(extent = {{50, 100}, {90, 80}}, textString = "%n_QLateral")}, coordinateSystem(initialScale = 0.1)));
 end QLateral;
```

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Reservoir.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/Reservoir.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QSISO.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Internal/QSISO.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/Level.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/Level.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/Discharge.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/BoundaryConditions/Discharge.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/HomotopicLinear.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/HomotopicLinear.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Internal/PartialHomotopic.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/Internal/PartialHomotopic.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/HomotopicTrapezoidal.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Branches/HomotopicTrapezoidal.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/Internal/PartialStorage.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Storage/Internal/PartialStorage.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Structures/DischargeControlledStructure.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Structures/DischargeControlledStructure.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/Internal/PartialReservoir.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/Hydraulic/Reservoir/Internal/PartialReservoir.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/BoundaryConditions/Inflow.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/BoundaryConditions/Inflow.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/PartialKLag.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/PartialKLag.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/PartialMuskingum.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Branches/Internal/PartialMuskingum.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/Storage.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Storage/Storage.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/DischargeControlledStructure.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/DischargeControlledStructure.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/RunOfRiverHydropowerComplexFixedHead.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Structures/RunOfRiverHydropowerComplexFixedHead.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Internal/PartialNode.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Internal/PartialNode.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/NodeHQPort.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/NodeHQPort.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Node.mo` & `rtc-tools-channel-flow-1.1.2/src/rtctools_channel_flow/modelica/Deltares/ChannelFlow/SimpleRouting/Nodes/Node.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-channel-flow-1.1.1rc1/versioneer.py` & `rtc-tools-channel-flow-1.1.2/versioneer.py`

 * *Files identical despite different names*

