# Comparing `tmp/mistapi-0.37.8.tar.gz` & `tmp/mistapi-0.40.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistapi-0.37.8.tar", last modified: Thu Apr 20 15:20:01 2023, max compression
+gzip compressed data, was "mistapi-0.40.0.tar", last modified: Tue May 30 10:33:53 2023, max compression
```

## Comparing `mistapi-0.37.8.tar` & `mistapi-0.40.0.tar`

### file list

```diff
@@ -1,225 +1,234 @@
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.849753 mistapi-0.37.8/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.37.8/LICENSE
--rw-r--r--   0 tmunzer    (502) staff       (20)    11332 2023-04-20 15:20:01.849851 mistapi-0.37.8/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)    10556 2023-02-22 14:11:31.000000 mistapi-0.37.8/README.md
--rw-r--r--   0 tmunzer    (502) staff       (20)      976 2023-04-20 15:19:52.000000 mistapi-0.37.8/pyproject.toml
--rw-r--r--   0 tmunzer    (502) staff       (20)      125 2023-04-20 15:20:01.850288 mistapi-0.37.8/setup.cfg
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.780870 mistapi-0.37.8/src/
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.788537 mistapi-0.37.8/src/mistapi/
--rw-r--r--   0 tmunzer    (502) staff       (20)     7909 2023-04-20 13:57:39.000000 mistapi-0.37.8/src/mistapi/__api_request.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2962 2023-02-21 11:06:36.000000 mistapi-0.37.8/src/mistapi/__api_response.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    19300 2023-02-09 10:15:49.000000 mistapi-0.37.8/src/mistapi/__api_session.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      635 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2229 2023-02-13 15:54:52.000000 mistapi-0.37.8/src/mistapi/__logger.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.790821 mistapi-0.37.8/src/mistapi/__models/
--rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.37.8/src/mistapi/__models/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1514 2023-02-21 08:35:01.000000 mistapi-0.37.8/src/mistapi/__models/privilege.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2029 2023-02-09 11:01:08.000000 mistapi-0.37.8/src/mistapi/__pagination.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.791153 mistapi-0.37.8/src/mistapi/api/
--rw-r--r--   0 tmunzer    (502) staff       (20)      446 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.791450 mistapi-0.37.8/src/mistapi/api/v1/
--rw-r--r--   0 tmunzer    (502) staff       (20)      869 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.796844 mistapi-0.37.8/src/mistapi/api/v1/const/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1133 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/alarm_defs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2027 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/ap_channels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1730 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/ap_led_status.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1713 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/applications.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1756 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/call_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/client_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1707 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/countries.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1402 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/default_gateway_config.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/device_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/device_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1794 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/insight_metrics.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1712 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/languages.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/mxedge_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/mxedge_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/const/traffic_types.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.797164 mistapi-0.37.8/src/mistapi/api/v1/installer/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/installer/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.799476 mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)      798 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1968 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1968 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7123 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1972 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1947 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1940 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7487 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/sites.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.800024 mistapi-0.37.8/src/mistapi/api/v1/installer/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)      471 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/installer/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1168 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/installer/sites/optimize.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.800623 mistapi-0.37.8/src/mistapi/api/v1/invite/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/invite/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1099 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/invite/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.802419 mistapi-0.37.8/src/mistapi/api/v1/login/
--rw-r--r--   0 tmunzer    (502) staff       (20)      584 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/login/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1136 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/login/login.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1145 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/login/lookup.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2628 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/login/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1155 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/login/two_factor.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.803192 mistapi-0.37.8/src/mistapi/api/v1/logout/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/logout/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      984 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/logout/logout.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.803808 mistapi-0.37.8/src/mistapi/api/v1/mobile/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/mobile/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1257 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/mobile/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.809196 mistapi-0.37.8/src/mistapi/api/v1/msps/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1060 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1250 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1205 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2667 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2620 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1828 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/logo.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3330 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2981 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/msps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/orggroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5244 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1660 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/search.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4002 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5981 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3637 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3225 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/msps/tickets.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.830053 mistapi-0.37.8/src/mistapi/api/v1/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)     3119 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3255 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6440 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7576 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4730 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/aptemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5989 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2344 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1709 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/cert.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1250 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    11381 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1236 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/clone.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1846 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/crl.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7074 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    20129 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4812 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4870 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/gatewaytemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6514 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2978 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5034 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2667 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6927 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/jsi.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2503 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4995 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1434 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4754 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/mxclusters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    15280 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/nacrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4618 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/nactags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4872 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/networktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1407 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/ocdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2975 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5923 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1913 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/pma.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4702 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/pskportals.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8274 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4730 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1316 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/sdkclients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6892 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/sdkinvites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4719 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/sdktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4721 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4825 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    12674 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4702 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8619 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4788 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/sitetemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8223 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4767 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    32186 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1747 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5449 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/templates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6846 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/tickets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1758 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/troubleshoot.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4541 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3540 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7426 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5236 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5887 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/orgs/wxtunnels.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.830900 mistapi-0.37.8/src/mistapi/api/v1/recover/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/recover/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1158 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/recover/recover.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1110 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/recover/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.831700 mistapi-0.37.8/src/mistapi/api/v1/register/
--rw-r--r--   0 tmunzer    (502) staff       (20)      508 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/register/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1161 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/register/register.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1103 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/register/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.833965 mistapi-0.37.8/src/mistapi/api/v1/self/
--rw-r--r--   0 tmunzer    (502) staff       (20)      707 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/self/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2916 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/self/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2596 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/self/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2015 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/self/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2109 2023-04-20 15:19:52.000000 mistapi-0.37.8/src/mistapi/api/v1/self/self.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/self/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1837 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/self/two_factor.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1756 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/self/update.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.848575 mistapi-0.37.8/src/mistapi/api/v1/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)     2273 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8657 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2655 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/anomaly.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1861 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/apps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4797 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6038 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4659 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/beacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2356 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    17319 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2327 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/count.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    57887 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5037 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4073 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7034 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9142 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1157 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8539 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/location.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    14132 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5297 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1184 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3117 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5810 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/pcaps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7530 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5752 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/rfdiags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5721 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/rogues.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3809 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/rrm.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4711 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/rssizones.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5978 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2404 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3881 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/skyatp.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    20771 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/sle.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1970 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    61687 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1707 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1905 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/synthetic_test.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4633 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/uisettings.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4683 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/vbeacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2239 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/visits.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5300 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3839 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6811 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5279 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5936 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4711 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/wxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4599 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/sites/zones.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.849500 mistapi-0.37.8/src/mistapi/api/v1/utils/
--rw-r--r--   0 tmunzer    (502) staff       (20)      511 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/utils/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1072 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/utils/test_telstra.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1184 2023-04-20 15:19:53.000000 mistapi-0.37.8/src/mistapi/api/v1/utils/test_twilio.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8484 2023-04-20 15:18:53.000000 mistapi-0.37.8/src/mistapi/cli.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 15:20:01.790248 mistapi-0.37.8/src/mistapi.egg-info/
--rw-r--r--   0 tmunzer    (502) staff       (20)    11332 2023-04-20 15:20:01.000000 mistapi-0.37.8/src/mistapi.egg-info/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)     7303 2023-04-20 15:20:01.000000 mistapi-0.37.8/src/mistapi.egg-info/SOURCES.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        1 2023-04-20 15:20:01.000000 mistapi-0.37.8/src/mistapi.egg-info/dependency_links.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)       66 2023-04-20 15:20:01.000000 mistapi-0.37.8/src/mistapi.egg-info/requires.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        8 2023-04-20 15:20:01.000000 mistapi-0.37.8/src/mistapi.egg-info/top_level.txt
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.651244 mistapi-0.40.0/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.40.0/LICENSE
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11332 2023-05-30 10:33:53.651367 mistapi-0.40.0/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10556 2023-02-22 14:11:31.000000 mistapi-0.40.0/README.md
+-rw-r--r--   0 tmunzer    (502) staff       (20)      976 2023-05-30 10:33:26.000000 mistapi-0.40.0/pyproject.toml
+-rw-r--r--   0 tmunzer    (502) staff       (20)      125 2023-05-30 10:33:53.651761 mistapi-0.40.0/setup.cfg
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.533791 mistapi-0.40.0/src/
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.543086 mistapi-0.40.0/src/mistapi/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7909 2023-04-20 13:57:39.000000 mistapi-0.40.0/src/mistapi/__api_request.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2962 2023-02-21 11:06:36.000000 mistapi-0.40.0/src/mistapi/__api_response.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    21519 2023-05-30 10:13:58.000000 mistapi-0.40.0/src/mistapi/__api_session.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      635 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2229 2023-02-13 15:54:52.000000 mistapi-0.40.0/src/mistapi/__logger.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.546008 mistapi-0.40.0/src/mistapi/__models/
+-rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.40.0/src/mistapi/__models/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.40.0/src/mistapi/__models/privilege.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2029 2023-02-09 11:01:08.000000 mistapi-0.40.0/src/mistapi/__pagination.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.546486 mistapi-0.40.0/src/mistapi/api/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      446 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.547060 mistapi-0.40.0/src/mistapi/api/v1/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      902 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.555066 mistapi-0.40.0/src/mistapi/api/v1/const/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1181 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/alarm_defs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2027 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/ap_channels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1730 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/ap_led_status.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1713 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/applications.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1756 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/call_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/client_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1707 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/countries.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1402 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/default_gateway_config.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/device_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1794 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/insight_metrics.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1712 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/languages.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1055 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/license_types.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/mxedge_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/mxedge_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/traffic_types.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.555420 mistapi-0.40.0/src/mistapi/api/v1/installer/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.558171 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      798 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1968 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1968 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7123 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1972 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1947 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1940 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7487 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/sites.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.558968 mistapi-0.40.0/src/mistapi/api/v1/installer/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      471 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1168 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/sites/optimize.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.562177 mistapi-0.40.0/src/mistapi/api/v1/invite/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/invite/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1099 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/invite/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.573537 mistapi-0.40.0/src/mistapi/api/v1/login/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      584 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/login/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1136 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/login/login.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1145 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/login/lookup.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2628 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/login/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1155 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/login/two_factor.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.574222 mistapi-0.40.0/src/mistapi/api/v1/logout/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/logout/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      984 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/logout/logout.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.574981 mistapi-0.40.0/src/mistapi/api/v1/mobile/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/mobile/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1257 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/mobile/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.585094 mistapi-0.40.0/src/mistapi/api/v1/msps/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1250 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1205 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2667 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2620 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1828 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/logo.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3330 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2981 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/msps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/orggroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5244 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1660 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/search.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4002 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5981 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3637 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1476 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/suggestion.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3225 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/tickets.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.623098 mistapi-0.40.0/src/mistapi/api/v1/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3119 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3255 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6440 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7576 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4730 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/aptemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5989 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2344 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1709 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/cert.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1250 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11381 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1236 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/clone.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1846 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/crl.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7034 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    20091 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4812 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4870 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/gatewaytemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6514 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2978 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5034 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2667 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6927 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/jsi.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2503 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4955 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1434 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4754 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/mxclusters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    15280 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/nacrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4618 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/nactags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4872 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/networktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1407 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/ocdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2975 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5923 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1913 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/pma.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4702 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/pskportals.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8274 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4730 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1316 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/sdkclients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6892 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/sdkinvites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4719 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/sdktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4721 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4825 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    15912 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4702 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8619 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4788 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/sitetemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8223 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4767 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    32140 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1747 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5449 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/templates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6846 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/tickets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1758 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/troubleshoot.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4541 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3540 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7466 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5236 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5887 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/wxtunnels.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.624075 mistapi-0.40.0/src/mistapi/api/v1/recover/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/recover/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1158 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/recover/recover.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1110 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/recover/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.625257 mistapi-0.40.0/src/mistapi/api/v1/register/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      508 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/register/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1161 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/register/register.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1103 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/register/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.628675 mistapi-0.40.0/src/mistapi/api/v1/self/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      707 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2916 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2596 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2015 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2109 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/self.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1837 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/two_factor.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1756 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/update.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.631300 mistapi-0.40.0/src/mistapi/api/v1/site/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      637 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/site/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2334 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/site/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2292 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/site/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2341 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/site/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2292 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/site/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2264 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/site/vpns.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.649900 mistapi-0.40.0/src/mistapi/api/v1/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2273 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8657 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2655 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/anomaly.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1861 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/apps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4797 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6038 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4659 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/beacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2356 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    17187 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2327 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/count.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    58343 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5037 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4073 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7034 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9142 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1157 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8539 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/location.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    14930 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5297 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1184 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3117 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5810 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/pcaps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7530 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5752 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/rfdiags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5721 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/rogues.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3809 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/rrm.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4711 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/rssizones.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5978 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2404 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3837 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/skyatp.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    20771 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/sle.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1970 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    61251 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1707 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1905 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/synthetic_test.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4633 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/uisettings.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4683 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/vbeacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2239 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/visits.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5300 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3839 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6811 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5279 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5936 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4711 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/wxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4599 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/zones.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.650961 mistapi-0.40.0/src/mistapi/api/v1/utils/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      511 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/utils/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1072 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/utils/test_telstra.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1184 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/utils/test_twilio.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11444 2023-05-30 10:31:44.000000 mistapi-0.40.0/src/mistapi/cli.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.545377 mistapi-0.40.0/src/mistapi.egg-info/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11332 2023-05-30 10:33:53.000000 mistapi-0.40.0/src/mistapi.egg-info/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7608 2023-05-30 10:33:53.000000 mistapi-0.40.0/src/mistapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        1 2023-05-30 10:33:53.000000 mistapi-0.40.0/src/mistapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)       66 2023-05-30 10:33:53.000000 mistapi-0.40.0/src/mistapi.egg-info/requires.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        8 2023-05-30 10:33:53.000000 mistapi-0.40.0/src/mistapi.egg-info/top_level.txt
```

### Comparing `mistapi-0.37.8/LICENSE` & `mistapi-0.40.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/PKG-INFO` & `mistapi-0.40.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.37.8
+Version: 0.40.0
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.37.8/README.md` & `mistapi-0.40.0/README.md`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/pyproject.toml` & `mistapi-0.40.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mistapi"
-version = "0.37.8"
+version = "0.40.0"
 authors = [{name="Thomas Munzer", email="tmunzer@juniper.net"}]
 description = "Python package to simplify the Mist System APIs usage"
 keywords = ["Mist", "Juniper", "API"]
 license = {text =  "MIT"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mistapi-0.37.8/src/mistapi/__api_request.py` & `mistapi-0.40.0/src/mistapi/__api_request.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/__api_response.py` & `mistapi-0.40.0/src/mistapi/__api_response.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/__api_session.py` & `mistapi-0.40.0/src/mistapi/__api_session.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-'''
+"""
 --------------------------------------------------------------------------------
 ------------------------- Mist API Python CLI Session --------------------------
 
     Written by: Thomas Munzer (tmunzer@juniper.net)
     Github    : https://github.com/tmunzer/mistapi_python
 
     This package is licensed under the MIT License.
 
 --------------------------------------------------------------------------------
 This module provide the APISession class, which is used to manage authentication
 and HTTP session (if login/password is used) with Mist Cloud.
-'''
+"""
 
 import os
 import sys
 import requests
 from dotenv import load_dotenv
 from pathlib import Path
 from getpass import getpass
@@ -27,47 +27,43 @@
 
 ###### GLOBALS ######
 clouds = [
     {"short": "Europe 01", "host": "api.eu.mist.com", "cookies_ext": ".eu"},
     {"short": "Global 01", "host": "api.mist.com", "cookies_ext": ""},
     {"short": "Global 02", "host": "api.gc1.mist.com", "cookies_ext": ".gc1"},
     {"short": "Global 03", "host": "api.ac2.mist.com", "cookies_ext": ".ac2"},
-    {"short": "Global 04", "host": "api.gc2.mist.com", "cookies_ext": ".gc2"}
+    {"short": "Global 04", "host": "api.gc2.mist.com", "cookies_ext": ".gc2"},
 ]
 
 
-def _header():
-    print("""
---------------------------------------------------------------------------------
-------------------------- Mist API Python CLI Session --------------------------
-
-    Written by: Thomas Munzer (tmunzer@juniper.net)
-    Github    : https://github.com/tmunzer/mistapi_python
-
-    This package is licensed under the MIT License.
-
---------------------------------------------------------------------------------    
-    """)
-
-
 #### PARAMETERS #####
 
+
 class APISession(APIRequest):
     """Class managing REST API Session"""
 
-    def __init__(self, email: str = None, password: str = None, apitoken: str = None, host: str = None, env_file: str = None, console_log_level: str = 20, logging_log_level: int = 10):
+    def __init__(
+        self,
+        email: str = None,
+        password: str = None,
+        apitoken: str = None,
+        host: str = None,
+        env_file: str = None,
+        console_log_level: str = 20,
+        logging_log_level: int = 10,
+    ):
         """
         :param str email        used if login/password is used. Can be defined later
         :param str password     used if login/password is used. Can be defined later
         :param str apitoken     used if API Token is used. Can de defined later
         :param str host         Mist Cloud to reach (e.g. "api.mist.com"). Can de defined later
         :param str env_file     path to the env file to load. See README.md for allowed variables
         :param int console_log_level
         :param int logging_log_level
-        """        
+        """
         self._cloud_uri = None
         self.email = None
         self._password = None
         self._apitoken = None
         self._csrftoken = None
         self._authenticated = False
         self._session = requests.session()
@@ -90,19 +86,28 @@
         self.last_name = ""
         self.via_sso = False
         self.tags = []
 
         self.privileges = Privileges([])
         self.session_expiry = ""
 
-        logger.debug('API Session initialized')
+        logger.debug("API Session initialized")
 
     def __str__(self):
-        fields = ["email", "first_name", "last_name", "phone", "via_sso",
-                  "privileges", "session_expiry", "tags", "authenticated"]
+        fields = [
+            "email",
+            "first_name",
+            "last_name",
+            "phone",
+            "via_sso",
+            "privileges",
+            "session_expiry",
+            "tags",
+            "authenticated",
+        ]
         string = ""
         for field in fields:
             if hasattr(self, field) and getattr(self, field) != "":
                 string += f"{field}:\r\n"
                 if field == "privileges":
                     string += Privileges(self.privileges).display()
                     string += "\r\n"
@@ -112,65 +117,62 @@
                 elif field == "authenticated":
                     string += f"{self.get_authentication_status()}\r\n"
                 else:
                     string += f"{getattr(self, field)}\r\n"
                 string += "\r\n"
         return string
 
-
-####################################
-# LOAD FUNCTIONS
-
-
+    ####################################
+    # LOAD FUNCTIONS
     def _load_env(self, env_file=None):
         if env_file:
             if env_file.startswith("~/"):
-                env_file = os.path.join(os.path.expanduser('~'), env_file.replace("~/",""))
+                env_file = os.path.join(
+                    os.path.expanduser("~"), env_file.replace("~/", "")
+                )
             env_file = os.path.abspath(env_file)
             console.debug(f"Loading settings from {env_file}")
             logger.debug(f"apisession:Loading settings from {env_file}")
             dotenv_path = Path(env_file)
             load_dotenv(dotenv_path=dotenv_path)
         else:
             console.debug("Loading settings from env file")
             logger.debug(f"apisession:Loading settings from env file")
             load_dotenv()
 
-        if os.getenv('MIST_HOST'):
-            self.set_cloud(os.getenv('MIST_HOST'))
-        if os.getenv('MIST_APITOKEN'):
-            self.set_api_token(os.getenv('MIST_APITOKEN'))
-        if os.getenv('MIST_USER'):
-            self.set_email(os.getenv('MIST_USER'))
-        if os.getenv('MIST_PASSWORD'):
-            self.set_password(os.getenv('MIST_PASSWORD'))
-        if os.getenv('CONSOLE_LOG_LEVEL'):
-            self._console_log_level = os.getenv('CONSOLE_LOG_LEVEL')
-        if os.getenv('LOGGING_LOG_LEVEL'):
-            self._logging_log_level = os.getenv('LOGGING_LOG_LEVEL')
+        if os.getenv("MIST_HOST"):
+            self.set_cloud(os.getenv("MIST_HOST"))
+        if os.getenv("MIST_APITOKEN"):
+            self.set_api_token(os.getenv("MIST_APITOKEN"))
+        if os.getenv("MIST_USER"):
+            self.set_email(os.getenv("MIST_USER"))
+        if os.getenv("MIST_PASSWORD"):
+            self.set_password(os.getenv("MIST_PASSWORD"))
+        if os.getenv("CONSOLE_LOG_LEVEL"):
+            self._console_log_level = os.getenv("CONSOLE_LOG_LEVEL")
+        if os.getenv("LOGGING_LOG_LEVEL"):
+            self._logging_log_level = os.getenv("LOGGING_LOG_LEVEL")
 
-####################################
-# CLOUD FUNCTIONS
+    ####################################
+    # CLOUD FUNCTIONS
     def set_cloud(self, cloud_uri: str) -> None:
         """
         Set Mist Cloud to reach.
 
         PARAMS
         -----------
         :param str cloud_uri - Mist FQDN to reach ("api.mist.com", "api.eu.mist.com", ...)
         """
         logger.debug(f"apisession:in  > set_cloud")
         self._cloud_uri = None
         for cloud in clouds:
             if cloud["host"] == cloud_uri:
                 self._cloud_uri = cloud_uri
-                logger.debug(
-                    f"apisession:Mist Cloud configured to {self._cloud_uri}")
-                console.debug(
-                    f"Mist Cloud configured to {self._cloud_uri}")
+                logger.debug(f"apisession:Mist Cloud configured to {self._cloud_uri}")
+                console.debug(f"Mist Cloud configured to {self._cloud_uri}")
         if not self._cloud_uri:
             logger.error(f"apisession:{cloud_uri} is not valid")
             console.error(f"{cloud_uri} is not valid")
 
     def get_cloud(self):
         """
         Return the Mist Cloud currently configured
@@ -206,17 +208,16 @@
                 else:
                     print(f"Please enter a number between 0 and {i}.")
                     self.select_cloud()
             except:
                 print("\r\nPlease enter a number.")
                 self.select_cloud()
 
-####################################
-# AUTH FUNCTIONS
-
+    ####################################
+    # AUTH FUNCTIONS
     def set_email(self, email: str = None) -> None:
         """
         Set the user email
 
         PARAMS
         -----------
         :param str email    If no email provided, an interactive input will ask for it
@@ -251,22 +252,21 @@
 
         PARAMS
         -----------
         :param str apitoken
         """
         logger.debug(f"apisession:in  > set_api_token")
         self._apitoken = apitoken
-        self._session.headers.update(
-            {'Authorization': "Token " + self._apitoken})
+        self._session.headers.update({"Authorization": "Token " + self._apitoken})
         logger.debug(f"apisession:API Token configured")
         console.debug(f"API Token configured")
 
     def _process_login(self):
         """
-        Function to authenticate a user with login/password. 
+        Function to authenticate a user with login/password.
         Will create and store a session used by other requests.
         """
 
         logger.debug(f"apisession:in  > _process_login")
         print()
         print(" Login/Pwd authentication ".center(80, "-"))
         print()
@@ -275,40 +275,39 @@
         if not self.email:
             self.set_email()
         if not self._password:
             self.set_password()
 
         logger.debug(f"apisession:Email/Password configured")
         uri = "/api/v1/login"
-        body = {
-            "email": self.email,
-            "password": self._password
-        }
+        body = {"email": self.email, "password": self._password}
         resp = self._session.post(self._url(uri), json=body)
         if resp.status_code == 200:
             logger.info(f"apisession:Authentication successful!")
             console.info("Authentication successful!")
             self._set_authenticated(True)
         else:
             logger.error(
-                f"apisession:Authentication failed: {resp.json().get('detail')}")
+                f"apisession:Authentication failed: {resp.json().get('detail')}"
+            )
             console.error(f"Authentication failed: {resp.json().get('detail')}\r\n")
             self.email = None
             self._password = None
             logger.debug(
-                f"apisession:Email/Password cleaned up. Restarting authentication function")
+                f"apisession:Email/Password cleaned up. Restarting authentication function"
+            )
             self._process_login()
 
     def login(self):
         """
         Log in on the Mist Cloud.
         If information are missing to get connected, they will be requested
         during the process.
-        If login/password is used, 2FA may be requests. Once authenticated, 
-        the HTTP session and CSRF Token will be stored and used during the 
+        If login/password is used, 2FA may be requests. Once authenticated,
+        the HTTP session and CSRF Token will be stored and used during the
         future API requests.
         """
         logger.debug(f"apisession:in  > login")
         if self._authenticated:
             logger.info(f"apisession:Already logged in...")
             console.info("Already logged in...")
         else:
@@ -345,49 +344,51 @@
                     console.error(resp.json()["detail"])
                 except:
                     console.error(resp.text)
 
     def _set_authenticated(self, authentication_status: bool) -> None:
         """
         Set the authentication status.
-        If True and Login/password is used, extract the HTTP session and 
-        CSRF Token from the cookies and store them in memory to be used 
+        If True and Login/password is used, extract the HTTP session and
+        CSRF Token from the cookies and store them in memory to be used
         during the future API requests.
         If False, clear the CSRF Token and delete the HTTP session.
 
         PARAMS
         -----------
         :param bool authentication_status
         """
         logger.debug(f"apisession:in  > _set_authenticated")
-        logger.debug(
-            f"apisession:authentication_status is {authentication_status}")
+        logger.debug(f"apisession:authentication_status is {authentication_status}")
         if authentication_status == True:
             self._authenticated = True
             logger.info(f"apisession:Session is now Authenticated")
             if not self._apitoken:
                 logger.debug(f"apisession:Processing HTTP cookies")
                 try:
                     cookies_ext = next(
-                        item["cookies_ext"] for item in clouds if item["host"] == self._cloud_uri)
+                        item["cookies_ext"]
+                        for item in clouds
+                        if item["host"] == self._cloud_uri
+                    )
                     logger.info(f"apisession:HTTP session cookies extracted")
                 except:
                     cookies_ext = ""
-                    logger.error(
-                        f"apisession:Unable to extract HTTP session cookies")
-                self._csrftoken = self._session.cookies['csrftoken' + cookies_ext]
-                self._session.headers.update({'X-CSRFToken': self._csrftoken})
+                    logger.error(f"apisession:Unable to extract HTTP session cookies")
+                self._csrftoken = self._session.cookies["csrftoken" + cookies_ext]
+                self._session.headers.update({"X-CSRFToken": self._csrftoken})
                 logger.info(f"apisession:CSRF Token stored")
         elif authentication_status == False:
             self._authenticated = False
             logger.info(f"apisession:Session is now Unauthenticated")
             self._csrftoken = ""
             del self._session
             logger.info(
-                f"apisession:CSRFT Token is cleaned up and HTTP Session deleted")
+                f"apisession:CSRFT Token is cleaned up and HTTP Session deleted"
+            )
 
     def get_authentication_status(self) -> bool:
         """
         RETURN
         -----------
         Return the authentication status.
         """
@@ -395,16 +396,15 @@
         return self._authenticated or self._apitoken
 
     def get_api_token(self):
         """
         Retrieve and display the User/Org API Tokens
         """
         logger.debug(f"apisession:in  > list_api_token")
-        logger.info(
-            f"apisession:Sending GET request to \"/api/v1/self/apitokens\"")
+        logger.info(f'apisession:Sending GET request to "/api/v1/self/apitokens"')
         resp = self.mist_get("/api/v1/self/apitokens")
         return resp
 
     def create_api_token(self, token_name: str = None):
         """
         Create a new API Token with the current account (user/org)
 
@@ -412,29 +412,31 @@
         -----------
         :param str API token name (optional)
         """
         logger.debug(f"apisession:in  > create_api_token")
         if token_name:
             body = {"name": token_name}
         logger.info(
-            f"apisession:Sending POST request to \"/api/v1/self/apitokens\" with name \"{token_name}\"")
+            f'apisession:Sending POST request to "/api/v1/self/apitokens" with name "{token_name}"'
+        )
         resp = self.mist_post("/api/v1/self/apitokens", body=body)
         return resp
 
     def delete_api_token(self, token_id: str):
         """
         Delete an API Token based on its token_id
 
         PARAMS
         -----------
         :param str api token_id
         """
         logger.debug(f"apisession:in  > delete_api_token")
         logger.info(
-            f"apisession:Sending DELETE request to \"/api/v1/self/apitokens\" with token_id \"{token_id}\"")
+            f'apisession:Sending DELETE request to "/api/v1/self/apitokens" with token_id "{token_id}"'
+        )
         uri = f"https://{self._cloud_uri}/api/v1/self/apitokens/{token_id}"
         resp = self._session.delete(uri)
         return resp
 
     def _two_factor_authentication(self, two_factor: str) -> bool:
         """
         Function called when 2FA is requested by Mist Cloud to authenticate
@@ -449,71 +451,136 @@
         :return bool - True if authentication succeed, False otherwise
         """
         logger.debug(f"apisession:in  > two_factor_authentication")
         uri = "/api/v1/login"
         body = {
             "email": self.email,
             "password": self._password,
-            "two_factor": two_factor
+            "two_factor": two_factor,
         }
         resp = self._session.post(self._url(uri), json=body)
         if resp.status_code == 200:
             logger.info(f"apisession:2FA authentication successed")
             console.info("2FA authentication successed")
             self._set_authenticated(True)
             return True
         else:
             logger.error(
-                f"apisession:2FA authentication failed with error code: {resp.status_code}")
-            console.error(f"2FA authentication failed with error code: {resp.status_code}\r\n")
+                f"apisession:2FA authentication failed with error code: {resp.status_code}"
+            )
+            console.error(
+                f"2FA authentication failed with error code: {resp.status_code}\r\n"
+            )
             return False
 
     def _getself(self) -> None:
         """
         Retrieve information about the current user and store them in the current object.
         """
         logger.debug(f"apisession:in  > getself")
         uri = "/api/v1/self"
-        logger.info(f"apisession:Sending GET request to \"{uri}\"")
+        logger.info(f'apisession:Sending GET request to "{uri}"')
         resp = self.mist_get(uri)
         if resp.data:
             # Deal with 2FA if needed
             if (
-                resp.data.get('two_factor_required') is True
-                and resp.data.get('two_factor_passed') is False
+                resp.data.get("two_factor_required") is True
+                and resp.data.get("two_factor_passed") is False
             ):
                 logger.info(f"apisession:2FA request by Mist Cloud")
                 two_factor_ok = False
                 while not two_factor_ok:
-                    two_factor = input(
-                        "Two Factor Authentication code required: ")
+                    two_factor = input("Two Factor Authentication code required: ")
                     two_factor_ok = self._two_factor_authentication(two_factor)
                 self._getself()
             # Get details of the account
             else:
                 logger.info(
-                    f"apisession:Authentication Ok. Processing account privileges")
+                    f"apisession:Authentication Ok. Processing account privileges"
+                )
                 for key, val in resp.data.items():
                     if key == "privileges":
                         self.privileges = Privileges(resp.data["privileges"])
                     if key == "tags":
                         for tag in resp.data["tags"]:
                             self.tags.append(tag)
                     else:
                         setattr(self, key, val)
                 print()
                 print(" Authenticated ".center(80, "-"))
                 print(f"\r\nWelcome {self.first_name} {self.last_name}!\r\n")
                 logger.info(
-                    f"apisession:Account used: {self.first_name} {self.last_name}")
+                    f"apisession:Account used: {self.first_name} {self.last_name}"
+                )
                 return True
         else:
             logger.error(f"apisession:Authentication not valid...")
             console.error("Authentication not valid...\r\n")
             resp = input(
-                f"Do you want to try with new credentials for {self._cloud_uri} (y/N)? " % ())
+                f"Do you want to try with new credentials for {self._cloud_uri} (y/N)? "
+                % ()
+            )
             if resp.lower() == "y":
                 self._process_login()
                 return self._getself()
             else:
                 sys.exit(0)
 
+    ####################################
+    # PRIVILEGES
+
+    def get_privilege_by_org_id(self, org_id: str):
+        logger.debug(f"apisession:in  > get_privilege_by_org_id")
+        org_priv = next(
+            (priv for priv in self.privileges if priv.get("org_id") == org_id), None
+        )
+        if org_priv:
+            logger.info(f"apisession:org {org_id} privileges found in user info")
+            logger.debug(f"apisession:{org_priv}")
+            return org_priv
+        else:
+            logger.warn(
+                f"apisession:Unable of find org {org_id} privileges in user data"
+            )
+            logger.info(
+                f"apisession:Trying to request org {org_id} info from the Cloud"
+            )
+            uri = f"/api/v1/orgs/{org_id}"
+            msp_id = None
+            try:
+                resp = self.mist_get(uri)
+                if resp.data and resp.data.get("msp_id"):
+                    logger.info(
+                        f"apisession:org {org_id} belong to msp_id {resp.data['msp_id']}"
+                    )
+                    msp_id = resp.data.get("msp_id")
+                else:
+                    logger.warn(
+                        "apisession: Not able to find msp_id information in the org info"
+                    )
+            except:
+                logger.error("apisession:Error when retrieving org info")
+            if msp_id:
+                msp_priv = next(
+                    (
+                        priv
+                        for priv in self.privileges
+                        if priv.get("scope") == "msp" and priv.get("msp_id") == msp_id
+                    ),
+                    None,
+                )
+                if not msp_priv:
+                    logger.warn(
+                        f"apisession:Unable of find msp {msp_id} privileges in user data"
+                    )
+                    return None
+                else:
+                    return {
+                        "scope": "org",
+                        "org_id": org_id,
+                        "name": resp.data.get("name"),
+                        "role": msp_priv["role"],
+                        "msp_id": msp_id,
+                        "msp_name": msp_priv["name"],
+                        "orggroup_ids": resp.data.get("orggroup_ids"),
+                        "msp_logo_url": resp.data.get("logo_url")
+                    }
```

### Comparing `mistapi-0.37.8/src/mistapi/__logger.py` & `mistapi-0.40.0/src/mistapi/__logger.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/__models/privilege.py` & `mistapi-0.40.0/src/mistapi/__models/privilege.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class Privileges:
     def __init__(self, privileges):
         self.privileges = []
         for privilege in privileges:
             self.privileges.append(_Privilege(privilege))           
 
     def __str__(self):
-        columns_headers = ["scope", "name", "site_id", "org_name", "org_id", 'msp_name', "msp_id" ]
+        columns_headers = ["scope", "role", "name", "site_id", "org_name", "org_id", 'msp_name', "msp_id" ]
         table = []
         for entry in self.privileges:
             temp = []
             for field in columns_headers:
                 if hasattr(entry, field):
                     temp.append(str(getattr(entry, field)))
                 else:
@@ -38,14 +38,14 @@
         self.sitegroup_ids = ""
         for key, val in privilege.items():
             setattr(self, key, val)
 
 
 
     def __str__(self):
-        fields = ["scope", "org_id", "org_name", "msp_id", "msp_name",
+        fields = ["scope", "role", "org_id", "org_name", "msp_id", "msp_name",
                   "orggroup_ids", "name", "role", "site_id", "sitegroup_ids"]
         string = ""
         for field in fields:
             if getattr(self, field) != "":
                 string += f"{field}: {getattr(self, field)} \r\n"
         return string
```

### Comparing `mistapi-0.37.8/src/mistapi/__pagination.py` & `mistapi-0.40.0/src/mistapi/__pagination.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/__init__.py` & `mistapi-0.40.0/src/mistapi/api/v1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 from mistapi.api.v1 import logout
 from mistapi.api.v1 import mobile
 from mistapi.api.v1 import msps
 from mistapi.api.v1 import orgs
 from mistapi.api.v1 import recover
 from mistapi.api.v1 import register
 from mistapi.api.v1 import self
+from mistapi.api.v1 import site
 from mistapi.api.v1 import sites
 from mistapi.api.v1 import utils
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/__init__.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,10 +18,11 @@
 from mistapi.api.v1.const import client_events
 from mistapi.api.v1.const import countries
 from mistapi.api.v1.const import default_gateway_config
 from mistapi.api.v1.const import device_events
 from mistapi.api.v1.const import device_models
 from mistapi.api.v1.const import insight_metrics
 from mistapi.api.v1.const import languages
+from mistapi.api.v1.const import license_types
 from mistapi.api.v1.const import mxedge_events
 from mistapi.api.v1.const import mxedge_models
 from mistapi.api.v1.const import traffic_types
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/alarm_defs.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/countries.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listAlarmDefinitions")  
-def getAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listCountryCodes")  
+def getCountryCodes(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listAlarmDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listCountryCodes
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/alarm_defs"
+    uri = f"/api/v1/const/countries"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
+def listCountryCodes(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listAlarmDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listCountryCodes
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/alarm_defs"
+    uri = f"/api/v1/const/countries"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/ap_channels.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/ap_channels.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listApChannels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listApChannels")  
 def getApChannels(mist_session:_APISession, country_code:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApChannels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/ap_led_status.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/ap_led_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listApLedDefinition")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listApLedDefinition")  
 def getApLedDefinition(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApLedDefinition
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/applications.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listApplications")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listApplications")  
 def getApplications(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApplications
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/call_events.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/call_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listCallEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listCallEventsDefinitions")  
 def getCallEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listCallEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/client_events.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/client_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listClientEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listClientEventsDefinitions")  
 def getClientEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listClientEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/countries.py` & `mistapi-0.40.0/src/mistapi/api/v1/self/subscriptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listCountryCodes")  
-def getCountryCodes(mist_session:_APISession) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listAlarmSubscriptions")  
+def getAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listCountryCodes
+    API doc: https://doc.mist-lab.fr/#operation/listAlarmSubscriptions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/countries"
+    uri = f"/api/v1/self/subscriptions"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listCountryCodes(mist_session:_APISession) -> _APIResponse:
+def listAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listCountryCodes
+    API doc: https://doc.mist-lab.fr/#operation/listAlarmSubscriptions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/countries"
+    uri = f"/api/v1/self/subscriptions"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/default_gateway_config.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/default_gateway_config.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/device_events.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/device_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listDeviceEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listDeviceEventsDefinitions")  
 def getDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listDeviceEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/device_models.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/alarm_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listDeviceModels")  
-def getDeviceModels(mist_session:_APISession) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listAlarmDefinitions")  
+def getAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listDeviceModels
+    API doc: https://doc.mist-lab.fr/#operation/listAlarmDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/device_models"
+    uri = f"/api/v1/const/alarm_defs"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listDeviceModels(mist_session:_APISession) -> _APIResponse:
+def listAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listDeviceModels
+    API doc: https://doc.mist-lab.fr/#operation/listAlarmDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/device_models"
+    uri = f"/api/v1/const/alarm_defs"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/insight_metrics.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/insight_metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteAvailableInsightMetrics")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteAvailableInsightMetrics")  
 def getSiteAvailableInsightMetrics(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableInsightMetrics
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/languages.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/languages.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteLanguages")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteLanguages")  
 def getSiteLanguages(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteLanguages
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/mxedge_events.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/mxedge_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listMxEdgeEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMxEdgeEventsDefinitions")  
 def getMxEdgeEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/mxedge_models.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/mxedge_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listMxEdgeModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMxEdgeModels")  
 def getMxEdgeModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeModels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/const/traffic_types.py` & `mistapi-0.40.0/src/mistapi/api/v1/const/traffic_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listTrafficTypes")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listTrafficTypes")  
 def getTrafficTypes(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/__init__.py` & `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/alarmtemplates.py` & `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/alarmtemplates.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listInstallerAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerAlarmTemplates")  
 def getInstallerAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerAlarmTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/deviceprofiles.py` & `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/deviceprofiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listInstallerDeviceProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerDeviceProfiles")  
 def getInstallerDeviceProfiles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerDeviceProfiles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/devices.py` & `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listInstallerListOfRenctlyClaimedDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerListOfRenctlyClaimedDevices")  
 def getInstallerListOfRenctlyClaimedDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerListOfRenctlyClaimedDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/rftemplates.py` & `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/rftemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listInstallerRfTemplatesNames")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerRfTemplatesNames")  
 def getInstallerRfTemplatesNames(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerRfTemplatesNames
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/secpolicies.py` & `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/secpolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listInstallerSecPolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerSecPolicies")  
 def getInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSecPolicies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/sitegroups.py` & `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/sitegroups.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listInstallerSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerSiteGroups")  
 def getInstallerSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSiteGroups
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/installer/orgs/sites.py` & `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/sites.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listInstallerSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerSites")  
 def getInstallerSites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSites
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -78,15 +78,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listInstallerMaps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerMaps")  
 def getInstallerMaps(mist_session:_APISession, org_id:str, site_name:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerMaps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/installer/sites/optimize.py` & `mistapi-0.40.0/src/mistapi/api/v1/installer/sites/optimize.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/invite/verify.py` & `mistapi-0.40.0/src/mistapi/api/v1/invite/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/login/__init__.py` & `mistapi-0.40.0/src/mistapi/api/v1/login/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/login/login.py` & `mistapi-0.40.0/src/mistapi/api/v1/login/login.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/login/lookup.py` & `mistapi-0.40.0/src/mistapi/api/v1/login/lookup.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/login/oauth.py` & `mistapi-0.40.0/src/mistapi/api/v1/login/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/login/two_factor.py` & `mistapi-0.40.0/src/mistapi/api/v1/login/two_factor.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/logout/logout.py` & `mistapi-0.40.0/src/mistapi/api/v1/logout/logout.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/mobile/verify.py` & `mistapi-0.40.0/src/mistapi/api/v1/mobile/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/__init__.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 from mistapi.api.v1.msps import logs
 from mistapi.api.v1.msps import orggroups
 from mistapi.api.v1.msps import orgs
 from mistapi.api.v1.msps import search
 from mistapi.api.v1.msps import ssoroles
 from mistapi.api.v1.msps import ssos
 from mistapi.api.v1.msps import stats
+from mistapi.api.v1.msps import suggestion
 from mistapi.api.v1.msps import tickets
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/admins.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/admins.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listMspAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspAdmins")  
 def getMspAdmins(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspAdmins
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/claim.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/insights.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/inventory.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/invites.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/licenses.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/licenses.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listMspLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspLicenses")  
 def getMspLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLicenses
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/logo.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/logo.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/logs.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listMspLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspLogs")  
 def getMspLogs(mist_session:_APISession, msp_id:str, org_id:str=None, admin_name:str=None, message:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLogs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/msps.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/msps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/orggroups.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/orggroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listMspOrgGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspOrgGroups")  
 def getMspOrgGroups(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgGroups
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/orgs.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/orgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listMspOrgs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspOrgs")  
 def getMspOrgs(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/search.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/search.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/ssoroles.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/ssoroles.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listMspSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspSsoRoles")  
 def getMspSsoRoles(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoRoles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/ssos.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listMspSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspSsoLatestFailures")  
 def getMspSsoLatestFailures(mist_session:_APISession, msp_id:str, sso_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoLatestFailures
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/stats.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listMspOrgLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspOrgLicenses")  
 def getMspOrgLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgLicenses
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -53,15 +53,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/stats/licenses"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listMspOrgStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspOrgStats")  
 def getMspOrgStats(mist_session:_APISession, msp_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/msps/tickets.py` & `mistapi-0.40.0/src/mistapi/api/v1/msps/tickets.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listMspTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspTickets")  
 def getMspTickets(mist_session:_APISession, msp_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspTickets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/__init__.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/admins.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/admins.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgAdmins")  
 def getOrgAdmins(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAdmins
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/alarms.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/alarmtemplates.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/alarmtemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgAlarmTemplates")  
 def getOrgAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAlarmTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -77,15 +77,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarmtemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgSuppressedAlarms")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSuppressedAlarms")  
 def getOrgSuppressedAlarms(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSuppressedAlarms
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/apitokens.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/apitokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgApiTokens")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgApiTokens")  
 def getOrgApiTokens(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApiTokens
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/aptemplates.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/aptemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgAptemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgAptemplates")  
 def getOrgAptemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAptemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/assetfilters.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/assetfilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgAssetFilters")  
 def getOrgAssetFilters(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetFilters
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/assets.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgAssets")  
 def getOrgAssets(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/call.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/cert.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/cert.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/claim.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/clients.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/clone.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/clone.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/crl.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/crl.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/deviceprofiles.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/deviceprofiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgDeviceProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgDeviceProfiles")  
 def getOrgDeviceProfiles(mist_session:_APISession, org_id:str, type:str="ap", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDeviceProfiles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -164,17 +164,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/deviceprofiles/{deviceprofile_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def assignOrgDeviceProfileToDevices(mist_session:_APISession, org_id:str, deviceprofile_id:str, body:object) -> _APIResponse:
+def assignOrgDeviceProfile(mist_session:_APISession, org_id:str, deviceprofile_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/assignOrgDeviceProfileToDevices
+    API doc: https://doc.mist-lab.fr/#operation/assignOrgDeviceProfile
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -189,17 +189,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/deviceprofiles/{deviceprofile_id}/assign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def unassignOrgDeviceProfilesFromDevices(mist_session:_APISession, org_id:str, deviceprofile_id:str, body:object) -> _APIResponse:
+def unassignOrgDeviceProfiles(mist_session:_APISession, org_id:str, deviceprofile_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/unassignOrgDeviceProfilesFromDevices
+    API doc: https://doc.mist-lab.fr/#operation/unassignOrgDeviceProfiles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/devices.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgDevices")  
 def getOrgDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -279,15 +279,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgApsMacs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgApsMacs")  
 def getOrgApsMacs(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApsMacs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -394,15 +394,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
 def getOrgMultiSitesDevicesUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMultiSitesDevicesUpgrades
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -483,17 +483,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/devices/upgrade/{upgrade_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def removeOrgGatewaysTunnel(mist_session:_APISession, org_id:str, device_id:str, body:object) -> _APIResponse:
+def clearOrgTunnel(mist_session:_APISession, org_id:str, device_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/removeOrgGatewaysTunnel
+    API doc: https://doc.mist-lab.fr/#operation/clearOrgTunnel
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -508,17 +508,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/devices/{device_id}/clear_tunnels"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def createOrgGatewaysCredentials(mist_session:_APISession, org_id:str, device_id:str, body:object) -> _APIResponse:
+def provisionOrgTunnel(mist_session:_APISession, org_id:str, device_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgGatewaysCredentials
+    API doc: https://doc.mist-lab.fr/#operation/provisionOrgTunnel
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/evpn_topologies.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/evpn_topologies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgEvpnTopologies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgEvpnTopologies")  
 def getOrgEvpnTopologies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgEvpnTopologies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/gatewaytemplates.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/gatewaytemplates.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgGatewayTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgGatewayTemplates")  
 def getOrgGatewayTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGatewayTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/guests.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/guests.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgGuestAuthorizations")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgGuestAuthorizations")  
 def getOrgGuestAuthorizations(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGuestAuthorizations
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/insights.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/inventory.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/invites.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/jsi.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/jsi.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgJsiDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgJsiDevices")  
 def getOrgJsiDevices(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None, mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -146,15 +146,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/jsi/devices/{device_mac}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgJsiPastPurchases")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgJsiPastPurchases")  
 def getOrgJsiPastPurchases(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiPastPurchases
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/licenses.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/logs.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgLogs")  
 def getOrgLogs(mist_session:_APISession, org_id:str, site_id:str=None, admin_name:str=None, message:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgLogs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -91,17 +91,17 @@
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     if page: query_params["page"]=page
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countOrgLogsByDistinctAttributes(mist_session:_APISession, org_id:str, distinct:str, admin_id:str=None, admin_name:str=None, site_id:str=None, message:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countOrgLogs(mist_session:_APISession, org_id:str, distinct:str, admin_id:str=None, admin_name:str=None, site_id:str=None, message:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countOrgLogsByDistinctAttributes
+    API doc: https://doc.mist-lab.fr/#operation/countOrgLogs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/maps.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/maps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/mxclusters.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/mxclusters.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgMxEdgeClusters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgMxEdgeClusters")  
 def getOrgMxEdgeClusters(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeClusters
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/mxedges.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/mxedges.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgMxEdges")  
 def getOrgMxEdges(mist_session:_APISession, org_id:str, for_sites:str="any", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdges
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -167,15 +167,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/unassign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgMxEdgeUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgMxEdgeUpgrades")  
 def getOrgMxEdgeUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeUpgrades
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/mxtunnels.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/mxtunnels.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgMxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgMxTunnels")  
 def getOrgMxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxTunnels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/nacrules.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/nacrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgNacRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgNacRules")  
 def getOrgNacRules(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/nactags.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/nactags.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgNacTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgNacTags")  
 def getOrgNacTags(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacTags
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/networks.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgNetworks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgNetworks")  
 def getOrgNetworks(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/networktemplates.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/networktemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgNetworkTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgNetworkTemplates")  
 def getOrgNetworkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworkTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/ocdevices.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/ocdevices.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/orgs.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/orgs.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/otherdevices.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/otherdevices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgOtherDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgOtherDevices")  
 def getOrgOtherDevices(mist_session:_APISession, org_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgOtherDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/pma.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/pma.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgPmaDashboards")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgPmaDashboards")  
 def getOrgPmaDashboards(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPmaDashboards
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/pskportals.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/pskportals.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgPskPortals")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgPskPortals")  
 def getOrgPskPortals(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPskPortals
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/psks.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/psks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgPsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgPsks")  
 def getOrgPsks(mist_session:_APISession, org_id:str, name:str=None, ssid:str=None, role:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPsks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/rftemplates.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/rftemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgRfTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgRfTemplates")  
 def getOrgRfTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgRfTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/sdkclients.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/sdkclients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/sdkinvites.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/sdkinvites.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSdkInvites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSdkInvites")  
 def getSdkInvites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkInvites
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/sdktemplates.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/sdktemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSdkTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSdkTemplates")  
 def getSdkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/secpolicies.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/secpolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgSecPolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSecPolicies")  
 def getOrgSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSecPolicies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/servicepolicies.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/servicepolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgServicePolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgServicePolicies")  
 def getOrgServicePolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServicePolicies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/services.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgServices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgServices")  
 def getOrgServices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/setting.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/setting.py`

 * *Files 8% similar despite different names*

```diff
@@ -168,14 +168,146 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/cradlepoint/sync"
     resp = mist_session.mist_post(uri=uri)
     return resp
     
+def getOrgJamfAppLinkedStatus(mist_session:_APISession, org_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getOrgJamfAppLinkedStatus
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str org_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/setting/jamf/link_accounts"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def deleteOrgJamfAppAuthorization(mist_session:_APISession, org_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgJamfAppAuthorization
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str org_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/setting/jamf/link_accounts"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def addOrgJamfAppAuthorization(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/addOrgJamfAppAuthorization
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str org_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/setting/jamf/link_accounts"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
+def getOrgJsecCredential(mist_session:_APISession, org_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getOrgJsecCredential
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str org_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/setting/jse/setup"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def deleteOrgJsecCredential(mist_session:_APISession, org_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgJsecCredential
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str org_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/setting/jse/setup"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def setupOrgJsecCredential(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/setupOrgJsecCredential
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str org_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/setting/jse/setup"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
 def linkOrgToJuniperJuniperAccount(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/linkOrgToJuniperJuniperAccount
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -327,50 +459,26 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/zscaler/setup"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def udpateOrgZscalerCredential(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/udpateOrgZscalerCredential
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str org_id        
-    
-    BODY PARAMS
-    -----------
-    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/setting/zscaler/setup"
-    resp = mist_session.mist_put(uri=uri, body=body)
-    return resp
-    
 def getOrgOauthAppLinkedStatus(mist_session:_APISession, org_id:str, app_name:str, forward:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getOrgOauthAppLinkedStatus
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str app_name - OAuth application name (Example : zoom, teams, etc..)        
+    :param str app_name - OAuth application name (Example : zoom, teams, intune        
     
     QUERY PARAMS
     ------------
     :param str forward - Mist portal url to which backend needs to redirect after succesful OAuth authorization. **Required** to get the `authorization_url`        
     
     RETURN
     -----------
@@ -389,15 +497,15 @@
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str app_name - OAuth application name (Example : zoom, teams, etc..)        
+    :param str app_name - OAuth application name (Example : zoom, teams, intune        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/{app_name}/link_accounts"
     query_params={}
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/sitegroups.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/sitegroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSiteGroups")  
 def getOrgSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteGroups
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/sites.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/sites.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSites")  
 def getOrgSites(mist_session:_APISession, org_id:str, limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSites
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/sitetemplates.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/sitetemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgSiteTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSiteTemplates")  
 def getOrgSiteTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/ssoroles.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/ssoroles.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSsoRoles")  
 def getOrgSsoRoles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoRoles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/ssos.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgSsos")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSsos")  
 def getOrgSsos(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsos
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -146,15 +146,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSsoLatestFailures")  
 def getOrgSsoLatestFailures(mist_session:_APISession, org_id:str, sso_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoLatestFailures
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/ssr.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/ssr.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/128routers/register_cmd"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgSsrUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSsrUpgrades")  
 def getOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/stats.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgAssetsStats")  
 def getOrgAssetsStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -241,15 +241,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/stats/bgp_peers/search"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgDevicesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgDevicesStats")  
 def getOrgDevicesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", type:str="ap", status:str="all", site_id:str=None, mac:str=None, evpntopo_id:str=None, evpn_unused:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevicesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -334,15 +334,15 @@
     if site_id: query_params["site_id"]=site_id
     if mac: query_params["mac"]=mac
     if evpntopo_id: query_params["evpntopo_id"]=evpntopo_id
     if evpn_unused: query_params["evpn_unused"]=evpn_unused
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgMxEdgesStats")  
 def getOrgMxEdgesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", for_site:str="false") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -541,17 +541,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countOrgByDisctinctAttributesOfSwitchPorts(mist_session:_APISession, org_id:str, distinct:str="mac", full_duplex:bool=None, mac:str=None, neighbor_mac:str=None, neighbor_port_desc:str=None, neighbor_system_name:str=None, poe_disabled:bool=None, poe_mode:str=None, poe_on:bool=None, port_id:str=None, port_mac:str=None, power_draw:float=None, tx_pkts:int=None, rx_pkts:int=None, rx_bytes:int=None, tx_bps:int=None, rx_bps:int=None, tx_mcast_pkts:int=None, tx_bcast_pkts:int=None, rx_mcast_pkts:int=None, rx_bcast_pkts:int=None, speed:int=None, stp_state:str=None, stp_role:str=None, auth_state:str=None, up:bool=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countOrgSwitchPorts(mist_session:_APISession, org_id:str, distinct:str="mac", full_duplex:bool=None, mac:str=None, neighbor_mac:str=None, neighbor_port_desc:str=None, neighbor_system_name:str=None, poe_disabled:bool=None, poe_mode:str=None, poe_on:bool=None, port_id:str=None, port_mac:str=None, power_draw:float=None, tx_pkts:int=None, rx_pkts:int=None, rx_bytes:int=None, tx_bps:int=None, rx_bps:int=None, tx_mcast_pkts:int=None, tx_bcast_pkts:int=None, rx_mcast_pkts:int=None, rx_bcast_pkts:int=None, speed:int=None, stp_state:str=None, stp_role:str=None, auth_state:str=None, up:bool=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countOrgByDisctinctAttributesOfSwitchPorts
+    API doc: https://doc.mist-lab.fr/#operation/countOrgSwitchPorts
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/subscriptions.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/templates.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgTemplates")  
 def getOrgTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/tickets.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/tickets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgTickets")  
 def getOrgTickets(mist_session:_APISession, org_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTickets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/troubleshoot.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/troubleshoot.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/vpns.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/vpns.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgsVpns")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgsVpns")  
 def getOrgsVpns(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/webhooks.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/webhooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgWebhooks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgWebhooks")  
 def getOrgWebhooks(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWebhooks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/wired_clients.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/wlans.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/wlans.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgWlans")  
 def getOrgWlans(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWlans
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -91,15 +91,15 @@
     
     PATH PARAMS
     -----------
     :param str org_id        
     
     QUERY PARAMS
     ------------
-    :param bool resolve - whether to resolve SITE_VARS        
+    :param bool resolve - whether to resolve SITE_VARS, default is false (as filter, optional)        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wlans/derived"
     query_params={}
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/wxrules.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/wxrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgWxRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgWxRules")  
 def getOrgWxRules(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/wxtags.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/wxtags.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgWxTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgWxTags")  
 def getOrgWxTags(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTags
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/orgs/wxtunnels.py` & `mistapi-0.40.0/src/mistapi/api/v1/orgs/wxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listOrgWxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgWxTunnels")  
 def getOrgWxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTunnels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/recover/recover.py` & `mistapi-0.40.0/src/mistapi/api/v1/recover/recover.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/recover/verify.py` & `mistapi-0.40.0/src/mistapi/api/v1/recover/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/register/register.py` & `mistapi-0.40.0/src/mistapi/api/v1/register/register.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/register/verify.py` & `mistapi-0.40.0/src/mistapi/api/v1/register/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/self/__init__.py` & `mistapi-0.40.0/src/mistapi/api/v1/self/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/self/apitokens.py` & `mistapi-0.40.0/src/mistapi/api/v1/self/apitokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listApiTokens")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listApiTokens")  
 def getApiTokens(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApiTokens
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/self/logs.py` & `mistapi-0.40.0/src/mistapi/api/v1/self/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSelfAuditLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSelfAuditLogs")  
 def getSelfAuditLogs(mist_session:_APISession, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSelfAuditLogs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/self/oauth.py` & `mistapi-0.40.0/src/mistapi/api/v1/self/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/self/self.py` & `mistapi-0.40.0/src/mistapi/api/v1/self/self.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/self/subscriptions.py` & `mistapi-0.40.0/src/mistapi/api/v1/self/two_factor.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,42 +10,49 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listAlarmSubscriptions")  
-def getAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
+def generateQrCodeForVerification(mist_session:_APISession, by:str="qrcode") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listAlarmSubscriptions
+    API doc: https://doc.mist-lab.fr/#operation/generateQrCodeForVerification
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    QUERY PARAMS
+    ------------
+    :param str by(qrcode)        
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/subscriptions"
-    query_params={}
+    uri = f"/api/v1/self/two_factor/token"
+    query_params={}
+    if by: query_params["by"]=by
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
+def verifyTwoFactor(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listAlarmSubscriptions
+    API doc: https://doc.mist-lab.fr/#operation/verifyTwoFactor
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/subscriptions"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/self/two_factor/verify"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/self/two_factor.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/sites.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,49 +10,73 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def generateQrCodeForVerification(mist_session:_APISession, by:str="qrcode") -> _APIResponse:
+def getSiteInfo(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/generateQrCodeForVerification
+    API doc: https://doc.mist-lab.fr/#operation/getSiteInfo
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    QUERY PARAMS
-    ------------
-    :param str by(qrcode)        
+    PATH PARAMS
+    -----------
+    :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/two_factor/token"
-    query_params={}
-    if by: query_params["by"]=by
+    uri = f"/api/v1/sites/{site_id}"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def verifyTwoFactor(mist_session:_APISession, body:object) -> _APIResponse:
+def deleteSite(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/verifyTwoFactor
+    API doc: https://doc.mist-lab.fr/#operation/deleteSite
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    :param str site_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def updateSiteInfo(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteInfo
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id        
+    
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/two_factor/verify"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/self/update.py` & `mistapi-0.40.0/src/mistapi/api/v1/self/update.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/__init__.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/alarms.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/anomaly.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/anomaly.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/apps.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteApps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteApps")  
 def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteApps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/assetfilters.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/assetfilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteAssetFilters")  
 def getSiteAssetFilters(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetFilters
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/assets.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteAssets")  
 def getSiteAssets(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/beacons.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/beacons.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteBeacons")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteBeacons")  
 def getSiteBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeacons
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/call.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/clients.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countSiteByDistinctAttributesOfClients(mist_session:_APISession, site_id:str, distinct:str, ssid:str=None, ap:str=None, ip_address:str=None, vlan:str=None, hostname:str=None, os:str=None, model:str=None, device:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteClients(mist_session:_APISession, site_id:str, distinct:str, ssid:str=None, ap:str=None, ip_address:str=None, vlan:str=None, hostname:str=None, os:str=None, model:str=None, device:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteByDistinctAttributesOfClients
+    API doc: https://doc.mist-lab.fr/#operation/countSiteClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -86,17 +86,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/clients/disconnect"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def countSiteByDistinctAttributesOfClientsEvents(mist_session:_APISession, site_id:str, distinct:str=None, type:str=None, reason_code:int=None, ssid:str=None, ap:str=None, proto:str=None, band:str=None, wlan_id:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteClientsEvents(mist_session:_APISession, site_id:str, distinct:str=None, type:str=None, reason_code:int=None, ssid:str=None, ap:str=None, proto:str=None, band:str=None, wlan_id:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteByDistinctAttributesOfClientsEvents
+    API doc: https://doc.mist-lab.fr/#operation/countSiteClientsEvents
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -232,17 +232,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countSiteByDistinctAttributesOfClientSessions(mist_session:_APISession, site_id:str, distinct:str="mac", ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteClientSessions(mist_session:_APISession, site_id:str, distinct:str="mac", ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteByDistinctAttributesOfClientSessions
+    API doc: https://doc.mist-lab.fr/#operation/countSiteClientSessions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/count.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/count.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/devices.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteDevices")  
 def getSiteDevices(mist_session:_APISession, site_id:str, type:str="ap", name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -673,64 +673,68 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/upgrade/{upgrade_id}/cancel"
     resp = mist_session.mist_post(uri=uri)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteAvailableDeviceVersions")  
-def getSiteAvailableDeviceVersions(mist_session:_APISession, site_id:str, type:str="ap") -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteAvailableDeviceVersions")  
+def getSiteAvailableDeviceVersions(mist_session:_APISession, site_id:str, type:str="ap", model:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableDeviceVersions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     QUERY PARAMS
     ------------
-    :param str type(ap, switch, gateway)        
+    :param str type(ap, switch, gateway) - fetch version for device type (E.g. switch)
+    :param str model - fetch version for device model, use/combine with `type` as needed (for switch and gateway devices)        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/versions"
     query_params={}
-    if type: query_params["type"]=type
+    if type: query_params["type"]=type
+    if model: query_params["model"]=model
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteAvailableDeviceVersions(mist_session:_APISession, site_id:str, type:str="ap") -> _APIResponse:
+def listSiteAvailableDeviceVersions(mist_session:_APISession, site_id:str, type:str="ap", model:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableDeviceVersions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     QUERY PARAMS
     ------------
-    :param str type(ap, switch, gateway)        
+    :param str type(ap, switch, gateway) - fetch version for device type (E.g. switch)
+    :param str model - fetch version for device model, use/combine with `type` as needed (for switch and gateway devices)        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/versions"
     query_params={}
-    if type: query_params["type"]=type
+    if type: query_params["type"]=type
+    if model: query_params["model"]=model
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def zeroizeSiteFipsAllAps(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/zeroizeSiteFipsAllAps
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/events.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/events.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/evpn_topologies.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/evpn_topologies.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/guests.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/guests.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteAllGuestAuthorizations")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteAllGuestAuthorizations")  
 def getSiteAllGuestAuthorizations(mist_session:_APISession, site_id:str, wlan_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAllGuestAuthorizations
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/insights.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/insights.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteRogueAPs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteRogueAPs")  
 def getSiteRogueAPs(mist_session:_APISession, site_id:str, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueAPs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -159,15 +159,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteRogueClients")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteRogueClients")  
 def getSiteRogueClients(mist_session:_APISession, site_id:str, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/licenses.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/location.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/location.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/maps.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteMaps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteMaps")  
 def getSiteMaps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMaps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -428,14 +428,39 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/{map_id}/set_map"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
+def confirmSiteApLocalizationData(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/confirmSiteApLocalizationData
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id
+    :param str map_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/use_auto_ap_values"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
 def importSiteWayfindings(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importSiteWayfindings
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/mxedges.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/mxedges.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteMxEdges")  
 def getSiteMxEdges(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdges
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/mxtunnels.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/mxtunnels.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/otherdevices.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/otherdevices.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteOtherDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteOtherDevices")  
 def getSiteOtherDevices(mist_session:_APISession, site_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteOtherDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/pcaps.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/pcaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSitePacketCaptures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSitePacketCaptures")  
 def getSitePacketCaptures(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", client_mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePacketCaptures
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/psks.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/psks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSitePsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSitePsks")  
 def getSitePsks(mist_session:_APISession, site_id:str, ssid:str=None, role:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePsks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/rfdiags.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/rfdiags.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/rogues.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/rogues.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/rrm.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/rrm.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/rssizones.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/rssizones.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteRssiZones")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteRssiZones")  
 def getSiteRssiZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRssiZones
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/setting.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/sites.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/subscriptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,73 +10,48 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteInfo(mist_session:_APISession, site_id:str) -> _APIResponse:
+def UnsubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteInfo
+    API doc: https://doc.mist-lab.fr/#operation/UnsubscribeSite
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def deleteSite(mist_session:_APISession, site_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSite
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str site_id        
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}"
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteInfo(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def SubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteInfo
+    API doc: https://doc.mist-lab.fr/#operation/SubscribeSite
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
-    BODY PARAMS
-    -----------
-    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
-    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
+    resp = mist_session.mist_post(uri=uri)
     return resp
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/skyatp.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/skyatp.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countSiteByDistringAttributesOfSkyatpEvents(mist_session:_APISession, site_id:str, distinct:str="type", type:str=None, mac:str=None, device_mac:str=None, threat_level:int=None, ip_address:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteSkyatpEvents(mist_session:_APISession, site_id:str, distinct:str="type", type:str=None, mac:str=None, device_mac:str=None, threat_level:int=None, ip_address:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteByDistringAttributesOfSkyatpEvents
+    API doc: https://doc.mist-lab.fr/#operation/countSiteSkyatpEvents
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/sle.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/sle.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/ssr.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/ssr.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/stats.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     if distinct: query_params["distinct"]=distinct
     if device_mac: query_params["device_mac"]=device_mac
     if app: query_params["app"]=app
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteAssetsStats")  
 def getSiteAssetsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -248,15 +248,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteBeaconsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteBeaconsStats")  
 def getSiteBeaconsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeaconsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -366,40 +366,42 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/bgp_peers/search"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countSiteCalls(mist_session:_APISession, site_id:str, distrinct:str="mac", app:str=None, start:str=None, end:str=None) -> _APIResponse:
+def countSiteCalls(mist_session:_APISession, site_id:str, distrinct:str="mac", rating:int=None, app:str=None, start:str=None, end:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countSiteCalls
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     QUERY PARAMS
     ------------
     :param str distrinct(mac)
+    :param int rating - feedback rating (e.g. "rating=1" or "rating=1,2")
     :param str app
     :param str start
     :param str end        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/calls/count"
     query_params={}
     if distrinct: query_params["distrinct"]=distrinct
+    if rating: query_params["rating"]=rating
     if app: query_params["app"]=app
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def searchSiteCalls(mist_session:_APISession, site_id:str, mac:str=None, app:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
@@ -434,15 +436,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteClientsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteClientsStats")  
 def getSiteClientsStats(mist_session:_APISession, site_id:str, wired:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteClientsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -514,88 +516,76 @@
     """
     uri = f"/api/v1/sites/{site_id}/stats/clients/{client_mac}"
     query_params={}
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteDevicesStats")  
-def getSiteDevicesStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", type:str="ap", status:str="all") -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteDevicesStats")  
+def getSiteDevicesStats(mist_session:_APISession, site_id:str, type:str="ap", status:str="all", page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     QUERY PARAMS
     ------------
-    :param int page
-    :param int limit
-    :param int start
-    :param int end
-    :param str duration
     :param str type(ap, switch, gateway, all)
-    :param str status(all, connected, disconnected)        
+    :param str status(all, connected, disconnected)
+    :param int page
+    :param int limit        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/devices"
     query_params={}
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
     if type: query_params["type"]=type
-    if status: query_params["status"]=status
+    if status: query_params["status"]=status
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteDevicesStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", type:str="ap", status:str="all") -> _APIResponse:
+def listSiteDevicesStats(mist_session:_APISession, site_id:str, type:str="ap", status:str="all", page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     QUERY PARAMS
     ------------
-    :param int page
-    :param int limit
-    :param int start
-    :param int end
-    :param str duration
     :param str type(ap, switch, gateway, all)
-    :param str status(all, connected, disconnected)        
+    :param str status(all, connected, disconnected)
+    :param int page
+    :param int limit        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/devices"
     query_params={}
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
     if type: query_params["type"]=type
-    if status: query_params["status"]=status
+    if status: query_params["status"]=status
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def getSiteDeviceStats(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteDeviceStats
     
@@ -635,15 +625,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/devices/{device_id}/clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteDiscoveredAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteDiscoveredAssets")  
 def getSiteDiscoveredAssets(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDiscoveredAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -982,15 +972,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/sdkclients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteUnconnectedClientStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteUnconnectedClientStats")  
 def getSiteUnconnectedClientStats(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteUnconnectedClientStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -1027,15 +1017,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/unconnected_clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteMxEdgesStats")  
 def getSiteMxEdgesStats(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdgesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -1092,17 +1082,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/mxedges/{mxedge_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countSiteByDisctinctAttributesOPorts(mist_session:_APISession, site_id:str, distinct:str="mac", full_duplex:bool=None, mac:str=None, neighbor_mac:str=None, neighbor_port_desc:str=None, neighbor_system_name:str=None, poe_disabled:bool=None, poe_mode:str=None, poe_on:bool=None, port_id:str=None, port_mac:str=None, power_draw:float=None, tx_pkts:int=None, rx_pkts:int=None, rx_bytes:int=None, tx_bps:int=None, rx_bps:int=None, tx_mcast_pkts:int=None, tx_bcast_pkts:int=None, rx_mcast_pkts:int=None, rx_bcast_pkts:int=None, speed:int=None, stp_state:str=None, stp_role:str=None, auth_state:str=None, up:bool=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteSwOrGwPorts(mist_session:_APISession, site_id:str, distinct:str="mac", full_duplex:bool=None, mac:str=None, neighbor_mac:str=None, neighbor_port_desc:str=None, neighbor_system_name:str=None, poe_disabled:bool=None, poe_mode:str=None, poe_on:bool=None, port_id:str=None, port_mac:str=None, power_draw:float=None, tx_pkts:int=None, rx_pkts:int=None, rx_bytes:int=None, tx_bps:int=None, rx_bps:int=None, tx_mcast_pkts:int=None, tx_bcast_pkts:int=None, rx_mcast_pkts:int=None, rx_bcast_pkts:int=None, speed:int=None, stp_state:str=None, stp_role:str=None, auth_state:str=None, up:bool=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteByDisctinctAttributesOPorts
+    API doc: https://doc.mist-lab.fr/#operation/countSiteSwOrGwPorts
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -1292,17 +1282,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/sdkclients/{sdkclient_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countSiteByDisctinctAttributesOfSwitchPorts(mist_session:_APISession, site_id:str, distinct:str="mac", full_duplex:bool=None, mac:str=None, neighbor_mac:str=None, neighbor_port_desc:str=None, neighbor_system_name:str=None, poe_disabled:bool=None, poe_mode:str=None, poe_on:bool=None, port_id:str=None, port_mac:str=None, power_draw:float=None, tx_pkts:int=None, rx_pkts:int=None, rx_bytes:int=None, tx_bps:int=None, rx_bps:int=None, tx_mcast_pkts:int=None, tx_bcast_pkts:int=None, rx_mcast_pkts:int=None, rx_bcast_pkts:int=None, speed:int=None, stp_state:str=None, stp_role:str=None, auth_state:str=None, up:bool=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteSwitchPorts(mist_session:_APISession, site_id:str, distinct:str="mac", full_duplex:bool=None, mac:str=None, neighbor_mac:str=None, neighbor_port_desc:str=None, neighbor_system_name:str=None, poe_disabled:bool=None, poe_mode:str=None, poe_on:bool=None, port_id:str=None, port_mac:str=None, power_draw:float=None, tx_pkts:int=None, rx_pkts:int=None, rx_bytes:int=None, tx_bps:int=None, rx_bps:int=None, tx_mcast_pkts:int=None, tx_bcast_pkts:int=None, rx_mcast_pkts:int=None, rx_bcast_pkts:int=None, speed:int=None, stp_state:str=None, stp_role:str=None, auth_state:str=None, up:bool=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteByDisctinctAttributesOfSwitchPorts
+    API doc: https://doc.mist-lab.fr/#operation/countSiteSwitchPorts
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -1529,15 +1519,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/wxrules"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteZonesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteZonesStats")  
 def getSiteZonesStats(mist_session:_APISession, site_id:str, map_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteZonesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/subscriptions.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/synthetic_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,48 +10,52 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def UnsubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteSyntheticTestStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/UnsubscribeSite
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSyntheticTestStatus
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/subscriptions"
+    uri = f"/api/v1/sites/{site_id}/synthetic_test"
     query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def SubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
+def triggerSiteSyntheticTest(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/SubscribeSite
+    API doc: https://doc.mist-lab.fr/#operation/triggerSiteSyntheticTest
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/subscriptions"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/sites/{site_id}/synthetic_test"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/synthetic_test.py` & `mistapi-0.40.0/src/mistapi/api/v1/site/services.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,52 +10,60 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteSyntheticTestStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteServicesDerived")  
+def getSiteServicesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteSyntheticTestStatus
+    API doc: https://doc.mist-lab.fr/#operation/listSiteServicesDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    QUERY PARAMS
+    ------------
+    :param bool resolve - whether resolve the site variables        
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/synthetic_test"
-    query_params={}
+    uri = f"/api/v1/site/{site_id}/services/derived"
+    query_params={}
+    if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def triggerSiteSyntheticTest(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def listSiteServicesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/triggerSiteSyntheticTest
+    API doc: https://doc.mist-lab.fr/#operation/listSiteServicesDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
-    BODY PARAMS
-    -----------
-    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    QUERY PARAMS
+    ------------
+    :param bool resolve - whether resolve the site variables        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/synthetic_test"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/site/{site_id}/services/derived"
+    query_params={}
+    if resolve: query_params["resolve"]=resolve
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/uisettings.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/uisettings.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/vbeacons.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/vbeacons.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteVBeacons")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteVBeacons")  
 def getSiteVBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteVBeacons
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/visits.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/visits.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/webhooks.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/webhooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteWebhooks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteWebhooks")  
 def getSiteWebhooks(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWebhooks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/wired_clients.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/wlans.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/wlans.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteWlans")  
 def getSiteWlans(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWlans
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/wxrules.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/wxrules.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteWxRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteWxRules")  
 def getSiteWxRules(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/wxtags.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/wxtags.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteWxTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteWxTags")  
 def getSiteWxTags(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/wxtunnels.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/wxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteWxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteWxTunnels")  
 def getSiteWxTunnels(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/sites/zones.py` & `mistapi-0.40.0/src/mistapi/api/v1/sites/zones.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.37.8", details="function replaced with listSiteZones")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteZones")  
 def getSiteZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteZones
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/utils/test_telstra.py` & `mistapi-0.40.0/src/mistapi/api/v1/utils/test_telstra.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/api/v1/utils/test_twilio.py` & `mistapi-0.40.0/src/mistapi/api/v1/utils/test_twilio.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.8/src/mistapi/cli.py` & `mistapi-0.40.0/src/mistapi/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,167 +1,253 @@
-'''
+"""
 --------------------------------------------------------------------------------
 ------------------------- Mist API Python CLI Session --------------------------
 
     Written by: Thomas Munzer (tmunzer@juniper.net)
     Github    : https://github.com/tmunzer/mistapi_python
 
     This package is licensed under the MIT License.
 
 --------------------------------------------------------------------------------
 This module is providing some functions to simplify Mist API use.
-'''
+"""
 
 import mistapi as mistapi
 import sys
 import json
 from tabulate import tabulate
 
+
 ###########################################
 def _search_org(orgs, org_id):
     i = 0
     for org in orgs:
-        if org['org_id'] == org_id:
+        if org["org_id"] == org_id:
             return i
-        i+=1
+        i += 1
     return None
 
+
 def _test_choice(val, val_max):
     try:
         val_int = int(val)
         if val_int >= 0 and val_int <= val_max:
             return val_int
         else:
             return -1
     except:
         return -2
 
+
 ###########################################
 #### CLI SELECTIONS
-def select_org(mist_session:mistapi.APISession, allow_many=False) -> list:
+def _forge_privileges(mist_session: mistapi.APISession, msp_id: str):
+    """
+    Function to generate user privileges for Orgs belonging to a MSP Account
+
+    PARAMS
+    -----------
+    :param APISession   mist_session - mistapi session including authentication and Mist host information
+    :param str          msp_id - msp_id of the MSP account to use to generate the privileges
+
+    RETURN
+    -----------
+    :return list - List of ORG privileges
+    """
+    resp = mistapi.api.v1.msps.orgs.listMspOrgs(mist_session, msp_id)
+    orgs = mistapi.get_all(mist_session, resp)
+    custom_privileges = []
+    for org in orgs:
+        custom_privileges.append(mist_session.get_privilege_by_org_id(org["id"]))
+    return custom_privileges
+
+
+def _select_msp(mist_session: mistapi.APISession) -> list:
+    """
+    Function to list all the Mist MSPs allowed for the current user
+    and ask to pick one. Return the list org ORG privileges based
+    on the user selection
+
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+
+    RETURN
+    -----------
+    :return list - List of ORG privileges
+    """
+    msp_accounts = [
+        priv for priv in mist_session.privileges if priv.get("scope") == "msp"
+    ]
+    if len(msp_accounts) == 0:
+        return mist_session.privileges
+    else:
+        msp_accounts = sorted(msp_accounts, key=lambda x: x["name"].lower())
+        while True:
+            i = -1
+            print("\r\nAvailable MSP Accounts:")
+            for privilege in msp_accounts:
+                i += 1
+                print(f"{i}) {privilege['name']} (id: {privilege['msp_id']})")
+
+            resp = input(
+                f'\r\nSelect the MSP Account to use (0 to {i}, "n" for None, or "q" to quit): '
+            )
+            if resp == "q":
+                sys.exit(0)
+            elif resp.lower() == "n":
+                return [priv for priv in mist_session.privileges if not priv.get("msp_id")]
+            else:
+                tested_val = _test_choice(resp, i)
+                if tested_val >= 0:
+                    return _forge_privileges(mist_session, msp_accounts[tested_val]["msp_id"])
+                elif tested_val == -1:
+                    print(f"{resp} is not part of the possibilities.")
+                elif tested_val == -2:
+                    print("Only numbers are allowed.")
+
+
+def select_org(mist_session: mistapi.APISession, allow_many=False) -> list:
     """
     Function to list all the Mist Orgs allowed for the current user
     and ask to pick one or many. Return the Org ID(s) of the selected
     org(s)
 
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     :param bool allow_many - If user is allowed to select multiple orgs. Default is False
 
     RETURN
     -----------
     :return list - list of the selected Org ID(s)
     """
-    i=-1
-    org_ids = []
-    resp_ids=[]
-    data = mist_session.privileges
-    data = [d for d in data if d['name']]
-    data=sorted(data, key=lambda x: x["name"].lower())
-    print("\r\nAvailable organizations:")
-    for privilege in data:
-        if privilege["scope"] == "org" and not privilege["org_id"] in org_ids:
-            i+=1
-            org_ids.append(privilege["org_id"])
-            print(f"{i}) {privilege['name']} (id: {privilege['org_id']})")
-
-    orgs_with_sites = []
-    for privilege in data:
-        if privilege["scope"] == "site" and not privilege["org_id"] in org_ids:
-            index = _search_org(orgs_with_sites, privilege["org_id"])
-            if index is None:
-                i+=1
+    data = _select_msp(mist_session)
+    data = [d for d in data if d["name"]]
+    data = sorted(data, key=lambda x: x["name"].lower())
+    while True:
+        i = -1
+        org_ids = []
+        resp_ids = []
+        print("\r\nAvailable organizations:")
+        for privilege in data:
+            if privilege["scope"] == "org" and not privilege["org_id"] in org_ids:
+                i += 1
                 org_ids.append(privilege["org_id"])
                 print(f"{i}) {privilege['name']} (id: {privilege['org_id']})")
-                orgs_with_sites.append({
-                    "org_id": privilege["org_id"], 
-                    "name": privilege["name"], 
-                    "sites": [
+
+        orgs_with_sites = []
+        for privilege in data:
+            if privilege["scope"] == "site" and not privilege["org_id"] in org_ids:
+                index = _search_org(orgs_with_sites, privilege["org_id"])
+                if index is None:
+                    i += 1
+                    org_ids.append(privilege["org_id"])
+                    print(f"{i}) {privilege['name']} (id: {privilege['org_id']})")
+                    orgs_with_sites.append(
+                        {
+                            "org_id": privilege["org_id"],
+                            "name": privilege["name"],
+                            "sites": [
+                                {"site_id": privilege["site_id"], "name": privilege["name"]}
+                            ],
+                        }
+                    )
+                else:
+                    orgs_with_sites[index]["sites"].append(
                         {"site_id": privilege["site_id"], "name": privilege["name"]}
-                        ]
-                    })
-            else:
-                orgs_with_sites[index]["sites"].append({"site_id": privilege["site_id"], "name": privilege["name"]})
+                    )
 
-    if allow_many: resp = input(f"\r\nSelect an Org (0 to {i}, \"0,1\" for sites 0 and 1, \"a\" for all, or q to exit): ")
-    else: resp = input(f"\r\nSelect an Org (0 to {i}, or q to exit): ")
-    if resp == "q":
-        sys.exit(0)
-    elif resp.lower() == "a" and allow_many:
-        return org_ids
-    else:            
-        resp = resp.split(",")
-        if not allow_many and len(resp) > 1 :
-            print(f"Only one org is allowed, you selected {len(resp)}")
-            return select_org(mist_session, allow_many)
-        for num in resp:
-            tested_val = _test_choice(num, i)
-            if tested_val >= 0:
-                resp_ids.append(org_ids[tested_val])
-            if tested_val == -1:
-                print(f"{num} is not part of the possibilities.")
-                return select_org(mist_session, allow_many)
-            if tested_val == -2:
-                print("Only numbers are allowed.")
+        if allow_many:
+            resp = input(
+                f'\r\nSelect an Org (0 to {i}, "0,1" for sites 0 and 1, "a" for all, "b" for back or "q" to quit): '
+            )
+        else:
+            resp = input(f'\r\nSelect an Org (0 to {i}, "b" for back or "q" to quit): ')
+        if resp.lower() == "b":
+            return select_org(mist_session)
+        elif resp.lower() == "q":
+            sys.exit(0)
+        elif resp.lower() == "a" and allow_many:
+            return org_ids
+        else:
+            selection_validated = True
+            resp = resp.split(",")
+            if not allow_many and len(resp) > 1:
+                print(f"Only one org is allowed, you selected {len(resp)}")
                 return select_org(mist_session, allow_many)
-        return resp_ids
-
-
-def select_site(mist_session:mistapi.APISession, org_id=None, allow_many=False) -> list:
+            for num in resp:
+                tested_val = _test_choice(num, i)
+                if tested_val >= 0:
+                    resp_ids.append(org_ids[tested_val])
+                if tested_val == -1:
+                    print(f"{num} is not part of the possibilities.")
+                    selection_validated = False
+                if tested_val == -2:
+                    print("Only numbers are allowed.")
+                    selection_validated = False
+            if selection_validated:
+                return resp_ids
+
+
+def select_site(
+    mist_session: mistapi.APISession, org_id=None, allow_many=False
+) -> list:
     """
     Function to list all the Sites from a Mist Org and ask user to pick one
     or many. Return the Site ID(s) of the selected site(s)
 
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     :param str org_id - Org ID to request
     :param bool allow_many - If user is allowed to select multiple orgs. Default is False
 
     RETURN
     -----------
     :return list - list of the selected Site ID(s)
     """
-    i=-1
-    site_ids=[]
+    i = -1
+    site_ids = []
     site_choices = []
-    resp_ids=[]
+    resp_ids = []
     org_access = False
 
     if org_id is None:
         org_id = select_org(mist_session)[0]
 
     for privilege in mist_session.privileges:
         if privilege["scope"] == "org" and privilege["org_id"] == org_id:
             org_access = True
         if privilege["scope"] == "site" and privilege["org_id"] == org_id:
             site_choices.append({"id": privilege["site_id"], "name": privilege["name"]})
 
     if site_choices == [] or org_access == True:
         site_choices = mistapi.api.v1.orgs.sites.listOrgSites(mist_session, org_id).data
 
-
-    
-    site_choices=sorted(site_choices, key=lambda x: x["name"].lower())
+    site_choices = sorted(site_choices, key=lambda x: x["name"].lower())
     print("\r\nAvailable sites:")
-    for site in site_choices:        
-        i+=1
+    for site in site_choices:
+        i += 1
         site_ids.append(site["id"])
         print(f"{i}) {site['name']} (id: {site['id']})")
-    if allow_many: resp = input(f"\r\nSelect a Site (0 to {i}, \"0,1\" for sites 0 and 1, \"a\" for all, or q to exit): ")
-    else: resp = input(f"\r\nSelect a Site (0 to {i}, or q to exit): ")
+    if allow_many:
+        resp = input(
+            f'\r\nSelect a Site (0 to {i}, "0,1" for sites 0 and 1, "a" for all, or q to exit): '
+        )
+    else:
+        resp = input(f"\r\nSelect a Site (0 to {i}, or q to exit): ")
 
     if resp.lower() == "q":
         sys.exit(0)
     elif resp.lower() == "a" and allow_many:
         return site_ids
-    else:                
+    else:
         resp = resp.split(",")
-        if not allow_many and len(resp) > 1 :
+        if not allow_many and len(resp) > 1:
             print(f"Only one site is allowed, you selected {len(resp)}")
             return select_site(mist_session, org_id, allow_many)
         for num in resp:
             tested_val = _test_choice(num, i)
             if tested_val >= 0:
                 resp_ids.append(site_choices[tested_val]["id"])
             if tested_val == -1:
@@ -171,73 +257,77 @@
                 print("Only numbers are allowed.")
                 return select_site(mist_session, org_id, allow_many)
         return resp_ids
 
 
 ###########################################
 #### DATA PROCESSING / DISPLAY
-def extract_field(json_data, field):   
+def extract_field(json_data, field):
     split_field = field.split(".")
     cur_field = split_field[0]
     next_fields = ".".join(split_field[1:])
     if cur_field in json_data:
         if len(split_field) > 1:
             return extract_field(json_data[cur_field], next_fields)
         else:
-            return json_data[cur_field] 
+            return json_data[cur_field]
     else:
         return "N/A"
 
-def save_to_csv(csv_file:str, data:list, fields:list, csv_separator:str=",") -> None:
-    """ 
+
+def save_to_csv(
+    csv_file: str, data: list, fields: list, csv_separator: str = ","
+) -> None:
+    """
     Write a list of lists in a CSV file
 
     PARAMS
     -----------
     :param str csv_file - path to the CSV file where to save the data
     :param list data - list containing the lists to save
     :param list fields - list of the columns headers
     :param str csv_separator - character to use to separate the cells. Default is ","
     """
     print("saving to file...")
     with open(csv_file, "w") as f:
         for column in fields:
             f.write(f"{column},")
-        f.write('\r\n')
+        f.write("\r\n")
         for row in data:
             for field in row:
                 if field is None:
                     f.write("")
                 else:
                     f.write(field)
                 f.write(csv_separator)
-            f.write('\r\n')
+            f.write("\r\n")
+
 
-def _json_to_array(json_data:object, fields:list) -> list:
+def _json_to_array(json_data: object, fields: list) -> list:
     data = []
     for field in fields:
         data.append(json_data.get(field, ""))
     return data
 
 
-def display_list_of_json_as_table(json_list:list, fields:list) -> None:
+def display_list_of_json_as_table(json_list: list, fields: list) -> None:
     table = []
     for data in json_list:
         table.append(_json_to_array(data, fields))
     print(tabulate(table, headers=fields))
 
 
 def pretty_print(response, fields=None):
     if "result" in response:
         data = response["result"]
     else:
         data = response
     print("")
-    if type(data) is list:  
+    if type(data) is list:
         if fields is None:
-            fields = "keys" 
+            fields = "keys"
         print(tabulate(data, headers=fields))
     elif type(data) == dict:
-        print(json.dumps(data, sort_keys=True, indent=4, separators=(',', ': ')))
+        print(json.dumps(data, sort_keys=True, indent=4, separators=(",", ": ")))
     else:
-        print(data)    
-    print("")
+        print(data)
+    print("")
```

### Comparing `mistapi-0.37.8/src/mistapi.egg-info/PKG-INFO` & `mistapi-0.40.0/src/mistapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.37.8
+Version: 0.40.0
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.37.8/src/mistapi.egg-info/SOURCES.txt` & `mistapi-0.40.0/src/mistapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 src/mistapi/api/v1/const/client_events.py
 src/mistapi/api/v1/const/countries.py
 src/mistapi/api/v1/const/default_gateway_config.py
 src/mistapi/api/v1/const/device_events.py
 src/mistapi/api/v1/const/device_models.py
 src/mistapi/api/v1/const/insight_metrics.py
 src/mistapi/api/v1/const/languages.py
+src/mistapi/api/v1/const/license_types.py
 src/mistapi/api/v1/const/mxedge_events.py
 src/mistapi/api/v1/const/mxedge_models.py
 src/mistapi/api/v1/const/traffic_types.py
 src/mistapi/api/v1/installer/__init__.py
 src/mistapi/api/v1/installer/orgs/__init__.py
 src/mistapi/api/v1/installer/orgs/alarmtemplates.py
 src/mistapi/api/v1/installer/orgs/deviceprofiles.py
@@ -68,14 +69,15 @@
 src/mistapi/api/v1/msps/msps.py
 src/mistapi/api/v1/msps/orggroups.py
 src/mistapi/api/v1/msps/orgs.py
 src/mistapi/api/v1/msps/search.py
 src/mistapi/api/v1/msps/ssoroles.py
 src/mistapi/api/v1/msps/ssos.py
 src/mistapi/api/v1/msps/stats.py
+src/mistapi/api/v1/msps/suggestion.py
 src/mistapi/api/v1/msps/tickets.py
 src/mistapi/api/v1/orgs/__init__.py
 src/mistapi/api/v1/orgs/admins.py
 src/mistapi/api/v1/orgs/alarms.py
 src/mistapi/api/v1/orgs/alarmtemplates.py
 src/mistapi/api/v1/orgs/apitokens.py
 src/mistapi/api/v1/orgs/aptemplates.py
@@ -148,14 +150,20 @@
 src/mistapi/api/v1/self/apitokens.py
 src/mistapi/api/v1/self/logs.py
 src/mistapi/api/v1/self/oauth.py
 src/mistapi/api/v1/self/self.py
 src/mistapi/api/v1/self/subscriptions.py
 src/mistapi/api/v1/self/two_factor.py
 src/mistapi/api/v1/self/update.py
+src/mistapi/api/v1/site/__init__.py
+src/mistapi/api/v1/site/deviceprofiles.py
+src/mistapi/api/v1/site/networks.py
+src/mistapi/api/v1/site/servicepolicies.py
+src/mistapi/api/v1/site/services.py
+src/mistapi/api/v1/site/vpns.py
 src/mistapi/api/v1/sites/__init__.py
 src/mistapi/api/v1/sites/alarms.py
 src/mistapi/api/v1/sites/anomaly.py
 src/mistapi/api/v1/sites/apps.py
 src/mistapi/api/v1/sites/assetfilters.py
 src/mistapi/api/v1/sites/assets.py
 src/mistapi/api/v1/sites/beacons.py
```

