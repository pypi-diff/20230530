# Comparing `tmp/seatsio-72.4.0.tar.gz` & `tmp/seatsio-73.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seatsio-72.4.0.tar", last modified: Mon May  8 11:12:59 2023, max compression
+gzip compressed data, was "seatsio-73.0.0.tar", last modified: Tue May 30 08:30:10 2023, max compression
```

## Comparing `seatsio-72.4.0.tar` & `seatsio-73.0.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 11:12:52.000000 seatsio-72.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 11:12:52.000000 seatsio-72.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-08 11:12:59.033161 seatsio-72.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-08 11:12:52.000000 seatsio-72.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.029161 seatsio-72.4.0/seatsio/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.029161 seatsio-72.4.0/seatsio/charts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/charts/chartsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/charts/chartsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/charts/socialDistancingRulesetsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.029161 seatsio-72.4.0/seatsio/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/changeBestAvailableObjectStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/changeObjectStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/channelProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/channelsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/channelsRequests.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/createMultipleEventsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/createSingleEventRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/eventProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/eventsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/extraDataRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/forSaleRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/objectProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/statusChangeRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.029161 seatsio-72.4.0/seatsio/holdtokens/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/holdtokens/HoldTokenClient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/holdtokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/httpClient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.029161 seatsio-72.4.0/seatsio/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/pagination/listableObjectsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/pagination/lister.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/pagination/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/pagination/pageFetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/pagination/pagedIterator.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/reports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/reports/charts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/charts/chartReports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/reports/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/events/eventReports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/reports/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/usage/usageReports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/seasons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/seasons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/seasons/seasonsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/subaccounts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/subaccounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/subaccounts/subaccountsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/workspaces/UpdateWorkspaceRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/workspaces/createWorkspaceRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/workspaces/workspacesClient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.029161 seatsio-72.4.0/seatsio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-08 11:12:58.000000 seatsio-72.4.0/seatsio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-08 11:12:59.000000 seatsio-72.4.0/seatsio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:12:58.000000 seatsio-72.4.0/seatsio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-08 11:12:58.000000 seatsio-72.4.0/seatsio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 11:12:58.000000 seatsio-72.4.0/seatsio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:12:59.033161 seatsio-72.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-08 11:12:55.000000 seatsio-72.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.854128 seatsio-73.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 08:30:03.000000 seatsio-73.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 08:30:03.000000 seatsio-73.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-30 08:30:10.854128 seatsio-73.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-30 08:30:03.000000 seatsio-73.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.846127 seatsio-73.0.0/seatsio/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.850127 seatsio-73.0.0/seatsio/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/charts/chartsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/charts/chartsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/charts/socialDistancingRulesetsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.850127 seatsio-73.0.0/seatsio/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/changeBestAvailableObjectStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/changeObjectStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/channelProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/channelsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/channelsRequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/createMultipleEventsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/createSingleEventRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/eventProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/eventsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/extraDataRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/forSaleRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/objectProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/events/statusChangeRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.850127 seatsio-73.0.0/seatsio/holdtokens/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/holdtokens/HoldTokenClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/holdtokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/httpClient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.850127 seatsio-73.0.0/seatsio/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/pagination/listableObjectsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/pagination/lister.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/pagination/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/pagination/pageFetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/pagination/pagedIterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.850127 seatsio-73.0.0/seatsio/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.850127 seatsio-73.0.0/seatsio/reports/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/reports/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/reports/charts/chartReports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.850127 seatsio-73.0.0/seatsio/reports/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/reports/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/reports/events/eventReports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.854128 seatsio-73.0.0/seatsio/reports/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/reports/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/reports/usage/usageReports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.854128 seatsio-73.0.0/seatsio/seasons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/seasons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/seasons/seasonsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.854128 seatsio-73.0.0/seatsio/subaccounts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/subaccounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/subaccounts/subaccountsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.854128 seatsio-73.0.0/seatsio/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/workspaces/UpdateWorkspaceRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/workspaces/createWorkspaceRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-30 08:30:03.000000 seatsio-73.0.0/seatsio/workspaces/workspacesClient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:30:10.846127 seatsio-73.0.0/seatsio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-30 08:30:10.000000 seatsio-73.0.0/seatsio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-30 08:30:10.000000 seatsio-73.0.0/seatsio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:30:10.000000 seatsio-73.0.0/seatsio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-30 08:30:10.000000 seatsio-73.0.0/seatsio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 08:30:10.000000 seatsio-73.0.0/seatsio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:30:10.854128 seatsio-73.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-30 08:30:08.000000 seatsio-73.0.0/setup.py
```

### Comparing `seatsio-72.4.0/LICENSE` & `seatsio-73.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/PKG-INFO` & `seatsio-73.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatsio
-Version: 72.4.0
+Version: 73.0.0
 Summary: The official Seats.io Python client library
 Home-page: https://github.com/seatsio/seatsio-python
 Author: The seats.io dev team
 Author-email: hello@seats.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `seatsio-72.4.0/README.md` & `seatsio-73.0.0/README.md`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/charts/chartsClient.py` & `seatsio-73.0.0/seatsio/charts/chartsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/charts/socialDistancingRulesetsRequest.py` & `seatsio-73.0.0/seatsio/charts/socialDistancingRulesetsRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/client.py` & `seatsio-73.0.0/seatsio/client.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/domain.py` & `seatsio-73.0.0/seatsio/domain.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/events/changeBestAvailableObjectStatusRequest.py` & `seatsio-73.0.0/seatsio/events/changeBestAvailableObjectStatusRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/events/changeObjectStatusRequest.py` & `seatsio-73.0.0/seatsio/events/changeObjectStatusRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/events/channelsClient.py` & `seatsio-73.0.0/seatsio/events/channelsClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,9 @@
     def remove_objects(self, event_key, channel_key, objects):
         self.http_client \
             .url("/events/{event_key}/channels/{channel_key}/objects", event_key=event_key, channel_key=channel_key) \
             .delete(EditObjectsForChannelRequest(objects))
 
     def replace(self, event_key, channels):
         self.http_client \
-            .url('/events/{event_key}/channels/update', event_key=event_key) \
+            .url('/events/{event_key}/channels/replace', event_key=event_key) \
             .post(ReplaceChannelsRequest(channels))
-
-    def set_objects(self, event_key, channels):
-        self.http_client \
-            .url('/events/{event_key}/channels/assign-objects', event_key=event_key) \
-            .post(AssignObjectsToChannelsRequest(channels))
```

### Comparing `seatsio-72.4.0/seatsio/events/channelsRequests.py` & `seatsio-73.0.0/seatsio/events/channelsRequests.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/events/createSingleEventRequest.py` & `seatsio-73.0.0/seatsio/events/createSingleEventRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/events/eventProperties.py` & `seatsio-73.0.0/seatsio/events/eventProperties.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/events/eventsClient.py` & `seatsio-73.0.0/seatsio/events/eventsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/events/statusChangeRequest.py` & `seatsio-73.0.0/seatsio/events/statusChangeRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/exceptions.py` & `seatsio-73.0.0/seatsio/exceptions.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/holdtokens/HoldTokenClient.py` & `seatsio-73.0.0/seatsio/holdtokens/HoldTokenClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/httpClient.py` & `seatsio-73.0.0/seatsio/httpClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/pagination/listableObjectsClient.py` & `seatsio-73.0.0/seatsio/pagination/listableObjectsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/pagination/lister.py` & `seatsio-73.0.0/seatsio/pagination/lister.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/pagination/page.py` & `seatsio-73.0.0/seatsio/pagination/page.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/pagination/pageFetcher.py` & `seatsio-73.0.0/seatsio/pagination/pageFetcher.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/pagination/pagedIterator.py` & `seatsio-73.0.0/seatsio/pagination/pagedIterator.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/reports/charts/chartReports.py` & `seatsio-73.0.0/seatsio/reports/charts/chartReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/reports/events/eventReports.py` & `seatsio-73.0.0/seatsio/reports/events/eventReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/reports/usage/usageReports.py` & `seatsio-73.0.0/seatsio/reports/usage/usageReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/seasons/seasonsClient.py` & `seatsio-73.0.0/seatsio/seasons/seasonsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/subaccounts/subaccountsClient.py` & `seatsio-73.0.0/seatsio/subaccounts/subaccountsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio/workspaces/workspacesClient.py` & `seatsio-73.0.0/seatsio/workspaces/workspacesClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/seatsio.egg-info/PKG-INFO` & `seatsio-73.0.0/seatsio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatsio
-Version: 72.4.0
+Version: 73.0.0
 Summary: The official Seats.io Python client library
 Home-page: https://github.com/seatsio/seatsio-python
 Author: The seats.io dev team
 Author-email: hello@seats.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `seatsio-72.4.0/seatsio.egg-info/SOURCES.txt` & `seatsio-73.0.0/seatsio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seatsio-72.4.0/setup.py` & `seatsio-73.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='seatsio',
-    version='v72.4.0',
+    version='v73.0.0',
     description='The official Seats.io Python client library',
     author='The seats.io dev team',
     author_email='hello@seats.io',
     url='https://github.com/seatsio/seatsio-python',
     license="MIT",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

