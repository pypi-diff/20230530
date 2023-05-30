# Comparing `tmp/msticpy-2.4.0.tar.gz` & `tmp/msticpy-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msticpy-2.4.0.tar", last modified: Fri Apr  7 02:24:49 2023, max compression
+gzip compressed data, was "msticpy-2.5.0.tar", last modified: Tue May 30 16:53:25 2023, max compression
```

## Comparing `msticpy-2.4.0.tar` & `msticpy-2.5.0.tar`

### file list

```diff
@@ -1,405 +1,418 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.049796 msticpy-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-07 02:24:33.000000 msticpy-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-07 02:24:33.000000 msticpy-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)   487752 2023-04-07 02:24:33.000000 msticpy-2.4.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-04-07 02:24:49.049796 msticpy-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15960 2023-04-07 02:24:33.000000 msticpy-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.953795 msticpy-2.4.0/msticpy/
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.957795 msticpy-2.4.0/msticpy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.957795 msticpy-2.4.0/msticpy/analysis/anomalous_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/anomalous_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/anomalous_sequence/anomalous.py
--rw-r--r--   0 runner    (1001) docker     (123)    29469 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/anomalous_sequence/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/anomalous_sequence/sessionize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.957795 msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/cmds_only.py
--rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py
--rw-r--r--   0 runner    (1001) docker     (123)    21586 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/cluster_auditd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/code_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/eventcluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/observationlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/outliers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/syslog_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/analysis/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.961795 msticpy-2.4.0/msticpy/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/auth/azure_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    15662 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/auth/azure_auth_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/auth/cloud_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/auth/cred_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/auth/keyring_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/auth/keyvault_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/auth/keyvault_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/auth/msal_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/auth/secret_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.965795 msticpy-2.4.0/msticpy/common/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/azure_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/check_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/pkg_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/provider_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/timespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.965795 msticpy-2.4.0/msticpy/common/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/utility/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/utility/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/utility/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/utility/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/common/wsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.969795 msticpy-2.4.0/msticpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/ce_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/ce_azure_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/ce_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/ce_data_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/ce_keyvault.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/ce_other_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/ce_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/ce_simple_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/ce_ti_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/ce_user_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/comp_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/compound_ctrls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/file_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/mp_config_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/mp_config_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/config/mp_config_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.973795 msticpy-2.4.0/msticpy/context/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.977795 msticpy-2.4.0/msticpy/context/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34998 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/azure/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/azure/sentinel_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/azure/sentinel_bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/azure/sentinel_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/azure/sentinel_dynamic_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    25652 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/azure/sentinel_dynamic_summary_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/azure/sentinel_incidents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/azure/sentinel_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/azure/sentinel_ti.py
--rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/azure/sentinel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/azure/sentinel_watchlists.py
--rw-r--r--   0 runner    (1001) docker     (123)    12290 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/azure/sentinel_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/contextlookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.977795 msticpy-2.4.0/msticpy/context/contextproviders/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/contextproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/contextproviders/context_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/contextproviders/http_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/contextproviders/servicenow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/domain_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/geoip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/http_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    25638 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/ip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26852 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/lookup_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/preprocess_observable.py
--rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tilookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.981795 msticpy-2.4.0/msticpy/context/tiproviders/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/alienvault_otx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/azure_sent_byoti.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/greynoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/ibm_xforce.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/intsights.py
--rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/kql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/mblookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/open_page_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/pulsedive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/result_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/riskiq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/ti_http_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/ti_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/tor_exit_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/tiproviders/virustotal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.985795 msticpy-2.4.0/msticpy/context/vtlookupv3/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/vtlookupv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/vtlookupv3/vtfile_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/vtlookupv3/vtlookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32429 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/context/vtlookupv3/vtlookupv3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.985795 msticpy-2.4.0/msticpy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.989796 msticpy-2.4.0/msticpy/data/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/azure/azure_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/azure/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/azure_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/azure_sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.989796 msticpy-2.4.0/msticpy/data/core/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29510 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/core/data_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/core/data_query_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/core/param_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/core/query_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/core/query_defns.py
--rw-r--r--   0 runner    (1001) docker     (123)    19982 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/core/query_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/core/query_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/data_obfus.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/data_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.993795 msticpy-2.4.0/msticpy/data/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15319 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/cybereason_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/driver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/elastic_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    23215 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/kql_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/kusto_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/local_data_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/mdatp_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    29077 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/mordor_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/odata_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/resource_graph_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/security_graph_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/splunk_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22155 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/drivers/sumologic_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.945795 msticpy-2.4.0/msticpy/data/queries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.997795 msticpy-2.4.0/msticpy/data/queries/cybereason/
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/cybereason/cybereason_connections.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/cybereason/cybereason_hosts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/cybereason/cybereason_processes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.997795 msticpy-2.4.0/msticpy/data/queries/localdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/localdata/local_data.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.997795 msticpy-2.4.0/msticpy/data/queries/m365d/
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/m365d/kql_mdatp_alerts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/m365d/kql_mdatp_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    29648 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/m365d/kql_mdatp_hunting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/m365d/kql_mdatp_network.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/m365d/kql_mdatp_process.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/m365d/kql_mdatp_user.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.001796 msticpy-2.4.0/msticpy/data/queries/mde/
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mde/kql_mdatp_alerts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mde/kql_mdatp_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mde/kql_mdatp_hunting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mde/kql_mdatp_network.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mde/kql_mdatp_process.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mde/kql_mdatp_user.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.001796 msticpy-2.4.0/msticpy/data/queries/msgraph/
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/msgraph/graph_alerts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.005796 msticpy-2.4.0/msticpy/data/queries/mssentinel/
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_alert.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_azure.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_net.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_o365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.005796 msticpy-2.4.0/msticpy/data/queries/resourcegraph/
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/resourcegraph/sentinel_resources.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.009796 msticpy-2.4.0/msticpy/data/queries/splunk/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/splunk/splunk_alert_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/splunk/splunk_authentication_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/splunk/splunk_queries.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.009796 msticpy-2.4.0/msticpy/data/queries/sumologic/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/queries/sumologic/sumologic_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/query_container.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/query_defns.py
--rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/sql_to_kql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.009796 msticpy-2.4.0/msticpy/data/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/storage/azure_blob_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.009796 msticpy-2.4.0/msticpy/data/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/uploaders/loganalytics_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/uploaders/splunk_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/data/uploaders/uploader_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.009796 msticpy-2.4.0/msticpy/datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.021796 msticpy-2.4.0/msticpy/datamodel/entities/
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/azure_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/cloud_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/cloud_logon_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/entity_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/entity_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/file_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/geo_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/graph_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/host_logon_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/iot_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/mail_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/mail_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/malware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/network_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/registry_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/registry_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/submission_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/threat_intelligence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/unknown_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/entities/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/pivot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.021796 msticpy-2.4.0/msticpy/datamodel/soc/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/soc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/soc/incident.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/datamodel/soc/sentinel_alert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.021796 msticpy-2.4.0/msticpy/init/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15537 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/azure_ml_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    19979 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/azure_synapse_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/mp_pandas_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)    32679 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/nbinit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/nbmagics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/pivot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.025796 msticpy-2.4.0/msticpy/init/pivot_core/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/pivot_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/pivot_core/pivot_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/pivot_core/pivot_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/pivot_core/pivot_magic_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/pivot_core/pivot_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/pivot_core/pivot_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/pivot_core/pivot_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/pivot_core/pivot_register_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.025796 msticpy-2.4.0/msticpy/init/pivot_init/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/pivot_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/pivot_init/pivot_data_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/pivot_init/pivot_ti_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/pivot_init/vt_pivot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/init/user_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/msticpyconfig.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.029796 msticpy-2.4.0/msticpy/nbtools/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/data_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/entityschema.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/morph_charts.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/nbdisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/nbwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/observationlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/process_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/security_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/security_alert_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    18315 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/security_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/security_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/ti_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/timeline_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/timeline_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbtools/wsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.033796 msticpy-2.4.0/msticpy/nbwidgets/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbwidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbwidgets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbwidgets/get_environment_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbwidgets/get_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbwidgets/lookback.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbwidgets/option_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbwidgets/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbwidgets/query_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbwidgets/select_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbwidgets/select_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/nbwidgets/select_subset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.033796 msticpy-2.4.0/msticpy/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   104245 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/resources/WinSecurityEvent.json
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/resources/cmd_line_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/resources/mp_pivot_reg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/resources/mpconfig_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/resources/obfuscation_cols.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.037796 msticpy-2.4.0/msticpy/sectools/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/auditdextract.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/base64unpack.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/domain_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/eventcluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/geoip.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/iocextract.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/ip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/proc_tree_build_mde.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/proc_tree_build_winlx.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/proc_tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/proc_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/proc_tree_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/sectools_magics.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/syslog_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/tilookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.037796 msticpy-2.4.0/msticpy/sectools/tiproviders/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/tiproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/tiproviders/ti_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/vtlookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.041796 msticpy-2.4.0/msticpy/sectools/vtlookupv3/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/vtlookupv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/vtlookupv3/vtfile_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/vtlookupv3/vtlookupv3.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/sectools/vtlookupv3/vtobject_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.041796 msticpy-2.4.0/msticpy/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/transform/auditdextract.py
--rw-r--r--   0 runner    (1001) docker     (123)    30712 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/transform/base64unpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/transform/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    26354 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/transform/iocextract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/transform/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/transform/proc_tree_build_mde.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/transform/proc_tree_build_winlx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/transform/proc_tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/transform/proc_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/transform/process_tree_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:49.049796 msticpy-2.4.0/msticpy/vis/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/code_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/data_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/entity_graph_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/figure_dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)    33234 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/matrix_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/mordor_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/morph_charts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/mp_pandas_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/nbdisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/network_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/process_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/query_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/ti_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/timeline_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/timeline_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/timeline_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/timeline_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-07 02:24:34.000000 msticpy-2.4.0/msticpy/vis/vtobject_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:24:48.953795 msticpy-2.4.0/msticpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-04-07 02:24:48.000000 msticpy-2.4.0/msticpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-04-07 02:24:48.000000 msticpy-2.4.0/msticpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 02:24:48.000000 msticpy-2.4.0/msticpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 02:24:48.000000 msticpy-2.4.0/msticpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-07 02:24:48.000000 msticpy-2.4.0/msticpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 02:24:48.000000 msticpy-2.4.0/msticpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-07 02:24:34.000000 msticpy-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-07 02:24:34.000000 msticpy-2.4.0/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-07 02:24:34.000000 msticpy-2.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-07 02:24:34.000000 msticpy-2.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-07 02:24:49.049796 msticpy-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-07 02:24:34.000000 msticpy-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.529810 msticpy-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-30 16:53:10.000000 msticpy-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 16:53:10.000000 msticpy-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)   487752 2023-05-30 16:53:10.000000 msticpy-2.5.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-05-30 16:53:25.529810 msticpy-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15960 2023-05-30 16:53:10.000000 msticpy-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.441810 msticpy-2.5.0/msticpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.445810 msticpy-2.5.0/msticpy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.445810 msticpy-2.5.0/msticpy/analysis/anomalous_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/anomalous_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/anomalous_sequence/anomalous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29469 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/anomalous_sequence/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/anomalous_sequence/sessionize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.449810 msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/cmds_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21586 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/cluster_auditd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/code_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/eventcluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/observationlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/outliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/polling_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/syslog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/analysis/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.449810 msticpy-2.5.0/msticpy/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/auth/azure_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/auth/azure_auth_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/auth/cloud_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/auth/cred_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/auth/keyring_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/auth/keyvault_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/auth/keyvault_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/auth/msal_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/auth/secret_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.453810 msticpy-2.5.0/msticpy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/azure_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/check_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19073 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/pkg_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/provider_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/proxy_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/timespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.453810 msticpy-2.5.0/msticpy/common/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/utility/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/utility/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/utility/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/utility/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/common/wsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.457810 msticpy-2.5.0/msticpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/ce_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/ce_azure_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/ce_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/ce_data_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/ce_keyvault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/ce_msticpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/ce_other_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/ce_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/ce_simple_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/ce_ti_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/ce_user_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/comp_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/compound_ctrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/file_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/mp_config_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/mp_config_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/config/mp_config_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.457810 msticpy-2.5.0/msticpy/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.461810 msticpy-2.5.0/msticpy/context/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34998 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/azure/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/azure/sentinel_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/azure/sentinel_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/azure/sentinel_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/azure/sentinel_dynamic_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25652 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/azure/sentinel_dynamic_summary_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/azure/sentinel_incidents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/azure/sentinel_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/azure/sentinel_ti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/azure/sentinel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/azure/sentinel_watchlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12290 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/azure/sentinel_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/contextlookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.461810 msticpy-2.5.0/msticpy/context/contextproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/contextproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/contextproviders/context_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/contextproviders/http_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/contextproviders/servicenow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11264 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/domain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/geoip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25638 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/ip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/lookup_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/preprocess_observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tilookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.465810 msticpy-2.5.0/msticpy/context/tiproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/alienvault_otx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/azure_sent_byoti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/greynoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/ibm_xforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/intsights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/kql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/mblookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/open_page_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/pulsedive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/result_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/riskiq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/ti_http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/ti_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/tor_exit_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/tiproviders/virustotal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.465810 msticpy-2.5.0/msticpy/context/vtlookupv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/vtlookupv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/vtlookupv3/vtfile_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/vtlookupv3/vtlookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32429 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/context/vtlookupv3/vtlookupv3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.469810 msticpy-2.5.0/msticpy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.469810 msticpy-2.5.0/msticpy/data/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/azure/azure_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/azure/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/azure_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/azure_sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.473810 msticpy-2.5.0/msticpy/data/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20161 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/core/data_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/core/data_query_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/core/param_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/core/query_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/core/query_defns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/core/query_provider_connections_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/core/query_provider_utils_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/core/query_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/core/query_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/core/query_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/data_obfus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/data_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.477810 msticpy-2.5.0/msticpy/data/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33479 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/azure_kusto_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23280 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/azure_monitor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/cybereason_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/driver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/elastic_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23295 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/kql_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/kusto_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/local_data_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/local_osquery_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/mdatp_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29511 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/mordor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/odata_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/resource_graph_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/security_graph_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/sentinel_query_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/splunk_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/drivers/sumologic_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.437810 msticpy-2.5.0/msticpy/data/queries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.477810 msticpy-2.5.0/msticpy/data/queries/cybereason/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/cybereason/cybereason_connections.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/cybereason/cybereason_hosts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/cybereason/cybereason_processes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.477810 msticpy-2.5.0/msticpy/data/queries/localdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/localdata/local_data.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.477810 msticpy-2.5.0/msticpy/data/queries/m365d/
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/m365d/kql_mdatp_alerts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/m365d/kql_mdatp_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    29648 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/m365d/kql_mdatp_hunting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/m365d/kql_mdatp_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/m365d/kql_mdatp_process.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/m365d/kql_mdatp_user.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.477810 msticpy-2.5.0/msticpy/data/queries/mde/
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mde/kql_mdatp_alerts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mde/kql_mdatp_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mde/kql_mdatp_hunting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mde/kql_mdatp_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mde/kql_mdatp_process.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mde/kql_mdatp_user.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.477810 msticpy-2.5.0/msticpy/data/queries/msgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/msgraph/graph_alerts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.481810 msticpy-2.5.0/msticpy/data/queries/mssentinel/
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_alert.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_azure.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_net.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_o365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.481810 msticpy-2.5.0/msticpy/data/queries/resourcegraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/resourcegraph/sentinel_resources.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.485810 msticpy-2.5.0/msticpy/data/queries/splunk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/splunk/splunk_alert_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/splunk/splunk_authentication_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/splunk/splunk_queries.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.485810 msticpy-2.5.0/msticpy/data/queries/sumologic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/queries/sumologic/sumologic_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/query_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/query_defns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/sql_to_kql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.485810 msticpy-2.5.0/msticpy/data/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/storage/azure_blob_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.485810 msticpy-2.5.0/msticpy/data/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/uploaders/loganalytics_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/uploaders/splunk_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/data/uploaders/uploader_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.485810 msticpy-2.5.0/msticpy/datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.493810 msticpy-2.5.0/msticpy/datamodel/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/azure_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/cloud_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/cloud_logon_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/entity_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/entity_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/file_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/graph_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/host_logon_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/iot_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/mail_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/mail_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/malware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/network_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/registry_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/registry_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/submission_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/threat_intelligence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/unknown_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/entities/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/pivot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.493810 msticpy-2.5.0/msticpy/datamodel/soc/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/soc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/soc/incident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/datamodel/soc/sentinel_alert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.497810 msticpy-2.5.0/msticpy/init/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15574 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/azure_ml_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19979 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/azure_synapse_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/mp_pandas_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/mp_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32396 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/nbinit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/nbmagics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/pivot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.501810 msticpy-2.5.0/msticpy/init/pivot_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/pivot_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/pivot_core/pivot_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/pivot_core/pivot_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/pivot_core/pivot_magic_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/pivot_core/pivot_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/pivot_core/pivot_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/pivot_core/pivot_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/pivot_core/pivot_register_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.501810 msticpy-2.5.0/msticpy/init/pivot_init/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/pivot_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/pivot_init/pivot_data_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/pivot_init/pivot_ti_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/pivot_init/vt_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/init/user_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/msticpyconfig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.509810 msticpy-2.5.0/msticpy/nbtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/entityschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/morph_charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/nbdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/nbwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/observationlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/process_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/security_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/security_alert_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18315 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/security_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/security_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/ti_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/timeline_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/timeline_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbtools/wsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.509810 msticpy-2.5.0/msticpy/nbwidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbwidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbwidgets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbwidgets/get_environment_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbwidgets/get_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbwidgets/lookback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbwidgets/option_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbwidgets/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbwidgets/query_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbwidgets/select_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbwidgets/select_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/nbwidgets/select_subset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.513810 msticpy-2.5.0/msticpy/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   104245 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/resources/WinSecurityEvent.json
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/resources/cmd_line_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/resources/mp_pivot_reg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/resources/mpconfig_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/resources/obfuscation_cols.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.517810 msticpy-2.5.0/msticpy/sectools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/auditdextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/base64unpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/domain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/eventcluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/geoip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/iocextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/ip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/proc_tree_build_mde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/proc_tree_build_winlx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/proc_tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/proc_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/proc_tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/sectools_magics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/syslog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/tilookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.517810 msticpy-2.5.0/msticpy/sectools/tiproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/tiproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/tiproviders/ti_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/vtlookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.521810 msticpy-2.5.0/msticpy/sectools/vtlookupv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/vtlookupv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/vtlookupv3/vtfile_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/vtlookupv3/vtlookupv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/sectools/vtlookupv3/vtobject_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.521810 msticpy-2.5.0/msticpy/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/transform/auditdextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30712 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/transform/base64unpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/transform/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26354 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/transform/iocextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/transform/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/transform/proc_tree_build_mde.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/transform/proc_tree_build_winlx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/transform/proc_tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/transform/proc_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/transform/process_tree_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.529810 msticpy-2.5.0/msticpy/vis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/code_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/data_viewer_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/entity_graph_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/figure_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33234 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/matrix_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/mordor_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/morph_charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/mp_pandas_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/nbdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/network_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/process_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/query_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/ti_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/timeline_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/timeline_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/timeline_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/timeline_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-30 16:53:10.000000 msticpy-2.5.0/msticpy/vis/vtobject_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:53:25.445810 msticpy-2.5.0/msticpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-05-30 16:53:25.000000 msticpy-2.5.0/msticpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-05-30 16:53:25.000000 msticpy-2.5.0/msticpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:53:25.000000 msticpy-2.5.0/msticpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:53:25.000000 msticpy-2.5.0/msticpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-30 16:53:25.000000 msticpy-2.5.0/msticpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 16:53:25.000000 msticpy-2.5.0/msticpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 16:53:10.000000 msticpy-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-30 16:53:10.000000 msticpy-2.5.0/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-30 16:53:10.000000 msticpy-2.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-30 16:53:10.000000 msticpy-2.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-30 16:53:25.529810 msticpy-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-30 16:53:10.000000 msticpy-2.5.0/setup.py
```

### Comparing `msticpy-2.4.0/LICENSE` & `msticpy-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/NOTICE.txt` & `msticpy-2.5.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/PKG-INFO` & `msticpy-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msticpy
-Version: 2.4.0
+Version: 2.5.0
 Summary: MSTIC Security Tools
 Home-page: https://github.com/microsoft/msticpy
 Author: Ian Hellen
 Author-email: ianhelle@microsoft.com
 Maintainer: Pete Bryan
 Maintainer-email: peter.bryan@microsoft.com
 License: MIT License
@@ -32,18 +32,20 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: vt3
 Provides-Extra: splunk
 Provides-Extra: sumologic
 Provides-Extra: kql
 Provides-Extra: _azure_core
+Provides-Extra: azure_query
 Provides-Extra: keyvault
 Provides-Extra: ml
 Provides-Extra: sql2kql
 Provides-Extra: riskiq
+Provides-Extra: panel
 Provides-Extra: all
 Provides-Extra: azure
 Provides-Extra: test
 Provides-Extra: azsentinel
 Provides-Extra: azuresentinel
 Provides-Extra: sentinel
 License-File: LICENSE
```

### Comparing `msticpy-2.4.0/README.md` & `msticpy-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/__init__.py` & `msticpy-2.5.0/msticpy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -112,29 +112,30 @@
 
 In the Azure ML and Azure Synapse environments, some additional
 initialization and checks are performed.
 
 """
 import importlib
 import os
-from typing import Any
+from typing import Any, Iterable, Union
 
 from . import nbwidgets
 
 # flake8: noqa: F403
 from ._version import VERSION
 from .common import pkg_config as settings
 from .common.check_version import check_version
 from .common.utility import search_name as search
 from .init.logging import set_logging_level, setup_logging
 
 __version__ = VERSION
 __author__ = "Ian Hellen, Pete Bryan, Ashwin Patil"
 
 refresh_config = settings.refresh_config
+get_config = settings.get_config
 setup_logging()
 
 if not os.environ.get("KQLMAGIC_EXTRAS_REQUIRES"):
     os.environ["KQLMAGIC_EXTRAS_REQUIRES"] = "jupyter-basic"
 
 _STATIC_ATTRIBS = list(locals().keys())
 
@@ -183,7 +184,30 @@
         return getattr(module, attrib)
     raise AttributeError(f"msticpy has no attribute {attrib}")
 
 
 def __dir__():
     """Return attribute list."""
     return sorted(set(_STATIC_ATTRIBS + list(_DEFAULT_IMPORTS)))
+
+
+def load_plugins(plugin_paths: Union[str, Iterable[str]]):
+    """
+    Load plugins from specified paths or configuration.
+
+    Parameters
+    ----------
+    plugin_paths : Union[str, Iterable[str]]
+        A path or collection of paths from which to
+        load plugins. If not supplied, msticpyconfig is checked for
+        a PluginFolders key and list of paths are read from there.
+
+    Notes
+    -----
+    No attempt to load plugins is made if both parameter and
+    configuration are empty.
+
+    """
+    # pylint: disable=import-outside-toplevel
+    from .init.mp_plugins import read_plugins
+
+    read_plugins(plugin_paths)
```

### Comparing `msticpy-2.4.0/msticpy/analysis/__init__.py` & `msticpy-2.5.0/msticpy/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/anomalous_sequence/anomalous.py` & `msticpy-2.5.0/msticpy/analysis/anomalous_sequence/anomalous.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/anomalous_sequence/model.py` & `msticpy-2.5.0/msticpy/analysis/anomalous_sequence/model.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/anomalous_sequence/sessionize.py` & `msticpy-2.5.0/msticpy/analysis/anomalous_sequence/sessionize.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/cmds_only.py` & `msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/cmds_only.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py` & `msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py` & `msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/data_structures.py` & `msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py` & `msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/anomalous_sequence/utils/probabilities.py` & `msticpy-2.5.0/msticpy/analysis/anomalous_sequence/utils/probabilities.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/cluster_auditd.py` & `msticpy-2.5.0/msticpy/analysis/cluster_auditd.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/code_cleanup.py` & `msticpy-2.5.0/msticpy/analysis/code_cleanup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/eventcluster.py` & `msticpy-2.5.0/msticpy/analysis/eventcluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/observationlist.py` & `msticpy-2.5.0/msticpy/analysis/observationlist.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/outliers.py` & `msticpy-2.5.0/msticpy/analysis/outliers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/syslog_utils.py` & `msticpy-2.5.0/msticpy/analysis/syslog_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/analysis/timeseries.py` & `msticpy-2.5.0/msticpy/analysis/timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,20 +264,20 @@
     data_column = kwargs.get("data_column")
 
     if not isinstance(data, pd.DataFrame):
         raise MsticpyException("input data should be a pandas dataframe")
 
     if time_column:
         data = data.set_index(time_column)
-    if data_column:
-        data = data[[data_column]]
+    data_column = data_column or data.columns[0]
+    data = data[[data_column]]
 
     # STL method does Season-Trend decomposition using LOESS.
     # Accepts timeseries dataframe
-    stl = STL(data, seasonal=seasonal, period=period)
+    stl = STL(data[data_column].values, seasonal=seasonal, period=period)
     # Fitting the data - Estimate season, trend and residuals components.
     res = stl.fit()
     result = data.copy()
     # Create dataframe columns from decomposition results
     result["residual"] = res.resid
     result["trend"] = res.trend
     result["seasonal"] = res.seasonal
```

### Comparing `msticpy-2.4.0/msticpy/auth/__init__.py` & `msticpy-2.5.0/msticpy/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/auth/azure_auth.py` & `msticpy-2.5.0/msticpy/auth/azure_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,7 +171,13 @@
     legacy_creds = CredentialWrapper(
         creds, resource_id=AzureCloudConfig(cloud).token_uri
     )
     if not creds:
         raise CloudError("Could not obtain credentials.")
 
     return AzCredentials(legacy_creds, creds)
+
+
+def get_default_resource_name(resource_uri: str) -> str:
+    """Get a default resource name for a resource URI."""
+    separator = "" if resource_uri.strip().endswith("/") else "/"
+    return f"{resource_uri}{separator}.default"
```

### Comparing `msticpy-2.4.0/msticpy/auth/azure_auth_core.py` & `msticpy-2.5.0/msticpy/auth/azure_auth_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
             ):
                 raise ValueError("AADSTS70043: The refresh token has expired")
 
         return AzureCliStatus.CLI_OK, "Azure CLI credentials available."
     except ImportError:
         # Azure CLI not installed
         return AzureCliStatus.CLI_NOT_INSTALLED, None
-    except Exception as ex:  # pylint: disable=broad-except, broad-exception-caught
+    except Exception as ex:  # pylint: disable=broad-except
         if "AADSTS70043: The refresh token has expired" in str(ex):
             message = (
                 "Azure CLI was detected but the token has expired. "
                 "For Azure CLI single sign-on, please sign in using '!az login'."
             )
             return AzureCliStatus.CLI_TOKEN_EXPIRED, message
         if "Please run 'az login' to setup account" in str(ex):
```

### Comparing `msticpy-2.4.0/msticpy/auth/cloud_mappings.py` & `msticpy-2.5.0/msticpy/auth/cloud_mappings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/auth/cred_wrapper.py` & `msticpy-2.5.0/msticpy/auth/cred_wrapper.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/auth/keyring_client.py` & `msticpy-2.5.0/msticpy/auth/keyring_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Settings provider for secrets."""
-import random
 from typing import Any, Set
 
 import keyring
-from keyring.errors import KeyringError, KeyringLocked, NoKeyringError
+from keyring.errors import KeyringError, KeyringLocked
 
 from .._version import VERSION
 from ..common.utility import export
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
@@ -113,20 +112,8 @@
 
         Returns
         -------
         bool
             True if Keyring has a usable backend, False if not.
 
         """
-        char_list = list("abcdefghijklm1234567890")
-        random.shuffle(char_list)
-        test_value = "".join(char_list)
-        try:
-            keyring.set_password("test", test_value, test_value)
-            # If no exception clear the test key
-            try:
-                keyring.delete_password("test", test_value)
-            except keyring.errors.PasswordDeleteError:
-                pass
-            return True
-        except NoKeyringError:
-            return False
+        return keyring.get_keyring() != keyring.backends.fail.Keyring
```

### Comparing `msticpy-2.4.0/msticpy/auth/keyvault_client.py` & `msticpy-2.5.0/msticpy/auth/keyvault_client.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/auth/keyvault_settings.py` & `msticpy-2.5.0/msticpy/auth/keyvault_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/auth/msal_auth.py` & `msticpy-2.5.0/msticpy/auth/msal_auth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/auth/secret_settings.py` & `msticpy-2.5.0/msticpy/auth/secret_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/common/__init__.py` & `msticpy-2.5.0/msticpy/common/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/common/azure_auth.py` & `msticpy-2.5.0/msticpy/common/azure_auth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/common/check_version.py` & `msticpy-2.5.0/msticpy/common/check_version.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/common/data_types.py` & `msticpy-2.5.0/msticpy/common/data_types.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/common/data_utils.py` & `msticpy-2.5.0/msticpy/common/data_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/common/exceptions.py` & `msticpy-2.5.0/msticpy/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/common/pkg_config.py` & `msticpy-2.5.0/msticpy/common/pkg_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,17 +281,15 @@
         if not pkg_root:
             raise MsticpyUserConfigError(
                 f"Unable to locate the package default {_CONFIG_FILE}",
                 "msticpy package may be corrupted.",
                 title=f"Package {_CONFIG_FILE} missing.",
             ) from mod_err
         conf_file = next(iter(pkg_root.glob(f"**/{_CONFIG_FILE}")))
-    if conf_file:
-        return _read_config_file(conf_file)
-    return {}
+    return _read_config_file(conf_file) if conf_file else {}
 
 
 def _get_custom_config():
     config_path = os.environ.get(_CONFIG_ENV_VAR, None)
     if config_path and Path(config_path).is_file():
         _CURRENT_CONF_FILE(str(Path(config_path).resolve()))
         return _read_config_file(current_config_path())
@@ -341,20 +339,27 @@
     for src, target in translate.items():
         src_value = _get_config(src, mp_config)
         _set_config(target, mp_config, src_value, True)
         _del_config(src, mp_config)
     return mp_config
 
 
+#############################
+# Specialized settings
+
+
 def get_http_timeout(
     **kwargs,
 ) -> httpx.Timeout:
     """Return timeout from settings or overridden in `kwargs`."""
+    config_timeout = get_config(
+        "msticpy.http_timeout", get_config("http_timeout", None)
+    )
     timeout_params = kwargs.get(
-        "timeout", kwargs.get("def_timeout", get_config("http_timeout", None))  # type: ignore
+        "timeout", kwargs.get("def_timeout", config_timeout)  # type: ignore
     )  # type: ignore
     if isinstance(timeout_params, dict):
         timeout_params = {
             name: _valid_timeout(val) for name, val in timeout_params.items()
         }
         return httpx.Timeout(**timeout_params)
     if isinstance(timeout_params, httpx.Timeout):
@@ -373,14 +378,17 @@
 def _valid_timeout(timeout_val) -> Union[float, None]:
     """Return float in valid range or None."""
     if isinstance(timeout_val, numbers.Real) and float(timeout_val) >= 0.0:
         return float(timeout_val)
     return None
 
 
+# End specialized settings
+############################
+
 # read initial config when first imported.
 refresh_config()
 
 
 def validate_config(mp_config: Dict[str, Any] = None, config_file: str = None):
     """
     Validate msticpy config settings.
@@ -392,15 +400,15 @@
         check the currently loaded settings.
     config_file : str
         path to config file to check, by default None
 
     """
     if config_file:
         mp_config = _read_config_file(config_file)
-    if not (mp_config or config_file):
+    if not mp_config and not config_file:
         mp_config = _settings
 
     if not isinstance(mp_config, dict):
         raise TypeError("Unknown format for configuration settings.")
 
     mp_errors, mp_warn = _validate_azure_sentinel(mp_config=mp_config)
 
@@ -422,17 +430,15 @@
         )
         if conf_section == _DP_KEY and mp_config.get(conf_section) is None:
             continue
         mp_errors.extend(prov_errors)
         mp_warn.extend(prov_warn)
 
     _print_validation_report(mp_errors, mp_warn)
-    if mp_errors or mp_warn:
-        return mp_errors, mp_warn
-    return [], []
+    return (mp_errors, mp_warn) if mp_errors or mp_warn else ([], [])
 
 
 def _print_validation_report(mp_errors, mp_warn):
     if mp_errors:
         _print_validation_item(
             "\nThe following configuration errors were found:", mp_errors
         )
```

### Comparing `msticpy-2.4.0/msticpy/common/provider_settings.py` & `msticpy-2.5.0/msticpy/common/provider_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     settings = {}
     for provider, item_settings in section_settings.items():
         prov_args = item_settings.get("Args")
         prov_settings = ProviderSettings(  # type: ignore[call-arg]
             name=provider,
             description=item_settings.get("Description"),
             args=_get_setting_args(
-                config_section=config_section,
+                config_path=config_section,
                 provider_name=provider,
                 prov_args=prov_args,
             ),
             primary=item_settings.get("Primary", False),
             provider=item_settings.get("Provider", provider),
         )
         settings[provider] = prov_settings
@@ -226,116 +226,138 @@
             auth_methods=auth_methods,
             credential=credential,
             **kwargs,
         )
         _SET_SECRETS_CLIENT(secrets_client=secrets_client)
 
 
+def get_protected_setting(config_path, setting_name) -> Any:
+    """Return a potentially protected setting value."""
+    config_settings = get_config(config_path)
+    prov_args = _get_protected_settings(config_path, config_settings)
+    return prov_args.get(setting_name)
+
+
 def _get_setting_args(
-    config_section: str, provider_name: str, prov_args: Optional[Dict[str, Any]]
+    config_path: str, provider_name: str, prov_args: Optional[Dict[str, Any]]
 ) -> ProviderArgs:
     """Extract the provider args from the settings."""
     if not prov_args:
         return ProviderArgs()
     name_map = {
         "workspaceid": "workspace_id",
         "tenantid": "tenant_id",
         "subscriptionid": "subscription_id",
     }
-    return _get_settings(
-        config_section=config_section,
-        provider_name=provider_name,
-        conf_group=prov_args,
+    return _get_protected_settings(
+        setting_path=f"{config_path}.{provider_name}.Args",
+        section_settings=prov_args,
         name_map=name_map,
     )
 
 
-def _get_settings(
-    config_section: str,
-    provider_name: str,
-    conf_group: Optional[Dict[str, Any]],
+def _get_protected_settings(
+    setting_path: str,
+    section_settings: Optional[Dict[str, Any]],
     name_map: Optional[Dict[str, str]] = None,
 ) -> ProviderArgs:
     """
     Lookup configuration values config, environment or KeyVault.
 
     Parameters
     ----------
-    config_section : str
-        Configuration section
-    provider_name: str
-        The name of the provider section
-    conf_group : Optional[Dict[str, Any]]
-        The configuration dictionary
+    setting_path : str
+        Dotted path to the setting
+    section_settings : Optional[Dict[str, Any]]
+        The configuration settings for this path.
     name_map : Optional[Dict[str, str]], optional
         Optional mapping to re-write setting names,
         by default None
 
     Returns
     -------
     ProviderArgs
         Dictionary of resolved settings
 
-    Raises
-    ------
-    NotImplementedError
-        Keyvault storage is not yet implemented
-
     """
-    if not conf_group:
+    if not section_settings:
         return ProviderArgs()
-    setting_dict: ProviderArgs = ProviderArgs(conf_group.copy())
+    setting_dict: ProviderArgs = ProviderArgs(section_settings.copy())
 
-    for arg_name, arg_value in conf_group.items():
+    for arg_name, arg_value in section_settings.items():
         target_name = arg_name
         if name_map:
             target_name = name_map.get(target_name.casefold(), target_name)
 
-        if isinstance(arg_value, str):
-            setting_dict[target_name] = arg_value
-        elif isinstance(arg_value, dict):
-            try:
-                setting_dict[target_name] = _fetch_setting(
-                    config_section, provider_name, arg_name, arg_value
-                )  # type: ignore
-            except NotImplementedError:
-                warnings.warn(
-                    f"Setting type for setting {arg_value} not yet implemented. "
-                )
+        try:
+            setting_dict[target_name] = _fetch_secret_setting(
+                f"{setting_path}.{arg_name}", arg_value
+            )
+        except NotImplementedError:
+            warnings.warn(f"Setting type for setting {arg_value} not yet implemented. ")
     return setting_dict
 
 
-def _fetch_setting(
-    config_section: str,
-    provider_name: str,
-    arg_name: str,
-    config_setting: Dict[str, Any],
+def _fetch_secret_setting(
+    setting_path: str,
+    config_setting: Union[str, Dict[str, Any]],
 ) -> Union[Optional[str], Callable[[], Any]]:
-    """Return required value for indirect settings (e.g. getting env var)."""
+    """
+    Return required value for potential secret setting.
+
+    Parameters
+    ----------
+    setting_path : str
+        Dotted path to the setting
+    config_setting : Union[str, Dict[str, Any]]
+        Setting value (str or Dict)
+
+    Returns
+    -------
+    Union[Optional[str], Callable[[], Any]]
+        Either a string or accessor function.
+
+    Raises
+    ------
+    MsticpyImportExtraError
+        _description_
+    NotImplementedError
+        _description_
+
+    """
+    if isinstance(config_setting, str):
+        return config_setting
+    if not isinstance(config_setting, dict):
+        return NotImplementedError(
+            "Configuration setting format not recognized.",
+            f"'{setting_path}' should be a string or dictionary",
+            "with either 'EnvironmentVar' or 'KeyVault' entry.",
+        )
     if "EnvironmentVar" in config_setting:
         env_value = os.environ.get(config_setting["EnvironmentVar"])
         if not env_value:
             warnings.warn(
                 f"Environment variable {config_setting['EnvironmentVar']}"
-                + f" (provider {provider_name})"
+                + f" ({setting_path})"
                 + " was not set"
             )
         return env_value
     if "KeyVault" in config_setting:
         if not _SECRETS_ENABLED:
             raise MsticpyImportExtraError(
                 "Cannot use this feature without Key Vault support installed",
-                title="Error importing Loading Key Vault and/or keyring libaries",
+                title="Error importing Loading Key Vault and/or keyring libraries.",
                 extra="keyvault",
             )
         if not _SECRETS_CLIENT:
             warnings.warn(
                 "Cannot use a KeyVault configuration setting without"
                 + "a KeyVault configuration section in msticpyconfig.yaml"
-                + f" (provider {provider_name})"
+                + f" ({setting_path})"
             )
             return None
-        config_path = (config_section, provider_name, "Args", arg_name)
-        return _SECRETS_CLIENT.get_secret_accessor(  # type:ignore
-            ".".join(config_path)
-        )
-    return None
+        return _SECRETS_CLIENT.get_secret_accessor(setting_path)
+    raise NotImplementedError(
+        "Configuration setting format not recognized.",
+        f"'{setting_path}' should be a string or dictionary",
+        "with either 'EnvironmentVar' or 'KeyVault' entry.",
+    )
```

### Comparing `msticpy-2.4.0/msticpy/common/timespan.py` & `msticpy-2.5.0/msticpy/common/timespan.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/common/utility/__init__.py` & `msticpy-2.5.0/msticpy/common/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/common/utility/format.py` & `msticpy-2.5.0/msticpy/common/utility/format.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/common/utility/ipython.py` & `msticpy-2.5.0/msticpy/common/utility/ipython.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/common/utility/package.py` & `msticpy-2.5.0/msticpy/common/utility/package.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Packaging utility functions."""
+import importlib
 import os
 import re
 import subprocess  # nosec
 import sys
 import warnings
 from pathlib import Path
 from platform import python_version
@@ -303,7 +304,37 @@
         Turn unit testing flag on or off, by default True
 
     """
     if on:
         os.environ[_U_TEST_ENV] = "True"
     else:
         os.environ.pop(_U_TEST_ENV, None)
+
+
+def init_getattr(module_name: str, dynamic_imports: Dict[str, str], attrib: str):
+    """Import and return dynamic attribute."""
+    if attrib in dynamic_imports:
+        module = importlib.import_module(dynamic_imports[attrib])
+        return getattr(module, attrib)
+    raise AttributeError(f"{module_name} has no attribute {attrib}")
+
+
+def init_dir(static_attribs: List[str], dynamic_imports: Dict[str, str]):
+    """Return list of available attributes."""
+    return sorted(set(static_attribs + list(dynamic_imports)))
+
+
+def lazy_import(module: str, attrib: str, call: bool = False):
+    """Import attribute from module on demand."""
+    attribute = None
+
+    def import_item(*args, **kwargs):
+        """Return the attribute, importing module if needed."""
+        nonlocal attribute
+        if attribute is None:
+            imp_module = importlib.import_module(module)
+            attribute = getattr(imp_module, attrib)
+        return (
+            attribute(*args, **kwargs) if (call and callable(attribute)) else attribute
+        )
+
+    return import_item
```

### Comparing `msticpy-2.4.0/msticpy/common/utility/types.py` & `msticpy-2.5.0/msticpy/common/utility/types.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/common/wsconfig.py` & `msticpy-2.5.0/msticpy/common/wsconfig.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Module for Log Analytics-related configuration."""
-
-
 import contextlib
 import json
 import os
+import re
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 import ipywidgets as widgets
 from IPython.display import display
 
 from .._version import VERSION
@@ -91,54 +90,80 @@
 
     CONF_WS_ID_KEY = "workspace_id"
     CONF_TENANT_ID_KEY = "tenant_id"
     CONF_SUB_ID_KEY = "subscription_id"
     CONF_RES_GROUP_KEY = "resource_group"
     CONF_WS_NAME_KEY = "workspace_name"
 
+    _SETTINGS_TO_CONFIG_NAME_MAP = {
+        PKG_CONF_TENANT_KEY: CONF_TENANT_ID_KEY,
+        PKG_CONF_WS_KEY: CONF_WS_ID_KEY,
+        PKG_CONF_SUB_KEY: CONF_SUB_ID_KEY,
+        PKG_CONF_RES_GROUP_KEY: CONF_RES_GROUP_KEY,
+        PKG_CONF_NAME_KEY: CONF_WS_NAME_KEY,
+    }
+    _CONFIG_TO_SETTINGS_NAME_MAP = {
+        val: key for key, val in _SETTINGS_TO_CONFIG_NAME_MAP.items()
+    }
+
     def __init__(
         self,
         workspace: Optional[str] = None,
         config_file: Optional[str] = None,
         interactive: bool = True,
+        config: Optional[Dict[str, str]] = None,
     ):
         """
         Load current Azure Notebooks configuration for Log Analytics.
 
         Parameters
         ----------
         config_file : Optional[str], optional
             path to a configuration file,
             If not specified, the defaults is to use a configured msticpyconfig.yaml
             If this isn't configured, it will search for (first) a config.json
             and (second) a msticpyconfig.yaml in (first) the current directory
             and (second) the parent directory and subfolders.
-        workspace : str, Optional[str]
+        workspace : Optional[str]
             Workspace name (where multiple workspaces are configured),
             by default the Default workspace will be used.
         interactive : bool, optional
             If this is False, initializing the class will not raise an
             exception if no configuration is found. By default, True.
+        config : Optional[Dict[str, str]],
+            Workspace configuration as dictionary.
 
         """
         self._config: Dict[str, str] = {}
         self._interactive = interactive
         self._config_file = config_file
         self.workspace_key = workspace or "Default"
         # If config file specified, use that
-        if config_file:
+        if config:
+            self._config.update(config)
+        elif config_file:
             self._config.update(self._read_config_values(config_file))
         else:
             self._determine_config_source(workspace)
 
+    def __getattr__(self, attribute: str):
+        """Return attribute from configuration."""
+        with contextlib.suppress(KeyError):
+            return self[attribute]
+        raise AttributeError(
+            f"{self.__class__.__name__} has no attribute '{attribute}'"
+        )
+
     def __getitem__(self, key: str):
         """Allow property get using dictionary key syntax."""
-        if key in self._config:
-            return self._config[key]
-        raise KeyError
+        if key in self._SETTINGS_TO_CONFIG_NAME_MAP:
+            return self._config.get(self._SETTINGS_TO_CONFIG_NAME_MAP[key])
+        if key in self._CONFIG_TO_SETTINGS_NAME_MAP:
+            return self._config.get(key)
+        raise KeyError(f"{self.__class__.__name__} has no attribute '{key}'")
 
     def __setitem__(self, key: str, value: Any):
         """Allow property set using dictionary key syntax."""
         self._config[key] = value
 
     def __contains__(self, key: str):
         """Allow property in test."""
@@ -204,25 +229,42 @@
             self.PKG_CONF_SUB_KEY: self._config.get(self.CONF_SUB_ID_KEY),
             self.PKG_CONF_WS_KEY: self._config.get(self.CONF_WS_ID_KEY),
             self.PKG_CONF_TENANT_KEY: self._config.get(self.CONF_TENANT_ID_KEY),
             self.PKG_CONF_RES_GROUP_KEY: self._config.get(self.CONF_RES_GROUP_KEY),
         }
 
     @classmethod
-    def from_settings(cls, settings: Dict[str, Any]):
+    def from_settings(cls, settings: Dict[str, Any]) -> "WorkspaceConfig":
         """Create a WorkstationConfig from MSTICPY Workspace settings."""
-        ws_config = cls(workspace="**DUMMY_WORKSPACE**")  # type: ignore
-        ws_config._config = {  # type: ignore
-            cls.CONF_WS_NAME_KEY: settings.get(cls.PKG_CONF_NAME_KEY),  # type: ignore
-            cls.CONF_SUB_ID_KEY: settings.get(cls.PKG_CONF_SUB_KEY),  # type: ignore
-            cls.CONF_WS_ID_KEY: settings.get(cls.PKG_CONF_WS_KEY),  # type: ignore
-            cls.CONF_TENANT_ID_KEY: settings.get(cls.PKG_CONF_TENANT_KEY),  # type: ignore
-            cls.CONF_RES_GROUP_KEY: settings.get(cls.PKG_CONF_RES_GROUP_KEY),  # type: ignore
-        }
-        return ws_config
+        return cls(
+            config={  # type: ignore
+                cls.CONF_WS_NAME_KEY: settings.get(cls.PKG_CONF_NAME_KEY),  # type: ignore
+                cls.CONF_SUB_ID_KEY: settings.get(cls.PKG_CONF_SUB_KEY),  # type: ignore
+                cls.CONF_WS_ID_KEY: settings.get(cls.PKG_CONF_WS_KEY),  # type: ignore
+                cls.CONF_TENANT_ID_KEY: settings.get(cls.PKG_CONF_TENANT_KEY),  # type: ignore
+                cls.CONF_RES_GROUP_KEY: settings.get(cls.PKG_CONF_RES_GROUP_KEY),  # type: ignore
+            }
+        )
+
+    @classmethod
+    def from_connection_string(cls, connection_str: str) -> "WorkspaceConfig":
+        """Create a WorkstationConfig from a connection string."""
+        tenant_regex = r".*tenant\(\s?['\"](?P<tenant_id>[\w]+)['\"].*"
+        workspace_regex = r".*workspace\(\s?['\"](?P<workspace_id>[\w]+)['\"].*"
+        tenant_id = workspace_id = None
+        if match := re.match(tenant_regex, connection_str):
+            tenant_id = match.groupdict()["tenant_id"]
+        if match := re.match(workspace_regex, connection_str):
+            workspace_id = match.groupdict()["workspace_id"]
+        return cls(
+            config={
+                cls.CONF_WS_ID_KEY: workspace_id,  # type: ignore[dict-item]
+                cls.CONF_TENANT_ID_KEY: tenant_id,  # type: ignore[dict-item]
+            }
+        )
 
     @staticmethod
     def _read_config_values(file_path: str) -> Dict[str, str]:
         """Read configuration file."""
         if not file_path:
             return {}
         with contextlib.suppress(json.JSONDecodeError):
@@ -287,33 +329,25 @@
         )
 
     def _determine_config_source(self, workspace):
         # First, try default MSTICPy config
         self._read_pkg_config_values(workspace_name=workspace)
         if self.config_loaded:
             return
-        # Next, search for a config.json in the current director
+        # Next, search for a config.json in the current directory
         if Path("./config.json").exists():
             self._config_file = "./config.json"
         else:
             self._config_file = self._search_for_file("**/config.json")
         if self._config_file:
             self._config.update(self._read_config_values(self._config_file))
             return
 
         # Finally, search for a msticpyconfig.yaml
-        if (
-            os.environ.get("MSTICPYCONFIG")
-            and Path(os.environ.get("MSTICPYCONFIG")).exists()
-        ):
-            self._config_file = os.environ.get("MSTICPYCONFIG")
-        elif Path("./msticpyconfig.yaml").exists():
-            self._config_file = "./msticpyconfig.yaml"
-        else:
-            self._config_file = self._search_for_file("**/msticpyconfig.yaml")
+        self._config_file = self._search_for_file("**/msticpyconfig.yaml")
         if self._config_file:
             os.environ["MSTICPYCONFIG"] = self._config_file
             refresh_config()
             self._read_pkg_config_values(workspace_name=workspace)
             return
         # Finally, throw an exception (unless non-interactive)
         if self._interactive:
@@ -323,52 +357,47 @@
                 MsticpyUserConfigError(
                     *_NO_CONFIG_ERR,
                     title="Workspace configuration missing.",
                     **{f"nb_{idx}_uri": res for idx, res in enumerate(_RESOURCES)},
                 )
             )
 
-    def _read_pkg_config_values(self, workspace_name: str = None):
-        as_settings = get_config("AzureSentinel", {})
-        if not as_settings:
-            return {}
-        ws_settings = as_settings.get("Workspaces")  # type: ignore
+    def _read_pkg_config_values(self, workspace_name: Optional[str] = None):
+        """Try to find a usable config from the MSTICPy config file."""
+        ws_settings = get_config("AzureSentinel", {}).get("Workspaces")  # type: ignore
         if not ws_settings:
-            return {}
-        if workspace_name and workspace_name in ws_settings:
-            selected_workspace = ws_settings[workspace_name]
+            return
+        selected_workspace: Dict[str, str] = {}
+        if workspace_name:
+            selected_workspace = self._lookup_ws_name_and_id(
+                workspace_name, ws_settings
+            )
         elif "Default" in ws_settings:
             selected_workspace = ws_settings["Default"]
         elif len(ws_settings) == 1:
             selected_workspace = next(iter(ws_settings.values()))
-        else:
-            return {}
-        if (
-            selected_workspace
-            and self.PKG_CONF_WS_KEY in selected_workspace
-            and self.PKG_CONF_TENANT_KEY in selected_workspace
-        ):
-            self._config[self.CONF_WS_ID_KEY] = selected_workspace.get(
-                self.PKG_CONF_WS_KEY
-            )
-            self._config[self.CONF_TENANT_ID_KEY] = selected_workspace.get(
-                self.PKG_CONF_TENANT_KEY
-            )
-        if self.PKG_CONF_SUB_KEY in selected_workspace:
-            self._config[self.CONF_SUB_ID_KEY] = selected_workspace.get(
-                self.PKG_CONF_SUB_KEY
-            )
-        if self.PKG_CONF_RES_GROUP_KEY in selected_workspace:
-            self._config[self.CONF_RES_GROUP_KEY] = selected_workspace.get(
-                self.PKG_CONF_RES_GROUP_KEY
-            )
-        if self.PKG_CONF_NAME_KEY in selected_workspace:
-            self._config[self.CONF_WS_NAME_KEY] = selected_workspace.get(
-                self.PKG_CONF_NAME_KEY
-            )
+
+        if selected_workspace:
+            self._config = {}
+            for name, value in selected_workspace.items():
+                tgt_name = self._SETTINGS_TO_CONFIG_NAME_MAP.get(name)
+                if tgt_name and value:
+                    self._config[tgt_name] = value
+
+    def _lookup_ws_name_and_id(self, ws_name: str, ws_configs: dict):
+        for name, ws_config in ws_configs.items():
+            if ws_name.casefold() == name.casefold():
+                return ws_config
+            if ws_config.get(self.PKG_CONF_WS_KEY, "").casefold() == ws_name.casefold():
+                return ws_config
+            if (
+                ws_config.get(self.PKG_CONF_NAME_KEY, "").casefold()
+                == ws_name.casefold()
+            ):
+                return ws_config
         return {}
 
     def _search_for_file(self, pattern: str) -> Optional[str]:
         config_file = None
         for start_path in (".", ".."):
             searched_configs = list(Path(start_path).glob(pattern))
             for found_file in searched_configs:
```

### Comparing `msticpy-2.4.0/msticpy/config/ce_azure.py` & `msticpy-2.5.0/msticpy/config/ce_azure.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/config/ce_azure_sentinel.py` & `msticpy-2.5.0/msticpy/config/ce_azure_sentinel.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,31 @@
 # --------------------------------------------------------------------------
 """Module docstring."""
 from datetime import datetime
 
 import ipywidgets as widgets
 
 from .._version import VERSION
-from ..context.azure.sentinel_core import MicrosoftSentinel
+from ..common.utility.package import lazy_import
+
+# from ..context.azure.sentinel_core import MicrosoftSentinel
 from .ce_common import (
     ITEM_LIST_LAYOUT,
     get_or_create_mpc_section,
     get_wgt_ctrl,
     print_debug,
 )
 from .comp_edit import CEItemsBase, CompEditDisplayMixin
 from .mp_config_control import MpConfigControls
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
+ms_sentinel = lazy_import("msticpy.context.azure.sentinel_core", "MicrosoftSentinel")
+
 
 # pylint: disable=too-many-ancestors
 class CEAzureSentinel(CEItemsBase):
     """Microsoft Sentinel Workspaces editor component."""
 
     _DESCRIPTION = "Microsoft Sentinel workspace settings"
     _COMP_PATH = "AzureSentinel.Workspaces"
@@ -212,15 +216,15 @@
     def _imp_ws_from_url(self, btn):
         """Import workspace settings from a portal URL."""
         del btn
         url = self.txt_imp_url.value
         if not url:
             self.set_status("Please paste portal URL into ")
             return
-        self._update_settings(MicrosoftSentinel.get_workspace_details_from_url(url))
+        self._update_settings(ms_sentinel().get_workspace_details_from_url(url))
 
     def _update_settings(self, ws_settings):
         """Update current controls with workspace settings."""
         if not ws_settings:
             self.set_status("Could not resolve workspace from URL")
             return
         ws_name = next(iter(ws_settings))
@@ -242,19 +246,19 @@
         if not (workspace_id or workspace_name):
             self.set_status(
                 "Need at least WorkspaceId or WorkspaceName to lookup settings."
             )
             return
         if workspace_id:
             self._update_settings(
-                MicrosoftSentinel.get_workspace_settings(workspace_id=workspace_id)
+                ms_sentinel().get_workspace_settings(workspace_id=workspace_id)
             )
         else:
             self._update_settings(
-                MicrosoftSentinel.get_workspace_settings_by_name(
+                ms_sentinel().get_workspace_settings_by_name(
                     workspace_name=workspace_name,
                     subscription_id=subscription_id,
                     resource_group=resource_group,
                 )
             )
 
     def _select_labels(self):
```

### Comparing `msticpy-2.4.0/msticpy/config/ce_common.py` & `msticpy-2.5.0/msticpy/config/ce_common.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/config/ce_data_providers.py` & `msticpy-2.5.0/msticpy/config/ce_data_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/config/ce_keyvault.py` & `msticpy-2.5.0/msticpy/config/ce_keyvault.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/config/ce_other_providers.py` & `msticpy-2.5.0/msticpy/config/ce_other_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/config/ce_provider_base.py` & `msticpy-2.5.0/msticpy/config/ce_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/config/ce_simple_settings.py` & `msticpy-2.5.0/msticpy/config/ce_simple_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/config/ce_ti_providers.py` & `msticpy-2.5.0/msticpy/config/ce_ti_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/config/ce_user_defaults.py` & `msticpy-2.5.0/msticpy/config/ce_user_defaults.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/config/comp_edit.py` & `msticpy-2.5.0/msticpy/config/comp_edit.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/config/compound_ctrls.py` & `msticpy-2.5.0/msticpy/config/compound_ctrls.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/config/file_browser.py` & `msticpy-2.5.0/msticpy/config/file_browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """File Browser class."""
+
+import contextlib
 from pathlib import Path
-from typing import Any, Callable, List, Optional, Tuple
+from typing import Any, Callable, List, Optional, Tuple, Union
 
 import ipywidgets as widgets
 
 from .._version import VERSION
 from .comp_edit import CompEditDisplayMixin
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 
+StrOrPath = Union[str, Path]
+
+
 # pylint: disable=too-many-instance-attributes
 class FileBrowser(CompEditDisplayMixin):
     """File system browser control."""
 
     PARENT = ".."
 
-    def __init__(self, path: str = ".", select_cb: Callable[[str], Any] = None):
+    def __init__(self, path: StrOrPath = ".", select_cb: Callable[[str], Any] = None):
         """
         Initialize the class for path and with optional callback.
 
         Parameters
         ----------
         path : str, optional
             Path to open at, by default "."
@@ -134,46 +139,50 @@
     def _return_file(self, btn):
         """Execute callback on selected file if one is defined."""
         del btn
         if self.action:
             self.action(self.file)
 
     @staticmethod
-    def read_folder(folder: str) -> Tuple[List[str], List[str]]:
+    def read_folder(folder: StrOrPath) -> Tuple[List[StrOrPath], List[StrOrPath]]:
         """
         Return folder contents.
 
         Parameters
         ----------
         folder : str
             Folder path.
 
         Returns
         -------
-        Tuple[List[str], List[str]]
+        Tuple[List[StrOrPath], List[StrOrPath]]
             List of folders and files in the folder.
 
         """
         contents = list(Path(folder).glob("*"))
-        files = [file.parts[-1] for file in contents if file.is_file()]
-        folders = [fld.parts[-1] for fld in contents if fld.is_dir()]
-        return folders, files
+        files = []
+        folders = []
+        for file in contents:
+            with contextlib.suppress(PermissionError, IOError):
+                if file.is_file():
+                    files.append(file)
+                elif file.is_dir():
+                    folders.append(file)
+        return folders, files  # type: ignore[return-value]
 
-    def get_folder_list(self, folders: List[str]) -> List[str]:
+    def get_folder_list(self, folders: List[StrOrPath]) -> List[StrOrPath]:
         """Return sorted list of folders with '..' inserted if not root."""
         if self.current_folder != Path(self.current_folder.parts[0]):
             return [self.PARENT, *(sorted(folders))]
         return sorted(folders)
 
     def _search(self, btn):
         """Handle event for search button."""
         del btn
         if self.txt_search.value:
             found_files: Optional[List[Path]] = None
             while found_files is None:
-                try:
+                with contextlib.suppress(FileNotFoundError):
                     found_files = list(self.current_folder.rglob(self.txt_search.value))
-                except FileNotFoundError:
-                    pass
             self.select_search.options = [
                 str(file) for file in found_files if file.exists()
             ]
```

### Comparing `msticpy-2.4.0/msticpy/config/mp_config_control.py` & `msticpy-2.5.0/msticpy/config/mp_config_control.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/config/mp_config_edit.py` & `msticpy-2.5.0/msticpy/config/mp_config_edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,38 +10,41 @@
 from IPython.display import display
 
 from .._version import VERSION
 from .ce_azure import CEAzure
 from .ce_azure_sentinel import CEAzureSentinel
 from .ce_data_providers import CEDataProviders
 from .ce_keyvault import CEKeyVault
+from .ce_msticpy import CEMsticpy
 from .ce_other_providers import CEOtherProviders
 from .ce_ti_providers import CETIProviders
-from .ce_user_defaults import CEAutoLoadComps, CEAutoLoadQProvs
+
+# from .ce_user_defaults import CEAutoLoadComps, CEAutoLoadQProvs
 from .comp_edit import CETabControlDef, CompEditDisplayMixin, CompEditTabs
 from .mp_config_control import MpConfigControls, get_mpconfig_definitions
 from .mp_config_file import MpConfigFile
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 
 # pylint: disable=too-many-instance-attributes
 class MpConfigEdit(CompEditDisplayMixin):
     """Msticpy Configuration helper class."""
 
     _TAB_DEFINITIONS = {
+        "MSTICPy": CEMsticpy,
         "MicrosoftSentinel": CEAzureSentinel,
         "TI Providers": CETIProviders,
         "Data Providers": CEDataProviders,
         "GeoIP Providers": CEOtherProviders,
         "Key Vault": CEKeyVault,
         "Azure": CEAzure,
-        "Autoload QueryProvs": CEAutoLoadQProvs,
-        "Autoload Components": CEAutoLoadComps,
+        # "Autoload QueryProvs": CEAutoLoadQProvs,
+        # "Autoload Components": CEAutoLoadComps,
     }
 
     def __init__(
         self,
         settings: Optional[Union[Dict[str, Any], MpConfigFile, str]] = None,
         conf_filepath: str = None,
     ):
```

### Comparing `msticpy-2.4.0/msticpy/config/mp_config_file.py` & `msticpy-2.5.0/msticpy/config/mp_config_file.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/__init__.py` & `msticpy-2.5.0/msticpy/context/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/azure/azure_data.py` & `msticpy-2.5.0/msticpy/context/azure/azure_data.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/azure/sentinel_analytics.py` & `msticpy-2.5.0/msticpy/context/azure/sentinel_analytics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/azure/sentinel_bookmarks.py` & `msticpy-2.5.0/msticpy/context/azure/sentinel_bookmarks.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/azure/sentinel_core.py` & `msticpy-2.5.0/msticpy/context/azure/sentinel_core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/azure/sentinel_dynamic_summary.py` & `msticpy-2.5.0/msticpy/context/azure/sentinel_dynamic_summary.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/azure/sentinel_dynamic_summary_types.py` & `msticpy-2.5.0/msticpy/context/azure/sentinel_dynamic_summary_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 # pylint: disable=too-many-instance-attributes
 @dataclasses.dataclass
 class DynamicSummaryItem:
     """
     DynamicSummaryItem class.
 
-    Attributes
+    Parameters
     ----------
     summary_item_id: Optional[str]
         The ID of the item
     relation_name: Optional[str] = None
         The name of the summary item relation
     relation_id: Optional[str] = None
         The ID of the summary item relation
```

### Comparing `msticpy-2.4.0/msticpy/context/azure/sentinel_incidents.py` & `msticpy-2.5.0/msticpy/context/azure/sentinel_incidents.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/azure/sentinel_search.py` & `msticpy-2.5.0/msticpy/context/azure/sentinel_search.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/azure/sentinel_ti.py` & `msticpy-2.5.0/msticpy/context/azure/sentinel_ti.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/azure/sentinel_utils.py` & `msticpy-2.5.0/msticpy/context/azure/sentinel_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
 
         Returns
         -------
         str
             The formatted resource ID.
 
         """
+        print("_build_sent_res_id", sub_id, res_grp, ws_name)
         if not sub_id or not res_grp or not ws_name:
             config = self._check_config(
                 workspace_name=ws_name,
                 items=["subscription_id", "resource_group", "workspace_name"],
             )
             sub_id = config["subscription_id"]
             res_grp = config["resource_group"]
```

### Comparing `msticpy-2.4.0/msticpy/context/azure/sentinel_watchlists.py` & `msticpy-2.5.0/msticpy/context/azure/sentinel_watchlists.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/azure/sentinel_workspaces.py` & `msticpy-2.5.0/msticpy/context/azure/sentinel_workspaces.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/contextlookup.py` & `msticpy-2.5.0/msticpy/context/contextlookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 Input can be a single Observable observable or a pandas DataFrame containing
 multiple observables. Processing may require a an API key and
 processing performance may be limited to a specific number of
 requests per minute for the account type that you have.
 
 """
-from typing import Iterable, List, Mapping, Optional, Union
+from typing import Dict, Iterable, List, Mapping, Optional, Union
 
 import pandas as pd
 
 from .._version import VERSION
 from ..common.utility import export
 
 # used in dynamic instantiation of providers
 from .contextproviders import CONTEXT_PROVIDERS
 from .lookup import Lookup
-from .provider_base import _make_sync
+from .provider_base import Provider, _make_sync
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 
 @export
 class ContextLookup(Lookup):
@@ -41,14 +41,15 @@
         "https://msticpy.readthedocs.io/en/latest/data_acquisition/"
         "ContextProviders.html#configuration-file"
     )
 
     PACKAGE = "contextproviders"
 
     PROVIDERS = CONTEXT_PROVIDERS
+    CUSTOM_PROVIDERS: Dict[str, Provider] = {}
 
     # pylint: disable=too-many-arguments
     def lookup_observable(
         self,
         observable: str,
         observable_type: Optional[str] = None,
         query_type: Optional[str] = None,
```

### Comparing `msticpy-2.4.0/msticpy/context/contextproviders/context_provider_base.py` & `msticpy-2.5.0/msticpy/context/contextproviders/context_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/contextproviders/http_context_provider.py` & `msticpy-2.5.0/msticpy/context/contextproviders/http_context_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/contextproviders/servicenow.py` & `msticpy-2.5.0/msticpy/context/contextproviders/servicenow.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,23 +35,23 @@
 
 
 # pylint: disable=too-few-public-methods
 @attr.s
 class _ServiceNowParams(APILookupParams):
     # override LookupParams to set common defaults
     def __attrs_post_init__(self):
-        self.auth_str = ["{API_ID}", "{API_KEY}"]
+        self.auth_str = ["{ApiID}", "{AuthKey}"]
         self.auth_type = "HTTPBasic"
 
 
 @export
 class ServiceNow(HttpContextProvider):
     """ServiceNow Lookup."""
 
-    _BASE_URL = "https://{INSTANCE}.service-now.com/api/now/table"
+    _BASE_URL = "https://{Instance}.service-now.com/api/now/table"
 
     _SERVICE_NOW_PARAMS = {
         "sysparm_display_value": True,
         "sysparm_exclude_reference_link": True,
         "sysparm_limit": 10,
     }
 
@@ -85,15 +85,15 @@
         "user": _ServiceNowParams(
             path="/sys_user",
             params={**_SERVICE_NOW_PARAMS, "sysparm_query": "nameLIKE{observable}"},
             headers=_DEF_HEADERS,
         ),
     }
 
-    _REQUIRED_PARAMS = ["API_ID", "API_KEY", "INSTANCE"]
+    _REQUIRED_PARAMS = ["ApiID", "AuthKey", "Instance"]
 
     def parse_results(self, response: Dict[str, Any]) -> Tuple[bool, Any]:
         """
         Return the details of the response.
 
         Parameters
         ----------
```

### Comparing `msticpy-2.4.0/msticpy/context/domain_utils.py` & `msticpy-2.5.0/msticpy/context/domain_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from IPython import display
 from ipywidgets import IntProgress
 from urllib3.exceptions import LocationParseError
 from urllib3.util import parse_url
 
 from .._version import VERSION
 from ..common.exceptions import MsticpyUserConfigError
-from ..common.pkg_config import get_config, get_http_timeout
+from ..common.settings import get_config, get_http_timeout
 from ..common.utility import export, mp_ua_header
 
 __version__ = VERSION
 __author__ = "Pete Bryan"
 
 
 @export
```

### Comparing `msticpy-2.4.0/msticpy/context/geoip.py` & `msticpy-2.5.0/msticpy/context/geoip.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/http_provider.py` & `msticpy-2.5.0/msticpy/context/http_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     .. code:: python
 
         _QUERIES = {
         # Community API
         "ipv4": APILookupParams(
             path="/v3/community/{observable}",
-            headers={"key": "{API_KEY}"},
+            headers={"key": "{AuthKey}"},
         ),
         # Enterprise API Quick Lookup
         "ipv4-quick": APILookupParams(
             ...
 
 
     Define list of required __init__ params
@@ -87,15 +87,15 @@
 
         _REQUIRED_PARAMS: List[str] = []
 
     For example:
 
     .. code:: python
 
-        _REQUIRED_PARAMS = ["API_KEY"]
+        _REQUIRED_PARAMS = ["AuthKey"]
 
     In __init__
 
     Be sure to call
 
     .. code::
 
@@ -127,21 +127,21 @@
     def __init__(self, **kwargs):
         """Initialize the class."""
         super().__init__(**kwargs)
         self._httpx_client = httpx.Client(timeout=get_http_timeout(**kwargs))
         self._request_params = {}
         if "ApiID" in kwargs:
             api_id = kwargs.pop("ApiID")
-            self._request_params["API_ID"] = api_id.strip() if api_id else None
+            self._request_params["ApiID"] = api_id.strip() if api_id else None
         if "AuthKey" in kwargs:
             auth_key = kwargs.pop("AuthKey")
-            self._request_params["API_KEY"] = auth_key.strip() if auth_key else None
+            self._request_params["AuthKey"] = auth_key.strip() if auth_key else None
         if "Instance" in kwargs:
             auth_key = kwargs.pop("Instance")
-            self._request_params["INSTANCE"] = auth_key.strip() if auth_key else None
+            self._request_params["Instance"] = auth_key.strip() if auth_key else None
 
         missing_params = [
             param
             for param in self._REQUIRED_PARAMS
             if param not in self._request_params
         ]
```

### Comparing `msticpy-2.4.0/msticpy/context/ip_utils.py` & `msticpy-2.5.0/msticpy/context/ip_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/lookup.py` & `msticpy-2.5.0/msticpy/context/lookup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 requests per minute for the account type that you have.
 
 """
 import asyncio
 import importlib
 import warnings
 from collections import ChainMap
-from typing import Any, Dict, Iterable, List, Mapping, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, List, Mapping, Optional, Tuple, Union, cast
 
 import nest_asyncio
 import pandas as pd
 from tqdm.auto import tqdm
 
 from .._version import VERSION
 from ..common.exceptions import MsticpyConfigError, MsticpyUserConfigError
@@ -66,14 +66,15 @@
     No Providers are loaded - please check that
     you have correctly configured your msticpyconfig.yaml settings.
     """
 
     _HELP_URI = "https://msticpy.readthedocs.io/en/latest/DataEnrichment.html"
 
     PROVIDERS: Dict[str, Tuple[str, str]] = {}
+    CUSTOM_PROVIDERS: Dict[str, Provider]
 
     PACKAGE: str = ""
 
     def __init__(self, providers: Optional[List[str]] = None, **kwargs):
         """
         Initialize TILookup instance.
 
@@ -603,23 +604,23 @@
                 final_remaining = await prog_counter.get_remaining()
                 if final_remaining:
                     prog_bar.update(total - final_remaining)
 
     @property
     def available_providers(self) -> List[str]:
         """
-        Return a list of builtin providers.
+        Return a list of builtin and plugin providers.
 
         Returns
         -------
         List[str]
             List of TI Provider classes.
 
         """
-        return list(self.PROVIDERS)
+        return list(self.PROVIDERS) + list(self.CUSTOM_PROVIDERS)
 
     @classmethod
     def list_available_providers(
         cls, show_query_types=False, as_list: bool = False
     ) -> Optional[List[str]]:  # type: ignore
         """
         Print a list of builtin providers with optional usage.
@@ -644,54 +645,54 @@
             provider_class = cls.import_provider(provider_name)
             if not as_list:
                 print(provider_name)
             providers.append(provider_name)
             if show_query_types and provider_class:
                 provider_class.usage()
 
-        if as_list:
-            return providers
-        return None
+        return providers if as_list else None
 
     @classmethod
     def import_provider(cls, provider: str) -> Provider:
         """Import provider class."""
         mod_name, cls_name = cls.PROVIDERS.get(provider, (None, None))
 
         if not (mod_name and cls_name):
+            if hasattr(cls, "CUSTOM_PROVIDERS") and provider in cls.CUSTOM_PROVIDERS:
+                return cast(Provider, cls.CUSTOM_PROVIDERS[provider])
             raise LookupError(
-                f"No driver available for environment {provider}.",
+                f"No provider named '{provider}'.",
                 "Possible values are:",
-                ", ".join(list(cls.PROVIDERS)),
+                ", ".join(list(cls.PROVIDERS) + list(cls.CUSTOM_PROVIDERS)),
             )
 
         imp_module = importlib.import_module(
             f"msticpy.context.{cls.PACKAGE}.{mod_name}", package="msticpy"
         )
         return getattr(imp_module, cls_name)
 
     def _load_providers(self, **kwargs):
         """Load provider classes based on config."""
         prov_type = kwargs.get("providers", "Providers")
         prov_settings = get_provider_settings(prov_type)
-
-        for provider_entry, settings in prov_settings.items():
-            # Allow overriding provider name to use another class
-            provider_name = settings.provider or provider_entry
+        provider_class: Provider
+        for provider_name, settings in prov_settings.items():
             if (
                 self._providers_to_load is not None
                 and provider_name not in self._providers_to_load
-            ) or provider_name == "--no-load--":
+            ) or settings.provider == "--no-load--":
                 continue
             try:
-                provider_class: Provider = self.import_provider(provider_name)
+                provider_name = settings.provider or provider_name
+                provider_class = self.import_provider(provider_name)
             except LookupError:
                 warnings.warn(
                     f"Could not find provider class for {provider_name} "
-                    f"in config section {provider_entry}"
+                    f"in config section '{provider_name}'. "
+                    f"Provider class name in config is '{settings.provider}'"
                 )
                 continue
 
             # instantiate class sending args from settings to init
             try:
                 provider_instance = provider_class(**(settings.args))
             except MsticpyConfigError as mp_ex:
```

### Comparing `msticpy-2.4.0/msticpy/context/lookup_result.py` & `msticpy-2.5.0/msticpy/context/lookup_result.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/preprocess_observable.py` & `msticpy-2.5.0/msticpy/context/preprocess_observable.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/provider_base.py` & `msticpy-2.5.0/msticpy/context/provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/tilookup.py` & `msticpy-2.5.0/msticpy/context/tilookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 Input can be a single IoC observable or a pandas DataFrame containing
 multiple observables. Processing may require a an API key and
 processing performance may be limited to a specific number of
 requests per minute for the account type that you have.
 
 """
 
-from typing import Iterable, List, Mapping, Optional, Union
+from typing import Dict, Iterable, List, Mapping, Optional, Union
 
 import pandas as pd
 
 from .._version import VERSION
 from ..common.utility import export
 from .lookup import Lookup
-from .provider_base import _make_sync
 
 # used in dynamic instantiation of providers
+from .provider_base import Provider, _make_sync
 from .tiproviders import TI_PROVIDERS
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 
 @export
@@ -40,14 +40,15 @@
     _HELP_URI = (
         "https://msticpy.readthedocs.io/en/latest/data_acquisition/"
         "TIProviders.html#configuration-file"
     )
 
     PROVIDERS = TI_PROVIDERS
     PACKAGE = "tiproviders"
+    CUSTOM_PROVIDERS: Dict[str, Provider] = {}
 
     # pylint: disable=too-many-arguments
     def lookup_ioc(
         self,
         ioc: Optional[str] = None,
         ioc_type: Optional[str] = None,
         ioc_query_type: Optional[str] = None,
```

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/__init__.py` & `msticpy-2.5.0/msticpy/context/tiproviders/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/alienvault_otx.py` & `msticpy-2.5.0/msticpy/context/tiproviders/alienvault_otx.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # pylint: disable=too-few-public-methods
 @attr.s
 class _OTXParams(APILookupParams):
     # override APILookupParams to set common defaults
     def __attrs_post_init__(self):
         # pylint: disable=
-        self.headers = {"X-OTX-API-KEY": "{API_KEY}"}
+        self.headers = {"X-OTX-API-KEY": "{AuthKey}"}
 
 
 @export
 class OTX(HttpTIProvider):
     """AlientVault OTX Lookup."""
 
     _BASE_URL = "https://otx.alienvault.com"
@@ -63,15 +63,15 @@
     }
 
     # aliases
     _QUERIES["md5_hash"] = _QUERIES["file_hash"]
     _QUERIES["sha1_hash"] = _QUERIES["file_hash"]
     _QUERIES["sha256_hash"] = _QUERIES["file_hash"]
 
-    _REQUIRED_PARAMS = ["API_KEY"]
+    _REQUIRED_PARAMS = ["AuthKey"]
 
     def __init__(self, **kwargs):
         """Set OTX specific settings."""
         super().__init__(**kwargs)
         self.require_url_encoding = True
 
     def parse_results(self, response: Dict) -> Tuple[bool, ResultSeverity, Any]:
```

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/azure_sent_byoti.py` & `msticpy-2.5.0/msticpy/context/tiproviders/azure_sent_byoti.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/greynoise.py` & `msticpy-2.5.0/msticpy/context/tiproviders/greynoise.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 
     _BASE_URL = "https://api.greynoise.io"
 
     _QUERIES = {
         # Community API
         "ipv4": APILookupParams(
             path="/v3/community/{observable}",
-            headers={"key": "{API_KEY}"},
+            headers={"key": "{AuthKey}"},
         ),
         # Enterprise API Quick Lookup
         "ipv4-quick": APILookupParams(
             path="/v2/noise/quick/{observable}",
-            headers={"key": "{API_KEY}"},
+            headers={"key": "{AuthKey}"},
         ),
         # Enterprise API Full Lookup
         "ipv4-full": APILookupParams(
             path="/v2/noise/context/{observable}",
-            headers={"key": "{API_KEY}"},
+            headers={"key": "{AuthKey}"},
         ),
     }
 
     def parse_results(self, response: Dict) -> Tuple[bool, ResultSeverity, Any]:
         """
         Return the details of the response.
```

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/ibm_xforce.py` & `msticpy-2.5.0/msticpy/context/tiproviders/ibm_xforce.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 # pylint: disable=too-few-public-methods
 @attr.s
 class _XForceParams(APILookupParams):
     # override APILookupParams to set common defaults
     def __attrs_post_init__(self):
-        self.auth_str = ["{API_ID}", "{API_KEY}"]
+        self.auth_str = ["{ApiID}", "{AuthKey}"]
         self.auth_type = "HTTPBasic"
 
 
 @export
 class XForce(HttpTIProvider):
     """IBM XForce Lookup."""
 
@@ -64,15 +64,15 @@
     _QUERIES["dns"] = _QUERIES["url"]
     _QUERIES["dns-malware"] = _QUERIES["url-malware"]
     _QUERIES["ipv4-passivedns"] = _QUERIES["dns-passivedns"]
     _QUERIES["ipv6-passivedns"] = _QUERIES["dns-passivedns"]
     _QUERIES["hostname-whois"] = _QUERIES["ipv4-whois"]
     _QUERIES["dns-whois"] = _QUERIES["ipv4-whois"]
 
-    _REQUIRED_PARAMS = ["API_ID", "API_KEY"]
+    _REQUIRED_PARAMS = ["ApiID", "AuthKey"]
 
     def parse_results(self, response: Dict) -> Tuple[bool, ResultSeverity, Any]:
         """
         Return the details of the response.
 
         Parameters
         ----------
```

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/intsights.py` & `msticpy-2.5.0/msticpy/context/tiproviders/intsights.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 # pylint: disable=too-few-public-methods
 @attr.s
 class _IntSightsParams(APILookupParams):
     # override APILookupParams to set common defaults
     def __attrs_post_init__(self):
-        self.auth_str = ["{API_ID}", "{API_KEY}"]
+        self.auth_str = ["{ApiID}", "{AuthKey}"]
         self.auth_type = "HTTPBasic"
 
 
 @export
 class IntSights(HttpTIProvider):
     """IntSights Lookup."""
 
@@ -83,15 +83,15 @@
         "email": _IntSightsParams(
             path="/public/v2/iocs/ioc-by-value",
             params={"iocValue": "{observable}"},
             headers=_DEF_HEADERS,
         ),
     }
 
-    _REQUIRED_PARAMS = ["API_ID", "API_KEY"]
+    _REQUIRED_PARAMS = ["ApiID", "AuthKey"]
 
     def parse_results(self, response: Dict) -> Tuple[bool, ResultSeverity, Any]:
         """
         Return the details of the response.
 
         Parameters
         ----------
```

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/kql_base.py` & `msticpy-2.5.0/msticpy/context/tiproviders/kql_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/mblookup.py` & `msticpy-2.5.0/msticpy/context/tiproviders/mblookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/open_page_rank.py` & `msticpy-2.5.0/msticpy/context/tiproviders/open_page_rank.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 
     _BASE_URL = "https://openpagerank.com"
 
     _QUERIES = {
         "dns": APILookupParams(
             path="/api/v1.0/getPageRank",
             params={"domains[0]": "{observable}"},
-            headers={"API-OPR": "{API_KEY}"},
+            headers={"API-OPR": "{AuthKey}"},
         )
     }
 
-    _REQUIRED_PARAMS = ["API_KEY"]
+    _REQUIRED_PARAMS = ["AuthKey"]
 
     def __init__(self, **kwargs):
         """Initialize a new instance of the class."""
         super().__init__(**kwargs)
 
         self._provider_name = self.__class__.__name__
         print(
```

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/pulsedive.py` & `msticpy-2.5.0/msticpy/context/tiproviders/pulsedive.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,39 +65,32 @@
 class PDlookup:
     """
     PDlookup: A class to interact with the Pulsedive API.
 
     This class allows you to look up indicators of compromise (IOCs) and
     explore different types of data available in the Pulsedive API.
 
-    Attributes
-    ----------
-    pd_key (str): An API key for the Pulsedive API.
-
-    Methods
-    -------
-    _make_pd_request(data): Makes a request to the Pulsedive API with the provided data.
-    lookup_ioc(observable: str, pd_type: str) -> pd.DataFrame: Lookup an indicator of
-    compromise in the Pulsedive API.
-    explore(query: str, pd_type: str) -> pd.DataFrame: Explore different types of data
-    available in the Pulsedive API.
-    scan(observable: str, pd_type: str) -> pd.DataFrame: Submits an indicator of compromise
-    to the Pulsedive API for scanning.
-
     """
 
     _SUPPORTED_PD_TYPES: Set[PDEntityType] = {
         PDEntityType.INDICATOR,
         PDEntityType.THREAT,
         PDEntityType.EXPLORE,
         PDEntityType.SCAN,
     }
 
     def __init__(self, pd_key=None):
-        """Init function to get the API key if necessary."""
+        """
+        Init function to get the API key if necessary.
+
+        Parameters
+        ----------
+        pd_key (str): An API key for the Pulsedive API.
+
+        """
         self.pd_key = pd_key or self._get_pd_api_key()
 
     def lookup_ioc(self, observable: str, pd_type: str = "indicator") -> pd.DataFrame:
         """
         Lookup an indicator of compromise (IOC) in the Pulsedive API.
 
         Parameters
@@ -279,15 +272,16 @@
         pd_settings = get_provider_settings("TIProviders").get("Pulsedive")
         if pd_settings and "AuthKey" in pd_settings.args:
             return pd_settings.args["AuthKey"]
         return None
 
 
 def _build_query_string(data, pd_type) -> PDQuery:
-    """Build query string for the API request based on the provided data and pd_type.
+    """
+    Build query string for the API request based on the provided data and pd_type.
 
     Parameters
     ----------
     data : Any
         Data to be mapped to query_item
 
     pd_type : str
```

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/result_severity.py` & `msticpy-2.5.0/msticpy/context/tiproviders/result_severity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/riskiq.py` & `msticpy-2.5.0/msticpy/context/tiproviders/riskiq.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/ti_http_provider.py` & `msticpy-2.5.0/msticpy/context/tiproviders/ti_http_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/ti_provider_base.py` & `msticpy-2.5.0/msticpy/context/tiproviders/ti_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/tor_exit_nodes.py` & `msticpy-2.5.0/msticpy/context/tiproviders/tor_exit_nodes.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/tiproviders/virustotal.py` & `msticpy-2.5.0/msticpy/context/tiproviders/virustotal.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 @export
 class VirusTotal(HttpTIProvider):
     """VirusTotal Lookup."""
 
     _BASE_URL = "https://www.virustotal.com/"
 
-    _PARAMS = {"apikey": "{API_KEY}"}
+    _PARAMS = {"apikey": "{AuthKey}"}
     _QUERIES = {
         "ipv4": APILookupParams(
             path="vtapi/v2/ip-address/report",
             params={**_PARAMS, "ip": "{observable}"},
             headers=_DEF_HEADERS,
         ),
         "dns": APILookupParams(
@@ -60,15 +60,15 @@
     }
 
     # aliases
     _QUERIES["md5_hash"] = _QUERIES["file_hash"]
     _QUERIES["sha1_hash"] = _QUERIES["file_hash"]
     _QUERIES["sha256_hash"] = _QUERIES["file_hash"]
 
-    _REQUIRED_PARAMS = ["API_KEY"]
+    _REQUIRED_PARAMS = ["AuthKey"]
 
     _VT_DETECT_RESULTS = {
         "detected_urls": ("url", "scan_date"),
         "detected_downloaded_samples": ("sha256", "date"),
         "detected_communicating_samples": ("sha256", "date"),
     }
```

### Comparing `msticpy-2.4.0/msticpy/context/vtlookupv3/__init__.py` & `msticpy-2.5.0/msticpy/context/vtlookupv3/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/vtlookupv3/vtfile_behavior.py` & `msticpy-2.5.0/msticpy/context/vtlookupv3/vtfile_behavior.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/vtlookupv3/vtlookup.py` & `msticpy-2.5.0/msticpy/context/vtlookupv3/vtlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/context/vtlookupv3/vtlookupv3.py` & `msticpy-2.5.0/msticpy/context/vtlookupv3/vtlookupv3.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/__init__.py` & `msticpy-2.5.0/msticpy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/azure/__init__.py` & `msticpy-2.5.0/msticpy/data/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/azure/azure_blob_storage.py` & `msticpy-2.5.0/msticpy/data/azure/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/azure/azure_data.py` & `msticpy-2.5.0/msticpy/data/azure/azure_data.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/azure_blob_storage.py` & `msticpy-2.5.0/msticpy/data/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/azure_data.py` & `msticpy-2.5.0/msticpy/data/azure_data.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/azure_sentinel.py` & `msticpy-2.5.0/msticpy/data/azure_sentinel.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/core/data_providers.py` & `msticpy-2.5.0/msticpy/data/drivers/mordor_driver.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,849 +1,946 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-"""Data provider loader."""
-import re
-from collections import abc
+"""Mordor/OTRF Security datasets driver."""
+import json
+import pickle  # nosec
+import zipfile
+from collections import defaultdict
 from datetime import datetime
-from functools import partial
-from itertools import tee
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, NamedTuple, Optional, Pattern, Union
+from typing import Any, Dict, Generator, Iterable, List, Optional, Set, Tuple, Union
+from zipfile import BadZipFile, ZipFile
 
+import attr
+import httpx
 import pandas as pd
+import yaml
 from tqdm.auto import tqdm
 
 from ..._version import VERSION
-from ...common.exceptions import MsticpyDataQueryError
+from ...common.exceptions import MsticpyUserError
 from ...common.pkg_config import get_config
-from ...common.utility import export, valid_pyname
-from ...nbwidgets import QueryTime
-from ..drivers import DriverBase, import_driver
-from .param_extractor import extract_query_params
-from .query_container import QueryContainer
-from .query_defns import DataEnvironment
-from .query_source import QuerySource
-from .query_store import QueryStore
+from ...common.utility import mp_ua_header
+from ..core.query_source import QuerySource
+from .driver_base import DriverBase, DriverProps
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
-_HELP_FLAGS = ("help", "?")
-_DEBUG_FLAGS = ("print", "debug_query", "print_query")
-_COMPATIBLE_DRIVER_MAPPINGS = {"mssentinel": ["m365d"], "mde": ["m365d"]}
 
+_MORDOR_TREE_URI = (
+    "https://api.github.com/repos/OTRF/Security-Datasets/git/trees/master?recursive=1"
+)
+
+_MITRE_JSON_URL = (
+    "https://raw.githubusercontent.com/mitre/cti/"
+    "master/enterprise-attack/enterprise-attack.json"
+)
+_MTR_TAC_CAT_URI = "https://attack.mitre.org/tactics/{cat}/"
+_MTR_TECH_CAT_URI = "https://attack.mitre.org/techniques/{cat}/"
+
+MITRE_TECHNIQUES: Optional[pd.DataFrame] = None
+MITRE_TACTICS: Optional[pd.DataFrame] = None
+
+_MITRE_TECH_CACHE = "mitre_tech_cache.pkl"
+_MITRE_TACTICS_CACHE = "mitre_tact_cache.pkl"
+_MORDOR_CACHE = "mordor_cache.json"
+
+_HTTP_TIMEOUT = DriverBase.get_http_timeout()
+
+
+# pylint: disable=too-many-instance-attributes
+class MordorDriver(DriverBase):
+    """Mordor data driver."""
+
+    def __init__(self, **kwargs):
+        """Initialize the Mordor driver."""
+        super().__init__(**kwargs)
+        self.use_query_paths = False
+        self.has_driver_queries = True
+        self.mitre_techniques: pd.DataFrame
+        self.mitre_tactics: pd.DataFrame
+        self.mordor_data: Dict[str, MordorEntry]
+        self.mdr_idx_tech: Dict[str, Set[str]]
+        self.mdr_idx_tact: Dict[str, Set[str]]
+        self._driver_queries: List[Dict[str, Any]] = []
+
+        mdr_settings = get_config("DataProviders.Mordor", {})
+        self.use_cached = kwargs.pop(
+            "used_cached", mdr_settings.get("used_cached", True)
+        )
+        self.save_folder = kwargs.pop(
+            "save_folder", mdr_settings.get("save_folder", ".")
+        )
+        self.save_folder = _resolve_cache_folder(self.save_folder)
+        self.silent = kwargs.pop("silent", False)
 
-class QueryParam(NamedTuple):
-    """
-    Named tuple for custom query parameters.
+        self._loaded = True
 
-    name and data_type are mandatory.
-    description and default are optional.
+    # pylint: disable=global-statement
 
-    """
+    def connect(self, connection_str: Optional[str] = None, **kwargs):
+        """
+        Connect to data source.
 
-    name: str
-    data_type: str
-    description: Optional[str] = None
-    default: Optional[str] = None
+        Parameters
+        ----------
+        connection_str : Optional[str]
+            Connect to a data source
 
+        """
+        global MITRE_TECHNIQUES, MITRE_TACTICS
+        cache_folder = self.save_folder if self.use_cached else None
+        print("Retrieving Mitre data...")
+
+        if MITRE_TECHNIQUES is None or MITRE_TACTICS is None:
+            MITRE_TECHNIQUES, MITRE_TACTICS = _get_mitre_categories(
+                cache_folder=cache_folder
+            )
+        self.mitre_techniques = MITRE_TECHNIQUES
+        self.mitre_tactics = MITRE_TACTICS
+
+        print("Retrieving Mordor data...")
+
+        self.mordor_data = _GET_MORDOR_METADATA(cache_folder=cache_folder)
+        self.mdr_idx_tech, self.mdr_idx_tact = _build_mdr_indexes(self.mordor_data)
+
+        self._connected = True
+        self.set_driver_property(
+            DriverProps.PUBLIC_ATTRS,
+            {
+                "mitre_techniques": self.mitre_techniques,
+                "mitre_tactics": self.mitre_tactics,
+                "driver_queries": self.driver_queries,
+                "search_queries": self.search_queries,
+            },
+        )
 
-@export
-class QueryProvider:
-    """
-    Container for query store and query execution provider.
+    # pylint: enable=global-statement
 
-    Instances of this class hold the query set and execution
-    methods for a specific data environment.
+    def query(
+        self, query: str, query_source: QuerySource = None, **kwargs
+    ) -> Union[pd.DataFrame, Any]:
+        """
+        Execute query string and return DataFrame of results.
 
-    """
+        Parameters
+        ----------
+        query : str
+            The query to execute
+        query_source : QuerySource
+            The query definition object
 
-    create_param = QueryParam
+        Other Parameters
+        ----------------
+        kwargs :
+            Are passed to the underlying provider query method,
+            if supported.
 
-    def __init__(  # noqa: MC0001
-        self,
-        data_environment: Union[str, DataEnvironment],
-        driver: DriverBase = None,
-        query_paths: List[str] = None,
-        **kwargs,
-    ):
+        Returns
+        -------
+        Union[pd.DataFrame, Any]
+            A DataFrame (if successfull) or
+            the underlying provider result if an error.
+
+        """
+        del query_source
+        if not self._connected:
+            raise self._create_not_connected_err("OTRF Datasets")
+        use_cached = kwargs.pop("used_cached", self.use_cached)
+        save_folder = kwargs.pop("save_folder", self.save_folder)
+        save_folder = _resolve_cache_folder(save_folder)
+        silent = kwargs.pop("silent", self.silent)
+        result_df = download_mdr_file(
+            file_uri=query,
+            use_cached=use_cached,
+            save_folder=save_folder,
+            silent=silent,
+        )
+        if not isinstance(result_df, pd.DataFrame) or result_df.empty:
+            return "Could not convert result to a DataFrame."
+        return result_df
+
+    def query_with_results(self, query: str, **kwargs) -> Tuple[pd.DataFrame, Any]:
         """
-        Query provider interface to queries.
+        Execute query string and return DataFrame plus native results.
 
         Parameters
         ----------
-        data_environment : Union[str, DataEnvironment]
-            Name or Enum of environment for the QueryProvider
-        driver : DriverBase, optional
-            Override the builtin driver (query execution class)
-            and use your own driver (must inherit from
-            `DriverBase`)
-        query_paths : List[str]
-            Additional paths to look for query definitions.
-        kwargs :
-            Other arguments are passed to the data provider driver.
+        query : str
+            The query to execute
 
-        See Also
-        --------
-        DataProviderBase : base class for data query providers.
-
-        """
-        # import at runtime to prevent circular import
-        # pylint: disable=import-outside-toplevel, cyclic-import
-        from ...init.pivot_init.pivot_data_queries import add_data_queries_to_entities
-
-        # pylint: enable=import-outside-toplevel
-        setattr(self.__class__, "_add_pivots", add_data_queries_to_entities)
-
-        if isinstance(data_environment, str):
-            data_env = DataEnvironment.parse(data_environment)
-            if data_env != DataEnvironment.Unknown:
-                data_environment = data_env
-            else:
-                raise TypeError(f"Unknown data environment {data_environment}")
-        self.environment = data_environment.name
-
-        self._driver_kwargs = kwargs.copy()
-        if driver is None:
-            self.driver_class = import_driver(data_environment)
-            if issubclass(self.driver_class, DriverBase):
-                driver = self.driver_class(data_environment=data_environment, **kwargs)
-            else:
-                raise LookupError(
-                    "Could not find suitable data provider for", f" {self.environment}"
+        Returns
+        -------
+        Tuple[pd.DataFrame,Any]
+            A DataFrame and native results.
+
+        """
+        result = self.query(query, **kwargs)
+        if isinstance(result, pd.DataFrame):
+            return result, "OK"
+        return pd.DataFrame, result
+
+    @property
+    def driver_queries(self) -> Iterable[Dict[str, Any]]:
+        """
+        Return generator of Mordor query definitions.
+
+        Yields
+        ------
+        Iterable[Dict[str, Any]]
+            Iterable of Dictionaries containing query definitions.
+
+        """
+        if not self._connected:
+            raise self._create_not_connected_err("OTRF Datasets")
+        if not self._driver_queries:
+            self._driver_queries = list(self._get_driver_queries())
+        return self._driver_queries
+
+    def _get_driver_queries(self):
+        """Generate iterable of Mordor queries."""
+        for mdr_item in self.mordor_data.values():
+            for file_path in mdr_item.get_file_paths():
+                mitre_data = mdr_item.get_attacks()
+                techniques = ", ".join(
+                    f"{att.technique}: {att.technique_name}" for att in mitre_data
+                )
+
+                tactics = ", ".join(
+                    f"{tac[0]}: {tac[1]}"
+                    for att in mitre_data
+                    for tac in att.tactics_full
                 )
-        else:
-            self.driver_class = driver.__class__
-        self._additional_connections: Dict[str, DriverBase] = {}
-        self._query_provider = driver
-        self.all_queries = QueryContainer()
-
-        # Add any query files
-        data_env_queries: Dict[str, QueryStore] = {}
-        if driver.use_query_paths:
-            data_env_queries.update(
-                self._read_queries_from_paths(query_paths=query_paths)
-            )
-        self.query_store = data_env_queries.get(
-            self.environment, QueryStore(self.environment)
-        )
-        self._add_query_functions()
-        self._query_time = QueryTime(units="day")
 
-    def __getattr__(self, name):
-        """Return the value of the named property 'name'."""
-        if "." in name:
-            parent_name, child_name = name.split(".", maxsplit=1)
-            parent = getattr(self, parent_name, None)
-            if parent:
-                return getattr(parent, child_name)
-        raise AttributeError(f"{name} is not a valid attribute.")
+                doc_string: List[str] = [
+                    f"{mdr_item.title}",
+                    "",
+                    "Notes",
+                    "-----",
+                    f"Mordor ID: {mdr_item.id}",
+                    mdr_item.description or "",
+                    "",
+                    f"Mitre Techniques: {techniques}",
+                    f"Mitre Tactics: {tactics}",
+                ]
+                q_container, _, full_name = file_path["qry_path"].partition(".")
+                short_name = file_path["qry_path"].split(".")[-1]
+                yield {
+                    "name": full_name,
+                    "description": "\n".join(doc_string),
+                    "query_name": short_name,
+                    "query": file_path["file_path"],
+                    "query_container": q_container,
+                    "metadata": {},
+                }
 
-    def connect(self, connection_str: str = None, **kwargs):
+    def search_queries(self, search: str) -> Iterable[str]:
         """
-        Connect to data source.
+        Search queries for matching attributes.
 
         Parameters
         ----------
-        connection_str : str
-            Connection string for the data source
+        search : str
+            Search string. Substrings separated by commas will
+            be treated as OR terms - e.g. "a, b" == "a" or "b".
+            Substrings separated by "+" will be treated as AND
+            terms - e.g. "a + b" == "a" and "b"
+
+        Returns
+        -------
+        Iterable[str]
+            Iterable of matching query names.
+
 
         """
-        self._query_provider.connect(connection_str=connection_str, **kwargs)
+        if not self._connected:
+            raise self._create_not_connected_err("OTRF Datasets")
+        matches = []
+        for mdr_id in search_mdr_data(self.mordor_data, terms=search):
+            for file_path in self.mordor_data[mdr_id].get_file_paths():
+                matches.append(
+                    f"{file_path['qry_path']} ({self.mordor_data[mdr_id].title})"
+                )
+        return matches
+
+
+def _resolve_cache_folder(cache_path: str):
+    """Expand and optionally creates cache folder."""
+    cache_folder = Path(cache_path).expanduser()
+    if not cache_folder.is_dir():
+        cache_folder.mkdir(parents=True, exist_ok=True)
+    return str(cache_folder)
+
 
-        # If the driver has any attributes to expose via the provider
-        # add those here.
-        for attr_name, attr in self._query_provider.public_attribs.items():
-            setattr(self, attr_name, attr)
+# pylint: enable=too-many-instance-attributes
 
-        # Add any built-in or dynamically retrieved queries from driver
-        if self._query_provider.has_driver_queries:
-            driver_queries = self._query_provider.driver_queries
-            self._add_driver_queries(queries=driver_queries)
-        # Since we're now connected, add Pivot functions
-        self._add_pivots(lambda: self._query_time.timespan)
 
-    def add_connection(
+class MitreAttack:
+    """MitreAttack container for techniques and tactics."""
+
+    MTR_TECH_URI = "https://attack.mitre.org/techniques/{technique_id}/"
+    MTR_TAC_URI = "https://attack.mitre.org/tactics/{tactic_id}/"
+
+    def __init__(
         self,
-        connection_str: Optional[str] = None,
-        alias: Optional[str] = None,
-        **kwargs,
+        attack: Dict[str, Any] = None,
+        technique: str = None,
+        sub_technique: str = None,
+        tactics: List[str] = None,
     ):
         """
-        Add an additional connection for the query provider.
+        Create instance of MitreAttack.
 
         Parameters
         ----------
-        connection_str : Optional[str], optional
-            Connection string for the provider, by default None
-        alias : Optional[str], optional
-            Alias to use for the connection, by default None
+        attack : Dict[str, Any], optional
+            attack data as dictionary, by default None
+        technique : str, optional
+            technique ID, by default None
+        sub_technique : str, optional
+            sub-technique ID, by default None
+        tactics : List[str], optional
+            List of associated tactics, by default None
+
+        """
+        if attack is None and (technique is None and tactics is None):
+            raise TypeError(
+                "Either 'attack' or 'technique' and 'tactics' must be specified."
+            )
+        self.technique = attack.get("technique") if attack else technique
+        self.sub_technique = attack.get("sub-technique") if attack else sub_technique
+        self.tactics = attack.get("tactics") if attack else tactics  # type: ignore
+
+        self._technique_name = None
+        self._technique_desc = None
+        self._technique_uri = None
+        self._tactics_full: List[Tuple[str, str, str, str]] = []
 
-        Other Parameters
-        ----------------
-        kwargs : Dict[str, Any]
-            Other parameters passed to the driver constructor.
-
-        Notes
-        -----
-        Some drivers may accept types other than strings for the
-        `connection_str` parameter.
-
-        """
-        # create a new instance of the driver class
-        new_driver = self.driver_class(**(self._driver_kwargs))
-        # connect
-        new_driver.connect(connection_str=connection_str, **kwargs)
-        # add to collection
-        driver_key = alias or str(len(self._additional_connections))
-        self._additional_connections[driver_key] = new_driver
-
-    @property
-    def connected(self) -> bool:
+    def __repr__(self) -> str:
         """
-        Return True if the provider is connected.
+        Return repr of MitreAttack object.
 
         Returns
         -------
-        bool
-            True if the provider is connected.
+        str
+            The repr of the object.
 
         """
-        return self._query_provider.connected
+        return "".join(
+            [
+                f"MitreAttack(technique={self.technique}), ",
+                f"sub_technique={self.sub_technique}, ",
+                f"tactics={repr(self.tactics)}",
+            ]
+        )
 
     @property
-    def connection_string(self) -> str:
+    def technique_name(self) -> Optional[str]:
         """
-        Return provider connection string.
+        Return Mitre Technique full name.
 
         Returns
         -------
-        str
-            Provider connection string.
+        Optional[str]
+            Name of the Mitre technique
 
         """
-        return self._query_provider.current_connection
+        if (
+            not self._technique_name
+            and self.technique in MITRE_TECHNIQUES.index  # type: ignore[union-attr]
+        ):
+            self._technique_name = MITRE_TECHNIQUES.loc[  # type: ignore[union-attr]
+                self.technique
+            ].Name
+        return self._technique_name
 
     @property
-    def schema(self) -> Dict[str, Dict]:
+    def technique_desc(self) -> Optional[str]:
         """
-        Return current data schema of connection.
+        Return Mitre technique description.
 
         Returns
         -------
-        Dict[str, Dict]
-            Data schema of current connection.
+        Optional[str]
+            Technique description
 
         """
-        return self._query_provider.schema
+        if (
+            not self._technique_desc
+            and self.technique in MITRE_TECHNIQUES.index  # type: ignore[union-attr]
+        ):
+            self._technique_desc = MITRE_TECHNIQUES.loc[  # type: ignore
+                self.technique
+            ].Description
+        return self._technique_desc
 
     @property
-    def schema_tables(self) -> List[str]:
+    def technique_uri(self) -> str:
         """
-        Return list of tables in the data schema of the connection.
+        Return Mitre Technique URI.
 
         Returns
         -------
-        List[str]
-            Tables in the of current connection.
+        Optional[str]
+            URI of the Mitre technique
 
         """
-        return list(self._query_provider.schema.keys())
+        return self.MTR_TECH_URI.format(technique_id=self.technique)
 
     @property
-    def instance(self) -> Optional[str]:
+    def tactics_full(self) -> List[Tuple[str, str, str, str]]:
         """
-        Return instance name, if any for provider.
+        Return full listing of Mitre tactics.
 
         Returns
         -------
-        Optional[str]
-            The instance name or None for drivers that do not
-            support multiple instances.
+        List[Tuple[str, str, str, str]]
+            List of tuples of:
+            (ID, Name, Description, URI)
 
         """
-        return self._query_provider.instance
+        if not self._tactics_full and self.tactics:
+            for tactic in self.tactics:
+                tactic_name = tactic_desc = "unknown"
+                if tactic in MITRE_TACTICS.index:  # type: ignore[union-attr]
+                    tactic_name = MITRE_TACTICS.loc[tactic].Name  # type: ignore[union-attr]
+                    tactic_desc = MITRE_TACTICS.loc[tactic].Description  # type: ignore[union-attr]
+                tactic_uri = self.MTR_TAC_URI.format(tactic_id=tactic)
+                self._tactics_full.append(
+                    (tactic, tactic_name, tactic_desc, tactic_uri)
+                )
+        return self._tactics_full
 
-    def import_query_file(self, query_file: str):
-        """
-        Import a yaml data source definition.
 
-        Parameters
-        ----------
-        query_file : str
-            Path to the file to import
+def _to_datetime(date_val) -> datetime:
+    """
+    Return datetime from parsed date string.
 
-        """
-        self.query_store.import_file(query_file)
-        self._add_query_functions()
+    Parameters
+    ----------
+    date_val : datetime
+        The datetime or datetime string.
+
+    Returns
+    -------
+    datetime
+        Parse datetime.
 
-    @classmethod
-    def list_data_environments(cls) -> List[str]:
-        """
-        Return list of current data environments.
+    """
+    if isinstance(date_val, datetime):
+        return date_val
+    try:
+        return pd.to_datetime(date_val)
+    except TypeError:
+        return datetime.min
 
-        Returns
-        -------
-        List[str]
-            List of current data environments
 
-        """
-        # pylint: disable=not-an-iterable
-        return [env for env in DataEnvironment.__members__ if env != "Unknown"]
-        # pylint: enable=not-an-iterable
+DS_PREFIX = "https://raw.githubusercontent.com/OTRF/Security-Datasets/master/datasets/"
 
-    def list_queries(self, substring: Optional[str] = None) -> List[str]:
-        """
-        Return list of family.query in the store.
 
-        Parameters
-        ----------
-        substring : Optional[str]
-            Optional pattern - will return only queries matching the pattern,
-            default None.
+# pylint: disable=not-an-iterable, no-member
+
+
+@attr.s(auto_attribs=True)
+class MordorEntry:
+    """Mordor data set metadata."""
+
+    title: str
+    id: str
+    type: str
+    creation_date: datetime = attr.ib(converter=_to_datetime)
+    modification_date: datetime = attr.ib(converter=_to_datetime)
+    contributors: List[str] = attr.Factory(list)
+    author: Optional[str] = None
+    platform: Optional[str] = None
+    description: Optional[str] = None
+    tags: List[str] = attr.Factory(list)
+    files: List[Dict[str, Any]] = attr.Factory(list)
+    datasets: List[Dict[str, Any]] = attr.Factory(list)
+    attack_mappings: List[Dict[str, Any]] = attr.Factory(list)
+    notebooks: List[Dict[str, str]] = attr.Factory(list)
+    simulation: Dict[str, Any] = attr.Factory(dict)
+    references: List[Any] = attr.Factory(list)
+    _rel_file_paths: List[Dict[str, Any]] = attr.Factory(list)
+
+    def get_notebooks(self) -> List[Tuple[str, str, str]]:
+        """
+        Return the list of notebooks for the dataset.
 
         Returns
         -------
-        List[str]
-            List of queries
+        List[Tuple[str, str, str]]
+            Tuples of (name, project, link)
 
         """
-        if substring:
-            return list(
-                filter(
-                    lambda x: substring in x.lower(),  # type: ignore
-                    self.query_store.query_names,
-                )
-            )
-        return list(self.query_store.query_names)
+        return [
+            (nbk.get("name", ""), nbk.get("project", ""), nbk.get("link", ""))
+            for nbk in self.notebooks
+        ]
 
-    def search(
-        self,
-        search: Union[str, Iterable[str]] = None,
-        table: Union[str, Iterable[str]] = None,
-        param: Union[str, Iterable[str]] = None,
-        ignore_case: bool = True,
-    ) -> List[str]:
+    def get_attacks(self) -> List[MitreAttack]:
         """
-        Search queries for match properties.
-
-        Parameters
-        ----------
-        search : Union[str, Iterable[str]], optional
-            String or iterable of search terms to match on
-            any property of the query, by default None.
-            The properties include: name, description, table,
-            parameter names and query_text.
-        table : Union[str, Iterable[str]], optional
-            String or iterable of search terms to match on
-            the query table name, by default None
-        param : Union[str, Iterable[str]], optional
-            String or iterable of search terms to match on
-            the query parameter names, by default None
-        ignore_case : bool
-            Use case-insensitive search, default is True.
+        Return list of Mitre attack classifications.
 
         Returns
         -------
-        List[str]
-            A list of matched queries
-
-        Notes
-        -----
-        Search terms are treated as regular expressions.
-        Supplying multiple parameters returns the intersection
-        of matches for each category. For example:
-        `qry_prov.search(search="account", table="syslog")` will
-        match queries that have a table parameter of "syslog" AND
-        have the term "Account" somewhere in the query properties.
-
-        """
-        if not (search or table or param):
-            return []
-
-        glob_searches = _normalize_to_regex(search, ignore_case)
-        table_searches = _normalize_to_regex(table, ignore_case)
-        param_searches = _normalize_to_regex(param, ignore_case)
-        search_hits: List[str] = []
-        for query, search_data in self.query_store.search_items.items():
-            glob_match = (not glob_searches) or any(
-                re.search(term, prop)
-                for term in glob_searches
-                for prop in search_data.values()
-            )
-            table_match = (not table_searches) or any(
-                re.search(term, search_data["table"]) for term in table_searches
-            )
-            param_match = (not param_searches) or any(
-                re.search(term, search_data["params"]) for term in param_searches
-            )
-            if glob_match and table_match and param_match:
-                search_hits.append(query)
-        return sorted(search_hits)
+        List[MitreAttack]
+            List of MitreAttack definitions.
 
-    def list_connections(self) -> List[str]:
         """
-        Return a list of current connections or the default connection.
+        return [MitreAttack(attack=attack) for attack in self.attack_mappings]
+
+    def get_file_paths(self) -> List[Dict[str, str]]:
+        """
+        Return list of data file links.
 
         Returns
         -------
-        List[str]
-            The alias and connection string for each connection.
+        List[Dict[str, str]]
+            list of dictionaries describing files.
+            Each entry has key/values for:
+            - file_type
+            - file_path
+            - relative_path
+            - qry_path
 
         """
-        add_connections = [
-            f"{alias}: {driver.current_connection}"
-            for alias, driver in self._additional_connections.items()
-        ]
-        return [f"Default: {self._query_provider.current_connection}", *add_connections]
+        if not self._rel_file_paths:
+            for file in self.files:
+                f_path = file.get("link")
+                if not f_path:
+                    continue
+                f_rel_path = f_path.replace(DS_PREFIX, "")
+                query_path = ".".join(Path(f_rel_path).parts).replace(
+                    Path(f_rel_path).suffix, ""
+                )
+                self._rel_file_paths.append(
+                    {
+                        "file_type": file.get("type"),
+                        "file_path": f_path,
+                        "relative_path": f_rel_path,
+                        "qry_path": query_path,
+                    }
+                )
+        return self._rel_file_paths
 
-    def query_help(self, query_name: str):
-        """
-        Print help for `query_name`.
 
-        Parameters
-        ----------
-        query_name : str
-            The name of the query.
+# pylint: disable=not-an-iterable, no-member
 
-        """
-        self.query_store[query_name].help()
 
-    def get_query(self, query_name: str) -> str:
-        """
-        Return the raw query text for `query_name`.
+def get_mdr_data_paths(item_type="metadata") -> Generator[str, None, None]:
+    """
+    Generate Mordor data sets from GitHub repo.
 
-        Parameters
-        ----------
-        query_name : str
-            The name of the query.
+    Parameters
+    ----------
+    item_type : str, optional
+        The type of item required, by default "metadata"
+        Other values are "large", "small.
+
+    Yields
+    ------
+    str
+        Iterable of paths
 
-        """
-        return self.query_store[query_name].query
+    """
+    md_tree = _GET_MORDOR_TREE(_MORDOR_TREE_URI)
+    yield from (
+        t_item["path"]
+        for t_item in md_tree.get("tree")
+        if t_item["type"] == "blob"
+        and t_item["path"].startswith("datasets")
+        and item_type in t_item["path"]
+    )
 
-    def exec_query(self, query: str, **kwargs) -> Union[pd.DataFrame, Any]:
-        """
-        Execute simple query string.
 
-        Parameters
-        ----------
-        query : str
-            [description]
-        use_connections : Union[str, List[str]]
+def _get_mdr_github_tree():
+    """Closure to wrap fetching Mordor tree from GitHub."""
+    mordor_tree = None
 
-        Other Parameters
-        ----------------
-        query_options : Dict[str, Any]
-            Additional options passed to query driver.
-        kwargs : Dict[str, Any]
-            Additional options passed to query driver.
+    def _get_mdr_tree(uri):
+        nonlocal mordor_tree
+        if mordor_tree is None:
+            resp = httpx.get(uri, timeout=_HTTP_TIMEOUT, headers=mp_ua_header())
+            mordor_tree = resp.json()
+        return mordor_tree
 
-        Returns
-        -------
-        Union[pd.DataFrame, Any]
-            Query results - a DataFrame if successful
-            or a KqlResult if unsuccessful.
+    return _get_mdr_tree
 
-        """
-        query_options = kwargs.pop("query_options", {}) or kwargs
-        query_source = kwargs.pop("query_source", None)
-        result = self._query_provider.query(
-            query, query_source=query_source, **query_options
-        )
-        if not self._additional_connections:
-            return result
-        # run query against all connections
-        results = [result]
-        print(f"Running query for {len(self._additional_connections)} connections.")
-        for con_name, connection in self._additional_connections.items():
-            print(f"{con_name}...")
-            try:
-                results.append(
-                    connection.query(query, query_source=query_source, **query_options)
-                )
-            except MsticpyDataQueryError:
-                print(f"Query {con_name} failed.")
-        return pd.concat(results)
 
-    def browse_queries(self, **kwargs):
-        """
-        Return QueryProvider query browser.
+# Create closure
+_GET_MORDOR_TREE = _get_mdr_github_tree()
 
-        Other Parameters
-        ----------------
-        kwargs :
-            passed to SelectItem constructor.
 
-        Returns
-        -------
-        SelectItem
-            SelectItem browser for TI Data.
+def _get_mdr_file(gh_file):
+    """Fetch a file from Mordor repo."""
+    file_blob_uri = (
+        f"https://raw.githubusercontent.com/OTRF/Security-Datasets/master/{gh_file}"
+    )
+    file_resp = httpx.get(file_blob_uri, timeout=_HTTP_TIMEOUT, headers=mp_ua_header())
+    return file_resp.content
 
-        """
-        # pylint: disable=import-outside-toplevel
-        from ...vis.query_browser import browse_queries
 
-        return browse_queries(self, **kwargs)
+def _create_mdr_metadata_cache():
+    md_metadata: Dict[str, MordorEntry] = {}
 
-    # alias for browse_queries
-    browse = browse_queries
+    def _get_mdr_metadata(cache_folder: Optional[str] = None):
+        nonlocal md_metadata
+        if not md_metadata:
+            md_metadata = _fetch_mdr_metadata(cache_folder=cache_folder)
+        return md_metadata
 
-    @property
-    def query_time(self):
-        """Return the default QueryTime control for queries."""
-        return self._query_time
+    return _get_mdr_metadata
 
-    def add_custom_query(
-        self,
-        name: str,
-        query: str,
-        family: Union[str, Iterable[str]],
-        description: Optional[str] = None,
-        parameters: Optional[Iterable[QueryParam]] = None,
-    ):
-        """
-        Add a custom function to the provider.
 
-        Parameters
-        ----------
-        name : str
-            The name of the query.
-        query : str
-            The query text (optionally parameterized).
-        family : Union[str, Iterable[str]]
-            The query group/family or list of families. The query will
-            be added to attributes of the query provider with these
-            names.
-        description : Optional[str], optional
-            Optional description (for query help), by default None
-        parameters : Optional[Iterable[QueryParam]], optional
-            Optional list of parameter definitions, by default None.
-            If the query is parameterized you must supply definitions
-            for the parameters here - at least name and type.
-            Parameters can be the named tuple QueryParam (also
-            exposed as QueryProvider.Param) or a 4-value
-
-        Examples
-        --------
-        >>> qp = QueryProvider("MSSentinel")
-        >>> qp_host = qp.create_paramramram("host_name", "str", "Name of Host")
-        >>> qp_start = qp.create_param("start", "datetime")
-        >>> qp_end = qp.create_param("end", "datetime")
-        >>> qp_evt = qp.create_param("event_id", "int", None, 4688)
-        >>>
-        >>> query = '''
-        >>> SecurityEvent
-        >>> | where EventID == {event_id}
-        >>> | where TimeGenerated between (datetime({start}) .. datetime({end}))
-        >>> | where Computer has "{host_name}"
-        >>> '''
-        >>>
-        >>> qp.add_custom_query(
-        >>>     name="test_host_proc",
-        >>>     query=query,
-        >>>     family="Custom",
-        >>>     parameters=[qp_host, qp_start, qp_end, qp_evt]
-        >>> )
-
-        """
-        if parameters:
-            param_dict = {
-                param[0]: {
-                    "type": param[1],
-                    "default": param[2],
-                    "description": param[3],
-                }
-                for param in parameters
-            }
-        else:
-            param_dict = {}
-        source = {
-            "args": {"query": query},
-            "description": description,
-            "parameters": param_dict,
-        }
-        metadata = {"data_families": [family] if isinstance(family, str) else family}
-        query_source = QuerySource(
-            name=name, source=source, defaults={}, metadata=metadata
-        )
-        self.query_store.add_data_source(query_source)
-        self._add_query_functions()
+# Create closure
+_GET_MORDOR_METADATA = _create_mdr_metadata_cache()
 
-    def _execute_query(self, *args, **kwargs) -> Union[pd.DataFrame, Any]:
-        if not self._query_provider.loaded:
-            raise ValueError("Provider is not loaded.")
-        if (
-            not self._query_provider.connected
-            and not _help_flag(*args)
-            and not _debug_flag(*args, **kwargs)
-        ):
-            raise ValueError(
-                "No connection to a data source.",
-                "Please call connect(connection_str) and retry.",
-            )
-        query_name = kwargs.pop("query_name")
-        family = kwargs.pop("query_path")
+_LAST_UPDATE_KEY = "mp_last_updated"
+_DEFAULT_TS = pd.Timestamp(pd.Timestamp.utcnow() - pd.Timedelta(days=60))
 
-        query_source = self.query_store.get_query(
-            query_path=family, query_name=query_name
-        )
-        if _help_flag(*args):
-            query_source.help()
-            return None
-
-        params, missing = extract_query_params(query_source, *args, **kwargs)
-        self._check_for_time_params(params, missing)
-        if missing:
-            query_source.help()
-            raise ValueError(f"No values found for these parameters: {missing}")
-
-        split_by = kwargs.pop("split_query_by", None)
-        if split_by:
-            split_result = self._exec_split_query(
-                split_by=split_by,
-                query_source=query_source,
-                query_params=params,
-                args=args,
-                **kwargs,
-            )
-            if split_result is not None:
-                return split_result
-            # if split queries could not be created, fall back to default
-        query_str = query_source.create_query(
-            formatters=self._query_provider.formatters, **params
-        )
-        # This looks for any of the "print query" debug args in args or kwargs
-        if _debug_flag(*args, **kwargs):
-            return query_str
-
-        # Handle any query options passed
-        query_options = _get_query_options(params, kwargs)
-        return self.exec_query(query_str, query_source=query_source, **query_options)
-
-    def _check_for_time_params(self, params, missing):
-        """Fall back on builtin query time if no time parameters were supplied."""
-        if "start" in missing:
-            missing.remove("start")
-            params["start"] = self._query_time.start
-        if "end" in missing:
-            missing.remove("end")
-            params["end"] = self._query_time.end
-
-    def _get_query_folder_for_env(self, root_path: str, environment: str) -> List[Path]:
-        """Return query folder for current environment."""
-        data_envs = [environment]
-        if environment.casefold() in _COMPATIBLE_DRIVER_MAPPINGS:
-            data_envs += _COMPATIBLE_DRIVER_MAPPINGS[environment.casefold()]
-        return [
-            _resolve_package_path(root_path).joinpath(data_env.casefold())
-            for data_env in data_envs
-        ]
 
-    def _read_queries_from_paths(self, query_paths) -> Dict[str, QueryStore]:
-        """Fetch queries from YAML files in specified paths."""
-        settings: Dict[str, Any] = get_config("QueryDefinitions", {})
-        all_query_paths: List[Union[Path, str]] = []
-        for def_qry_path in settings.get("Default"):  # type: ignore
-            # only read queries from environment folder
-            builtin_qry_paths = self._get_query_folder_for_env(
-                def_qry_path, self.environment
-            )
-            all_query_paths.extend(
-                str(qry_path) for qry_path in builtin_qry_paths if qry_path.is_dir()
-            )
+# pylint: disable=global-statement
+def _fetch_mdr_metadata(cache_folder: Optional[str] = None) -> Dict[str, MordorEntry]:
+    """
+    Return full metadata for Mordor datasets.
 
-        if settings.get("Custom") is not None:
-            for custom_path in settings.get("Custom"):  # type: ignore
-                custom_qry_path = _resolve_path(custom_path)
-                if custom_qry_path:
-                    all_query_paths.append(custom_qry_path)
-        if query_paths:
-            for param_path in query_paths:
-                param_qry_path = _resolve_path(param_path)
-                if param_qry_path:
-                    all_query_paths.append(param_qry_path)
-        if all_query_paths:
-            return QueryStore.import_files(
-                source_path=all_query_paths,
-                recursive=True,
-                driver_query_filter=self._query_provider.query_attach_spec,
-            )
-        # if no queries - just return an empty store
-        return {self.environment: QueryStore(self.environment)}
+    Parameters
+    ----------
+    cache_folder : Optional[str]
+        Folder to search for mordor cache, by default None
+
+    Returns
+    -------
+    Dict[str, MordorEntry]:
+        Mordor data set metadata keyed by MordorID
 
-    def _add_query_functions(self):
-        """Add queries to the module as callable methods."""
-        for qual_query_name in self.list_queries():
-            query_path = qual_query_name.split(".")
-            query_name = query_path[-1]
-            current_node = self
-            for container_name in query_path[:-1]:
-                container_name = valid_pyname(container_name)
-                if hasattr(current_node, container_name):
-                    current_node = getattr(current_node, container_name)
-                else:
-                    new_node = QueryContainer()
-                    setattr(current_node, container_name, new_node)
-                    current_node = new_node
-
-            query_cont_name = ".".join(query_path[:-1])
-
-            # Create the partial function
-            query_func = partial(
-                self._execute_query, query_path=query_cont_name, query_name=query_name
-            )
-            query_func.__doc__ = self.query_store.get_query(
-                query_path=query_cont_name, query_name=query_name
-            ).create_doc_string()
-
-            query_name = valid_pyname(query_name)
-            setattr(current_node, query_name, query_func)
-            setattr(self.all_queries, query_name, query_func)
-
-    def _add_driver_queries(self, queries: Iterable[Dict[str, str]]):
-        """Add driver queries to the query store."""
-        for query in queries:
-            self.query_store.add_query(
-                name=query["name"],
-                query=query["query"],
-                query_paths=query["query_container"],
-                description=query["description"],
-            )
-        # For now, just add all of the functions again (with any connect-time acquired
-        # queries) - we could be more efficient than this but unless there are 1000s of
-        # queries it should not be noticeable.
-        self._add_query_functions()
+    """
+    global MITRE_TECHNIQUES, MITRE_TACTICS
 
-    def _exec_split_query(
-        self,
-        split_by: str,
-        query_source: QuerySource,
-        query_params: Dict[str, Any],
-        args,
-        **kwargs,
-    ) -> Union[pd.DataFrame, str, None]:
-        start = query_params.pop("start", None)
-        end = query_params.pop("end", None)
-        if not (start or end):
-            print(
-                "Cannot split a query that does not have 'start' and 'end' parameters"
+    if MITRE_TECHNIQUES is None or MITRE_TACTICS is None:
+        MITRE_TECHNIQUES, MITRE_TACTICS = _get_mitre_categories()
+    md_metadata: Dict[str, MordorEntry] = {}
+
+    md_cached_metadata = _read_mordor_cache(cache_folder)
+    mdr_md_paths = list(get_mdr_data_paths("metadata"))
+    for filename in tqdm(
+        mdr_md_paths, unit=" files", desc="Downloading Mordor metadata"
+    ):
+        cache_valid = False
+        if filename in md_cached_metadata:
+            metadata_doc = md_cached_metadata[filename]
+            last_timestamp = pd.Timestamp(
+                metadata_doc.get(_LAST_UPDATE_KEY, _DEFAULT_TS)
             )
-            return None
+            cache_valid = (pd.Timestamp.utcnow() - last_timestamp).days < 30
+
+        if not cache_valid:
+            gh_file_content = _get_mdr_file(filename)
+            try:
+                metadata_doc = yaml.safe_load(gh_file_content)
+            except yaml.error.YAMLError:
+                continue
+            metadata_doc[_LAST_UPDATE_KEY] = pd.Timestamp.utcnow().isoformat()
+            md_cached_metadata[filename] = metadata_doc
+        doc_id = metadata_doc.get("id")
+        mdr_entry = metadata_doc.copy()
+        mdr_entry.pop(_LAST_UPDATE_KEY, None)
+        md_metadata[doc_id] = MordorEntry(**mdr_entry)
+
+    _write_mordor_cache(md_cached_metadata, cache_folder)
+    return md_metadata
+
+
+# pylint: enable=global-statement
+
+
+def _read_mordor_cache(cache_folder) -> Dict[str, Any]:
+    """Return dictionary of cached metadata if cached_folder is a valid path."""
+    md_cached_metadata: Dict[str, Any] = {}
+    mordor_cache = Path(cache_folder).joinpath(_MORDOR_CACHE)
+    if _valid_cache(mordor_cache):
         try:
-            split_delta = pd.Timedelta(split_by)
-        except ValueError:
-            split_delta = pd.Timedelta("1D")
-
-        ranges = _calc_split_ranges(start, end, split_delta)
-
-        split_queries = [
-            query_source.create_query(
-                formatters=self._query_provider.formatters,
-                start=q_start,
-                end=q_end,
-                **query_params,
-            )
-            for q_start, q_end in ranges
-        ]
-        # This looks for any of the "print query" debug args in args or kwargs
-        if _debug_flag(*args, **kwargs):
-            return "\n\n".join(split_queries)
-
-        # Retrieve any query options passed (other than query params)
-        # and send to query function.
-        query_options = _get_query_options(query_params, kwargs)
-        query_dfs = [
-            self.exec_query(query_str, query_source=query_source, **query_options)
-            for query_str in tqdm(split_queries, unit="sub-queries", desc="Running")
-        ]
+            md_json = Path(mordor_cache).read_text(encoding="utf-8")
+            md_cached_metadata = json.loads(md_json)
+        except json.JSONDecodeError:
+            pass
+    return md_cached_metadata
+
+
+def _write_mordor_cache(md_cached_metadata, cache_folder):
+    """Write dictionary of cached metadata if cached_folder is a valid path."""
+    mordor_cache = Path(cache_folder).joinpath(_MORDOR_CACHE)
+    json_text = json.dumps(md_cached_metadata, indent=4)
+    Path(mordor_cache).write_text(json_text, encoding="utf-8")
+
+
+def _build_mdr_indexes(
+    mdr_metadata: Dict[str, MordorEntry]
+) -> Tuple[Dict[str, Set[str]], Dict[str, Set[str]]]:
+    """
+    Return dictionaries mapping Mitre items to Mordor datasets.
+
+    Parameters
+    ----------
+    mdr_metadata : Dict[str, MordorEntry]
+        Dictionary of mordor dataset metadata.
+
+    Returns
+    -------
+    Tuple[Dict[str, Set[str]], Dict[str, Set[str]]]
+        Mordor dataset IDs keyed by Mitre Technique and Mitre Tactic.
 
-        return pd.concat(query_dfs)
+    """
+    md_idx_techniques = defaultdict(set)
+    md_idx_tactics = defaultdict(set)
+
+    for md_id, md_file in mdr_metadata.items():
+        for attack in md_file.get_attacks():
+            md_idx_techniques[attack.technique].add(md_id)
+            if not attack.tactics:
+                continue
+            for tactic in attack.tactics:
+                md_idx_tactics[tactic].add(md_id)
+
+    return md_idx_techniques, md_idx_tactics  # type: ignore
+
+
+def download_mdr_file(
+    file_uri: str, use_cached: bool = True, save_folder: str = ".", silent: bool = False
+) -> pd.DataFrame:
+    """
+    Download data file from Mordor.
 
+    Parameters
+    ----------
+    file_uri : str
+        The URI of the file to download.
+    use_cached : bool, optional
+        Try to use locally saved file first, by default True
+    save_folder : str, optional
+        Path to output folder, by default "."
+    silent : bool
+        If True, suppress feedback. By default, False.
+
+    Returns
+    -------
+    pd.DataFrame
+        DataFrame of Dataset
 
-def _calc_split_ranges(start: datetime, end: datetime, split_delta: pd.Timedelta):
-    """Return a list of time ranges split by `split_delta`."""
-    # Use pandas date_range and split the result into 2 iterables
-    s_ranges, e_ranges = tee(pd.date_range(start, end, freq=split_delta))
-    next(e_ranges, None)  # skip to the next item in the 2nd iterable
-    # Zip them together to get a list of (start, end) tuples of ranges
-    # Note: we subtract 1 nanosecond from the 'end' value of each range so
-    # to avoid getting duplicated records at the boundaries of the ranges.
-    # Some providers don't have nanosecond granularity so we might
-    # get duplicates in these cases
-    ranges = [
-        (s_time, e_time - pd.Timedelta("1ns"))
-        for s_time, e_time in zip(s_ranges, e_ranges)
-    ]
+    """
+    if not silent:
+        print(file_uri)
+    if not file_uri.lower().endswith("zip"):
+        raise TypeError(f"File type not supported {file_uri}")
+    if not Path(save_folder).is_dir():
+        Path(save_folder).mkdir(parents=True, exist_ok=True)
+    save_path = "-".join(Path(file_uri.replace(DS_PREFIX, "")).parts)
+    save_file = Path(save_folder).joinpath(save_path)
+    if not use_cached or not save_file.is_file():
+        # streamed download
+        with open(str(save_file), "wb") as fdesc:
+            with httpx.stream(
+                "GET", file_uri, timeout=_HTTP_TIMEOUT, headers=mp_ua_header()
+            ) as resp:
+                for chunk in resp.iter_bytes(chunk_size=1024):
+                    fdesc.write(chunk)
+
+    try:
+        with zipfile.ZipFile(str(save_file)) as zip_file:
+            file_names = zip_file.namelist()
+            d_frames = {
+                file_name: _extract_zip_file_to_df(
+                    zip_file, file_name, use_cached, save_folder, silent
+                )
+                for file_name in file_names
+            }
+            return pd.concat(d_frames.values())
+    except BadZipFile as bad_zip_err:
+        raise MsticpyUserError(
+            f"Could not extract zip file for {file_uri}.",
+            "File does not exist or is corrupt.",
+            title="Mordor download error",
+            help_uri="https://msticpy.readthedocs.io/en/latest/data_acquisition/MordorData.html",
+        ) from bad_zip_err
+
+
+def _extract_zip_file_to_df(  # noqa: MC0001
+    zip_file: ZipFile,
+    file_name: str,
+    use_cached: bool = True,
+    save_folder: str = ".",
+    silent: bool = False,
+) -> pd.DataFrame:
+    """
+    Extract from zip and parse json file to DataFrame.
+
+    Parameters
+    ----------
+    zip_file : ZipFile
+        ZipFile object containing the file
+    file_name : str
+        File name to extract
+    use_cached : bool, optional
+        Try to use locally saved file first, by default True
+    save_folder : str, optional
+        Path to output folder, by default "."
+    silent : bool
+        If False, suppress feedback. By default, True.
+
+    Returns
+    -------
+    pd.DataFrame
+        Extracted DataFrame
+
+    """
+    if not silent:
+        print("Extracting", file_name)
+
+    file_path = Path(save_folder).joinpath(file_name)
+    if not use_cached or not file_path.is_file():
+        zip_file.extract(file_name, path=save_folder)
+
+    out_df = pd.DataFrame()
+    if file_path.suffix.lower() == ".json":
+        out_df = pd.read_json(file_path, lines=True)
+    if file_path.suffix.lower() == ".csv":
+        out_df = pd.read_csv(file_path)
+    if file_path.suffix.lower() not in (".json", ".csv"):
+        print(f"Cannot process files of type {file_path.suffix.lower()}")
+    if not use_cached:
+        Path(file_name).unlink()
+    return out_df
+
+
+def search_mdr_data(
+    mdr_data: Dict[str, MordorEntry], terms: str = None, subset: Iterable[str] = None
+) -> Set[str]:
+    """
+    Return IDs for items matching terms.
 
-    # Since the generated time ranges are based on deltas from 'start'
-    # we need to adjust the end time on the final range.
-    # If the difference between the calculated last range end and
-    # the query 'end' that the user requested is small (< 10% of a delta),
-    # we just replace the last "end" time with our query end time.
-    if (ranges[-1][1] - end) < (split_delta / 10):
-        ranges[-1] = ranges[-1][0], end
+    Parameters
+    ----------
+    mdr_data : Dict[str, MordorEntry]
+        Mordor dataset
+    terms : str, optional
+        Search terms, by default None
+        (comma-separated values are treated as OR terms
+        plus-separated values are treated as AND terms)
+    subset : Iterable[str], optional
+        A subset of IDs over which to search, by default None
+
+    Returns
+    -------
+    Set[str]
+        The set of matching IDs.
+
+    """
+    if terms is None:
+        return set(subset or mdr_data.keys())
+    logic = "OR"
+    if "," in terms:
+        search_terms = terms.split(",")
+    elif "+" in terms:
+        search_terms = terms.split("+")
+        logic = "AND"
     else:
-        # otherwise append a new range starting after the last range
-        # in ranges and ending in 'end"
-        # note - we need to add back our subtracted 1 nanosecond
-        ranges.append((ranges[-1][0] + pd.Timedelta("1ns"), end))
-    return ranges
+        search_terms = [terms]
+    results: Set[str] = set()
+    for search_idx, term in enumerate(search_terms):
+        item_results = set()
+        for md_id, item in mdr_data.items():
+            if subset is not None and md_id not in subset:
+                continue
+            if term.strip() in str(item):
+                item_results.add(md_id)
+        if logic == "OR":
+            results = results | item_results
+        else:
+            # Don't AND if search_idx == 0 (and-ing against empty results)
+            results = results & item_results if search_idx else item_results
+    return results
+
+
+def _extract_mitre_refs(ext_refs):
+    ref_dict = [
+        ref
+        for ref in ext_refs
+        if "source_name" in ref and ref["source_name"] == "mitre-attack"
+    ]
+    if ref_dict:
+        return ref_dict[0]
+    return {}
 
 
-def _resolve_package_path(config_path: str) -> Path:
-    """Resolve path relative to current package."""
+def _reshape_mitre_df(data):
+    col_rename = {"external_id": "ID", "name": "Name", "description": "Description"}
     return (
-        Path(config_path)
-        if Path(config_path).is_absolute()
-        else Path(__file__).resolve().parent.parent.joinpath(config_path)
+        data.join(
+            data.apply(
+                lambda x: _extract_mitre_refs(x.external_references),
+                axis=1,
+                result_type="expand",
+            )
+        )
+        .assign(MitreGroup="Enterprise")[["external_id", "name", "description", "url"]]
+        .rename(columns=col_rename)
+        .sort_values("ID")
+        .set_index("ID")
     )
 
 
-def _resolve_path(config_path: str) -> Optional[str]:
-    """Resolve path."""
-    if not Path(config_path).is_absolute():
-        config_path = str(Path(config_path).expanduser().resolve())
-    if not Path(config_path).is_dir():
-        print(f"Warning: Custom query definitions path {config_path} not found")
-        return None
-    return config_path
-
-
-def _help_flag(*args) -> bool:
-    """Return True if help parameter passed."""
-    return any(help_flag for help_flag in _HELP_FLAGS if help_flag in args)
-
-
-def _debug_flag(*args, **kwargs) -> bool:
-    """Return True if debug/print args passed."""
-    return any(db_arg for db_arg in _DEBUG_FLAGS if db_arg in args) or any(
-        db_arg for db_arg in _DEBUG_FLAGS if kwargs.get(db_arg, False)
-    )
+def _get_mitre_categories(
+    cache_folder: Optional[str] = None,
+) -> Tuple[pd.DataFrame, pd.DataFrame]:
+    """
+    Download and return Mitre techniques and tactics.
 
+    Parameters
+    ----------
+    cache_folder : Optional[str]
+        Folder to search for mordor cache, by default None
+
+    Returns
+    -------
+    Tuple[pd.DataFrame, pd.DataFrame]
+        Tuple of techniques, tactics with IDs, names,
+        descriptions.
 
-def _get_query_options(
-    params: Dict[str, Any], kwargs: Dict[str, Any]
-) -> Dict[str, Any]:
-    # sourcery skip: inline-immediately-returned-variable, use-or-for-fallback
-    """Return any kwargs not already in params."""
-    query_options = kwargs.pop("query_options", {})
-    if not query_options:
-        # Any kwargs left over we send to the query provider driver
-        query_options = {key: val for key, val in kwargs.items() if key not in params}
-    return query_options
-
-
-def _normalize_to_regex(
-    search_term: Union[str, Iterable[str], None], ignore_case: bool
-) -> List[Pattern[str]]:
-    """Return iterable or str search term as list of compiled reg expressions."""
-    if not search_term:
-        return []
-    regex_opts = [re.IGNORECASE] if ignore_case else []
-    if isinstance(search_term, str):
-        return [re.compile(search_term, *regex_opts)]
-    if isinstance(search_term, abc.Iterable):
-        return [re.compile(term, *regex_opts) for term in set(search_term)]
-    return []
+    """
+    if cache_folder:
+        tech_cache = Path(cache_folder).joinpath(_MITRE_TECH_CACHE)
+        tactics_cache = Path(cache_folder).joinpath(_MITRE_TACTICS_CACHE)
+        if _valid_cache(tech_cache) and _valid_cache(tactics_cache):
+            try:
+                # caching location only used if sepcified.
+                tech_df = pd.read_pickle(tech_cache)  # nosec
+                tactics_df = pd.read_pickle(tactics_cache)  # nosec
+                return tech_df, tactics_df
+            except pickle.PickleError:
+                pass
+    resp = httpx.get(_MITRE_JSON_URL, timeout=_HTTP_TIMEOUT, headers=mp_ua_header())
+    mitre = pd.json_normalize(resp.json()["objects"])
+
+    # remove deprecated items
+    mitre["x_mitre_deprecated"].fillna(False, inplace=True)
+    mitre = mitre[~(mitre["x_mitre_deprecated"])]
+
+    tech_df = _reshape_mitre_df(mitre[mitre.type == "attack-pattern"])
+    tactics_df = _reshape_mitre_df(mitre[mitre.type == "x-mitre-tactic"])
+    if cache_folder:
+        tech_df.to_pickle(tech_cache)
+        tactics_df.to_pickle(tactics_cache)
+
+    return tech_df, tactics_df
+
+
+def _valid_cache(path: Path, expired_days=30):
+    """Return True if the file exists and is younger than `expired_days`."""
+    if not path.is_file():
+        return False
+    days_old = (datetime.now() - datetime.fromtimestamp(path.stat().st_mtime)).days
+    return days_old < expired_days
```

### Comparing `msticpy-2.4.0/msticpy/data/core/data_query_reader.py` & `msticpy-2.5.0/msticpy/data/core/data_query_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/core/param_extractor.py` & `msticpy-2.5.0/msticpy/data/core/param_extractor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/core/query_container.py` & `msticpy-2.5.0/msticpy/data/core/query_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/core/query_defns.py` & `msticpy-2.5.0/msticpy/data/core/query_defns.py`

 * *Files 9% similar despite different names*

```diff
@@ -101,14 +101,17 @@
     OTRF = 8
     Mordor = 8
     ResourceGraph = 9
     Sumologic = 10
     M365D = 11
     Cybereason = 12
     Elastic = 14
+    OSQueryLogs = 15
+    MSSentinel_New = 16
+    Kusto_New = 17
 
     @classmethod
     def parse(cls, value: Union[str, int]) -> "DataEnvironment":
         """
         Convert string or int to enum.
 
         Parameters
```

### Comparing `msticpy-2.4.0/msticpy/data/core/query_source.py` & `msticpy-2.5.0/msticpy/data/core/query_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,42 +83,32 @@
 
         Notes
         -----
         A data source can belong to multiple families (e.g. a query
         that joins data from several sources)
 
         """
+        self.show = True
         self.name = name
         self._source: Dict[str, Any] = source or {}
         self.defaults: Dict[str, Any] = defaults or {}
         self._global_metadata: Dict[str, Any] = dict(metadata) if metadata else {}
         self.query_store: Optional["QueryStore"] = None  # type: ignore  # noqa: F821
 
-        # consolidate source metadata - source-specifc
+        # consolidate source metadata - source-specific
         # overrides global
         # add an empty dict in case neither has defined params
-        # self.metadata = ChainMap(
-        #     _value_or_default(self._source, "metadata", {}),
-        #     _value_or_default(self.defaults, "metadata", {}),
-        #     self._global_metadata,
-        # )
         self.metadata = collapse_dicts(
             self._global_metadata,
             self.defaults.get("metadata", {}),
             self._source.get("metadata", {}),
         )
         # make ChainMap for parameters from with source
         # higher priority than default
         # add an empty dict in case neither has defined params
-        # self.params = ChainMap(
-        #     _value_or_default(self._source, "parameters", {}),
-        #     _value_or_default(self.defaults, "parameters", {}),
-        #     # self._source.get("parameters", {}),
-        #     # self.defaults.get("parameters", {}),
-        # )
         self.params = collapse_dicts(
             self.defaults.get("parameters", {}),
             self._source.get("parameters", {}),
         )
 
         self._query: str = self["args.query"]
         self._replace_query_macros()
```

### Comparing `msticpy-2.4.0/msticpy/data/core/query_store.py` & `msticpy-2.5.0/msticpy/data/core/query_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """QueryStore class - holds a collection of QuerySources."""
 from collections import defaultdict
 from functools import cached_property
 from os import path
-from typing import Any, Dict, Iterable, List, Optional, Set, Union
+from typing import Any, Callable, Dict, Iterable, List, Optional, Set, Union
 
 from ..._version import VERSION
 from ...common.exceptions import MsticpyUserConfigError
 from .data_query_reader import find_yaml_files, read_query_def_file
 from .query_defns import DataEnvironment, DataFamily
 from .query_source import QuerySource
 
@@ -75,14 +75,15 @@
         environment : str
             The data environment
 
         """
         self.environment: str = environment
         self.data_families: Dict[str, Dict[str, QuerySource]] = defaultdict(dict)
         self.data_family_defaults: Dict[str, Dict[str, Any]] = defaultdict(dict)
+        self._all_sources: List[QuerySource] = []
 
     def __getattr__(self, name: str):
         """Return the item in dot-separated path `name`."""
         return _get_dot_path(elem_path=name, data_map=self.data_families)
 
     def __getitem__(self, key: str):
         """Allow query retrieval using dotted key path."""
@@ -98,15 +99,16 @@
         Iterable[str]
             List of queries
 
         """
         for family in sorted(self.data_families):
             yield from [
                 f"{family}.{query}"
-                for query in sorted(self.data_families[family].keys())
+                for query, query_source in sorted(self.data_families[family].items())
+                if query_source.show
             ]
 
     @cached_property
     def search_items(self) -> Dict[str, Dict[str, str]]:
         """Return searchable metadata and query for all queries."""
         search_props: Dict[str, Dict[str, str]] = {}
         for family, sources in self.data_families.items():
@@ -128,14 +130,15 @@
         ----------
         source : QuerySource
             The source to add. An existing item with
             the same name will be overwritten
 
         """
         source.query_store = self
+        self._all_sources.append(source)
         for family in source.data_families:
             self.data_families[family][source.name] = source
             # we want to update any new defaults for the data family
             self.data_family_defaults[family].update(source.defaults)
 
             # we also replace the defaults dict in each source with
             # a reference to the data family defaults so that as
@@ -214,14 +217,29 @@
         """
         sources, defaults, metadata = read_query_def_file(query_file)
 
         for source_name, source in sources.items():
             new_source = QuerySource(source_name, source, defaults, metadata)
             self.add_data_source(new_source)
 
+    def apply_query_filter(self, query_filter: Callable[[QuerySource], bool]):
+        """
+        Apply a filter to the query sources.
+
+        Parameters
+        ----------
+        query_filter : Callable[[bool], QuerySource]
+            A function that takes a QuerySource and returns True
+            if the query should be displayed.
+
+        """
+        for source in self._all_sources:
+            source.show = query_filter(source)
+
+    # pylint: disable=too-many-locals
     @classmethod  # noqa: MC0001
     def import_files(  # noqa: MC0001
         cls,
         source_path: list,
         recursive: bool = True,
         driver_query_filter: Optional[Dict[str, Set[str]]] = None,
     ) -> Dict[str, "QueryStore"]:
@@ -266,28 +284,31 @@
                     )
                     continue
 
                 for env_value in metadata["data_environments"]:
                     if "." in env_value:
                         env_value = env_value.split(".")[1]
                     environment = DataEnvironment.parse(env_value)
-                    if environment == DataEnvironment.Unknown:
-                        raise ValueError(f"Unknown environment {env_value}")
+                    environment_name = (
+                        environment.name
+                        if environment != DataEnvironment.Unknown
+                        else env_value
+                    )
 
-                    if environment.name not in env_stores:
-                        env_stores[environment.name] = cls(environment=environment.name)
+                    if environment_name not in env_stores:
+                        env_stores[environment_name] = cls(environment=environment_name)
                     for source_name, source in sources.items():
                         new_source = QuerySource(
                             source_name, source, defaults, metadata
                         )
                         if not driver_query_filter or (
                             driver_query_filter
                             and _matches_driver_filter(new_source, driver_query_filter)
                         ):
-                            env_stores[environment.name].add_data_source(new_source)
+                            env_stores[environment_name].add_data_source(new_source)
         return env_stores
 
     def get_query(
         self, query_name: str, query_path: Union[str, DataFamily] = None
     ) -> "QuerySource":
         """
         Return query with name `data_family` and `query_name`.
```

### Comparing `msticpy-2.4.0/msticpy/data/data_obfus.py` & `msticpy-2.5.0/msticpy/data/data_obfus.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/data_providers.py` & `msticpy-2.5.0/msticpy/data/data_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/drivers/__init__.py` & `msticpy-2.5.0/msticpy/data/drivers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Data provider sub-package."""
 import importlib
-from typing import Union
+from functools import singledispatch
+from typing import Dict, Union
 
 from ..._version import VERSION
 from ..core.query_defns import DataEnvironment
 
 # flake8: noqa: F403
 from .driver_base import DriverBase
 
@@ -19,32 +20,60 @@
     DataEnvironment.LogAnalytics: ("kql_driver", "KqlDriver"),
     DataEnvironment.AzureSecurityCenter: ("kql_driver", "KqlDriver"),
     DataEnvironment.SecurityGraph: ("security_graph_driver", "SecurityGraphDriver"),
     DataEnvironment.Kusto: ("kusto_driver", "KustoDriver"),
     DataEnvironment.MDATP: ("mdatp_driver", "MDATPDriver"),
     DataEnvironment.MDE: ("mdatp_driver", "MDATPDriver"),
     DataEnvironment.LocalData: ("local_data_driver", "LocalDataDriver"),
+    DataEnvironment.OSQueryLogs: ("local_osquery_driver", "OSQueryLogDriver"),
     DataEnvironment.Splunk: ("splunk_driver", "SplunkDriver"),
     DataEnvironment.Mordor: ("mordor_driver", "MordorDriver"),
     DataEnvironment.Sumologic: ("sumologic_driver", "SumologicDriver"),
     DataEnvironment.ResourceGraph: ("resource_graph_driver", "ResourceGraphDriver"),
     DataEnvironment.M365D: ("mdatp_driver", "MDATPDriver"),
     DataEnvironment.Cybereason: ("cybereason_driver", "CybereasonDriver"),
     DataEnvironment.Elastic: ("elastic_driver", "ElasticDriver"),
+    DataEnvironment.MSSentinel_New: ("azure_monitor_driver", "AzureMonitorDriver"),
+    DataEnvironment.Kusto_New: ("azure_kusto_driver", "AzureKustoDriver"),
 }
 
+CUSTOM_PROVIDERS: Dict[str, type] = {}
 
-def import_driver(data_environment: DataEnvironment) -> type:
+
+@singledispatch
+def import_driver(data_environment) -> type:
+    """Unsupported type for environment."""
+    raise TypeError(
+        "'data_environment' must be a str or DataEnvironment type.",
+        f"Called with type: {type(data_environment)}",
+    )
+
+
+@import_driver.register
+def _(data_environment: DataEnvironment) -> type:
     """Import driver class for a data environment."""
     mod_name, cls_name = _ENVIRONMENT_DRIVERS.get(data_environment, (None, None))
 
     if not (mod_name and cls_name):
         raise ValueError(
             f"No driver available for environment {data_environment.name}.",
             "Possible values are:",
             ", ".join(env.name for env in _ENVIRONMENT_DRIVERS),
         )
 
     imp_module = importlib.import_module(
         f"msticpy.data.drivers.{mod_name}", package="msticpy"
     )
     return getattr(imp_module, cls_name)
+
+
+@import_driver.register
+def _(data_environment: str) -> type:
+    """Import custom driver class for a data environment."""
+    if plugin_cls := CUSTOM_PROVIDERS.get(data_environment):
+        return plugin_cls
+
+    raise ValueError(
+        f"No driver available for environment {data_environment}.",
+        "Possible values are:",
+        ", ".join(CUSTOM_PROVIDERS),
+    )
```

### Comparing `msticpy-2.4.0/msticpy/data/drivers/cybereason_driver.py` & `msticpy-2.5.0/msticpy/data/drivers/cybereason_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import pandas as pd
 
 from ..._version import VERSION
 from ...common.exceptions import MsticpyUserConfigError
 from ...common.provider_settings import ProviderArgs, get_provider_settings
 from ...common.utility import mp_ua_header
 from ..core.query_defns import Formatters
-from .driver_base import DriverBase, QuerySource
+from .driver_base import DriverBase, DriverProps, QuerySource
 
 __version__ = VERSION
 __author__ = "Florian Bracq"
 
 _HELP_URI = (
     "https://msticpy.readthedocs.io/en/latest/data_acquisition/DataProviders.html"
 )
@@ -83,19 +83,22 @@
         self.search_endpoint: str = "/rest/visualsearch/query/simple"
         self._loaded = True
         self.client = httpx.Client(
             follow_redirects=True,
             timeout=self.get_http_timeout(timeout=timeout, def_timeout=120),
             headers=mp_ua_header(),
         )
-        self.formatters = {
-            Formatters.PARAM_HANDLER: self._custom_param_handler,
-            Formatters.DATETIME: self._format_datetime,
-            Formatters.LIST: self._format_list,
-        }
+        self.set_driver_property(
+            DriverProps.FORMATTERS,
+            {
+                Formatters.PARAM_HANDLER: self._custom_param_handler,
+                Formatters.DATETIME: self._format_datetime,
+                Formatters.LIST: self._format_list,
+            },
+        )
 
         self._debug = kwargs.get("debug", False)
 
     def query(
         self, query: str, query_source: QuerySource = None, **kwargs
     ) -> Union[pd.DataFrame, Any]:
         """
```

### Comparing `msticpy-2.4.0/msticpy/data/drivers/driver_base.py` & `msticpy-2.5.0/msticpy/data/drivers/driver_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,46 +3,110 @@
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Data driver base class."""
 import abc
 from abc import ABC
 from collections import defaultdict
-from typing import Any, Callable, Dict, Iterable, Optional, Set, Tuple, Union
+from typing import Any, Dict, Iterable, Optional, Set, Tuple, Union
 
 import pandas as pd
 
 from ..._version import VERSION
 from ...common.exceptions import MsticpyNotConnectedError
 from ...common.pkg_config import get_http_timeout
 from ...common.provider_settings import ProviderSettings, get_provider_settings
+from ..core.query_defns import DataEnvironment
 from ..core.query_source import QuerySource
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 
+class DriverProps:
+    """Defined driver properties."""
+
+    PUBLIC_ATTRS = "public_attribs"
+    FORMATTERS = "formatters"
+    USE_QUERY_PATHS = "use_query_paths"
+    HAS_DRIVER_QUERIES = "has_driver_queries"
+    EFFECTIVE_ENV = "effective_environment"
+    SUPPORTS_THREADING = "supports_threading"
+    SUPPORTS_ASYNC = "supports_async"
+    MAX_PARALLEL = "max_parallel"
+    FILTER_ON_CONNECT = "filter_queries_on_connect"
+
+    PROPERTY_TYPES: Dict[str, Any] = {
+        PUBLIC_ATTRS: dict,
+        FORMATTERS: dict,
+        USE_QUERY_PATHS: bool,
+        HAS_DRIVER_QUERIES: bool,
+        EFFECTIVE_ENV: (str, DataEnvironment),
+        SUPPORTS_THREADING: bool,
+        SUPPORTS_ASYNC: bool,
+        MAX_PARALLEL: int,
+        FILTER_ON_CONNECT: bool,
+    }
+
+    @classmethod
+    def defaults(cls):
+        """Return default values for driver properties."""
+        return {
+            cls.PUBLIC_ATTRS: {},
+            cls.FORMATTERS: {},
+            cls.USE_QUERY_PATHS: True,
+            cls.HAS_DRIVER_QUERIES: False,
+            cls.EFFECTIVE_ENV: None,
+            cls.SUPPORTS_THREADING: False,
+            cls.SUPPORTS_ASYNC: False,
+            cls.MAX_PARALLEL: 4,
+            cls.FILTER_ON_CONNECT: False,
+        }
+
+    @classmethod
+    def valid_type(cls, property_name: str, value: Any) -> bool:
+        """Return expected property type."""
+        if property_name not in cls.PROPERTY_TYPES:
+            return True
+        return isinstance(value, cls.PROPERTY_TYPES[property_name])
+
+
 # pylint: disable=too-many-instance-attributes
 class DriverBase(ABC):
     """Base class for data providers."""
 
     def __init__(self, **kwargs):
         """Initialize new instance."""
         self._kwargs = kwargs
         self._loaded = False
         self._connected = False
         self.current_connection = None
-        self.public_attribs: Dict[str, Any] = {}
-        self.formatters: Dict[str, Callable] = {}
-        self.use_query_paths = True
-        self.has_driver_queries = False
+        # self.public_attribs: Dict[str, Any] = {}
+        # self.formatters: Dict[str, Callable] = {}
+        # self.use_query_paths = True
+        # self.has_driver_queries = False
         self._previous_connection = False
         self.data_environment = kwargs.get("data_environment")
         self._query_filter: Dict[str, Set[str]] = defaultdict(set)
         self._instance: Optional[str] = None
+        self.properties = DriverProps.defaults()
+        self.set_driver_property(
+            name=DriverProps.EFFECTIVE_ENV,
+            value=(
+                self.data_environment.name
+                if isinstance(self.data_environment, DataEnvironment)
+                else self.data_environment or ""
+            ),
+        )
+
+    def __getattr__(self, attrib):
+        """Return item from the properties dictionary as an attribute."""
+        if attrib in self.properties:
+            return self.properties[attrib]
+        raise AttributeError(f"{self.__class__.__name__} has no attribute '{attrib}'")
 
     @property
     def loaded(self) -> bool:
         """
         Return true if the provider is loaded.
 
         Returns
@@ -115,15 +179,15 @@
             Connect to a data source
 
         """
         return None
 
     @abc.abstractmethod
     def query(
-        self, query: str, query_source: QuerySource = None, **kwargs
+        self, query: str, query_source: Optional[QuerySource] = None, **kwargs
     ) -> Union[pd.DataFrame, Any]:
         """
         Execute query string and return DataFrame of results.
 
         Parameters
         ----------
         query : str
@@ -136,15 +200,15 @@
         kwargs :
             Are passed to the underlying provider query method,
             if supported.
 
         Returns
         -------
         Union[pd.DataFrame, Any]
-            A DataFrame (if successfull) or
+            A DataFrame (if successful) or
             the underlying provider result if an error.
 
         """
 
     @abc.abstractmethod
     def query_with_results(self, query: str, **kwargs) -> Tuple[pd.DataFrame, Any]:
         """
@@ -191,23 +255,44 @@
         return [{}]
 
     @property
     def query_attach_spec(self) -> Dict[str, Set[str]]:
         """Parameters that determine whether a query is relevant for the driver."""
         return self._query_filter
 
-    def add_query_filter(self, name, query_filter):
+    def add_query_filter(self, name: str, query_filter: Union[str, Iterable]):
         """Add an expression to the query attach filter."""
         allowed_names = {"data_environments", "data_families", "data_sources"}
         if name not in allowed_names:
             raise ValueError(
                 f"'name' {name} must be one of:",
                 ", ".join(f"'{name}'" for name in allowed_names),
             )
-        self._query_filter[name].add(query_filter)
+        if isinstance(query_filter, str):
+            self._query_filter[name].add(query_filter)
+        else:
+            self._query_filter[name].update(query_filter)
+
+    def set_driver_property(self, name: str, value: Any):
+        """Set an item in driver properties."""
+        if not DriverProps.valid_type(name, value):
+            raise TypeError(
+                f"Property '{name}' is not the correct type.",
+                f"Expected: '{DriverProps.PROPERTY_TYPES[name]}'.",
+            )
+        self.properties[name] = value
+
+    def get_driver_property(self, name: str) -> Any:
+        """Return value or KeyError from driver properties."""
+        return self.properties[name]
+
+    def query_usable(self, query_source: QuerySource) -> bool:
+        """Return True if query should be exposed for this driver."""
+        del query_source
+        return True
 
     # Read values from configuration
     @staticmethod
     def _get_config_settings(prov_name) -> Dict[Any, Any]:
         """Get config from msticpyconfig."""
         data_provs = get_provider_settings(config_section="DataProviders")
         splunk_settings: Optional[ProviderSettings] = data_provs.get(prov_name)
```

### Comparing `msticpy-2.4.0/msticpy/data/drivers/elastic_driver.py` & `msticpy-2.5.0/msticpy/data/drivers/elastic_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import pandas as pd
 
 from ..._version import VERSION
 from ...common.exceptions import MsticpyUserConfigError
 from ...common.utility import check_kwargs, export
 from ..core.query_defns import Formatters
-from .driver_base import DriverBase, QuerySource
+from .driver_base import DriverBase, DriverProps, QuerySource
 
 __version__ = VERSION
 __author__ = "Neil Desai, Ian Hellen"
 
 
 ELASTIC_CONNECT_ARGS: Dict[str, str] = {
     # TBD - you may not need these - mainly for user
@@ -38,19 +38,22 @@
         """Instantiate Elastic Driver."""
         super().__init__(**kwargs)
         self.service = None
         self._loaded = True
         self._connected = False
         self._debug = kwargs.get("debug", False)
 
-        self.formatters = {
-            Formatters.PARAM_HANDLER: self._custom_param_handler,
-            Formatters.DATETIME: self._format_datetime,
-            Formatters.LIST: self._format_list,
-        }
+        self.set_driver_property(
+            DriverProps.FORMATTERS,
+            {
+                Formatters.PARAM_HANDLER: self._custom_param_handler,
+                Formatters.DATETIME: self._format_datetime,
+                Formatters.LIST: self._format_list,
+            },
+        )
 
     def connect(self, connection_str: str = None, **kwargs):
         """
         Connect to Elastic cluster.
 
         Parameters
         ----------
```

### Comparing `msticpy-2.4.0/msticpy/data/drivers/kql_driver.py` & `msticpy-2.5.0/msticpy/data/drivers/kql_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     MsticpyKqlConnectionError,
     MsticpyNoDataSourceError,
     MsticpyNotConnectedError,
 )
 from ...common.utility import MSTICPY_USER_AGENT, export
 from ...common.wsconfig import WorkspaceConfig
 from ..core.query_defns import DataEnvironment
-from .driver_base import DriverBase, QuerySource
+from .driver_base import DriverBase, DriverProps, QuerySource
 
 _KQL_ENV_OPTS = "KQLMAGIC_CONFIGURATION"
 
 
 # Need to set KQL option before importing
 def _set_kql_env_option(option, value):
     """Set an item in the KqlMagic main config environment variable."""
@@ -114,15 +114,18 @@
             print out additional diagnostic information.
 
         """
         self._ip = get_ipython()
         self._debug = kwargs.get("debug", False)
         super().__init__(**kwargs)
 
-        self.formatters = {"datetime": self._format_datetime, "list": self._format_list}
+        self.set_driver_property(
+            DriverProps.FORMATTERS,
+            {"datetime": self._format_datetime, "list": self._format_list},
+        )
         self._loaded = self._is_kqlmagic_loaded()
 
         os.environ["KQLMAGIC_LOAD_MODE"] = "silent"
         if not self._loaded:
             self._load_kql_magic()
 
         self._set_kql_option("request_user_agent_tag", MSTICPY_USER_AGENT)
```

### Comparing `msticpy-2.4.0/msticpy/data/drivers/kusto_driver.py` & `msticpy-2.5.0/msticpy/data/drivers/kusto_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             alias for `db`
         connection_str : str, Optional
 
 
         Returns
         -------
         Union[pd.DataFrame, results.ResultSet]
-            A DataFrame (if successfull) or
+            A DataFrame (if successful) or
             the underlying provider result if an error.
 
         """
         new_connection = self._get_connection_string(
             query_source=query_source, **kwargs
         )
         if new_connection:
@@ -210,20 +210,20 @@
         if cluster_key not in self._kusto_settings:
             raise MsticpyUserConfigError(
                 f"The cluster {cluster} was not found in the configuration.",
                 "You must have an entry for the cluster in the 'DataProviders section",
                 "of your msticyconfig.yaml",
                 "Expected format:",
                 "Kusto[-instance_name]:",
-                "  args:",
+                "  Args:",
                 "    Cluster: cluster_uri",
                 "    Integrated: True",
                 "or",
                 "Kusto[-instance_name]:",
-                "  args:",
+                "  Args:",
                 "    Cluster: cluster_uri",
                 "    TenantId: tenant_uuid",
                 "    ClientId: tenant_uuid",
                 "    ClientSecret: (string|KeyVault|EnvironmentVar:)",
                 title="Unknown cluster.",
             )
         return self._format_connection_str(cluster, database)
```

### Comparing `msticpy-2.4.0/msticpy/data/drivers/local_data_driver.py` & `msticpy-2.5.0/msticpy/data/drivers/local_data_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/drivers/mdatp_driver.py` & `msticpy-2.5.0/msticpy/data/drivers/mdatp_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,15 @@
         self.cloud = cs_dict.pop("cloud", "global")
         if "cloud" in kwargs and kwargs["cloud"]:
             self.cloud = kwargs["cloud"]
 
         api_uri, oauth_uri, api_suffix = _select_api_uris(
             self.data_environment, self.cloud
         )
-        self.add_query_filter("data_environments", "MDE")
-        self.add_query_filter("data_environments", "M365D")
-        self.add_query_filter("data_environments", "MDATP")
+        self.add_query_filter("data_environments", ("MDE", "M365D", "MDATP"))
 
         self.req_body = {
             "client_id": None,
             "client_secret": None,
             "grant_type": "client_credentials",
             "resource": api_uri,
         }
```

### Comparing `msticpy-2.4.0/msticpy/data/drivers/mordor_driver.py` & `msticpy-2.5.0/msticpy/vis/foliummap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,933 +1,1058 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-"""Mordor/OTRF Security datasets driver."""
-import json
-import pickle  # nosec
-import zipfile
-from collections import defaultdict
-from datetime import datetime
-from pathlib import Path
-from typing import Any, Dict, Generator, Iterable, List, Optional, Set, Tuple, Union
-from zipfile import BadZipFile, ZipFile
+"""Folium map class."""
 
-import attr
-import httpx
+import contextlib
+import itertools
+import math
+import statistics as stats
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generator,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+    Union,
+)
+
+import folium
 import pandas as pd
-import yaml
-from tqdm.auto import tqdm
+from folium.plugins import FeatureGroupSubGroup, MarkerCluster
+
+from .._version import VERSION
+from ..common.exceptions import MsticpyMissingDependencyError
+from ..common.utility import export
+from ..datamodel.entities import Entity, GeoLocation, IpAddress
+
+from ..context.geoip import GeoLiteLookup  # isort: skip
+
+try:
+    import pygeohash
+except ImportError:
+    pygeohash = None  # pylint: disable=invalid-name
 
-from ..._version import VERSION
-from ...common.exceptions import MsticpyUserError
-from ...common.pkg_config import get_config
-from ...common.utility import mp_ua_header
-from ..core.query_source import QuerySource
-from .driver_base import DriverBase
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
+_GEO_LITE = GeoLiteLookup()
 
-_MORDOR_TREE_URI = (
-    "https://api.github.com/repos/OTRF/Security-Datasets/git/trees/master?recursive=1"
-)
 
-_MITRE_JSON_URL = (
-    "https://raw.githubusercontent.com/mitre/cti/"
-    "master/enterprise-attack/enterprise-attack.json"
-)
-_MTR_TAC_CAT_URI = "https://attack.mitre.org/tactics/{cat}/"
-_MTR_TECH_CAT_URI = "https://attack.mitre.org/techniques/{cat}/"
-
-MITRE_TECHNIQUES: pd.DataFrame = None
-MITRE_TACTICS: pd.DataFrame = None
+# pylint: disable=too-many-lines
+@export
+class FoliumMap:
+    """Wrapper class for Folium/Leaflet mapping."""
 
-_MITRE_TECH_CACHE = "mitre_tech_cache.pkl"
-_MITRE_TACTICS_CACHE = "mitre_tact_cache.pkl"
-_MORDOR_CACHE = "mordor_cache.json"
-
-_HTTP_TIMEOUT = DriverBase.get_http_timeout()
-
-
-# pylint: disable=too-many-instance-attributes
-class MordorDriver(DriverBase):
-    """Mordor data driver."""
-
-    def __init__(self, **kwargs):
-        """Initialize the Mordor driver."""
-        super().__init__(**kwargs)
-        self.use_query_paths = False
-        self.has_driver_queries = True
-        self.mitre_techniques: pd.DataFrame
-        self.mitre_tactics: pd.DataFrame
-        self.mordor_data: Dict[str, MordorEntry]
-        self.mdr_idx_tech: Dict[str, Set[str]]
-        self.mdr_idx_tact: Dict[str, Set[str]]
-        self._driver_queries: List[Dict[str, Any]] = []
-
-        mdr_settings = get_config("DataProviders.Mordor", {})
-        self.use_cached = kwargs.pop(
-            "used_cached", mdr_settings.get("used_cached", True)
-        )
-        self.save_folder = kwargs.pop(
-            "save_folder", mdr_settings.get("save_folder", ".")
-        )
-        self.save_folder = _resolve_cache_folder(self.save_folder)
-        self.silent = kwargs.pop("silent", False)
+    def __init__(
+        self,
+        title: str = "OpenStreetMap",
+        zoom_start: float = 2.5,
+        tiles=None,
+        width: str = "100%",
+        height: str = "100%",
+        location: list = None,
+    ):
+        """
+        Create an instance of the folium map.
 
-        self._loaded = True
+        Parameters
+        ----------
+        title : str, optional
+            Name of the main tile layer (the default is 'OpenStreetMap')
+        zoom_start : int, optional
+            The zoom level of the map (the default is 7)
+        tiles : [type], optional
+            Custom set of tiles or tile URL (the default is None)
+        width : str, optional
+            Map display width (the default is '100%')
+        height : str, optional
+            Map display height (the default is '100%')
+        location : list, optional
+            Location to center map on
 
-    # pylint: disable=global-statement
+        Attributes
+        ----------
+        folium_map : folium.Map
+            The map object.
 
-    def connect(self, connection_str: Optional[str] = None, **kwargs):
         """
-        Connect to data source.
+        if not location:
+            location = [47.67, -122.13]
 
-        Parameters
-        ----------
-        connection_str : Optional[str]
-            Connect to a data source
+        self.folium_map = folium.Map(
+            zoom_start=zoom_start,
+            tiles=tiles,
+            width=width,
+            height=height,
+            location=location,
+            control_scale=True,
+        )
+        folium.TileLayer(name=title).add_to(self.folium_map)
+        self.locations: List[Tuple[float, float]] = []
 
+    def _repr_html_(self):
+        """Return folium map as HTML."""
+        # pylint: disable=protected-access
+        return self.folium_map._repr_html_()
+        # pylint: enable=protected-access
+
+    def center_map(self):
+        """Calculate and set map center based on current coordinates."""
+        self.folium_map.location = _get_center_coords(self.locations)
+
+    def add_ip_cluster(
+        self, ip_entities: Iterable[IpAddress], layer: Optional[str] = None, **kwargs
+    ):
         """
-        global MITRE_TECHNIQUES, MITRE_TACTICS
-        cache_folder = self.save_folder if self.use_cached else None
-        print("Retrieving Mitre data...")
+        Add a collection of IP Entities to the map.
 
-        if MITRE_TECHNIQUES is None or MITRE_TACTICS is None:
-            MITRE_TECHNIQUES, MITRE_TACTICS = _get_mitre_categories(
-                cache_folder=cache_folder
-            )
-        self.mitre_techniques = MITRE_TECHNIQUES
-        self.mitre_tactics = MITRE_TACTICS
+        Parameters
+        ----------
+        ip_entities : Iterable[IpAddress]
+            a iterable of IpAddress Entities
+        layer : str, optional
+            If not none, it will add the entities to a new layer.
 
-        print("Retrieving Mordor data...")
+        Other Parameters
+        ----------------
+        kwargs: icon properties to use for displaying this cluster
 
-        self.mordor_data = _GET_MORDOR_METADATA(cache_folder=cache_folder)
-        self.mdr_idx_tech, self.mdr_idx_tact = _build_mdr_indexes(self.mordor_data)
+        """
+        ip_entities = _get_location_for_ip_entities(ip_entities)
 
-        self._connected = True
-        self.public_attribs = {
-            "mitre_techniques": self.mitre_techniques,
-            "mitre_tactics": self.mitre_tactics,
-            "driver_queries": self.driver_queries,
-            "search_queries": self.search_queries,
-        }
+        if layer:
+            marker_target = folium.FeatureGroup(name=layer)
+            marker_target.add_to(self.folium_map)
+            folium.LayerControl().add_to(self.folium_map)
+        else:
+            marker_target = self.folium_map
+        for ip_entity in ip_entities:
+            if ip_entity.Location is None:
+                continue
+            if (
+                not (
+                    isinstance(ip_entity.Location.Latitude, (int, float))
+                    and isinstance(ip_entity.Location.Longitude, (int, float))
+                )
+                or math.isnan(ip_entity.Location.Latitude)
+                or math.isnan(ip_entity.Location.Longitude)
+            ):
+                continue
+            popup_text = _get_popup_text(ip_entity)
+            tooltip_text = _get_tooltip_text(ip_entity)
 
-    # pylint: enable=global-statement
+            marker = folium.Marker(
+                location=[ip_entity.Location.Latitude, ip_entity.Location.Longitude],
+                popup=popup_text,
+                tooltip=tooltip_text,
+                icon=folium.Icon(**kwargs),
+            )
+            marker.add_to(marker_target)
+            self.locations.append(
+                (ip_entity.Location.Latitude, ip_entity.Location.Longitude)
+            )
 
-    def query(
-        self, query: str, query_source: QuerySource = None, **kwargs
-    ) -> Union[pd.DataFrame, Any]:
+    def add_ips(self, ip_addresses: Iterable[str], **kwargs):
         """
-        Execute query string and return DataFrame of results.
+        Add a collection of GeoLocation objects to the map.
 
         Parameters
         ----------
-        query : str
-            The query to execute
-        query_source : QuerySource
-            The query definition object
+        ip_addresses : Iterable[str]
+            Iterable of ip strings.
+        layer : str, optional
+            If not none, it will add the entities to a new layer.
 
         Other Parameters
         ----------------
-        kwargs :
-            Are passed to the underlying provider query method,
-            if supported.
+        kwargs: icon properties to use for displaying this cluster
 
-        Returns
-        -------
-        Union[pd.DataFrame, Any]
-            A DataFrame (if successfull) or
-            the underlying provider result if an error.
-
-        """
-        del query_source
-        if not self._connected:
-            raise self._create_not_connected_err("OTRF Datasets")
-        use_cached = kwargs.pop("used_cached", self.use_cached)
-        save_folder = kwargs.pop("save_folder", self.save_folder)
-        save_folder = _resolve_cache_folder(save_folder)
-        silent = kwargs.pop("silent", self.silent)
-        result_df = download_mdr_file(
-            file_uri=query,
-            use_cached=use_cached,
-            save_folder=save_folder,
-            silent=silent,
-        )
-        if not isinstance(result_df, pd.DataFrame) or result_df.empty:
-            return "Could not convert result to a DataFrame."
-        return result_df
+        """
+        _, ip_entities = _GEO_LITE.lookup_ip(ip_addr_list=ip_addresses)
+        self.add_ip_cluster(ip_entities=ip_entities, **kwargs)
 
-    def query_with_results(self, query: str, **kwargs) -> Tuple[pd.DataFrame, Any]:
+    def add_geoloc_cluster(self, geo_locations: Iterable[GeoLocation], **kwargs):
         """
-        Execute query string and return DataFrame plus native results.
+        Add a collection of GeoLocation objects to the map.
 
         Parameters
         ----------
-        query : str
-            The query to execute
+        geo_locations : Iterable[GeoLocation]
+            Iterable of GeoLocation entities.
+        layer : str, optional
+            If not none, it will add the entities to a new layer.
 
-        Returns
-        -------
-        Tuple[pd.DataFrame,Any]
-            A DataFrame and native results.
+        Other Parameters
+        ----------------
+        kwargs: icon properties to use for displaying this cluster
 
         """
-        result = self.query(query, **kwargs)
-        if isinstance(result, pd.DataFrame):
-            return result, "OK"
-        return pd.DataFrame, result
-
-    @property
-    def driver_queries(self) -> Iterable[Dict[str, Any]]:
-        """
-        Return generator of Mordor query definitions.
-
-        Yields
-        ------
-        Iterable[Dict[str, Any]]
-            Iterable of Dictionaries containing query definitions.
-
-        """
-        if not self._connected:
-            raise self._create_not_connected_err("OTRF Datasets")
-        if not self._driver_queries:
-            self._driver_queries = list(self._get_driver_queries())
-        return self._driver_queries
-
-    def _get_driver_queries(self):
-        """Generate iterable of Mordor queries."""
-        for mdr_item in self.mordor_data.values():
-            for file_path in mdr_item.get_file_paths():
-                mitre_data = mdr_item.get_attacks()
-                techniques = ", ".join(
-                    f"{att.technique}: {att.technique_name}" for att in mitre_data
-                )
-
-                tactics = ", ".join(
-                    f"{tac[0]}: {tac[1]}"
-                    for att in mitre_data
-                    for tac in att.tactics_full
-                )
+        ip_entities = [IpAddress(Address="na", Location=geo) for geo in geo_locations]
+        self.add_ip_cluster(ip_entities=ip_entities, **kwargs)
 
-                doc_string: List[str] = [
-                    f"{mdr_item.title}",
-                    "",
-                    "Notes",
-                    "-----",
-                    f"Mordor ID: {mdr_item.id}",
-                    mdr_item.description or "",
-                    "",
-                    f"Mitre Techniques: {techniques}",
-                    f"Mitre Tactics: {tactics}",
-                ]
-                q_container, _, full_name = file_path["qry_path"].partition(".")
-                short_name = file_path["qry_path"].split(".")[-1]
-                yield {
-                    "name": full_name,
-                    "description": "\n".join(doc_string),
-                    "query_name": short_name,
-                    "query": file_path["file_path"],
-                    "query_container": q_container,
-                    "metadata": {},
-                }
-
-    def search_queries(self, search: str) -> Iterable[str]:
+    def add_locations(self, locations: Iterable[Tuple[float, float]], **kwargs):
         """
-        Search queries for matching attributes.
+        Add a collection of lat/long tuples to the map.
 
         Parameters
         ----------
-        search : str
-            Search string. Substrings separated by commas will
-            be treated as OR terms - e.g. "a, b" == "a" or "b".
-            Substrings separated by "+" will be treated as AND
-            terms - e.g. "a + b" == "a" and "b"
+        locations : Iterable[Tuple[float, float]]
+            Iterable of location tuples.
+        layer : str, optional
+            If not none, it will add the entities to a new layer.
 
-        Returns
-        -------
-        Iterable[str]
-            Iterable of matching query names.
+        Other Parameters
+        ----------------
+        kwargs: icon properties to use for displaying this cluster
 
+        """
+        geo_entities = [
+            GeoLocation(Latitude=lat, Longitude=long) for lat, long in locations
+        ]
+        self.add_geoloc_cluster(geo_locations=geo_entities, **kwargs)
 
+    def add_geo_hashes(self, geohashes: Iterable[str], **kwargs):
         """
-        if not self._connected:
-            raise self._create_not_connected_err("OTRF Datasets")
-        matches = []
-        for mdr_id in search_mdr_data(self.mordor_data, terms=search):
-            for file_path in self.mordor_data[mdr_id].get_file_paths():
-                matches.append(
-                    f"{file_path['qry_path']} ({self.mordor_data[mdr_id].title})"
-                )
-        return matches
+        Add decoded geohashes to the map.
 
+        Parameters
+        ----------
+        geohashes : Iterable[str]
+            Iterable of geolocation hashes
+        layer : str, optional
+            If not none, it will add the entities to a new layer.
 
-def _resolve_cache_folder(cache_path: str):
-    """Expand and optionally creates cache folder."""
-    cache_folder = Path(cache_path).expanduser()
-    if not cache_folder.is_dir():
-        cache_folder.mkdir(parents=True, exist_ok=True)
-    return str(cache_folder)
+        Other Parameters
+        ----------------
+        kwargs: icon properties to use for displaying this cluster
 
+        """
+        geo_entities = []
+        for geohash in geohashes:
+            decoded_location = decode_geo_hash(geohash)
+            geo_entities.append(
+                GeoLocation(Latitude=decoded_location[0], Longitude=decoded_location[1])
+            )
 
-# pylint: enable=too-many-instance-attributes
+        self.add_geoloc_cluster(geo_locations=geo_entities, **kwargs)
 
+    def add_marker_clusters(self, clusters: Iterable[MarkerCluster]):
+        """
+        Add MarkerClusters and to the map.
 
-class MitreAttack:
-    """MitreAttack container for techniques and tactics."""
+        Parameters
+        ----------
+        clusters: Iterable[MarkerCluster]
+            Iterable of MarkerClusters
 
-    MTR_TECH_URI = "https://attack.mitre.org/techniques/{technique_id}/"
-    MTR_TAC_URI = "https://attack.mitre.org/tactics/{tactic_id}/"
+        """
+        for cluster in clusters:
+            self.folium_map.add_child(cluster)
 
-    def __init__(
-        self,
-        attack: Dict[str, Any] = None,
-        technique: str = None,
-        sub_technique: str = None,
-        tactics: List[str] = None,
-    ):
+    def add_feature_sub_groups(self, subgroups: Iterable[FeatureGroupSubGroup]):
         """
-        Create instance of MitreAttack.
+        Add FeatureGroupSubGroups and to the map.
 
         Parameters
         ----------
-        attack : Dict[str, Any], optional
-            attack data as dictionary, by default None
-        technique : str, optional
-            technique ID, by default None
-        sub_technique : str, optional
-            sub-technique ID, by default None
-        tactics : List[str], optional
-            List of associated tactics, by default None
+        subgroups: Iterable[FeatureGroupSubGroup]
+            Iterable of FeatureGroupSubGroups
 
         """
-        if attack is None and (technique is None and tactics is None):
-            raise TypeError(
-                "Either 'attack' or 'technique' and 'tactics' must be specified."
-            )
-        self.technique = attack.get("technique") if attack else technique
-        self.sub_technique = attack.get("sub-technique") if attack else sub_technique
-        self.tactics = attack.get("tactics") if attack else tactics  # type: ignore
-
-        self._technique_name = None
-        self._technique_desc = None
-        self._technique_uri = None
-        self._tactics_full: List[Tuple[str, str, str, str]] = []
+        for subgroup in subgroups:
+            self.folium_map.add_child(subgroup)
 
-    def __repr__(self) -> str:
+    def save_map(self, path: str):
         """
-        Return repr of MitreAttack object.
+        Save the map to `path`.
 
-        Returns
-        -------
-        str
-            The repr of the object.
+        Parameters
+        ----------
+        path: str
+            File path to save the current map
 
         """
-        return "".join(
-            [
-                f"MitreAttack(technique={self.technique}), ",
-                f"sub_technique={self.sub_technique}, ",
-                f"tactics={repr(self.tactics)}",
-            ]
-        )
+        self.folium_map.save(path)
 
-    @property
-    def technique_name(self) -> Optional[str]:
+    def add_locations_to_feature_subgroup(
+        self,
+        locations: Iterable[Tuple[float, float]],
+        subgroup: FeatureGroupSubGroup,
+        **kwargs,
+    ):
         """
-        Return Mitre Technique full name.
+        Create markers from locations and add the FeatureGroupSubGroup.
 
-        Returns
-        -------
-        Optional[str]
-            Name of the Mitre technique
+        Parameters
+        ----------
+        locations: Iterable[Tuple[float, float]]
+            Collection of Latitude/Longitude coordinates to be added
+            to the FeatureGroupSubGroup
+        subgroup: FeatureGroupSubGroup
+            Subgroup to add locations to, then add to the map
 
         """
-        if not self._technique_name and self.technique in MITRE_TECHNIQUES.index:
-            self._technique_name = MITRE_TECHNIQUES.loc[self.technique].Name
-        return self._technique_name
+        for point in locations:
+            marker = self.create_marker(location=point, **kwargs)
+            marker.add_to(subgroup)
+            self.locations.append(point)
 
-    @property
-    def technique_desc(self) -> Optional[str]:
-        """
-        Return Mitre technique description.
+        subgroups = [subgroup]
 
-        Returns
-        -------
-        Optional[str]
-            Technique description
+        self.add_feature_sub_groups(subgroups)
 
+    def add_locations_to_marker_cluster(
+        self, locations: Iterable[Tuple[float, float]], cluster: MarkerCluster, **kwargs
+    ):
         """
-        if not self._technique_desc and self.technique in MITRE_TECHNIQUES.index:
-            self._technique_desc = MITRE_TECHNIQUES.loc[self.technique].Description
-        return self._technique_desc
+        Create markers from locations and add to MarkerCluster.
+
+        Parameters
+        ----------
+        locations: Iterable[Tuple[float, float]]
+            Collection of Latitude/Longitude coordinates to be added
+            to the MarkerCluster
+        cluster: MarkerCluster
+            Marker cluster to add locations to, then add to the map
 
-    @property
-    def technique_uri(self) -> str:
         """
-        Return Mitre Technique URI.
+        for point in locations:
+            marker = self.create_marker(location=point, **kwargs)
+            marker.add_to(cluster)
+            self.locations.append(point)
 
-        Returns
-        -------
-        Optional[str]
-            URI of the Mitre technique
+        clusters = [cluster]
 
-        """
-        return self.MTR_TECH_URI.format(technique_id=self.technique)
+        self.add_marker_clusters(clusters)
 
-    @property
-    def tactics_full(self) -> List[Tuple[str, str, str, str]]:
+    def create_new_cluster_with_locations(
+        self, locations: Iterable[Tuple[float, float]], name: str, **kwargs
+    ):
         """
-        Return full listing of Mitre tactics.
+        Create a MarkerCluster with locations.
 
-        Returns
-        -------
-        List[Tuple[str, str, str, str]]
-            List of tuples of:
-            (ID, Name, Description, URI)
+        Parameters
+        ----------
+        locations: Iterable[Tuple[float, float]]
+            Collection of Latitude/Longitude coordinates to be added to the
+            MarkerCluster
+        name: str
+            Name of Marker Cluster to create, add locations to,
+            then add to the map
 
         """
-        if not self._tactics_full and self.tactics:
-            for tactic in self.tactics:
-                tactic_name = tactic_desc = "unknown"
-                if tactic in MITRE_TACTICS.index:
-                    tactic_name = MITRE_TACTICS.loc[tactic].Name
-                    tactic_desc = MITRE_TACTICS.loc[tactic].Description
-                tactic_uri = self.MTR_TAC_URI.format(tactic_id=tactic)
-                self._tactics_full.append(
-                    (tactic, tactic_name, tactic_desc, tactic_uri)
-                )
-        return self._tactics_full
+        marker_cluster = MarkerCluster(name=name)
 
+        self.add_locations_to_marker_cluster(
+            locations=locations, cluster=marker_cluster, **kwargs
+        )
 
-def _to_datetime(date_val) -> datetime:
-    """
-    Return datetime from parsed date string.
+    def create_new_subgroup_with_locations(
+        self,
+        locations: Iterable[Tuple[float, float]],
+        subgroup_name: str,
+        cluster_name: str,
+        **kwargs,
+    ):
+        """
+        Create subgroup of markers from locations.
 
-    Parameters
-    ----------
-    date_val : datetime
-        The datetime or datetime string.
+        Parameters
+        ----------
+        locations: Iterable[Tuple[float, float]]
+            Collection of Latitude/Longitude coordinates to be added
+            to the FeatureGroupSubGroup
+        subgroup_name: str
+            Name of FeatureGroupSubGroup to create, add locations to,
+            then add to the map
+        cluster_name : str
+            Name of the cluster
+
+        Notes
+        -----
+        This function creates a marker cluster and FeatureGroupSubGroup,
+        then add the locations to the subgroup, then add the subgroup to the map.
 
-    Returns
-    -------
-    datetime
-        Parse datetime.
+        """
+        marker_cluster = MarkerCluster(name=cluster_name)
+        feature_subgroup = FeatureGroupSubGroup(marker_cluster, name=subgroup_name)
 
-    """
-    if isinstance(date_val, datetime):
-        return date_val
-    try:
-        return pd.to_datetime(date_val)
-    except TypeError:
-        return datetime.min
+        self.add_locations_to_feature_subgroup(
+            locations=locations, subgroup=feature_subgroup, **kwargs
+        )
 
+    def enable_layer_control(self):
+        """
+        Enable Layer Control on the map.
 
-DS_PREFIX = "https://raw.githubusercontent.com/OTRF/Security-Datasets/master/datasets/"
+        Parameters
+        ----------
+        None
 
+        """
+        folium.LayerControl().add_to(self.folium_map)
 
-# pylint: disable=not-an-iterable, no-member
+    def create_new_cluster_with_geohashes(
+        self, geohashes: Iterable[str], name: str, **kwargs
+    ):
+        """
+        Create a MarkerCluster and add geohash locations.
 
+        Parameters
+        ----------
+        geohashes: Iterable[str]
+            Collection of geohashes to be decoded and added to the MarkerCluster
+        name: str
+            Name of Marker Cluster to create, add locations to, then add to the map
 
-@attr.s(auto_attribs=True)
-class MordorEntry:
-    """Mordor data set metadata."""
+        """
+        locations = decode_geohash_collection(geohashes)
+        self.create_new_cluster_with_locations(locations=locations, name=name, **kwargs)
 
-    title: str
-    id: str
-    type: str
-    creation_date: datetime = attr.ib(converter=_to_datetime)
-    modification_date: datetime = attr.ib(converter=_to_datetime)
-    contributors: List[str] = attr.Factory(list)
-    author: Optional[str] = None
-    platform: Optional[str] = None
-    description: Optional[str] = None
-    tags: List[str] = attr.Factory(list)
-    files: List[Dict[str, Any]] = attr.Factory(list)
-    datasets: List[Dict[str, Any]] = attr.Factory(list)
-    attack_mappings: List[Dict[str, Any]] = attr.Factory(list)
-    notebooks: List[Dict[str, str]] = attr.Factory(list)
-    simulation: Dict[str, Any] = attr.Factory(dict)
-    references: List[Any] = attr.Factory(list)
-    _rel_file_paths: List[Dict[str, Any]] = attr.Factory(list)
+    def create_new_subgroup_with_geohashes(
+        self, geohashes: Iterable[str], subgroup_name: str, cluster_name: str, **kwargs
+    ):
+        """
+        Create a FeatureSubGroup with collection of geohash locations.
 
-    def get_notebooks(self) -> List[Tuple[str, str, str]]:
+        Parameters
+        ----------
+        geohashes: Iterable[str]
+            Collection of geohashes to be decoded and added to
+            the FeatureGroupSubGroup
+        subgroup_name: str
+            Name of SubGroup to create, add locations to, then add to the map
+        cluster_name: str
+            Name of the Marker Cluster to create and add the SubGroup to
+
+        """
+        locations = decode_geohash_collection(geohashes)
+
+        self.create_new_subgroup_with_locations(
+            locations=locations,
+            subgroup_name=subgroup_name,
+            cluster_name=cluster_name,
+            **kwargs,
+        )
+
+    @staticmethod
+    def create_marker(
+        location: Tuple[float, float],
+        tooltip: str = None,
+        popup: str = None,
+        **kwargs,
+    ) -> folium.Marker:
         """
-        Return the list of notebooks for the dataset.
+        Create and return a Folium Marker at a given location.
+
+        Parameters
+        ----------
+        location: Tuple[float,float]
+            Latitude/Longitude coordinates for the Marker
+        tooltip: str [Optional]
+            Tooltip text for the Marker
+        popup: str [Optional]
+            Popup text for the Marker
 
         Returns
         -------
-        List[Tuple[str, str, str]]
-            Tuples of (name, project, link)
+        Marker
+            A Folium Marker at the given location coordinates
 
         """
-        return [
-            (nbk.get("name", ""), nbk.get("project", ""), nbk.get("link", ""))
-            for nbk in self.notebooks
-        ]
+        return folium.Marker(
+            location=location, tooltip=tooltip, popup=popup, icon=folium.Icon(**kwargs)
+        )
 
-    def get_attacks(self) -> List[MitreAttack]:
+    @staticmethod
+    def create_marker_cluster(name: str):
         """
-        Return list of Mitre attack classifications.
+        Create and return a MarkerCluster with name.
+
+        Parameters
+        ----------
+        name: str
+            Name of the MarkerCluster
 
         Returns
         -------
-        List[MitreAttack]
-            List of MitreAttack definitions.
+        MarkerCluster
+            A Folium MarkerCluster with the provided name
 
         """
-        return [MitreAttack(attack=attack) for attack in self.attack_mappings]
+        return MarkerCluster(name=name)
 
-    def get_file_paths(self) -> List[Dict[str, str]]:
+    @staticmethod
+    def create_feature_sub_group_of_marker_cluster(
+        cluster: MarkerCluster, name: str
+    ) -> FeatureGroupSubGroup:
         """
-        Return list of data file links.
+        Return a FeatureGroupSubGroup with `name` for a MarkerCluster.
+
+        Parameters
+        ----------
+        cluster: MarkerCluster
+            Folium MarkerCluster to add FeatureGroupSubGroup to
+        name: str
+            Desired name of the MarkerCluster
 
         Returns
         -------
-        List[Dict[str, str]]
-            list of dictionaries describing files.
-            Each entry has key/values for:
-            - file_type
-            - file_path
-            - relative_path
-            - qry_path
-
-        """
-        if not self._rel_file_paths:
-            for file in self.files:
-                f_path = file.get("link")
-                if not f_path:
-                    continue
-                f_rel_path = f_path.replace(DS_PREFIX, "")
-                query_path = ".".join(Path(f_rel_path).parts).replace(
-                    Path(f_rel_path).suffix, ""
-                )
-                self._rel_file_paths.append(
-                    {
-                        "file_type": file.get("type"),
-                        "file_path": f_path,
-                        "relative_path": f_rel_path,
-                        "qry_path": query_path,
-                    }
-                )
-        return self._rel_file_paths
-
+        FeatureGroupSubGroup
+            A Folium FeatureGroupSubGroup with the provided name as part
+            of the given MarkerCluster
 
-# pylint: disable=not-an-iterable, no-member
+        """
+        return FeatureGroupSubGroup(cluster, name=name)
 
 
-def get_mdr_data_paths(item_type="metadata") -> Generator[str, None, None]:
+@export
+def decode_geo_hash(geohash: str) -> Tuple[float, float, float, float]:
     """
-    Generate Mordor data sets from GitHub repo.
+    Decode a geohash.
 
     Parameters
     ----------
-    item_type : str, optional
-        The type of item required, by default "metadata"
-        Other values are "large", "small.
+    geohash: str
+        A string representation of a location
 
-    Yields
+    Returns
+    -------
+    Tuple
+        Tuple representation of a geohash, format of:
+        (Latitude, Longitude,
+        Latitude Error interval, Longitude Error Interval)
+
+    Raises
     ------
-    str
-        Iterable of paths
+    MsticpyMissingDependencyError
+        If pygeohash is not installed.
 
     """
-    md_tree = _GET_MORDOR_TREE(_MORDOR_TREE_URI)
-    yield from (
-        t_item["path"]
-        for t_item in md_tree.get("tree")
-        if t_item["type"] == "blob"
-        and t_item["path"].startswith("datasets")
-        and item_type in t_item["path"]
-    )
-
+    if pygeohash is not None:
+        return pygeohash.decode_exactly(geohash)
+    raise MsticpyMissingDependencyError(packages="pygeohash")
 
-def _get_mdr_github_tree():
-    """Closure to wrap fetching Mordor tree from GitHub."""
-    mordor_tree = None
 
-    def _get_mdr_tree(uri):
-        nonlocal mordor_tree
-        if mordor_tree is None:
-            resp = httpx.get(uri, timeout=_HTTP_TIMEOUT, headers=mp_ua_header())
-            mordor_tree = resp.json()
-        return mordor_tree
-
-    return _get_mdr_tree
+@export
+def decode_geohash_collection(geohashes: Iterable[str]):
+    """
+    Return collection of geohashes decoded into location coordinates.
 
+    Parameters
+    ----------
+    geohashes: Iterable[str]
+        Collection of geohashes to be decoded
 
-# Create closure
-_GET_MORDOR_TREE = _get_mdr_github_tree()
+    Returns
+    -------
+    Iterable[Tuple[float, float]]
+        Collection of location coordinates in Latitude/Longitude
 
+    """
+    locations = []
 
-def _get_mdr_file(gh_file):
-    """Fetch a file from Mordor repo."""
-    file_blob_uri = (
-        f"https://raw.githubusercontent.com/OTRF/Security-Datasets/master/{gh_file}"
+    for geohash in geohashes:
+        exact_location = decode_geo_hash(geohash)
+        locations.append((exact_location[0], exact_location[1]))
+
+    return locations
+
+
+def _get_tooltip_text(ip_entity):
+    """Return tooltip text for marker."""
+    return "<br>".join(
+        str(line)
+        for line in [
+            ip_entity.Address,
+            ip_entity.Location.City or "Unknown city",
+            ip_entity.Location.CountryCode or "Unknown country",
+            *(list(ip_entity.AdditionalData.items())),
+        ]
     )
-    file_resp = httpx.get(file_blob_uri, timeout=_HTTP_TIMEOUT, headers=mp_ua_header())
-    return file_resp.content
-
-
-def _create_mdr_metadata_cache():
-    md_metadata: Dict[str, MordorEntry] = {}
 
-    def _get_mdr_metadata(cache_folder: Optional[str] = None):
-        nonlocal md_metadata
-        if not md_metadata:
-            md_metadata = _fetch_mdr_metadata(cache_folder=cache_folder)
-        return md_metadata
-
-    return _get_mdr_metadata
 
+def _get_popup_text(ip_entity):
+    """Return popup text for marker."""
+    return "<br>".join(
+        str(line)
+        for line in [
+            ip_entity.Address,
+            *(list(ip_entity.Location.properties.values())),
+            *(list(ip_entity.AdditionalData.items())),
+        ]
+    )
 
-# Create closure
-_GET_MORDOR_METADATA = _create_mdr_metadata_cache()
 
-_LAST_UPDATE_KEY = "mp_last_updated"
-_DEFAULT_TS = pd.Timestamp(pd.Timestamp.utcnow() - pd.Timedelta(days=60))
+IconMapper = Union[Callable[[str], Dict[str, Any]], Dict[str, Any], None]
 
 
-# pylint: disable=global-statement
-def _fetch_mdr_metadata(cache_folder: Optional[str] = None) -> Dict[str, MordorEntry]:
+# pylint: disable=too-many-locals, too-many-arguments
+def plot_map(
+    data: pd.DataFrame,
+    ip_column: Optional[str] = None,
+    lat_column: Optional[str] = None,
+    long_column: Optional[str] = None,
+    layer_column: Optional[str] = None,
+    icon_column: Optional[str] = None,
+    icon_map: IconMapper = None,
+    popup_columns: Optional[List[str]] = None,
+    tooltip_columns: Optional[List[str]] = None,
+    **kwargs,
+) -> folium.Map:
     """
-    Return full metadata for Mordor datasets.
+    Plot folium map from DataFrame.
 
     Parameters
     ----------
-    cache_folder : Optional[str]
-        Folder to search for mordor cache, by default None
+    data : pd.DataFrame
+        The input DataFrame, must have either an IP address
+        column or latitude and longitude columns.
+    ip_column : Optional[str], optional
+        The name of the IP Address column, by default None
+    lat_column : Optional[str], optional
+        The name of the location 'latitude' column, by default None
+    long_column : Optional[str], optional
+        The name of the location 'longitude' column, by default None
+    layer_column : Optional[str], optional
+        The column to group markers into for displaying on different
+        map layers, by default None
+    icon_column : Optional[str], optional
+        Optional column containing the name of the icon to use
+        for the marker in this row, by default None
+    icon_map : IconMapper, optional
+        Mapping dictionary or function, by default None
+        See Notes for more details.
+    popup_columns : Optional[List[str]], optional
+        List of columns to use for the popup text, by default None
+    tooltip_columns : Optional[List[str]], optional
+        List of columns to use for the tooltip text, by default None
+
+
+    Other Parameters
+    ----------------
+    marker_cluster : bool, optional
+        Use marker clustering, default is True.
+    default_color : str, optional
+        Default color for marker icons, by default "blue"
+    title : str, optional
+        Name of the layer (the default is 'layer1')
+        (passed to FoliumMap constructor)
+    zoom_start : int, optional
+        The zoom level of the map (the default is 7)
+        (passed to FoliumMap constructor)
+    tiles : [type], optional
+        Custom set of tiles or tile URL (the default is None)
+        (passed to FoliumMap constructor)
+    width : str, optional
+        Map display width (the default is '100%')
+        (passed to FoliumMap constructor)
+    height : str, optional
+        Map display height (the default is '100%')
+        (passed to FoliumMap constructor)
+    location : list, optional
+        Location to center map on
 
     Returns
     -------
-    Dict[str, MordorEntry]:
-        Mordor data set metadata keyed by MordorID
+    folium.Map
+        Folium Map object.
 
-    """
-    global MITRE_TECHNIQUES, MITRE_TACTICS
-
-    if MITRE_TECHNIQUES is None or MITRE_TACTICS is None:
-        MITRE_TECHNIQUES, MITRE_TACTICS = _get_mitre_categories()
-    md_metadata: Dict[str, MordorEntry] = {}
+    Raises
+    ------
+    ValueError
+        If neither `ip_column` nor `lat_column` and `long_column` are passed.
+    LookupError
+        If one of the passed columns does not exist in `data`
+
+    Notes
+    -----
+    There are two ways of providing custom icon settings based on the
+    the row of the input DataFrame.
+
+    If `icon_map` is a dict it should contain keys that map to the
+    value of `icon_col` and values that a dicts of valid
+    folium Icon properties ("color", "icon_color", "icon", "angle", "prefix").
+    The dict should include a "default" entry that will be used if the
+    value in the DataFrame[icon_col] doesn't match any key.
+    For example:
+
+    .. code:: python
+
+        icon_map = {
+            "high": {
+                "color": "red",
+                "icon": "warning",
+            },
+            "medium": {
+                "color": "orange",
+                "icon": "triangle-exclamation",
+                "prefix": "fa",
+            },
+            "default": {
+                "color": "blue",
+                "icon": "info-sign",
+            },
+        }
 
-    md_cached_metadata = _read_mordor_cache(cache_folder)
-    mdr_md_paths = list(get_mdr_data_paths("metadata"))
-    for filename in tqdm(
-        mdr_md_paths, unit=" files", desc="Downloading Mordor metadata"
-    ):
-        cache_valid = False
-        if filename in md_cached_metadata:
-            metadata_doc = md_cached_metadata[filename]
-            last_timestamp = pd.Timestamp(
-                metadata_doc.get(_LAST_UPDATE_KEY, _DEFAULT_TS)
-            )
-            cache_valid = (pd.Timestamp.utcnow() - last_timestamp).days < 30
+    If icon_map is a function it should take a single str parameter
+    (the item key) and return a dict of icon properties. It should
+    return a default set of values if the key does not match a known
+    key. The `icon_col` value for each row will be passed to this
+    function and the return value used to populate the Icon arguments.
+
+    For example:
+
+    .. code::python
+
+        def icon_mapper(icon_key):
+            if icon_key.startswith("bad"):
+                return {
+                    "color": "red",
+                    "icon": "triangle-alert",
+                }
+            ...
+            else:
+                return {
+                    "color": "blue",
+                    "icon": "info-sign",
+                }
 
-        if not cache_valid:
-            gh_file_content = _get_mdr_file(filename)
-            try:
-                metadata_doc = yaml.safe_load(gh_file_content)
-            except yaml.error.YAMLError:
-                continue
-            metadata_doc[_LAST_UPDATE_KEY] = pd.Timestamp.utcnow().isoformat()
-            md_cached_metadata[filename] = metadata_doc
-        doc_id = metadata_doc.get("id")
-        mdr_entry = metadata_doc.copy()
-        mdr_entry.pop(_LAST_UPDATE_KEY, None)
-        md_metadata[doc_id] = MordorEntry(**mdr_entry)
+    FontAwesome icon (prefix "fa") names are available at https://fontawesome.com/
+    GlyphIcons icons (prefix "glyphicon") are available at https://www.glyphicons.com/
 
-    _write_mordor_cache(md_cached_metadata, cache_folder)
-    return md_metadata
+    """
+    folium_map = FoliumMap(**kwargs)
+    if ip_column and not (lat_column and long_column):
+        # resolve IP location and merge with input data.
+        data = data.merge(
+            # pylint: disable=no-member
+            _GEO_LITE.lookup_ips(data, column=ip_column),
+            # pylint: enable=no-member
+            left_on=ip_column,
+            right_on="IpAddress",
+            suffixes=("_src", None),
+        ).dropna(axis="index", subset=["Latitude", "Longitude"])
+        lat_column, long_column = ["Latitude", "Longitude"]
+        if not tooltip_columns:
+            tooltip_columns = _default_columns(data, [ip_column, "CountryCode", "City"])
+        if not popup_columns:
+            popup_columns = _default_columns(
+                data, [ip_column, "CountryName", "City", lat_column, long_column]
+            )
+    else:
+        if not tooltip_columns:
+            tooltip_columns = []
+            tooltip_columns.extend(col for col in (lat_column, long_column) if col)
+        if not popup_columns:
+            popup_columns = []
+            popup_columns.extend(col for col in (lat_column, long_column) if col)
+
+    _validate_columns(
+        data,
+        ip_column,
+        lat_column,
+        long_column,
+        [layer_column, icon_column],
+    )
+    popup_columns = _validate_optional_columns(data, popup_columns)
+    tooltip_columns = _validate_optional_columns(data, tooltip_columns)
 
+    folium_map.locations.extend(
+        data.apply(lambda row: (row[lat_column], row[long_column]), axis=1)
+    )
+    # common dictionary of kwargs to _create_feature_group
+    static_kwargs = {
+        "lat_column": lat_column,
+        "long_column": long_column,
+        "icon_column": icon_column,
+        "icon_map": icon_map,
+        "popup_cols": popup_columns,
+        "tooltip_cols": tooltip_columns,
+        "use_marker_cluster": kwargs.pop("marker_cluster", True),
+    }
+    if layer_column is None:
+        feature_group = _create_feature_group(
+            data=data,
+            layer_name="All locations",
+            def_layer_color=kwargs.pop("default_color", "blue"),
+            **static_kwargs,  # type: ignore
+        )
+        feature_group.add_to(folium_map.folium_map)
+    else:
+        for index, (layer, layer_df) in enumerate(data.groupby(layer_column)):
+            def_layer_color = _get_icon_layer_color(index)
+            feature_group = _create_feature_group(
+                data=layer_df,
+                layer_name=layer,
+                def_layer_color=def_layer_color,
+                **static_kwargs,  # type: ignore
+            )
+            feature_group.add_to(folium_map.folium_map)
+        folium.LayerControl().add_to(folium_map.folium_map)
+    if "location" not in kwargs:
+        folium_map.center_map()
+    return folium_map
 
-# pylint: enable=global-statement
 
+# pylint: enable=too-many-locals, too-many-arguments
 
-def _read_mordor_cache(cache_folder) -> Dict[str, Any]:
-    """Return dictionary of cached metadata if cached_folder is a valid path."""
-    md_cached_metadata: Dict[str, Any] = {}
-    mordor_cache = Path(cache_folder).joinpath(_MORDOR_CACHE)
-    if _valid_cache(mordor_cache):
-        try:
-            md_json = Path(mordor_cache).read_text(encoding="utf-8")
-            md_cached_metadata = json.loads(md_json)
-        except json.JSONDecodeError:
-            pass
-    return md_cached_metadata
 
+def _default_columns(data, defaults: Iterable[str]) -> List[str]:
+    return [col_name for col_name in defaults if col_name in data.columns]
 
-def _write_mordor_cache(md_cached_metadata, cache_folder):
-    """Write dictionary of cached metadata if cached_folder is a valid path."""
-    mordor_cache = Path(cache_folder).joinpath(_MORDOR_CACHE)
-    json_text = json.dumps(md_cached_metadata, indent=4)
-    Path(mordor_cache).write_text(json_text, encoding="utf-8")
 
+def _validate_columns(data, ip_column, lat_column, long_column, other_columns):
+    """Validate required columns and that optional cols are in the data."""
+    if not ip_column and not (lat_column and long_column):
+        raise ValueError(
+            "Data must have either an IpAddress ('ip_column')",
+            "or latitude ('lat_column') and longitude ('long_column')",
+        )
+    param_cols: List[str] = []
+    for param in other_columns:
+        if not param:
+            continue
+        if isinstance(param, list):
+            param_cols.extend(param)
+        else:
+            param_cols.append(param)
+    missing_columns = {col for col in param_cols if col not in data.columns}
+    if missing_columns:
+        raise LookupError(
+            "The following columns are not in the supplied DataFrame",
+            ",".join(f"'{col}'" for col in missing_columns),
+        )
 
-def _build_mdr_indexes(
-    mdr_metadata: Dict[str, MordorEntry]
-) -> Tuple[Dict[str, Set[str]], Dict[str, Set[str]]]:
-    """
-    Return dictionaries mapping Mitre items to Mordor datasets.
 
-    Parameters
-    ----------
-    mdr_metadata : Dict[str, MordorEntry]
-        Dictionary of mordor dataset metadata.
+def _validate_optional_columns(data, optional_columns: Iterable[str]) -> List[str]:
+    """Validate that optional columns are in the data."""
+    return [col for col in optional_columns if col in data.columns]
+
+
+# pylint: disable=too-many-arguments
+def _create_feature_group(
+    data: pd.DataFrame,
+    layer_name: str,
+    lat_column: str,
+    long_column: str,
+    icon_column: Optional[str],
+    icon_map: IconMapper,
+    popup_cols: List[str],
+    tooltip_cols: List[str],
+    def_layer_color: str,
+    use_marker_cluster: bool = True,
+) -> folium.FeatureGroup:
+    """Create folium feature group."""
+    feature_group = folium.FeatureGroup(name=layer_name)
+    if use_marker_cluster:
+        container = MarkerCluster(name=layer_name)
+        container.add_to(feature_group)
+    else:
+        container = feature_group
+    data.apply(
+        lambda row: folium.Marker(
+            location=(row[lat_column], row[long_column]),
+            tooltip=_create_marker_text(row, tooltip_cols),
+            popup=_create_marker_text(row, popup_cols),
+            icon=_create_mapped_icon(row, icon_column, icon_map, def_layer_color),
+        ).add_to(feature_group),
+        axis=1,
+    )
+    return feature_group
 
-    Returns
-    -------
-    Tuple[Dict[str, Set[str]], Dict[str, Set[str]]]
-        Mordor dataset IDs keyed by Mitre Technique and Mitre Tactic.
 
-    """
-    md_idx_techniques = defaultdict(set)
-    md_idx_tactics = defaultdict(set)
+# pylint: enable=too-many-arguments
 
-    for md_id, md_file in mdr_metadata.items():
-        for attack in md_file.get_attacks():
-            md_idx_techniques[attack.technique].add(md_id)
-            if not attack.tactics:
-                continue
-            for tactic in attack.tactics:
-                md_idx_tactics[tactic].add(md_id)
 
-    return md_idx_techniques, md_idx_tactics  # type: ignore
+def _create_marker_text(row: pd.Series, columns: List[str]) -> str:
+    """Return HTML formatted text for tooltips and popups."""
+    return "<br>".join(f"{col}: {row[col]}" for col in columns)
+
+
+def _get_icon_layer_color(layer_index: int) -> str:
+    """Get a color from folium.color options."""
+    col_options = folium.Icon.color_options - {"white"}
+    return list(col_options)[layer_index % len(col_options)]
+
+
+def _create_mapped_icon(
+    row: pd.Series,
+    icon_column: Optional[str] = None,
+    icon_map: Optional[IconMapper] = None,
+    def_layer_color: str = "blue",
+) -> folium.Icon:
+    """Return folium Icon from mapping or defaults."""
+    icon_kwargs: Dict[str, str] = {}
+    if isinstance(icon_map, dict):
+        icon_kwargs = icon_map.get(row[icon_column], icon_map.get("default", {}))
+    elif callable(icon_map):
+        icon_kwargs = icon_map(row[icon_column])
+    elif icon_column:
+        icon_kwargs = {"icon": row[icon_column]}
+    if "color" not in icon_kwargs:
+        icon_kwargs["color"] = def_layer_color
+    return folium.Icon(**icon_kwargs)
+
+
+def _get_location_for_ip_entities(
+    ip_entities: Iterable[IpAddress],
+) -> Generator[IpAddress, None, None]:
+    for ip_entity in ip_entities:
+        if (
+            ip_entity.Location is None
+            or ip_entity.Location.Longitude is None
+            or ip_entity.Location.Latitude is None
+        ):
+            _, ip_res_list = _GEO_LITE.lookup_ip(ip_entity=ip_entity)
+            if ip_res_list:
+                ip_entity.Location = ip_res_list[0].Location  # type: ignore
+        yield ip_entity
 
 
-def download_mdr_file(
-    file_uri: str, use_cached: bool = True, save_folder: str = ".", silent: bool = False
-) -> pd.DataFrame:
+@export
+def get_map_center(entities: Iterable[Entity], mode: str = "modal"):
     """
-    Download data file from Mordor.
+    Calculate median point between Entity IP locations.
 
     Parameters
     ----------
-    file_uri : str
-        The URI of the file to download.
-    use_cached : bool, optional
-        Try to use locally saved file first, by default True
-    save_folder : str, optional
-        Path to output folder, by default "."
-    silent : bool
-        If True, suppress feedback. By default, False.
+    entities : Iterable[Entity]
+        An iterable of entities containing IpAddress geolocation information.
+        The entities can be IpAddress entities or other entities that
+        have IpAddress properties.
+        The entities must all be of the same type.
+    mode : str, optional
+        The averaging method to use, by default "median".
+        "median" and "mean" are the supported values.
 
     Returns
     -------
-    pd.DataFrame
-        DataFrame of Dataset
+    Tuple
+        The Latitude and Longitude calculated
+
+    Notes
+    -----
+    The function uses the first entity in the `entities` to determine
+    how to process the collection. E.g. if the first entity has properties
+    src_ip and dest_ip of type `IpAddress`, these are the only properties
+    that will be processed for the remainder of the entities.
 
     """
-    if not silent:
-        print(file_uri)
-    if not file_uri.lower().endswith("zip"):
-        raise TypeError(f"File type not supported {file_uri}")
-    if not Path(save_folder).is_dir():
-        Path(save_folder).mkdir(parents=True, exist_ok=True)
-    save_path = "-".join(Path(file_uri.replace(DS_PREFIX, "")).parts)
-    save_file = Path(save_folder).joinpath(save_path)
-    if not use_cached or not save_file.is_file():
-        # streamed download
-        with open(str(save_file), "wb") as fdesc:
-            with httpx.stream(
-                "GET", file_uri, timeout=_HTTP_TIMEOUT, headers=mp_ua_header()
-            ) as resp:
-                for chunk in resp.iter_bytes(chunk_size=1024):
-                    fdesc.write(chunk)
-
-    try:
-        with zipfile.ZipFile(str(save_file)) as zip_file:
-            file_names = zip_file.namelist()
-            d_frames = {
-                file_name: _extract_zip_file_to_df(
-                    zip_file, file_name, use_cached, save_folder, silent
-                )
-                for file_name in file_names
-            }
-            return pd.concat(d_frames.values())
-    except BadZipFile as bad_zip_err:
-        raise MsticpyUserError(
-            f"Could not extract zip file for {file_uri}.",
-            "File does not exist or is corrupt.",
-            title="Mordor download error",
-            help_uri="https://msticpy.readthedocs.io/en/latest/data_acquisition/MordorData.html",
-        ) from bad_zip_err
-
-
-def _extract_zip_file_to_df(  # noqa: MC0001
-    zip_file: ZipFile,
-    file_name: str,
-    use_cached: bool = True,
-    save_folder: str = ".",
-    silent: bool = False,
-) -> pd.DataFrame:
-    """
-    Extract from zip and parse json file to DataFrame.
+    ip_entities: List[IpAddress] = []
+    loc_entities: List[GeoLocation] = []
+    if not entities:
+        return (0, 0)
+    entities = list(entities)
+    if isinstance(entities[0], IpAddress):
+        return get_center_ip_entities(entities)  # type: ignore
+    loc_props = [
+        p_name
+        for p_name, p_val in entities[0].properties.items()
+        if isinstance(p_val, (IpAddress, GeoLocation))
+    ]
+    for entity, prop in itertools.product(entities, loc_props):
+        if prop not in entity:
+            continue
+        loc_entity = entity[prop]
+        if isinstance(loc_entity, IpAddress):
+            ip_entities.append(loc_entity)
+        elif isinstance(loc_entity, GeoLocation):
+            loc_entities.append(loc_entity)
+    locs_ips = _extract_locs_ip_entities(ip_entities)
+    return get_center_geo_locs(locs_ips + loc_entities, mode=mode)
 
-    Parameters
-    ----------
-    zip_file : ZipFile
-        ZipFile object containing the file
-    file_name : str
-        File name to extract
-    use_cached : bool, optional
-        Try to use locally saved file first, by default True
-    save_folder : str, optional
-        Path to output folder, by default "."
-    silent : bool
-        If False, suppress feedback. By default, True.
 
-    Returns
-    -------
-    pd.DataFrame
-        Extracted DataFrame
+def _extract_locs_ip_entities(ip_entities: Iterable[IpAddress]):
+    """Return the list of IP entities that have a Location property."""
+    if isinstance(ip_entities[0], list):  # type: ignore
+        return [
+            ip[0]["Location"]  # type: ignore
+            for ip in ip_entities
+            if bool(ip[0].Location)  # type: ignore
+        ]
+    return [ip["Location"] for ip in ip_entities if bool(ip.Location)]
 
-    """
-    if not silent:
-        print("Extracting", file_name)
 
-    file_path = Path(save_folder).joinpath(file_name)
-    if not use_cached or not file_path.is_file():
-        zip_file.extract(file_name, path=save_folder)
-
-    out_df = pd.DataFrame()
-    if file_path.suffix.lower() == ".json":
-        out_df = pd.read_json(file_path, lines=True)
-    if file_path.suffix.lower() == ".csv":
-        out_df = pd.read_csv(file_path)
-    if file_path.suffix.lower() not in (".json", ".csv"):
-        print(f"Cannot process files of type {file_path.suffix.lower()}")
-    if not use_cached:
-        Path(file_name).unlink()
-    return out_df
-
-
-def search_mdr_data(
-    mdr_data: Dict[str, MordorEntry], terms: str = None, subset: Iterable[str] = None
-) -> Set[str]:
+@export
+def get_center_ip_entities(
+    ip_entities: Iterable[IpAddress], mode: str = "median"
+) -> Tuple[float, float]:
     """
-    Return IDs for items matching terms.
+    Return the geographical center of the IP address locations.
 
     Parameters
     ----------
-    mdr_data : Dict[str, MordorEntry]
-        Mordor dataset
-    terms : str, optional
-        Search terms, by default None
-        (comma-separated values are treated as OR terms
-        plus-separated values are treated as AND terms)
-    subset : Iterable[str], optional
-        A subset of IDs over which to search, by default None
+    ip_entities : Iterable[IpAddress]
+        IpAddress entities with location information
+    mode : str, optional
+        The averaging method to us, by default "median".
+        "median" and "mean" are the supported values.
 
     Returns
     -------
-    Set[str]
-        The set of matching IDs.
+    Tuple[Union[int, float], Union[int, float]]
+        Tuple of latitude, longitude
 
     """
-    if terms is None:
-        return set(subset or mdr_data.keys())
-    logic = "OR"
-    if "," in terms:
-        search_terms = terms.split(",")
-    elif "+" in terms:
-        search_terms = terms.split("+")
-        logic = "AND"
-    else:
-        search_terms = [terms]
-    results: Set[str] = set()
-    for search_idx, term in enumerate(search_terms):
-        item_results = set()
-        for md_id, item in mdr_data.items():
-            if subset is not None and md_id not in subset:
-                continue
-            if term.strip() in str(item):
-                item_results.add(md_id)
-        if logic == "OR":
-            results = results | item_results
-        else:
-            # Don't AND if search_idx == 0 (and-ing against empty results)
-            results = results & item_results if search_idx else item_results
-    return results
+    ip_locs_longs = _extract_locs_ip_entities(ip_entities)
+    return get_center_geo_locs(ip_locs_longs, mode=mode)
 
 
-def _extract_mitre_refs(ext_refs):
-    ref_dict = [
-        ref
-        for ref in ext_refs
-        if "source_name" in ref and ref["source_name"] == "mitre-attack"
+def _extract_coords_loc_entities(loc_entities: Iterable[GeoLocation]):
+    """Return list of coordinate tuples from GeoLocation entities."""
+    return [
+        (loc["Latitude"], loc["Longitude"])
+        for loc in loc_entities
+        if "Latitude" in loc and "Longitude" in loc
     ]
-    if ref_dict:
-        return ref_dict[0]
-    return {}
 
 
-def _reshape_mitre_df(data):
-    col_rename = {"external_id": "ID", "name": "Name", "description": "Description"}
-    return (
-        data.join(
-            data.apply(
-                lambda x: _extract_mitre_refs(x.external_references),
-                axis=1,
-                result_type="expand",
-            )
-        )
-        .assign(MitreGroup="Enterprise")[["external_id", "name", "description", "url"]]
-        .rename(columns=col_rename)
-        .sort_values("ID")
-        .set_index("ID")
-    )
-
-
-def _get_mitre_categories(
-    cache_folder: Optional[str] = None,
-) -> Tuple[pd.DataFrame, pd.DataFrame]:
+@export
+def get_center_geo_locs(
+    loc_entities: Iterable[GeoLocation], mode: str = "median"
+) -> Tuple[float, float]:
     """
-    Download and return Mitre techniques and tactics.
+    Return the geographical center of the geo locations.
 
     Parameters
     ----------
-    cache_folder : Optional[str]
-        Folder to search for mordor cache, by default None
+    loc_entities : Iterable[GeoLocation]
+        GeoLocation entities with location information
+    mode : str, optional
+        The averaging method to use, by default "median".
+        "median" and "mean" are the supported values.
 
     Returns
     -------
-    Tuple[pd.DataFrame, pd.DataFrame]
-        Tuple of techniques, tactics with IDs, names,
-        descriptions.
-
-    """
-    if cache_folder:
-        tech_cache = Path(cache_folder).joinpath(_MITRE_TECH_CACHE)
-        tactics_cache = Path(cache_folder).joinpath(_MITRE_TACTICS_CACHE)
-        if _valid_cache(tech_cache) and _valid_cache(tactics_cache):
-            try:
-                # caching location only used if sepcified.
-                tech_df = pd.read_pickle(tech_cache)  # nosec
-                tactics_df = pd.read_pickle(tactics_cache)  # nosec
-                return tech_df, tactics_df
-            except pickle.PickleError:
-                pass
-    resp = httpx.get(_MITRE_JSON_URL, timeout=_HTTP_TIMEOUT, headers=mp_ua_header())
-    mitre = pd.json_normalize(resp.json()["objects"])
-
-    # remove deprecated items
-    mitre["x_mitre_deprecated"].fillna(False, inplace=True)
-    mitre = mitre[~(mitre["x_mitre_deprecated"])]
-
-    tech_df = _reshape_mitre_df(mitre[mitre.type == "attack-pattern"])
-    tactics_df = _reshape_mitre_df(mitre[mitre.type == "x-mitre-tactic"])
-    if cache_folder:
-        tech_df.to_pickle(tech_cache)
-        tactics_df.to_pickle(tactics_cache)
-
-    return tech_df, tactics_df
-
-
-def _valid_cache(path: Path, expired_days=30):
-    """Return True if the file exists and is younger than `expired_days`."""
-    if not path.is_file():
-        return False
-    days_old = (datetime.now() - datetime.fromtimestamp(path.stat().st_mtime)).days
-    return days_old < expired_days
+    Tuple[Union[int, float], Union[int, float]]
+        Tuple of latitude, longitude
+
+    """
+    lat_longs = _extract_coords_loc_entities(loc_entities)
+    return _get_center_coords(lat_longs, mode=mode)
+
+
+def _get_center_coords(
+    locations: Iterable[Tuple[float, float]], mode: str = "median"
+) -> Tuple[float, float]:
+    """Return the center (median) of the coordinates."""
+    if not locations:
+        return 0, 0
+    locs = list(locations)
+    if mode == "median":
+        with contextlib.suppress(stats.StatisticsError):
+            return (
+                stats.median([loc[0] for loc in locs if not math.isnan(loc[0])]),
+                stats.median([loc[1] for loc in locs if not math.isnan(loc[1])]),
+            )
+    return (
+        stats.mean([loc[0] for loc in locs if not math.isnan(loc[0])]),
+        stats.mean([loc[1] for loc in locs if not math.isnan(loc[1])]),
+    )
```

### Comparing `msticpy-2.4.0/msticpy/data/drivers/odata_driver.py` & `msticpy-2.5.0/msticpy/data/drivers/odata_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/drivers/resource_graph_driver.py` & `msticpy-2.5.0/msticpy/data/drivers/resource_graph_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/drivers/security_graph_driver.py` & `msticpy-2.5.0/msticpy/data/drivers/security_graph_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/drivers/splunk_driver.py` & `msticpy-2.5.0/msticpy/init/pivot_core/pivot_pd_accessor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,402 +1,456 @@
-#  -------------------------------------------------------------------------
-#  Copyright (c) Microsoft Corporation. All rights reserved.
-#  Licensed under the MIT License. See License.txt in the project root for
-#  license information.
-#  --------------------------------------------------------------------------
-"""Splunk Driver class."""
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License.txt in the project root for
+# license information.
+# --------------------------------------------------------------------------
+"""Pandas DataFrame accessor for Pivot functions."""
+
+import contextlib
+import json
+import re
+import warnings
 from datetime import datetime
-from time import sleep
-from typing import Any, Dict, Iterable, Optional, Tuple, Union
+from json import JSONDecodeError
+from numbers import Number
+from typing import Callable, Dict, Iterable, Set, Union
 
+import numpy as np
 import pandas as pd
-from tqdm import tqdm
+from IPython import get_ipython
+from IPython.display import HTML, display
+from pkg_resources import parse_version
 
 from ..._version import VERSION
-from ...common.exceptions import (
-    MsticpyConnectionError,
-    MsticpyImportExtraError,
-    MsticpyUserConfigError,
-)
-from ...common.utility import check_kwargs, export
-from ..core.query_defns import Formatters
-from .driver_base import DriverBase, QuerySource
-
-try:
-    import splunklib.client as sp_client
-    import splunklib.results as sp_results
-    from splunklib.client import AuthenticationError, HTTPError
-except ImportError as imp_err:
-    raise MsticpyImportExtraError(
-        "Cannot use this feature without splunk-sdk installed",
-        title="Error importing splunk-sdk",
-        extra="splunk",
-    ) from imp_err
 
 __version__ = VERSION
-__author__ = "Ashwin Patil"
+__author__ = "Ian Hellen"
 
 
-SPLUNK_CONNECT_ARGS = {
-    "host": "(string) The host name (the default is 'localhost').",
-    "port": "(integer) The port number (the default is 8089).",
-    "http_scheme": "('https' or 'http') The scheme for accessing the service "
-    + "(the default is 'https').",
-    "verify": "(Boolean) Enable (True) or disable (False) SSL verrification for "
-    + "https connections. (optional, the default is True)",
-    "owner": "(string) The owner context of the namespace (optional).",
-    "app": "(string) The app context of the namespace (optional).",
-    "sharing": "('global', 'system', 'app', or 'user') "
-    + "The sharing mode for the namespace (the default is 'user').",
-    "token": "(string) The current session token (optional). Session tokens can be"
-    + " shared across multiple service instances.",
-    "cookie": "(string) A session cookie. When provided, you don’t need to call"
-    + " login(). This parameter is only supported for Splunk 6.2+.",
-    "autologin": "(boolean) When True, automatically tries to log in again if"
-    + " the session terminates.",
-    "username": "(string) The Splunk account username, which is used to "
-    + "authenticate the Splunk instance.",
-    "password": "(string) The password for the Splunk account.",
-}
-
-
-@export
-class SplunkDriver(DriverBase):
-    """Driver to connect and query from Splunk."""
-
-    _SPLUNK_REQD_ARGS = ["host", "username", "password"]
-    _CONNECT_DEFAULTS: Dict[str, Any] = {"port": 8089}
-    _TIME_FORMAT = '"%Y-%m-%d %H:%M:%S.%6N"'
-
-    def __init__(self, **kwargs):
-        """Instantiate Splunk Driver."""
-        super().__init__(**kwargs)
-        self.service = None
-        self._loaded = True
-        self._connected = False
-        self._debug = kwargs.get("debug", False)
-        self.public_attribs = {
-            "client": self.service,
-            "saved_searches": self._saved_searches,
-            "fired_alerts": self._fired_alerts,
-        }
-        self.formatters = {
-            Formatters.DATETIME: self._format_datetime,
-            Formatters.LIST: self._format_list,
-        }
+def _verbose_out(data, func, st_time, verbose=False, debug=False, **kwargs):
+    """Output verbose or debug info."""
+    end_time = datetime.now()
 
-    def connect(self, connection_str: str = None, **kwargs):
+    if verbose or debug:
+        print(f"{len(data)} rows returned from function {func.__name__}")
+    if debug:
+        print(f"Columns in result from function {func.__name__}:")
+        print(data.columns)
+        print(f"Execution time: {end_time - st_time}")
+        print(f"Parameters: {kwargs}")
+
+
+@pd.api.extensions.register_dataframe_accessor("mp_pivot")
+class PivotAccessor:
+    """Pandas api extension for Pivot functions."""
+
+    def __init__(self, pandas_obj):
+        """Instantiate pivot extension class."""
+        self._df = pandas_obj
+        self._ip = get_ipython()
+
+    def run(self, func: Callable[..., pd.DataFrame], **kwargs) -> pd.DataFrame:
         """
-        Connect to Splunk via splunk-sdk.
+        Run a pivot function on the current DataFrame.
 
         Parameters
         ----------
-        connection_str : Optional[str], optional
-            Connection string with Splunk connection parameters
+        func : Callable[..., pd.DataFrame]
+            Pivot function to run
+        kwargs:
+            Keyword arguments to pass to `func`.
+            A column specification (e.g. column="src_col_name")
+            is usually the minimum needed.
+            For data queries the `column` keyword must be the
+            name of the the query parameter (e.g. host_name = "src_col_name")
 
-        Other Parameters
-        ----------------
-        kwargs :
-            Connection parameters can be supplied as keyword parameters.
+        Returns
+        -------
+        pd.DataFrame
+            The output DataFrame from the function.
 
         Notes
         -----
-        Default configuration is read from the DataProviders/Splunk
-        section of msticpyconfig.yaml, if available.
-
-        """
-        cs_dict = self._get_connect_args(connection_str, **kwargs)
-
-        arg_dict = {
-            key: val for key, val in cs_dict.items() if key in SPLUNK_CONNECT_ARGS
-        }
-        try:
-            self.service = sp_client.connect(**arg_dict)
-        except AuthenticationError as err:
-            raise MsticpyConnectionError(
-                f"Authentication error connecting to Splunk: {err}",
-                title="Splunk connection",
-                help_uri="https://msticpy.readthedocs.io/en/latest/DataProviders.html",
-            ) from err
-        except HTTPError as err:
-            raise MsticpyConnectionError(
-                f"Communication error connecting to Splunk: {err}",
-                title="Splunk connection",
-                help_uri="https://msticpy.readthedocs.io/en/latest/DataProviders.html",
-            ) from err
-        except Exception as err:
-            raise MsticpyConnectionError(
-                f"Error connecting to Splunk: {err}",
-                title="Splunk connection",
-                help_uri="https://msticpy.readthedocs.io/en/latest/DataProviders.html",
-            ) from err
-        self._connected = True
-        print("connected")
-
-    def _get_connect_args(
-        self, connection_str: Optional[str], **kwargs
-    ) -> Dict[str, Any]:
-        """Check and consolidate connection parameters."""
-        cs_dict: Dict[str, Any] = self._CONNECT_DEFAULTS
-        # Fetch any config settings
-        cs_dict.update(self._get_config_settings("Splunk"))
-        # If a connection string - parse this and add to config
-        if connection_str:
-            cs_items = connection_str.split(";")
-            cs_dict.update(
-                {
-                    cs_item.split("=")[0].strip(): cs_item.split("=")[1]
-                    for cs_item in cs_items
-                }
-            )
-        elif kwargs:
-            # if connection args supplied as kwargs
-            cs_dict.update(kwargs)
-            check_kwargs(cs_dict, list(SPLUNK_CONNECT_ARGS.keys()))
-
-        cs_dict["port"] = int(cs_dict["port"])
-        verify_opt = cs_dict.get("verify")
-        if isinstance(verify_opt, str):
-            cs_dict["verify"] = "true" in verify_opt.casefold()
-        elif isinstance(verify_opt, bool):
-            cs_dict["verify"] = verify_opt
-
-        missing_args = set(self._SPLUNK_REQD_ARGS) - cs_dict.keys()
-        if missing_args:
-            raise MsticpyUserConfigError(
-                "One or more connection parameters missing for Splunk connector",
-                ", ".join(missing_args),
-                f"Required parameters are {', '.join(self._SPLUNK_REQD_ARGS)}",
-                "All parameters:",
-                *[f"{arg}: {desc}" for arg, desc in SPLUNK_CONNECT_ARGS.items()],
-                title="no Splunk connection parameters",
+        You can pass the `join` keyword argument to most
+        pivot functions. Values for join are "inner", "left", "right"
+        or "outer".
+
+        """
+        st_time = datetime.now()
+        verbose = kwargs.pop("verbose", False)
+        debug = kwargs.pop("debug", False)
+        result = self._df.pipe((func, "data"), **kwargs)
+        if verbose or debug:
+            _verbose_out(
+                data=result,
+                func=func,
+                st_time=st_time,
+                verbose=verbose,
+                debug=debug,
+                **kwargs,
             )
-        return cs_dict
+        return result
 
-    def query(
-        self, query: str, query_source: QuerySource = None, **kwargs
-    ) -> Union[pd.DataFrame, Any]:
+    def display(
+        self,
+        title: str = None,
+        cols: Iterable[str] = None,
+        query: str = None,
+        head: int = None,
+    ) -> pd.DataFrame:
         """
-        Execute splunk query and retrieve results via OneShot or async search mode.
+        Display the DataFrame in the middle of a pipeline.
 
         Parameters
         ----------
-        query : str
-            Splunk query to execute via OneShot or async search mode
-        query_source : QuerySource
-            The query definition object
-
-        Other Parameters
-        ----------------
-        count : int, optional
-            Passed to Splunk oneshot method if `oneshot` is True, by default, 0
-        oneshot : bool, optional
-            Set to True for oneshot (blocking) mode, by default False
+        title : str, optional
+            Title to display for the DataFrame, by default None
+        cols : Iterable[str], optional
+            List of columns to display, by default None
+        query : str, optional
+            Query to filter the displayed data, by default None
+            This should be a string executable by the DataFrame.query
+            function
+        head : int, optional
+            Limit the displayed output to `head` rows, by default None
 
         Returns
         -------
-        Union[pd.DataFrame, Any]
-            Query results in a dataframe.
-            or query response if an error.
-
-        """
-        del query_source
-        if not self._connected:
-            raise self._create_not_connected_err("Splunk")
-
-        # default to unlimited query unless count is specified
-        count = kwargs.pop("count", 0)
-
-        # Normal, oneshot or blocking searches. Defaults to non-blocking
-        # Oneshot is blocking a blocking HTTP call which may cause time-outs
-        # https://dev.splunk.com/enterprise/docs/python/sdk-python/howtousesplunkpython/howtorunsearchespython
-        is_oneshot = kwargs.get("oneshot", False)
-
-        if is_oneshot is True:
-            query_results = self.service.jobs.oneshot(query, count=count, **kwargs)
-            reader = sp_results.ResultsReader(query_results)
+        pd.DataFrame
+            Passed through input DataFrame.
 
-        else:
-            # Set mode and initialize async job
-            kwargs_normalsearch = {"exec_mode": "normal"}
-            query_job = self.service.jobs.create(query, **kwargs_normalsearch)
-
-            # Initiate progress bar and start while loop, waiting for async query to complete
-            progress_bar = tqdm(total=100, desc="Waiting Splunk job to complete")
-            while not query_job.is_done():
-                current_state = query_job.state
-                progress = float(current_state["content"]["doneProgress"]) * 100
-                progress_bar.update(progress)
-                sleep(1)
-
-            # Update progress bar indicating completion and fetch results
-            progress_bar.update(100)
-            progress_bar.close()
-            reader = sp_results.ResultsReader(query_job.results())
-
-        resp_rows = [row for row in reader if isinstance(row, dict)]
-        if not resp_rows:
-            print("Warning - query did not return any results.")
-            return [row for row in reader if isinstance(row, sp_results.Message)]
-        return pd.DataFrame(resp_rows)
+        """
+        if title:
+            display(HTML(f"<h3>{title}</h3>"))
+        disp_df = self._df
+        if cols:
+            disp_df = disp_df[cols]
+        if query:
+            disp_df = disp_df.query(query)  # , parser='python', engine='python')
+        if head:
+            disp_df = disp_df.head(head)
+        display(disp_df)
+        return self._df
 
-    def query_with_results(self, query: str, **kwargs) -> Tuple[pd.DataFrame, Any]:
+    def tee(self, var_name: str, clobber: bool = False) -> pd.DataFrame:
         """
-        Execute query string and return DataFrame of results.
+        Save current dataframe to `var_name` in the IPython user namespace.
 
         Parameters
         ----------
-        query : str
-            Query to execute against splunk instance.
+        var_name : str
+            The name of the DF variable to create.
+        clobber : bool, optional
+            Whether to overwrite an existing variable of the same name,
+            by default False
 
         Returns
         -------
-        Union[pd.DataFrame,Any]
-            A DataFrame (if successful) or
-            the underlying provider result if an error occurs.
+        pd.DataFrame
+            Passed through input DataFrame.
+
+        Notes
+        -----
+        This function only works in an IPython/Jupyter notebook environment.
+        It will attempt to create a variable in the user local namespace
+        that references the current state of the DataFrame in the pipeline.
+
+        By default it will not overwrite an existing variable of the same
+        name (specify `clobber=True` to overwrite)
 
         """
-        raise NotImplementedError(f"Not supported for {self.__class__.__name__}")
+        if self._ip and var_name:
+            if var_name in self._ip.ns_table["user_local"] and not clobber:
+                warnings.warn(f"Did not overwrite existing {var_name} in namespace")
+            else:
+                self._ip.ns_table["user_local"][var_name] = self._df
+        return self._df
 
-    @property
-    def service_queries(self) -> Tuple[Dict[str, str], str]:
+    def tee_exec(self, df_func: str, *args, **kwargs) -> pd.DataFrame:
         """
-        Return dynamic queries available on connection to service.
+        Run a dataframe method on the dataframe without changing it.
+
+        Parameters
+        ----------
+        df_func : str
+            The name of the function to execute. Accessor methods
+            must be of the form "accessor.method".
+        args : tuple
+            Positional arguments to be passed to the function
+        kwargs : dict
+            Keyword arguments to be passed to the function.
 
         Returns
         -------
-        Tuple[Dict[str, str], str]
-            Dictionary of query_name, query_text.
-            Name of container to add queries to.
+        pd.DataFrame
+            Passed through input DataFrame.
 
-        """
-        if not self.connected:
-            raise self._create_not_connected_err("Splunk")
-        if hasattr(self.service, "saved_searches") and self.service.saved_searches:
-            queries = {
-                search.name.strip().replace(" ", "_"): f"search {search['search']}"
-                for search in self.service.saved_searches
-            }
-            return queries, "SavedSearches"
-        return {}, "SavedSearches"
+        Notes
+        -----
+        This function runs the DataFrame method or accessor function.
+        It does not alter the DataFrame (unless the function does
+        any kind of in-place modification). The function is run and
+        the original input DataFrame is returned.
 
-    @property
-    def driver_queries(self) -> Iterable[Dict[str, Any]]:
         """
-        Return dynamic queries available on connection to service.
+        acc_name = func_name = func = None
+        if "." in df_func:
+            acc_name, func_name = df_func.split(".")
+            accessor = getattr(self._df, acc_name, None)
+            if accessor:
+                func = getattr(accessor, func_name, None)
+        else:
+            func = getattr(self._df, df_func, None)
+        if func:
+            # run the function with any additional args
+            func(*args, **kwargs)
+        return self._df
+
+    def filter_cols(
+        self,
+        cols: Union[str, Iterable[str]],
+        match_case: bool = False,
+        sort_cols: bool = False,
+    ) -> pd.DataFrame:
+        """
+        Filter output columns matching names in `cols` expression(s).
+
+        Parameters
+        ----------
+        cols : Union[str, Iterable[str]]
+            Either a string or a list of strings with filter expressions.
+            These can be exact matches for column names, wildcard patterns
+            ("*" matches multiple chars and "?" matches a single char),
+            or regular expressions.
+        match_case: bool, optional
+            Use case-sensitive matching, by default False
+        sort_cols : bool, optional
+            Alphabetically sort column names, by default False
 
         Returns
         -------
-        Iterable[Dict[str, Any]]
-            List of queries with properties: "name", "query", "container"
-            and (optionally) "description"
-
-        Raises
-        ------
-        MsticpyNotConnectedError
-            If called before driver is connected.
+        pd.DataFrame
+            The input DataFrame with only columns that match the
+            filtering expressions.
 
         """
-        if not self.connected:
-            raise self._create_not_connected_err("Splunk")
-        if hasattr(self.service, "saved_searches") and self.service.saved_searches:
-            return [
-                {
-                    "name": search.name.strip().replace(" ", "_"),
-                    "query": f"search {search['search']}",
-                    "query_paths": "SavedSearches",
-                    "description": "",
-                }
-                for search in self.service.saved_searches
-            ]
-        return []
+        curr_cols = self._df.columns
+        filt_cols: Set[str] = set()
+        if isinstance(cols, str):
+            filt_cols.update(_name_match(curr_cols, cols, match_case))
+        elif isinstance(cols, list):
+            for col_filter in cols:
+                filt_cols.update(_name_match(curr_cols, col_filter, match_case))
+        if not filt_cols:
+            raise ValueError("Column filter expression(s) did not match any columns")
 
-    @property
-    def _saved_searches(self) -> Union[pd.DataFrame, Any]:
+        if sort_cols:
+            out_cols = sorted(filt_cols)
+        else:
+            # keep the existing order
+            out_cols = [col for col in curr_cols if col in filt_cols]
+        return self._df[out_cols]
+
+    def filter(
+        self,
+        expr: Union[str, Number],
+        match_case: bool = False,
+        numeric_col: bool = False,
+    ) -> pd.DataFrame:
         """
-        Return list of saved searches in dataframe.
+        Filter all columns of DataFrame, return rows with any matches.
+
+        Parameters
+        ----------
+        expr : Union[str, Number]
+            String or regular expression to match or a (partial) number.
+            If `expr` is a string it is matched against any string or object
+            columns using pandas `str.contains(..regex=True)`
+            If `expr` is a number or if `numeric_col` is True, `expr`
+            is converted to a string and matched as a substring of any numeric
+            columns.
+        match_case : bool, optional
+            The match is not case-sensitive by default. Set to True to force
+            case-sensitive matches.
+        numeric_col : bool, optional
+            If `expr` is a numeric string or number this will force a match against
+            only numeric columns, by default False
 
         Returns
         -------
         pd.DataFrame
-            Dataframe with list of saved searches with name and query columns.
+            The filtered dataframe
+
+        Raises
+        ------
+        TypeError
+            If `expr` is neither a string or number.
 
         """
-        return self._get_saved_searches() if self.connected else None
+        if isinstance(expr, str) and not numeric_col:
+            text_cols = self._df.select_dtypes(include=[object, "string"])
+            return self._df[
+                text_cols.apply(
+                    lambda col: col.str.contains(
+                        expr, regex=True, case=match_case, na=False
+                    )
+                ).any(axis=1)
+            ]
+        if isinstance(expr, Number) or numeric_col:
+            num_cols = self._df.select_dtypes(include="number")
+            str_expr = str(expr)
+            return self._df[
+                num_cols.apply(
+                    lambda col: col.astype("string").str.contains(str_expr, regex=True)
+                ).any(axis=1)
+            ]
+        raise TypeError("expr '{expr}' must be a string or numeric type.")
 
-    def _get_saved_searches(self) -> Union[pd.DataFrame, Any]:
-        # sourcery skip: class-extract-method
+    def sort(
+        self, cols: Union[str, Iterable[str], Dict[str, str]], ascending: bool = None
+    ) -> pd.DataFrame:
         """
-        Return list of saved searches in dataframe.
+        Sort output by column expression.
+
+        Parameters
+        ----------
+        cols : Union[str, Iterable[str], Dict[str, str]]
+            If this is a string, then this should be a column name expression. A column name
+            expression is either a column name, a case-insenstive column name or a
+            regular expression to match one or more column names.
+            Each column name expression can be of
+            the format `col_name_expr:desc` to sort descending (`col_name_expr:asc` is the default).
+            The col_name can also be a regular expression or partial column name.
+            If this is a list, then each element should be a column name expression
+            with an optional ':asc' or ':desc' suffix.
+            If this is a dict, then the keys should be column name expressions and the
+            values bools indication 'ascending' (True) or 'descending' (False) sort.
+        ascending : [type], optional
+            Overrides any ordering specified for individual columns and sorts
+            'ascending' if True or 'descending' if False. If not supplied and no
+            column-specific ordering is supplied it sorts ascending.
 
         Returns
         -------
         pd.DataFrame
-            Dataframe with list of saved searches with name and query columns.
+            The sorted DataFrame
 
-        """
-        if not self.connected:
-            raise self._create_not_connected_err("Splunk")
-        savedsearches = self.service.saved_searches
-
-        out_df = pd.DataFrame(columns=["name", "query"])
+        Raises
+        ------
+        ValueError
+            One or more column expressions matched no column name in the input.
 
-        namelist = []
-        querylist = []
-        for savedsearch in savedsearches:
-            namelist.append(savedsearch.name.replace(" ", "_"))
-            querylist.append(savedsearch["search"])
-        out_df["name"] = namelist
-        out_df["query"] = querylist
+        """
+        if isinstance(cols, dict):
+            col_dict = cols
+        else:
+            if isinstance(cols, str):
+                col_list = [col.strip() for col in cols.split(",")]
+            else:
+                col_list = list(cols)
+            col_dict = {
+                col.split(":")[0].strip(): not col.casefold().endswith(":desc")
+                for col in col_list
+            }
 
-        return out_df
+        sort_cols = {}
+        # create case-insensitive mapping for DF cols
+        df_cols = {col.casefold(): col for col in self._df.columns}
+        for col in col_dict:
+            # Use case-matched name, if available
+            if col in self._df.columns:
+                sort_cols[col] = col_dict[col]
+                continue
+            # Look for case-insensitive match
+            df_col = df_cols.get(col.casefold())
+            if df_col:
+                sort_cols[col] = col_dict[col]
+                continue
+            # look for regex matches for col name
+            df_match_cols = [
+                df_cols[s_col]
+                for s_col in df_cols
+                if re.match(col, s_col, re.IGNORECASE)
+            ]
+            # we might get multiple matches
+            if df_match_cols:
+                sort_cols.update({df_col: col_dict[col] for df_col in df_match_cols})
+                continue
+            raise ValueError(
+                f"'{col}' column in sort list did not match any columns in input data."
+            )
+        # create the ascending parameter
+        asc_param = ascending if ascending is not None else list(sort_cols.values())
+        return self._df.sort_values(list(sort_cols.keys()), ascending=asc_param)
 
-    @property
-    def _fired_alerts(self) -> Union[pd.DataFrame, Any]:
+    def list_to_rows(self, cols: Union[str, Iterable[str]]) -> pd.DataFrame:
         """
-        Return list of fired alerts in dataframe.
+        Expand a list column to individual rows.
+
+        Parameters
+        ----------
+        cols : Union[str, Iterable[str]]
+            The columns to be expanded.
 
         Returns
         -------
         pd.DataFrame
-            Dataframe with list of fired alerts with alert name and count columns.
+            The expanded DataFrame
 
         """
-        return self._get_fired_alerts() if self.connected else None
+        orig_cols = self._df.columns
+        if parse_version(pd.__version__) >= parse_version("1.3.0"):
+            return self._df.explode(column=cols)
+        data = self._df
+        if isinstance(cols, str):
+            cols = [cols]
+        for col in cols:
+            item_col = f"{col}_list_item$$"
+            ren_col = {item_col: col}
+            data = (
+                pd.DataFrame(data[col].to_list(), index=data.index)
+                .replace([None], np.nan)  # convert any Nones to NaN
+                .merge(data, right_index=True, left_index=True)
+                .melt(id_vars=orig_cols, value_name=item_col)
+                .dropna(subset=[item_col])  # get rid of rows with NaNs in this col
+                .drop([col, "variable"], axis=1)
+                .rename(columns=ren_col)
+            )
+        return data
 
-    def _get_fired_alerts(self) -> Union[pd.DataFrame, Any]:
+    def parse_json(self, cols: Union[str, Iterable[str]]) -> pd.DataFrame:
         """
-        Return list of fired alerts in dataframe.
+        Convert JSON string columns to Python types.
+
+        Parameters
+        ----------
+        cols : Union[str, Iterable[str]]
+            Column or iterable of columns to process
 
         Returns
         -------
         pd.DataFrame
-            Dataframe with list of fired alerts with alert name and count columns.
+            Processed dataframe
 
         """
-        if not self.connected:
-            raise self._create_not_connected_err("Splunk")
-        firedalerts = self.service.fired_alerts
-
-        out_df = pd.DataFrame(columns=["name", "count"])
-
-        alert_names = []
-        alert_counts = []
-        for alert in firedalerts:
-            alert_names.append(alert.name)
-            alert_counts.append(alert.count)
-        out_df["name"] = alert_names
-        out_df["count"] = alert_counts
-
-        return out_df
-
-    # Parameter Formatting methods
-    @staticmethod
-    def _format_datetime(date_time: datetime) -> str:
-        """Return datetime-formatted string."""
-        return f'"{date_time.isoformat(sep=" ")}"'
-
-    @staticmethod
-    def _format_list(param_list: Iterable[Any]) -> str:
-        """Return formatted list parameter."""
-        fmt_list = [f'"{item}"' for item in param_list]
-        return ",".join(fmt_list)
+        if isinstance(cols, str):
+            cols = [cols]
+        data = self._df
+        for col in cols:
+            col_parsed = f"{col}_parsed"
+            data[col_parsed] = data[col].apply(_json_safe_conv)
+            data = data.drop([col], axis=1).rename(columns={col_parsed: col})
+        return data
+
+
+def _name_match(cur_cols: Iterable[str], col_filter, match_case):
+    col_filter = re.sub(r"[^.]\*", ".*", col_filter)
+    col_filter = re.sub(r"[^.]\?", ".?", col_filter)
+    regex_opts = [] if match_case else [re.IGNORECASE]
+    return {col for col in cur_cols if re.match(col_filter, col, *regex_opts)}
+
+
+def _json_safe_conv(val):
+    if val:
+        with contextlib.suppress(TypeError, JSONDecodeError):
+            return json.loads(val)
+    return val
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `msticpy-2.4.0/msticpy/data/drivers/sumologic_driver.py` & `msticpy-2.5.0/msticpy/data/drivers/sumologic_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from ...common.exceptions import (
     MsticpyConnectionError,
     MsticpyUserConfigError,
     MsticpyUserError,
 )
 from ...common.provider_settings import ProviderSettings, get_provider_settings
 from ...common.utility import check_kwargs, export
-from .driver_base import DriverBase, QuerySource
+from .driver_base import DriverBase, DriverProps, QuerySource
 
 __version__ = VERSION
 __author__ = "juju4"
 
 
 SUMOLOGIC_CONNECT_ARGS = {
     "connection_str": "(string) The url endpoint (the default is"
@@ -58,18 +58,18 @@
     def __init__(self, **kwargs):
         """Instantiate Sumologic Driver."""
         super().__init__(**kwargs)
         self.service = None
         self._loaded = True
         self._connected = False
         self._debug = kwargs.get("debug", False)
-        self.public_attribs = {
-            "client": self.service,
-        }
-        self.formatters = {"datetime": self._format_datetime}
+        self.set_driver_property(DriverProps.PUBLIC_ATTRS, {"client": self.service})
+        self.set_driver_property(
+            DriverProps.FORMATTERS, {"datetime": self._format_datetime}
+        )
         self.checkinterval = self._DEF_CHECKINTERVAL
         self.timeout = self._DEF_TIMEOUT
 
     def connect(self, connection_str: str = None, **kwargs):
         """
         Connect to Sumologic via sumologic-sdk.
```

### Comparing `msticpy-2.4.0/msticpy/data/queries/cybereason/cybereason_connections.yaml` & `msticpy-2.5.0/msticpy/data/queries/cybereason/cybereason_connections.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/cybereason/cybereason_hosts.yaml` & `msticpy-2.5.0/msticpy/data/queries/cybereason/cybereason_hosts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/cybereason/cybereason_processes.yaml` & `msticpy-2.5.0/msticpy/data/queries/cybereason/cybereason_processes.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/localdata/local_data.yaml` & `msticpy-2.5.0/msticpy/data/queries/localdata/local_data.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/m365d/kql_mdatp_alerts.yaml` & `msticpy-2.5.0/msticpy/data/queries/m365d/kql_mdatp_alerts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/m365d/kql_mdatp_file.yaml` & `msticpy-2.5.0/msticpy/data/queries/m365d/kql_mdatp_file.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/m365d/kql_mdatp_hunting.yaml` & `msticpy-2.5.0/msticpy/data/queries/m365d/kql_mdatp_hunting.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/m365d/kql_mdatp_network.yaml` & `msticpy-2.5.0/msticpy/data/queries/m365d/kql_mdatp_network.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/m365d/kql_mdatp_process.yaml` & `msticpy-2.5.0/msticpy/data/queries/m365d/kql_mdatp_process.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/m365d/kql_mdatp_user.yaml` & `msticpy-2.5.0/msticpy/data/queries/m365d/kql_mdatp_user.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mde/kql_mdatp_alerts.yaml` & `msticpy-2.5.0/msticpy/data/queries/mde/kql_mdatp_alerts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mde/kql_mdatp_file.yaml` & `msticpy-2.5.0/msticpy/data/queries/mde/kql_mdatp_file.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mde/kql_mdatp_hunting.yaml` & `msticpy-2.5.0/msticpy/data/queries/mde/kql_mdatp_hunting.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mde/kql_mdatp_network.yaml` & `msticpy-2.5.0/msticpy/data/queries/mde/kql_mdatp_network.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mde/kql_mdatp_process.yaml` & `msticpy-2.5.0/msticpy/data/queries/mde/kql_mdatp_process.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mde/kql_mdatp_user.yaml` & `msticpy-2.5.0/msticpy/data/queries/mde/kql_mdatp_user.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/msgraph/graph_alerts.yaml` & `msticpy-2.5.0/msticpy/data/queries/msgraph/graph_alerts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_alert.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_alert.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_azure.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_azure.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_net.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_net.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_o365.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_o365.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml` & `msticpy-2.5.0/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml` & `msticpy-2.5.0/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/resourcegraph/sentinel_resources.yaml` & `msticpy-2.5.0/msticpy/data/queries/resourcegraph/sentinel_resources.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/splunk/splunk_alert_queries.yaml` & `msticpy-2.5.0/msticpy/data/queries/splunk/splunk_alert_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/splunk/splunk_authentication_queries.yaml` & `msticpy-2.5.0/msticpy/data/queries/splunk/splunk_authentication_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/splunk/splunk_queries.yaml` & `msticpy-2.5.0/msticpy/data/queries/splunk/splunk_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/queries/sumologic/sumologic_queries.yaml` & `msticpy-2.5.0/msticpy/data/queries/sumologic/sumologic_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/query_container.py` & `msticpy-2.5.0/msticpy/data/query_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/query_defns.py` & `msticpy-2.5.0/msticpy/data/query_defns.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/sql_to_kql.py` & `msticpy-2.5.0/msticpy/data/sql_to_kql.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/storage/azure_blob_storage.py` & `msticpy-2.5.0/msticpy/data/storage/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/uploaders/__init__.py` & `msticpy-2.5.0/msticpy/data/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/uploaders/loganalytics_uploader.py` & `msticpy-2.5.0/msticpy/data/uploaders/loganalytics_uploader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/uploaders/splunk_uploader.py` & `msticpy-2.5.0/msticpy/data/uploaders/splunk_uploader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/data/uploaders/uploader_base.py` & `msticpy-2.5.0/msticpy/data/uploaders/uploader_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/__init__.py` & `msticpy-2.5.0/msticpy/datamodel/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/account.py` & `msticpy-2.5.0/msticpy/datamodel/entities/account.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/alert.py` & `msticpy-2.5.0/msticpy/datamodel/entities/alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/azure_resource.py` & `msticpy-2.5.0/msticpy/datamodel/entities/azure_resource.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/cloud_application.py` & `msticpy-2.5.0/msticpy/datamodel/entities/cloud_application.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/cloud_logon_session.py` & `msticpy-2.5.0/msticpy/datamodel/entities/cloud_logon_session.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/dns.py` & `msticpy-2.5.0/msticpy/datamodel/entities/dns.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/entity.py` & `msticpy-2.5.0/msticpy/datamodel/entities/entity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/entity_enums.py` & `msticpy-2.5.0/msticpy/datamodel/entities/entity_enums.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/entity_graph.py` & `msticpy-2.5.0/msticpy/datamodel/entities/entity_graph.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/file.py` & `msticpy-2.5.0/msticpy/datamodel/entities/file.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/file_hash.py` & `msticpy-2.5.0/msticpy/datamodel/entities/file_hash.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/geo_location.py` & `msticpy-2.5.0/msticpy/datamodel/entities/geo_location.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/graph_property.py` & `msticpy-2.5.0/msticpy/datamodel/entities/graph_property.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/host.py` & `msticpy-2.5.0/msticpy/datamodel/entities/host.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/host_logon_session.py` & `msticpy-2.5.0/msticpy/datamodel/entities/host_logon_session.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/iot_device.py` & `msticpy-2.5.0/msticpy/datamodel/entities/iot_device.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/ip_address.py` & `msticpy-2.5.0/msticpy/datamodel/entities/ip_address.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/mail_cluster.py` & `msticpy-2.5.0/msticpy/datamodel/entities/mail_cluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/mail_message.py` & `msticpy-2.5.0/msticpy/datamodel/entities/mail_message.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/mailbox.py` & `msticpy-2.5.0/msticpy/datamodel/entities/mailbox.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/malware.py` & `msticpy-2.5.0/msticpy/datamodel/entities/malware.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/network_connection.py` & `msticpy-2.5.0/msticpy/datamodel/entities/network_connection.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/process.py` & `msticpy-2.5.0/msticpy/datamodel/entities/process.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/registry_key.py` & `msticpy-2.5.0/msticpy/datamodel/entities/registry_key.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/registry_value.py` & `msticpy-2.5.0/msticpy/datamodel/entities/registry_value.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/security_group.py` & `msticpy-2.5.0/msticpy/datamodel/entities/security_group.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/submission_mail.py` & `msticpy-2.5.0/msticpy/datamodel/entities/submission_mail.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/threat_intelligence.py` & `msticpy-2.5.0/msticpy/datamodel/entities/threat_intelligence.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/unknown_entity.py` & `msticpy-2.5.0/msticpy/datamodel/entities/unknown_entity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/entities/url.py` & `msticpy-2.5.0/msticpy/datamodel/entities/url.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/pivot.py` & `msticpy-2.5.0/msticpy/datamodel/pivot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/soc/incident.py` & `msticpy-2.5.0/msticpy/datamodel/soc/incident.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/datamodel/soc/sentinel_alert.py` & `msticpy-2.5.0/msticpy/datamodel/soc/sentinel_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/__init__.py` & `msticpy-2.5.0/msticpy/init/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/azure_ml_tools.py` & `msticpy-2.5.0/msticpy/init/azure_ml_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     WorkingSet,
     parse_version,
 )
 
 from .._version import VERSION
 from ..common.pkg_config import _HOME_PATH, refresh_config
 from ..common.utility import search_for_file
-from ..config import MpConfigFile
+from ..config import MpConfigFile  # pylint: disable=no-name-in-module
 
 __version__ = VERSION
 
 logger = logging.getLogger(__name__)
 
 AZ_GET_STARTED = (
     "https://github.com/Azure/Azure-Sentinel-Notebooks/blob/master/A%20Getting"
```

### Comparing `msticpy-2.4.0/msticpy/init/azure_synapse_tools.py` & `msticpy-2.5.0/msticpy/init/azure_synapse_tools.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/logging.py` & `msticpy-2.5.0/msticpy/init/logging.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/mp_pandas_accessors.py` & `msticpy-2.5.0/msticpy/init/mp_pandas_accessors.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/nbinit.py` & `msticpy-2.5.0/msticpy/init/nbinit.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,26 +55,31 @@
 from typing import Any, Callable, Dict, List, Literal, Optional, Tuple
 
 import ipywidgets as widgets
 import pandas as pd
 from IPython import get_ipython
 from IPython.core.interactiveshell import InteractiveShell
 from IPython.display import HTML, display
-from matplotlib import MatplotlibDeprecationWarning
 
 try:
     import seaborn as sns
 except ImportError:
     sns = None
 
 from .._version import VERSION
 from ..auth.azure_auth_core import AzureCliStatus, check_cli_credentials
 from ..common.check_version import check_version
 from ..common.exceptions import MsticpyException, MsticpyUserError
-from ..common.pkg_config import _HOME_PATH, get_config, refresh_config, validate_config
+from ..common.pkg_config import _HOME_PATH
+from ..common.settings import (
+    current_config_path,
+    get_config,
+    refresh_config,
+    validate_config,
+)
 from ..common.utility import (
     check_and_install_missing_packages,
     check_kwargs,
     is_ipython,
     md,
     search_for_file,
     unit_testing,
@@ -178,16 +183,14 @@
     dict(pkg="pandas", alias="pd"),
     dict(pkg="IPython", tgt="get_ipython"),
     dict(pkg="IPython.display", tgt="display"),
     dict(pkg="IPython.display", tgt="HTML"),
     dict(pkg="IPython.display", tgt="Markdown"),
     dict(pkg="ipywidgets", alias="widgets"),
     dict(pkg="pathlib", tgt="Path"),
-    dict(pkg="matplotlib.pyplot", alias="plt"),
-    dict(pkg="matplotlib", tgt="MatplotlibDeprecationWarning"),
     dict(pkg="numpy", alias="np"),
 ]
 if sns is not None:
     _NB_IMPORTS.append(dict(pkg="seaborn", alias="sns"))
 
 _MP_IMPORTS = [
     dict(pkg="msticpy"),
@@ -208,16 +211,14 @@
     dict(pkg="msticpy.vis", tgt="nbdisplay"),
     dict(pkg="msticpy.init", tgt="mp_pandas_accessors"),
     dict(pkg="msticpy", tgt="nbwidgets"),
 ]
 
 _MP_IMPORT_ALL: List[Dict[str, str]] = [
     dict(module_name="msticpy.datamodel.entities"),
-    dict(module_name="msticpy.nbtools"),
-    dict(module_name="msticpy.sectools"),
 ]
 # pylint: enable=use-dict-literal
 
 _CONF_URI = (
     "https://msticpy.readthedocs.io/en/latest/getting_started/msticpyconfig.html"
 )
 
@@ -343,15 +344,15 @@
         Passing `False` for this parameter disables environment detection.
         Alternatively, you can pass a list of environments that you
         want to detect. Current supported environments are 'aml' (Azure
         Machine Learning) and 'synapse' (Azure Synapse).
 
     Raises
     ------
-    MsticpyException
+    MsticpyException :
         If extra_imports data format is incorrect.
         If package with required version check has no version
         information.
 
     Notes
     -----
     This module performs several steps to initialize MSTICPy:
@@ -666,21 +667,24 @@
         raise ValueError(f"Configuration file {config_file} not found")
     os.environ["MSTICPYCONFIG"] = config_file
     refresh_config()
 
 
 def _get_or_create_config() -> bool:
     # Cases
+    # 0. Current config file exists -> return ok
     # 1. Env var set and mpconfig exists -> goto 4
     # 2. Env var set and mpconfig file not exists - warn and continue
     # 3. search_for_file finds mpconfig -> goto 4
     # 4. if file and check_file_contents -> return ok
     # 5. search_for_file(config.json)
     # 6. If aml user try to import config.json into mpconfig and save
     # 7. Error - no Microsoft Sentinel config
+    if current_config_path() is not None:
+        return True
     mp_path = os.environ.get("MSTICPYCONFIG")
     if mp_path and not Path(mp_path).is_file():
         _err_output(_MISSING_MPCONFIG_ENV_ERR)
         logger.warning("MSTICPYCONFIG set to %s but no file found", mp_path)
     if not mp_path or not Path(mp_path).is_file():
         mp_path = search_for_file("msticpyconfig.yaml", paths=[".", _HOME_PATH])
 
@@ -723,17 +727,14 @@
 
 def _set_nb_options(namespace):
     namespace["WIDGET_DEFAULTS"] = {
         "layout": widgets.Layout(width="95%"),
         "style": {"description_width": "initial"},
     }
 
-    # Some of our dependencies (networkx) still use deprecated Matplotlib
-    # APIs - we can't do anything about it, so suppress them from view
-    warnings.simplefilter("ignore", category=MatplotlibDeprecationWarning)
     warnings.filterwarnings("ignore", category=DeprecationWarning)
     if sns:
         sns.set()
     pd.set_option("display.max_rows", 100)
     pd.set_option("display.max_columns", 50)
     pd.set_option("display.max_colwidth", 100)
```

### Comparing `msticpy-2.4.0/msticpy/init/nbmagics.py` & `msticpy-2.5.0/msticpy/init/nbmagics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/pivot.py` & `msticpy-2.5.0/msticpy/init/pivot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/pivot_core/pivot_browser.py` & `msticpy-2.5.0/msticpy/init/pivot_core/pivot_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/pivot_core/pivot_container.py` & `msticpy-2.5.0/msticpy/init/pivot_core/pivot_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/pivot_core/pivot_magic_core.py` & `msticpy-2.5.0/msticpy/init/pivot_core/pivot_magic_core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/pivot_core/pivot_pd_accessor.py` & `msticpy-2.5.0/msticpy/transform/auditdextract.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,456 +1,531 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-"""Pandas DataFrame accessor for Pivot functions."""
+"""
+Auditd extractor.
 
-import contextlib
-import json
+Module to load and decode Linux audit logs. It collapses messages
+sharing the same message ID into single events, decodes hex-encoded data
+fields and performs some event-specific formatting and normalization
+(e.g. for process start events it will re-assemble the process command
+line arguments into a single string). This is still a work-in-progress.
+
+"""
+import codecs
 import re
-import warnings
 from datetime import datetime
-from json import JSONDecodeError
-from numbers import Number
-from typing import Callable, Dict, Iterable, Set, Union
+from typing import Any, Dict, List, Mapping, Optional, Set, Tuple
 
-import numpy as np
 import pandas as pd
-from IPython import get_ipython
-from IPython.display import HTML, display
-from pkg_resources import parse_version
 
-from ..._version import VERSION
+from ..common.utility import export
+from .proc_tree_builder import build_process_tree
+
+try:
+    # pylint: disable=unused-import
+    from ..analysis import cluster_auditd  # type: ignore
+except ImportError:
+
+    def cluster_auditd(*args, **kwargs):  # type: ignore
+        """Fake cluster_auditd function for partial install."""
+        raise NotImplementedError("Cannot import auditd cluster module.")
+
+
+from .._version import VERSION
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
+# Constants
+# Fields that we know are frequently encoded
+_ENCODED_PARAMS: Dict[str, Set[str]] = {
+    "EXECVE": {"a0", "a1", "a2", "a3", "arch"},
+    "PROCTITLE": {"proctitle"},
+    "USER_CMD": {"cmd"},
+}
+
+# USER_START message schema
+_USER_START: Dict[str, Optional[str]] = {
+    "pid": "int",
+    "uid": "int",
+    "auid": "int",
+    "ses": "int",
+    "msg": None,
+    "acct": None,
+    "exe": None,
+    "hostname": None,
+    "addr": None,
+    "terminal": None,
+    "res": None,
+}
+
+# Message types schema
+_FIELD_DEFS: Dict[str, Dict[str, Optional[str]]] = {
+    "SYSCALL": {
+        "success": None,
+        "ppid": "int",
+        "pid": "int",
+        "auid": "int",
+        "uid": "int",
+        "gid": "int",
+        "euid": "int",
+        "egid": "int",
+        "ses": "int",
+        "exe": None,
+        "com": None,
+    },
+    "CWD": {"cwd": None},
+    "PROCTITLE": {"proctitle": None},
+    "LOGIN": {
+        "pid": "int",
+        "uid": "int",
+        "tty": None,
+        "old-ses": "int",
+        "ses": "int",
+        "res": None,
+    },
+    "EXECVE": {"argc": "int", "a0": None, "a1": None, "a2": None},
+    "_USER_START": _USER_START,
+    "USER_END": _USER_START,
+    "CRED_DISP": _USER_START,
+    "USER_ACCT": _USER_START,
+    "CRED_ACQ": _USER_START,
+    "USER_CMD": {
+        "pid": "int",
+        "uid": "int",
+        "auid": "int",
+        "ses": "int",
+        "msg": None,
+        "cmd": None,
+        "terminal": None,
+        "res": None,
+    },
+}
+
+
+@export
+def unpack_auditd(audit_str: List[Dict[str, str]]) -> Mapping[str, Mapping[str, Any]]:
+    """
+    Unpack an Audit message and returns a dictionary of fields.
+
+    Parameters
+    ----------
+    audit_str : str
+        The auditd raw record
+
+    Returns
+    -------
+    Mapping[str, Any]
+        The extracted message fields and values
+
+    """
+    event_dict: Dict[str, Dict[str, Any]] = {}
+    # The audit_str should be a list of dicts - '{EXECVE : {'p1': 'foo', p2: 'bar'...},
+    #                                      PATH: {'a1': 'xyz',....}}
+
+    for record in audit_str:
+        # process a single message type, splitting into type name
+        # and contents
+        for rec_key, rec_val in record.items():
+            rec_dict: Dict[str, Optional[str]] = {}
+            # Get our field mapping for encoded params for this
+            # mssg_type (rec_key)
+            encoded_fields_map = _ENCODED_PARAMS.get(rec_key, None)
+            for rec_item in rec_val:
+                # for each mssg item, split into k/v pair
+                rec_split = rec_item.split("=", maxsplit=1)
+                if len(rec_split) == 1:
+                    rec_dict[rec_split[0]] = None
+                    continue
+                if (
+                    not encoded_fields_map
+                    or rec_split[1].startswith('"')
+                    or rec_split[0] not in encoded_fields_map
+                ):
+                    field_value = rec_split[1].strip('"')
+                else:
+                    try:
+                        # Try to decode this from hex-string to text
+                        # Mypy thinks codecs.decode returns a str so
+                        # incorrectly issues a type warning - in this case it
+                        # will return a bytes string.
+                        field_value = codecs.decode(  # type: ignore
+                            bytes(rec_split[1], "utf-8"), "hex"
+                        ).decode("utf-8")
+                    except ValueError:
+                        field_value = rec_split[1]
+                        print(rec_val)
+                        print(
+                            "ERR:",
+                            rec_key,
+                            rec_split[0],
+                            rec_split[1],
+                            type(rec_split[1]),
+                        )
+                rec_dict[rec_split[0]] = field_value
+            event_dict[rec_key] = rec_dict
+
+    return event_dict
+
+
+def _extract_event(message_dict: Mapping[str, Any]) -> Tuple[str, Mapping[str, Any]]:
+    """
+    Assemble discrete messages sharing the same message Id into a single event.
+
+    Parameters
+    ----------
+    message_dict : Mapping[str, Any]
+        the input dictionary
+
+    Returns
+    -------
+    Tuple[str, Mapping[str, Any]
+        the assembled message type and contents
+
+    """
+    # Handle process executions specially
+    if "SYSCALL" in message_dict and "EXECVE" in message_dict:
+        proc_create_dict: Dict[str, Any] = {}
+        for mssg_type in ["SYSCALL", "CWD", "EXECVE", "PROCTITLE"]:
+            if mssg_type not in message_dict or mssg_type not in _FIELD_DEFS:
+                continue
+            _extract_mssg_value(mssg_type, message_dict, proc_create_dict)
 
-def _verbose_out(data, func, st_time, verbose=False, debug=False, **kwargs):
-    """Output verbose or debug info."""
-    end_time = datetime.now()
-
-    if verbose or debug:
-        print(f"{len(data)} rows returned from function {func.__name__}")
-    if debug:
-        print(f"Columns in result from function {func.__name__}:")
-        print(data.columns)
-        print(f"Execution time: {end_time - st_time}")
-        print(f"Parameters: {kwargs}")
-
-
-@pd.api.extensions.register_dataframe_accessor("mp_pivot")
-class PivotAccessor:
-    """Pandas api extension for Pivot functions."""
-
-    def __init__(self, pandas_obj):
-        """Instantiate pivot extension class."""
-        self._df = pandas_obj
-        self._ip = get_ipython()
-
-    def run(self, func: Callable[..., pd.DataFrame], **kwargs) -> pd.DataFrame:
-        """
-        Run a pivot function on the current DataFrame.
-
-        Parameters
-        ----------
-        func : Callable[..., pd.DataFrame]
-            Pivot function to run
-        kwargs:
-            Keyword arguments to pass to `func`.
-            A column specification (e.g. column="src_col_name")
-            is usually the minimum needed.
-            For data queries the `column` keyword must be the
-            name of the the query parameter (e.g. host_name = "src_col_name")
-
-        Returns
-        -------
-        pd.DataFrame
-            The output DataFrame from the function.
-
-        Notes
-        -----
-        You can pass the `join` keyword argument to most
-        pivot functions. Values for join are "inner", "left", "right"
-        or "outer".
-
-        """
-        st_time = datetime.now()
-        verbose = kwargs.pop("verbose", False)
-        debug = kwargs.pop("debug", False)
-        result = self._df.pipe((func, "data"), **kwargs)
-        if verbose or debug:
-            _verbose_out(
-                data=result,
-                func=func,
-                st_time=st_time,
-                verbose=verbose,
-                debug=debug,
-                **kwargs,
-            )
-        return result
-
-    def display(
-        self,
-        title: str = None,
-        cols: Iterable[str] = None,
-        query: str = None,
-        head: int = None,
-    ) -> pd.DataFrame:
-        """
-        Display the DataFrame in the middle of a pipeline.
-
-        Parameters
-        ----------
-        title : str, optional
-            Title to display for the DataFrame, by default None
-        cols : Iterable[str], optional
-            List of columns to display, by default None
-        query : str, optional
-            Query to filter the displayed data, by default None
-            This should be a string executable by the DataFrame.query
-            function
-        head : int, optional
-            Limit the displayed output to `head` rows, by default None
-
-        Returns
-        -------
-        pd.DataFrame
-            Passed through input DataFrame.
-
-        """
-        if title:
-            display(HTML(f"<h3>{title}</h3>"))
-        disp_df = self._df
-        if cols:
-            disp_df = disp_df[cols]
-        if query:
-            disp_df = disp_df.query(query)  # , parser='python', engine='python')
-        if head:
-            disp_df = disp_df.head(head)
-        display(disp_df)
-        return self._df
-
-    def tee(self, var_name: str, clobber: bool = False) -> pd.DataFrame:
-        """
-        Save current dataframe to `var_name` in the IPython user namespace.
-
-        Parameters
-        ----------
-        var_name : str
-            The name of the DF variable to create.
-        clobber : bool, optional
-            Whether to overwrite an existing variable of the same name,
-            by default False
-
-        Returns
-        -------
-        pd.DataFrame
-            Passed through input DataFrame.
-
-        Notes
-        -----
-        This function only works in an IPython/Jupyter notebook environment.
-        It will attempt to create a variable in the user local namespace
-        that references the current state of the DataFrame in the pipeline.
-
-        By default it will not overwrite an existing variable of the same
-        name (specify `clobber=True` to overwrite)
-
-        """
-        if self._ip and var_name:
-            if var_name in self._ip.ns_table["user_local"] and not clobber:
-                warnings.warn(f"Did not overwrite existing {var_name} in namespace")
-            else:
-                self._ip.ns_table["user_local"][var_name] = self._df
-        return self._df
-
-    def tee_exec(self, df_func: str, *args, **kwargs) -> pd.DataFrame:
-        """
-        Run a dataframe method on the dataframe without changing it.
-
-        Parameters
-        ----------
-        df_func : str
-            The name of the function to execute. Accessor methods
-            must be of the form "accessor.method".
-        args : tuple
-            Positional arguments to be passed to the function
-        kwargs : dict
-            Keyword arguments to be passed to the function.
-
-        Returns
-        -------
-        pd.DataFrame
-            Passed through input DataFrame.
-
-        Notes
-        -----
-        This function runs the DataFrame method or accessor function.
-        It does not alter the DataFrame (unless the function does
-        any kind of in-place modification). The function is run and
-        the original input DataFrame is returned.
-
-        """
-        acc_name = func_name = func = None
-        if "." in df_func:
-            acc_name, func_name = df_func.split(".")
-            accessor = getattr(self._df, acc_name, None)
-            if accessor:
-                func = getattr(accessor, func_name, None)
-        else:
-            func = getattr(self._df, df_func, None)
-        if func:
-            # run the function with any additional args
-            func(*args, **kwargs)
-        return self._df
-
-    def filter_cols(
-        self,
-        cols: Union[str, Iterable[str]],
-        match_case: bool = False,
-        sort_cols: bool = False,
-    ) -> pd.DataFrame:
-        """
-        Filter output columns matching names in `cols` expression(s).
-
-        Parameters
-        ----------
-        cols : Union[str, Iterable[str]]
-            Either a string or a list of strings with filter expressions.
-            These can be exact matches for column names, wildcard patterns
-            ("*" matches multiple chars and "?" matches a single char),
-            or regular expressions.
-        match_case: bool, optional
-            Use case-sensitive matching, by default False
-        sort_cols : bool, optional
-            Alphabetically sort column names, by default False
-
-        Returns
-        -------
-        pd.DataFrame
-            The input DataFrame with only columns that match the
-            filtering expressions.
-
-        """
-        curr_cols = self._df.columns
-        filt_cols: Set[str] = set()
-        if isinstance(cols, str):
-            filt_cols.update(_name_match(curr_cols, cols, match_case))
-        elif isinstance(cols, list):
-            for col_filter in cols:
-                filt_cols.update(_name_match(curr_cols, col_filter, match_case))
-        if not filt_cols:
-            raise ValueError("Column filter expression(s) did not match any columns")
-
-        if sort_cols:
-            out_cols = sorted(filt_cols)
+            if mssg_type == "EXECVE":
+                args = int(proc_create_dict.get("argc", 1))
+                arg_strs = [
+                    proc_create_dict.get(f"a{arg_idx}", "") for arg_idx in range(args)
+                ]
+                proc_create_dict["cmdline"] = " ".join(arg_strs)
+        return "SYSCALL_EXECVE", proc_create_dict
+
+    event_dict: Dict[str, Any] = {}
+    for mssg_type, _ in message_dict.items():
+        if mssg_type in _FIELD_DEFS:
+            _extract_mssg_value(mssg_type, message_dict, event_dict)
         else:
-            # keep the existing order
-            out_cols = [col for col in curr_cols if col in filt_cols]
-        return self._df[out_cols]
-
-    def filter(
-        self,
-        expr: Union[str, Number],
-        match_case: bool = False,
-        numeric_col: bool = False,
-    ) -> pd.DataFrame:
-        """
-        Filter all columns of DataFrame, return rows with any matches.
-
-        Parameters
-        ----------
-        expr : Union[str, Number]
-            String or regular expression to match or a (partial) number.
-            If `expr` is a string it is matched against any string or object
-            columns using pandas `str.contains(..regex=True)`
-            If `expr` is a number or if `numeric_col` is True, `expr`
-            is converted to a string and matched as a substring of any numeric
-            columns.
-        match_case : bool, optional
-            The match is not case-sensitive by default. Set to True to force
-            case-sensitive matches.
-        numeric_col : bool, optional
-            If `expr` is a numeric string or number this will force a match against
-            only numeric columns, by default False
-
-        Returns
-        -------
-        pd.DataFrame
-            The filtered dataframe
-
-        Raises
-        ------
-        TypeError
-            If `expr` is neither a string or number.
-
-        """
-        if isinstance(expr, str) and not numeric_col:
-            text_cols = self._df.select_dtypes(include=[object, "string"])
-            return self._df[
-                text_cols.apply(
-                    lambda col: col.str.contains(
-                        expr, regex=True, case=match_case, na=False
-                    )
-                ).any(axis=1)
-            ]
-        if isinstance(expr, Number) or numeric_col:
-            num_cols = self._df.select_dtypes(include="number")
-            str_expr = str(expr)
-            return self._df[
-                num_cols.apply(
-                    lambda col: col.astype("string").str.contains(str_expr, regex=True)
-                ).any(axis=1)
-            ]
-        raise TypeError("expr '{expr}' must be a string or numeric type.")
-
-    def sort(
-        self, cols: Union[str, Iterable[str], Dict[str, str]], ascending: bool = None
-    ) -> pd.DataFrame:
-        """
-        Sort output by column expression.
-
-        Parameters
-        ----------
-        cols : Union[str, Iterable[str], Dict[str, str]]
-            If this is a string, then this should be a column name expression. A column name
-            expression is either a column name, a case-insenstive column name or a
-            regular expression to match one or more column names.
-            Each column name expression can be of
-            the format `col_name_expr:desc` to sort descending (`col_name_expr:asc` is the default).
-            The col_name can also be a regular expression or partial column name.
-            If this is a list, then each element should be a column name expression
-            with an optional ':asc' or ':desc' suffix.
-            If this is a dict, then the keys should be column name expressions and the
-            values bools indication 'ascending' (True) or 'descending' (False) sort.
-        ascending : [type], optional
-            Overrides any ordering specified for individual columns and sorts
-            'ascending' if True or 'descending' if False. If not supplied and no
-            column-specific ordering is supplied it sorts ascending.
-
-        Returns
-        -------
-        pd.DataFrame
-            The sorted DataFrame
-
-        Raises
-        ------
-        ValueError
-            One or more column expressions matched no column name in the input.
-
-        """
-        if isinstance(cols, dict):
-            col_dict = cols
+            # We don't check for duplicated keys here - if
+            # there are multiple messages with the same key, the
+            # last one will overwrite the previous value
+            event_dict.update(message_dict[mssg_type])
+    return list(message_dict.keys())[0], event_dict
+
+
+def _extract_mssg_value(
+    mssg_type: str,
+    message_dict: Mapping[str, Mapping[str, Any]],
+    event_dict: Dict[str, Any],
+):
+    """
+    Extract field/value from the message dictionary.
+
+    Parameters
+    ----------
+    mssg_type : str
+        The Audit message type
+    message_dict : Mapping[str, str]
+        The input dictionary
+    event_dict : Dict[str, Any]
+        The output dictionary
+
+    """
+    # if the field requires conversion conv will specify the
+    # target type - only int currently
+    for fieldname, conv in _FIELD_DEFS[mssg_type].items():
+        value = message_dict[mssg_type].get(fieldname, None)
+        if not value:
+            return
+        if conv and conv == "int":
+            value = int(value)
+            if value == 4294967295:
+                value = -1
+        if fieldname in event_dict:
+            event_dict[f"{fieldname}_{mssg_type}"] = value
         else:
-            if isinstance(cols, str):
-                col_list = [col.strip() for col in cols.split(",")]
-            else:
-                col_list = list(cols)
-            col_dict = {
-                col.split(":")[0].strip(): not col.casefold().endswith(":desc")
-                for col in col_list
-            }
-
-        sort_cols = {}
-        # create case-insensitive mapping for DF cols
-        df_cols = {col.casefold(): col for col in self._df.columns}
-        for col in col_dict:
-            # Use case-matched name, if available
-            if col in self._df.columns:
-                sort_cols[col] = col_dict[col]
-                continue
-            # Look for case-insensitive match
-            df_col = df_cols.get(col.casefold())
-            if df_col:
-                sort_cols[col] = col_dict[col]
-                continue
-            # look for regex matches for col name
-            df_match_cols = [
-                df_cols[s_col]
-                for s_col in df_cols
-                if re.match(col, s_col, re.IGNORECASE)
-            ]
-            # we might get multiple matches
-            if df_match_cols:
-                sort_cols.update({df_col: col_dict[col] for df_col in df_match_cols})
-                continue
-            raise ValueError(
-                f"'{col}' column in sort list did not match any columns in input data."
-            )
-        # create the ascending parameter
-        asc_param = ascending if ascending is not None else list(sort_cols.values())
-        return self._df.sort_values(list(sort_cols.keys()), ascending=asc_param)
-
-    def list_to_rows(self, cols: Union[str, Iterable[str]]) -> pd.DataFrame:
-        """
-        Expand a list column to individual rows.
-
-        Parameters
-        ----------
-        cols : Union[str, Iterable[str]]
-            The columns to be expanded.
-
-        Returns
-        -------
-        pd.DataFrame
-            The expanded DataFrame
-
-        """
-        orig_cols = self._df.columns
-        if parse_version(pd.__version__) >= parse_version("1.3.0"):
-            return self._df.explode(column=cols)
-        data = self._df
-        if isinstance(cols, str):
-            cols = [cols]
-        for col in cols:
-            item_col = f"{col}_list_item$$"
-            ren_col = {item_col: col}
-            data = (
-                pd.DataFrame(data[col].to_list(), index=data.index)
-                .replace([None], np.nan)  # convert any Nones to NaN
-                .merge(data, right_index=True, left_index=True)
-                .melt(id_vars=orig_cols, value_name=item_col)
-                .dropna(subset=[item_col])  # get rid of rows with NaNs in this col
-                .drop([col, "variable"], axis=1)
-                .rename(columns=ren_col)
-            )
-        return data
-
-    def parse_json(self, cols: Union[str, Iterable[str]]) -> pd.DataFrame:
-        """
-        Convert JSON string columns to Python types.
-
-        Parameters
-        ----------
-        cols : Union[str, Iterable[str]]
-            Column or iterable of columns to process
-
-        Returns
-        -------
-        pd.DataFrame
-            Processed dataframe
-
-        """
-        if isinstance(cols, str):
-            cols = [cols]
-        data = self._df
-        for col in cols:
-            col_parsed = f"{col}_parsed"
-            data[col_parsed] = data[col].apply(_json_safe_conv)
-            data = data.drop([col], axis=1).rename(columns={col_parsed: col})
-        return data
-
-
-def _name_match(cur_cols: Iterable[str], col_filter, match_case):
-    col_filter = re.sub(r"[^.]\*", ".*", col_filter)
-    col_filter = re.sub(r"[^.]\?", ".?", col_filter)
-    regex_opts = [] if match_case else [re.IGNORECASE]
-    return {col for col in cur_cols if re.match(col_filter, col, *regex_opts)}
-
-
-def _json_safe_conv(val):
-    if val:
-        with contextlib.suppress(TypeError, JSONDecodeError):
-            return json.loads(val)
-    return val
+            event_dict[fieldname] = value
+
+
+def _move_cols_to_front(data: pd.DataFrame, column_count: int = 1) -> pd.DataFrame:
+    """
+    Move N columns from end to front of DataFrame.
+
+    Parameters
+    ----------
+    data : pd.DataFrame
+        The input DataFrame
+    column_count : int, optional
+        The number of columns to move (the default is 1)
+
+    Returns
+    -------
+    pd.DataFrame
+        DataFrame with `column_count` columns shifted to front
+
+    """
+    return data[list(data.columns[-column_count:]) + list(data.columns[:-column_count])]
+
+
+@export
+def extract_events_to_df(
+    data: pd.DataFrame,
+    input_column: str = "AuditdMessage",
+    event_type: str = None,
+    verbose: bool = False,
+) -> pd.DataFrame:
+    """
+    Extract auditd raw messages into a dataframe.
+
+    Parameters
+    ----------
+    data : pd.DataFrame
+        The input dataframe with raw auditd data in
+        a single string column
+    input_column : str, optional
+        the input column name (the default is 'AuditdMessage')
+    event_type : str, optional
+        the event type, if None, defaults to all (the default is None)
+    verbose : bool, optional
+        Give feedback on stages of processing (the default is False)
+
+    Returns
+    -------
+    pd.DataFrame
+        The resultant DataFrame
+
+    """
+    if verbose:
+        start_time = datetime.utcnow()
+        print(f"Unpacking auditd messages for {len(data)} events...")
+
+    # If the provided table has auditd messages as a string format and
+    # extract key elements.
+    if isinstance(data[input_column].head(1)[0], str):
+        data["mssg_id"] = data.apply(
+            lambda x: _extract_timestamp(x[input_column]), axis=1
+        )
+        data[input_column] = data.apply(
+            lambda x: _parse_audit_message(x[input_column]), axis=1
+        )
+
+    # Our first pandas expression does most of the work - unpacking the
+    # column contents, then extracting these into a two columns
+    # EventType (the main auditd mssg type) and a dict of k/v values
+    # EventData
+    tmp_df = data.apply(
+        lambda x: _extract_event(unpack_auditd(x[input_column])),
+        axis=1,
+        result_type="expand",
+    ).rename(columns={0: "EventType", 1: "EventData"})
+    # if only one type of event is requested
+    if event_type:
+        tmp_df = tmp_df.loc[tmp_df["EventType"] == event_type]
+        if verbose:
+            print(f"Event subset = {event_type} (events: {len(tmp_df)})")
+
+    if verbose:
+        print("Building output dataframe...")
+
+    # We convert the EventData dict into a series,
+    # then merge with:
+    # First - the intermediate input DF to add back the EventType column
+    # Second - the original input DF to add back metadata columns like Computer
+    # Finally get rid of any empty columns
+    tmp_df = (
+        tmp_df.apply(lambda x: pd.Series(x.EventData), axis=1)
+        .merge(tmp_df[["EventType"]], left_index=True, right_index=True)
+        .merge(
+            data.drop([input_column], axis=1),
+            how="inner",
+            left_index=True,
+            right_index=True,
+        )
+        .dropna(axis=1, how="all")
+    )
+
+    if verbose:
+        print("Fixing timestamps...")
+
+    # extract real timestamp from mssg_id
+    tmp_df["TimeStamp"] = tmp_df.apply(
+        lambda x: datetime.utcfromtimestamp(float(x["mssg_id"].split(":")[0])), axis=1
+    )
+    if "TimeGenerated" in tmp_df:
+        tmp_df = tmp_df.drop(["TimeGenerated"], axis=1)
+    tmp_df = tmp_df.rename(columns={"TimeStamp": "TimeGenerated"}).pipe(
+        _move_cols_to_front, column_count=5
+    )
+    if verbose:
+        print(f"Complete. {len(tmp_df)} output rows", end=" ")
+        delta = datetime.utcnow() - start_time
+        print(f"time: {delta.seconds + delta.microseconds/1_000_000} sec")
+
+    return tmp_df
+
+
+@export
+def get_event_subset(data: pd.DataFrame, event_type: str) -> pd.DataFrame:
+    """
+    Return a subset of the events matching type event_type.
+
+    Parameters
+    ----------
+    data : pd.DataFrame
+        The input data
+    event_type : str
+        The event type to select
+
+    Returns
+    -------
+    pd.DataFrame
+        The subset of the data where
+        data['EventType'] == event_type
+
+    """
+    return (
+        data[data["EventType"] == event_type].dropna(axis=1, how="all").infer_objects()
+    )
+
+
+@export
+def read_from_file(
+    filepath: str, event_type: str = None, verbose: bool = False, dummy_sep: str = "\t"
+) -> pd.DataFrame:
+    r"""
+    Extract Audit events from a log file.
+
+    Parameters
+    ----------
+    filepath : str
+        path to the input file
+    event_type : str, optional
+        The type of event to extract if only a subset required.
+        (the default is None, which processes all types)
+    verbose : bool, optional
+        If true more progress messages are output
+        (the default is False)
+    dummy_sep : str, optional
+        Separator to use for reading the 'csv' file
+        (default is tab - '\t')
+
+    Returns
+    -------
+    pd.DataFrame
+        The output DataFrame
+
+    Notes
+    -----
+    The dummy_sep parameter should be a character that does not
+    occur in an input line. This function uses pandas read_csv
+    to read the audit lines into a single column. Using a separator
+    that does appear in the input (e.g. space or comma) will cause
+    data to be parsed into multiple columns and anything after the
+    first separator in a line will be lost.
+
+    """
+    # read in the file using pd.read_csv()
+    df_raw: pd.DataFrame = pd.read_csv(
+        filepath, sep=dummy_sep, names=["raw_data"], skip_blank_lines=True
+    )
+
+    # extract message ID into separate column
+    df_raw["mssg_id"] = df_raw.apply(
+        lambda x: _extract_timestamp(x["raw_data"]), axis=1
+    )
+    # pylint: disable=unsupported-assignment-operation, no-member
+    # Pack message type and content into a dictionary:
+    # {'mssg_type: ['item1=x, item2=y....]}
+    df_raw["AuditdMessage"] = df_raw.apply(
+        lambda x: _parse_audit_message(x["raw_data"]), axis=1
+    )
+
+    # Group the data by message id string and concatenate the message content
+    # dictionaries in a list.
+    df_grouped_cols = (
+        df_raw.groupby(["mssg_id"]).agg({"AuditdMessage": list}).reset_index()
+    )
+    # pylint: enable=unsupported-assignment-operation, no-member
+
+    # pass this DataFrame to the event extractor.
+    return extract_events_to_df(
+        data=df_grouped_cols,
+        input_column="AuditdMessage",
+        event_type=event_type,
+        verbose=verbose,
+    )
+
+
+def _parse_audit_message(audit_str: str) -> Dict[str, List[str]]:
+    """
+    Parse an auditd message string into Dict format required by unpack_auditd.
+
+    Parameters
+    ----------
+    audit_str : str
+        The Audit message
+
+    Returns
+    -------
+    Dict[str, str]
+        The extracted message values
+
+    """
+    audit_message = audit_str.rstrip().split(": ")
+    audit_headers = audit_message[0]
+    audit_hdr_match = re.match(r"type=([^\s]+)", audit_headers)
+    if audit_hdr_match:
+        return {audit_hdr_match.group(1): audit_message[1].split(" ")}
+    return {}  # type ignore
+
+
+def _extract_timestamp(audit_str: str) -> str:
+    """
+    Parse an auditd message string and extract the message time.
+
+    Parameters
+    ----------
+    audit_str : str
+        The Audit message
+
+    Returns
+    -------
+    str
+        The extracted message time string
+
+    """
+    audit_message = audit_str.rstrip().split(": ")
+    audit_headers = audit_message[0]
+    audit_hdr_match = re.match(r".*msg=audit\(([^\)]+)\)", audit_headers)
+    if audit_hdr_match:
+        return audit_hdr_match.group(1).split(":")[0]
+    return ""
+
+
+# pylint: disable=too-many-branches
+@export
+def generate_process_tree(  # noqa: MC0001
+    audit_data: pd.DataFrame, branch_depth: int = 4, processes: pd.DataFrame = None
+) -> pd.DataFrame:
+    """
+    Generate process tree data from auditd logs.
+
+    Parameters
+    ----------
+    audit_data : pd.DataFrame
+        The Audit data containing process creation events
+    branch_depth: int, optional
+        The maximum depth of parent or child processes to extract from the data
+        (The default is 4)
+    processes: pd.DataFrame, optional
+        Dataframe of processes to generate tree for
+
+    Returns
+    -------
+    pd.DataFrame
+        The formatted process tree data
+
+    """
+    # Superceded by process_tree_utils module
+    del branch_depth, processes
+    return build_process_tree(audit_data)
```

### Comparing `msticpy-2.4.0/msticpy/init/pivot_core/pivot_pipeline.py` & `msticpy-2.5.0/msticpy/init/pivot_core/pivot_pipeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/pivot_core/pivot_register.py` & `msticpy-2.5.0/msticpy/init/pivot_core/pivot_register.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/pivot_core/pivot_register_reader.py` & `msticpy-2.5.0/msticpy/init/pivot_core/pivot_register_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/pivot_init/pivot_data_queries.py` & `msticpy-2.5.0/msticpy/init/pivot_init/pivot_data_queries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/pivot_init/pivot_ti_provider.py` & `msticpy-2.5.0/msticpy/init/pivot_init/pivot_ti_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/pivot_init/vt_pivot.py` & `msticpy-2.5.0/msticpy/init/pivot_init/vt_pivot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/init/user_config.py` & `msticpy-2.5.0/msticpy/init/user_config.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/__init__.py` & `msticpy-2.5.0/msticpy/nbtools/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/data_viewer.py` & `msticpy-2.5.0/msticpy/nbtools/data_viewer.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/entityschema.py` & `msticpy-2.5.0/msticpy/nbtools/entityschema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/foliummap.py` & `msticpy-2.5.0/msticpy/nbtools/foliummap.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/morph_charts.py` & `msticpy-2.5.0/msticpy/nbtools/morph_charts.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/nbdisplay.py` & `msticpy-2.5.0/msticpy/nbtools/nbdisplay.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/nbwidgets.py` & `msticpy-2.5.0/msticpy/nbtools/nbwidgets.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/observationlist.py` & `msticpy-2.5.0/msticpy/nbtools/observationlist.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/process_tree.py` & `msticpy-2.5.0/msticpy/nbtools/process_tree.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/security_alert.py` & `msticpy-2.5.0/msticpy/nbtools/security_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/security_alert_graph.py` & `msticpy-2.5.0/msticpy/nbtools/security_alert_graph.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/security_base.py` & `msticpy-2.5.0/msticpy/nbtools/security_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/security_event.py` & `msticpy-2.5.0/msticpy/nbtools/security_event.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/ti_browser.py` & `msticpy-2.5.0/msticpy/nbtools/ti_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/timeline.py` & `msticpy-2.5.0/msticpy/nbtools/timeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/timeline_duration.py` & `msticpy-2.5.0/msticpy/nbtools/timeline_duration.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/timeline_pd_accessor.py` & `msticpy-2.5.0/msticpy/nbtools/timeline_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/timeseries.py` & `msticpy-2.5.0/msticpy/nbtools/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/utility.py` & `msticpy-2.5.0/msticpy/nbtools/utility.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbtools/wsconfig.py` & `msticpy-2.5.0/msticpy/nbtools/wsconfig.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbwidgets/__init__.py` & `msticpy-2.5.0/msticpy/nbwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbwidgets/core.py` & `msticpy-2.5.0/msticpy/nbwidgets/core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbwidgets/get_environment_key.py` & `msticpy-2.5.0/msticpy/nbwidgets/get_environment_key.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbwidgets/get_text.py` & `msticpy-2.5.0/msticpy/nbwidgets/get_text.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbwidgets/lookback.py` & `msticpy-2.5.0/msticpy/nbwidgets/lookback.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbwidgets/option_buttons.py` & `msticpy-2.5.0/msticpy/nbwidgets/option_buttons.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbwidgets/progress.py` & `msticpy-2.5.0/msticpy/nbwidgets/progress.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbwidgets/query_time.py` & `msticpy-2.5.0/msticpy/nbwidgets/query_time.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbwidgets/select_alert.py` & `msticpy-2.5.0/msticpy/nbwidgets/select_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbwidgets/select_item.py` & `msticpy-2.5.0/msticpy/nbwidgets/select_item.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/nbwidgets/select_subset.py` & `msticpy-2.5.0/msticpy/nbwidgets/select_subset.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/resources/WinSecurityEvent.json` & `msticpy-2.5.0/msticpy/resources/WinSecurityEvent.json`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/resources/mp_pivot_reg.yaml` & `msticpy-2.5.0/msticpy/resources/mp_pivot_reg.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/resources/mpconfig_defaults.yaml` & `msticpy-2.5.0/msticpy/resources/mpconfig_defaults.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,19 @@
       AuthKey: *cred_key
   IntSights:
     Primary: bool(default=True)
     Provider: "IntSights"
     Args:
       ApiID: str()
       AuthKey: *cred_key
+  Pulsedive:
+    Args:
+      AuthKey: *cred_key
+    Primary: bool(default=False)
+    Provider: "Pulsedive"
 OtherProviders:
   GeoIPLite:
     Args:
       AuthKey: *cred_key
       DBFolder: str(default="~/.msticpy")
     Provider: "GeoLiteLookup"
   IPStack:
@@ -189,14 +194,19 @@
     Args:
       Cluster: str()
       TenantId: str(format=uuid)
       IntegratedAuth: bool()
       ClientId: str(required=False, format=uuid)
       # [SuppressMessage("Microsoft.Security", "CS002:SecretInNextLine", Justification="Test code")]
       ClientSecret: *cred_key_opt
+msticpy:
+  FriendlyExceptions: bool(default=True, required=False)
+  QueryDefinitions: list(required=False)
+  http_timeout: int(required=False)
+  # Proxies key not yet supported
 AzureCLI:
   # Deprecated section - use DataProviders.AzureCLI
   Args:
     auth_methods: m_enum(required=False,
       options=[env; msi; cli; devicecode; interactive; vscode; powershell; clientsecret; certificate],
       default=["cli"; "msi", "interactive"]
       )
```

### Comparing `msticpy-2.4.0/msticpy/resources/obfuscation_cols.yaml` & `msticpy-2.5.0/msticpy/resources/obfuscation_cols.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/__init__.py` & `msticpy-2.5.0/msticpy/sectools/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/auditdextract.py` & `msticpy-2.5.0/msticpy/sectools/auditdextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/base64unpack.py` & `msticpy-2.5.0/msticpy/sectools/base64unpack.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/cmd_line.py` & `msticpy-2.5.0/msticpy/sectools/cmd_line.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/domain_utils.py` & `msticpy-2.5.0/msticpy/sectools/domain_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/eventcluster.py` & `msticpy-2.5.0/msticpy/sectools/eventcluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/geoip.py` & `msticpy-2.5.0/msticpy/sectools/geoip.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/iocextract.py` & `msticpy-2.5.0/msticpy/sectools/iocextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/ip_utils.py` & `msticpy-2.5.0/msticpy/sectools/ip_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/proc_tree_build_mde.py` & `msticpy-2.5.0/msticpy/sectools/proc_tree_build_mde.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/proc_tree_build_winlx.py` & `msticpy-2.5.0/msticpy/sectools/proc_tree_build_winlx.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/proc_tree_builder.py` & `msticpy-2.5.0/msticpy/sectools/proc_tree_builder.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/proc_tree_schema.py` & `msticpy-2.5.0/msticpy/sectools/proc_tree_schema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/proc_tree_utils.py` & `msticpy-2.5.0/msticpy/sectools/proc_tree_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/sectools_magics.py` & `msticpy-2.5.0/msticpy/sectools/sectools_magics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/syslog_utils.py` & `msticpy-2.5.0/msticpy/sectools/syslog_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/tilookup.py` & `msticpy-2.5.0/msticpy/sectools/tilookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/tiproviders/ti_provider_base.py` & `msticpy-2.5.0/msticpy/sectools/tiproviders/ti_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/vtlookup.py` & `msticpy-2.5.0/msticpy/sectools/vtlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/vtlookupv3/__init__.py` & `msticpy-2.5.0/msticpy/sectools/vtlookupv3/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/vtlookupv3/vtfile_behavior.py` & `msticpy-2.5.0/msticpy/sectools/vtlookupv3/vtfile_behavior.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/vtlookupv3/vtlookupv3.py` & `msticpy-2.5.0/msticpy/sectools/vtlookupv3/vtlookupv3.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/sectools/vtlookupv3/vtobject_browser.py` & `msticpy-2.5.0/msticpy/sectools/vtlookupv3/vtobject_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/transform/auditdextract.py` & `msticpy-2.5.0/msticpy/data/drivers/splunk_driver.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,531 +1,513 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for
-# license information.
-# --------------------------------------------------------------------------
-"""
-Auditd extractor.
-
-Module to load and decode Linux audit logs. It collapses messages
-sharing the same message ID into single events, decodes hex-encoded data
-fields and performs some event-specific formatting and normalization
-(e.g. for process start events it will re-assemble the process command
-line arguments into a single string). This is still a work-in-progress.
-
-"""
-import codecs
-import re
-from datetime import datetime
-from typing import Any, Dict, List, Mapping, Optional, Set, Tuple
+#  -------------------------------------------------------------------------
+#  Copyright (c) Microsoft Corporation. All rights reserved.
+#  Licensed under the MIT License. See License.txt in the project root for
+#  license information.
+#  --------------------------------------------------------------------------
+"""Splunk Driver class."""
+import logging
+from datetime import datetime, timedelta
+from time import sleep
+from typing import Any, Dict, Iterable, Optional, Tuple, Union
 
 import pandas as pd
+from tqdm import tqdm
 
-from ..common.utility import export
-from .proc_tree_builder import build_process_tree
+from ..._version import VERSION
+from ...common.exceptions import (
+    MsticpyConnectionError,
+    MsticpyDataQueryError,
+    MsticpyImportExtraError,
+    MsticpyUserConfigError,
+)
+from ...common.utility import check_kwargs, export
+from ..core.query_defns import Formatters
+from .driver_base import DriverBase, DriverProps, QuerySource
 
 try:
-    # pylint: disable=unused-import
-    from ..analysis import cluster_auditd  # type: ignore
-except ImportError:
-
-    def cluster_auditd(*args, **kwargs):  # type: ignore
-        """Fake cluster_auditd function for partial install."""
-        raise NotImplementedError("Cannot import auditd cluster module.")
-
-
-from .._version import VERSION
+    import splunklib.client as sp_client
+    import splunklib.results as sp_results
+    from splunklib.client import AuthenticationError, HTTPError
+except ImportError as imp_err:
+    raise MsticpyImportExtraError(
+        "Cannot use this feature without splunk-sdk installed",
+        title="Error importing splunk-sdk",
+        extra="splunk",
+    ) from imp_err
 
 __version__ = VERSION
-__author__ = "Ian Hellen"
+__author__ = "Ashwin Patil"
 
-# Constants
-# Fields that we know are frequently encoded
-_ENCODED_PARAMS: Dict[str, Set[str]] = {
-    "EXECVE": {"a0", "a1", "a2", "a3", "arch"},
-    "PROCTITLE": {"proctitle"},
-    "USER_CMD": {"cmd"},
-}
+logger = logging.getLogger(__name__)
 
-# USER_START message schema
-_USER_START: Dict[str, Optional[str]] = {
-    "pid": "int",
-    "uid": "int",
-    "auid": "int",
-    "ses": "int",
-    "msg": None,
-    "acct": None,
-    "exe": None,
-    "hostname": None,
-    "addr": None,
-    "terminal": None,
-    "res": None,
-}
 
-# Message types schema
-_FIELD_DEFS: Dict[str, Dict[str, Optional[str]]] = {
-    "SYSCALL": {
-        "success": None,
-        "ppid": "int",
-        "pid": "int",
-        "auid": "int",
-        "uid": "int",
-        "gid": "int",
-        "euid": "int",
-        "egid": "int",
-        "ses": "int",
-        "exe": None,
-        "com": None,
-    },
-    "CWD": {"cwd": None},
-    "PROCTITLE": {"proctitle": None},
-    "LOGIN": {
-        "pid": "int",
-        "uid": "int",
-        "tty": None,
-        "old-ses": "int",
-        "ses": "int",
-        "res": None,
-    },
-    "EXECVE": {"argc": "int", "a0": None, "a1": None, "a2": None},
-    "_USER_START": _USER_START,
-    "USER_END": _USER_START,
-    "CRED_DISP": _USER_START,
-    "USER_ACCT": _USER_START,
-    "CRED_ACQ": _USER_START,
-    "USER_CMD": {
-        "pid": "int",
-        "uid": "int",
-        "auid": "int",
-        "ses": "int",
-        "msg": None,
-        "cmd": None,
-        "terminal": None,
-        "res": None,
-    },
+SPLUNK_CONNECT_ARGS = {
+    "host": "(string) The host name (the default is 'localhost').",
+    "port": "(integer) The port number (the default is 8089).",
+    "http_scheme": "('https' or 'http') The scheme for accessing the service "
+    + "(the default is 'https').",
+    "verify": "(Boolean) Enable (True) or disable (False) SSL verrification for "
+    + "https connections. (optional, the default is True)",
+    "owner": "(string) The owner context of the namespace (optional).",
+    "app": "(string) The app context of the namespace (optional).",
+    "sharing": "('global', 'system', 'app', or 'user') "
+    + "The sharing mode for the namespace (the default is 'user').",
+    "token": "(string) The current session token (optional). Session tokens can be"
+    + " shared across multiple service instances.",
+    "cookie": "(string) A session cookie. When provided, you don’t need to call"
+    + " login(). This parameter is only supported for Splunk 6.2+.",
+    "autologin": "(boolean) When True, automatically tries to log in again if"
+    + " the session terminates.",
+    "username": "(string) The Splunk account username, which is used to "
+    + "authenticate the Splunk instance.",
+    "password": "(string) The password for the Splunk account.",
 }
 
 
 @export
-def unpack_auditd(audit_str: List[Dict[str, str]]) -> Mapping[str, Mapping[str, Any]]:
-    """
-    Unpack an Audit message and returns a dictionary of fields.
-
-    Parameters
-    ----------
-    audit_str : str
-        The auditd raw record
-
-    Returns
-    -------
-    Mapping[str, Any]
-        The extracted message fields and values
-
-    """
-    event_dict: Dict[str, Dict[str, Any]] = {}
-    # The audit_str should be a list of dicts - '{EXECVE : {'p1': 'foo', p2: 'bar'...},
-    #                                      PATH: {'a1': 'xyz',....}}
-
-    for record in audit_str:
-        # process a single message type, splitting into type name
-        # and contents
-        for rec_key, rec_val in record.items():
-            rec_dict: Dict[str, Optional[str]] = {}
-            # Get our field mapping for encoded params for this
-            # mssg_type (rec_key)
-            encoded_fields_map = _ENCODED_PARAMS.get(rec_key, None)
-            for rec_item in rec_val:
-                # for each mssg item, split into k/v pair
-                rec_split = rec_item.split("=", maxsplit=1)
-                if len(rec_split) == 1:
-                    rec_dict[rec_split[0]] = None
-                    continue
-                if (
-                    not encoded_fields_map
-                    or rec_split[1].startswith('"')
-                    or rec_split[0] not in encoded_fields_map
-                ):
-                    field_value = rec_split[1].strip('"')
-                else:
-                    try:
-                        # Try to decode this from hex-string to text
-                        # Mypy thinks codecs.decode returns a str so
-                        # incorrectly issues a type warning - in this case it
-                        # will return a bytes string.
-                        field_value = codecs.decode(  # type: ignore
-                            bytes(rec_split[1], "utf-8"), "hex"
-                        ).decode("utf-8")
-                    except ValueError:
-                        field_value = rec_split[1]
-                        print(rec_val)
-                        print(
-                            "ERR:",
-                            rec_key,
-                            rec_split[0],
-                            rec_split[1],
-                            type(rec_split[1]),
-                        )
-                rec_dict[rec_split[0]] = field_value
-            event_dict[rec_key] = rec_dict
-
-    return event_dict
-
-
-def _extract_event(message_dict: Mapping[str, Any]) -> Tuple[str, Mapping[str, Any]]:
-    """
-    Assemble discrete messages sharing the same message Id into a single event.
-
-    Parameters
-    ----------
-    message_dict : Mapping[str, Any]
-        the input dictionary
-
-    Returns
-    -------
-    Tuple[str, Mapping[str, Any]
-        the assembled message type and contents
-
-    """
-    # Handle process executions specially
-    if "SYSCALL" in message_dict and "EXECVE" in message_dict:
-        proc_create_dict: Dict[str, Any] = {}
-        for mssg_type in ["SYSCALL", "CWD", "EXECVE", "PROCTITLE"]:
-            if mssg_type not in message_dict or mssg_type not in _FIELD_DEFS:
-                continue
-            _extract_mssg_value(mssg_type, message_dict, proc_create_dict)
-
-            if mssg_type == "EXECVE":
-                args = int(proc_create_dict.get("argc", 1))
-                arg_strs = [
-                    proc_create_dict.get(f"a{arg_idx}", "") for arg_idx in range(args)
-                ]
-                proc_create_dict["cmdline"] = " ".join(arg_strs)
-        return "SYSCALL_EXECVE", proc_create_dict
-
-    event_dict: Dict[str, Any] = {}
-    for mssg_type, _ in message_dict.items():
-        if mssg_type in _FIELD_DEFS:
-            _extract_mssg_value(mssg_type, message_dict, event_dict)
-        else:
-            # We don't check for duplicated keys here - if
-            # there are multiple messages with the same key, the
-            # last one will overwrite the previous value
-            event_dict.update(message_dict[mssg_type])
-    return list(message_dict.keys())[0], event_dict
-
-
-def _extract_mssg_value(
-    mssg_type: str,
-    message_dict: Mapping[str, Mapping[str, Any]],
-    event_dict: Dict[str, Any],
-):
-    """
-    Extract field/value from the message dictionary.
-
-    Parameters
-    ----------
-    mssg_type : str
-        The Audit message type
-    message_dict : Mapping[str, str]
-        The input dictionary
-    event_dict : Dict[str, Any]
-        The output dictionary
-
-    """
-    # if the field requires conversion conv will specify the
-    # target type - only int currently
-    for fieldname, conv in _FIELD_DEFS[mssg_type].items():
-        value = message_dict[mssg_type].get(fieldname, None)
-        if not value:
-            return
-        if conv and conv == "int":
-            value = int(value)
-            if value == 4294967295:
-                value = -1
-        if fieldname in event_dict:
-            event_dict[f"{fieldname}_{mssg_type}"] = value
-        else:
-            event_dict[fieldname] = value
+class SplunkDriver(DriverBase):
+    """Driver to connect and query from Splunk."""
 
-
-def _move_cols_to_front(data: pd.DataFrame, column_count: int = 1) -> pd.DataFrame:
-    """
-    Move N columns from end to front of DataFrame.
-
-    Parameters
-    ----------
-    data : pd.DataFrame
-        The input DataFrame
-    column_count : int, optional
-        The number of columns to move (the default is 1)
-
-    Returns
-    -------
-    pd.DataFrame
-        DataFrame with `column_count` columns shifted to front
-
-    """
-    return data[list(data.columns[-column_count:]) + list(data.columns[:-column_count])]
-
-
-@export
-def extract_events_to_df(
-    data: pd.DataFrame,
-    input_column: str = "AuditdMessage",
-    event_type: str = None,
-    verbose: bool = False,
-) -> pd.DataFrame:
-    """
-    Extract auditd raw messages into a dataframe.
-
-    Parameters
-    ----------
-    data : pd.DataFrame
-        The input dataframe with raw auditd data in
-        a single string column
-    input_column : str, optional
-        the input column name (the default is 'AuditdMessage')
-    event_type : str, optional
-        the event type, if None, defaults to all (the default is None)
-    verbose : bool, optional
-        Give feedback on stages of processing (the default is False)
-
-    Returns
-    -------
-    pd.DataFrame
-        The resultant DataFrame
-
-    """
-    if verbose:
-        start_time = datetime.utcnow()
-        print(f"Unpacking auditd messages for {len(data)} events...")
-
-    # If the provided table has auditd messages as a string format and
-    # extract key elements.
-    if isinstance(data[input_column].head(1)[0], str):
-        data["mssg_id"] = data.apply(
-            lambda x: _extract_timestamp(x[input_column]), axis=1
+    _SPLUNK_REQD_ARGS = ["host", "username", "password"]
+    _CONNECT_DEFAULTS: Dict[str, Any] = {"port": 8089}
+    _TIME_FORMAT = '"%Y-%m-%d %H:%M:%S.%6N"'
+
+    def __init__(self, **kwargs):
+        """Instantiate Splunk Driver."""
+        super().__init__(**kwargs)
+        self.service = None
+        self._loaded = True
+        self._connected = False
+        if kwargs.get("debug", False):
+            logger.setLevel(logging.DEBUG)
+
+        self.set_driver_property(
+            DriverProps.PUBLIC_ATTRS,
+            {
+                "client": self.service,
+                "saved_searches": self._saved_searches,
+                "fired_alerts": self._fired_alerts,
+            },
         )
-        data[input_column] = data.apply(
-            lambda x: _parse_audit_message(x[input_column]), axis=1
+        self.set_driver_property(
+            DriverProps.FORMATTERS,
+            {
+                Formatters.DATETIME: self._format_datetime,
+                Formatters.LIST: self._format_list,
+            },
         )
 
-    # Our first pandas expression does most of the work - unpacking the
-    # column contents, then extracting these into a two columns
-    # EventType (the main auditd mssg type) and a dict of k/v values
-    # EventData
-    tmp_df = data.apply(
-        lambda x: _extract_event(unpack_auditd(x[input_column])),
-        axis=1,
-        result_type="expand",
-    ).rename(columns={0: "EventType", 1: "EventData"})
-    # if only one type of event is requested
-    if event_type:
-        tmp_df = tmp_df.loc[tmp_df["EventType"] == event_type]
-        if verbose:
-            print(f"Event subset = {event_type} (events: {len(tmp_df)})")
-
-    if verbose:
-        print("Building output dataframe...")
-
-    # We convert the EventData dict into a series,
-    # then merge with:
-    # First - the intermediate input DF to add back the EventType column
-    # Second - the original input DF to add back metadata columns like Computer
-    # Finally get rid of any empty columns
-    tmp_df = (
-        tmp_df.apply(lambda x: pd.Series(x.EventData), axis=1)
-        .merge(tmp_df[["EventType"]], left_index=True, right_index=True)
-        .merge(
-            data.drop([input_column], axis=1),
-            how="inner",
-            left_index=True,
-            right_index=True,
+    def connect(self, connection_str: Optional[str] = None, **kwargs):
+        """
+        Connect to Splunk via splunk-sdk.
+
+        Parameters
+        ----------
+        connection_str : Optional[str], optional
+            Connection string with Splunk connection parameters
+
+        Other Parameters
+        ----------------
+        kwargs :
+            Connection parameters can be supplied as keyword parameters.
+
+        Notes
+        -----
+        Default configuration is read from the DataProviders/Splunk
+        section of msticpyconfig.yaml, if available.
+
+        """
+        cs_dict = self._get_connect_args(connection_str, **kwargs)
+
+        arg_dict = {
+            key: val for key, val in cs_dict.items() if key in SPLUNK_CONNECT_ARGS
+        }
+        try:
+            self.service = sp_client.connect(**arg_dict)
+        except AuthenticationError as err:
+            raise MsticpyConnectionError(
+                f"Authentication error connecting to Splunk: {err}",
+                title="Splunk connection",
+                help_uri="https://msticpy.readthedocs.io/en/latest/DataProviders.html",
+            ) from err
+        except HTTPError as err:
+            raise MsticpyConnectionError(
+                f"Communication error connecting to Splunk: {err}",
+                title="Splunk connection",
+                help_uri="https://msticpy.readthedocs.io/en/latest/DataProviders.html",
+            ) from err
+        except Exception as err:
+            raise MsticpyConnectionError(
+                f"Error connecting to Splunk: {err}",
+                title="Splunk connection",
+                help_uri="https://msticpy.readthedocs.io/en/latest/DataProviders.html",
+            ) from err
+        self._connected = True
+        print("connected")
+
+    def _get_connect_args(
+        self, connection_str: Optional[str], **kwargs
+    ) -> Dict[str, Any]:
+        """Check and consolidate connection parameters."""
+        cs_dict: Dict[str, Any] = self._CONNECT_DEFAULTS
+        # Fetch any config settings
+        cs_dict.update(self._get_config_settings("Splunk"))
+        # If a connection string - parse this and add to config
+        if connection_str:
+            cs_items = connection_str.split(";")
+            cs_dict.update(
+                {
+                    cs_item.split("=")[0].strip(): cs_item.split("=")[1]
+                    for cs_item in cs_items
+                }
+            )
+        elif kwargs:
+            # if connection args supplied as kwargs
+            cs_dict.update(kwargs)
+            check_kwargs(cs_dict, list(SPLUNK_CONNECT_ARGS.keys()))
+
+        cs_dict["port"] = int(cs_dict["port"])
+        verify_opt = cs_dict.get("verify")
+        if isinstance(verify_opt, str):
+            cs_dict["verify"] = "true" in verify_opt.casefold()
+        elif isinstance(verify_opt, bool):
+            cs_dict["verify"] = verify_opt
+
+        missing_args = set(self._SPLUNK_REQD_ARGS) - cs_dict.keys()
+        if missing_args:
+            raise MsticpyUserConfigError(
+                "One or more connection parameters missing for Splunk connector",
+                ", ".join(missing_args),
+                f"Required parameters are {', '.join(self._SPLUNK_REQD_ARGS)}",
+                "All parameters:",
+                *[f"{arg}: {desc}" for arg, desc in SPLUNK_CONNECT_ARGS.items()],
+                title="no Splunk connection parameters",
+            )
+        return cs_dict
+
+    def query(
+        self, query: str, query_source: Optional[QuerySource] = None, **kwargs
+    ) -> Union[pd.DataFrame, Any]:
+        """
+        Execute splunk query and retrieve results via OneShot or async search mode.
+
+        Parameters
+        ----------
+        query : str
+            Splunk query to execute via OneShot or async search mode
+        query_source : QuerySource
+            The query definition object
+
+        Other Parameters
+        ----------------
+        count : int, optional
+            Passed to Splunk job that indicates the maximum number
+            of entities to return. A value of 0 indicates no maximum,
+            by default, 0
+        oneshot : bool, optional
+            Set to True for oneshot (blocking) mode, by default False
+        page_size = int, optional
+            Pass to Splunk results reader in terms of fetch speed,
+            which sets of result amount will be got at a time,
+            by default, 100
+        timeout : int, optional
+            Amount of time to wait for results, by default 60
+
+        Returns
+        -------
+        Union[pd.DataFrame, Any]
+            Query results in a dataframe.
+            or query response if an error.
+
+        """
+        del query_source
+        if not self._connected:
+            raise self._create_not_connected_err("Splunk")
+
+        # default to unlimited query unless count is specified
+        count = kwargs.pop("count", 0)
+
+        # Get sets of N results at a time, N=100 by default
+        page_size = kwargs.pop("page_size", 100)
+
+        # Normal (non-blocking) searches or oneshot (blocking) searches.
+        # Defaults to Normal(non-blocking)
+
+        # Oneshot is a blocking search that is scheduled to run immediately.
+        # Instead of returning a search job, this mode returns the results
+        # of the search once completed.
+        # Because this is a blocking search, the results are not available
+        # until the search has finished.
+        # https://dev.splunk.com/enterprise/docs/python/
+        # sdk-python/howtousesplunkpython/howtorunsearchespython
+        is_oneshot = kwargs.get("oneshot", False)
+
+        if is_oneshot is True:
+            kwargs["output_mode"] = "json"
+            query_results = self.service.jobs.oneshot(query, count=count, **kwargs)
+
+            reader = sp_results.JSONResultsReader(  # pylint: disable=no-member
+                query_results
+            )  # due to DeprecationWarning of normal ResultsReader
+            resp_rows = [row for row in reader if isinstance(row, dict)]
+        else:
+            # Set mode and initialize async job
+            kwargs_normalsearch = {"exec_mode": "normal"}
+            query_job = self.service.jobs.create(
+                query, count=count, **kwargs_normalsearch
+            )
+            resp_rows, reader = self._exec_async_search(query_job, page_size, **kwargs)
+
+        if len(resp_rows) == 0 or not resp_rows:
+            print("Warning - query did not return any results.")
+            return [row for row in reader if isinstance(row, sp_results.Message)]
+        return pd.DataFrame(resp_rows)
+
+    def query_with_results(self, query: str, **kwargs) -> Tuple[pd.DataFrame, Any]:
+        """
+        Execute query string and return DataFrame of results.
+
+        Parameters
+        ----------
+        query : str
+            Query to execute against splunk instance.
+
+        Returns
+        -------
+        Union[pd.DataFrame,Any]
+            A DataFrame (if successful) or
+            the underlying provider result if an error occurs.
+
+        """
+        raise NotImplementedError(f"Not supported for {self.__class__.__name__}")
+
+    @property
+    def service_queries(self) -> Tuple[Dict[str, str], str]:
+        """
+        Return dynamic queries available on connection to service.
+
+        Returns
+        -------
+        Tuple[Dict[str, str], str]
+            Dictionary of query_name, query_text.
+            Name of container to add queries to.
+
+        """
+        if not self.connected:
+            raise self._create_not_connected_err("Splunk")
+        if hasattr(self.service, "saved_searches") and self.service.saved_searches:
+            queries = {
+                search.name.strip().replace(" ", "_"): f"search {search['search']}"
+                for search in self.service.saved_searches
+            }
+            return queries, "SavedSearches"
+        return {}, "SavedSearches"
+
+    @property
+    def driver_queries(self) -> Iterable[Dict[str, Any]]:
+        """
+        Return dynamic queries available on connection to service.
+
+        Returns
+        -------
+        Iterable[Dict[str, Any]]
+            List of queries with properties: "name", "query", "container"
+            and (optionally) "description"
+
+        Raises
+        ------
+        MsticpyNotConnectedError
+            If called before driver is connected.
+
+        """
+        if not self.connected:
+            raise self._create_not_connected_err("Splunk")
+        if hasattr(self.service, "saved_searches") and self.service.saved_searches:
+            return [
+                {
+                    "name": search.name.strip().replace(" ", "_"),
+                    "query": f"search {search['search']}",
+                    "query_paths": "SavedSearches",
+                    "description": "",
+                }
+                for search in self.service.saved_searches
+            ]
+        return []
+
+    def _exec_async_search(self, query_job, page_size, timeout=60):
+        """Execute an async search and return results."""
+        # Initiate progress bar and start while loop, waiting for async query to complete
+        progress_bar = tqdm(total=100, desc="Waiting Splunk job to complete")
+        prev_progress = 0
+        offset = 0  # Start at result 0
+        start_time = datetime.now()
+        end_time = start_time + timedelta(seconds=timeout)
+        while True:
+            while not query_job.is_ready():
+                sleep(1)
+            if self._retrieve_job_status(query_job, progress_bar, prev_progress):
+                break
+            if datetime.now() > end_time:
+                raise MsticpyDataQueryError(
+                    "Timeout waiting for Splunk query to complete",
+                    f"Job completion reported {query_job['doneProgress']}",
+                    title="Splunk query timeout",
+                )
+            sleep(1)
+        # Update progress bar indicating job completion
+        progress_bar.update(100)
+        progress_bar.close()
+        sleep(2)
+
+        logger.info("Implicit parameter dump - 'page_size': %d", page_size)
+        return self._retrieve_results(query_job, offset, page_size)
+
+    @staticmethod
+    def _retrieve_job_status(query_job, progress_bar, prev_progress):
+        """Poll the status of a job and update the progress bar."""
+        stats = {
+            "is_done": query_job["isDone"],
+            "done_progress": float(query_job["doneProgress"]) * 100,
+            "scan_count": int(query_job["scanCount"]),
+            "event_count": int(query_job["eventCount"]),
+            "result_count": int(query_job["resultCount"]),
+        }
+        status = (
+            "\r%(done_progress)03.1f%%   %(scan_count)d scanned   "
+            "%(event_count)d matched   %(result_count)d results"
+        ) % stats
+        if prev_progress == 0:
+            progress = stats["done_progress"]
+        else:
+            progress = stats["done_progress"] - prev_progress
+        prev_progress = stats["done_progress"]
+        progress_bar.update(progress)
+
+        if stats["is_done"] == "1":
+            logger.info(status)
+            logger.info("Splunk job completed.")
+            return True
+        return False
+
+    @staticmethod
+    def _retrieve_results(query_job, offset, page_size):
+        """Retrieve the results of a job, decode and return them."""
+        # Retrieving all the results by paginate
+        result_count = int(
+            query_job["resultCount"]
+        )  # Number of results this job returned
+
+        resp_rows = []
+        progress_bar_paginate = tqdm(
+            total=result_count, desc="Waiting Splunk result to retrieve"
         )
-        .dropna(axis=1, how="all")
-    )
-
-    if verbose:
-        print("Fixing timestamps...")
-
-    # extract real timestamp from mssg_id
-    tmp_df["TimeStamp"] = tmp_df.apply(
-        lambda x: datetime.utcfromtimestamp(float(x["mssg_id"].split(":")[0])), axis=1
-    )
-    if "TimeGenerated" in tmp_df:
-        tmp_df = tmp_df.drop(["TimeGenerated"], axis=1)
-    tmp_df = tmp_df.rename(columns={"TimeStamp": "TimeGenerated"}).pipe(
-        _move_cols_to_front, column_count=5
-    )
-    if verbose:
-        print(f"Complete. {len(tmp_df)} output rows", end=" ")
-        delta = datetime.utcnow() - start_time
-        print(f"time: {delta.seconds + delta.microseconds/1_000_000} sec")
-
-    return tmp_df
-
-
-@export
-def get_event_subset(data: pd.DataFrame, event_type: str) -> pd.DataFrame:
-    """
-    Return a subset of the events matching type event_type.
-
-    Parameters
-    ----------
-    data : pd.DataFrame
-        The input data
-    event_type : str
-        The event type to select
-
-    Returns
-    -------
-    pd.DataFrame
-        The subset of the data where
-        data['EventType'] == event_type
-
-    """
-    return (
-        data[data["EventType"] == event_type].dropna(axis=1, how="all").infer_objects()
-    )
-
-
-@export
-def read_from_file(
-    filepath: str, event_type: str = None, verbose: bool = False, dummy_sep: str = "\t"
-) -> pd.DataFrame:
-    r"""
-    Extract Audit events from a log file.
-
-    Parameters
-    ----------
-    filepath : str
-        path to the input file
-    event_type : str, optional
-        The type of event to extract if only a subset required.
-        (the default is None, which processes all types)
-    verbose : bool, optional
-        If true more progress messages are output
-        (the default is False)
-    dummy_sep : str, optional
-        Separator to use for reading the 'csv' file
-        (default is tab - '\t')
-
-    Returns
-    -------
-    pd.DataFrame
-        The output DataFrame
-
-    Notes
-    -----
-    The dummy_sep parameter should be a character that does not
-    occur in an input line. This function uses pandas read_csv
-    to read the audit lines into a single column. Using a separator
-    that does appear in the input (e.g. space or comma) will cause
-    data to be parsed into multiple columns and anything after the
-    first separator in a line will be lost.
-
-    """
-    # read in the file using pd.read_csv()
-    df_raw: pd.DataFrame = pd.read_csv(
-        filepath, sep=dummy_sep, names=["raw_data"], skip_blank_lines=True
-    )
-
-    # extract message ID into separate column
-    df_raw["mssg_id"] = df_raw.apply(
-        lambda x: _extract_timestamp(x["raw_data"]), axis=1
-    )
-    # pylint: disable=unsupported-assignment-operation, no-member
-    # Pack message type and content into a dictionary:
-    # {'mssg_type: ['item1=x, item2=y....]}
-    df_raw["AuditdMessage"] = df_raw.apply(
-        lambda x: _parse_audit_message(x["raw_data"]), axis=1
-    )
-
-    # Group the data by message id string and concatenate the message content
-    # dictionaries in a list.
-    df_grouped_cols = (
-        df_raw.groupby(["mssg_id"]).agg({"AuditdMessage": list}).reset_index()
-    )
-    # pylint: enable=unsupported-assignment-operation, no-member
-
-    # pass this DataFrame to the event extractor.
-    return extract_events_to_df(
-        data=df_grouped_cols,
-        input_column="AuditdMessage",
-        event_type=event_type,
-        verbose=verbose,
-    )
-
-
-def _parse_audit_message(audit_str: str) -> Dict[str, List[str]]:
-    """
-    Parse an auditd message string into Dict format required by unpack_auditd.
-
-    Parameters
-    ----------
-    audit_str : str
-        The Audit message
-
-    Returns
-    -------
-    Dict[str, str]
-        The extracted message values
-
-    """
-    audit_message = audit_str.rstrip().split(": ")
-    audit_headers = audit_message[0]
-    audit_hdr_match = re.match(r"type=([^\s]+)", audit_headers)
-    if audit_hdr_match:
-        return {audit_hdr_match.group(1): audit_message[1].split(" ")}
-    return {}  # type ignore
-
-
-def _extract_timestamp(audit_str: str) -> str:
-    """
-    Parse an auditd message string and extract the message time.
-
-    Parameters
-    ----------
-    audit_str : str
-        The Audit message
-
-    Returns
-    -------
-    str
-        The extracted message time string
-
-    """
-    audit_message = audit_str.rstrip().split(": ")
-    audit_headers = audit_message[0]
-    audit_hdr_match = re.match(r".*msg=audit\(([^\)]+)\)", audit_headers)
-    if audit_hdr_match:
-        return audit_hdr_match.group(1).split(":")[0]
-    return ""
-
-
-# pylint: disable=too-many-branches
-@export
-def generate_process_tree(  # noqa: MC0001
-    audit_data: pd.DataFrame, branch_depth: int = 4, processes: pd.DataFrame = None
-) -> pd.DataFrame:
-    """
-    Generate process tree data from auditd logs.
-
-    Parameters
-    ----------
-    audit_data : pd.DataFrame
-        The Audit data containing process creation events
-    branch_depth: int, optional
-        The maximum depth of parent or child processes to extract from the data
-        (The default is 4)
-    processes: pd.DataFrame, optional
-        Dataframe of processes to generate tree for
-
-    Returns
-    -------
-    pd.DataFrame
-        The formatted process tree data
-
-    """
-    # Superceded by process_tree_utils module
-    del branch_depth, processes
-    return build_process_tree(audit_data)
+        while offset < result_count:
+            kwargs_paginate = {
+                "count": page_size,
+                "offset": offset,
+                "output_mode": "json",
+            }
+            # Get the search results and display them
+            search_results = query_job.results(**kwargs_paginate)
+            # due to DeprecationWarning of normal ResultsReader
+            reader = sp_results.JSONResultsReader(  # pylint: disable=no-member
+                search_results
+            )
+            resp_rows.extend([row for row in reader if isinstance(row, dict)])
+            progress_bar_paginate.update(page_size)
+            offset += page_size
+        # Update progress bar indicating fetch results
+        progress_bar_paginate.update(result_count)
+        progress_bar_paginate.close()
+        logger.info("Retrieved %d results.", len(resp_rows))
+        return resp_rows, reader
+
+    @property
+    def _saved_searches(self) -> Union[pd.DataFrame, Any]:
+        """
+        Return list of saved searches in dataframe.
+
+        Returns
+        -------
+        pd.DataFrame
+            Dataframe with list of saved searches with name and query columns.
+
+        """
+        return self._get_saved_searches() if self.connected else None
+
+    def _get_saved_searches(self) -> Union[pd.DataFrame, Any]:
+        # sourcery skip: class-extract-method
+        """
+        Return list of saved searches in dataframe.
+
+        Returns
+        -------
+        pd.DataFrame
+            Dataframe with list of saved searches with name and query columns.
+
+        """
+        if not self.connected:
+            raise self._create_not_connected_err("Splunk")
+        savedsearches = self.service.saved_searches
+
+        out_df = pd.DataFrame(columns=["name", "query"])
+
+        namelist = []
+        querylist = []
+        for savedsearch in savedsearches:
+            namelist.append(savedsearch.name.replace(" ", "_"))
+            querylist.append(savedsearch["search"])
+        out_df["name"] = namelist
+        out_df["query"] = querylist
+
+        return out_df
+
+    @property
+    def _fired_alerts(self) -> Union[pd.DataFrame, Any]:
+        """
+        Return list of fired alerts in dataframe.
+
+        Returns
+        -------
+        pd.DataFrame
+            Dataframe with list of fired alerts with alert name and count columns.
+
+        """
+        return self._get_fired_alerts() if self.connected else None
+
+    def _get_fired_alerts(self) -> Union[pd.DataFrame, Any]:
+        """
+        Return list of fired alerts in dataframe.
+
+        Returns
+        -------
+        pd.DataFrame
+            Dataframe with list of fired alerts with alert name and count columns.
+
+        """
+        if not self.connected:
+            raise self._create_not_connected_err("Splunk")
+        firedalerts = self.service.fired_alerts
+
+        out_df = pd.DataFrame(columns=["name", "count"])
+
+        alert_names = []
+        alert_counts = []
+        for alert in firedalerts:
+            alert_names.append(alert.name)
+            alert_counts.append(alert.count)
+        out_df["name"] = alert_names
+        out_df["count"] = alert_counts
+
+        return out_df
+
+    # Parameter Formatting methods
+    @staticmethod
+    def _format_datetime(date_time: datetime) -> str:
+        """Return datetime-formatted string."""
+        return f'"{date_time.isoformat(sep=" ")}"'
+
+    @staticmethod
+    def _format_list(param_list: Iterable[Any]) -> str:
+        """Return formatted list parameter."""
+        fmt_list = [f'"{item}"' for item in param_list]
+        return ",".join(fmt_list)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `msticpy-2.4.0/msticpy/transform/base64unpack.py` & `msticpy-2.5.0/msticpy/transform/base64unpack.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/transform/cmd_line.py` & `msticpy-2.5.0/msticpy/transform/cmd_line.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/transform/iocextract.py` & `msticpy-2.5.0/msticpy/transform/iocextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/transform/network.py` & `msticpy-2.5.0/msticpy/transform/network.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/transform/proc_tree_build_mde.py` & `msticpy-2.5.0/msticpy/transform/proc_tree_build_mde.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/transform/proc_tree_build_winlx.py` & `msticpy-2.5.0/msticpy/transform/proc_tree_build_winlx.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/transform/proc_tree_builder.py` & `msticpy-2.5.0/msticpy/transform/proc_tree_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # pylint: disable=unused-import
 from .proc_tree_schema import ProcSchema  # noqa: F401
 from .proc_tree_schema import (  # noqa: F401
     HX_PROCESSEVENT_SCH,
     LX_EVENT_SCH,
     MDE_EVENT_SCH,
     MDE_INT_EVENT_SCH,
+    OSQUERY_EVENT_SCH,
     SUPPORTED_SCHEMAS,
     SYSMON_PROCESS_CREATE_EVENT_SCH,
     WIN_EVENT_SCH,
 )
 from .proc_tree_schema import ColNames as Col
 from .process_tree_utils import get_summary_info
```

### Comparing `msticpy-2.4.0/msticpy/transform/proc_tree_schema.py` & `msticpy-2.5.0/msticpy/transform/proc_tree_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -238,14 +238,30 @@
     user_name="User",
     path_separator="\\",
     event_id_column="EventID",
     event_id_identifier=1,
     host_name_column="Computer",
 )
 
+# Osquery process (may vary depending on exact query)
+OSQUERY_EVENT_SCH = ProcSchema(
+    time_stamp="calendarTime",
+    # host_name_column = "hostIdentifier",
+    process_name="name",
+    process_id="pid",
+    parent_name="pcmdline",
+    parent_id="parent",
+    logon_id=None,
+    target_logon_id=None,
+    cmd_line="cmdline",
+    user_name="username",
+    path_separator="/",
+    user_id="uid",
+)
+
 # FireEye HX processEvent from 'stateagentinspector' or 'eventbuffer' audits
 HX_PROCESSEVENT_SCH = ProcSchema(
     time_stamp="starttime",
     process_name="process",
     process_id="pid",
     parent_name="parentprocess",
     parent_id="parentpid",
@@ -259,14 +275,15 @@
 
 SUPPORTED_SCHEMAS = (
     WIN_EVENT_SCH,
     LX_EVENT_SCH,
     MDE_INT_EVENT_SCH,
     MDE_EVENT_SCH,
     SYSMON_PROCESS_CREATE_EVENT_SCH,
+    OSQUERY_EVENT_SCH,
     HX_PROCESSEVENT_SCH,
 )
 
 
 # pylint: disable=too-few-public-methods
 class ColNames:
     """Class to hold constant column names."""
```

### Comparing `msticpy-2.4.0/msticpy/transform/process_tree_utils.py` & `msticpy-2.5.0/msticpy/transform/process_tree_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/__init__.py` & `msticpy-2.5.0/msticpy/vis/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 Visualization sub-package.
 
 This contains the following functionality:
 
 - entity_graph_tools - graphing and timeline support for entity visualization
 - data_viewer - Bokeh-based data browser
+- data_viewer_pane - PyVis Panel-based data browser
 - foliummap - mapping using the folium package
 - matrix_plot - matrix/interaction plots
 - morph_charts - experimental morph charts support
 - mp_pandas_plot - pandas `mp_plot` accessor for plotting functions
 - process_tree - process tree visualization
 - timeline - event timeline and timeline_values visualizations
 - timeline_duration - timeline durations
```

### Comparing `msticpy-2.4.0/msticpy/vis/code_view.py` & `msticpy-2.5.0/msticpy/vis/code_view.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/data_viewer.py` & `msticpy-2.5.0/msticpy/vis/data_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,32 @@
     TableColumn,
 )
 from IPython.display import display
 
 from .. import nbwidgets
 from .._version import VERSION
 
+# pylint: disable=unused-import
+try:
+    import panel as pn  # noqa: F401
+
+    _PANEL_AVAILABLE = True
+    from .data_viewer_panel import DataViewer as DataViewerPanel
+except ImportError:
+    _PANEL_AVAILABLE = False
+
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 
 FilterExpr = namedtuple("FilterExpr", "column, inv, operator, expr")
 
 
 # pylint: disable=too-many-instance-attributes
-class DataViewer:
+class DataViewerBokeh:
     """Data viewer class."""
 
     _DEF_HEIGHT = 550
 
     def __init__(
         self, data: pd.DataFrame, selected_cols: List[str] = None, debug=False
     ):
@@ -530,7 +539,12 @@
             formatter=DateFormatter(format=date_fmt),
             width=_get_col_width(data, col),
         )
         for col in dt_cols
     }
     columns.update(dt_columns)
     return {col: columns[col] for col in col_order}
+
+
+# If panel is imported we want to use that version
+# else use the existing Bokeh implementation
+DataViewer = DataViewerPanel if _PANEL_AVAILABLE else DataViewerBokeh
```

### Comparing `msticpy-2.4.0/msticpy/vis/entity_graph_tools.py` & `msticpy-2.5.0/msticpy/vis/entity_graph_tools.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/figure_dimension.py` & `msticpy-2.5.0/msticpy/vis/figure_dimension.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/matrix_plot.py` & `msticpy-2.5.0/msticpy/vis/matrix_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/mordor_browser.py` & `msticpy-2.5.0/msticpy/vis/mordor_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/morph_charts.py` & `msticpy-2.5.0/msticpy/vis/morph_charts.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/mp_pandas_plot.py` & `msticpy-2.5.0/msticpy/vis/mp_pandas_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/nbdisplay.py` & `msticpy-2.5.0/msticpy/vis/nbdisplay.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/network_plot.py` & `msticpy-2.5.0/msticpy/vis/network_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/process_tree.py` & `msticpy-2.5.0/msticpy/vis/process_tree.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/query_browser.py` & `msticpy-2.5.0/msticpy/vis/query_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/ti_browser.py` & `msticpy-2.5.0/msticpy/vis/ti_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/timeline.py` & `msticpy-2.5.0/msticpy/vis/timeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/timeline_common.py` & `msticpy-2.5.0/msticpy/vis/timeline_common.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/timeline_duration.py` & `msticpy-2.5.0/msticpy/vis/timeline_duration.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/timeline_pd_accessor.py` & `msticpy-2.5.0/msticpy/vis/timeline_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/timeline_values.py` & `msticpy-2.5.0/msticpy/vis/timeline_values.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/timeseries.py` & `msticpy-2.5.0/msticpy/vis/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy/vis/vtobject_browser.py` & `msticpy-2.5.0/msticpy/vis/vtobject_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/msticpy.egg-info/PKG-INFO` & `msticpy-2.5.0/msticpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msticpy
-Version: 2.4.0
+Version: 2.5.0
 Summary: MSTIC Security Tools
 Home-page: https://github.com/microsoft/msticpy
 Author: Ian Hellen
 Author-email: ianhelle@microsoft.com
 Maintainer: Pete Bryan
 Maintainer-email: peter.bryan@microsoft.com
 License: MIT License
@@ -32,18 +32,20 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: vt3
 Provides-Extra: splunk
 Provides-Extra: sumologic
 Provides-Extra: kql
 Provides-Extra: _azure_core
+Provides-Extra: azure_query
 Provides-Extra: keyvault
 Provides-Extra: ml
 Provides-Extra: sql2kql
 Provides-Extra: riskiq
+Provides-Extra: panel
 Provides-Extra: all
 Provides-Extra: azure
 Provides-Extra: test
 Provides-Extra: azsentinel
 Provides-Extra: azuresentinel
 Provides-Extra: sentinel
 License-File: LICENSE
```

### Comparing `msticpy-2.4.0/msticpy.egg-info/SOURCES.txt` & `msticpy-2.5.0/msticpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 msticpy.egg-info/top_level.txt
 msticpy/analysis/__init__.py
 msticpy/analysis/cluster_auditd.py
 msticpy/analysis/code_cleanup.py
 msticpy/analysis/eventcluster.py
 msticpy/analysis/observationlist.py
 msticpy/analysis/outliers.py
+msticpy/analysis/polling_detection.py
 msticpy/analysis/syslog_utils.py
 msticpy/analysis/timeseries.py
 msticpy/analysis/anomalous_sequence/__init__.py
 msticpy/analysis/anomalous_sequence/anomalous.py
 msticpy/analysis/anomalous_sequence/model.py
 msticpy/analysis/anomalous_sequence/sessionize.py
 msticpy/analysis/anomalous_sequence/utils/__init__.py
@@ -50,27 +51,30 @@
 msticpy/common/azure_auth.py
 msticpy/common/check_version.py
 msticpy/common/data_types.py
 msticpy/common/data_utils.py
 msticpy/common/exceptions.py
 msticpy/common/pkg_config.py
 msticpy/common/provider_settings.py
+msticpy/common/proxy_settings.py
+msticpy/common/settings.py
 msticpy/common/timespan.py
 msticpy/common/wsconfig.py
 msticpy/common/utility/__init__.py
 msticpy/common/utility/format.py
 msticpy/common/utility/ipython.py
 msticpy/common/utility/package.py
 msticpy/common/utility/types.py
 msticpy/config/__init__.py
 msticpy/config/ce_azure.py
 msticpy/config/ce_azure_sentinel.py
 msticpy/config/ce_common.py
 msticpy/config/ce_data_providers.py
 msticpy/config/ce_keyvault.py
+msticpy/config/ce_msticpy.py
 msticpy/config/ce_other_providers.py
 msticpy/config/ce_provider_base.py
 msticpy/config/ce_simple_settings.py
 msticpy/config/ce_ti_providers.py
 msticpy/config/ce_user_defaults.py
 msticpy/config/comp_edit.py
 msticpy/config/compound_ctrls.py
@@ -140,28 +144,35 @@
 msticpy/data/azure/azure_data.py
 msticpy/data/core/__init__.py
 msticpy/data/core/data_providers.py
 msticpy/data/core/data_query_reader.py
 msticpy/data/core/param_extractor.py
 msticpy/data/core/query_container.py
 msticpy/data/core/query_defns.py
+msticpy/data/core/query_provider_connections_mixin.py
+msticpy/data/core/query_provider_utils_mixin.py
 msticpy/data/core/query_source.py
 msticpy/data/core/query_store.py
+msticpy/data/core/query_template.py
 msticpy/data/drivers/__init__.py
+msticpy/data/drivers/azure_kusto_driver.py
+msticpy/data/drivers/azure_monitor_driver.py
 msticpy/data/drivers/cybereason_driver.py
 msticpy/data/drivers/driver_base.py
 msticpy/data/drivers/elastic_driver.py
 msticpy/data/drivers/kql_driver.py
 msticpy/data/drivers/kusto_driver.py
 msticpy/data/drivers/local_data_driver.py
+msticpy/data/drivers/local_osquery_driver.py
 msticpy/data/drivers/mdatp_driver.py
 msticpy/data/drivers/mordor_driver.py
 msticpy/data/drivers/odata_driver.py
 msticpy/data/drivers/resource_graph_driver.py
 msticpy/data/drivers/security_graph_driver.py
+msticpy/data/drivers/sentinel_query_reader.py
 msticpy/data/drivers/splunk_driver.py
 msticpy/data/drivers/sumologic_driver.py
 msticpy/data/queries/cybereason/cybereason_connections.yaml
 msticpy/data/queries/cybereason/cybereason_hosts.yaml
 msticpy/data/queries/cybereason/cybereason_processes.yaml
 msticpy/data/queries/localdata/local_data.yaml
 msticpy/data/queries/m365d/kql_mdatp_alerts.yaml
@@ -244,14 +255,15 @@
 msticpy/datamodel/soc/incident.py
 msticpy/datamodel/soc/sentinel_alert.py
 msticpy/init/__init__.py
 msticpy/init/azure_ml_tools.py
 msticpy/init/azure_synapse_tools.py
 msticpy/init/logging.py
 msticpy/init/mp_pandas_accessors.py
+msticpy/init/mp_plugins.py
 msticpy/init/nbinit.py
 msticpy/init/nbmagics.py
 msticpy/init/pivot.py
 msticpy/init/user_config.py
 msticpy/init/pivot_core/__init__.py
 msticpy/init/pivot_core/pivot_browser.py
 msticpy/init/pivot_core/pivot_container.py
@@ -334,14 +346,15 @@
 msticpy/transform/proc_tree_build_winlx.py
 msticpy/transform/proc_tree_builder.py
 msticpy/transform/proc_tree_schema.py
 msticpy/transform/process_tree_utils.py
 msticpy/vis/__init__.py
 msticpy/vis/code_view.py
 msticpy/vis/data_viewer.py
+msticpy/vis/data_viewer_panel.py
 msticpy/vis/entity_graph_tools.py
 msticpy/vis/figure_dimension.py
 msticpy/vis/foliummap.py
 msticpy/vis/matrix_plot.py
 msticpy/vis/mordor_browser.py
 msticpy/vis/morph_charts.py
 msticpy/vis/mp_pandas_plot.py
```

### Comparing `msticpy-2.4.0/msticpy.egg-info/requires.txt` & `msticpy-2.5.0/msticpy.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 beautifulsoup4>=4.0.0
 bokeh<=2.4.3,>=1.4.0
 cryptography>=3.1
 deprecated>=1.2.4
 dnspython<3.0.0,>=2.0.0
 folium>=0.9.0
 geoip2>=2.9.0
-httpx==0.23.3
+httpx==0.24.0
 html5lib
 ipywidgets<8.0.0,>=7.4.2
 KqlmagicCustom[auth_code_clipboard,jupyter-basic]>=0.1.114.post22
 lxml>=4.6.5
-matplotlib>=3.0.0
 msal>=1.12.0
 msal_extensions>=0.3.0
 msrest>=0.6.0
 msrestazure>=0.6.0
 nest_asyncio>=1.4.0
 networkx>=2.2
 numpy>=1.15.4
@@ -49,70 +48,84 @@
 azure-mgmt-resource>=16.1.0
 azure-storage-blob>=12.5.0
 azure-mgmt-resourcegraph>=8.0.0
 
 [all]
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
 azure-keyvault-secrets>=4.0.0
+azure-kusto-data>=4.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
 azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
+azure-monitor-query>=1.0.0
 azure-storage-blob>=12.5.0
 keyring>=13.2.1
+matplotlib>=3.0.0
 mo-sql-parsing<9.0.0,>=8
 nest_asyncio>=1.4.0
 openpyxl>=3.0
+panel>=0.14.4
 passivetotal>=2.5.3
 scikit-learn>=1.0.0
 scipy>=1.1.0
 splunk-sdk>=1.6.0
 statsmodels>=0.11.1
 sumologic-sdk>=0.1.11
 vt-graph-api>=2.0
 vt-py>=0.6.1
 
 [azsentinel]
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
 azure-keyvault-secrets>=4.0.0
+azure-kusto-data>=4.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
 azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
+azure-monitor-query>=1.0.0
 azure-storage-blob>=12.5.0
 keyring>=13.2.1
 
 [azure]
 azure-keyvault-secrets>=4.0.0
+azure-kusto-data>=4.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
 azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
+azure-monitor-query>=1.0.0
 azure-storage-blob>=12.5.0
 keyring>=13.2.1
 
+[azure_query]
+azure-kusto-data>=4.0.0
+azure-monitor-query>=1.0.0
+
 [azuresentinel]
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
 azure-keyvault-secrets>=4.0.0
+azure-kusto-data>=4.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
 azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
+azure-monitor-query>=1.0.0
 azure-storage-blob>=12.5.0
 keyring>=13.2.1
 
 [dev]
 aiohttp>=3.7.4
 async-cache>=1.1.1
 bandit>=1.7.0
@@ -158,28 +171,34 @@
 [kql]
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
 
 [ml]
 scikit-learn>=1.0.0
 scipy>=1.1.0
 statsmodels>=0.11.1
+matplotlib>=3.0.0
+
+[panel]
+panel>=0.14.4
 
 [riskiq]
 passivetotal>=2.5.3
 
 [sentinel]
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
 azure-keyvault-secrets>=4.0.0
+azure-kusto-data>=4.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
 azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
+azure-monitor-query>=1.0.0
 azure-storage-blob>=12.5.0
 keyring>=13.2.1
 
 [splunk]
 splunk-sdk>=1.6.0
 
 [sql2kql]
@@ -190,40 +209,44 @@
 openpyxl>=3.0
 
 [test]
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
 aiohttp>=3.7.4
 async-cache>=1.1.1
 azure-keyvault-secrets>=4.0.0
+azure-kusto-data>=4.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
 azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
+azure-monitor-query>=1.0.0
 azure-storage-blob>=12.5.0
 bandit>=1.7.0
 beautifulsoup4>=4.0.0
 black>=20.8b1
 coverage>=5.5
 docutils<0.20.0
 filelock>=3.0.0
 flake8>=3.8.4
 isort>=5.10.1
 keyring>=13.2.1
 markdown>=3.3.4
+matplotlib>=3.0.0
 mccabe>=0.6.1
 mo-sql-parsing<9.0.0,>=8
 mypy>=0.812
 nbconvert>=6.1.0
 nbdime>=2.1.0
 nest_asyncio>=1.4.0
 openpyxl>=3.0
 pandas<2.0.0,>=1.4.0
+panel>=0.14.4
 passivetotal>=2.5.3
 pep8-naming>=0.10.0
 pep8>=1.7.1
 pipreqs>=0.4.9
 pre-commit>=2.7.1
 pycodestyle>=2.6.0
 pydocstyle>=6.0.0
```

### Comparing `msticpy-2.4.0/requirements-all.txt` & `msticpy-2.5.0/requirements-all.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 attrs>=18.2.0
 azure-common>=1.1.18
 azure-core>=1.24.0
 azure-identity>=1.10.0
 azure-keyvault-secrets>=4.0.0
+azure-kusto-data>=4.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
 azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
 azure-mgmt-subscription>=3.0.0
+azure-monitor-query>=1.0.0
 azure-storage-blob>=12.5.0
 beautifulsoup4>=4.0.0
 bokeh>=1.4.0, <=2.4.3
 cryptography>=3.1
 deprecated>=1.2.4
 dnspython>=2.0.0, <3.0.0
 folium>=0.9.0
 geoip2>=2.9.0
-httpx==0.23.3
+httpx==0.24.0
 html5lib
 ipython >= 7.1.1; python_version < "3.8"
 ipython >= 7.23.1; python_version >= "3.8"
 ipywidgets>=7.4.2, <8.0.0
 keyring>=13.2.1
 KqlmagicCustom[jupyter-basic,auth_code_clipboard]>=0.1.114.post22
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
@@ -35,14 +37,15 @@
 msrest>=0.6.0
 msrestazure>=0.6.0
 nest_asyncio>=1.4.0
 networkx>=2.2
 numpy>=1.15.4  # pandas
 openpyxl>=3.0
 pandas>=1.4.0, <2.0.0
+panel>=0.14.4
 passivetotal>=2.5.3
 pygments>=2.0.0
 pyjwt>=2.3.0
 python-dateutil>=2.8.1  # pandas
 pytz>=2019.2  # pandas
 pyyaml>=3.13
 scikit-learn>=1.0.0
```

### Comparing `msticpy-2.4.0/requirements-dev.txt` & `msticpy-2.5.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/requirements.txt` & `msticpy-2.5.0/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,22 +6,21 @@
 beautifulsoup4>=4.0.0
 bokeh>=1.4.0, <=2.4.3
 cryptography>=3.1
 deprecated>=1.2.4
 dnspython>=2.0.0, <3.0.0
 folium>=0.9.0
 geoip2>=2.9.0
-httpx==0.23.3
+httpx==0.24.0
 html5lib
 ipython >= 7.1.1; python_version < "3.8"
 ipython >= 7.23.1; python_version >= "3.8"
 ipywidgets>=7.4.2, <8.0.0
 KqlmagicCustom[jupyter-basic,auth_code_clipboard]>=0.1.114.post22
 lxml>=4.6.5
-matplotlib>=3.0.0
 msal>=1.12.0
 msal_extensions>=0.3.0
 msrest>=0.6.0
 msrestazure>=0.6.0
 nest_asyncio>=1.4.0
 networkx>=2.2
 numpy>=1.15.4  # pandas
```

### Comparing `msticpy-2.4.0/setup.cfg` & `msticpy-2.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `msticpy-2.4.0/setup.py` & `msticpy-2.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,34 +37,44 @@
         "azure-mgmt-core>=1.2.1",
         "azure-mgmt-monitor>=2.0.0",
         "azure-mgmt-network>=2.7.0",
         "azure-mgmt-resource>=16.1.0",
         "azure-storage-blob>=12.5.0",
         "azure-mgmt-resourcegraph>=8.0.0",
     ],
+    "azure_query": [
+        "azure-kusto-data>=4.0.0",
+        "azure-monitor-query>=1.0.0",
+    ],
     "keyvault": [
         "azure-keyvault-secrets>=4.0.0",
         "azure-mgmt-keyvault>=2.0.0",
         "keyring>=13.2.1",  # needed by Key Vault package
     ],
-    "ml": ["scikit-learn>=1.0.0", "scipy>=1.1.0", "statsmodels>=0.11.1"],
+    "ml": [
+        "scikit-learn>=1.0.0",
+        "scipy>=1.1.0",
+        "statsmodels>=0.11.1",
+        "matplotlib>=3.0.0",
+    ],
     "sql2kql": ["mo-sql-parsing>=8, <9.0.0"],
     "riskiq": ["passivetotal>=2.5.3"],
+    "panel": ["panel>=0.14.4"],
 }
 extras_all = [
     extra for name, extras in EXTRAS.items() for extra in extras if name != "dev"
 ]
 EXTRAS["all"] = extras_all
 
 # Create combination extras
 EXTRAS["all"] = sorted(
     _combine_extras(list({name for name in EXTRAS if name != "dev"}))
 )
 
-EXTRAS["azure"] = sorted(_combine_extras(["_azure_core", "keyvault"]))
+EXTRAS["azure"] = sorted(_combine_extras(["_azure_core", "keyvault", "azure_query"]))
 EXTRAS["test"] = sorted(_combine_extras(["all", "dev"]))
 EXTRAS["azsentinel"] = sorted(_combine_extras(["azure", "kql", "keyvault"]))
 EXTRAS["azuresentinel"] = sorted(_combine_extras(["azure", "kql", "keyvault"]))
 EXTRAS["sentinel"] = sorted(_combine_extras(["azure", "kql", "keyvault"]))
 
 
 if __name__ == "__main__":
```

