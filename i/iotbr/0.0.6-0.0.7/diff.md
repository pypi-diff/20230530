# Comparing `tmp/iotbr-0.0.6.tar.gz` & `tmp/iotbr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotbr-0.0.6.tar", last modified: Tue May 30 16:12:33 2023, max compression
+gzip compressed data, was "iotbr-0.0.7.tar", last modified: Tue May 30 20:34:32 2023, max compression
```

## Comparing `iotbr-0.0.6.tar` & `iotbr-0.0.7.tar`

### file list

```diff
@@ -1,272 +1,272 @@
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 16:12:33.844331 iotbr-0.0.6/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     1080 2023-05-01 17:49:02.000000 iotbr-0.0.6/LICENSE
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      229 2023-05-06 21:48:33.000000 iotbr-0.0.6/MANIFEST.in
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   146122 2023-05-30 16:12:33.844331 iotbr-0.0.6/PKG-INFO
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   145676 2023-05-24 20:25:10.000000 iotbr-0.0.6/README.md
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 16:12:33.628328 iotbr-0.0.6/iotbr/
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 16:12:33.628328 iotbr-0.0.6/iotbr/IBGE/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     4960 2023-05-05 18:36:06.000000 iotbr-0.0.6/iotbr/IBGE/dictionary_1.csv
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 16:12:33.672329 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2000.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2001.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2002.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2003.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2004.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2005.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2006.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2007.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2008.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2009.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    47104 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2010.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    47104 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    47104 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    47104 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    47104 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    47616 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51200 2019-10-16 14:02:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    47616 2020-09-14 19:16:14.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    48128 2020-10-06 13:56:14.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    50176 2021-09-17 17:20:56.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    50688 2022-09-16 17:58:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2020.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2000.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2001.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2002.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2003.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2004.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2005.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2006.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2007.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2008.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2009.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2010.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2019-11-07 14:08:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    69120 2019-10-16 14:02:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2020-09-14 19:15:04.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2020-09-14 19:49:06.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    62976 2021-09-17 17:21:00.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    62976 2022-09-16 17:58:04.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2020.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2001.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2002.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2003.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2004.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2005.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    48128 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2006.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    48128 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2007.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    48128 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2008.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    48128 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2009.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    48128 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2010.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    48640 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    48640 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    48640 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    48640 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    48640 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    52224 2019-10-16 14:02:36.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49152 2020-09-14 19:17:14.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    49152 2020-09-14 19:46:16.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51200 2021-09-17 17:21:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2022-09-16 17:58:06.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2020.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2001.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2002.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2003.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2004.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2005.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2006.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2007.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2008.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2009.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2010.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2019-11-07 14:08:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2019-11-07 14:08:36.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2019-11-07 14:08:36.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    62464 2019-10-16 14:02:38.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2020-09-14 19:18:58.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2020-09-14 19:56:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    57856 2021-09-17 17:21:04.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    57856 2022-09-16 17:58:06.000000 iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2020.xls
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 16:12:33.700329 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2010.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    55808 2019-10-16 14:03:20.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    52224 2020-09-14 19:21:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    52224 2020-09-14 19:41:20.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    55808 2021-09-17 17:21:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2022-09-16 17:58:20.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2020.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    75264 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2010.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    78848 2019-10-16 14:03:22.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2020-09-14 19:23:14.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2020-09-14 19:41:54.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    74752 2021-09-17 17:21:36.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    74752 2022-09-16 17:58:22.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2020.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    55808 2019-10-16 14:03:26.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    52224 2020-09-14 19:22:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    52224 2020-09-14 19:50:12.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    55808 2021-09-17 17:21:40.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    55808 2022-09-16 17:58:24.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2020.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2019-11-07 14:10:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    68608 2019-10-16 14:03:28.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2020-09-14 19:21:56.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2020-09-14 19:50:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    63488 2021-09-17 17:21:42.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    63488 2022-09-16 17:58:26.000000 iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2020.xls
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 16:12:33.792330 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2000.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   126464 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2001.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   125952 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2002.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   124928 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2003.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   125440 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2004.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2005.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2006.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2007.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2008.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   130560 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2009.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   101376 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2010.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   141312 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   106496 2019-10-16 14:04:16.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2020-09-15 17:23:48.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2020-09-15 17:31:40.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   309248 2021-09-23 23:57:38.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   110592 2022-09-22 13:14:22.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2020.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2000.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2001.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2002.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2003.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2004.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2005.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2006.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2007.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2008.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2009.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   114688 2019-11-07 14:12:30.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2010.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   154112 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   115200 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   115200 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   115200 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   115200 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   122880 2019-10-16 14:04:20.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   115712 2020-09-15 17:43:56.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   115200 2020-09-15 17:46:26.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   350720 2021-09-24 00:02:28.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   119808 2022-09-22 13:11:42.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2020.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   126464 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2001.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   125952 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2002.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   124928 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2003.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   125440 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2004.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2005.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2006.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2007.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2008.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   126976 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2009.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   128512 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2010.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   108032 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   106496 2019-10-16 14:04:22.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2021-11-12 12:55:04.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2021-11-12 12:55:38.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   110080 2021-11-12 12:53:56.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   110592 2022-09-22 13:11:12.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2020.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   147456 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2001.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2002.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2003.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2004.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2005.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2006.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2007.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2008.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2009.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   147456 2019-11-07 14:12:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2010.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   146432 2019-11-07 14:12:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   107520 2019-11-07 14:12:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   107520 2019-11-07 14:12:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   107520 2019-11-07 14:12:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   107520 2019-11-07 14:12:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   114176 2019-10-16 14:04:24.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   107520 2021-11-12 12:56:08.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   107520 2021-11-12 12:54:18.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   111616 2021-11-12 12:51:16.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   111616 2022-09-23 13:27:22.000000 iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2020.xls
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 16:12:33.844331 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   140288 2019-11-07 14:09:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2010.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:32.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   141312 2019-10-16 14:05:16.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   139264 2020-09-14 19:24:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   139264 2020-09-14 19:55:38.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   158720 2021-09-17 17:21:54.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   158720 2022-09-16 17:58:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2020.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   159232 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2010.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   159744 2019-10-16 14:05:18.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2020-09-14 19:25:26.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2020-09-14 19:56:10.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   171008 2021-09-17 17:21:58.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   171008 2022-09-16 17:58:36.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2020.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   141312 2019-10-16 14:05:20.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   139264 2020-09-14 19:24:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   139264 2020-09-14 19:49:38.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   158208 2021-09-17 17:22:02.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   158720 2022-09-16 17:58:36.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2020.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   140800 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2011.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   140800 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2012.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   140800 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2013.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   140800 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2014.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   140800 2019-11-07 14:09:34.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2015.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   145920 2019-10-16 14:05:24.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2016.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   140800 2020-09-14 19:24:58.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2017.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   140288 2020-09-15 02:05:08.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2018.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   153600 2021-09-17 17:22:04.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2019.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   153600 2022-09-16 17:58:38.000000 iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2020.xls
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-04-01 21:15:48.000000 iotbr-0.0.6/iotbr/__init__.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     8509 2023-05-30 16:10:49.000000 iotbr-0.0.6/iotbr/io_system.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     4474 2023-05-10 21:18:08.000000 iotbr-0.0.6/iotbr/tru.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     5067 2023-05-10 21:44:43.000000 iotbr-0.0.6/iotbr/tru_pb.py
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 16:12:33.628328 iotbr-0.0.6/iotbr.egg-info/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   146122 2023-05-30 16:12:33.000000 iotbr-0.0.6/iotbr.egg-info/PKG-INFO
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    12940 2023-05-30 16:12:33.000000 iotbr-0.0.6/iotbr.egg-info/SOURCES.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        1 2023-05-30 16:12:33.000000 iotbr-0.0.6/iotbr.egg-info/dependency_links.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        5 2023-05-30 16:12:33.000000 iotbr-0.0.6/iotbr.egg-info/requires.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        6 2023-05-30 16:12:33.000000 iotbr-0.0.6/iotbr.egg-info/top_level.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      103 2021-04-01 21:15:48.000000 iotbr-0.0.6/pyproject.toml
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      593 2023-05-30 16:12:33.844331 iotbr-0.0.6/setup.cfg
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 20:34:32.447476 iotbr-0.0.7/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     1080 2023-05-01 17:49:02.000000 iotbr-0.0.7/LICENSE
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      229 2023-05-06 21:48:33.000000 iotbr-0.0.7/MANIFEST.in
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   146122 2023-05-30 20:34:32.447476 iotbr-0.0.7/PKG-INFO
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   145676 2023-05-24 20:25:10.000000 iotbr-0.0.7/README.md
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 20:34:32.191402 iotbr-0.0.7/iotbr/
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 20:34:32.195403 iotbr-0.0.7/iotbr/IBGE/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     4959 2023-05-30 20:29:54.000000 iotbr-0.0.7/iotbr/IBGE/dictionary_1.csv
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 20:34:32.251420 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2000.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2001.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2002.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2003.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2004.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2005.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2006.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2007.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2008.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2009.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    47104 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2010.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    47104 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    47104 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    47104 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    47104 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    47616 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51200 2019-10-16 14:02:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    47616 2020-09-14 19:16:14.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    48128 2020-10-06 13:56:14.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    50176 2021-09-17 17:20:56.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    50688 2022-09-16 17:58:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2020.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2000.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2001.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2002.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2003.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2004.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2005.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2006.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2007.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2008.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    64512 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2009.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2010.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2019-11-07 14:08:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    69120 2019-10-16 14:02:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2020-09-14 19:15:04.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    60416 2020-09-14 19:49:06.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    62976 2021-09-17 17:21:00.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    62976 2022-09-16 17:58:04.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2020.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2001.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2002.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2003.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2004.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49664 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2005.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    48128 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2006.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    48128 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2007.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    48128 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2008.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    48128 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2009.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    48128 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2010.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    48640 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    48640 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    48640 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    48640 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    48640 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    52224 2019-10-16 14:02:36.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49152 2020-09-14 19:17:14.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    49152 2020-09-14 19:46:16.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51200 2021-09-17 17:21:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2022-09-16 17:58:06.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2020.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2001.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2002.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2003.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2004.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2005.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2006.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2007.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2008.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2009.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    58368 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2010.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2019-11-07 14:08:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2019-11-07 14:08:36.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2019-11-07 14:08:36.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    62464 2019-10-16 14:02:38.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2020-09-14 19:18:58.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2020-09-14 19:56:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    57856 2021-09-17 17:21:04.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    57856 2022-09-16 17:58:06.000000 iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2020.xls
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 20:34:32.287430 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2010.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    55808 2019-10-16 14:03:20.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    52224 2020-09-14 19:21:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    52224 2020-09-14 19:41:20.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    55808 2021-09-17 17:21:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    56320 2022-09-16 17:58:20.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2020.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    75264 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2010.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    78848 2019-10-16 14:03:22.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2020-09-14 19:23:14.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    70656 2020-09-14 19:41:54.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    74752 2021-09-17 17:21:36.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    74752 2022-09-16 17:58:22.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2020.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    51712 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    55808 2019-10-16 14:03:26.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    52224 2020-09-14 19:22:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    52224 2020-09-14 19:50:12.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    55808 2021-09-17 17:21:40.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    55808 2022-09-16 17:58:24.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2020.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2019-11-07 14:10:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    68608 2019-10-16 14:03:28.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2020-09-14 19:21:56.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    61440 2020-09-14 19:50:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    63488 2021-09-17 17:21:42.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    63488 2022-09-16 17:58:26.000000 iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2020.xls
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 20:34:32.387459 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2000.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   126464 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2001.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   125952 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2002.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   124928 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2003.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   125440 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2004.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2005.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2006.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2007.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2008.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   130560 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2009.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   101376 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2010.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   141312 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   106496 2019-10-16 14:04:16.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2020-09-15 17:23:48.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2020-09-15 17:31:40.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   309248 2021-09-23 23:57:38.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   110592 2022-09-22 13:14:22.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2020.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2000.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2001.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2002.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2003.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2004.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2005.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2006.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2007.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2008.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   161792 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2009.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   114688 2019-11-07 14:12:30.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2010.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   154112 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   115200 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   115200 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   115200 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   115200 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   122880 2019-10-16 14:04:20.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   115712 2020-09-15 17:43:56.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   115200 2020-09-15 17:46:26.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   350720 2021-09-24 00:02:28.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   119808 2022-09-22 13:11:42.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2020.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   126464 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2001.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   125952 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2002.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   124928 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2003.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   125440 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2004.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2005.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2006.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2007.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   127488 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2008.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   126976 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2009.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   128512 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2010.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   108032 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   106496 2019-10-16 14:04:22.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2021-11-12 12:55:04.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   102912 2021-11-12 12:55:38.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   110080 2021-11-12 12:53:56.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   110592 2022-09-22 13:11:12.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2020.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   147456 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2001.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2002.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2003.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2004.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2005.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2006.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2007.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2008.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   147968 2019-11-07 14:12:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2009.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   147456 2019-11-07 14:12:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2010.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   146432 2019-11-07 14:12:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   107520 2019-11-07 14:12:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   107520 2019-11-07 14:12:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   107520 2019-11-07 14:12:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   107520 2019-11-07 14:12:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   114176 2019-10-16 14:04:24.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   107520 2021-11-12 12:56:08.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   107520 2021-11-12 12:54:18.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   111616 2021-11-12 12:51:16.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   111616 2022-09-23 13:27:22.000000 iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2020.xls
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 20:34:32.443475 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   140288 2019-11-07 14:09:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2010.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:32.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   141312 2019-10-16 14:05:16.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   139264 2020-09-14 19:24:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   139264 2020-09-14 19:55:38.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   158720 2021-09-17 17:21:54.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   158720 2022-09-16 17:58:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2020.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   159232 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2010.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   159744 2019-10-16 14:05:18.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2020-09-14 19:25:26.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   153088 2020-09-14 19:56:10.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   171008 2021-09-17 17:21:58.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   171008 2022-09-16 17:58:36.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2020.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   138752 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   141312 2019-10-16 14:05:20.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   139264 2020-09-14 19:24:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   139264 2020-09-14 19:49:38.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   158208 2021-09-17 17:22:02.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   158720 2022-09-16 17:58:36.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2020.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   140800 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2011.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   140800 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2012.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   140800 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2013.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   140800 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2014.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   140800 2019-11-07 14:09:34.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2015.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   145920 2019-10-16 14:05:24.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2016.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   140800 2020-09-14 19:24:58.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2017.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   140288 2020-09-15 02:05:08.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2018.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   153600 2021-09-17 17:22:04.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2019.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   153600 2022-09-16 17:58:38.000000 iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2020.xls
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-04-01 21:15:48.000000 iotbr-0.0.7/iotbr/__init__.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     8509 2023-05-30 16:10:49.000000 iotbr-0.0.7/iotbr/io_system.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     4474 2023-05-10 21:18:08.000000 iotbr-0.0.7/iotbr/tru.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     5067 2023-05-10 21:44:43.000000 iotbr-0.0.7/iotbr/tru_pb.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-05-30 20:34:32.195403 iotbr-0.0.7/iotbr.egg-info/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   146122 2023-05-30 20:34:32.000000 iotbr-0.0.7/iotbr.egg-info/PKG-INFO
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    12940 2023-05-30 20:34:32.000000 iotbr-0.0.7/iotbr.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        1 2023-05-30 20:34:32.000000 iotbr-0.0.7/iotbr.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        5 2023-05-30 20:34:32.000000 iotbr-0.0.7/iotbr.egg-info/requires.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        6 2023-05-30 20:34:32.000000 iotbr-0.0.7/iotbr.egg-info/top_level.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      103 2021-04-01 21:15:48.000000 iotbr-0.0.7/pyproject.toml
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      593 2023-05-30 20:34:32.447476 iotbr-0.0.7/setup.cfg
```

### Comparing `iotbr-0.0.6/LICENSE` & `iotbr-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/PKG-INFO` & `iotbr-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotbr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Import data from Table of Input-Output from IBGE
 Home-page: https://github.com/fms-1988
 Author: Felipe Morelli Da Silva
 Author-email: fms.morelli@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iotbr-0.0.6/README.md` & `iotbr-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/dictionary_1.csv` & `iotbr-0.0.7/iotbr/IBGE/dictionary_1.csv`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 CIF_FOB,importacao,tab1,12,x,x,x,x,12,vector,vector | Ajuste CIF/FOB |  ,2010
 M_bens,importacao,tab1,12,x,x,x,x,12,vector,vector | Importação de bens |  ,2010
 M_serv,importacao,tab1,12,x,x,x,x,12,vector,vector | Importação de serviços |  ,2010
 CI_matrix,CI,tab2,12,2,2,1,2,12,matrix,matrix | Consumo intermediário das atividades |  ,2010
 D_ci,CI,tab2,12,14,22,52,70,12,vector,vector | Total do produto (Tabela 2 CI) |  ,2010
 X_bens,demanda,tab2,12,x,x,x,x,12,vector,vector | Exportação de bens  |  ,2010
 X_serv,demanda,tab2,12,x,x,x,x,12,vector,vector | Exportação de serviços |  ,2010
-C_g,demanda,tab2,12,4,3,3,3,12,vector,vector | Consumo da administração pública |  ,2010
-C_ong,demanda,tab2,12,5,4,4,4,12,vector,vector | Consumo das  ISFLSF |  ,2010
-C_f,demanda,tab2,12,6,5,5,5,12,vector,vector | Consumo das famílias |  ,2010
-FBKF,demanda,tab2,12,7,6,6,6,12,vector,vector | Formação bruta de capital fixo |  ,2010
-DE,demanda,tab2,12,8,7,7,7,12,vector,vector | Variação de estoque |  ,2010
-D_final,demanda,tab2,12,9,8,8,8,12,vector,vector | Demanda final |  ,2010
-D_total,demanda,tab2,12,10,9,9,9,12,vector,vector | Demanda total |  ,2010
+C_g,demanda,tab2,12,3,3,3,3,12,vector,vector | Consumo da administração pública |  ,2010
+C_ong,demanda,tab2,12,4,4,4,4,12,vector,vector | Consumo das  ISFLSF |  ,2010
+C_f,demanda,tab2,12,5,5,5,5,12,vector,vector | Consumo das famílias |  ,2010
+FBKF,demanda,tab2,12,6,6,6,6,12,vector,vector | Formação bruta de capital fixo |  ,2010
+DE,demanda,tab2,12,7,7,7,7,12,vector,vector | Variação de estoque |  ,2010
+D_final,demanda,tab2,12,8,8,8,8,12,vector,vector | Demanda final |  ,2010
+D_total,demanda,tab2,12,9,9,9,9,12,vector,vector | Demanda total |  ,2010
 VA_table,VA,tab2,12,1,1,1,1,14–14--12--14,table,matrix | Componentes do valor adicionado |  ,2010
 M_bens_serv,importacao,tab1,12,2,2,1,2,12,vector,Importação de bens e serviços (1) (1) Importação de bens e serviços líquida de ajuste CIF/FOB.,2010
 X_bens_serv,demanda,tab2,12,2,2,1,2,12,vector,(1) Importação de bens e serviços líquida de ajuste CIF/FOB.,2010
 OT_pm,oferta,tab1,12,2,x,1,x,12,vector,vector | Oferta total a preço de consumidor |  ,2000
 MG_com,oferta,tab1,12,3,x,2,x,12,vector,vector | Margem de comércio |  ,2000
 MG_tra,oferta,tab1,12,4,x,3,x,12,vector,vector | Margem de transporte |  ,2000
 I_imp,oferta,tab1,12,5,x,4,x,12,vector,vector | Imposto de importação |  ,2000
```

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2000.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2000.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2001.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2001.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2002.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2002.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2003.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2003.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2004.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2004.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2005.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2005.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2006.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2006.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2007.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2007.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2008.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2008.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2009.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2009.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2010.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2010.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab1_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2000.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2000.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2001.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2001.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2002.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2002.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2003.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2003.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2004.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2004.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2005.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2005.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2006.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2006.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2007.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2007.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2008.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2008.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2009.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2009.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2010.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2010.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab2_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2001.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2001.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2002.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2002.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2003.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2003.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2004.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2004.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2005.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2005.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2006.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2006.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2007.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2007.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2008.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2008.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2009.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2009.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2010.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2010.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab3_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2001.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2001.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2002.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2002.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2003.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2003.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2004.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2004.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2005.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2005.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2006.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2006.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2007.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2007.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2008.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2008.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2009.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2009.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2010.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2010.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_12_2000_2020_xls/12_tab4_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2010.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2010.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab1_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2010.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2010.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab2_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab3_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_20_2010_2020_xls/20_tab4_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2000.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2000.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2001.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2001.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2002.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2002.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2003.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2003.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2004.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2004.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2005.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2005.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2006.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2006.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2007.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2007.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2008.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2008.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2009.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2009.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2010.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2010.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab1_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2000.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2000.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2001.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2001.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2002.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2002.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2003.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2003.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2004.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2004.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2005.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2005.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2006.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2006.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2007.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2007.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2008.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2008.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2009.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2009.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2010.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2010.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab2_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2001.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2001.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2002.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2002.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2003.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2003.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2004.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2004.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2005.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2005.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2006.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2006.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2007.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2007.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2008.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2008.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2009.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2009.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2010.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2010.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab3_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2001.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2001.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2002.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2002.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2003.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2003.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2004.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2004.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2005.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2005.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2006.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2006.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2007.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2007.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2008.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2008.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2009.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2009.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2010.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2010.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_51_2000_2020_xls/51_tab4_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2010.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2010.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab1_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2010.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2010.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab2_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab3_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2011.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2011.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2012.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2012.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2013.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2013.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2014.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2014.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2015.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2015.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2016.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2016.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2017.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2017.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2018.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2018.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2019.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2019.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2020.xls` & `iotbr-0.0.7/iotbr/IBGE/nivel_68_2010_2020_xls/68_tab4_2020.xls`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/io_system.py` & `iotbr-0.0.7/iotbr/io_system.py`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/tru.py` & `iotbr-0.0.7/iotbr/tru.py`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr/tru_pb.py` & `iotbr-0.0.7/iotbr/tru_pb.py`

 * *Files identical despite different names*

### Comparing `iotbr-0.0.6/iotbr.egg-info/PKG-INFO` & `iotbr-0.0.7/iotbr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotbr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Import data from Table of Input-Output from IBGE
 Home-page: https://github.com/fms-1988
 Author: Felipe Morelli Da Silva
 Author-email: fms.morelli@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iotbr-0.0.6/iotbr.egg-info/SOURCES.txt` & `iotbr-0.0.7/iotbr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

