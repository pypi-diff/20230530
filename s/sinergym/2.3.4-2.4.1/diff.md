# Comparing `tmp/sinergym-2.3.4.tar.gz` & `tmp/sinergym-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinergym-2.3.4.tar", last modified: Wed May 10 07:17:54 2023, max compression
+gzip compressed data, was "sinergym-2.4.1.tar", last modified: Tue May 30 13:36:31 2023, max compression
```

## Comparing `sinergym-2.3.4.tar` & `sinergym-2.4.1.tar`

### file list

```diff
@@ -1,80 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.781370 sinergym-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 07:17:52.000000 sinergym-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 07:17:52.000000 sinergym-2.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-05-10 07:17:54.781370 sinergym-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-05-10 07:17:52.000000 sinergym-2.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 07:17:53.000000 sinergym-2.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-10 07:17:54.781370 sinergym-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-10 07:17:53.000000 sinergym-2.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.745370 sinergym-2.3.4/sinergym/
--rw-r--r--   0 runner    (1001) docker     (123)    94684 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.745370 sinergym-2.3.4/sinergym/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.749370 sinergym-2.3.4/sinergym/data/buildings/
--rw-r--r--   0 runner    (1001) docker     (123)   168677 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf
--rw-r--r--   0 runner    (1001) docker     (123)   140099 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/buildings/5ZoneAutoDXVAV.idf
--rw-r--r--   0 runner    (1001) docker     (123)   586238 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf
--rw-r--r--   0 runner    (1001) docker     (123)   373188 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf
--rw-r--r--   0 runner    (1001) docker     (123)   475269 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/buildings/OfficeGridStorageSmoothing.idf
--rw-r--r--   0 runner    (1001) docker     (123)   265862 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/buildings/ShopWithVandBattery.idf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.753370 sinergym-2.3.4/sinergym/data/variables/
--rw-r--r--   0 runner    (1001) docker     (123)    35474 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    32612 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/variables/5ZoneAutoDXVAV.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    39868 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    42336 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/variables/OfficeGridStorageSmoothing.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/variables/ShopWithVandBattery.rdd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.777371 sinergym-2.3.4/sinergym/data/weather/
--rw-r--r--   0 runner    (1001) docker     (123)    28629 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1565086 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28503 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1550279 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28704 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1621761 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1553382 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28801 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1558629 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1558423 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1601571 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1637298 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1629153 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1639985 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29614 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1613784 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1624547 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1625209 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.777371 sinergym-2.3.4/sinergym/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/envs/eplus_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.777371 sinergym-2.3.4/sinergym/simulators/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/simulators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24425 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/simulators/eplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/simulators/eplus_alpha.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.781370 sinergym-2.3.4/sinergym/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    32883 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    39674 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.749370 sinergym-2.3.4/sinergym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.872037 sinergym-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-30 13:36:28.000000 sinergym-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-30 13:36:28.000000 sinergym-2.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-05-30 13:36:31.872037 sinergym-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-05-30 13:36:28.000000 sinergym-2.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 13:36:30.000000 sinergym-2.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-30 13:36:31.872037 sinergym-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-30 13:36:30.000000 sinergym-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.840037 sinergym-2.4.1/sinergym/
+-rw-r--r--   0 runner    (1001) docker     (123)    95172 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.840037 sinergym-2.4.1/sinergym/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36306 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/config/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.836037 sinergym-2.4.1/sinergym/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.844037 sinergym-2.4.1/sinergym/data/buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)   155871 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON
+-rw-r--r--   0 runner    (1001) docker     (123)   147138 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON
+-rw-r--r--   0 runner    (1001) docker     (123)   627443 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.epJSON
+-rw-r--r--   0 runner    (1001) docker     (123)   361854 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.epJSON
+-rw-r--r--   0 runner    (1001) docker     (123)   521353 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/buildings/OfficeGridStorageSmoothing.epJSON
+-rw-r--r--   0 runner    (1001) docker     (123)   251292 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/buildings/ShopWithVandBattery.epJSON
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.844037 sinergym-2.4.1/sinergym/data/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)    35474 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    32612 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/variables/5ZoneAutoDXVAV.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    39868 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    42336 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/variables/OfficeGridStorageSmoothing.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/variables/ShopWithVandBattery.rdd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.868037 sinergym-2.4.1/sinergym/data/weather/
+-rw-r--r--   0 runner    (1001) docker     (123)    28629 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1565086 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28503 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1550279 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28704 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1621761 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1553382 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28801 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1558629 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1558423 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1601571 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1637298 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1629153 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1639985 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29614 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1613784 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1624547 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1625209 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.868037 sinergym-2.4.1/sinergym/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/envs/eplus_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.872037 sinergym-2.4.1/sinergym/simulators/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/simulators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25211 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/simulators/eplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/simulators/eplus_alpha.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.872037 sinergym-2.4.1/sinergym/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39674 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.840037 sinergym-2.4.1/sinergym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-05-30 13:36:31.000000 sinergym-2.4.1/sinergym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-30 13:36:31.000000 sinergym-2.4.1/sinergym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:36:31.000000 sinergym-2.4.1/sinergym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-30 13:36:31.000000 sinergym-2.4.1/sinergym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 13:36:31.000000 sinergym-2.4.1/sinergym.egg-info/top_level.txt
```

### Comparing `sinergym-2.3.4/LICENSE` & `sinergym-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/PKG-INFO` & `sinergym-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 2.3.4
+Version: 2.4.1
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 2.3.4 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 2.4.1 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-2.3.4/README.md` & `sinergym-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/setup.py` & `sinergym-2.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
               'wandb',
               'pytest',
               'pytest-cov',
               'pytest-xdist',  # Unit test repository
               'sphinx',  # documentation
               'sphinx-rtd-theme',  # documentation theme
               'sphinxcontrib-spelling',  # documentation spelling
-              'sphinxcontrib-jquery==2.0.0',
+              'sphinxcontrib-jquery',
               # documentation versioning
               'sphinx-multiversion @ git+https://github.com/Holzhaus/sphinx-multiversion#egg=sphinx-multiversion',
               'sphinx-multitoc-numbering',  # Section numbering
               'pyenchant',
               'nbsphinx',
               'nbsphinx_link',
               'google-api-python-client==2.58.0',
@@ -44,26 +44,24 @@
               'google-cloud-storage==2.5.0',
               'IPython'
           ],
           'test': [
               'pytest',
               'pytest-cov',
               'pytest-xdist',
-              'stable-baselines3==2.0.0a5',
-              'wandb'
           ],
           'DRL': [
               'stable-baselines3==2.0.0a5',
               'wandb'
           ],
           'doc': [
               'sphinx',
               'sphinx-rtd-theme',
               'sphinxcontrib-spelling',
-              'sphinxcontrib-jquery==2.0.0',
+              'sphinxcontrib-jquery',
               'sphinx-multiversion @ git+https://github.com/Holzhaus/sphinx-multiversion#egg=sphinx-multiversion',
               'sphinx-multitoc-numbering',
               'pyenchant',
               'nbsphinx',
               'nbsphinx_link',
               'IPython'
           ],
```

### Comparing `sinergym-2.3.4/sinergym/__init__.py` & `sinergym-2.4.1/sinergym/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #                          5ZoneAutoDXVAV Environments                         #
 # ---------------------------------------------------------------------------- #
 # 0) Demo environment
 register(
     id='Eplus-demo-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '5ZoneAutoDXVAV.idf',
+        'building_file': '5ZoneAutoDXVAV.epJSON',
         'weather_file': 'USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw',
         'observation_space': DEFAULT_5ZONE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_5ZONE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_5ZONE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_5ZONE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_5ZONE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -40,15 +40,15 @@
         'action_definition': DEFAULT_5ZONE_ACTION_DEFINITION})
 
 # 1) 5-zone, hot weather, discrete actions
 register(
     id='Eplus-5Zone-hot-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '5ZoneAutoDXVAV.idf',
+        'building_file': '5ZoneAutoDXVAV.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_5ZONE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_5ZONE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_5ZONE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_5ZONE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_5ZONE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -62,15 +62,15 @@
         'action_definition': DEFAULT_5ZONE_ACTION_DEFINITION})
 
 # 2) 5-zone, mixed weather, discrete actions
 register(
     id='Eplus-5Zone-mixed-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '5ZoneAutoDXVAV.idf',
+        'building_file': '5ZoneAutoDXVAV.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_5ZONE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_5ZONE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_5ZONE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_5ZONE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_5ZONE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -84,15 +84,15 @@
         'action_definition': DEFAULT_5ZONE_ACTION_DEFINITION})
 
 # 3) 5-zone, cool weather, discrete actions
 register(
     id='Eplus-5Zone-cool-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '5ZoneAutoDXVAV.idf',
+        'building_file': '5ZoneAutoDXVAV.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_5ZONE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_5ZONE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_5ZONE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_5ZONE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_5ZONE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -106,15 +106,15 @@
         'action_definition': DEFAULT_5ZONE_ACTION_DEFINITION})
 
 # 4) 5-zone, hot weather, discrete actions and stochastic
 register(
     id='Eplus-5Zone-hot-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '5ZoneAutoDXVAV.idf',
+        'building_file': '5ZoneAutoDXVAV.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_5ZONE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_5ZONE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_5ZONE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_5ZONE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_5ZONE_ACTION_MAPPING,
         'weather_variability': (
@@ -132,15 +132,15 @@
         'action_definition': DEFAULT_5ZONE_ACTION_DEFINITION})
 
 # 5) 5-zone, mixed weather, discrete actions and stochastic
 register(
     id='Eplus-5Zone-mixed-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '5ZoneAutoDXVAV.idf',
+        'building_file': '5ZoneAutoDXVAV.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_5ZONE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_5ZONE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_5ZONE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_5ZONE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_5ZONE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -155,15 +155,15 @@
         'action_definition': DEFAULT_5ZONE_ACTION_DEFINITION})
 
 # 6) 5-zone, cool weather, discrete actions and stochastic
 register(
     id='Eplus-5Zone-cool-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '5ZoneAutoDXVAV.idf',
+        'building_file': '5ZoneAutoDXVAV.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_5ZONE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_5ZONE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_5ZONE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_5ZONE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_5ZONE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -178,15 +178,15 @@
         'action_definition': DEFAULT_5ZONE_ACTION_DEFINITION})
 
 # 7) 5-zone, hot weather, continuous actions
 register(
     id='Eplus-5Zone-hot-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '5ZoneAutoDXVAV.idf',
+        'building_file': '5ZoneAutoDXVAV.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_5ZONE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_5ZONE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_5ZONE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_5ZONE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_5ZONE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -203,15 +203,15 @@
         'action_definition': DEFAULT_5ZONE_ACTION_DEFINITION})
 
 # 8) 5-zone, mixed weather, continuous actions
 register(
     id='Eplus-5Zone-mixed-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '5ZoneAutoDXVAV.idf',
+        'building_file': '5ZoneAutoDXVAV.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_5ZONE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_5ZONE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_5ZONE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_5ZONE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_5ZONE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -228,15 +228,15 @@
         'action_definition': DEFAULT_5ZONE_ACTION_DEFINITION})
 
 # 9) 5-zone, cool weather, continuous actions
 register(
     id='Eplus-5Zone-cool-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '5ZoneAutoDXVAV.idf',
+        'building_file': '5ZoneAutoDXVAV.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_5ZONE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_5ZONE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_5ZONE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_5ZONE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_5ZONE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -253,15 +253,15 @@
         'action_definition': DEFAULT_5ZONE_ACTION_DEFINITION})
 
 # 10) 5-zone, hot weather, continuous actions and stochastic
 register(
     id='Eplus-5Zone-hot-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '5ZoneAutoDXVAV.idf',
+        'building_file': '5ZoneAutoDXVAV.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_5ZONE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_5ZONE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_5ZONE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_5ZONE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_5ZONE_ACTION_MAPPING,
         'weather_variability': (
@@ -282,15 +282,15 @@
         'action_definition': DEFAULT_5ZONE_ACTION_DEFINITION})
 
 # 11) 5-zone, mixed weather, continuous actions and stochastic
 register(
     id='Eplus-5Zone-mixed-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '5ZoneAutoDXVAV.idf',
+        'building_file': '5ZoneAutoDXVAV.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_5ZONE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_5ZONE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_5ZONE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_5ZONE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_5ZONE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -305,15 +305,15 @@
         'action_definition': DEFAULT_5ZONE_ACTION_DEFINITION})
 
 # 12) 5-zone, cool weather, continuous actions and stochastic
 register(
     id='Eplus-5Zone-cool-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '5ZoneAutoDXVAV.idf',
+        'building_file': '5ZoneAutoDXVAV.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_5ZONE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_5ZONE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_5ZONE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_5ZONE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_5ZONE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -331,15 +331,15 @@
 #                            Datacenter Environments                           #
 # ---------------------------------------------------------------------------- #
 # 13) DC, hot weather, discrete actions
 register(
     id='Eplus-datacenter-hot-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '2ZoneDataCenterHVAC_wEconomizer.idf',
+        'building_file': '2ZoneDataCenterHVAC_wEconomizer.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_DATACENTER_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_DATACENTER_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_DATACENTER_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_DATACENTER_ACTION_VARIABLES,
         'action_mapping': DEFAULT_DATACENTER_ACTION_MAPPING,
         'reward': LinearReward,
@@ -358,15 +358,15 @@
 )
 
 # 14) DC, hot weather, continuous actions
 register(
     id='Eplus-datacenter-hot-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '2ZoneDataCenterHVAC_wEconomizer.idf',
+        'building_file': '2ZoneDataCenterHVAC_wEconomizer.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_DATACENTER_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_DATACENTER_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_DATACENTER_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_DATACENTER_ACTION_VARIABLES,
         'action_mapping': DEFAULT_DATACENTER_ACTION_MAPPING,
         'reward': LinearReward,
@@ -385,15 +385,15 @@
 )
 
 # 15) DC, hot weather, discrete actions and stochastic
 register(
     id='Eplus-datacenter-hot-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '2ZoneDataCenterHVAC_wEconomizer.idf',
+        'building_file': '2ZoneDataCenterHVAC_wEconomizer.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_DATACENTER_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_DATACENTER_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_DATACENTER_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_DATACENTER_ACTION_VARIABLES,
         'action_mapping': DEFAULT_DATACENTER_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -413,15 +413,15 @@
 )
 
 # 16) DC, hot weather, continuous actions and stochastic
 register(
     id='Eplus-datacenter-hot-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '2ZoneDataCenterHVAC_wEconomizer.idf',
+        'building_file': '2ZoneDataCenterHVAC_wEconomizer.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_DATACENTER_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_DATACENTER_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_DATACENTER_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_DATACENTER_ACTION_VARIABLES,
         'action_mapping': DEFAULT_DATACENTER_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -441,15 +441,15 @@
 )
 
 # 17) DC, mixed weather, discrete actions
 register(
     id='Eplus-datacenter-mixed-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '2ZoneDataCenterHVAC_wEconomizer.idf',
+        'building_file': '2ZoneDataCenterHVAC_wEconomizer.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_DATACENTER_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_DATACENTER_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_DATACENTER_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_DATACENTER_ACTION_VARIABLES,
         'action_mapping': DEFAULT_DATACENTER_ACTION_MAPPING,
         'reward': LinearReward,
@@ -466,15 +466,15 @@
         'action_definition': DEFAULT_DATACENTER_ACTION_DEFINITION})
 
 # 18) DC, mixed weather, continuous actions
 register(
     id='Eplus-datacenter-mixed-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '2ZoneDataCenterHVAC_wEconomizer.idf',
+        'building_file': '2ZoneDataCenterHVAC_wEconomizer.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_DATACENTER_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_DATACENTER_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_DATACENTER_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_DATACENTER_ACTION_VARIABLES,
         'action_mapping': DEFAULT_DATACENTER_ACTION_MAPPING,
         'reward': LinearReward,
@@ -491,15 +491,15 @@
         'action_definition': DEFAULT_DATACENTER_ACTION_DEFINITION})
 
 # 19) DC, mixed weather, discrete actions and stochastic
 register(
     id='Eplus-datacenter-mixed-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '2ZoneDataCenterHVAC_wEconomizer.idf',
+        'building_file': '2ZoneDataCenterHVAC_wEconomizer.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_DATACENTER_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_DATACENTER_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_DATACENTER_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_DATACENTER_ACTION_VARIABLES,
         'action_mapping': DEFAULT_DATACENTER_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -517,15 +517,15 @@
         'action_definition': DEFAULT_DATACENTER_ACTION_DEFINITION})
 
 # 20) DC, mixed weather, continuous actions and stochastic
 register(
     id='Eplus-datacenter-mixed-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '2ZoneDataCenterHVAC_wEconomizer.idf',
+        'building_file': '2ZoneDataCenterHVAC_wEconomizer.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_DATACENTER_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_DATACENTER_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_DATACENTER_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_DATACENTER_ACTION_VARIABLES,
         'action_mapping': DEFAULT_DATACENTER_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -543,15 +543,15 @@
         'action_definition': DEFAULT_DATACENTER_ACTION_DEFINITION})
 
 # 21) DC, cool weather, discrete actions
 register(
     id='Eplus-datacenter-cool-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '2ZoneDataCenterHVAC_wEconomizer.idf',
+        'building_file': '2ZoneDataCenterHVAC_wEconomizer.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_DATACENTER_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_DATACENTER_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_DATACENTER_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_DATACENTER_ACTION_VARIABLES,
         'action_mapping': DEFAULT_DATACENTER_ACTION_MAPPING,
         'reward': LinearReward,
@@ -570,15 +570,15 @@
         'action_definition': DEFAULT_DATACENTER_ACTION_DEFINITION})
 
 # 22) DC, cool weather, continuous actions
 register(
     id='Eplus-datacenter-cool-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '2ZoneDataCenterHVAC_wEconomizer.idf',
+        'building_file': '2ZoneDataCenterHVAC_wEconomizer.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_DATACENTER_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_DATACENTER_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_DATACENTER_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_DATACENTER_ACTION_VARIABLES,
         'action_mapping': DEFAULT_DATACENTER_ACTION_MAPPING,
         'reward': LinearReward,
@@ -595,15 +595,15 @@
         'action_definition': DEFAULT_DATACENTER_ACTION_DEFINITION})
 
 # 23) DC, cool weather, discrete actions and stochastic
 register(
     id='Eplus-datacenter-cool-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '2ZoneDataCenterHVAC_wEconomizer.idf',
+        'building_file': '2ZoneDataCenterHVAC_wEconomizer.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_DATACENTER_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_DATACENTER_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_DATACENTER_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_DATACENTER_ACTION_VARIABLES,
         'action_mapping': DEFAULT_DATACENTER_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -621,15 +621,15 @@
         'action_definition': DEFAULT_DATACENTER_ACTION_DEFINITION})
 
 # 24) DC, cool weather, continuous actions and stochastic
 register(
     id='Eplus-datacenter-cool-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': '2ZoneDataCenterHVAC_wEconomizer.idf',
+        'building_file': '2ZoneDataCenterHVAC_wEconomizer.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_DATACENTER_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_DATACENTER_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_DATACENTER_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_DATACENTER_ACTION_VARIABLES,
         'action_mapping': DEFAULT_DATACENTER_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -651,15 +651,15 @@
 # ---------------------------------------------------------------------------- #
 
 # 25) WH, hot weather, discrete actions
 register(
     id='Eplus-warehouse-hot-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_Warehouse_Denver.idf',
+        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -677,15 +677,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 26) WH, hot weather, continuous actions
 register(
     id='Eplus-warehouse-hot-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_Warehouse_Denver.idf',
+        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -703,15 +703,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 27) WH, hot weather, discrete actions and stochastic
 register(
     id='Eplus-warehouse-hot-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_Warehouse_Denver.idf',
+        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -730,15 +730,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 28) WH, hot weather, continuous actions and stochastic
 register(
     id='Eplus-warehouse-hot-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_Warehouse_Denver.idf',
+        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -757,15 +757,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 29) WH, mixed weather, discrete actions
 register(
     id='Eplus-warehouse-mixed-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_Warehouse_Denver.idf',
+        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -783,15 +783,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 30) WH, mixed weather, continuous actions
 register(
     id='Eplus-warehouse-mixed-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_Warehouse_Denver.idf',
+        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -809,15 +809,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 31) WH, mixed weather, discrete actions and stochastic
 register(
     id='Eplus-warehouse-mixed-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_Warehouse_Denver.idf',
+        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -836,15 +836,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 32) WH, mixed weather, continuous actions and stochastic
 register(
     id='Eplus-warehouse-mixed-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_Warehouse_Denver.idf',
+        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -863,15 +863,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 33) WH, cool weather, discrete actions
 register(
     id='Eplus-warehouse-cool-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_Warehouse_Denver.idf',
+        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -889,15 +889,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 34) WH, cool weather, continuous actions
 register(
     id='Eplus-warehouse-cool-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_Warehouse_Denver.idf',
+        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -915,15 +915,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 35) WH, cool weather, discrete actions and stochastic
 register(
     id='Eplus-warehouse-cool-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_Warehouse_Denver.idf',
+        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -942,15 +942,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 36) WH, cool weather, continuous actions and stochastic
 register(
     id='Eplus-warehouse-cool-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_Warehouse_Denver.idf',
+        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -974,15 +974,15 @@
 # ---------------------------------------------------------------------------- #
 
 # 37) MO, hot weather, discrete actions
 register(
     id='Eplus-office-hot-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_OfficeMedium_Denver.idf',
+        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1015,15 +1015,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 38) MO, hot weather, continuous actions
 register(
     id='Eplus-office-hot-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_OfficeMedium_Denver.idf',
+        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1056,15 +1056,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 39) MO, hot weather, discrete actions and stochastic
 register(
     id='Eplus-office-hot-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_OfficeMedium_Denver.idf',
+        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1098,15 +1098,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 40) MO, hot weather, continuous actions and stochastic
 register(
     id='Eplus-office-hot-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_OfficeMedium_Denver.idf',
+        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1140,15 +1140,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 41) MO, mixed weather, discrete actions
 register(
     id='Eplus-office-mixed-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_OfficeMedium_Denver.idf',
+        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1181,15 +1181,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 42) MO, mixed weather, continuous actions
 register(
     id='Eplus-office-mixed-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_OfficeMedium_Denver.idf',
+        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1222,15 +1222,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 43) MO, mixed weather, discrete actions and stochastic
 register(
     id='Eplus-office-mixed-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_OfficeMedium_Denver.idf',
+        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1264,15 +1264,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 44) MO, mixed weather, continuous actions and stochastic
 register(
     id='Eplus-office-mixed-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_OfficeMedium_Denver.idf',
+        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1306,15 +1306,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 45) MO, cool weather, discrete actions
 register(
     id='Eplus-office-cool-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_OfficeMedium_Denver.idf',
+        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1347,15 +1347,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 46) MO, cool weather, continuous actions
 register(
     id='Eplus-office-cool-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_OfficeMedium_Denver.idf',
+        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1388,15 +1388,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 47) MO, cool weather, discrete actions and stochastic
 register(
     id='Eplus-office-cool-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_OfficeMedium_Denver.idf',
+        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1430,15 +1430,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 48) MO, cool weather, continuous actions and stochastic
 register(
     id='Eplus-office-cool-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ASHRAE9012016_OfficeMedium_Denver.idf',
+        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1475,15 +1475,15 @@
 #                                  Office Grid                                 #
 # ---------------------------------------------------------------------------- #
 
 register(
     id='Eplus-officegrid-cool-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'OfficeGridStorageSmoothing.idf',
+        'building_file': 'OfficeGridStorageSmoothing.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_OFFICEGRID_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICEGRID_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICEGRID_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICEGRID_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICEGRID_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1517,15 +1517,15 @@
         'env_name': 'officegrid-cool-continuous-v1',
         'action_definition': DEFAULT_OFFICEGRID_ACTION_DEFINITION})
 
 register(
     id='Eplus-officegrid-mixed-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'OfficeGridStorageSmoothing.idf',
+        'building_file': 'OfficeGridStorageSmoothing.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_OFFICEGRID_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICEGRID_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICEGRID_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICEGRID_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICEGRID_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1559,15 +1559,15 @@
         'env_name': 'officegrid-mixed-continuous-v1',
         'action_definition': DEFAULT_OFFICEGRID_ACTION_DEFINITION})
 
 register(
     id='Eplus-officegrid-hot-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'OfficeGridStorageSmoothing.idf',
+        'building_file': 'OfficeGridStorageSmoothing.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_OFFICEGRID_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICEGRID_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICEGRID_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICEGRID_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICEGRID_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1601,15 +1601,15 @@
         'env_name': 'officegrid-hot-continuous-v1',
         'action_definition': DEFAULT_OFFICEGRID_ACTION_DEFINITION})
 
 register(
     id='Eplus-officegrid-cool-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'OfficeGridStorageSmoothing.idf',
+        'building_file': 'OfficeGridStorageSmoothing.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_OFFICEGRID_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICEGRID_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICEGRID_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICEGRID_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICEGRID_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1644,15 +1644,15 @@
         'env_name': 'officegrid-cool-continuous-stochastic-v1',
         'action_definition': DEFAULT_OFFICEGRID_ACTION_DEFINITION})
 
 register(
     id='Eplus-officegrid-mixed-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'OfficeGridStorageSmoothing.idf',
+        'building_file': 'OfficeGridStorageSmoothing.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_OFFICEGRID_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICEGRID_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICEGRID_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICEGRID_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICEGRID_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1687,15 +1687,15 @@
         'env_name': 'officegrid-mixed-continuous-stochastic-v1',
         'action_definition': DEFAULT_OFFICEGRID_ACTION_DEFINITION})
 
 register(
     id='Eplus-officegrid-hot-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'OfficeGridStorageSmoothing.idf',
+        'building_file': 'OfficeGridStorageSmoothing.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_OFFICEGRID_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICEGRID_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICEGRID_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICEGRID_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICEGRID_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1734,15 +1734,15 @@
 #                                 Shop Battery                                 #
 # ---------------------------------------------------------------------------- #
 
 register(
     id='Eplus-shop-cool-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ShopWithVandBattery.idf',
+        'building_file': 'ShopWithVandBattery.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_SHOP_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_SHOP_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_SHOP_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_SHOP_ACTION_VARIABLES,
         'action_mapping': DEFAULT_SHOP_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1762,15 +1762,15 @@
         'env_name': 'shop-cool-continuous-v1',
         'action_definition': DEFAULT_SHOP_ACTION_DEFINITION})
 
 register(
     id='Eplus-shop-mixed-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ShopWithVandBattery.idf',
+        'building_file': 'ShopWithVandBattery.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_SHOP_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_SHOP_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_SHOP_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_SHOP_ACTION_VARIABLES,
         'action_mapping': DEFAULT_SHOP_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1790,15 +1790,15 @@
         'env_name': 'shop-mixed-continuous-v1',
         'action_definition': DEFAULT_SHOP_ACTION_DEFINITION})
 
 register(
     id='Eplus-shop-hot-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ShopWithVandBattery.idf',
+        'building_file': 'ShopWithVandBattery.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_SHOP_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_SHOP_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_SHOP_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_SHOP_ACTION_VARIABLES,
         'action_mapping': DEFAULT_SHOP_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1818,15 +1818,15 @@
         'env_name': 'shop-hot-continuous-v1',
         'action_definition': DEFAULT_SHOP_ACTION_DEFINITION})
 
 register(
     id='Eplus-shop-cool-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ShopWithVandBattery.idf',
+        'building_file': 'ShopWithVandBattery.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_SHOP_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_SHOP_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_SHOP_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_SHOP_ACTION_VARIABLES,
         'action_mapping': DEFAULT_SHOP_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1847,15 +1847,15 @@
         'env_name': 'shop-cool-continuous-stochastic-v1',
         'action_definition': DEFAULT_SHOP_ACTION_DEFINITION})
 
 register(
     id='Eplus-shop-mixed-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ShopWithVandBattery.idf',
+        'building_file': 'ShopWithVandBattery.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_SHOP_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_SHOP_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_SHOP_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_SHOP_ACTION_VARIABLES,
         'action_mapping': DEFAULT_SHOP_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1876,15 +1876,15 @@
         'env_name': 'shop-mixed-continuous-stochastic-v1',
         'action_definition': DEFAULT_SHOP_ACTION_DEFINITION})
 
 register(
     id='Eplus-shop-hot-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'idf_file': 'ShopWithVandBattery.idf',
+        'building_file': 'ShopWithVandBattery.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_SHOP_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_SHOP_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_SHOP_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_SHOP_ACTION_VARIABLES,
         'action_mapping': DEFAULT_SHOP_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
```

### Comparing `sinergym-2.3.4/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd` & `sinergym-2.4.1/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/variables/5ZoneAutoDXVAV.rdd` & `sinergym-2.4.1/sinergym/data/variables/5ZoneAutoDXVAV.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd` & `sinergym-2.4.1/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd` & `sinergym-2.4.1/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/variables/OfficeGridStorageSmoothing.rdd` & `sinergym-2.4.1/sinergym/data/variables/OfficeGridStorageSmoothing.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/variables/ShopWithVandBattery.rdd` & `sinergym-2.4.1/sinergym/data/variables/ShopWithVandBattery.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy` & `sinergym-2.4.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw` & `sinergym-2.4.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy` & `sinergym-2.4.1/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/COL_Bogota.802220_IWEC.epw` & `sinergym-2.4.1/sinergym/data/weather/COL_Bogota.802220_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy` & `sinergym-2.4.1/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/ESP_Granada.084190_SWEC.epw` & `sinergym-2.4.1/sinergym/data/weather/ESP_Granada.084190_SWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy` & `sinergym-2.4.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw` & `sinergym-2.4.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy` & `sinergym-2.4.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw` & `sinergym-2.4.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy` & `sinergym-2.4.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw` & `sinergym-2.4.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy` & `sinergym-2.4.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw` & `sinergym-2.4.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy` & `sinergym-2.4.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw` & `sinergym-2.4.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy` & `sinergym-2.4.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw` & `sinergym-2.4.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy` & `sinergym-2.4.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw` & `sinergym-2.4.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy` & `sinergym-2.4.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw` & `sinergym-2.4.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy` & `sinergym-2.4.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw` & `sinergym-2.4.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy` & `sinergym-2.4.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw` & `sinergym-2.4.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/envs/eplus_env.py` & `sinergym-2.4.1/sinergym/envs/eplus_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     metadata = {'render_modes': ['human']}
 
     # ---------------------------------------------------------------------------- #
     #                            ENVIRONMENT CONSTRUCTOR                           #
     # ---------------------------------------------------------------------------- #
     def __init__(
         self,
-        idf_file: str,
+        building_file: str,
         weather_file: Union[str, List[str]],
         observation_space: gym.spaces.Box = gym.spaces.Box(
             low=-5e6, high=5e6, shape=(4,), dtype=np.float32),
         observation_variables: List[str] = [],
         action_space: Union[gym.spaces.Box, gym.spaces.Discrete] = gym.spaces.Box(
             low=0, high=0, shape=(0,), dtype=np.float32),
         action_variables: List[str] = [],
@@ -41,20 +41,20 @@
         action_definition: Optional[Dict[str, Any]] = None,
         env_name: str = 'eplus-env-v1',
         config_params: Optional[Dict[str, Any]] = None
     ):
         """Environment with EnergyPlus simulator.
 
         Args:
-            idf_file (str): Name of the IDF file with the building definition.
+            building_file (str): Name of the JSON file with the building definition.
             weather_file (Union[str,List[str]]): Name of the EPW file for weather conditions. It can be specified a list of weathers files in order to sample a weather in each episode randomly.
             observation_space (gym.spaces.Box, optional): Gym Observation Space definition. Defaults to an empty observation_space (no control).
-            observation_variables (List[str], optional): List with variables names in IDF. Defaults to an empty observation variables (no control).
+            observation_variables (List[str], optional): List with variables names in building. Defaults to an empty observation variables (no control).
             action_space (Union[gym.spaces.Box, gym.spaces.Discrete], optional): Gym Action Space definition. Defaults to an empty action_space (no control).
-            action_variables (List[str],optional): Action variables to be controlled in IDF, if that actions names have not been configured manually in IDF, you should configure or use extra_config. Default to empty List.
+            action_variables (List[str],optional): Action variables to be controlled in building, if that actions names have not been configured manually in building, you should configure or use action_definition. Default to empty List.
             action_mapping (Dict[int, Tuple[float, ...]], optional): Action mapping list for discrete actions spaces only. Defaults to empty list.
             weather_variability (Optional[Tuple[float]], optional): Tuple with sigma, mu and tao of the Ornstein-Uhlenbeck process to be applied to weather data. Defaults to None.
             reward (Any, optional): Reward function instance used for agent feedback. Defaults to LinearReward.
             reward_kwargs (Optional[Dict[str, Any]], optional): Parameters to be passed to the reward function. Defaults to empty dict.
             act_repeat (int, optional): Number of timesteps that an action is repeated in the simulator, regardless of the actions it receives during that repetition interval.
             max_ep_data_store_num (int, optional): Number of last sub-folders (one for each episode) generated during execution on the simulation.
             action_definition (Optional[Dict[str, Any]): Dict with building components to being controlled by Sinergym automatically if it is supported. Default value to None.
@@ -64,16 +64,16 @@
 
         # ---------------------------------------------------------------------------- #
         #                          Energyplus, BCVTB and paths                         #
         # ---------------------------------------------------------------------------- #
         eplus_path = os.environ['EPLUS_PATH']
         bcvtb_path = os.environ['BCVTB_PATH']
 
-        # IDF file
-        self.idf_file = idf_file
+        # building file
+        self.building_file = building_file
         # EPW file(s) (str or List of EPW's)
         if isinstance(weather_file, str):
             self.weather_files = [weather_file]
         else:
             self.weather_files = weather_file
 
         # ---------------------------------------------------------------------------- #
@@ -92,15 +92,15 @@
         # ---------------------------------------------------------------------------- #
         #                                   Simulator                                  #
         # ---------------------------------------------------------------------------- #
         self.simulator = EnergyPlus(
             env_name=env_name,
             eplus_path=eplus_path,
             bcvtb_path=bcvtb_path,
-            idf_file=self.idf_file,
+            building_file=self.building_file,
             weather_files=self.weather_files,
             variables=self.variables,
             act_repeat=act_repeat,
             max_ep_data_store_num=max_ep_data_store_num,
             action_definition=action_definition,
             config_params=config_params
         )
@@ -259,35 +259,14 @@
         """End simulation."""
 
         self.simulator.end_env()
 
     # ---------------------------------------------------------------------------- #
     #                           Environment functionality                          #
     # ---------------------------------------------------------------------------- #
-    def get_schedulers(self, path: Optional[str] = None) -> Dict[str, Any]:
-        """Extract all schedulers available in the building model to be controlled.
-
-        Args:
-            path (str, optional): If path is specified, then this method export a xlsx file version in addition to return the dictionary.
-
-        Returns:
-            Dict[str, Any]: Python Dictionary: For each scheduler found, it shows type value and where this scheduler is present (Object name, Object field and Object type).
-        """
-        schedulers = self.simulator._config.schedulers
-        if path is not None:
-            export_actuators_to_excel(actuators=schedulers, path=path)
-        return schedulers
-
-    def get_zones(self) -> List[str]:
-        """Get the zone names available in the building model of that environment.
-
-        Returns:
-            List[str]: List of the zone names.
-        """
-        return self.simulator._config.idf_zone_names
 
     def _get_action(self, action: Any) -> Union[int,
                                                 float,
                                                 np.integer,
                                                 np.ndarray,
                                                 List[Any],
                                                 Tuple[Any]]:
@@ -387,14 +366,37 @@
             assert hasattr(
                 self, 'setpoints_space'), 'Continuous environment: setpoints_space attribute should have been defined.'
             assert not hasattr(
                 self, 'action_mapping'), 'Continuous environment: action mapping should not have been defined.'
             assert len(self._action_space.low) == len(self.variables['action']) and len(self._action_space.high) == len(
                 self.variables['action']), 'Continuous environment: low and high values action space definition should have the same number of values than action variables.'
 
+    def get_schedulers(
+            self, path: Optional[str] = None) -> Dict[str, Dict[str, Union[str, Dict[str, str]]]]:
+        """Extract all schedulers available in the building model to be controlled.
+
+        Args:
+            path (str, optional): If path is specified, then this method export a xlsx file version in addition to return the dictionary.
+
+        Returns:
+            Dict[str, Any]: Python Dictionary: For each scheduler found, it shows type value and where this scheduler is present (Object name, Object field and Object type).
+        """
+        if path is not None:
+            export_actuators_to_excel(
+                actuators=self.simulator.schedulers, path=path)
+        return self.simulator.schedulers
+
+    def get_zones(self) -> List[str]:
+        """Get the zone names available in the building model of that environment.
+
+        Returns:
+            List[str]: List of the zone names.
+        """
+        return self.simulator.zone_names
+
     # ---------------------------------------------------------------------------- #
     #                                  Properties                                  #
     # ---------------------------------------------------------------------------- #
     @property
     def action_space(
         self,
     ) -> gym.spaces.Space[Any] | gym.spaces.Space[Any]:
```

### Comparing `sinergym-2.3.4/sinergym/simulators/base.py` & `sinergym-2.4.1/sinergym/simulators/base.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/simulators/eplus.py` & `sinergym-2.4.1/sinergym/simulators/eplus.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,44 +15,44 @@
 import threading
 import time
 from typing import Any, Dict, List, Optional, Tuple, Union
 from xml.etree.ElementTree import Element, SubElement, tostring
 
 import numpy as np
 
+from sinergym.config.modeling import ModelJSON
 from sinergym.utils.common import *
-from sinergym.utils.config import Config
 from sinergym.utils.logger import Logger
 
 LOG_LEVEL_MAIN = 'INFO'
 LOG_LEVEL_EPLS = 'FATAL'
 LOG_FMT = "[%(asctime)s] %(name)s %(levelname)s:%(message)s"
 
 
 class EnergyPlus(object):
 
     def __init__(
             self,
             eplus_path: str,
             bcvtb_path: str,
             weather_files: List[str],
-            idf_file: str,
+            building_file: str,
             env_name: str,
             variables: Dict[str, List[str]],
             act_repeat: int = 1,
             max_ep_data_store_num: int = 10,
             action_definition: Optional[Dict[str, Any]] = None,
             config_params: Optional[Dict[str, Any]] = None):
         """EnergyPlus simulation class.
 
         Args:
             eplus_path (str):  EnergyPlus installation path.
             bcvtb_path (str): BCVTB installation path.
             weather_files (List[str]): EnergyPlus weather file list (sampling one in each episode).
-            idf_file (str): EnergyPlus input description file (.idf) file.
+            building_file (str): EnergyPlus input description file (.json).
             env_name (str): The environment name.
             variables (Dict[str,List[str]]): Variables list with observation and action keys in a dictionary.
             act_repeat (int, optional): The number of times to repeat the control action. Defaults to 1.
             max_ep_data_store_num (int, optional): The number of simulation results to keep. Defaults to 10.
             config_params (Optional[Dict[str, Any]], optional): Dictionary with all extra configuration for simulator. Defaults to None.
         """
         self._env_name = env_name
@@ -78,58 +78,59 @@
 
         self.logger_main.debug(
             'Socket is listening on host %s port %d' % (sockname))
 
         # Path attributes
         self._eplus_path = eplus_path
         self._weather_files = weather_files
-        self._idf_file = idf_file
+        self._building_file = building_file
         # Episode existed
         self._episode_existed = False
 
         self._epi_num = 0
         self._act_repeat = act_repeat
         self._max_ep_data_store_num = max_ep_data_store_num
         self._last_action = [21.0, 25.0]
 
         # Creating models config (with extra params if exits)
-        self._config = Config(
-            idf_file=self._idf_file,
+        self._config = ModelJSON(
+            json_file=self._building_file,
             weather_files=self._weather_files,
             variables=variables,
             env_name=self._env_name,
             max_ep_store=self._max_ep_data_store_num,
             action_definition=action_definition,
             extra_config=config_params)
 
         # Annotate experiment path in simulator
         self._env_working_dir_parent = self._config.experiment_path
-        # Setting an external interface if IDF building has not got.
+        # Setting an external interface if building has no one.
         self.logger_main.info(
-            'Updating idf ExternalInterface object if it is not present...')
+            'Updating Building model ExternalInterface object if it is not present...')
         self._config.set_external_interface()
-        # Updating IDF file (Location and DesignDays) with EPW file
+        # Updating JSON file (Location and DesignDays) with EPW file
         self.logger_main.info(
-            'Updating idf Site:Location and SizingPeriod:DesignDay(s) to weather and ddy file...')
-        self._config.adapt_idf_to_epw()
-        # Updating IDF file Output:Variables with observation variables
+            'Updating Building model Site:Location and SizingPeriod:DesignDay(s) to weather and ddy file...')
+        self._config.adapt_building_to_epw()
+        # Updating building model Output:Variables with observation variables
         # specified in environment and variables.cfg construction
         self.logger_main.info(
-            'Updating idf OutPut:Variable and variables XML tree model for BVCTB connection.')
-        self._config. adapt_variables_to_cfg_and_idf()
+            'Updating building model OutPut:Variable and variables XML tree model for BVCTB connection.')
+        self._config. adapt_variables_to_cfg_and_building()
         # Setting up extra configuration if exists
         self.logger_main.info(
             'Setting up extra configuration in building model if exists...')
         self._config.apply_extra_conf()
         # Setting up action definition automatic manipulation if exists
         self.logger_main.info(
             'Setting up action definition in building model if exists...')
-        self._config.adapt_idf_to_action_definition()
+        self._config.adapt_building_to_action_definition()
 
-        # In this lines Epm model is modified but no IDF is stored anywhere yet
+        # Note: In this lines building model is modified but no building file is stored
+        # anywhere yet
 
         # Eplus run info
         (self._eplus_run_st_mon,
          self._eplus_run_st_day,
          self._eplus_run_st_year,
          self._eplus_run_ed_mon,
          self._eplus_run_ed_day,
@@ -146,15 +147,15 @@
               options: Optional[Dict[str,
                                      Any]] = None) -> Tuple[List[float],
                                                             Dict[str,
                                                                  Any]]:
         """Resets the environment.
         This method does the following:
         1. Makes a new EnergyPlus working directory.
-        2. Copies .idf and variables.cfg file to the working directory.
+        2. Copies building.json and variables.cfg file to the working directory.
         3. Creates the socket.cfg file in the working directory.
         4. Creates the EnergyPlus subprocess.
         5. Establishes the socket connection with EnergyPlus.
         6. Reads the first sensor data from the EnergyPlus.
         7. Uses a new weather file if passed.
 
         Args:
@@ -174,23 +175,25 @@
                 'EnergyPlus episode completed successfully. ')
             self._epi_num += 1
             # Update weather file used if it is specified more than one
             if len(self._weather_files) > 1:
                 self.logger_main.info(
                     'Updating weather file for new episode (sampling)...')
                 self._config.update_weather_path()
-                self.logger_main.info('Adapting idf to new weather file...')
-                self._config.adapt_idf_to_epw()
+                self.logger_main.info(
+                    'Adapting building to new weather file...')
+                self._config.adapt_building_to_epw()
 
         # Create EnergyPlus simulation process
         self.logger_main.info('Creating new EnergyPlus simulation episode...')
         # Creating episode working dir
         eplus_working_dir = self._config.set_episode_working_dir()
-        # Getting IDF, WEATHER, VARIABLES and OUTPUT path for current episode
-        eplus_working_idf_path = self._config.save_building_model()
+        # Getting BUILDING, WEATHER, VARIABLES and OUTPUT path for current
+        # episode
+        eplus_working_building_path = self._config.save_building_model()
         eplus_working_var_path = self._config.save_variables_cfg()
         eplus_working_out_path = (eplus_working_dir + '/' + 'output')
         eplus_working_weather_path = self._config.apply_weather_variability(
             variation=options.get('weather_variability'))
 
         self._create_socket_cfg(self._host,
                                 self._port,
@@ -201,15 +204,15 @@
         # Create new random weather file in case variability was specified
         # noise always from original EPW
 
         # Select new weather if it is passed into the method
         eplus_process = self._create_eplus(
             self._eplus_path,
             eplus_working_weather_path,
-            eplus_working_idf_path,
+            eplus_working_building_path,
             eplus_working_out_path,
             eplus_working_dir)
         self.logger_main.debug(
             'EnergyPlus process is still running ? %r' %
             self._get_is_subprocess_running(eplus_process))
         self._eplus_process = eplus_process
 
@@ -230,16 +233,16 @@
         # Start the first data exchange
         rcv_1st = conn.recv(2048).decode(encoding='ISO-8859-1')
         self.logger_main.debug(
             'Got the first message successfully: ' + rcv_1st)
         version, flag, nDb, nIn, nBl, curSimTim, Dblist \
             = self._disassembleMsg(rcv_1st)
         # get time info in simulation
-        time_info = get_current_time_info(self._config.building, curSimTim)
-        # Add time_info date in the end of the Energyplus observation
+        time_info = self._config.get_current_time_info(curSimTim)
+        # Add time_info date in the beginning of the Energyplus observation
         Dblist = time_info + Dblist
         # Remember the message header, useful when send data back to EnergyPlus
         self._eplus_msg_header = [version, flag]
         self._curSimTim = curSimTim
         # Check if episode terminates
         is_terminal = False
         if curSimTim >= self._eplus_one_epi_len:  # pragma: no cover
@@ -313,15 +316,15 @@
                 is_terminal = True
                 # Remember the last action
                 self._last_action = action
             act_repeat_i += 1
         # Construct the return, which is the state observation of the last step
         # plus the integral item
         # get time info in simulation
-        time_info = get_current_time_info(self._config.building, curSimTim)
+        time_info = self._config.get_current_time_info(curSimTim)
         # Add time_info to the observation (year,month,day and hour) at the
         # beggining
         Dblist = time_info + Dblist
         # Add terminal state
         # Change some attributes
         self._curSimTim = curSimTim
         self._last_action = action
@@ -340,37 +343,37 @@
 
         return Dblist, is_terminal, False, info
 
     def _create_eplus(
             self,
             eplus_path: str,
             weather_path: str,
-            idf_path: str,
+            building_path: str,
             out_path: str,
             eplus_working_dir: str) -> subprocess.Popen:
         """Creates the EnergyPlus process.
 
         Args:
             eplus_path (str): EnergyPlus path.
             weather_path (str): Weather file path (.epw).
-            idf_path (str): Building model path (.idf).
+            building_path (str): Building model path (.epJSON).
             out_path (str): Output path.
             eplus_working_dir (str): EnergyPlus working directory.
 
         Returns:
             subprocess.Popen: EnergyPlus process.
         """
 
         eplus_process = subprocess.Popen(
             '%s -w %s -d %s %s' %
             (eplus_path +
              '/energyplus',
              weather_path,
              out_path,
-             idf_path),
+             building_path),
             shell=True,
             cwd=eplus_working_dir,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             preexec_fn=os.setsid)
         return eplus_process
 
@@ -525,15 +528,15 @@
         Args:
             version (str): EnergyPlus version.
             flag (str):
             nDb (str):
             nIn (str):
             nBl (str):
             curSimTim (str): Current simulation time.
-            Dblist (str): State of enviroment (depending on variables:output fixed in IDF file).
+            Dblist (str): State of enviroment (depending on variables:output fixed in epJSON file).
 
         Returns:
             str: All values concatenated in correct format to send to EnergyPlus subprocess.
         """
 
         ret = ''
         ret += '%d' % (version)
@@ -626,7 +629,25 @@
     def env_name(self) -> str:  # pragma: no cover
         """Returns the environment name.
 
         Returns:
             str: Environment name
         """
         return self._env_name
+
+    @property
+    def zone_names(self) -> List[str]:  # pragma: no cover
+        """Returns the zone names available in the building.
+
+        Returns:
+            List[str]: Building zones
+        """
+        return self._config.zone_names
+
+    @property
+    def schedulers(self) -> Dict[str, Dict[str, Union[str, Dict[str, str]]]]:  # pragma: no cover
+        """Returns the schedulers information available in the building.
+
+        Returns:
+            Dict[str,Dict[str,Union[str,Dict[str,str]]]]: Dictionary structure with all the information.
+        """
+        return self._config.schedulers
```

### Comparing `sinergym-2.3.4/sinergym/simulators/eplus_alpha.py` & `sinergym-2.4.1/sinergym/simulators/eplus_alpha.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/utils/callbacks.py` & `sinergym-2.4.1/sinergym/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/utils/common.py` & `sinergym-2.4.1/sinergym/utils/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pydoc import locate
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import gymnasium as gym
 import numpy as np
 import pandas as pd
 import xlsxwriter
+from eppy.modeleditor import IDF
 from opyplus import Epm, WeatherData
 from opyplus.epm.record import Record
 
 from sinergym.utils.constants import YEAR
 
 
 def get_delta_seconds(
@@ -42,42 +43,14 @@
     startTime = datetime(st_year, st_mon, st_day, 0, 0, 0)
     endTime = datetime(end_year, end_mon, end_day,
                        23, 0, 0) + timedelta(0, 3600)
     delta_sec = (endTime - startTime).total_seconds()
     return delta_sec
 
 
-def get_current_time_info(
-        epm: Epm, sec_elapsed: float) -> List[int]:
-    """Returns the current day, month and hour given the seconds elapsed since the simulation started.
-
-    Args:
-        epm (opyplus.Epm): EnergyPlus model object.
-        sec_elapsed (float): Seconds elapsed since the start of the simulation
-
-    Returns:
-        List[int]: A List composed by the current year, day, month and hour in the simulation.
-
-    """
-    start_date = datetime(
-        year=int(YEAR if epm.RunPeriod[0]['begin_year'] is None else epm.RunPeriod[0]['begin_year']),
-        month=int(1 if epm.RunPeriod[0]['begin_month'] is None else epm.RunPeriod[0]['begin_month']),
-        day=int(1 if epm.RunPeriod[0]['begin_day_of_month'] is None else epm.RunPeriod[0]['begin_day_of_month'])
-    )
-
-    current_date = start_date + timedelta(seconds=sec_elapsed)
-
-    return [
-        int(current_date.year),
-        int(current_date.month),
-        int(current_date.day),
-        int(current_date.hour),
-    ]
-
-
 def is_wrapped(env: Type[gym.Env], wrapper_class: Type[gym.Wrapper]) -> bool:
     """
     Check if a given environment has been wrapped with a given wrapper.
 
     :param env: Environment to check
     :param wrapper_class: Wrapper class to look for
     :return: True if environment has been wrapped with ``wrapper_class``.
@@ -214,61 +187,34 @@
 
      Returns:
         List[str]: Key list from record.
     """
     return [field.ref for field in record._table._dev_descriptor._field_descriptors]
 
 
-def prepare_batch_from_records(records: List[Record]) -> List[Dict[str, Any]]:
-    """Prepare a list of dictionaries in order to use Epm.add_batch directly
+def eppy_element_to_dict(element: IDF) -> Dict[str, Dict[str, str]]:
+    """Given a eppy element, this function will create a dictionary using the name as key and the rest of fields as value. Following de EnergyPlus epJSON standard.
 
     Args:
-        records List[opyplus.Epm.Record]: List of records which will be converted to dictionary batch.
+        element (IDF): eppy element to be converted.
 
     Returns:
-        List[Dict[str, Any]]: List of dicts where each dictionary is a record element.
+        Dict[str,Dict[str,str]]: Python dictionary with epJSON format of eppy element.
     """
-
-    batch = []
-    for record in records:
-        aux_dict = {}
-        for key in get_record_keys(record):
-            aux_dict[key] = record[key]
-        batch.append(aux_dict)
-
-    return batch
-
-
-def to_idf(building: Epm, file_path: str) -> None:
-    """Given a building model (opyplus Epm object), this function export an IDF file with all content specified.
-
-    Args:
-        building (Epm): Building model from the opyplus object Epm.
-        file_path (str): Path where IDF file will be exported.
-    """
-
-    if building._comment != "":
-        comment = textwrap.indent(building._comment, "! ", lambda line: True)
-    comment += "\n\n"
-
-    dir_path, file_name = os.path.split(file_path)
-    model_name, _ = os.path.splitext(file_name)
-
-    # prepare body
-    formatted_records = []
-    for table_ref, table in building._tables.items(
-    ):  # self._tables is already sorted
-        formatted_records.extend(
-            [r.to_idf(model_name=model_name) for r in table])
-    body = "\n\n".join(formatted_records)
-
-    # write content
-    content = comment + body
-    with open(file_path, "w") as f:
-        f.write(content)
+    fields = {}
+    for fieldname in element.fieldnames:
+        fieldname_fixed = fieldname.lower().replace(
+            'drybulb', 'dry_bulb')
+        if fieldname != 'Name' and fieldname != 'key':
+            if element[fieldname] != '':
+                if element[fieldname] == 'Wetbulb':
+                    fields[fieldname_fixed] = 'WetBulb'
+                else:
+                    fields[fieldname_fixed] = element[fieldname]
+    return {element.Name.lower(): fields}
 
 
 def get_season_comfort_range(
         year: int, month: int, day: int) -> Tuple[float, float]:
     """Get comfort temperature range depending on season. The comfort ranges are those
     defined by ASHRAE in Standard 55—Thermal Environmental Conditions for Human Occupancy (2004).
 
@@ -330,33 +276,32 @@
     current_row += 1
 
     for key, info in actuators.items():
         worksheet.write(current_row, current_col, key, actuator_format)
         current_col += 1
         worksheet.write(current_row, current_col, info['Type'], cells_format)
         current_col += 1
-        for object in info.values():
-            if isinstance(object, dict):
+        for object_name, values in info.items():
+            if isinstance(values, dict):
                 worksheet.write(
                     current_row,
                     current_col,
-                    'Name: ' +
-                    object['object_name'])
+                    'Name: ' + object_name)
                 current_col += 1
                 worksheet.write(
                     current_row,
                     current_col,
                     'Field: ' +
-                    object['object_field_name'])
+                    values['field_name'])
                 current_col += 1
                 worksheet.write(
                     current_row,
                     current_col,
                     'Table type: ' +
-                    object['object_type'])
+                    values['table_name'])
                 current_col += 1
         # Update max column if it is necessary
         if current_col > max_col:
             max_col = current_col
 
         current_row += 1
         current_col = 0
```

### Comparing `sinergym-2.3.4/sinergym/utils/config.py` & `sinergym-2.4.1/sinergym/config/modeling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,208 +1,332 @@
-"""Class and utilities for set up extra configuration in experiments with Sinergym (extra params, weather_variability, building model modification and files management)"""
+"""Class and utilities for backend modeling in Python with Sinergym (extra params, weather_variability, building model modification and files management)"""
+import json
 import os
 import random
 import xml.etree.cElementTree as ElementTree
+from abc import ABC, abstractmethod
 from copy import deepcopy
+from datetime import datetime, timedelta
 from shutil import rmtree
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas
+from eppy import modeleditor
+from eppy.modeleditor import IDF
 from opyplus import Epm, Idd, WeatherData
 from opyplus.epm.record import Record
 
-from sinergym.utils.common import (get_delta_seconds, get_record_keys,
-                                   prepare_batch_from_records, to_idf)
+from sinergym.utils.common import eppy_element_to_dict, get_delta_seconds
 from sinergym.utils.constants import CWD, PKG_DATA_PATH, WEEKDAY_ENCODING, YEAR
 
 
-class Config(object):
-    """Config object to manage extra configuration in Sinergym experiments.
+class Model(ABC):
+    """Class to determine the Sinergym models' structure.
+    """
+
+    def __init__(self):
+        pass
+
+    # ---------------------------------------------------------------------------- #
+    #                  Variables and Building model adaptation                     #
+    # ---------------------------------------------------------------------------- #
+
+    @abstractmethod
+    def update_weather_path(self) -> None:
+        pass
+
+    @abstractmethod
+    def adapt_building_to_epw(
+            self,
+            summerday: str = 'Ann Clg .4% Condns DB=>MWB',
+            winterday: str = 'Ann Htg 99.6% Condns DB') -> None:
+        pass
+
+    @abstractmethod
+    def adapt_variables_to_cfg_and_building(self) -> None:
+        pass
+
+    @abstractmethod
+    def set_external_interface(self) -> None:
+        pass
+
+    @abstractmethod
+    def apply_extra_conf(self) -> None:
+        pass
+
+    @abstractmethod
+    def adapt_building_to_action_definition(self) -> None:
+        pass
+
+    @abstractmethod
+    def save_variables_cfg(self) -> str:
+        pass
+
+    @abstractmethod
+    def save_building_model(self) -> str:
+        pass
+
+    @abstractmethod
+    def get_schedulers(self) -> Dict[str, Dict[str, Any]]:
+        pass
+
+    # ---------------------------------------------------------------------------- #
+    #                        EPW and Weather Data management                       #
+    # ---------------------------------------------------------------------------- #
+
+    @abstractmethod
+    def apply_weather_variability(
+            self,
+            columns: List[str],
+            variation: Optional[Tuple[float, float, float]]) -> str:
+        pass
+
+    # ---------------------------------------------------------------------------- #
+    #                        Model and Config Functionality                        #
+    # ---------------------------------------------------------------------------- #
+
+    @abstractmethod
+    def _get_eplus_run_info(
+            self) -> Tuple[int, int, int, int, int, int, int, int]:
+        pass
+
+    @abstractmethod
+    def _get_one_epi_len(self) -> float:
+        pass
+
+    # ---------------------------------------------------------------------------- #
+    #                  Working Folder for Simulation Management                    #
+    # ---------------------------------------------------------------------------- #
+
+    @abstractmethod
+    def set_experiment_working_dir(self, env_name: str) -> str:
+        pass
+
+    @abstractmethod
+    def set_episode_working_dir(self) -> str:
+        pass
+
+    @abstractmethod
+    def _get_working_folder(
+            self,
+            directory_path: str,
+            base_name: str) -> str:
+        pass
 
-        :param _idf_path: IDF path origin for apply extra configuration.
+    @abstractmethod
+    def _rm_past_history_dir(
+            self,
+            episode_path: str,
+            base_name: str) -> None:
+        pass
+
+    # ---------------------------------------------------------------------------- #
+    #                             Config class checker                             #
+    # ---------------------------------------------------------------------------- #
+
+    @abstractmethod
+    def _check_eplus_config(self) -> None:
+        pass
+
+    @abstractmethod
+    def _check_observation_variables(self) -> None:
+        pass
+
+
+class ModelJSON(object):
+    """Class to manage backend models (building, weathers...) and folders in Sinergym (JSON version).
+
+        :param _json_path: JSON path origin for apply extra configuration.
         :param weather_files: weather available files for each episode
         :param _weather_path: EPW path origin for apply weather to simulation in current episode.
         :param _ddy_path: DDY path origin for get DesignDays and weather Location
         :param experiment_path: Path for Sinergym experiment output
         :param episode_path: Path for Sinergym specific episode (before first simulator reset this param is None)
         :param max_ep_store: Number of episodes directories will be stored in experiment_path
         :param config: Dict config with extra configuration which is required to modify IDF model (may be None)
         :param _idd: IDD opyplus object to set up Epm
-        :param building: opyplus Epm object with IDF model
+        :param building: Building model (Dictionary extracted from JSON)
         :param ddy_model: opyplus Epm object with DDY model
         :param weather_data: opyplus WeatherData object with EPW data
         :param action_definition: Dict with action definition to automatic building model preparation.
     """
 
     def __init__(
             self,
-            idf_file: str,
+            json_file: str,
             weather_files: List[str],
             variables: Dict[str, List[str]],
             env_name: str,
             max_ep_store: int,
             action_definition: Optional[Dict[str, Any]],
             extra_config: Dict[str, Any]):
 
         self.pkg_data_path = PKG_DATA_PATH
 
-        # Transform IDF file name in path
-        self._idf_path = os.path.join(
-            self.pkg_data_path, 'buildings', idf_file)
+        # ----------------------- Transform filenames in paths ----------------------- #
+
+        # JSON
+        self._json_path = os.path.join(
+            self.pkg_data_path, 'buildings', json_file)
 
-        # Transform EPW file name in path
+        # EPW
         self.weather_files = weather_files
 
+        # IDD
+        self._idd = os.path.join(os.environ['EPLUS_PATH'], 'Energy+.idd')
+
         # Select one weather randomly (if there are more than one)
         self._weather_path = os.path.join(
             self.pkg_data_path, 'weather', random.choice(self.weather_files))
-        # RDD file name is deducible using idf name (only change .idf by .rdd)
+
+        # RDD file name is deducible using json name (only change .epJSON by
+        # .rdd)
         self._rdd_path = os.path.join(
             self.pkg_data_path,
             'variables',
-            self._idf_path.split('/')[-1].split('.idf')[0] +
+            self._json_path.split('/')[-1].split('.epJSON')[0] +
             '.rdd')
+
         # DDY path is deducible using weather_path (only change .epw by .ddy)
         self._ddy_path = self._weather_path.split('.epw')[0] + '.ddy'
-        self.experiment_path = self.set_experiment_working_dir(env_name)
-        self.episode_path = None
-        self.max_ep_store = max_ep_store
 
-        # Set config and action definition as config attribute
-        self.config = extra_config
-        self.action_definition = action_definition
+        # -------------------------------- File Models ------------------------------- #
 
-        # Variables XML Tree (empty at the beginning)
+        # BCVTB variable as XMLtree
         self.variables = variables
         self.variables_tree = ElementTree.Element('BCVTB-variables')
 
-        # Opyplus objects
-        self._idd = Idd(os.path.join(os.environ['EPLUS_PATH'], 'Energy+.idd'))
-        self.building = Epm.from_idf(
-            self._idf_path,
-            idd_or_version=self._idd,
-            check_length=False)
-        self.ddy_model = Epm.from_idf(
-            self._ddy_path,
-            idd_or_version=self._idd,
-            check_length=False)
+        # Building model object (Python dictionaty from epJSON file)
+        with open(self._json_path) as json_f:
+            self.building = json.load(json_f)
+
+        # DDY model (eppy object)
+        IDF.setiddname(self._idd)
+        self.ddy_model = IDF(self._ddy_path)
+
+        # Weather data (opyplus object)
         self.weather_data = WeatherData.from_epw(self._weather_path)
 
-        # Extract idf zone names
-        self.idf_zone_names = []
-        for idf_zone in self.building.Zone:
-            self.idf_zone_names.append(idf_zone.name.lower())
         # Extract rdd observation variables names
         data = pandas.read_csv(self._rdd_path, skiprows=1)
         rdd_variable_names = list(map(
             lambda name: name.split(' [')[0],
             data['Variable Name [Units]'].tolist()))
         rdd_variable_types = data['Var Type (reported time step)'].tolist()
         assert len(rdd_variable_names) == len(
             rdd_variable_types), 'RDD file: Number of variable names and variables types column should be the same.'
         # self.rdd_variables is a dict with keys as name of the variable and
         # body as variable type (Zone or HVAC)
         self.rdd_variables = dict()
         for i, variable_name in enumerate(rdd_variable_names):
             self.rdd_variables[variable_name] = rdd_variable_types[i]
 
+        # ----------------------------- Other attributes ----------------------------- #
+
+        self.experiment_path = self.set_experiment_working_dir(env_name)
+        self.episode_path = None
+        self.max_ep_store = max_ep_store
+        self.config = extra_config
+        self.action_definition = action_definition
+        # Extract building zones
+        self.zone_names = list(self.building['Zone'].keys())
         # Extract schedulers available in building model
         self.schedulers = self.get_schedulers()
 
+        # ------------------------ Checking config definition ------------------------ #
+
         # Check observation variables definition
         self._check_observation_variables()
         # Check config definition
         self._check_eplus_config()
 
     # ---------------------------------------------------------------------------- #
-    #            IDF, variables and Building model adaptation                      #
+    #                 Variables and Building model adaptation                      #
     # ---------------------------------------------------------------------------- #
 
     def update_weather_path(self) -> None:
-        """When this method is called, weather file is changed randomly and IDF is adapted to new one.
+        """When this method is called, weather file is changed randomly and building model is adapted to new one.
         """
         self._weather_path = os.path.join(
             self.pkg_data_path, 'weather', random.choice(self.weather_files))
         self._ddy_path = self._weather_path.split('.epw')[0] + '.ddy'
-        self.ddy_model = Epm.from_idf(
-            self._ddy_path,
-            idd_or_version=self._idd,
-            check_length=False)
+        self.ddy_model = IDF(self._ddy_path)
         self.weather_data = WeatherData.from_epw(self._weather_path)
 
-    def adapt_idf_to_epw(self,
-                         summerday: str = 'Ann Clg .4% Condns DB=>MWB',
-                         winterday: str = 'Ann Htg 99.6% Condns DB') -> None:
-        """Given a summer day name and winter day name from DDY file, this method modify IDF Location and DesingDay's in order to adapt IDF to EPW.
+    def adapt_building_to_epw(
+            self,
+            summerday: str = 'Ann Clg .4% Condns DB=>MWB',
+            winterday: str = 'Ann Htg 99.6% Condns DB') -> None:
+        """Given a summer day name and winter day name from DDY file, this method modify Location and DesingDay's in order to adapt building model to EPW.
 
         Args:
             summerday (str): Design day for summer day specifically (DDY has several of them).
             winterday (str): Design day for winter day specifically (DDY has several of them).
         """
 
-        old_location = self.building.site_location[0]
-        old_designdays = self.building.SizingPeriod_DesignDay
+        # Getting the new location and designdays based on ddy file (Records
+        # must be converted to dictionary)
 
-        # Adding the new location and designdays based on ddy file
         # LOCATION
-        new_location = prepare_batch_from_records(
-            [self.ddy_model.site_location[0]])
-        # DESIGNDAYS
-        winter_designday = self.ddy_model.SizingPeriod_DesignDay.one(
-            lambda designday: winterday.lower() in designday.name.lower())
-        summer_designday = self.ddy_model.SizingPeriod_DesignDay.one(
-            lambda designday: summerday.lower() in designday.name.lower())
-        new_designdays = prepare_batch_from_records(
-            [winter_designday, summer_designday])
-
-        # Deleting the old location and old DesignDays from Epm
-        old_location.delete()
-        old_designdays.delete()
-
-        # Added New Location and DesignDays to Epm
-        self.building.site_location.batch_add(new_location)
-        self.building.SizingPeriod_DesignDay.batch_add(new_designdays)
+        new_location = self.ddy_model.idfobjects['Site:Location'][0]
+        new_location = eppy_element_to_dict(new_location)
 
-    def adapt_variables_to_cfg_and_idf(self) -> None:
-        """This method adds to XML variable tree all observation and action variables information. In addition, it modifies IDF Output:Variable in order to adapt to new observation variables set.
+        # DESIGNDAYS
+        ddy_designdays = self.ddy_model.idfobjects['SizingPeriod:DesignDay']
+        summer_designdays = list(
+            filter(
+                lambda designday: summerday in designday.Name,
+                ddy_designdays))[0]
+        winter_designdays = list(
+            filter(
+                lambda designday: winterday in designday.Name,
+                ddy_designdays))[0]
+        new_designdays = {}
+        new_designdays.update(eppy_element_to_dict(winter_designdays))
+        new_designdays.update(eppy_element_to_dict(summer_designdays))
+
+        # Addeding new location and DesignDays to Building model
+        self.building['Site:Location'] = new_location
+        self.building['SizingPeriod:DesignDay'] = new_designdays
+
+    def adapt_variables_to_cfg_and_building(self) -> None:
+        """This method adds to XML variable tree all observation and action variables information.
+        In addition, it modifies building Output:Variable in order to adapt to new observation variables set.
         """
+
         # OBSERVATION VARIABLES
-        output_variables = []
+        output_variables = {}
         self.variables_tree.append(ElementTree.Comment(
             'Observation variables: Received from EnergyPlus'))
-        for obs_var in self.variables['observation']:
+        for i, obs_var in enumerate(self.variables['observation'], start=1):
             # obs_var = "<variable_name>(<variable_zone>)"
             var_elements = obs_var.split('(')
             var_name = var_elements[0]
             var_zone = var_elements[1][:-1]
 
             # Add obs name and zone to XML variables tree
             new_xml_obs = ElementTree.SubElement(
                 self.variables_tree, 'variable', source='EnergyPlus')
             ElementTree.SubElement(
                 new_xml_obs,
                 'EnergyPlus',
                 name=var_zone,
                 type=var_name)
 
-            # Add IDF record Output:Variable
-            if var_zone.lower() == 'Environment'.lower(
-            ) or var_zone.lower() == 'Whole Building'.lower():
+            # Add element Output:Variable to the building model
+            if var_zone.lower() == 'environment' or var_zone.lower() == 'whole building':
                 var_zone = '*'
-            output_variables.append(
-                dict(
-                    key_value=var_zone,
-                    variable_name=var_name,
-                    reporting_frequency='timestep'))
+            output_variables['Output:Variable ' + str(i)] = {'key_value': var_zone,
+                                                             'variable_name': var_name,
+                                                             'reporting_frequency': 'Timestep'}
 
         # Delete default Output:Variables and added observation_variables
         # specified
-        self.building.output_variable.delete()
-        self.building.output_variable.batch_add(output_variables)
+        self.building['Output:Variable'] = output_variables
 
         # ACTION VARIABLES
         self.variables_tree.append(
             ElementTree.Comment('Action variables: Sent to EnergyPlus'))
         for act_var in self.variables['action']:
 
             new_xml_variable = ElementTree.SubElement(
@@ -213,61 +337,66 @@
                 schedule=act_var)
 
     def set_external_interface(self) -> None:
         """Set an empty external interface with Ptolemy server if is not in the current building
         """
 
         # If no ExternalInterface object found
-        if len(self.building.ExternalInterface) == 0:
+        if 'ExternalInterface' not in self.building:
             # Create PtolemyServer interface in building
-            self.building.ExternalInterface.add(
-                name_of_external_interface='PtolemyServer')
+            self.building['ExternalInterface'] = {
+                'ExternalInterface 1': {
+                    'name_of_external_interface': 'PtolemyServer'}
+            }
 
     def apply_extra_conf(self) -> None:
         """Set extra configuration in building model
         """
         if self.config is not None:
 
             # Timesteps processed in a simulation hour
             if self.config.get('timesteps_per_hour'):
-                self.building.timestep[0].number_of_timesteps_per_hour = self.config['timesteps_per_hour']
+                list(self.building['Timestep'].values())[
+                    0]['number_of_timesteps_per_hour'] = self.config['timesteps_per_hour']
 
             # Runperiod datetimes --> Tuple(start_day, start_month, start_year,
             # end_day, end_month, end_year)
             if self.config.get('runperiod'):
-                runperiod = self.building.RunPeriod[0]
-                runperiod.begin_day_of_month = int(self.config['runperiod'][0])
-                runperiod.begin_month = int(self.config['runperiod'][1])
-                runperiod.begin_year = int(self.config['runperiod'][2])
-                runperiod.end_day_of_month = int(self.config['runperiod'][3])
-                runperiod.end_month = int(self.config['runperiod'][4])
-                runperiod.end_year = int(self.config['runperiod'][5])
+                runperiod = list(self.building['RunPeriod'].values())[0]
+                runperiod['begin_day_of_month'] = int(
+                    self.config['runperiod'][0])
+                runperiod['begin_month'] = int(self.config['runperiod'][1])
+                runperiod['begin_year'] = int(self.config['runperiod'][2])
+                runperiod['end_day_of_month'] = int(
+                    self.config['runperiod'][3])
+                runperiod['end_month'] = int(self.config['runperiod'][4])
+                runperiod['end_year'] = int(self.config['runperiod'][5])
 
-    def adapt_idf_to_action_definition(self) -> None:
-        """Interpret action definition and apply changes in IDF in order to control schedulers specified.
+    def adapt_building_to_action_definition(self) -> None:
+        """Interpret action definition and apply changes in building model, in order to control schedulers specified.
         """
         if self.action_definition is not None:
+            # Create ExternalInterface:Schedule table if it doesn't exist
+            if 'ExternalInterface:Schedule' not in self.building:
+                self.building['ExternalInterface:Schedule'] = {}
             # Iterate in schedulers to control in action definition
             for original_sch_name, new_sch in self.action_definition.items():
                 # Search original scheduler information in building model
-                original_sch = self.schedulers[original_sch_name.lower()]
-                # Add external interface to IDF
-                self.building.ExternalInterface_Schedule.add(
-                    name=new_sch['name'],
-                    schedule_type_limits_name=original_sch['Type'],
-                    initial_value=new_sch['initial_value'])
+                original_sch = self.schedulers[original_sch_name]
+                # Add external interface to building model
+                self.building['ExternalInterface:Schedule'][new_sch['name']] = {
+                    'schedule_type_limits_name': original_sch['Type'],
+                    'initial_value': new_sch['initial_value']
+                }
                 # Look for scheduler elements where appear and substitute for new
                 # one name
-                for key, element in original_sch.items():
-                    if isinstance(element, dict):
-                        table_name = element['object_type'].replace(
-                            ':', '_').replace(' ', '_').lower()
-                        record = self.building._tables[table_name].one(
-                            lambda record: record.name == element['object_name'])
-                        record[element['object_field_name']] = new_sch['name']
+                for sch_name, sch_info in original_sch.items():
+                    if isinstance(sch_info, dict):  # this skip Type key
+                        self.building[sch_info['table_name']][sch_name
+                                                              ][sch_info['field_name']] = new_sch['name']
 
     def save_variables_cfg(self) -> str:
         """This method saves current XML variables tree model into a variables.cfg file.
 
         Raises:
             RuntimeError: If this method is used without an episode_path generated (see reset method in simulator), this exception is raised.
 
@@ -286,61 +415,73 @@
                     '<?xml version="1.0" encoding="ISO-8859-1"?>\n<!DOCTYPE BCVTB-variables SYSTEM "variables.dtd">\n'.encode('utf8'))
                 ElementTree.ElementTree(self.variables_tree).write(f, 'utf-8')
 
             return episode_cfg_path
 
         else:
             raise RuntimeError(
-                '[Simulator Config] Episode path should be set before saving variables.cfg.')
+                '[Simulator Modeling] Episode path should be set before saving variables.cfg.')
 
     def save_building_model(self) -> str:
-        """Take current building model and save as IDF in current env_working_dir episode folder.
+        """Take current building model and save as epJSON in current env_working_dir episode folder.
 
         Returns:
-            str: Path of IDF file stored (episode folder).
+            str: Path of epJSON file stored (episode folder).
         """
-        # If no path specified, then use idf_path to save it.
+
+        # If no path specified, then use json_path to save it.
         if self.episode_path is not None:
-            episode_idf_path = os.path.join(self.episode_path,
-                                            os.path.basename(self._idf_path))
-            # self.building.save(episode_idf_path)
-            to_idf(building=self.building, file_path=episode_idf_path)
-            return episode_idf_path
+            episode_json_path = os.path.join(self.episode_path,
+                                             os.path.basename(self._json_path))
+            with open(episode_json_path, "w") as outfile:
+                json.dump(self.building, outfile, indent=4)
+
+            return episode_json_path
         else:
             raise RuntimeError(
-                '[Simulator Config] Episode path should be set before saving building model.')
+                '[Simulator Modeling] Episode path should be set before saving building model.')
 
-    def get_schedulers(self) -> Dict[str, Any]:
+    def get_schedulers(self) -> Dict[str,
+                                     Dict[str, Union[str, Dict[str, str]]]]:
         """Extract all schedulers available in the building model to be controlled.
 
         Returns:
-            Dict[str, Any]: Python Dictionary: For each scheduler found, it shows type value and where this scheduler is present (Object name, Object field and Object type).
+            Dict[str, Dict[str, Any]]: Python Dictionary: For each scheduler found, it shows type value and where this scheduler is present (table, object and field).
         """
         result = {}
-        schedule_tables = [
-            self.building.schedule_compact,
-            self.building.schedule_year]
-        for schedule_table in schedule_tables:
-            for schedule in schedule_table:
-                object_index = 1
-                result[schedule.name] = {}
-                result[schedule.name]['Type'] = schedule.schedule_type_limits_name.name
-                # Extract objects where scheduler is present as value field
-                for table in self.building:
-                    if table.get_name() != 'Schedule:Compact' and table.get_name() != 'Schedule:Year':
-                        for record in table:
-                            for i, value in enumerate(record):
-                                if isinstance(value, Record):
-                                    if (value._table._dev_descriptor.table_name == 'Schedule:Compact' or value._table._dev_descriptor.table_name ==
-                                            'Schedule:Year') and value.name == schedule.name:
-                                        result[schedule.name]['Object' + str(object_index)] = {'object_name': record.name,
-                                                                                               'object_field_name': record._table._dev_descriptor._field_descriptors[i].ref,
-                                                                                               'object_type': record._table._dev_descriptor.table_name}
-                                        object_index += 1
-
+        schedules = {}
+        # Mount a dict with only building schedulers
+        if 'Schedule:Compact' in self.building:
+            schedules.update(self.building['Schedule:Compact'])
+        if 'Schedule:Year' in self.building:
+            schedules.update(self.building['Schedule:Year'])
+
+        for sch_name, sch_info in schedules.items():
+            # Write sch_name and data type in output
+            result[sch_name] = {
+                'Type': sch_info['schedule_type_limits_name'],
+            }
+            # We are going to search where that scheduler appears in whole
+            # building model
+            for table, elements in self.building.items():
+                # Don't include themselves
+                if table != 'Schedule:Compact' and table != 'Schedule:Year':
+                    # For each object of a table type
+                    for element_name, element_fields in elements.items():
+                        # For each field in a object
+                        for field_key, field_value in element_fields.items():
+                            # If a field value is the schedule name
+                            if field_value == sch_name:
+                                # We annotate the object name as key and the
+                                # field name where sch name appears and the
+                                # table where belong to
+                                result[sch_name][element_name] = {
+                                    'field_name': field_key,
+                                    'table_name': table
+                                }
         return result
 
     # ---------------------------------------------------------------------------- #
     #                        EPW and Weather Data management                       #
     # ---------------------------------------------------------------------------- #
 
     def apply_weather_variability(
@@ -405,71 +546,99 @@
 
     # ---------------------------------------------------------------------------- #
     #                        Model and Config Functionality                        #
     # ---------------------------------------------------------------------------- #
 
     def _get_eplus_run_info(
             self) -> Tuple[int, int, int, int, int, int, int, int]:
-        """This method read the building model from config and finds the running start month, start day, start year, end month, end day, end year, start weekday and the number of steps in a hour simulation. If any value is Unknown, then value will be 0. If step per hour is < 1, then default value will be 4.
+        """This method read the building model from config and finds the running start month, start day, start year, end month, end day, end year, start weekday and the number of steps in a hour simulation.
+        If any value is Unknown, then value will be 0. If step per hour is < 1, then default value will be 4.
 
         Returns:
             Tuple[int, int, int, int, int, int, int, int]: A tuple with: the start month, start day, start year, end month, end day, end year, start weekday and number of steps in a hour simulation.
         """
-        # Get runperiod object inner IDF
-        runperiod = self.building.RunPeriod[0]
+        # Get runperiod object inner building model
+        runperiod = list(self.building['RunPeriod'].values())[0]
 
         # Extract information about runperiod
         start_month = int(
-            0 if runperiod.begin_month is None else runperiod.begin_month)
+            0 if runperiod['begin_month'] is None else runperiod['begin_month'])
         start_day = int(
-            0 if runperiod.begin_day_of_month is None else runperiod.begin_day_of_month)
+            0 if runperiod['begin_day_of_month'] is None else runperiod['begin_day_of_month'])
         start_year = int(
-            YEAR if runperiod.begin_year is None else runperiod.begin_year)
+            YEAR if runperiod['begin_year'] is None else runperiod['begin_year'])
         end_month = int(
-            0 if runperiod.end_month is None else runperiod.end_month)
-        end_day = int(
-            0 if runperiod.end_day_of_month is None else runperiod.end_day_of_month)
+            0 if runperiod['end_month'] is None else runperiod['end_month'])
+        end_day = int(0 if runperiod['end_day_of_month']
+                      is None else runperiod['end_day_of_month'])
         end_year = int(
-            YEAR if runperiod.end_year is None else runperiod.end_year)
-        start_weekday = WEEKDAY_ENCODING[runperiod.day_of_week_for_start_day.lower(
+            YEAR if runperiod['end_year'] is None else runperiod['end_year'])
+        start_weekday = WEEKDAY_ENCODING[runperiod['day_of_week_for_start_day'].lower(
         )]
-        n_steps_per_hour = self.building.timestep[0].number_of_timesteps_per_hour
+        n_steps_per_hour = list(self.building['Timestep'].values())[
+            0]['number_of_timesteps_per_hour']
         if n_steps_per_hour < 1 or n_steps_per_hour is None:  # pragma: no cover
             n_steps_per_hour = 4  # default value
 
         return (
             start_month,
             start_day,
             start_year,
             end_month,
             end_day,
             end_year,
             start_weekday,
             n_steps_per_hour)
 
+    def get_current_time_info(self, sec_elapsed: float) -> List[int]:
+        """Returns the current day, month and hour given the seconds elapsed since the simulation started.
+
+        Args:
+            sec_elapsed (float): Seconds elapsed since the start of the simulation
+
+        Returns:
+            List[int]: A List composed by the current year, day, month and hour in the simulation.
+
+        """
+        runperiod = list(self.building['RunPeriod'].values())[0]
+        start_date = datetime(
+            year=int(
+                YEAR if runperiod['begin_year'] is None else runperiod['begin_year']), month=int(
+                1 if runperiod['begin_month'] is None else runperiod['begin_month']), day=int(
+                1 if runperiod['begin_day_of_month'] is None else runperiod['begin_day_of_month']))
+
+        current_date = start_date + timedelta(seconds=sec_elapsed)
+
+        return [
+            int(current_date.year),
+            int(current_date.month),
+            int(current_date.day),
+            int(current_date.hour),
+        ]
+
     def _get_one_epi_len(self) -> float:
         """Gets the length of one episode (an EnergyPlus process run to the end) depending on the config of simulation.
 
         Returns:
-            float: The simulation time step in which the simulation ends.
+            float: The simulation time in which the simulation ends (seconds).
         """
-        # Get runperiod object inner IDF
-        runperiod = self.building.RunPeriod[0]
+        # Get runperiod object inner building model
+        runperiod = list(self.building['RunPeriod'].values())[0]
         start_year = int(
-            YEAR if runperiod.begin_year is None else runperiod.begin_year)
+            YEAR if runperiod['begin_year'] is None else runperiod['begin_year'])
         start_month = int(
-            0 if runperiod.begin_month is None else runperiod.begin_month)
+            0 if runperiod['begin_month'] is None else runperiod['begin_month'])
         start_day = int(
-            0 if runperiod.begin_day_of_month is None else runperiod.begin_day_of_month)
+            0 if runperiod['begin_day_of_month'] is None else runperiod['begin_day_of_month'])
         end_year = int(
-            YEAR if runperiod.end_year is None else runperiod.end_year)
+            YEAR if runperiod['end_year'] is None else runperiod['end_year'])
         end_month = int(
-            0 if runperiod.end_month is None else runperiod.end_month)
-        end_day = int(
-            0 if runperiod.end_day_of_month is None else runperiod.end_day_of_month)
+            0 if runperiod['end_month'] is None else runperiod['end_month'])
+        end_day = int(0 if runperiod['end_day_of_month']
+                      is None else runperiod['end_day_of_month'])
 
         return get_delta_seconds(
             start_year,
             start_month,
             start_day,
             end_year,
             end_month,
@@ -633,15 +802,15 @@
                 assert set(
                     new_sch.keys()) == set(
                     ['name', 'initial_value']), 'Action definition: keys in new scheduler definition must be name and initial_value.'
                 assert isinstance(
                     new_sch['name'], str), 'Action definition: Name field in new scheduler must be a str element.'
                 # Check action definition component is in schedulers available
                 # in building model
-                assert original_sch_name.lower() in self.schedulers.keys(
+                assert original_sch_name in self.schedulers.keys(
                 ), 'Action definition: Object called {} is not an existing component in building model.'.format(original_sch_name)
                 # Check new variable is present in action variables
                 assert new_sch['name'] in self.variables['action'], 'Action definition: {} external variable should be in action variables.'.format(
                     new_sch['name'])
 
     def _check_observation_variables(self) -> None:
         """This method checks whether observation variables are available in building model definition (Checking variable type definition too).
@@ -650,50 +819,22 @@
             # Name of the observation variable and element (Zone or HVAC
             # element name)
             obs_name = obs_var.split('(')[0]
             obs_element_name = obs_var.split('(')[1][:-1]
 
             # Check observarion variables names
             assert obs_name in list(self.rdd_variables.keys(
-            )), 'Observation variables: Variable called {} in observation variables is not valid for IDF building model'.format(obs_name)
+            )), 'Observation variables: Variable called {} in observation variables is not valid for the building model'.format(obs_name)
             # Check observation variables about zones (if variable type is
             # Zone)
             if self.rdd_variables[obs_name] == 'Zone':
                 # Check that obs zone is not Environment or Whole building tag
                 if obs_element_name.lower() != 'Environment'.lower(
                 ) and obs_element_name.lower() != 'Whole Building'.lower():
                     # zones names with people 1 or lights 1, etc. The second name
                     # is ignored, only check that zone is a substr from obs
                     # zone
-                    assert any(list(map(lambda zone: zone.lower() in obs_element_name.lower(), self.idf_zone_names))
-                               ), 'Observation variables: Zone called {} in observation variables does not exist in IDF building model.'.format(obs_element_name)
+                    assert any(list(map(lambda zone: zone.lower() in obs_element_name.lower(), self.zone_names))
+                               ), 'Observation variables: Zone called {} in observation variables does not exist in the building model.'.format(obs_element_name)
             # Check observation variables about HVAC
             elif self.rdd_variables[obs_name] == 'HVAC':
                 pass
-
-                # ---------------------------------------------------------------------------- #
-                #                                    OTHERS                                    #
-                # ---------------------------------------------------------------------------- #
-
-                # def _set_thermostat_zone_control(self,
-                #                                  zone_control: Record,
-                #                                  controller_type: str,
-                #                                  controller: Dict[str,
-                #                                                   Any]) -> None:
-                #     """Modify Thermostat:ZoneControl object from IDF model in order to set a new controller
-
-                #     Args:
-                #         zone_control (Record): Zone Control to be modified.
-                #         controller_type (str): Controller type you want to change.
-                #         controller (Dict[str, Any]): controller to set in Zone Control.
-                #     """
-                #     # We iterate all record fields searching
-                #     # controller_type value
-                #     for i in range(len(get_record_keys(zone_control))):
-                #         if isinstance(zone_control[i], str):
-                #             if zone_control[i].lower() == controller_type.lower():
-                #                 # Then, the next field will be always the DualSetpoint
-                #                 # thermostat name, so we change it
-                #                 zone_control[i + 1] = controller['name']
-                #                 # We do not need to search more fields in that record
-                #                 # specifically, so break it
-                #                 break
```

### Comparing `sinergym-2.3.4/sinergym/utils/constants.py` & `sinergym-2.4.1/sinergym/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/utils/controllers.py` & `sinergym-2.4.1/sinergym/utils/controllers.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/utils/env_checker.py` & `sinergym-2.4.1/sinergym/utils/env_checker.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/utils/evaluation.py` & `sinergym-2.4.1/sinergym/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/utils/gcloud.py` & `sinergym-2.4.1/sinergym/utils/gcloud.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/utils/logger.py` & `sinergym-2.4.1/sinergym/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,22 @@
 import csv
 import logging
 import os
 import sys
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
-import wandb
-from stable_baselines3.common.logger import KVWriter, Logger
+import pkg_resources
+
+required = {'stable-baselines3', 'wandb'}
+installed = {pkg.key for pkg in pkg_resources.working_set}
+missing = required - installed
+if not missing:
+    import wandb
+    from stable_baselines3.common.logger import KVWriter
 
 
 class Logger():
     """Sinergym terminal logger for simulation executions.
     """
 
     def getLogger(
@@ -300,29 +306,30 @@
 
     def deactivate_flag(self) -> None:
         """Deactivate Sinergym CSV logger
         """
         self.flag = False
 
 
-class WandBOutputFormat(KVWriter):
-    """
-    Dumps key/value pairs onto WandB. This class is based on SB3 used in logger callback
-    """
+if not missing:
+    class WandBOutputFormat(KVWriter):
+        """
+        Dumps key/value pairs onto WandB. This class is based on SB3 used in logger callback
+        """
 
-    def write(
-        self,
-        key_values: Dict[str, Any],
-        key_excluded: Dict[str, Union[str, Tuple[str, ...]]],
-        step: int = 0,
-    ) -> None:
-
-        for (key, value), (_, excluded) in zip(
-            sorted(key_values.items()), sorted(key_excluded.items())
-        ):
-
-            if excluded is not None and "wandb" in excluded:
-                continue
-
-            if isinstance(value, np.ScalarType):
-                if not isinstance(value, str):
-                    wandb.log({key: value}, step=step)
+        def write(
+            self,
+            key_values: Dict[str, Any],
+            key_excluded: Dict[str, Union[str, Tuple[str, ...]]],
+            step: int = 0,
+        ) -> None:
+
+            for (key, value), (_, excluded) in zip(
+                sorted(key_values.items()), sorted(key_excluded.items())
+            ):
+
+                if excluded is not None and "wandb" in excluded:
+                    continue
+
+                if isinstance(value, np.ScalarType):
+                    if not isinstance(value, str):
+                        wandb.log({key: value}, step=step)
```

### Comparing `sinergym-2.3.4/sinergym/utils/rewards.py` & `sinergym-2.4.1/sinergym/utils/rewards.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.4/sinergym/utils/wrappers.py` & `sinergym-2.4.1/sinergym/utils/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,16 +489,17 @@
         # Params
         self.env = env
         self.current_setpoints = []
         self.max_values = max_values
         self.min_values = min_values
 
         # calculate initial values for setpoints
-        for external_schedule in self.env.simulator._config.building.ExternalInterface_Schedule:
-            self.current_setpoints.append(external_schedule.initial_value)
+        for external_schedule in list(
+                self.env.simulator._config.building['ExternalInterface:Schedule'].values()):
+            self.current_setpoints.append(external_schedule['initial_value'])
 
         # Check environment is valid
         assert len(
             self.current_setpoints) == len(
             self.env.variables['action']), 'IncrementalWrapper: Number of variables is different from environment'
         assert len(
             self.current_setpoints) == len(
@@ -549,20 +550,20 @@
 
     # ---------------------- Specific environment wrappers ---------------------#
 
 
 class OfficeGridStorageSmoothingActionConstraintsWrapper(
         gym.ActionWrapper):  # pragma: no cover
     def __init__(self, env):
-        assert env.idf_path.split(
-            '/')[-1] == 'OfficeGridStorageSmoothing.idf', 'OfficeGridStorageSmoothingActionConstraintsWrapper: This wrapper is not valid for this environment.'
+        assert env.building_path.split(
+            '/')[-1] == 'OfficeGridStorageSmoothing.epJSON', 'OfficeGridStorageSmoothingActionConstraintsWrapper: This wrapper is not valid for this environment.'
         super().__init__(env)
 
     def action(self, act: np.ndarray) -> np.ndarray:
-        """Due to Charge rate and Discharge rate can't be more than 0.0 simultaneously (in OfficeGridStorageSmoothing.idf),
+        """Due to Charge rate and Discharge rate can't be more than 0.0 simultaneously (in OfficeGridStorageSmoothing.epJSON),
            this wrapper clips one of the to 0.0 when both have a value upper than 0.0 (randomly).
 
         Args:
             act (np.ndarray): Action to be clipped
 
         Returns:
             np.ndarray: Action Clipped
```

### Comparing `sinergym-2.3.4/sinergym.egg-info/PKG-INFO` & `sinergym-2.4.1/sinergym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 2.3.4
+Version: 2.4.1
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 2.3.4 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 2.4.1 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-2.3.4/sinergym.egg-info/SOURCES.txt` & `sinergym-2.4.1/sinergym.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 sinergym/__init__.py
 sinergym/version.txt
 sinergym.egg-info/PKG-INFO
 sinergym.egg-info/SOURCES.txt
 sinergym.egg-info/dependency_links.txt
 sinergym.egg-info/requires.txt
 sinergym.egg-info/top_level.txt
-sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf
-sinergym/data/buildings/5ZoneAutoDXVAV.idf
-sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf
-sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf
-sinergym/data/buildings/OfficeGridStorageSmoothing.idf
-sinergym/data/buildings/ShopWithVandBattery.idf
+sinergym/config/__init__.py
+sinergym/config/modeling.py
+sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON
+sinergym/data/buildings/5ZoneAutoDXVAV.epJSON
+sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.epJSON
+sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.epJSON
+sinergym/data/buildings/OfficeGridStorageSmoothing.epJSON
+sinergym/data/buildings/ShopWithVandBattery.epJSON
 sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
 sinergym/data/variables/5ZoneAutoDXVAV.rdd
 sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd
 sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd
 sinergym/data/variables/OfficeGridStorageSmoothing.rdd
 sinergym/data/variables/ShopWithVandBattery.rdd
 sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
@@ -54,15 +56,14 @@
 sinergym/simulators/__init__.py
 sinergym/simulators/base.py
 sinergym/simulators/eplus.py
 sinergym/simulators/eplus_alpha.py
 sinergym/utils/__init__.py
 sinergym/utils/callbacks.py
 sinergym/utils/common.py
-sinergym/utils/config.py
 sinergym/utils/constants.py
 sinergym/utils/controllers.py
 sinergym/utils/env_checker.py
 sinergym/utils/evaluation.py
 sinergym/utils/gcloud.py
 sinergym/utils/logger.py
 sinergym/utils/rewards.py
```

### Comparing `sinergym-2.3.4/sinergym.egg-info/requires.txt` & `sinergym-2.4.1/sinergym.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 autopep8
 eppy
 gymnasium
 isort
 numpy
 opyplus
 pandas
+pipdeptree
 pytype
 twine
 xlsxwriter
 
 [DRL]
 stable-baselines3==2.0.0a5
 wandb
@@ -18,15 +19,15 @@
 nbsphinx
 nbsphinx_link
 pyenchant
 sphinx
 sphinx-multitoc-numbering
 sphinx-multiversion@ git+https://github.com/Holzhaus/sphinx-multiversion#egg=sphinx-multiversion
 sphinx-rtd-theme
-sphinxcontrib-jquery==2.0.0
+sphinxcontrib-jquery
 sphinxcontrib-spelling
 
 [extras]
 IPython
 google-api-python-client==2.58.0
 google-cloud-storage==2.5.0
 matplotlib
@@ -37,26 +38,24 @@
 pytest
 pytest-cov
 pytest-xdist
 sphinx
 sphinx-multitoc-numbering
 sphinx-multiversion@ git+https://github.com/Holzhaus/sphinx-multiversion#egg=sphinx-multiversion
 sphinx-rtd-theme
-sphinxcontrib-jquery==2.0.0
+sphinxcontrib-jquery
 sphinxcontrib-spelling
 stable-baselines3==2.0.0a5
 wandb
 
 [gcloud]
 google-api-python-client==2.58.0
 google-cloud-storage==2.5.0
 oauth2client==4.1.3
 
 [test]
 pytest
 pytest-cov
 pytest-xdist
-stable-baselines3==2.0.0a5
-wandb
 
 [visualization]
 matplotlib
```

