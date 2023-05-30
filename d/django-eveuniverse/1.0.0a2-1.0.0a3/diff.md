# Comparing `tmp/django_eveuniverse-1.0.0a2.tar.gz` & `tmp/django_eveuniverse-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "django_eveuniverse-1.0.0a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_eveuniverse-1.0.0a2.tar` & `django_eveuniverse-1.0.0a3.tar`

### file list

```diff
@@ -1,72 +1,71 @@
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/__init__.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/admin.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/app_settings.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/apps.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/backends.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/constants.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/helpers.py
--rw-r--r--   0        0        0    41499 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/managers.py
--rw-r--r--   0        0        0    58930 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/models.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/providers.py
--rw-r--r--   0        0        0   887006 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/swagger.json
--rw-r--r--   0        0        0    10500 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tasks.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/__init__.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/dotlan.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/esitools.py
--rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/eveimageserver.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/eveitems.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/evemicros.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/evesdeapi.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/eveskinserver.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/evewho.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/evexml.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/zkillboard.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/management/commands/__init__.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/management/commands/eveuniverse_load_data.py
--rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/management/commands/eveuniverse_load_types.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/management/commands/eveuniverse_purge_data.py
--rw-r--r--   0        0        0    51659 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0001_initial.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0002_load_eveunit.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0003_evemarketprice.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0004_effect_longer_name.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0005_type_materials_and_sections.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0006_alter_evedogmaeffectmodifier_operator.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0007_evetype_description.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/__init__.py
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/eve_unit.json
--rw-r--r--   0        0        0    14542 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/static/eveuniverse/skin_generic_128.png
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/static/eveuniverse/skin_generic_32.png
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/static/eveuniverse/skin_generic_64.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/pilot.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_backends.py
--rw-r--r--   0        0        0    10286 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_commands.py
--rw-r--r--   0        0        0    22388 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_core.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_helpers.py
--rw-r--r--   0        0        0    42399 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_1.py
--rw-r--r--   0        0        0    28631 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_2.py
--rw-r--r--   0        0        0    43206 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_3.py
--rw-r--r--   0        0        0    30849 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_4.py
--rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_tasks.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_tools_testdata.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_utils.py
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata_example.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/__init__.py
--rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/esi.py
--rw-r--r--   0        0        0    78321 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/esi_data.json
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/factories.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/fetch_esi_raw_data.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/generate_sde.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/sde.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/sde_data.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/tools/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/tools/clear_celery_once_locks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tools/__init__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tools/drop_tables.sql
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tools/testdata.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/LICENSE
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/README.md
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2020-10-23 18:01:44.555775 django_eveuniverse-1.0.0a3/LICENSE
+-rw-r--r--   0        0        0     2912 2023-05-29 23:34:30.809916 django_eveuniverse-1.0.0a3/README.rst
+-rw-r--r--   0        0        0      110 2023-05-29 22:01:07.214581 django_eveuniverse-1.0.0a3/eveuniverse/__init__.py
+-rw-r--r--   0        0        0     1314 2020-10-23 18:01:44.567774 django_eveuniverse-1.0.0a3/eveuniverse/admin.py
+-rw-r--r--   0        0        0     2753 2023-04-15 14:33:43.514933 django_eveuniverse-1.0.0a3/eveuniverse/app_settings.py
+-rw-r--r--   0        0        0      254 2022-03-01 16:54:35.914600 django_eveuniverse-1.0.0a3/eveuniverse/apps.py
+-rw-r--r--   0        0        0      873 2023-05-29 21:04:02.196043 django_eveuniverse-1.0.0a3/eveuniverse/backends.py
+-rw-r--r--   0        0        0      370 2023-04-15 10:37:18.591750 django_eveuniverse-1.0.0a3/eveuniverse/constants.py
+-rw-r--r--   0        0        0        0 2023-05-30 00:29:12.272272 django_eveuniverse-1.0.0a3/eveuniverse/core/__init__.py
+-rw-r--r--   0        0        0     1781 2022-02-11 14:09:07.543015 django_eveuniverse-1.0.0a3/eveuniverse/core/dotlan.py
+-rw-r--r--   0        0        0      423 2022-06-18 12:37:45.694321 django_eveuniverse-1.0.0a3/eveuniverse/core/esitools.py
+-rw-r--r--   0        0        0     5127 2023-05-29 21:04:02.196043 django_eveuniverse-1.0.0a3/eveuniverse/core/eveimageserver.py
+-rw-r--r--   0        0        0      358 2022-01-04 21:23:14.332955 django_eveuniverse-1.0.0a3/eveuniverse/core/eveitems.py
+-rw-r--r--   0        0        0     2598 2023-05-29 21:04:02.196043 django_eveuniverse-1.0.0a3/eveuniverse/core/evemicros.py
+-rw-r--r--   0        0        0     2431 2023-05-29 21:04:02.196043 django_eveuniverse-1.0.0a3/eveuniverse/core/evesdeapi.py
+-rw-r--r--   0        0        0      457 2022-01-04 21:23:14.332955 django_eveuniverse-1.0.0a3/eveuniverse/core/eveskinserver.py
+-rw-r--r--   0        0        0     1145 2023-05-29 21:04:02.196043 django_eveuniverse-1.0.0a3/eveuniverse/core/evewho.py
+-rw-r--r--   0        0        0     2864 2022-02-11 14:41:18.613728 django_eveuniverse-1.0.0a3/eveuniverse/core/evexml.py
+-rw-r--r--   0        0        0     1713 2023-05-29 21:04:02.196043 django_eveuniverse-1.0.0a3/eveuniverse/core/zkillboard.py
+-rw-r--r--   0        0        0     1644 2023-05-29 21:04:02.200043 django_eveuniverse-1.0.0a3/eveuniverse/helpers.py
+-rw-r--r--   0        0        0      365 2023-04-15 10:37:18.591750 django_eveuniverse-1.0.0a3/eveuniverse/management/commands/__init__.py
+-rw-r--r--   0        0        0     4574 2023-04-15 10:37:18.591750 django_eveuniverse-1.0.0a3/eveuniverse/management/commands/eveuniverse_load_data.py
+-rw-r--r--   0        0        0     5348 2023-04-15 10:37:18.591750 django_eveuniverse-1.0.0a3/eveuniverse/management/commands/eveuniverse_load_types.py
+-rw-r--r--   0        0        0     1644 2021-04-16 13:44:19.227872 django_eveuniverse-1.0.0a3/eveuniverse/management/commands/eveuniverse_purge_data.py
+-rw-r--r--   0        0        0    42091 2023-05-29 21:04:02.200043 django_eveuniverse-1.0.0a3/eveuniverse/managers.py
+-rw-r--r--   0        0        0    51659 2023-04-15 17:15:38.755939 django_eveuniverse-1.0.0a3/eveuniverse/migrations/0001_initial.py
+-rw-r--r--   0        0        0      968 2023-04-15 17:15:38.755939 django_eveuniverse-1.0.0a3/eveuniverse/migrations/0002_load_eveunit.py
+-rw-r--r--   0        0        0     1009 2023-04-15 17:15:38.755939 django_eveuniverse-1.0.0a3/eveuniverse/migrations/0003_evemarketprice.py
+-rw-r--r--   0        0        0      478 2023-04-15 17:15:38.755939 django_eveuniverse-1.0.0a3/eveuniverse/migrations/0004_effect_longer_name.py
+-rw-r--r--   0        0        0     2702 2023-04-15 17:15:38.755939 django_eveuniverse-1.0.0a3/eveuniverse/migrations/0005_type_materials_and_sections.py
+-rw-r--r--   0        0        0      429 2023-04-15 17:15:38.759939 django_eveuniverse-1.0.0a3/eveuniverse/migrations/0006_alter_evedogmaeffectmodifier_operator.py
+-rw-r--r--   0        0        0      409 2023-04-15 17:15:38.759939 django_eveuniverse-1.0.0a3/eveuniverse/migrations/0007_evetype_description.py
+-rw-r--r--   0        0        0        0 2023-05-30 00:29:12.276272 django_eveuniverse-1.0.0a3/eveuniverse/migrations/__init__.py
+-rw-r--r--   0        0        0     5336 2020-11-20 16:10:16.158594 django_eveuniverse-1.0.0a3/eveuniverse/migrations/eve_unit.json
+-rw-r--r--   0        0        0    59855 2023-05-29 21:04:02.200043 django_eveuniverse-1.0.0a3/eveuniverse/models.py
+-rw-r--r--   0        0        0      250 2022-06-18 12:37:45.694321 django_eveuniverse-1.0.0a3/eveuniverse/providers.py
+-rw-r--r--   0        0        0    14542 2020-12-18 18:17:56.637925 django_eveuniverse-1.0.0a3/eveuniverse/static/eveuniverse/skin_generic_128.png
+-rw-r--r--   0        0        0     2142 2020-12-18 18:17:56.637925 django_eveuniverse-1.0.0a3/eveuniverse/static/eveuniverse/skin_generic_32.png
+-rw-r--r--   0        0        0     4141 2020-12-18 18:17:56.637925 django_eveuniverse-1.0.0a3/eveuniverse/static/eveuniverse/skin_generic_64.png
+-rw-r--r--   0        0        0   887006 2022-06-18 12:37:45.702321 django_eveuniverse-1.0.0a3/eveuniverse/swagger.json
+-rw-r--r--   0        0        0    10774 2023-05-29 21:04:02.200043 django_eveuniverse-1.0.0a3/eveuniverse/tasks.py
+-rw-r--r--   0        0        0        0 2023-05-30 00:29:12.276272 django_eveuniverse-1.0.0a3/eveuniverse/tests/__init__.py
+-rw-r--r--   0        0        0     1274 2023-04-15 17:15:38.759939 django_eveuniverse-1.0.0a3/eveuniverse/tests/pilot.py
+-rw-r--r--   0        0        0     1046 2023-04-13 02:39:52.214185 django_eveuniverse-1.0.0a3/eveuniverse/tests/test_backends.py
+-rw-r--r--   0        0        0    10286 2023-04-13 19:30:17.215558 django_eveuniverse-1.0.0a3/eveuniverse/tests/test_commands.py
+-rw-r--r--   0        0        0    22736 2023-05-29 21:04:02.204043 django_eveuniverse-1.0.0a3/eveuniverse/tests/test_core.py
+-rw-r--r--   0        0        0     2136 2023-05-29 21:04:02.204043 django_eveuniverse-1.0.0a3/eveuniverse/tests/test_helpers.py
+-rw-r--r--   0        0        0    45961 2023-05-29 21:04:02.204043 django_eveuniverse-1.0.0a3/eveuniverse/tests/test_models_1.py
+-rw-r--r--   0        0        0    28631 2023-04-15 12:19:39.042614 django_eveuniverse-1.0.0a3/eveuniverse/tests/test_models_2.py
+-rw-r--r--   0        0        0    43206 2023-04-15 12:19:39.042614 django_eveuniverse-1.0.0a3/eveuniverse/tests/test_models_3.py
+-rw-r--r--   0        0        0    30849 2023-04-15 12:19:39.042614 django_eveuniverse-1.0.0a3/eveuniverse/tests/test_models_4.py
+-rw-r--r--   0        0        0     6759 2023-04-12 21:38:05.746923 django_eveuniverse-1.0.0a3/eveuniverse/tests/test_tasks.py
+-rw-r--r--   0        0        0     2958 2021-04-16 13:44:19.231871 django_eveuniverse-1.0.0a3/eveuniverse/tests/test_tools_testdata.py
+-rw-r--r--   0        0        0     3975 2023-04-15 17:15:38.759939 django_eveuniverse-1.0.0a3/eveuniverse/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 00:29:12.276272 django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     7725 2022-03-08 21:55:48.715606 django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/esi.py
+-rw-r--r--   0        0        0    78321 2023-04-15 12:19:39.042614 django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/esi_data.json
+-rw-r--r--   0        0        0     4500 2023-01-18 17:00:28.727344 django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/factories.py
+-rw-r--r--   0        0        0     1649 2023-04-15 14:33:43.518934 django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/fetch_esi_raw_data.py
+-rw-r--r--   0        0        0     1183 2023-04-05 13:26:14.320189 django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/generate_sde.py
+-rw-r--r--   0        0        0      584 2021-04-16 13:44:19.235871 django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/sde.py
+-rw-r--r--   0        0        0     4044 2021-02-21 19:32:52.395908 django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/sde_data.json
+-rw-r--r--   0        0        0     4636 2020-11-20 16:10:16.170594 django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata_example.json
+-rw-r--r--   0        0        0        0 2023-05-30 00:29:12.276272 django_eveuniverse-1.0.0a3/eveuniverse/tests/tools/__init__.py
+-rw-r--r--   0        0        0      760 2023-04-15 12:19:39.046614 django_eveuniverse-1.0.0a3/eveuniverse/tests/tools/clear_celery_once_locks.py
+-rw-r--r--   0        0        0        0 2023-05-30 00:29:12.276272 django_eveuniverse-1.0.0a3/eveuniverse/tools/__init__.py
+-rw-r--r--   0        0        0     1373 2020-11-20 16:10:16.170594 django_eveuniverse-1.0.0a3/eveuniverse/tools/drop_tables.sql
+-rw-r--r--   0        0        0     5235 2023-04-12 22:26:32.188851 django_eveuniverse-1.0.0a3/eveuniverse/tools/testdata.py
+-rw-r--r--   0        0        0     2817 2023-05-29 21:04:02.204043 django_eveuniverse-1.0.0a3/eveuniverse/utils.py
+-rw-r--r--   0        0        0     1802 2023-05-29 21:50:31.778126 django_eveuniverse-1.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     4263 1970-01-01 00:00:00.000000 django_eveuniverse-1.0.0a3/PKG-INFO
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/admin.py` & `django_eveuniverse-1.0.0a3/eveuniverse/admin.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/app_settings.py` & `django_eveuniverse-1.0.0a3/eveuniverse/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/backends.py` & `django_eveuniverse-1.0.0a3/eveuniverse/backends.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,12 +19,12 @@
     def __init__(self, settings):
         pass
 
     @staticmethod
     def raise_or_lock(key, timeout):
         acquired = cache.add(key=key, value="lock", timeout=timeout)
         if not acquired:
-            raise AlreadyQueued(int(cache.ttl(key)))
+            raise AlreadyQueued(int(cache.ttl(key)))  # type: ignore
 
     @staticmethod
     def clear_lock(key):
         return cache.delete(key)
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/helpers.py` & `django_eveuniverse-1.0.0a3/eveuniverse/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 import hashlib
 import json
 from typing import Any, Dict, Optional
 
 from django.db import models
 
 
-def meters_to_ly(value: float) -> float:
+def meters_to_ly(value: float) -> Optional[float]:
     """converts meters into lightyears"""
     return float(value) / 9_460_730_472_580_800 if value is not None else None
 
 
-def meters_to_au(value: float) -> float:
+def meters_to_au(value: float) -> Optional[float]:
     """converts meters into AU"""
     return float(value) / 149_597_870_691 if value is not None else None
 
 
 def get_or_create_esi_or_none(
     prop_name: str, dct: dict, Model: type
 ) -> Optional[models.Model]:
     """tries to create a new eveuniverse object from a dictionary entry
 
     return the object on success or None
     """
-    if dct.get(prop_name):
-        obj, _ = Model.objects.get_or_create_esi(id=dct.get(prop_name))
-    else:
-        obj = None
-
-    return obj
+    if eve_id := dct.get(prop_name):
+        return Model.objects.get_or_create_esi(id=eve_id)[0]  # type: ignore
+    return None
 
 
 class EveEntityNameResolver:
     """Container with a mapping between entity Ids and entity names
     and a performant API
     """
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/managers.py` & `django_eveuniverse-1.0.0a3/eveuniverse/managers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime as dt
 import logging
 from collections import defaultdict, namedtuple
-from typing import Iterable, List, Optional, Set, Tuple
+from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, TypeVar
 
 import requests
 from bravado.exception import HTTPNotFound
 from django.core.cache import cache
 from django.db import models, transaction
 from django.db.utils import IntegrityError
 from django.utils.timezone import now
@@ -24,15 +24,15 @@
 logger = LoggerAddTag(logging.getLogger(__name__), __title__)
 
 FakeResponse = namedtuple("FakeResponse", ["status_code"])
 
 
 class EveUniverseBaseModelManager(models.Manager):
     def _defaults_from_esi_obj(
-        self, eve_data_obj: dict, enabled_sections: Set[str] = None
+        self, eve_data_obj: dict, enabled_sections: Optional[Set[str]] = None
     ) -> dict:
         """compiles defaults from an esi data object for update/creating the model"""
         defaults = dict()
         for field_name, mapping in self.model._esi_mapping(enabled_sections).items():
             if not mapping.is_pk:
                 if not isinstance(mapping.esi_name, tuple):
                     if mapping.esi_name in eve_data_obj:
@@ -74,24 +74,27 @@
                             value = esi_value
 
                     defaults[field_name] = value
 
         return defaults
 
 
+ModelType = TypeVar("ModelType", bound=models.Model)
+
+
 class EveUniverseEntityModelManager(EveUniverseBaseModelManager):
     def get_or_create_esi(
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
-        enabled_sections: Iterable[str] = None,
-        task_priority: int = None,
-    ) -> Tuple[models.Model, bool]:
+        enabled_sections: Optional[Iterable[str]] = None,
+        task_priority: Optional[int] = None,
+    ) -> Tuple[ModelType, bool]:
         """gets or creates an eve universe object.
 
         The object is automatically fetched from ESI if it does not exist (blocking).
         Will always get/create parent objects.
 
         Args:
             id: Eve Online ID of object
@@ -100,25 +103,25 @@
             enabled_sections: Sections to load regardless of current settings, e.g. `[EveType.Section.DOGMAS]` will always load dogmas for EveTypes
             task_priority: priority of started tasks
 
         Returns:
             A tuple consisting of the requested object and a created flag
         """
         id = int(id)
-        enabled_sections = self.model.determine_effective_sections(enabled_sections)
+        effective_sections = self.model.determine_effective_sections(enabled_sections)
         try:
-            enabled_sections_filter = self._enabled_sections_filter(enabled_sections)
+            enabled_sections_filter = self._enabled_sections_filter(effective_sections)
             obj = self.filter(**enabled_sections_filter).get(id=id)
             return obj, False
         except self.model.DoesNotExist:
             return self.update_or_create_esi(
                 id=id,
                 include_children=include_children,
                 wait_for_children=wait_for_children,
-                enabled_sections=enabled_sections,
+                enabled_sections=effective_sections,
                 task_priority=task_priority,
             )
 
     def _enabled_sections_filter(self, enabled_sections: Iterable[str]) -> dict:
         return {
             "enabled_sections": getattr(self.model.enabled_sections, section)
             for section in enabled_sections
@@ -127,73 +130,73 @@
 
     def update_or_create_esi(
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
-        enabled_sections: Iterable[str] = None,
-        task_priority: int = None,
-    ) -> Tuple[models.Model, bool]:
+        enabled_sections: Optional[Iterable[str]] = None,
+        task_priority: Optional[int] = None,
+    ) -> Tuple[ModelType, bool]:
         """updates or creates an Eve universe object by fetching it from ESI (blocking).
         Will always get/create parent objects
 
         Args:
             id: Eve Online ID of object
             include_children: if child objects should be updated/created as well (if any)
             wait_for_children: when true child objects will be updated/created blocking (if any), else async
             enabled_sections: Sections to load regardless of current settings, e.g. `[EveType.Section.DOGMAS]` will always load dogmas for EveTypes
             task_priority: priority of started tasks
 
         Returns:
             A tuple consisting of the requested object and a created flag
         """
         id = int(id)
-        enabled_sections = self.model.determine_effective_sections(enabled_sections)
+        effective_sections = self.model.determine_effective_sections(enabled_sections)
         eve_data_obj = self._transform_esi_response_for_list_endpoints(
-            id, self._fetch_from_esi(id=id, enabled_sections=enabled_sections)
+            id, self._fetch_from_esi(id=id, enabled_sections=effective_sections)
         )
         if eve_data_obj:
-            defaults = self._defaults_from_esi_obj(eve_data_obj, enabled_sections)
+            defaults = self._defaults_from_esi_obj(eve_data_obj, effective_sections)
             obj, created = self.update_or_create(id=id, defaults=defaults)
-            if enabled_sections and hasattr(obj, "enabled_sections"):
+            if effective_sections and hasattr(obj, "enabled_sections"):
                 updated_sections = False
-                for section in enabled_sections:
+                for section in effective_sections:
                     if str(section) in self.model.Section.values():
                         setattr(obj.enabled_sections, section, True)
                         updated_sections = True
                 if updated_sections:
                     obj.save()
-            inline_objects = self.model._inline_objects(enabled_sections)
+            inline_objects = self.model._inline_objects(effective_sections)
             if inline_objects:
                 self._update_or_create_inline_objects(
                     parent_eve_data_obj=eve_data_obj,
                     parent_obj=obj,
                     inline_objects=inline_objects,
                     wait_for_children=wait_for_children,
-                    enabled_sections=enabled_sections,
+                    enabled_sections=effective_sections,
                     task_priority=task_priority,
                 )
             if include_children:
                 self._update_or_create_children(
                     parent_eve_data_obj=eve_data_obj,
                     include_children=include_children,
                     wait_for_children=wait_for_children,
-                    enabled_sections=enabled_sections,
+                    enabled_sections=effective_sections,
                     task_priority=task_priority,
                 )
         else:
             raise HTTPNotFound(
-                FakeResponse(status_code=404),
+                FakeResponse(status_code=404),  # type: ignore
                 message=f"{self.model.__name__} object with id {id} not found",
             )
         return obj, created
 
     def _fetch_from_esi(
-        self, id: int = None, enabled_sections: Iterable[str] = None
+        self, id: Optional[int] = None, enabled_sections: Optional[Iterable[str]] = None
     ) -> dict:
         """make request to ESI and return response data.
         Can handle raw ESI response from both list and normal endpoints.
         """
         if id is not None and not self.model._is_list_only_endpoint():
             args = {self.model._esi_pk(): id}
         else:
@@ -201,41 +204,40 @@
         category, method = self.model._esi_path_object()
         esi_data = getattr(
             getattr(esi.client, category),
             method,
         )(**args).results()
         return esi_data
 
-    def _transform_esi_response_for_list_endpoints(self, id: int, esi_data) -> object:
+    def _transform_esi_response_for_list_endpoints(self, id: int, esi_data) -> dict:
         """Transforms raw ESI response from list endpoints if this is one
         else just passes the ESI response through
         """
         if not self.model._is_list_only_endpoint():
             return esi_data
 
-        else:
-            esi_pk = self.model._esi_pk()
-            for row in esi_data:
-                if esi_pk in row and row[esi_pk] == id:
-                    return row
-
-            raise HTTPNotFound(
-                FakeResponse(status_code=404),
-                message=f"{self.model.__name__} object with id {id} not found",
-            )
+        esi_pk = self.model._esi_pk()
+        for row in esi_data:
+            if esi_pk in row and row[esi_pk] == id:
+                return row
+
+        raise HTTPNotFound(
+            FakeResponse(status_code=404),  # type: ignore
+            message=f"{self.model.__name__} object with id {id} not found",
+        )
 
     def _update_or_create_inline_objects(
         self,
         *,
         parent_eve_data_obj: dict,
-        parent_obj: models.Model,
+        parent_obj,
         inline_objects: dict,
         wait_for_children: bool,
         enabled_sections: Iterable[str],
-        task_priority: int = None,
+        task_priority: Optional[int] = None,
     ) -> None:
         """updates_or_creates eve objects that are returned "inline" from ESI
         for the parent eve objects as defined for this parent model (if any)
         """
         from .tasks import (
             update_or_create_inline_object as task_update_or_create_inline_object,
         )
@@ -288,37 +290,37 @@
                             eve_data_obj=eve_data_obj,
                             other_pk_info=other_pk_info,
                             parent2_model_name=parent2_model_name,
                             inline_model_name=model_name,
                             enabled_sections=enabled_sections,
                         )
                     else:
-                        params = {
+                        params: Dict[str, Any] = {
                             "kwargs": {
                                 "parent_obj_id": parent_obj.id,
                                 "parent_fk": parent_fk,
                                 "eve_data_obj": eve_data_obj,
                                 "other_pk_info": other_pk_info,
                                 "parent2_model_name": parent2_model_name,
                                 "inline_model_name": model_name,
                                 "parent_model_name": type(parent_obj).__name__,
                                 "enabled_sections": list(enabled_sections),
                             }
                         }
                         if task_priority:
                             params["priority"] = task_priority
-                        task_update_or_create_inline_object.apply_async(**params)
+                        task_update_or_create_inline_object.apply_async(**params)  # type: ignore
 
     def _update_or_create_inline_object(
         self,
         parent_obj_id: int,
         parent_fk: str,
         eve_data_obj: dict,
-        other_pk_info: dict,
-        parent2_model_name: str,
+        other_pk_info: Dict[str, Any],
+        parent2_model_name: Optional[str],
         inline_model_name: str,
         enabled_sections: Iterable[str],
     ):
         """Updates or creates a single inline object.
         Will automatically create additional parent objects as needed
         """
         InlineModel = self.model.get_model_class(inline_model_name)
@@ -333,28 +335,29 @@
                 try:
                     value, _ = ParentClass2.objects.update_or_create_esi(id=esi_value)
                 except AttributeError:
                     value = None
         else:
             value = esi_value
 
-        args[other_pk_info["name"]] = value
+        key = other_pk_info["name"]
+        args[key] = value  # type: ignore
         args["defaults"] = InlineModel.objects._defaults_from_esi_obj(
             eve_data_obj,
         )
         InlineModel.objects.update_or_create(**args)
 
     def _update_or_create_children(
         self,
         *,
         parent_eve_data_obj: dict,
         include_children: bool,
         wait_for_children: bool,
-        enabled_sections: Iterable[str] = None,
-        task_priority: int = None,
+        enabled_sections: Iterable[str],
+        task_priority: Optional[int] = None,
     ) -> None:
         """updates or creates child objects as defined for this parent model (if any)"""
         from .tasks import (
             update_or_create_eve_object as task_update_or_create_eve_object,
         )
 
         if not parent_eve_data_obj:
@@ -375,57 +378,57 @@
                             include_children=include_children,
                             wait_for_children=wait_for_children,
                             enabled_sections=enabled_sections,
                             task_priority=task_priority,
                         )
 
                     else:
-                        params = {
+                        params: Dict[str, Any] = {
                             "kwargs": {
                                 "model_name": child_class,
                                 "id": id,
                                 "include_children": include_children,
                                 "wait_for_children": wait_for_children,
                                 "enabled_sections": list(enabled_sections),
                                 "task_priority": task_priority,
                             },
                         }
                         if task_priority:
                             params["priority"] = task_priority
-                        task_update_or_create_eve_object.apply_async(**params)
+                        task_update_or_create_eve_object.apply_async(**params)  # type: ignore
 
     def update_or_create_all_esi(
         self,
         *,
         include_children: bool = False,
         wait_for_children: bool = True,
-        enabled_sections: Iterable[str] = None,
-        task_priority: int = None,
+        enabled_sections: Optional[Iterable[str]] = None,
+        task_priority: Optional[int] = None,
     ) -> None:
         """updates or creates all objects of this class from ESI.
 
         Loading all objects can take a long time. Use with care!
 
         Args:
             include_children: if child objects should be updated/created as well (if any)
             wait_for_children: when false all objects will be loaded async, else blocking
             enabled_sections: Sections to load regardless of current settings
         """
         from .tasks import (
             update_or_create_eve_object as task_update_or_create_eve_object,
         )
 
-        enabled_sections = self.model.determine_effective_sections(enabled_sections)
+        effective_sections = self.model.determine_effective_sections(enabled_sections)
 
         if self.model._is_list_only_endpoint():
             esi_pk = self.model._esi_pk()
             for eve_data_obj in self._fetch_from_esi():
                 args = {"id": eve_data_obj[esi_pk]}
                 args["defaults"] = self._defaults_from_esi_obj(
-                    eve_data_obj=eve_data_obj, enabled_sections=enabled_sections
+                    eve_data_obj=eve_data_obj, enabled_sections=effective_sections
                 )
                 self.update_or_create(**args)
 
         else:
             if self.model._has_esi_path_list():
                 category, method = self.model._esi_path_list()
                 ids = getattr(
@@ -434,44 +437,44 @@
                 )().results()
                 for id in ids:
                     if wait_for_children:
                         self.update_or_create_esi(
                             id=id,
                             include_children=include_children,
                             wait_for_children=wait_for_children,
-                            enabled_sections=enabled_sections,
+                            enabled_sections=effective_sections,
                         )
                     else:
-                        params = {
+                        params: Dict[str, Any] = {
                             "kwargs": {
                                 "model_name": self.model.__name__,
                                 "id": id,
                                 "include_children": include_children,
                                 "wait_for_children": wait_for_children,
-                                "enabled_sections": list(enabled_sections),
+                                "enabled_sections": list(effective_sections),
                                 "task_priority": task_priority,
                             },
                         }
                         if task_priority:
                             params["priority"] = task_priority
-                        task_update_or_create_eve_object.apply_async(**params)
+                        task_update_or_create_eve_object.apply_async(**params)  # type: ignore
 
             else:
                 raise TypeError(
                     f"ESI does not provide a list endpoint for {self.model.__name__}"
                 )
 
     def bulk_get_or_create_esi(
         self,
         *,
-        ids: List[int],
+        ids: Iterable[int],
         include_children: bool = False,
         wait_for_children: bool = True,
-        enabled_sections: Iterable[str] = None,
-        task_priority: int = None,
+        enabled_sections: Optional[Iterable[str]] = None,
+        task_priority: Optional[int] = None,
     ) -> models.QuerySet:
         """Gets or creates objects in bulk.
 
         Nonexisting objects will be fetched from ESI (blocking).
         Will always get/create parent objects.
 
         Args:
@@ -480,35 +483,37 @@
             wait_for_children: when true child objects will be updated/created blocking (if any), else async
             enabled_sections: Sections to load regardless of current settings
 
         Returns:
             Queryset with all requested eve objects
         """
         ids = set(map(int, ids))
-        enabled_sections = self.model.determine_effective_sections(enabled_sections)
-        enabled_sections_filter = self._enabled_sections_filter(enabled_sections)
+        effective_sections = self.model.determine_effective_sections(enabled_sections)
+        enabled_sections_filter = self._enabled_sections_filter(effective_sections)
         existing_ids = set(
             self.filter(id__in=ids)
             .filter(**enabled_sections_filter)
             .values_list("id", flat=True)
         )
         for id in ids.difference(existing_ids):
             self.update_or_create_esi(
                 id=int(id),
                 include_children=include_children,
                 wait_for_children=wait_for_children,
-                enabled_sections=enabled_sections,
+                enabled_sections=effective_sections,
                 task_priority=task_priority,
             )
 
         return self.filter(id__in=ids)
 
 
 class EvePlanetManager(EveUniverseEntityModelManager):
-    def _fetch_from_esi(self, id: int, enabled_sections: Iterable[str] = None) -> dict:
+    def _fetch_from_esi(
+        self, id: int, enabled_sections: Optional[Iterable[str]] = None
+    ) -> dict:
         from .models import EveSolarSystem
 
         esi_data = super()._fetch_from_esi(id=id)
         # no need to proceed if all children have been disabled
         if not self.model._children(enabled_sections):
             return esi_data
 
@@ -537,15 +542,17 @@
 
 
 class EvePlanetChildrenManager(EveUniverseEntityModelManager):
     def __init__(self) -> None:
         super().__init__()
         self._my_property_name = None
 
-    def _fetch_from_esi(self, id: int, enabled_sections: Iterable[str] = None) -> dict:
+    def _fetch_from_esi(
+        self, id: int, enabled_sections: Optional[Iterable[str]] = None
+    ) -> dict:
         from .models import EveSolarSystem
 
         if not self._my_property_name:
             raise RuntimeWarning("my_property_name not initialized")
 
         esi_data = super()._fetch_from_esi(id=id)
         if "system_id" not in esi_data:
@@ -588,17 +595,17 @@
 
     def update_or_create_esi(
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
-        enabled_sections: Iterable[str] = None,
-        task_priority: int = None,
-    ) -> Tuple[models.Model, bool]:
+        enabled_sections: Optional[Iterable[str]] = None,
+        task_priority: Optional[int] = None,
+    ) -> Tuple[ModelType, bool]:
         """updates or creates an EveStargate object by fetching it from ESI (blocking).
         Will always get/create parent objects
 
         Args:
             id: Eve Online ID of object
             include_children: (no effect)
             wait_for_children: (no effect)
@@ -628,19 +635,19 @@
 class EveStationManager(EveUniverseEntityModelManager):
     """For special handling of station services"""
 
     def _update_or_create_inline_objects(
         self,
         *,
         parent_eve_data_obj: dict,
-        parent_obj: models.Model,
+        parent_obj,
         inline_objects: dict,
         wait_for_children: bool,
         enabled_sections: Iterable[str],
-        task_priority: int = None,
+        task_priority: Optional[int] = None,
     ) -> None:
         """updates_or_creates station service objects for EveStations"""
         from .models import EveStationService
 
         if "services" in parent_eve_data_obj:
             services = list()
             for service_name in parent_eve_data_obj["services"]:
@@ -654,17 +661,17 @@
 class EveTypeManager(EveUniverseEntityModelManager):
     def update_or_create_esi(
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
-        enabled_sections: Iterable[str] = None,
-        task_priority: int = None,
-    ) -> Tuple[models.Model, bool]:
+        enabled_sections: Optional[Iterable[str]] = None,
+        task_priority: Optional[int] = None,
+    ) -> Tuple[ModelType, bool]:
         obj, created = super().update_or_create_esi(
             id=id,
             include_children=include_children,
             wait_for_children=wait_for_children,
             enabled_sections=enabled_sections,
             task_priority=task_priority,
         )
@@ -703,17 +710,17 @@
 
     def get_or_create_esi(
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
-        enabled_sections: Iterable[str] = None,
-        task_priority: int = None,
-    ) -> Tuple[models.Model, bool]:
+        enabled_sections: Optional[Iterable[str]] = None,
+        task_priority: Optional[int] = None,
+    ) -> Tuple[ModelType, bool]:
         """gets or creates an EvEntity object.
 
         The object is automatically fetched from ESI if it does not exist (blocking)
         or if it has not yet been resolved.
 
         Args:
             id: Eve Online ID of object
@@ -737,17 +744,17 @@
 
     def update_or_create_esi(
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
-        enabled_sections: Iterable[str] = None,
-        task_priority: int = None,
-    ) -> Tuple[Optional[models.Model], bool]:
+        enabled_sections: Optional[Iterable[str]] = None,
+        task_priority: Optional[int] = None,
+    ) -> Tuple[ModelType, bool]:
         """Update or create an EveEntity object by fetching it from ESI (blocking).
 
         Args:
             id: Eve Online ID of object
             include_children: (no effect)
             wait_for_children: (no effect)
 
@@ -796,42 +803,42 @@
             objects,
             batch_size=EVEUNIVERSE_BULK_METHODS_BATCH_SIZE,
             ignore_conflicts=True,
         )
         to_update_qs = self.filter(id__in=new_ids) | self.filter(
             id__in=ids.difference(new_ids), name=""
         )
-        return to_update_qs.update_from_esi()
+        return to_update_qs.update_from_esi()  # type: ignore
 
     def update_or_create_all_esi(
         self,
         *,
         include_children: bool = False,
         wait_for_children: bool = True,
-        enabled_sections: Iterable[str] = None,
-        task_priority: int = None,
+        enabled_sections: Optional[Iterable[str]] = None,
+        task_priority: Optional[int] = None,
     ) -> None:
         """not implemented - do not use"""
         raise NotImplementedError()
 
     def bulk_update_new_esi(self) -> int:
         """updates all unresolved EveEntity objects in the database from ESI.
 
         Returns:
             Count of updated entities.
         """
-        return self.filter(name="").update_from_esi()
+        return self.filter(name="").update_from_esi()  # type: ignore
 
     def bulk_update_all_esi(self):
         """Updates all EveEntity objects in the database from ESI.
 
         Returns:
             Count of updated entities.
         """
-        return self.all().update_from_esi()
+        return self.all().update_from_esi()  # type: ignore
 
     def resolve_name(self, id: int) -> str:
         """Return the name for the given Eve entity ID
         or an empty string if ID is not valid.
         """
         if id is not None:
             obj, _ = self.get_or_create_esi(id=int(id))
@@ -964,27 +971,30 @@
                     )
                 except IntegrityError:
                     pass
         return resolved_counter
 
 
 class EveMarketPriceManager(models.Manager):
-    def update_from_esi(self, minutes_until_stale: int = None) -> int:
+    def update_from_esi(self, minutes_until_stale: Optional[int] = None) -> int:
         """Updates market prices from ESI. Will only create new price objects for EveTypes that already exist in the database.
 
         Args:
             minutes_until_stale: only prices older then given minutes are regarding as stale and will be updated. Will use default (60) if not specified.
 
         Returns:
             Count of updated types
         """
         from .models import EveType
 
-        if minutes_until_stale is None:
-            minutes_until_stale = self.model.DEFAULT_MINUTES_UNTIL_STALE
+        minutes_until_stale = (
+            self.model.DEFAULT_MINUTES_UNTIL_STALE
+            if minutes_until_stale is None
+            else minutes_until_stale
+        )
 
         logger.info("Fetching market prices from ESI...")
         entries = esi.client.Market.get_markets_prices().results()
         if not entries:
             return 0
 
         entries_2 = {int(x["type_id"]): x for x in entries if "type_id" in x}
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/models.py` & `django_eveuniverse-1.0.0a3/eveuniverse/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,37 +121,37 @@
                 cls,
                 EveUniverseEntityModel,
                 EveUniverseInlineModel,
             ):
                 mappings.append(
                     {
                         "model": ModelClass,
-                        "load_order": ModelClass._eve_universe_meta_attr(
-                            "load_order", is_mandatory=True
+                        "load_order": ModelClass._eve_universe_meta_attr_strict(
+                            "load_order"
                         ),
                     }
                 )
 
         return [y["model"] for y in sorted(mappings, key=lambda x: x["load_order"])]
 
     @classmethod
-    def get_model_class(cls, model_name: str) -> models.Model:
+    def get_model_class(cls, model_name: str):
         """returns the model class for the given name"""
         classes = {
             x[0]: x[1]
             for x in inspect.getmembers(sys.modules[__name__], inspect.isclass)
             if issubclass(x[1], (EveUniverseBaseModel, EveUniverseInlineModel))
         }
         try:
             return classes[model_name]
         except KeyError:
             raise ValueError("Unknown model_name: %s" % model_name) from None
 
     @classmethod
-    def _esi_mapping(cls, enabled_sections: Set[str] = None) -> dict:
+    def _esi_mapping(cls, enabled_sections: Optional[Set[str]] = None) -> dict:
         field_mappings = cls._eve_universe_meta_attr("field_mappings")
         functional_pk = cls._eve_universe_meta_attr("functional_pk")
         parent_fk = cls._eve_universe_meta_attr("parent_fk")
         dont_create_related = cls._eve_universe_meta_attr("dont_create_related")
         disabled_fields = cls._disabled_fields(enabled_sections)
         mapping = dict()
         for field in [
@@ -165,15 +165,15 @@
             if field_mappings and field.name in field_mappings:
                 esi_name = field_mappings[field.name]
             else:
                 esi_name = field.name
 
             if field.primary_key is True:
                 is_pk = True
-                esi_name = cls._esi_pk()
+                esi_name = cls._esi_pk()  # FIXME: This might fail
             elif functional_pk and field.name in functional_pk:
                 is_pk = True
             else:
                 is_pk = False
 
             if parent_fk and is_pk and field.name in parent_fk:
                 is_parent_fk = True
@@ -202,25 +202,34 @@
                 is_charfield=isinstance(field, (models.CharField, models.TextField)),
                 create_related=create_related,
             )
 
         return mapping
 
     @classmethod
-    def _disabled_fields(cls, enabled_sections: Set[str] = None) -> set:
-        """returns name of fields that must not be loaded from ESI"""
-        return {}
+    def _disabled_fields(cls, enabled_sections: Optional[Set[str]] = None) -> set:
+        """Return name of fields that must not be loaded from ESI."""
+        return set()
 
     @classmethod
-    def _eve_universe_meta_attr(
+    def _eve_universe_meta_attr(cls, attr_name: str) -> Optional[Any]:
+        """Return value of an attribute from EveUniverseMeta or None"""
+        return cls._eve_universe_meta_attr_flexible(attr_name, is_mandatory=False)
+
+    @classmethod
+    def _eve_universe_meta_attr_strict(cls, attr_name: str) -> Any:
+        """Return value of an attribute from EveUniverseMeta or raise exception."""
+        return cls._eve_universe_meta_attr_flexible(attr_name, is_mandatory=True)
+
+    @classmethod
+    def _eve_universe_meta_attr_flexible(
         cls, attr_name: str, is_mandatory: bool = False
     ) -> Optional[Any]:
-        """returns value of an attribute from EveUniverseMeta or None"""
         try:
-            value = getattr(cls.EveUniverseMeta, attr_name)
+            value = getattr(cls.EveUniverseMeta, attr_name)  # type: ignore
         except AttributeError:
             value = None
             if is_mandatory:
                 raise ValueError(
                     "Mandatory attribute EveUniverseMeta.%s not defined "
                     "for class %s" % (attr_name, cls.__name__)
                 ) from None
@@ -263,15 +272,15 @@
         abstract = True
 
     def __str__(self) -> str:
         return self.name
 
     @staticmethod
     def determine_effective_sections(
-        enabled_sections: Iterable[str] = None,
+        enabled_sections: Optional[Iterable[str]] = None,
     ) -> Set[str]:
         """Determine currently effective sections."""
         enabled_sections = set(enabled_sections) if enabled_sections else set()
         if EVEUNIVERSE_LOAD_ASTEROID_BELTS:
             enabled_sections.add(EvePlanet.Section.ASTEROID_BELTS.value)
         if EVEUNIVERSE_LOAD_DOGMAS:
             enabled_sections.add(EveType.Section.DOGMAS.value)
@@ -299,53 +308,57 @@
         else and empty string
         """
         return ""
 
     @classmethod
     def _esi_pk(cls) -> str:
         """returns the name of the pk column on ESI that must exist"""
-        return cls._eve_universe_meta_attr("esi_pk", is_mandatory=True)
+        return cls._eve_universe_meta_attr_strict("esi_pk")
 
     @classmethod
-    def _has_esi_path_list(cls) -> str:
+    def _has_esi_path_list(cls) -> bool:
         return bool(cls._eve_universe_meta_attr("esi_path_list"))
 
     @classmethod
-    def _esi_path_list(cls) -> str:
+    def _esi_path_list(cls) -> Tuple[str, str]:
         return cls._esi_path("list")
 
     @classmethod
-    def _esi_path_object(cls) -> str:
+    def _esi_path_object(cls) -> Tuple[str, str]:
         return cls._esi_path("object")
 
     @classmethod
     def _esi_path(cls, variant: str) -> Tuple[str, str]:
         attr_name = f"esi_path_{str(variant)}"
-        path = cls._eve_universe_meta_attr(attr_name, is_mandatory=True)
+        path = cls._eve_universe_meta_attr_strict(attr_name)
         if len(path.split(".")) != 2:
             raise ValueError(f"{attr_name} not valid")
         return path.split(".")
 
     @classmethod
-    def _children(cls, enabled_sections: Iterable[str] = None) -> dict:
+    def _children(cls, enabled_sections: Optional[Iterable[str]] = None) -> dict:
         """returns the mapping of children for this class"""
         mappings = cls._eve_universe_meta_attr("children")
         return mappings if mappings else dict()
 
     @classmethod
-    def _inline_objects(cls, enabled_sections: Set[str] = None) -> dict:
+    def _inline_objects(cls, enabled_sections: Optional[Set[str]] = None) -> dict:
         """returns a dict of inline objects if any"""
         inline_objects = cls._eve_universe_meta_attr("inline_objects")
         return inline_objects if inline_objects else dict()
 
     @classmethod
     def _is_list_only_endpoint(cls) -> bool:
         esi_path_list = cls._eve_universe_meta_attr("esi_path_list")
         esi_path_object = cls._eve_universe_meta_attr("esi_path_object")
-        return esi_path_list and esi_path_object and esi_path_list == esi_path_object
+        return (
+            bool(esi_path_list)
+            and bool(esi_path_object)
+            and esi_path_list == esi_path_object
+        )
 
 
 class EveUniverseInlineModel(EveUniverseBaseModel):
     """Base class for Eve Universe Inline models
 
     Inline models are objects which do not have a dedicated ESI endpoint and are
     provided through the endpoint of another entity
@@ -528,15 +541,15 @@
 
     def update_from_esi(self) -> "EveEntity":
         """Update the current object from ESI
 
         Returns:
             itself after update
         """
-        obj, _ = EveEntity.objects.update_or_create_esi(id=self.id)
+        obj = EveEntity.objects.update_or_create_esi(id=self.id)[0]
         return obj
 
     def icon_url(self, size: int = EveUniverseEntityModel.DEFAULT_ICON_SIZE) -> str:
         """Create image URL for related EVE icon
 
         Args:
             size: size of image file in pixels, allowed values: 32, 64, 128, 256, 512
@@ -1037,15 +1050,15 @@
         null=True, default=None, blank=True, help_text="z position in the solar system"
     )
     enabled_sections = BitField(
         flags=tuple(Section.values()),
         help_text=(
             "Flags for loadable sections. True if instance was loaded with section."
         ),  # no index, because MySQL does not support it for bitwise operations
-    )
+    )  # type: ignore
 
     objects = EvePlanetManager()
 
     class EveUniverseMeta:
         esi_pk = "planet_id"
         esi_path_object = "Universe.get_universe_planets_planet_id"
         field_mappings = {
@@ -1055,15 +1068,15 @@
             "position_y": ("position", "y"),
             "position_z": ("position", "z"),
         }
         children = {"moons": "EveMoon", "asteroid_belts": "EveAsteroidBelt"}
         load_order = 205
 
     @classmethod
-    def _children(cls, enabled_sections: Iterable[str] = None) -> dict:
+    def _children(cls, enabled_sections: Optional[Iterable[str]] = None) -> dict:
         enabled_sections = cls.determine_effective_sections(enabled_sections)
         children = dict()
         if cls.Section.ASTEROID_BELTS in enabled_sections:
             children["asteroid_belts"] = "EveAsteroidBelt"
         if cls.Section.MOONS in enabled_sections:
             children["moons"] = "EveMoon"
         return children
@@ -1136,15 +1149,15 @@
     )
     security_status = models.FloatField()
     enabled_sections = BitField(
         flags=tuple(Section.values()),
         help_text=(
             "Flags for loadable sections. True if instance was loaded with section."
         ),  # no index, because MySQL does not support it for bitwise operations
-    )
+    )  # type: ignore
 
     class EveUniverseMeta:
         esi_pk = "system_id"
         esi_path_list = "Universe.get_universe_systems"
         esi_path_object = "Universe.get_universe_systems_system_id"
         field_mappings = {
             "eve_constellation": "constellation_id",
@@ -1195,42 +1208,49 @@
 
         Args:
             destination: Other solar system to use in calculation
 
         Returns:
             Distance in meters or None if one of the systems is in WH space
         """
+        if not self.position_x or not self.position_y or not self.position_z:
+            return None
+        if (
+            not destination
+            or not destination.position_x
+            or not destination.position_y
+            or not destination.position_z
+        ):
+            return None
         if self.is_w_space or destination.is_w_space:
             return None
-        else:
-            return math.sqrt(
-                (destination.position_x - self.position_x) ** 2
-                + (destination.position_y - self.position_y) ** 2
-                + (destination.position_z - self.position_z) ** 2
-            )
+        return math.sqrt(
+            (destination.position_x - self.position_x) ** 2
+            + (destination.position_y - self.position_y) ** 2
+            + (destination.position_z - self.position_z) ** 2
+        )
 
     def route_to(
         self, destination: "EveSolarSystem"
     ) -> Optional[List["EveSolarSystem"]]:
         """Calculates the shortest route between the current and the given solar system
 
         Args:
             destination: Other solar system to use in calculation
 
         Returns:
             List of solar system objects incl. origin and destination or None if no route can be found (e.g. if one system is in WH space)
         """
         path_ids = self._calc_route_esi(self.id, destination.id)
-        if path_ids is not None:
-            return [
-                EveSolarSystem.objects.get_or_create_esi(id=solar_system_id)
-                for solar_system_id in path_ids
-            ]
-        else:
+        if path_ids is None:
             return None
+        return [
+            EveSolarSystem.objects.get_or_create_esi(id=solar_system_id)
+            for solar_system_id in path_ids
+        ]
 
     def jumps_to(self, destination: "EveSolarSystem") -> Optional[int]:
         """Calculates the shortest route between the current and the given solar system
 
         Args:
             destination: Other solar system to use in calculation
 
@@ -1257,15 +1277,15 @@
             return esi.client.Routes.get_route_origin_destination(
                 origin=origin_id, destination=destination_id
             ).results()
         except HTTPNotFound:
             return None
 
     def nearest_celestial(
-        self, x: int, y: int, z: int, group_id: int = None
+        self, x: int, y: int, z: int, group_id: Optional[int] = None
     ) -> Optional[NearestCelestial]:
         """Determine nearest celestial to given coordinates as eveuniverse object.
 
         Args:
             x, y, z: Start point in space to look from
             group_id: Eve ID of group to filter results by
 
@@ -1295,38 +1315,37 @@
             return None
         obj, _ = MyClass.objects.get_or_create_esi(id=item.id)
         return self.NearestCelestial(
             eve_type=eve_type, eve_object=obj, distance=item.distance
         )
 
     @classmethod
-    def _children(cls, enabled_sections: Iterable[str] = None) -> dict:
+    def _children(cls, enabled_sections: Optional[Iterable[str]] = None) -> dict:
         enabled_sections = cls.determine_effective_sections(enabled_sections)
         children = dict()
         if cls.Section.PLANETS in enabled_sections:
             children["planets"] = "EvePlanet"
         if cls.Section.STARGATES in enabled_sections:
             children["stargates"] = "EveStargate"
         if cls.Section.STATIONS in enabled_sections:
             children["stations"] = "EveStation"
         return children
 
     @classmethod
-    def _disabled_fields(cls, enabled_sections: Set[str] = None) -> set:
+    def _disabled_fields(cls, enabled_sections: Optional[Set[str]] = None) -> set:
         enabled_sections = cls.determine_effective_sections(enabled_sections)
         if cls.Section.STARS not in enabled_sections:
             return {"eve_star"}
-        return {}
+        return set()
 
     @classmethod
-    def _inline_objects(cls, enabled_sections: Set[str] = None) -> dict:
-        if enabled_sections and cls.Section.PLANETS in enabled_sections:
-            return super()._inline_objects()
-        else:
+    def _inline_objects(cls, enabled_sections: Optional[Set[str]] = None) -> dict:
+        if not enabled_sections or cls.Section.PLANETS not in enabled_sections:
             return dict()
+        return super()._inline_objects()
 
 
 class EveStar(EveUniverseEntityModel):
     """A star in Eve Online"""
 
     age = models.BigIntegerField()
     eve_type = models.ForeignKey(
@@ -1502,15 +1521,15 @@
     published = models.BooleanField()
     volume = models.FloatField(default=None, null=True)
     enabled_sections = BitField(
         flags=tuple(Section.values()),
         help_text=(
             "Flags for loadable sections. True if instance was loaded with section."
         ),  # no index, because MySQL does not support it for bitwise operations
-    )
+    )  # type: ignore
 
     objects = EveTypeManager()
 
     class EveUniverseMeta:
         esi_pk = "type_id"
         esi_path_list = "Universe.get_universe_types"
         esi_path_object = "Universe.get_universe_types_type_id"
@@ -1544,17 +1563,17 @@
 
         SKIN = enum.auto()
         """SKIN"""
 
     def icon_url(
         self,
         size: int = EveUniverseEntityModel.DEFAULT_ICON_SIZE,
-        variant: IconVariant = None,
-        category_id: int = None,
-        is_blueprint: bool = None,
+        variant: Optional[IconVariant] = None,
+        category_id: Optional[int] = None,
+        is_blueprint: Optional[bool] = None,
     ) -> str:
         """returns an image URL to this type as icon. Also works for blueprints and SKINs.
 
         Will try to auto-detect the variant based on the types's category,
         unless `variant` or `category_id` is specified.
 
         Args:
@@ -1597,29 +1616,28 @@
         return eveimageserver.type_icon_url(self.id, size=size)
 
     def render_url(self, size=EveUniverseEntityModel.DEFAULT_ICON_SIZE) -> str:
         """return an image URL to this type as render"""
         return eveimageserver.type_render_url(self.id, size=size)
 
     @classmethod
-    def _disabled_fields(cls, enabled_sections: Set[str] = None) -> set:
+    def _disabled_fields(cls, enabled_sections: Optional[Set[str]] = None) -> set:
         enabled_sections = cls.determine_effective_sections(enabled_sections)
         disabled_fields = set()
         if cls.Section.GRAPHICS not in enabled_sections:
             disabled_fields.add("eve_graphic")
         if cls.Section.MARKET_GROUPS not in enabled_sections:
             disabled_fields.add("eve_market_group")
         return disabled_fields
 
     @classmethod
-    def _inline_objects(cls, enabled_sections: Set[str] = None) -> dict:
-        if enabled_sections and cls.Section.DOGMAS in enabled_sections:
-            return super()._inline_objects()
-        else:
+    def _inline_objects(cls, enabled_sections: Optional[Set[str]] = None) -> dict:
+        if not enabled_sections or cls.Section.DOGMAS not in enabled_sections:
             return dict()
+        return super()._inline_objects()
 
     @classmethod
     def eve_entity_category(cls) -> str:
         return EveEntity.CATEGORY_INVENTORY_TYPE
 
 
 class EveTypeDogmaAttribute(EveUniverseInlineModel):
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/swagger.json` & `django_eveuniverse-1.0.0a3/eveuniverse/swagger.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tasks.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Iterable, List
+from typing import Iterable, List, Optional
 
 from celery import shared_task
 from celery_once import QueueOnce as BaseQueueOnce
 from django.db.utils import OperationalError
 
 from . import __title__, models
 from .app_settings import EVEUNIVERSE_LOAD_TASKS_PRIORITY, EVEUNIVERSE_TASKS_TIME_LIMIT
@@ -46,41 +46,41 @@
     model_name: str, id: int, include_children=False, wait_for_children=True
 ) -> None:
     """Task for loading an eve object.
     Will only be created from ESI if it does not exist
     """
     logger.info("Loading %s with ID %s", model_name, id)
     ModelClass = EveUniverseEntityModel.get_model_class(model_name)
-    ModelClass.objects.get_or_create_esi(
+    ModelClass.objects.get_or_create_esi(  # type: ignore
         id=id, include_children=include_children, wait_for_children=wait_for_children
     )
 
 
 @shared_task(**TASK_ESI_DEFAULTS_ONCE)
 def update_or_create_eve_object(
     model_name: str,
     id: int,
     include_children=False,
     wait_for_children=True,
-    enabled_sections: List[str] = None,
-    task_priority: int = None,
+    enabled_sections: Optional[List[str]] = None,
+    task_priority: Optional[int] = None,
 ) -> None:
     """Update or create an eve object from ESI.
 
     Args:
         model_name: Name of the respective Django model, e.g. ``"EveType"``
         id: Eve Online ID of object
         include_children: if child objects should be updated/created as well (only when a new object is created)
         wait_for_children: when true child objects will be updated/created blocking (if any), else async (only when a new object is created)
         enabled_sections: Sections to load regardless of current settings, e.g. `[EveType.Section.DOGMAS]` will always load dogmas for EveTypes
         task_priority: priority of started tasks
     """
     logger.info("Updating/Creating %s with ID %s", model_name, id)
     ModelClass = EveUniverseEntityModel.get_model_class(model_name)
-    ModelClass.objects.update_or_create_esi(
+    ModelClass.objects.update_or_create_esi(  # type: ignore
         id=id,
         include_children=include_children,
         wait_for_children=wait_for_children,
         enabled_sections=enabled_sections,
         task_priority=task_priority,
     )
 
@@ -90,25 +90,25 @@
     parent_obj_id: int,
     parent_fk: str,
     eve_data_obj: dict,
     other_pk_info: dict,
     parent2_model_name: str,
     inline_model_name: str,
     parent_model_name: str,
-    enabled_sections: List[str] = None,
+    enabled_sections: Optional[List[str]] = None,
 ) -> None:
     """Task for updating or creating a single inline object from ESI"""
     logger.info(
         "Updating/Creating inline object %s for %s wit ID %s",
         inline_model_name,
         parent_model_name,
         parent_obj_id,
     )
     ModelClass = EveUniverseEntityModel.get_model_class(parent_model_name)
-    ModelClass.objects._update_or_create_inline_object(
+    ModelClass.objects._update_or_create_inline_object(  # type: ignore
         parent_obj_id=parent_obj_id,
         parent_fk=parent_fk,
         eve_data_obj=eve_data_obj,
         other_pk_info=other_pk_info,
         parent2_model_name=parent2_model_name,
         inline_model_name=inline_model_name,
         enabled_sections=enabled_sections,
@@ -126,31 +126,31 @@
 
 @shared_task(**TASK_ESI_DEFAULTS_ONCE)
 def update_unresolved_eve_entities() -> None:
     """Update all unresolved EveEntity objects from ESI.
 
     Will resolve entities in parallel to speed up resolving large sets.
     """
-    ids = list(EveEntity.objects.filter(name="").valid_ids())
+    ids = list(EveEntity.objects.filter(name="").valid_ids())  # type: ignore
     logger.info("Updating %d unresolved entities from ESI", len(ids))
     for chunk_ids in chunks(ids, POST_UNIVERSE_NAMES_MAX_ITEMS):
-        _update_unresolved_eve_entities_for_page.delay(chunk_ids)
+        _update_unresolved_eve_entities_for_page.delay(chunk_ids)  # type: ignore
 
 
 @shared_task(**TASK_ESI_DEFAULTS)
 def _update_unresolved_eve_entities_for_page(ids: Iterable[int]) -> None:
     """Update unresolved EveEntity objects for given ids from ESI."""
     EveEntity.objects.update_from_esi_by_id(ids)
 
 
 # Object loaders
 
 
 @shared_task(**TASK_ESI_DEFAULTS_ONCE)
-def load_map(enabled_sections: List[str] = None) -> None:
+def load_map(enabled_sections: Optional[List[str]] = None) -> None:
     """Load the complete Eve map with all regions, constellation and solar systems
     and additional related entities if they are enabled.
 
     Args:
         enabled_sections: Sections to load regardless of current settings
     """
     logger.info(
@@ -166,19 +166,19 @@
         update_or_create_eve_object.delay(
             model_name="EveRegion",
             id=id,
             include_children=True,
             wait_for_children=False,
             enabled_sections=enabled_sections,
             task_priority=EVEUNIVERSE_LOAD_TASKS_PRIORITY,
-        )
+        )  # type: ignore
 
 
 @shared_task(**TASK_ESI_DEFAULTS_ONCE)
-def load_all_types(enabled_sections: List[str] = None) -> None:
+def load_all_types(enabled_sections: Optional[List[str]] = None) -> None:
     """Load all eve types.
 
     Args:
         enabled_sections: Sections to load regardless of current settings
     """
     logger.info(
         "Loading all eve types from ESI including these sections: %s",
@@ -197,87 +197,87 @@
             category_id=category_id, enabled_sections=enabled_sections
         )
 
 
 def _load_category_with_children(
     category_id: int,
     force_loading_dogma: bool = False,
-    enabled_sections: List[str] = None,
+    enabled_sections: Optional[List[str]] = None,
 ) -> None:
     """Start loading a category async incl. all it's children from ESI."""
     enabled_sections = enabled_sections or []
     if force_loading_dogma:
         enabled_sections.append(EveType.Section.DOGMAS.value)
     update_or_create_eve_object.delay(
         model_name="EveCategory",
         id=category_id,
         include_children=True,
         wait_for_children=False,
         enabled_sections=enabled_sections,
         task_priority=EVEUNIVERSE_LOAD_TASKS_PRIORITY,
-    )
+    )  # type: ignore
 
 
 def _load_group_with_children(group_id: int, force_loading_dogma: bool = False) -> None:
     """Starts a task for loading a group incl. all it's children from ESI"""
     enabled_sections = [EveType.Section.DOGMAS.value] if force_loading_dogma else None
     update_or_create_eve_object.delay(
         model_name="EveGroup",
         id=group_id,
         include_children=True,
         wait_for_children=False,
         enabled_sections=enabled_sections,
         task_priority=EVEUNIVERSE_LOAD_TASKS_PRIORITY,
-    )
+    )  # type: ignore
 
 
 def _load_type_with_children(type_id: int, force_loading_dogma: bool = False) -> None:
     """Starts a task for loading a type incl. all it's children from ESI"""
     enabled_sections = [EveType.Section.DOGMAS.value] if force_loading_dogma else None
     update_or_create_eve_object.delay(
         model_name="EveType",
         id=type_id,
         include_children=False,
         wait_for_children=False,
         enabled_sections=enabled_sections,
         task_priority=EVEUNIVERSE_LOAD_TASKS_PRIORITY,
-    )
+    )  # type: ignore
 
 
 @shared_task(**TASK_ESI_DEFAULTS_ONCE)
-def load_ship_types(enabled_sections: List[str] = None) -> None:
+def load_ship_types(enabled_sections: Optional[List[str]] = None) -> None:
     """Load all ship types.
 
     Args:
         enabled_sections: Sections to load regardless of current settings
     """
     logger.info("Started loading all ship types into eveuniverse")
     _load_category_with_children(
         category_id=EveCategoryId.SHIP.value, enabled_sections=enabled_sections
     )
 
 
 @shared_task(**TASK_ESI_DEFAULTS_ONCE)
-def load_structure_types(enabled_sections: List[str] = None) -> None:
+def load_structure_types(enabled_sections: Optional[List[str]] = None) -> None:
     """Load all structure types.
 
     Args:
         enabled_sections: Sections to load regardless of current settings
     """
     logger.info("Started loading all structure types into eveuniverse")
     _load_category_with_children(
         category_id=EveCategoryId.STRUCTURE.value, enabled_sections=enabled_sections
     )
 
 
 @shared_task(**TASK_ESI_DEFAULTS_ONCE)
 def load_eve_types(
-    category_ids: List[int] = None,
-    group_ids: List[int] = None,
-    type_ids: List[int] = None,
+    category_ids: Optional[List[int]] = None,
+    group_ids: Optional[List[int]] = None,
+    type_ids: Optional[List[int]] = None,
     force_loading_dogma: bool = False,
 ) -> None:
     """Load specified eve types from ESI. Will always load all children except for EveType
 
     Args:
     - category_ids: EveCategory IDs
     - group_ids: EveGroup IDs
@@ -295,11 +295,11 @@
 
     if type_ids:
         for type_id in type_ids:
             _load_type_with_children(type_id, force_loading_dogma)
 
 
 @shared_task(**TASK_ESI_DEFAULTS_ONCE)
-def update_market_prices(minutes_until_stale: int = None):
+def update_market_prices(minutes_until_stale: Optional[int] = None):
     """Updates market prices from ESI.
     see EveMarketPrice.objects.update_from_esi() for details"""
     EveMarketPrice.objects.update_from_esi(minutes_until_stale)
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/utils.py` & `django_eveuniverse-1.0.0a3/eveuniverse/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import socket
+from typing import Any, Optional
 
 from django.conf import settings
 from django.test import TestCase
 
 # Format for output of datetime for this app
 DATETIME_FORMAT = "%Y-%m-%d %H:%M"
 
@@ -26,28 +27,28 @@
     """Yield successive sized chunks from lst."""
     for i in range(0, len(lst), size):
         yield lst[i : i + size]
 
 
 def clean_setting(
     name: str,
-    default_value: object,
-    min_value: int = None,
-    max_value: int = None,
-    required_type: type = None,
-    choices: list = None,
+    default_value: Any,
+    min_value: Optional[int] = None,
+    max_value: Optional[int] = None,
+    required_type: Optional[type] = None,
+    choices: Optional[list] = None,
 ):
     """cleans the input for a custom setting
 
     Will use `default_value` if settings does not exit or has the wrong type
     or is outside define boundaries (for int only)
 
     Need to define `required_type` if `default_value` is `None`
 
-    Will assume `min_value` of 0 for int (can be overriden)
+    Will assume `min_value` of 0 for int (can be overridden)
 
     Returns cleaned value for setting
     """
     if default_value is None and not required_type:
         raise ValueError("You must specify a required_type for None defaults")
 
     if not required_type:
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/core/dotlan.py` & `django_eveuniverse-1.0.0a3/eveuniverse/core/dotlan.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/core/eveimageserver.py` & `django_eveuniverse-1.0.0a3/eveuniverse/core/eveimageserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Fetching image URLs for Eve objects."""
 
 import enum
+from typing import Optional
 
 _EVE_IMAGE_SERVER_URL = "https://images.evetech.net"
 _DEFAULT_IMAGE_SIZE = 32
 
 
 class EsiCategory(enum.Enum):
     """Enum class for ESI categories"""
@@ -30,19 +31,19 @@
 class EsiTenant(enum.Enum):
     """Enum class for ESI tenants"""
 
     TRANQUILITY = "tranquility"
 
 
 def _eve_entity_image_url(
-    category: str,
+    category: EsiCategory,
     entity_id: int,
     size: int = 32,
-    variant: ImageVariant = None,
-    tenant: EsiTenant = None,
+    variant: Optional[ImageVariant] = None,
+    tenant: Optional[EsiTenant] = None,
 ) -> str:
     """returns image URL for an Eve Online ID.
     Supported categories: alliance, corporation, character, inventory_type
 
     Arguments:
     - category: category of the ID, see ESI category constants
     - entity_id: Eve ID of the entity
@@ -99,23 +100,24 @@
         endpoint = categories[category]["endpoint"]
 
     if variant:
         if variant not in categories[category]["variants"]:
             raise ValueError(
                 "Invalid variant {} for category {}".format(variant, category)
             )
+        my_variant = variant
     else:
-        variant = categories[category]["variants"][0]
+        my_variant = categories[category]["variants"][0]
 
     if tenant and type(tenant) is not EsiTenant:
         raise ValueError("Invalid tenant {}".format(tenant))
 
     # compose result URL
     result = "{}/{}/{}/{}?size={}".format(
-        _EVE_IMAGE_SERVER_URL, endpoint, entity_id, variant.value, size
+        _EVE_IMAGE_SERVER_URL, endpoint, entity_id, my_variant.value, size
     )
     if tenant:
         result += "&tenant={}".format(tenant.value)
 
     return result
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/core/evemicros.py` & `django_eveuniverse-1.0.0a3/eveuniverse/core/evemicros.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     id: int
     name: str
     type_id: int
     distance: float
 
 
 def nearest_celestial(
-    solar_system_id: int, x: int, y: int, z: int, group_id: int = None
+    solar_system_id: int, x: int, y: int, z: int, group_id: Optional[int] = None
 ) -> Optional[EveItem]:
     """Fetch nearest celestial to given coordinates from API. Results are cached.
 
     Args:
         solar_system_id: Eve ID of solar system
         x, y, z: Start point in space to look from
         group_id: Eve ID of group to filter results by
@@ -64,15 +64,15 @@
         if "ok" not in data or not data["ok"] or "result" not in data:
             return None
         result = data["result"]
         cache.set(key=cache_key, value=result, timeout=_CACHE_TIMEOUT)
     return result
 
 
-def _get_item_from_result(result, group_id) -> Optional[dict]:
+def _get_item_from_result(result, group_id) -> Optional[EveItem]:
     """Tries to find item in result. Returns None if item can not be found."""
     if not result:
         return None
     if not group_id:
         return _create_item(result[0])
     for item in result:
         if item["groupID"] == group_id:
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/core/evesdeapi.py` & `django_eveuniverse-1.0.0a3/eveuniverse/core/evesdeapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             name=str(record["name"]),
             type_id=int(record["type_id"]),
             distance=float(record["distance"]),
         )
 
 
 def nearest_celestial(
-    solar_system_id: float, x: float, y: float, z: float, group_id: int = None
+    solar_system_id: float, x: float, y: float, z: float, group_id: Optional[int] = None
 ) -> Optional[EveItem]:
     """Fetch nearest celestial to given coordinates from API. Results are cached.
 
     Args:
         solar_system_id: Eve ID of solar system
         x, y, z: Start point in space to look from
         group_id: Eve ID of group to filter results by
@@ -56,15 +56,15 @@
     )
     if not result:
         return None
     return EveItem.from_dict(result[0])
 
 
 def _fetch_items_from_endpoint_cached(
-    solar_system_id: float, x: float, y: float, z: float, group_id: int = None
+    solar_system_id: float, x: float, y: float, z: float, group_id: Optional[int] = None
 ) -> Optional[dict]:
     """Fetch items from endpoint with caching.
 
     Returns None if data from API does not have expected structure.
     """
     params = {"x": x, "y": y, "z": z}
     if group_id is not None:
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/core/evewho.py` & `django_eveuniverse-1.0.0a3/eveuniverse/core/evewho.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     CHARACTER = auto()
     CORPORAITON = auto()
 
 
 _BASE_URL = "https://evewho.com"
 
 
-def _build_url(category: str, eve_id: int) -> str:
+def _build_url(category: _Category, eve_id: int) -> str:
     """URL to profile page for an eve entity."""
 
     partials = {
         _Category.ALLIANCE: "alliance",
         _Category.CHARACTER: "character",
         _Category.CORPORAITON: "corporation",
     }
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/core/evexml.py` & `django_eveuniverse-1.0.0a3/eveuniverse/core/evexml.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/core/zkillboard.py` & `django_eveuniverse-1.0.0a3/eveuniverse/core/zkillboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     REGION = auto()
     SOLARSYSTEM = auto()
 
 
 _BASE_URL = "https://zkillboard.com"
 
 
-def _build_url(category: str, eve_id: int) -> str:
+def _build_url(category: _Category, eve_id: int) -> str:
     """URL to profile page for an eve entity."""
     partials = {
         _Category.ALLIANCE: "alliance",
         _Category.CHARACTER: "character",
         _Category.CORPORATION: "corporation",
         _Category.KILLMAIL: "kill",
         _Category.REGION: "region",
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/management/commands/eveuniverse_load_data.py` & `django_eveuniverse-1.0.0a3/eveuniverse/management/commands/eveuniverse_load_data.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/management/commands/eveuniverse_load_types.py` & `django_eveuniverse-1.0.0a3/eveuniverse/management/commands/eveuniverse_load_types.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/management/commands/eveuniverse_purge_data.py` & `django_eveuniverse-1.0.0a3/eveuniverse/management/commands/eveuniverse_purge_data.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/migrations/0001_initial.py` & `django_eveuniverse-1.0.0a3/eveuniverse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/migrations/0002_load_eveunit.py` & `django_eveuniverse-1.0.0a3/eveuniverse/migrations/0002_load_eveunit.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/migrations/0003_evemarketprice.py` & `django_eveuniverse-1.0.0a3/eveuniverse/migrations/0003_evemarketprice.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/migrations/0005_type_materials_and_sections.py` & `django_eveuniverse-1.0.0a3/eveuniverse/migrations/0005_type_materials_and_sections.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/migrations/eve_unit.json` & `django_eveuniverse-1.0.0a3/eveuniverse/migrations/eve_unit.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/static/eveuniverse/skin_generic_128.png` & `django_eveuniverse-1.0.0a3/eveuniverse/static/eveuniverse/skin_generic_128.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/static/eveuniverse/skin_generic_32.png` & `django_eveuniverse-1.0.0a3/eveuniverse/static/eveuniverse/skin_generic_32.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/static/eveuniverse/skin_generic_64.png` & `django_eveuniverse-1.0.0a3/eveuniverse/static/eveuniverse/skin_generic_64.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/pilot.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/pilot.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_backends.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_commands.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_core.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 
 import requests_mock
 from bravado.exception import HTTPInternalServerError
 from django.core.cache import cache
 from django.test import TestCase
 from requests.exceptions import HTTPError
 
-from ..constants import EveGroupId
-from ..core import (
+from eveuniverse.constants import EveGroupId
+from eveuniverse.core import (
     dotlan,
     esitools,
     eveimageserver,
     eveitems,
     evemicros,
     evesdeapi,
     eveskinserver,
     evewho,
     evexml,
     zkillboard,
 )
-from ..models import EveEntity
-from ..utils import NoSocketsTestCase
+from eveuniverse.models import EveEntity
+from eveuniverse.utils import NoSocketsTestCase
+
 from .testdata.esi import EsiClientStub
 from .testdata.factories import (
     create_eve_entity,
     create_evemicros_response,
     create_evesdeapi_response,
 )
 
@@ -112,27 +113,37 @@
         self.assertEqual(
             eveimageserver._eve_entity_image_url(
                 eveimageserver.EsiCategory.CHARACTER, 42, size=1024
             ),
             "https://images.evetech.net/characters/42/portrait?size=1024",
         )
         with self.assertRaises(ValueError):
-            eveimageserver._eve_entity_image_url("corporation", 42, size=-5)
+            eveimageserver._eve_entity_image_url(
+                eveimageserver.EsiCategory.CORPORATION, 42, size=-5
+            )
 
         with self.assertRaises(ValueError):
-            eveimageserver._eve_entity_image_url("corporation", 42, size=0)
+            eveimageserver._eve_entity_image_url(
+                eveimageserver.EsiCategory.CORPORATION, 42, size=0
+            )
 
         with self.assertRaises(ValueError):
-            eveimageserver._eve_entity_image_url("corporation", 42, size=31)
+            eveimageserver._eve_entity_image_url(
+                eveimageserver.EsiCategory.CORPORATION, 42, size=31
+            )
 
         with self.assertRaises(ValueError):
-            eveimageserver._eve_entity_image_url("corporation", 42, size=1025)
+            eveimageserver._eve_entity_image_url(
+                eveimageserver.EsiCategory.CORPORATION, 42, size=1025
+            )
 
         with self.assertRaises(ValueError):
-            eveimageserver._eve_entity_image_url("corporation", 42, size=2048)
+            eveimageserver._eve_entity_image_url(
+                eveimageserver.EsiCategory.CORPORATION, 42, size=2048
+            )
 
     def test_variant(self):
         self.assertEqual(
             eveimageserver._eve_entity_image_url(
                 eveimageserver.EsiCategory.CHARACTER,
                 42,
                 variant=eveimageserver.ImageVariant.PORTRAIT,
@@ -170,28 +181,28 @@
         self.assertEqual(
             eveimageserver._eve_entity_image_url(
                 eveimageserver.EsiCategory.CHARACTER, 42
             ),
             "https://images.evetech.net/characters/42/portrait?size=32",
         )
         with self.assertRaises(ValueError):
-            eveimageserver._eve_entity_image_url("invalid", 42)
+            eveimageserver._eve_entity_image_url("invalid", 42)  # type: ignore
 
     def test_tenants(self):
         self.assertEqual(
             eveimageserver._eve_entity_image_url(
                 eveimageserver.EsiCategory.CHARACTER,
                 42,
                 tenant=eveimageserver.EsiTenant.TRANQUILITY,
             ),
             "https://images.evetech.net/characters/42/portrait?size=32&tenant=tranquility",
         )
         with self.assertRaises(ValueError):
             eveimageserver._eve_entity_image_url(
-                eveimageserver.EsiCategory.CHARACTER, 42, tenant="xxx"
+                eveimageserver.EsiCategory.CHARACTER, 42, tenant="xxx"  # type: ignore
             )
 
     def test_alliance_logo_url(self):
         expected = "https://images.evetech.net/alliances/42/logo?size=128"
         self.assertEqual(eveimageserver.alliance_logo_url(42, 128), expected)
 
     def test_corporation_logo_url(self):
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_1.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/test_models_1.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     def test_eve_universe_meta_attr_2(self):
         """When not defined, then return None"""
         self.assertIsNone(EveType._eve_universe_meta_attr("undefined_param"))
 
     def test_eve_universe_meta_attr_3(self):
         """When not defined and is_mandatory, then raise exception"""
         with self.assertRaises(ValueError):
-            EveType._eve_universe_meta_attr("undefined_param", is_mandatory=True)
+            EveType._eve_universe_meta_attr_strict("undefined_param")
 
     def test_eve_universe_meta_attr_4(self):
         """When EveUniverseMeta class not defined, then return None"""
         self.assertIsNone(
             EveUniverseBaseModel._eve_universe_meta_attr("undefined_param")
         )
 
@@ -886,21 +886,14 @@
             id=30045339, include_children=True
         )
         self.assertTrue(created)
         self.assertEqual(obj.id, 30045339)
 
         self.assertTrue(EveStation.objects.filter(id=60015068).exists())
 
-    def test_distance_to(self, mock_esi):
-        mock_esi.client = EsiClientStub()
-
-        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
-        akidagi, _ = EveSolarSystem.objects.get_or_create_esi(id=30045342)
-        self.assertEqual(meters_to_ly(enaluri.distance_to(akidagi)), 1.947802326920925)
-
     def test_can_identify_highsec_system(self, mock_esi):
         mock_esi.client = EsiClientStub()
 
         jita, _ = EveSolarSystem.objects.get_or_create_esi(id=30000142)
         self.assertTrue(jita.is_high_sec)
         self.assertFalse(jita.is_low_sec)
         self.assertFalse(jita.is_null_sec)
@@ -929,23 +922,113 @@
 
         thera, _ = EveSolarSystem.objects.get_or_create_esi(id=31000005)
         self.assertTrue(thera.is_w_space)
         self.assertFalse(thera.is_null_sec)
         self.assertFalse(thera.is_low_sec)
         self.assertFalse(thera.is_high_sec)
 
+    """
+    @patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_STARGATES", True)
+    @patch(MODELS_PATH + ".cache")
+    def test_can_calculate_route(self, mock_cache, mock_esi):
+        def my_get_or_set(key, func, timeout):
+            return func()
+
+        mock_esi.client = EsiClientStub()
+        mock_cache.get.return_value = None
+        mock_cache.get_or_set.side_effect = my_get_or_set
+
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(
+            id=30045339, include_children=True
+        )
+        akidagi, _ = EveSolarSystem.objects.get_or_create_esi(
+            id=30045342, include_children=True
+        )
+        self.assertEqual(enaluri.jumps_to(akidagi), 1)
+    """
+
+
+@patch(MANAGERS_PATH + ".esi")
+class TestEveSolarSystemDistanceTo(NoSocketsTestCase):
+    def test_should_calculate_distance_between_normal_systems(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        akidagi, _ = EveSolarSystem.objects.get_or_create_esi(id=30045342)
+        # when
+        result = enaluri.distance_to(akidagi)
+        # then
+        self.assertEqual(meters_to_ly(result), 1.947802326920925)
+
+    def test_should_return_none_when_one_system_in_wh_space_1(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        thera, _ = EveSolarSystem.objects.get_or_create_esi(id=31000005)
+        # when
+        result = enaluri.distance_to(thera)
+        # then
+        self.assertIsNone(result)
+
+    def test_should_return_none_when_one_system_in_wh_space_2(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        thera, _ = EveSolarSystem.objects.get_or_create_esi(id=31000005)
+        # when
+        result = thera.distance_to(enaluri)
+        # then
+        self.assertIsNone(result)
+
+    def test_should_return_none_when_no_destination(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        # when
+        result = enaluri.distance_to(None)
+        # then
+        self.assertIsNone(result)
+
+    def test_should_return_none_when_origin_has_not_coordinates(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        enaluri.position_x = None
+        enaluri.position_y = None
+        enaluri.position_z = None
+        akidagi, _ = EveSolarSystem.objects.get_or_create_esi(id=30045342)
+        # when
+        result = enaluri.distance_to(akidagi)
+        # then
+        self.assertIsNone(result)
+
+    def test_should_return_none_when_destination_has_not_coordinates(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        enaluri.position_x = None
+        enaluri.position_y = None
+        enaluri.position_z = None
+        akidagi, _ = EveSolarSystem.objects.get_or_create_esi(id=30045342)
+        # when
+        result = akidagi.distance_to(enaluri)
+        # then
+        self.assertIsNone(result)
+
+
+@patch(MANAGERS_PATH + ".esi")
+class TestEveSolarSystemJumpsTo(NoSocketsTestCase):
     @staticmethod
-    def esi_get_route_origin_destination(origin, destination, **kwargs) -> list:
+    def esi_get_route_origin_destination(origin, destination, **kwargs):
         routes = {
             30045339: {30045342: [30045339, 30045342]},
         }
         if origin in routes and destination in routes[origin]:
             return BravadoOperationStub(routes[origin][destination])
-        else:
-            raise HTTPNotFound(Mock(**{"response.status_code": 404}))
+        raise HTTPNotFound(Mock(**{"response.status_code": 404}))
 
     @patch("eveuniverse.models.esi")
     def test_can_calculate_jumps(self, mock_esi_2, mock_esi):
         mock_esi.client = EsiClientStub()
         mock_esi_2.client.Routes.get_route_origin_destination.side_effect = (
             self.esi_get_route_origin_destination
         )
@@ -961,33 +1044,47 @@
             self.esi_get_route_origin_destination
         )
 
         enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
         jita, _ = EveSolarSystem.objects.get_or_create_esi(id=30000142)
         self.assertIsNone(enaluri.jumps_to(jita))
 
-    """
-    @patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_STARGATES", True)
-    @patch(MODELS_PATH + ".cache")
-    def test_can_calculate_route(self, mock_cache, mock_esi):
-        def my_get_or_set(key, func, timeout):
-            return func()
 
+@patch(MODELS_PATH + ".EveSolarSystem._calc_route_esi")
+@patch(MANAGERS_PATH + ".esi")
+class TestEveSolarSystemRouteTo(NoSocketsTestCase):
+    def test_should_return_valid_route(self, mock_esi, mock_calc_route_esi):
+        # given
         mock_esi.client = EsiClientStub()
-        mock_cache.get.return_value = None
-        mock_cache.get_or_set.side_effect = my_get_or_set
+        mock_calc_route_esi.return_value = [30045339, 30045342]
+        enaluri: EveSolarSystem = EveSolarSystem.objects.get_or_create_esi(id=30045339)[
+            0
+        ]
+        akidagi: EveSolarSystem = EveSolarSystem.objects.get_or_create_esi(id=30045342)[
+            0
+        ]
+        # when
+        result = enaluri.route_to(akidagi)
+        # then
+        self.assertListEqual(result, [(enaluri, False), (akidagi, False)])
 
-        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(
-            id=30045339, include_children=True
-        )
-        akidagi, _ = EveSolarSystem.objects.get_or_create_esi(
-            id=30045342, include_children=True
-        )
-        self.assertEqual(enaluri.jumps_to(akidagi), 1)
-    """
+    def test_should_return_none_when_no_route_found(
+        self, mock_esi, mock_calc_route_esi
+    ):
+        # given
+        mock_esi.client = EsiClientStub()
+        mock_calc_route_esi.return_value = None
+        enaluri: EveSolarSystem = EveSolarSystem.objects.get_or_create_esi(id=30045339)[
+            0
+        ]
+        thera, _ = EveSolarSystem.objects.get_or_create_esi(id=31000005)
+        # when
+        result = enaluri.route_to(thera)
+        # then
+        self.assertIsNone(result)
 
 
 @patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_DOGMAS", False)
 @patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_MARKET_GROUPS", False)
 @patch(MANAGERS_PATH + ".esi")
 class TestEveStar(NoSocketsTestCase):
     def test_create_from_esi(self, mock_esi):
```

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_2.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/test_models_2.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_3.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/test_models_3.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_4.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/test_models_4.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_tasks.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_tools_testdata.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/test_tools_testdata.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_utils.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata_example.json` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata_example.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/esi.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/esi.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/esi_data.json` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/esi_data.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/factories.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/fetch_esi_raw_data.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/fetch_esi_raw_data.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/generate_sde.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/generate_sde.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/sde.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/sde.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/sde_data.json` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/testdata/sde_data.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tests/tools/clear_celery_once_locks.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tests/tools/clear_celery_once_locks.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tools/drop_tables.sql` & `django_eveuniverse-1.0.0a3/eveuniverse/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/eveuniverse/tools/testdata.py` & `django_eveuniverse-1.0.0a3/eveuniverse/tools/testdata.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/LICENSE` & `django_eveuniverse-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a2/README.md` & `django_eveuniverse-1.0.0a3/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,56 @@
-# Eve Universe
+django-eveuniverse
+==================
 
-Complete set of Eve Online Universe models in Django with on-demand loading from ESI
+Complete set of Eve Online Universe models in Django with on-demand
+loading from ESI.
 
-[![release](https://img.shields.io/pypi/v/django-eveuniverse?label=release)](https://pypi.org/project/django-eveuniverse/)
-[![python](https://img.shields.io/pypi/pyversions/django-eveuniverse)](https://pypi.org/project/django-eveuniverse/)
-[![django](https://img.shields.io/pypi/djversions/django-eveuniverse?label=django)](https://pypi.org/project/django-eveuniverse/)
-[![pipeline](https://gitlab.com/ErikKalkoken/django-eveuniverse/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/django-eveuniverse/-/pipelines)
-[![codecov](https://codecov.io/gl/ErikKalkoken/django-eveuniverse/branch/master/graph/badge.svg?token=YZF6RVSK0P)](https://codecov.io/gl/ErikKalkoken/django-eveuniverse)
-[![Documentation Status](https://readthedocs.org/projects/django-eveuniverse/badge/?version=latest)](https://django-eveuniverse.readthedocs.io/en/latest/?badge=latest)
-[![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/django-eveuniverse/-/blob/master/LICENSE)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
+|release| |python| |django| |pipeline| |codecov| |Documentation Status|
+|license| |pre-commit| |Code style: black| |chat|
 
-## Overview
-
-*django-eveuniverse* is a foundation app meant to help speed up the development of Eve Online apps with Django and ESI. It provides all classic "static" Eve classes as Django models, including all relationships, ready to be used in your project. Furthermore, all Eve models have an on-demand loading mechanism for fetching new objects from ESI.
+Overview
+--------
+
+*django-eveuniverse* is a foundation app meant to help speed up the
+development of Eve Online apps with Django and ESI. It provides all
+classic “static” Eve classes as Django models, including all
+relationships, ready to be used in your project. Furthermore, all Eve
+models have an on-demand loading mechanism for fetching new objects from
+ESI.
 
 Here is an overview of the main features:
 
-- Complete set of ESI's Eve Universe objects as Django models like regions, types or planets.
-- On-demand loading mechanism that allows retrieving Eve universe objects ad-hoc from ESI
-- Management commands for preloading often used sets of data like the map or ships types
-- Eve models come with additional useful features, e.g. a route finder between solar systems or image URLs for types
-- Special model EveEntity for quickly resolving Eve Online IDs to names
-- Optional asynchronous loading of eve models and loading of all related children. (e.g. load all types for a specific group)
-- Additional models for selected data from the SDE that is not covered by ESI, e.g. type materials
-
-## Documentation
-
-For details on how to install and use *django-eveuniverse* please see the [documentation](https://django-eveuniverse.readthedocs.io/en/latest/).
+*  Complete set of ESI's Eve Universe objects as Django models like
+   regions, types or planets.
+*  On-demand loading mechanism that allows retrieving Eve universe
+   objects ad-hoc from ESI
+*  Management commands for preloading often used sets of data like the
+   map or ships types
+*  Eve models come with additional useful features, e.g. a route finder
+   between solar systems or image URLs for types
+*  Special model EveEntity for quickly resolving Eve Online IDs to names
+*  Optional asynchronous loading of eve models and loading of all
+   related children. (e.g. load all types for a specific group)
+*  Additional models for selected data from the SDE that is not covered
+   by ESI, e.g. type materials
+
+
+.. |release| image:: https://img.shields.io/pypi/v/django-eveuniverse?label=release
+   :target: https://pypi.org/project/django-eveuniverse/
+.. |python| image:: https://img.shields.io/pypi/pyversions/django-eveuniverse
+   :target: https://pypi.org/project/django-eveuniverse/
+.. |django| image:: https://img.shields.io/pypi/djversions/django-eveuniverse?label=django
+   :target: https://pypi.org/project/django-eveuniverse/
+.. |pipeline| image:: https://gitlab.com/ErikKalkoken/django-eveuniverse/badges/master/pipeline.svg
+   :target: https://gitlab.com/ErikKalkoken/django-eveuniverse/-/pipelines
+.. |codecov| image:: https://codecov.io/gl/ErikKalkoken/django-eveuniverse/branch/master/graph/badge.svg?token=YZF6RVSK0P
+   :target: https://codecov.io/gl/ErikKalkoken/django-eveuniverse
+.. |Documentation Status| image:: https://readthedocs.org/projects/django-eveuniverse/badge/?version=latest
+   :target: https://django-eveuniverse.readthedocs.io/en/latest/?badge=latest
+.. |license| image:: https://img.shields.io/badge/license-MIT-green
+   :target: https://gitlab.com/ErikKalkoken/django-eveuniverse/-/blob/master/LICENSE
+.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+   :target: https://github.com/pre-commit/pre-commit
+.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+.. |chat| image:: https://img.shields.io/discord/790364535294132234
+   :target: https://discord.gg/zmh52wnfvM
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django_eveuniverse-1.0.0a2/pyproject.toml` & `django_eveuniverse-1.0.0a3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-eveuniverse"
 dynamic = ["version"]
 description = "Complete set of Eve Universe models with on-demand loading from ESI"
-readme = "README.md"
-license = "MIT"
-requires-python = "~=3.8"
+readme = "README.rst"
+license = {file = "LICENSE"}
+requires-python = ">=3.8"
 authors = [
     { name = "Erik Kalkoken", email = "kalkoken87@gmail.com" },
 ]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
@@ -35,23 +35,20 @@
     "django-bitfield>=2.2",
     "django-esi>=4,<5",
     "django>=3.2",
     "requests",
 ]
 
 [project.urls]
-Homepage = "https://gitlab.com/ErikKalkoken/django-eveuniverse"
+Documentation = "https://django-eveuniverse.readthedocs.io/en/latest/"
+Source = "https://gitlab.com/ErikKalkoken/django-eveuniverse"
+Tracker = "https://gitlab.com/ErikKalkoken/django-eveuniverse/issues"
 
-[tool.hatch.version]
-path = "eveuniverse/__init__.py"
-
-[tool.hatch.build]
-include = [
-    "/eveuniverse",
-]
+[tool.flit.module]
+name = "eveuniverse"
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.'MASTER']
 ignore-patterns="test_.*.py,__init__.py,generate_.*.py"
```

### Comparing `django_eveuniverse-1.0.0a2/PKG-INFO` & `django_eveuniverse-1.0.0a3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: django-eveuniverse
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Complete set of Eve Universe models with on-demand loading from ESI
-Project-URL: Homepage, https://gitlab.com/ErikKalkoken/django-eveuniverse
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
-License-Expression: MIT
-License-File: LICENSE
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,48 +16,74 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.8
-Requires-Dist: celery-once>=3.0.1
 Requires-Dist: celery>=4.0.2
+Requires-Dist: celery_once>=3.0.1
 Requires-Dist: django-bitfield>=2.2
-Requires-Dist: django-esi<5,>=4
+Requires-Dist: django-esi>=4,<5
 Requires-Dist: django>=3.2
 Requires-Dist: requests
-Description-Content-Type: text/markdown
-
-# Eve Universe
-
-Complete set of Eve Online Universe models in Django with on-demand loading from ESI
-
-[![release](https://img.shields.io/pypi/v/django-eveuniverse?label=release)](https://pypi.org/project/django-eveuniverse/)
-[![python](https://img.shields.io/pypi/pyversions/django-eveuniverse)](https://pypi.org/project/django-eveuniverse/)
-[![django](https://img.shields.io/pypi/djversions/django-eveuniverse?label=django)](https://pypi.org/project/django-eveuniverse/)
-[![pipeline](https://gitlab.com/ErikKalkoken/django-eveuniverse/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/django-eveuniverse/-/pipelines)
-[![codecov](https://codecov.io/gl/ErikKalkoken/django-eveuniverse/branch/master/graph/badge.svg?token=YZF6RVSK0P)](https://codecov.io/gl/ErikKalkoken/django-eveuniverse)
-[![Documentation Status](https://readthedocs.org/projects/django-eveuniverse/badge/?version=latest)](https://django-eveuniverse.readthedocs.io/en/latest/?badge=latest)
-[![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/django-eveuniverse/-/blob/master/LICENSE)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
-
-## Overview
-
-*django-eveuniverse* is a foundation app meant to help speed up the development of Eve Online apps with Django and ESI. It provides all classic "static" Eve classes as Django models, including all relationships, ready to be used in your project. Furthermore, all Eve models have an on-demand loading mechanism for fetching new objects from ESI.
+Project-URL: Documentation, https://django-eveuniverse.readthedocs.io/en/latest/
+Project-URL: Source, https://gitlab.com/ErikKalkoken/django-eveuniverse
+Project-URL: Tracker, https://gitlab.com/ErikKalkoken/django-eveuniverse/issues
+
+django-eveuniverse
+==================
+
+Complete set of Eve Online Universe models in Django with on-demand
+loading from ESI.
+
+|release| |python| |django| |pipeline| |codecov| |Documentation Status|
+|license| |pre-commit| |Code style: black| |chat|
+
+Overview
+--------
+
+*django-eveuniverse* is a foundation app meant to help speed up the
+development of Eve Online apps with Django and ESI. It provides all
+classic “static” Eve classes as Django models, including all
+relationships, ready to be used in your project. Furthermore, all Eve
+models have an on-demand loading mechanism for fetching new objects from
+ESI.
 
 Here is an overview of the main features:
 
-- Complete set of ESI's Eve Universe objects as Django models like regions, types or planets.
-- On-demand loading mechanism that allows retrieving Eve universe objects ad-hoc from ESI
-- Management commands for preloading often used sets of data like the map or ships types
-- Eve models come with additional useful features, e.g. a route finder between solar systems or image URLs for types
-- Special model EveEntity for quickly resolving Eve Online IDs to names
-- Optional asynchronous loading of eve models and loading of all related children. (e.g. load all types for a specific group)
-- Additional models for selected data from the SDE that is not covered by ESI, e.g. type materials
-
-## Documentation
+*  Complete set of ESI's Eve Universe objects as Django models like
+   regions, types or planets.
+*  On-demand loading mechanism that allows retrieving Eve universe
+   objects ad-hoc from ESI
+*  Management commands for preloading often used sets of data like the
+   map or ships types
+*  Eve models come with additional useful features, e.g. a route finder
+   between solar systems or image URLs for types
+*  Special model EveEntity for quickly resolving Eve Online IDs to names
+*  Optional asynchronous loading of eve models and loading of all
+   related children. (e.g. load all types for a specific group)
+*  Additional models for selected data from the SDE that is not covered
+   by ESI, e.g. type materials
+
+
+.. |release| image:: https://img.shields.io/pypi/v/django-eveuniverse?label=release
+   :target: https://pypi.org/project/django-eveuniverse/
+.. |python| image:: https://img.shields.io/pypi/pyversions/django-eveuniverse
+   :target: https://pypi.org/project/django-eveuniverse/
+.. |django| image:: https://img.shields.io/pypi/djversions/django-eveuniverse?label=django
+   :target: https://pypi.org/project/django-eveuniverse/
+.. |pipeline| image:: https://gitlab.com/ErikKalkoken/django-eveuniverse/badges/master/pipeline.svg
+   :target: https://gitlab.com/ErikKalkoken/django-eveuniverse/-/pipelines
+.. |codecov| image:: https://codecov.io/gl/ErikKalkoken/django-eveuniverse/branch/master/graph/badge.svg?token=YZF6RVSK0P
+   :target: https://codecov.io/gl/ErikKalkoken/django-eveuniverse
+.. |Documentation Status| image:: https://readthedocs.org/projects/django-eveuniverse/badge/?version=latest
+   :target: https://django-eveuniverse.readthedocs.io/en/latest/?badge=latest
+.. |license| image:: https://img.shields.io/badge/license-MIT-green
+   :target: https://gitlab.com/ErikKalkoken/django-eveuniverse/-/blob/master/LICENSE
+.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+   :target: https://github.com/pre-commit/pre-commit
+.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+.. |chat| image:: https://img.shields.io/discord/790364535294132234
+   :target: https://discord.gg/zmh52wnfvM
 
-For details on how to install and use *django-eveuniverse* please see the [documentation](https://django-eveuniverse.readthedocs.io/en/latest/).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

