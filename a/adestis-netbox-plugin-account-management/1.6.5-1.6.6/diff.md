# Comparing `tmp/adestis-netbox-plugin-account-management-1.6.5.tar.gz` & `tmp/adestis-netbox-plugin-account-management-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adestis-netbox-plugin-account-management-1.6.5.tar", last modified: Tue May 30 12:14:14 2023, max compression
+gzip compressed data, was "adestis-netbox-plugin-account-management-1.6.6.tar", last modified: Tue May 30 15:03:40 2023, max compression
```

## Comparing `adestis-netbox-plugin-account-management-1.6.5.tar` & `adestis-netbox-plugin-account-management-1.6.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 12:14:14.463203 adestis-netbox-plugin-account-management-1.6.5/
--rw-rw-rw-   0        0        0     1088 2023-02-09 23:32:58.000000 adestis-netbox-plugin-account-management-1.6.5/LICENSE
--rw-rw-rw-   0        0        0      175 2023-05-30 11:37:32.000000 adestis-netbox-plugin-account-management-1.6.5/MANIFEST.in
--rw-rw-rw-   0        0        0      326 2023-05-30 12:14:14.388201 adestis-netbox-plugin-account-management-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     1374 2023-05-30 11:37:32.000000 adestis-netbox-plugin-account-management-1.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 12:14:13.303182 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/
--rw-rw-rw-   0        0        0      494 2023-05-30 11:56:56.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:14:13.462184 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/api/
--rw-rw-rw-   0        0        0        0 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/api/__init__.py
--rw-rw-rw-   0        0        0      516 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/api/nested_serializer.py
--rw-rw-rw-   0        0        0     2693 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/api/serializers.py
--rw-rw-rw-   0        0        0      301 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/api/urls.py
--rw-rw-rw-   0        0        0      659 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/api/views.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:14:13.526182 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/filtersets/
--rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/filtersets/__init__.py
--rw-rw-rw-   0        0        0     1899 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/filtersets/login_credentials.py
--rw-rw-rw-   0        0        0     2610 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/filtersets/system.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:14:13.579186 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/forms/
--rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/forms/__init__.py
--rw-rw-rw-   0        0        0     4733 2023-05-30 12:09:40.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/forms/login_credentials.py
--rw-rw-rw-   0        0        0     8074 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/forms/system.py
--rw-rw-rw-   0        0        0      878 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/graphql.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:14:13.835186 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/
--rw-rw-rw-   0        0        0     4725 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      444 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0002_alter_system_system_url.py
--rw-rw-rw-   0        0        0      756 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py
--rw-rw-rw-   0        0        0     4163 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py
--rw-rw-rw-   0        0        0     1470 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py
--rw-rw-rw-   0        0        0      761 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py
--rw-rw-rw-   0        0        0      286 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0007_remove_logincredentials_person.py
--rw-rw-rw-   0        0        0      662 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py
--rw-rw-rw-   0        0        0        0 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:14:13.942185 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/models/
--rw-rw-rw-   0        0        0       80 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/models/__init__.py
--rw-rw-rw-   0        0        0     3303 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/models/login_credentials.py
--rw-rw-rw-   0        0        0     2805 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/models/person.py
--rw-rw-rw-   0        0        0     3347 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/models/system.py
--rw-rw-rw-   0        0        0     1331 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/navigation.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:14:14.028778 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/tables/
--rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/tables/__init__.py
--rw-rw-rw-   0        0        0      939 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/tables/login_credentials.py
--rw-rw-rw-   0        0        0     1180 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/tables/system.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:14:13.170181 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/templates/
-drwxrwxrwx   0        0        0        0 2023-05-30 12:14:14.213199 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/
--rw-rw-rw-   0        0        0      371 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/device_login_credentials_table.html
--rw-rw-rw-   0        0        0     1685 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html
--rw-rw-rw-   0        0        0     2865 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html
--rw-rw-rw-   0        0        0     2110 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/urls.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:14:14.372200 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/views/
--rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/views/__init__.py
--rw-rw-rw-   0        0        0     2544 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/views/login_credentials.py
--rw-rw-rw-   0        0        0     1734 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/views/system.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:14:13.367191 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management.egg-info/
--rw-rw-rw-   0        0        0      326 2023-05-30 12:14:12.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2988 2023-05-30 12:14:12.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 12:14:12.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-30 12:14:12.000000 adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 12:14:14.464203 adestis-netbox-plugin-account-management-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0      602 2023-05-30 12:13:53.000000 adestis-netbox-plugin-account-management-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:03:40.007635 adestis-netbox-plugin-account-management-1.6.6/
+-rw-rw-rw-   0        0        0     1088 2023-02-09 23:32:58.000000 adestis-netbox-plugin-account-management-1.6.6/LICENSE
+-rw-rw-rw-   0        0        0      175 2023-05-30 11:37:32.000000 adestis-netbox-plugin-account-management-1.6.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      326 2023-05-30 15:03:39.988637 adestis-netbox-plugin-account-management-1.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1374 2023-05-30 11:37:32.000000 adestis-netbox-plugin-account-management-1.6.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 15:03:38.854226 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/
+-rw-rw-rw-   0        0        0      494 2023-05-30 12:56:32.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:03:38.999538 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/
+-rw-rw-rw-   0        0        0        0 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/__init__.py
+-rw-rw-rw-   0        0        0      516 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/nested_serializer.py
+-rw-rw-rw-   0        0        0     2693 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/serializers.py
+-rw-rw-rw-   0        0        0      301 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/urls.py
+-rw-rw-rw-   0        0        0      659 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/views.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.076328 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/filtersets/
+-rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/filtersets/__init__.py
+-rw-rw-rw-   0        0        0     1899 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/filtersets/login_credentials.py
+-rw-rw-rw-   0        0        0     2610 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/filtersets/system.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.148741 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/forms/
+-rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/forms/__init__.py
+-rw-rw-rw-   0        0        0     4733 2023-05-30 12:18:13.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/forms/login_credentials.py
+-rw-rw-rw-   0        0        0     8074 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/forms/system.py
+-rw-rw-rw-   0        0        0      878 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/graphql.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.400424 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/
+-rw-rw-rw-   0        0        0     4725 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      444 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0002_alter_system_system_url.py
+-rw-rw-rw-   0        0        0      756 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py
+-rw-rw-rw-   0        0        0     4163 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py
+-rw-rw-rw-   0        0        0     1470 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py
+-rw-rw-rw-   0        0        0      761 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py
+-rw-rw-rw-   0        0        0      286 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0007_remove_logincredentials_person.py
+-rw-rw-rw-   0        0        0      662 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py
+-rw-rw-rw-   0        0        0        0 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.512797 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/
+-rw-rw-rw-   0        0        0       80 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/__init__.py
+-rw-rw-rw-   0        0        0     3303 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/login_credentials.py
+-rw-rw-rw-   0        0        0     2805 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/person.py
+-rw-rw-rw-   0        0        0     3347 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/system.py
+-rw-rw-rw-   0        0        0     1331 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/navigation.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.593633 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/tables/
+-rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/tables/__init__.py
+-rw-rw-rw-   0        0        0      947 2023-05-30 14:24:33.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/tables/login_credentials.py
+-rw-rw-rw-   0        0        0     1180 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/tables/system.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:03:38.721206 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/
+drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.820637 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/
+-rw-rw-rw-   0        0        0      371 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/device_login_credentials_table.html
+-rw-rw-rw-   0        0        0     1685 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html
+-rw-rw-rw-   0        0        0     2865 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html
+-rw-rw-rw-   0        0        0     2110 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/urls.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.964632 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/views/
+-rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/views/__init__.py
+-rw-rw-rw-   0        0        0     2544 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/views/login_credentials.py
+-rw-rw-rw-   0        0        0     1734 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/views/system.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:03:38.911543 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-05-30 15:03:37.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2988 2023-05-30 15:03:38.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 15:03:37.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-30 15:03:37.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 15:03:40.010641 adestis-netbox-plugin-account-management-1.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      602 2023-05-30 12:56:38.000000 adestis-netbox-plugin-account-management-1.6.6/setup.py
```

### Comparing `adestis-netbox-plugin-account-management-1.6.5/LICENSE` & `adestis-netbox-plugin-account-management-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/README.md` & `adestis-netbox-plugin-account-management-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/api/nested_serializer.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/nested_serializer.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/api/serializers.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/serializers.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/api/views.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/views.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/filtersets/login_credentials.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/filtersets/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/filtersets/system.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/filtersets/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/forms/login_credentials.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/forms/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/forms/system.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/forms/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/graphql.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/graphql.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0001_initial.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/models/login_credentials.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/models/person.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/person.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/models/system.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/navigation.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/navigation.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/tables/login_credentials.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/tables/login_credentials.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,8 +24,8 @@
     tags = columns.TagColumn()
 
     class Meta(NetBoxTable.Meta):
         model = LoginCredentials
         fields = ['pk', 'id', 'logon_name', 'contact', 'system', 'valid_from', 'valid_to',
                   'login_credentials_status', 'comments', 'actions', 'tags', 'created', 'last_updated']
         default_columns = ['logon_name', 'contact', 'system', 'valid_from', 'valid_to',
-                           'login_credentials_status']
+                           'login_credentials_status', 'tags']
```

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/tables/system.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/tables/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/urls.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/urls.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/views/login_credentials.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/views/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management/views/system.py` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/views/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt` & `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.5/setup.py` & `adestis-netbox-plugin-account-management-1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='adestis-netbox-plugin-account-management',
-    version='1.6.5',
+    version='1.6.6',
     description='ADESTIS Account Management',
     url='https://github.com/adestis/netbox-account-management',
     author='ADESTIS GmbH',
     author_email='pypi@adestis.de',
     install_requires=[],
     packages=find_packages(),
     include_package_data=True,
```

