# Comparing `tmp/IntuneCD-1.4.7.tar.gz` & `tmp/IntuneCD-1.4.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IntuneCD-1.4.7.tar", last modified: Tue May 30 08:45:11 2023, max compression
+gzip compressed data, was "IntuneCD-1.4.7b1.tar", last modified: Sat May 27 12:22:39 2023, max compression
```

## Comparing `IntuneCD-1.4.7.tar` & `IntuneCD-1.4.7b1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:45:11.827232 IntuneCD-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-30 08:45:11.827232 IntuneCD-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-30 08:45:11.827232 IntuneCD-1.4.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:45:11.815232 IntuneCD-1.4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:45:11.823232 IntuneCD-1.4.7/src/IntuneCD/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/assignment_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_AppProtection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_apns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_appConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_appleEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_assignmentFilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_autopilotDevices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_compliancePartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_conditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_configurationPolicies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_customAttributeShellScript.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_deviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_enrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_enrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_groupPolicyConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_managedGPlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_managementIntents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_managementPartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_notificationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_powershellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_proactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_remoteAssistancePartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_shellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_vppTokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/backup_windowsEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/check_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/clean_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/diff_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/get_accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/get_authparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/graph_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/remove_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/run_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/run_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/run_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/save_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_appConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_appProtection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_appleEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_assignmentFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_conditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_configurationPolicies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_customAttributeShellScript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_deviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_enrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_enrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_groupPolicyConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_managementIntents.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_notificationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_powershellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_proactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16118 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_shellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/src/IntuneCD/update_windowsEnrollmentProfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:45:11.827232 IntuneCD-1.4.7/src/IntuneCD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-30 08:45:11.000000 IntuneCD-1.4.7/src/IntuneCD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-30 08:45:11.000000 IntuneCD-1.4.7/src/IntuneCD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:45:11.000000 IntuneCD-1.4.7/src/IntuneCD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-30 08:45:11.000000 IntuneCD-1.4.7/src/IntuneCD.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 08:45:11.000000 IntuneCD-1.4.7/src/IntuneCD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 08:45:11.000000 IntuneCD-1.4.7/src/IntuneCD.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:45:11.827232 IntuneCD-1.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_check_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_clean_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_diff_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_get_added_removed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_get_authparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_graph_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    17428 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_group_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_remove_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_save_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-30 08:45:00.000000 IntuneCD-1.4.7/tests/test_update_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:38.995552 IntuneCD-1.4.7b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/src/IntuneCD/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/assignment_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_AppProtection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_apns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_appConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_appleEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_assignmentFilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_autopilotDevices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_compliancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_conditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_configurationPolicies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_customAttributeShellScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_deviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_enrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_enrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_groupPolicyConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_managedGPlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_managementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_managementPartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_notificationTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_powershellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_proactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_remoteAssistancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_shellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_vppTokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_windowsEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/check_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/clean_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/diff_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/get_accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/get_authparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/graph_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/load_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/remove_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/run_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/run_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/run_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/save_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_appConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_appProtection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_appleEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_assignmentFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_conditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_configurationPolicies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_customAttributeShellScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_deviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_enrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_enrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_groupPolicyConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_managementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_notificationTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_powershellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_proactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16118 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_shellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_windowsEnrollmentProfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_check_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_clean_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_diff_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_get_added_removed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_get_authparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_graph_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17428 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_group_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_load_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_remove_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_save_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_update_frontend.py
```

### Comparing `IntuneCD-1.4.7/LICENSE` & `IntuneCD-1.4.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/PKG-INFO` & `IntuneCD-1.4.7b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.7
+Version: 1.4.7b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.7/README.md` & `IntuneCD-1.4.7b1/README.md`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/setup.cfg` & `IntuneCD-1.4.7b1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = IntuneCD
-version = 1.4.7
+version = 1.4.7.beta1
 author = Tobias Almén
 author_email = almenscorner@outlook.com
 description = Tool to backup and update configurations in Intune
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/almenscorner/IntuneCD
 project_urls =
```

### Comparing `IntuneCD-1.4.7/src/IntuneCD/archive.py` & `IntuneCD-1.4.7b1/src/IntuneCD/archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/assignment_report.py` & `IntuneCD-1.4.7b1/src/IntuneCD/assignment_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_AppProtection.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_AppProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_apns.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_apns.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_appConfiguration.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_appConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_appleEnrollmentProfile.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_applications.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_applications.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_assignmentFilters.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_assignmentFilters.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_autopilotDevices.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_autopilotDevices.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_compliance.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_compliancePartner.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_compliancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_conditionalAccess.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_conditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_configurationPolicies.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_configurationPolicies.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_customAttributeShellScript.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_customAttributeShellScript.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_deviceManagementSettings.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_enrollmentConfigurations.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_enrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_enrollmentStatusPage.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_enrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_groupPolicyConfiguration.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_groupPolicyConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_managedGPlay.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_managedGPlay.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_managementIntents.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_managementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_managementPartner.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_managementPartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_notificationTemplate.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_notificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_powershellScripts.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_powershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_proactiveRemediation.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_proactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_profiles.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_profiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_remoteAssistancePartner.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_remoteAssistancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_shellScripts.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_shellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_vppTokens.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_vppTokens.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/backup_windowsEnrollmentProfile.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_windowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/check_file.py` & `IntuneCD-1.4.7b1/src/IntuneCD/check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/clean_filename.py` & `IntuneCD-1.4.7b1/src/IntuneCD/clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/diff_summary.py` & `IntuneCD-1.4.7b1/src/IntuneCD/diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/documentation_functions.py` & `IntuneCD-1.4.7b1/src/IntuneCD/documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/get_accesstoken.py` & `IntuneCD-1.4.7b1/src/IntuneCD/get_accesstoken.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/get_authparams.py` & `IntuneCD-1.4.7b1/src/IntuneCD/get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/graph_batch.py` & `IntuneCD-1.4.7b1/src/IntuneCD/graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/graph_request.py` & `IntuneCD-1.4.7b1/src/IntuneCD/graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/load_file.py` & `IntuneCD-1.4.7b1/src/IntuneCD/load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/remove_keys.py` & `IntuneCD-1.4.7b1/src/IntuneCD/remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/run_backup.py` & `IntuneCD-1.4.7b1/src/IntuneCD/run_backup.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/run_documentation.py` & `IntuneCD-1.4.7b1/src/IntuneCD/run_documentation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/run_update.py` & `IntuneCD-1.4.7b1/src/IntuneCD/run_update.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/save_output.py` & `IntuneCD-1.4.7b1/src/IntuneCD/save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_appConfiguration.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_appConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_appProtection.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_appProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_appleEnrollmentProfile.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_assignment.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_assignment.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_assignmentFilter.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_assignmentFilter.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_compliance.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_conditionalAccess.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_conditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_configurationPolicies.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_configurationPolicies.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_customAttributeShellScript.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_customAttributeShellScript.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_deviceManagementSettings.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_enrollmentConfigurations.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_enrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_enrollmentStatusPage.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_enrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_frontend.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_frontend.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_groupPolicyConfiguration.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_groupPolicyConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_managementIntents.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_managementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_notificationTemplate.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_notificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_powershellScripts.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_powershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_proactiveRemediation.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_proactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_profiles.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_profiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_shellScripts.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_shellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD/update_windowsEnrollmentProfile.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_windowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/src/IntuneCD.egg-info/PKG-INFO` & `IntuneCD-1.4.7b1/src/IntuneCD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.7
+Version: 1.4.7b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.7/src/IntuneCD.egg-info/SOURCES.txt` & `IntuneCD-1.4.7b1/src/IntuneCD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_archive.py` & `IntuneCD-1.4.7b1/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_check_file.py` & `IntuneCD-1.4.7b1/tests/test_check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_clean_filename.py` & `IntuneCD-1.4.7b1/tests/test_clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_diff_summary.py` & `IntuneCD-1.4.7b1/tests/test_diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_documentation_functions.py` & `IntuneCD-1.4.7b1/tests/test_documentation_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,27 +107,27 @@
 
         self.assertEqual(self.result, self.expected_list)
 
     def test_document_configs(self):
         """The list should be returned."""
         self.directory.write(
             "config/test_file_name.json",
-            '{"@odata.type":"test","test":"test","name":"test","description":"test","testvals":"1,2","testbool":false,"testlist":["test"],"testlistdict":[{"test":{"test":{"test":["1"],"testb64":"dW5pY29ybg=="}}}],"testdict2":{"test":{"test":{"test":["1"]}}},"testdictlist":{"test":["a","b","c"]},"assignments":[{"intent":"apply","target":{"@odata.type":"#test","groupName":"test-group","deviceAndAppManagementAssignmentFilterId":"test-filter","deviceAndAppManagementAssignmentFilterType":"test"}}]}',
+            '{"@odata.type":"test","test":"test","name":"test","description":"test","testvals":"1,2","testbool":false,"testlist":["test"],"testlistdict":[{"test":{"test":{"test":["1"]}}}],"testdict2":{"test":{"test":{"test":["1"]}}},"testdictlist":{"test":["a","b","c"]},"assignments":[{"intent":"apply","target":{"@odata.type":"#test","groupName":"test-group","deviceAndAppManagementAssignmentFilterId":"test-filter","deviceAndAppManagementAssignmentFilterType":"test"}}]}',
             encoding="utf-8",
         )
-        self.expected_data = "#test##testDescription:test###Assignments|intent|target|filtertype|filtername||------|----------|-----------|-----------||apply|test-group|test|test-filter|###Configuration|setting|value||------------|--------------------------------------------------------------------------------||Odatatype|test||Test|test||Name|test||Testvals|1,2||Testbool|False||Testlist|test<br/>||Testlistdict|**test:**<ul>**test:**<ul><li>1</li></ul>**testb64:**unicorn</br></ul><br/>||Testdict2|**test**<ul>**test:**<ul><li>1</li></ul><br/></ul>||Testdictlist|**test:**<ul><li>a</li><li>b</li><li>c</li></ul>|"
+        self.expected_data = "#test##testDescription:test###Assignments|intent|target|filtertype|filtername||------|----------|-----------|-----------||apply|test-group|test|test-filter|###Configuration|setting|value||------------|-------------------------------------------------------||Odatatype|test||Test|test||Name|test||Testvals|1,2||Testbool|False||Testlist|test<br/>||Testlistdict|**test:**<ul>**test:**<ul><li>1</li></ul></ul><br/>||Testdict2|**test**<ul>**test:**<ul><li>1</li></ul><br/></ul>||Testdictlist|**test:**<ul><li>a</li><li>b</li><li>c</li></ul>|"
 
         document_configs(
             f"{self.directory.path}/config",
             f"{self.directory.path}/test.md",
             "test",
             100,
             split=False,
             cleanup=True,
-            decode=True,
+            decode=False,
         )
 
         with open(f"{self.directory.path}/test.md", "r") as f:
             self.data = f.read()
             self.result = "".join([line.strip() for line in self.data])
 
         self.assertEqual(self.result, self.expected_data)
```

### Comparing `IntuneCD-1.4.7/tests/test_get_added_removed.py` & `IntuneCD-1.4.7b1/tests/test_get_added_removed.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_get_authparams.py` & `IntuneCD-1.4.7b1/tests/test_get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_graph_batch.py` & `IntuneCD-1.4.7b1/tests/test_graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_graph_request.py` & `IntuneCD-1.4.7b1/tests/test_graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_group_report.py` & `IntuneCD-1.4.7b1/tests/test_group_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_load_file.py` & `IntuneCD-1.4.7b1/tests/test_load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_match.py` & `IntuneCD-1.4.7b1/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_remove_keys.py` & `IntuneCD-1.4.7b1/tests/test_remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_save_output.py` & `IntuneCD-1.4.7b1/tests/test_save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7/tests/test_update_frontend.py` & `IntuneCD-1.4.7b1/tests/test_update_frontend.py`

 * *Files identical despite different names*

