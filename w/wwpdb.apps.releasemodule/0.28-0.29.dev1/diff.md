# Comparing `tmp/wwpdb.apps.releasemodule-0.28.tar.gz` & `tmp/wwpdb.apps.releasemodule-0.29.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.releasemodule-0.28.tar", last modified: Sat Jan 14 14:07:41 2023, max compression
+gzip compressed data, was "wwpdb.apps.releasemodule-0.29.dev1.tar", last modified: Tue May 30 10:29:44 2023, max compression
```

## Comparing `wwpdb.apps.releasemodule-0.28.tar` & `wwpdb.apps.releasemodule-0.29.dev1.tar`

### file list

```diff
@@ -1,82 +1,80 @@
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-01-14 14:07:41.555494 wwpdb.apps.releasemodule-0.28/
--rw-r--r--   0 peisach    (502) staff       (20)      728 2023-01-14 14:07:41.555622 wwpdb.apps.releasemodule-0.28/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)       52 2018-11-27 13:57:08.000000 wwpdb.apps.releasemodule-0.28/README.md
--rw-r--r--   0 peisach    (502) staff       (20)      531 2023-01-14 14:07:41.556169 wwpdb.apps.releasemodule-0.28/setup.cfg
--rwxr-xr-x   0 peisach    (502) staff       (20)     2509 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/setup.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-01-14 14:07:41.524918 wwpdb.apps.releasemodule-0.28/wwpdb/
--rw-r--r--   0 peisach    (502) staff       (20)       65 2018-11-27 14:55:37.000000 wwpdb.apps.releasemodule-0.28/wwpdb/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-01-14 14:07:41.527561 wwpdb.apps.releasemodule-0.28/wwpdb/apps/
--rw-r--r--   0 peisach    (502) staff       (20)       65 2018-11-27 14:55:39.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-01-14 14:07:41.527972 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/
--rw-r--r--   0 peisach    (502) staff       (20)      150 2023-01-14 13:53:33.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-01-14 14:07:41.534314 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/
--rw-r--r--   0 peisach    (502) staff       (20)    10015 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/Analysis.py
--rw-r--r--   0 peisach    (502) staff       (20)     2526 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/CheckResult.py
--rw-r--r--   0 peisach    (502) staff       (20)    15681 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/CitationFinder.py
--rw-r--r--   0 peisach    (502) staff       (20)     5280 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/FetchMP.py
--rw-r--r--   0 peisach    (502) staff       (20)    35131 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/FetchResultParser.py
--rw-r--r--   0 peisach    (502) staff       (20)     4447 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/FetchUtil.py
--rw-r--r--   0 peisach    (502) staff       (20)     3599 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/MatchMP.py
--rw-r--r--   0 peisach    (502) staff       (20)     2508 2021-07-21 19:08:17.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/MatchUtil.py
--rw-r--r--   0 peisach    (502) staff       (20)     8070 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py
--rw-r--r--   0 peisach    (502) staff       (20)    14457 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py
--rw-r--r--   0 peisach    (502) staff       (20)     6901 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/RisCitationParser.py
--rw-r--r--   0 peisach    (502) staff       (20)     4974 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/SearchMP.py
--rw-r--r--   0 peisach    (502) staff       (20)     1629 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/SearchResultParser.py
--rw-r--r--   0 peisach    (502) staff       (20)     3153 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/SearchUtil.py
--rw-r--r--   0 peisach    (502) staff       (20)     2505 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/StringUtil.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2017-04-24 14:01:16.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-01-14 14:07:41.538709 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/
--rw-r--r--   0 peisach    (502) staff       (20)     2904 2022-09-12 12:37:17.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py
--rw-r--r--   0 peisach    (502) staff       (20)    19491 2022-09-12 12:37:17.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictBase.py
--rw-r--r--   0 peisach    (502) staff       (20)     7724 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py
--rw-r--r--   0 peisach    (502) staff       (20)    19597 2022-09-12 12:37:17.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py
--rw-r--r--   0 peisach    (502) staff       (20)     7582 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py
--rw-r--r--   0 peisach    (502) staff       (20)     4158 2022-09-12 12:37:17.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py
--rw-r--r--   0 peisach    (502) staff       (20)     4437 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py
--rw-r--r--   0 peisach    (502) staff       (20)     6428 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictRequest.py
--rw-r--r--   0 peisach    (502) staff       (20)    14638 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2017-04-24 14:01:16.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/__init__.py
--rw-r--r--   0 peisach    (502) staff       (20)      934 2022-09-12 12:37:17.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/test_Depict.py
--rw-r--r--   0 peisach    (502) staff       (20)      894 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/test_DepictCitation.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-01-14 14:07:41.548040 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/
--rw-r--r--   0 peisach    (502) staff       (20)    12660 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/AutoReRelease.py
--rw-r--r--   0 peisach    (502) staff       (20)    12851 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py
--rw-r--r--   0 peisach    (502) staff       (20)    12693 2023-01-14 13:53:33.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/EmReleaseUtil.py
--rw-r--r--   0 peisach    (502) staff       (20)      919 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/Emd2XmlTranslator.py
--rw-r--r--   0 peisach    (502) staff       (20)     3069 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py
--rw-r--r--   0 peisach    (502) staff       (20)     2600 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/EntryPullProcess.py
--rw-r--r--   0 peisach    (502) staff       (20)    25384 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/EntryUpdateBase.py
--rw-r--r--   0 peisach    (502) staff       (20)    25079 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py
--rw-r--r--   0 peisach    (502) staff       (20)     3537 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/InputFormParser_v2.py
--rw-r--r--   0 peisach    (502) staff       (20)    17268 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py
--rw-r--r--   0 peisach    (502) staff       (20)     4828 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/NmrDataGenerator.py
--rw-r--r--   0 peisach    (502) staff       (20)    21726 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py
--rw-r--r--   0 peisach    (502) staff       (20)    23667 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/ReleaseUtil.py
--rw-r--r--   0 peisach    (502) staff       (20)     3479 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py
--rw-r--r--   0 peisach    (502) staff       (20)     3774 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/UpdateBase.py
--rw-r--r--   0 peisach    (502) staff       (20)    22113 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/UpdateFormParser.py
--rw-r--r--   0 peisach    (502) staff       (20)    13024 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2017-04-24 14:01:15.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-01-14 14:07:41.554473 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/
--rw-r--r--   0 peisach    (502) staff       (20)    23712 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/CombineDbApi.py
--rw-r--r--   0 peisach    (502) staff       (20)    22302 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/ContentDbApi.py
--rw-r--r--   0 peisach    (502) staff       (20)     7405 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/DbApiUtil.py
--rw-r--r--   0 peisach    (502) staff       (20)     4439 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/JournalAbbrev.py
--rw-r--r--   0 peisach    (502) staff       (20)     6429 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/MessageBaseClass.py
--rw-r--r--   0 peisach    (502) staff       (20)     9479 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py
--rw-r--r--   0 peisach    (502) staff       (20)     1574 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/MultiProcLimit.py
--rw-r--r--   0 peisach    (502) staff       (20)     6170 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py
--rw-r--r--   0 peisach    (502) staff       (20)     3456 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/TimeUtil.py
--rw-r--r--   0 peisach    (502) staff       (20)    12748 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/Utility.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2017-04-24 14:01:14.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-01-14 14:07:41.555269 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/webapp/
--rw-r--r--   0 peisach    (502) staff       (20)    46743 2022-11-14 12:47:25.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2017-04-24 14:01:16.000000 wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/webapp/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-01-14 14:07:41.527153 wwpdb.apps.releasemodule-0.28/wwpdb.apps.releasemodule.egg-info/
--rw-r--r--   0 peisach    (502) staff       (20)      728 2023-01-14 14:07:41.000000 wwpdb.apps.releasemodule-0.28/wwpdb.apps.releasemodule.egg-info/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)     3356 2023-01-14 14:07:41.000000 wwpdb.apps.releasemodule-0.28/wwpdb.apps.releasemodule.egg-info/SOURCES.txt
--rw-r--r--   0 peisach    (502) staff       (20)        1 2023-01-14 14:07:41.000000 wwpdb.apps.releasemodule-0.28/wwpdb.apps.releasemodule.egg-info/dependency_links.txt
--rw-r--r--   0 peisach    (502) staff       (20)        1 2018-11-27 15:03:14.000000 wwpdb.apps.releasemodule-0.28/wwpdb.apps.releasemodule.egg-info/not-zip-safe
--rw-r--r--   0 peisach    (502) staff       (20)      246 2023-01-14 14:07:41.000000 wwpdb.apps.releasemodule-0.28/wwpdb.apps.releasemodule.egg-info/requires.txt
--rw-r--r--   0 peisach    (502) staff       (20)        6 2023-01-14 14:07:41.000000 wwpdb.apps.releasemodule-0.28/wwpdb.apps.releasemodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.117573 wwpdb.apps.releasemodule-0.29.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      733 2023-05-30 10:29:44.117573 wwpdb.apps.releasemodule-0.29.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       52 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      531 2023-05-30 10:29:44.117573 wwpdb.apps.releasemodule-0.29.dev1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2509 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.105573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.105573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.105573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.109573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10466 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/Analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2661 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/CheckResult.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15685 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/CitationFinder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5284 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/FetchMP.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35269 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/FetchResultParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4490 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/FetchUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3611 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/MatchMP.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2569 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/MatchUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8181 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14457 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6962 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/RisCitationParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4999 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/SearchMP.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1635 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/SearchResultParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3194 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/SearchUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2505 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/StringUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.109573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2904 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19491 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7724 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19597 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7582 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4158 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4437 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6428 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14638 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      894 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/test_DepictCitation.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.113573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/
+-rw-r--r--   0 vsts      (1001) docker     (123)    12660 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/AutoReRelease.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12851 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12694 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EmReleaseUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3069 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2600 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryPullProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    25384 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryUpdateBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    25079 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3537 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/InputFormParser_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17268 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4828 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/NmrDataGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    21726 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    23667 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/ReleaseUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3479 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3774 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/UpdateBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    22156 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/UpdateFormParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13024 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.117573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)    23712 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/CombineDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    22302 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/ContentDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7405 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/DbApiUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4439 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/JournalAbbrev.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6429 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/MessageBaseClass.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9479 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1574 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/MultiProcLimit.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6170 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3456 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12748 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/Utility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.117573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)    46743 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.105573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      733 2023-05-30 10:29:44.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     3256 2023-05-30 10:29:44.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-30 10:29:44.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-30 10:29:26.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      246 2023-05-30 10:29:44.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-05-30 10:29:44.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.releasemodule-0.28/PKG-INFO` & `wwpdb.apps.releasemodule-0.29.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.releasemodule
-Version: 0.28
+Version: 0.29.dev1
 Summary: wwPDB sequence module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_releasemodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.releasemodule-0.28/setup.cfg` & `wwpdb.apps.releasemodule-0.29.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/setup.py` & `wwpdb.apps.releasemodule-0.29.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/Analysis.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/Analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,25 +34,26 @@
     import pickle
 
 # from mmcif.api.PdbxContainers import *
 from mmcif.api.PdbxContainers import DataContainer
 from mmcif.api.DataCategory import DataCategory
 from mmcif.io.PdbxWriter import PdbxWriter
 from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
-from wwpdb.apps.entity_transform.utils.mmCIFUtil import mmCIFUtil
+# from wwpdb.apps.entity_transform.utils.mmCIFUtil import mmCIFUtil
+from wwpdb.io.file.mmCIFUtil import mmCIFUtil
 from wwpdb.apps.releasemodule.citation.MatchMP import MatchMP
 # from wwpdb.apps.releasemodule.utils.Utility import *
 from wwpdb.apps.releasemodule.utils.Utility import RunScript
 
 
 class Analysis(object):
     """
     """
 
-    def __init__(self, siteId="WWPDB_DEPLOY_TEST", path='.', input='result.db', log=sys.stderr, verbose=False):
+    def __init__(self, siteId="WWPDB_DEPLOY_TEST", path='.', input='result.db', log=sys.stderr, verbose=False):  # pylint: disable=redefined-builtin
         """ Initial Analysis class
         """
         self.__sessionPath = path
         self.__picklefile = input
         self.__resultfile = 'result.cif'
         self.__lfh = log
         self.__verbose = verbose
@@ -99,15 +100,15 @@
             #    mUtil.run()
             #    mList = mUtil.getMatchList()
             #
             if not mList:
                 continue
             #
             plist = []
-            for list in mList:
+            for list in mList:  # pylint: disable=redefined-builtin
                 if list[0] not in self.__pubmedInfo:
                     continue
                 #
                 pdir = copy.deepcopy(self.__pubmedInfo[list[0]])
                 pdir['similarity_score'] = list[1]
                 plist.append(pdir)
             #
@@ -126,17 +127,17 @@
             #
         #
 
     def _sortEntryMap(self):
         if not self.__annotEntryMap:
             return
         #
-        map = self.__annotEntryMap
+        map = self.__annotEntryMap  # pylint: disable=redefined-builtin
         self.__annotEntryMap = {}
-        for k, list in map.items():
+        for k, list in map.items():  # pylint: disable=redefined-builtin
             if len(list) < 2:
                 self.__annotEntryMap[k] = list
             else:
                 dmap = {}
                 slist = []
                 for cdt in list:
                     dmap[cdt['structure_id']] = cdt
@@ -210,15 +211,15 @@
             return None
         #
         cat = DataCategory('author_pubmed_mapping')
         cat.appendAttribute('author')
         cat.appendAttribute('pubmed_ids')
         #
         row = 0
-        for key, list in self.__termMap.items():
+        for key, list in self.__termMap.items():  # pylint: disable=redefined-builtin
             cat.setValue(str(key), 'author', row)
             cat.setValue(str(','.join(list)), 'pubmed_ids', row)
             row += 1
         #
         return cat
 
     def _getPubmedCitationCategory(self):
@@ -226,15 +227,15 @@
             return None
         #
         cat = DataCategory('pubmed_info')
         cat.appendAttribute('id')
         cat.appendAttribute('title')
         #
         row = 0
-        for key, dir in self.__pubmedInfo.items():
+        for _key, dir in self.__pubmedInfo.items():  # pylint: disable=redefined-builtin
             cat.setValue(str(dir['pdbx_database_id_PubMed']), 'id', row)
             cat.setValue(str(dir['title']), 'title', row)
             row += 1
         #
         return cat
 
     def _runCitationMatch(self):
@@ -257,15 +258,15 @@
             return
         #
         cifObj = mmCIFUtil(filePath=filename)
         rlist = cifObj.GetValue('entry_pubmed_mapping')
         if not rlist:
             return
         #
-        for dir in rlist:
+        for dir in rlist:  # pylint: disable=redefined-builtin
             if 'structure_id' not in dir or \
                     'pubmed_id' not in dir or \
                     'similarity_score' not in dir:
                 continue
             #
             structure_id = dir['structure_id']
             pubmed_id = dir['pubmed_id']
@@ -277,17 +278,17 @@
             #
         #
 
     def _sortMatchResultMap(self):
         if not self.__matchResultMap:
             return
         #
-        map = self.__matchResultMap
+        map = self.__matchResultMap  # pylint: disable=redefined-builtin
         self.__matchResultMap = {}
-        for k, list in map.items():
+        for k, list in map.items():  # pylint: disable=redefined-builtin
             if len(list) > 1:
                 list.sort(key=operator.itemgetter(1))
                 list.reverse()
             self.__matchResultMap[k] = list
         #
 
     def Read(self):
@@ -299,19 +300,23 @@
         self._getMatchList()
         self._sortEntryMap()
 
     def getResult(self):
         return self.__annotEntryMap
 
 
-if __name__ == '__main__':
+def doMain():
     startTime = time.time()
     cf = Analysis(log=sys.stderr, verbose=False)
     cf.Read()
-    dir = cf.getResult()
+    dir = cf.getResult()  # pylint: disable=redefined-builtin
     endTime = time.time()
     diffTime = endTime - startTime
     print(diffTime)
-    for k, list in list(dir.items()):
-        print('annot=' + k + ': Total=' + str(len(list)))
-        for d in list:
+    for k, dlist in list(dir.items()):
+        print('annot=' + k + ': Total=' + str(len(dlist)))
+        for d in dlist:
             print(d['structure_id'] + '=' + str(len(d['pubmed'])))
+
+
+if __name__ == '__main__':
+    doMain()
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/CheckResult.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/CheckResult.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,38 +32,38 @@
 from wwpdb.apps.releasemodule.citation.StringUtil import calStringSimilarity
 
 
 class CheckResult(object):
     """
     """
 
-    def __init__(self, path='.', input='result.db', log=sys.stderr, verbose=False):
+    def __init__(self, path='.', input='result.db', log=sys.stderr, verbose=False):  # pylint: disable=unused-argument,redefined-builtin
         """ Initial CheckResult class
         """
         self.__sessionPath = path
         self.__picklefile = input
-        self.__lfh = log
-        self.__verbose = verbose
+        # self.__lfh = log
+        # self.__verbose = verbose
         self.__annotEntryMap = {}
         #
         self._deserialize()
         #
 
     def _deserialize(self):
         filename = os.path.join(self.__sessionPath, self.__picklefile)
         fb = open(filename, 'rb')
         self.__annotEntryMap = pickle.load(fb)
         fb.close()
 
     def Check(self):
-        map = self.__annotEntryMap
+        aemap = self.__annotEntryMap
         self.__annotEntryMap = {}
-        for k, list in map.items():
+        for k, list in aemap.items():  # pylint: disable=redefined-builtin
             elist = []
-            for dir in list:
+            for dir in list:  # pylint: disable=redefined-builtin
                 print(dir['structure_id'] + ': ' + dir['c_title'])
                 plist = []
                 for pdir in dir['pubmed']:
                     sim = calStringSimilarity(dir['c_title'], pdir['title'])
                     if sim < 0.5:
                         continue
                     #
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/CitationFinder.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/CitationFinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     def _getPubmedIdList(self):
         """ Get unique Pubmed ID list
         """
         if not self.__termMap:
             return
         #
         tmap = {}
-        for key, plist in self.__termMap.items():
+        for _key, plist in self.__termMap.items():
             for pid in plist:
                 if pid in tmap:
                     continue
                 #
                 tmap[pid] = 'y'
                 self.__pubmedIdList.append(pid)
             #
@@ -330,15 +330,15 @@
         #
         cat = DataCategory('pubmed_info')
         cat.appendAttribute('id')
         cat.appendAttribute('doi')
         cat.appendAttribute('title')
         #
         row = 0
-        for key, v_dict in self.__pubmedInfo.items():
+        for _key, v_dict in self.__pubmedInfo.items():
             cat.setValue(str(v_dict['pdbx_database_id_PubMed']), 'id', row)
             if 'pdbx_database_id_DOI' in v_dict:
                 cat.setValue(str(v_dict['pdbx_database_id_DOI']), 'doi', row)
             else:
                 cat.setValue('?', 'doi', row)
             #
             cat.setValue(str(v_dict['title']), 'title', row)
@@ -481,9 +481,9 @@
 
 
 if __name__ == '__main__':
     startTime = time.time()
     cf = CitationFinder(siteId=sys.argv[1], path=sys.argv[2], output=sys.argv[3], log=sys.stderr, verbose=False)
     cf.searchPubmed()
     endTime = time.time()
-    diffTime = endTime - startTime
-    print(diffTime)
+    ldiffTime = endTime - startTime
+    print(ldiffTime)
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/FetchMP.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/FetchMP.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,16 +122,16 @@
         for subList in subLists:
             taskQueue.put(subList)
         #
         for i in range(numProc):
             taskQueue.put(None)
         #
         for i in range(len(subLists)):
-            list = resultQueue.get()
-            for info in list:
+            rlist = resultQueue.get()
+            for info in rlist:
                 self.__pubmedInfoMap[info['pdbx_database_id_PubMed']] = info
             #
         #
         try:
             for w in workers:
                 w.terminate()
                 w.join(1)
@@ -163,12 +163,12 @@
     data = f.read()
     f.close()
     #
     idlist = data.split('\n')
     print('idlist=' + str(len(idlist)))
     cf = FetchMP(idList=idlist, log=sys.stderr, verbose=False)
     cf.run()
-    dir = cf.getPubmedInfoMap()
-    print('dir=' + str(len(dir)))
+    pdir = cf.getPubmedInfoMap()
+    print('dir=' + str(len(pdir)))
     #
     # for k,v in dir.items():
     #    print v
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/FetchResultParser.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/FetchResultParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 
 class UniCodeHandler(object):
     """ Convert non-ascii unicode into ascii code if possible
     """
 
     def __init__(self):
+        # pylint: disable=redundant-u-string-prefix
         self.__unicodeMapping = {
             u'\u00C0': 'A',
             u'\u00C1': 'A',
             u'\u00C2': 'A',
             u'\u00C3': 'A',
             u'\u00C4': 'A',
             u'\u00C6': 'Ae',
@@ -801,15 +802,15 @@
         data = data.strip()
         for word in self.__greekLetter:
             data = data.replace('- ' + word, '-' + word)
             data = data.replace(word + ' -', word + '-')
         return data
 
     def __processUniCode(self, input_data, Mapping):
-        data = u''
+        data = u''  # pylint: disable=redundant-u-string-prefix
         for c in input_data:
             if c in Mapping:
                 data += Mapping[c]
             else:
                 data += c
         return data
 
@@ -861,15 +862,15 @@
                 except:  # noqa: E722 pylint: disable=bare-except
                     continue
             #
         #
         return infolist
 
     def _processMedlineCitationNode(self, entry):
-        id = ''
+        id = ''  # pylint: disable=redefined-builtin
         info = {}
         for node in entry.childNodes:
             if node.nodeType != node.ELEMENT_NODE:
                 continue
             #
             if node.tagName == 'PMID':
                 id = str(node.firstChild.data)
@@ -1003,18 +1004,18 @@
             if node.tagName == 'MedlinePgn':
                 pages = self._processNodes(node.childNodes, False)
                 if not pages:
                     continue
                 #
                 first = pages
                 last = pages
-                list = pages.split('-')
-                if len(list) == 2:
-                    first = list[0].strip()
-                    last = list[1].strip()
+                plist = pages.split('-')
+                if len(plist) == 2:
+                    first = plist[0].strip()
+                    last = plist[1].strip()
                     if len(last) < len(first):
                         idx = len(first) - len(last)
                         last = first[0:idx] + last
                     #
                 #
                 info['page_first'] = first
                 info['page_last'] = last
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/FetchUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/FetchUtil.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,22 @@
 from wwpdb.apps.releasemodule.citation.FetchResultParser import FetchResultParser
 from wwpdb.apps.releasemodule.utils.Utility import getFileName, RunScript
 
 
 class FetchUtil(object):
     """
     """
-    def __init__(self, path='.', processLabel='', idList=None, siteId=None, mpl=None, log=sys.stderr, verbose=False):
+    def __init__(self, path='.', processLabel='', idList=None, siteId=None, mpl=None, log=sys.stderr, verbose=False):  # pylint: disable=unused-argument
         """
         """
         self.__sessionPath = path
         self.__processLabel = processLabel
         self.__pubmedIdList = idList
-        self.__lfh = log
-        self.__verbose = verbose
+        # self.__lfh = log
+        # self.__verbose = verbose
         self.__pubmedInfoList = []
         # self.__pubmedInfoMap = {}
         self.__cI = ConfigInfo(siteId)
         self.__apikey = self.__cI.get('NCBI_API_KEY')
         self.__mpl = mpl
 
     def doFetch(self):
@@ -132,11 +132,11 @@
         #    self.__pubmedInfoMap[info['pdbx_database_id_PubMed']] = info
         #
 
 
 if __name__ == '__main__':
     cf = FetchUtil(idList=['23542341', '23326635'], log=sys.stderr, verbose=False)
     cf.doFetch()
-    list = cf.getPubmedInfoList()
-    print(list)
-    dir = cf.getPubmedInfoMap()
-    print(dir)
+    clist = cf.getPubmedInfoList()
+    print(clist)
+    cdir = cf.getPubmedInfoMap()
+    print(cdir)
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/MatchMP.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/MatchMP.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,19 @@
             nextList = self.__taskQueue.get()
             # end of queue condition
             if nextList is None:
                 break
             #
             resultList = []
             for entry in nextList:
-                list = self.getMatchList(entry)
-                if not list:
+                mlist = self.getMatchList(entry)
+                if not mlist:
                     continue
                 #
-                resultList.append([entry['structure_id'], list])
+                resultList.append([entry['structure_id'], mlist])
             #
             self.__resultQueue.put(resultList)
         #
 
 
 class MatchMP(object):
     """
@@ -102,16 +102,16 @@
             taskQueue.put(None)
         #
         for i in range(len(subLists)):
             lists = resultQueue.get()
             if not lists:
                 continue
             #
-            for list in lists:
-                self.__matchResultMap[list[0]] = list[1]
+            for reslist in lists:
+                self.__matchResultMap[reslist[0]] = reslist[1]
             #
         #
         try:
             for w in workers:
                 w.terminate()
                 w.join(1)
             #
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/MatchUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/MatchUtil.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,22 +26,22 @@
 from wwpdb.apps.releasemodule.citation.StringUtil import calStringSimilarity
 
 
 class MatchUtil(object):
     """
     """
 
-    def __init__(self, entry=None, termMap=None, pubmedInfo=None, log=sys.stderr, verbose=False):
+    def __init__(self, entry=None, termMap=None, pubmedInfo=None, log=sys.stderr, verbose=False):  # pylint: disable=unused-argument
         """ Initial MatchUtil class
         """
         self.__entry = entry
         self.__termMap = termMap
         self.__pubmedInfo = pubmedInfo
-        self.__lfh = log
-        self.__verbose = verbose
+        # self.__lfh = log
+        # self.__verbose = verbose
         self.__pubmedMatchList = []
 
     def run(self):
         if 'rcsb_annotator' not in self.__entry or \
                 'c_title' not in self.__entry or \
                 'pubmed_author' not in self.__entry or \
                 'structure_id' not in self.__entry:
@@ -54,37 +54,37 @@
         self._findMatchList(idlist)
 
     def getMatchList(self):
         return self.__pubmedMatchList
 
     def _getUniquePubmedIdList(self):
         idlist = []
-        map = {}
+        t_map = {}
         for term in self.__entry['pubmed_author']:
             if term not in self.__termMap:
                 continue
             #
-            for id in self.__termMap[term]:
-                if id in map:
+            for t_id in self.__termMap[term]:
+                if t_id in t_map:
                     continue
                 #
-                map[id] = 'y'
-                idlist.append(id)
+                t_map[t_id] = 'y'
+                idlist.append(t_id)
             #
         return idlist
 
     def _findMatchList(self, idlist):
-        for id in idlist:
-            if id not in self.__pubmedInfo:
+        for p_id in idlist:
+            if p_id not in self.__pubmedInfo:
                 continue
             sim = calStringSimilarity(self.__entry['c_title'],
-                                      self.__pubmedInfo[id]['title'])
+                                      self.__pubmedInfo[p_id]['title'])
             if sim < 0.5:
                 continue
             #
-            self.__pubmedMatchList.append([id, '%.3f' % sim])
+            self.__pubmedMatchList.append([p_id, '%.3f' % sim])
         #
         if len(self.__pubmedMatchList) < 2:
             return
         #
         self.__pubmedMatchList.sort(key=operator.itemgetter(1))
         self.__pubmedMatchList.reverse()
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         #
 
     def __getEntryIDList(self, annotator):
         if (not self.__annotEntryMap) or (annotator not in self.__annotEntryMap):
             return
         #
         foundList = []
-        for dir in self.__annotEntryMap[annotator]:
+        for dir in self.__annotEntryMap[annotator]:  # pylint: disable=redefined-builtin
             if isDEPLocked(dir['structure_id']):
                 foundList.append(dir)
                 #
                 for pdir in dir['pubmed']:
                     if not pdir['pdbx_database_id_PubMed'] in self.__allPubmedIdList:
                         self.__allPubmedIdList.append(pdir['pdbx_database_id_PubMed'])
                     #
@@ -116,15 +116,15 @@
         items = ['pdbx_database_id_DOI', 'title', 'journal_abbrev', 'journal_volume',
                  'page_first', 'page_last', 'year', 'journal_id_ISSN', 'author']
         #
         RelList = db.getThisWeekRelEntries(annotator)
         #
         num_hit = 0
         num_update = 0
-        for dir in foundEntryList:
+        for dir in foundEntryList:  # pylint: disable=redefined-builtin
             #
             # Get current citation information from database
             #
             cinfo = db.getCitation(dir['structure_id'])
             #
             # Update citation information
             #
@@ -191,15 +191,15 @@
             #
             # if found_update:
             #    num_update += 1
             #
         #
         f.write(annotator + ' \t ' + str(num_hit) + ' \t ' + str(num_update) + '\n')
 
-    def __compareCitationInfo(self, cinfo, dir, release_flag):
+    def __compareCitationInfo(self, cinfo, dir, release_flag):  # pylint: disable=redefined-builtin
         code = ' '
         if ('pdbx_database_id_PubMed' not in cinfo) or ('pdbx_database_id_PubMed' not in dir):
             return code
         #
         if str(cinfo['pdbx_database_id_PubMed']) != dir['pdbx_database_id_PubMed']:
             return code
         #
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/RisCitationParser.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/RisCitationParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,16 @@
             if minor > 3:
                 import html as parser
             else:
                 import html.parser
                 parser = html.parser.HTMLParser()
             #
         else:
-            import HTMLParser
+            # Python 2
+            import HTMLParser  # pylint: disable=import-error
             parser = HTMLParser.HTMLParser()
         #
         doc = minidom.parseString("<RisStringTag>" + parser.unescape(ris_value).replace("&", "&#38;").replace("<", "&#60;") + "</RisStringTag>")
         return self.__processNodes(doc.getElementsByTagName("RisStringTag")[0].childNodes, angstromFlag)
 
     def __processNodes(self, childNodes, angstromFlag):
         text = ""
@@ -195,12 +196,12 @@
             self.__convertedCitationData["author"].append({"name": cif_author, "orcid": ""})
         else:
             self.__convertedCitationData["author"] = [{"name": cif_author, "orcid": ""}]
         #
 
 
 if __name__ == "__main__":
-    parser = RisCitationParser(sys.argv[1])
-    citDict = parser.getCitationData()
-    for key, val in citDict.items():
-        sys.stderr.write("%r=%r\n" % (key, val))
+    rparser = RisCitationParser(sys.argv[1])
+    citDict = rparser.getCitationData()
+    for key, c_val in citDict.items():
+        sys.stderr.write("%r=%r\n" % (key, c_val))
     #
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/SearchMP.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/SearchMP.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,22 +61,22 @@
             nextList = self.__taskQueue.get()
             # end of queue condition
             if nextList is None:
                 break
             #
             resultList = []
             for term in nextList:
-                list = self.fetchEntryList(term)
-                if not list:
+                f_list = self.fetchEntryList(term)
+                if not f_list:
                     continue
                 #
-                dir = {}
-                dir['term'] = term
-                dir['id'] = list
-                resultList.append(dir)
+                tdir = {}
+                tdir['term'] = term
+                tdir['id'] = f_list
+                resultList.append(tdir)
             #
             self.__resultQueue.put(resultList)
         #
 
 
 class SearchMP(object):
     """
@@ -125,20 +125,20 @@
         for subList in subLists:
             taskQueue.put(subList)
         #
         for i in range(numProc):
             taskQueue.put(None)
         #
         for i in range(len(subLists)):
-            list = resultQueue.get()
-            if not list:
+            rqlist = resultQueue.get()
+            if not rqlist:
                 continue
             #
-            for dir in list:
-                self.__termMap[dir['term']] = dir['id']
+            for rqdir in rqlist:
+                self.__termMap[rqdir['term']] = rqdir['id']
             #
         #
         try:
             for w in workers:
                 w.terminate()
                 w.join(1)
             #
@@ -158,11 +158,11 @@
     f.close()
     #
     termlist = data.split('\n')
     termlist.remove('')
     print('termlist=' + str(len(termlist)))
     cf = SearchMP(termList=termlist, log=sys.stderr, verbose=False)
     cf.run()
-    dir = cf.getTermMap()
-    print('dir=' + str(len(dir)))
-    print(dir)
+    cdir = cf.getTermMap()
+    print('dir=' + str(len(cdir)))
+    print(cdir)
     #
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/SearchResultParser.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/SearchResultParser.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,19 +47,19 @@
 
     def _parseDoc(self, doc):
         idlist = []
         entryList = doc.getElementsByTagName('Id')
         if len(entryList) > 0:
             for entry in entryList:
                 if entry.firstChild:
-                    id = str(entry.firstChild.data)
-                    idlist.append(id)
+                    d_id = str(entry.firstChild.data)
+                    idlist.append(d_id)
                 #
             #
         #
         return idlist
 
 
 if __name__ == "__main__":
     parser = SearchResultParser(sys.argv[1])
-    list = parser.getIdList()
-    print(list)
+    clist = parser.getIdList()
+    print(clist)
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/SearchUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/SearchUtil.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,22 +31,22 @@
 from wwpdb.apps.releasemodule.utils.Utility import getFileName, RunScript
 
 
 class SearchUtil(object):
     """
     """
 
-    def __init__(self, path='.', processLabel='', term=None, siteId=None, log=sys.stderr, verbose=False):
+    def __init__(self, path='.', processLabel='', term=None, siteId=None, log=sys.stderr, verbose=False):  # pylint: disable=unused-argument
         """
         """
         self.__sessionPath = path
         self.__processLabel = processLabel
         self.__term = term
-        self.__lfh = log
-        self.__verbose = verbose
+        # self.__lfh = log
+        # self.__verbose = verbose
         self.__pubmedIdList = []
         self.__cI = ConfigInfo(siteId)
         self.__apikey = self.__cI.get('NCBI_API_KEY')
 
     def doSearch(self):
         """ Create NCBI webservice URL and run pubmed author search webservice
         """
@@ -90,9 +90,9 @@
     def getPubmedIdList(self):
         return self.__pubmedIdList
 
 
 if __name__ == '__main__':
     cf = SearchUtil(term='Badger+J[au]', log=sys.stderr, verbose=False)
     cf.doSearch()
-    list = cf.getPubmedIdList()
-    print(list)
+    plist = cf.getPubmedIdList()
+    print(plist)
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/citation/StringUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/StringUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictBase.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/DepictRequest.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/depict/test_DepictCitation.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/test_DepictCitation.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/AutoReRelease.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/AutoReRelease.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/EmReleaseUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EmReleaseUtil.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import sys
 import traceback
 
 from wwpdb.apps.releasemodule.update.EntryUpdateBase import EntryUpdateBase
 from wwpdb.utils.config.ConfigInfoData import ConfigInfoData
 from wwpdb.utils.emdb.cif_emdb_translator.cif_emdb_translator import CifEMDBTranslator
 
+
 class EmReleaseUtil(EntryUpdateBase):
     """ Class responsible for release/pull off entries
     """
     def __init__(self, reqObj=None, entryDir=None, verbose=False, log=sys.stderr):
         super(EmReleaseUtil, self).__init__(reqObj=reqObj, entryDir=entryDir, statusDB=None, verbose=verbose, log=log)
         # fmt: off
         self.__additionalTypeList = [ [ 'em-mask-volume',       '_msk',        'masks',            False, True,  True  ],
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/EntryPullProcess.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryPullProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/EntryUpdateBase.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryUpdateBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/InputFormParser_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/InputFormParser_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/NmrDataGenerator.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/NmrDataGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/ReleaseUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/ReleaseUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/UpdateBase.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/UpdateBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/UpdateFormParser.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/UpdateFormParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,15 +392,15 @@
             max_author_num = int(val)
             author_list = []
             orderMap = {}
             for i in range(0, max_author_num):
                 order = str(self.__reqObj.getValue('order_' + str(i + 1)))
                 try:
                     int_order = int(order)
-                except:
+                except:  # noqa: E722 pylint: disable=bare-except
                     self.__errorContent += "Author ordinal number '" + order + "' is not an integer.\n"
                     continue
                 #
                 if int_order < 1:
                     continue
                 #
                 name = self.__codeHandler.process(self.__reqObj.getRawValue('name_' + str(i + 1)), False)
@@ -420,15 +420,15 @@
                 a_dir = {}
                 a_dir['order'] = int_order
                 a_dir['id'] = citation['id']
                 a_dir['name'] = name
                 a_dir['orcid'] = orcid
                 author_list.append(a_dir)
             #
-            for key,val in orderMap.items():
+            for key, val in orderMap.items():
                 if val > 1:
                     self.__errorContent += "There are " + str(val) + " 'Author " + str(key) + "'.\n"
                 #
             #
             if len(author_list) > 1:
                 author_list.sort(key=itemgetter('order'))
             #
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/CombineDbApi.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/CombineDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/ContentDbApi.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/ContentDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/DbApiUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/DbApiUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/JournalAbbrev.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/JournalAbbrev.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/MessageBaseClass.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/MessageBaseClass.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/MultiProcLimit.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/MultiProcLimit.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/TimeUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/utils/Utility.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/Utility.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb.apps.releasemodule.egg-info/PKG-INFO` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.releasemodule
-Version: 0.28
+Version: 0.29.dev1
 Summary: wwPDB sequence module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_releasemodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.releasemodule-0.28/wwpdb.apps.releasemodule.egg-info/SOURCES.txt` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -32,20 +32,18 @@
 wwpdb/apps/releasemodule/depict/DepictCitation_v2.py
 wwpdb/apps/releasemodule/depict/DepictEntryHistory.py
 wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py
 wwpdb/apps/releasemodule/depict/DepictRemovalMark.py
 wwpdb/apps/releasemodule/depict/DepictRequest.py
 wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py
 wwpdb/apps/releasemodule/depict/__init__.py
-wwpdb/apps/releasemodule/depict/test_Depict.py
 wwpdb/apps/releasemodule/depict/test_DepictCitation.py
 wwpdb/apps/releasemodule/update/AutoReRelease.py
 wwpdb/apps/releasemodule/update/CitationFormParser_v2.py
 wwpdb/apps/releasemodule/update/EmReleaseUtil.py
-wwpdb/apps/releasemodule/update/Emd2XmlTranslator.py
 wwpdb/apps/releasemodule/update/EntryFormParser_v2.py
 wwpdb/apps/releasemodule/update/EntryPullProcess.py
 wwpdb/apps/releasemodule/update/EntryUpdateBase.py
 wwpdb/apps/releasemodule/update/EntryUpdateProcess.py
 wwpdb/apps/releasemodule/update/InputFormParser_v2.py
 wwpdb/apps/releasemodule/update/MultiUpdateProcess.py
 wwpdb/apps/releasemodule/update/NmrDataGenerator.py
```

