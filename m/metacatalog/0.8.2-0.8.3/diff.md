# Comparing `tmp/metacatalog-0.8.2.tar.gz` & `tmp/metacatalog-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metacatalog-0.8.2.tar", last modified: Tue Feb 28 09:23:18 2023, max compression
+gzip compressed data, was "metacatalog-0.8.3.tar", last modified: Tue May 30 19:29:32 2023, max compression
```

## Comparing `metacatalog-0.8.2.tar` & `metacatalog-0.8.3.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.954594 metacatalog-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-02-28 09:23:07.000000 metacatalog-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-02-28 09:23:07.000000 metacatalog-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-02-28 09:23:18.954594 metacatalog-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-02-28 09:23:07.000000 metacatalog-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-02-28 09:23:07.000000 metacatalog-0.8.2/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.938594 metacatalog-0.8.2/metacatalog/
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.942594 metacatalog-0.8.2/metacatalog/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/api/_mapping.py
--rw-r--r--   0 runner    (1001) docker     (122)    31778 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/api/add.py
--rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     9722 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/api/db.py
--rw-r--r--   0 runner    (1001) docker     (122)    43135 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/api/find.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/api/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/api/show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.942594 metacatalog-0.8.2/metacatalog/cmd/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/cmd/_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/cmd/add.py
--rw-r--r--   0 runner    (1001) docker     (122)      635 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/cmd/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)      760 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/cmd/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/cmd/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     3396 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/cmd/find.py
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/cmd/init.py
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/cmd/migration.py
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/cmd/populate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/cmd/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     8005 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/command_line.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.946594 metacatalog-0.8.2/metacatalog/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      443 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/data/datasource_types.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1538 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/data/datatypes.csv
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/data/entrygroup_types.csv
--rw-r--r--   0 runner    (1001) docker     (122)   489380 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/data/keywords.csv
--rw-r--r--   0 runner    (1001) docker     (122)     4405 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/data/licenses.csv
--rw-r--r--   0 runner    (1001) docker     (122)     3645 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/data/person_roles.csv
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/data/thesaurus.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/data/units.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/data/variables.csv
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.946594 metacatalog-0.8.2/metacatalog/db/
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4828 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/migration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.950594 metacatalog-0.8.2/metacatalog/db/revisions/
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev0.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev1.py
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev10.py
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev11.py
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev12.py
--rw-r--r--   0 runner    (1001) docker     (122)      945 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev13.py
--rw-r--r--   0 runner    (1001) docker     (122)      823 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev14.py
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev3.py
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev4.py
--rw-r--r--   0 runner    (1001) docker     (122)     1438 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev5.py
--rw-r--r--   0 runner    (1001) docker     (122)     4546 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev6.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev7.py
--rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev8.py
--rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/revisions/rev9.py
--rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/db/session.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.950594 metacatalog-0.8.2/metacatalog/ext/
--rw-r--r--   0 runner    (1001) docker     (122)     4714 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3789 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.950594 metacatalog-0.8.2/metacatalog/ext/export/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17549 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/export/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.950594 metacatalog-0.8.2/metacatalog/ext/io/
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/io/appender.py
--rw-r--r--   0 runner    (1001) docker     (122)     4772 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/io/deleter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/io/extension.py
--rw-r--r--   0 runner    (1001) docker     (122)     9716 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/io/importer.py
--rw-r--r--   0 runner    (1001) docker     (122)    12174 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/io/interface.py
--rw-r--r--   0 runner    (1001) docker     (122)     3926 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/io/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.950594 metacatalog-0.8.2/metacatalog/ext/standards_export/
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/standards_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16616 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/standards_export/extension.py
--rw-r--r--   0 runner    (1001) docker     (122)    25458 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/ext/standards_export/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.950594 metacatalog-0.8.2/metacatalog/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2854 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    21912 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/datasource.py
--rw-r--r--   0 runner    (1001) docker     (122)     5804 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/details.py
--rw-r--r--   0 runner    (1001) docker     (122)    41934 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     9220 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/entrygroup.py
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/generic_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/geometry_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     9646 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/keyword.py
--rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/license.py
--rw-r--r--   0 runner    (1001) docker     (122)     8838 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/person.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/timeseries_legacy.py
--rw-r--r--   0 runner    (1001) docker     (122)     7106 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/models/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.954594 metacatalog-0.8.2/metacatalog/test/
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2027 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/_util.py
--rw-r--r--   0 runner    (1001) docker     (122)    11141 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_api_add_find.py
--rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_api_install.py
--rw-r--r--   0 runner    (1001) docker     (122)     1748 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_api_location.py
--rw-r--r--   0 runner    (1001) docker     (122)    15064 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_array_type_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_cli_find.py
--rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_db_migrations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2710 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_export_extension.py
--rw-r--r--   0 runner    (1001) docker     (122)     4089 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_groups_projects.py
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     3148 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_models_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_pg_install.py
--rw-r--r--   0 runner    (1001) docker     (122)     6778 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_result_set.py
--rw-r--r--   0 runner    (1001) docker     (122)     5012 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_standards_export.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_todict_fromdict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/test/test_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.954594 metacatalog-0.8.2/metacatalog/util/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/util/dict_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9407 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/util/location.py
--rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/util/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    22714 2023-02-28 09:23:07.000000 metacatalog-0.8.2/metacatalog/util/results.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 09:23:18.942594 metacatalog-0.8.2/metacatalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-02-28 09:23:18.000000 metacatalog-0.8.2/metacatalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3588 2023-02-28 09:23:18.000000 metacatalog-0.8.2/metacatalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-28 09:23:18.000000 metacatalog-0.8.2/metacatalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-02-28 09:23:18.000000 metacatalog-0.8.2/metacatalog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-28 09:23:18.000000 metacatalog-0.8.2/metacatalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-02-28 09:23:18.000000 metacatalog-0.8.2/metacatalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-28 09:23:18.000000 metacatalog-0.8.2/metacatalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-02-28 09:23:07.000000 metacatalog-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-28 09:23:18.954594 metacatalog-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-02-28 09:23:07.000000 metacatalog-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.610525 metacatalog-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-30 19:29:21.000000 metacatalog-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-30 19:29:21.000000 metacatalog-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-05-30 19:29:32.610525 metacatalog-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-05-30 19:29:21.000000 metacatalog-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-30 19:29:21.000000 metacatalog-0.8.3/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.594524 metacatalog-0.8.3/metacatalog/
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.594524 metacatalog-0.8.3/metacatalog/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/api/_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31778 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9722 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/api/db.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43135 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/api/find.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/api/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/api/show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.598525 metacatalog-0.8.3/metacatalog/cmd/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/cmd/_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/cmd/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)      635 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/cmd/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)      760 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/cmd/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/cmd/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3396 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/cmd/find.py
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/cmd/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/cmd/migration.py
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/cmd/populate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/cmd/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8005 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.598525 metacatalog-0.8.3/metacatalog/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      443 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/data/datasource_types.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     1538 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/data/datatypes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/data/entrygroup_types.csv
+-rw-r--r--   0 runner    (1001) docker     (122)   489380 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/data/keywords.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     4405 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/data/licenses.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     3645 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/data/person_roles.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/data/thesaurus.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/data/units.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/data/variables.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.598525 metacatalog-0.8.3/metacatalog/db/
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4828 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/migration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.602525 metacatalog-0.8.3/metacatalog/db/revisions/
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev0.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev1.py
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev10.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev11.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev12.py
+-rw-r--r--   0 runner    (1001) docker     (122)      945 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev13.py
+-rw-r--r--   0 runner    (1001) docker     (122)      823 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev14.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev3.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev4.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1438 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev5.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4546 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev6.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev7.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev8.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/revisions/rev9.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/db/session.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.602525 metacatalog-0.8.3/metacatalog/ext/
+-rw-r--r--   0 runner    (1001) docker     (122)     4714 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3789 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.602525 metacatalog-0.8.3/metacatalog/ext/export/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17549 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/export/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.602525 metacatalog-0.8.3/metacatalog/ext/io/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/io/appender.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4772 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/io/deleter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/io/extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9716 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/io/importer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12174 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/io/interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3926 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/io/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.606525 metacatalog-0.8.3/metacatalog/ext/standards_export/
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/standards_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21014 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/standards_export/extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29298 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/ext/standards_export/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.606525 metacatalog-0.8.3/metacatalog/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2854 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21912 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5804 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/details.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41934 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9220 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/entrygroup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/generic_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/geometry_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9646 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/keyword.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/license.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8838 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/timeseries_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7106 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/models/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.610525 metacatalog-0.8.3/metacatalog/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2027 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11141 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_api_add_find.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_api_install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1748 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_api_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15064 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_array_type_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_cli_find.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_db_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2710 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_export_extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4089 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_groups_projects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3148 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_models_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_pg_install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6778 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_result_set.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7489 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_standards_export.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_todict_fromdict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/test/test_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.610525 metacatalog-0.8.3/metacatalog/util/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/util/dict_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9407 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/util/location.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22714 2023-05-30 19:29:21.000000 metacatalog-0.8.3/metacatalog/util/results.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 19:29:32.594524 metacatalog-0.8.3/metacatalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-05-30 19:29:32.000000 metacatalog-0.8.3/metacatalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3588 2023-05-30 19:29:32.000000 metacatalog-0.8.3/metacatalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 19:29:32.000000 metacatalog-0.8.3/metacatalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-30 19:29:32.000000 metacatalog-0.8.3/metacatalog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 19:29:32.000000 metacatalog-0.8.3/metacatalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-05-30 19:29:32.000000 metacatalog-0.8.3/metacatalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-30 19:29:32.000000 metacatalog-0.8.3/metacatalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-05-30 19:29:21.000000 metacatalog-0.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 19:29:32.610525 metacatalog-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-05-30 19:29:21.000000 metacatalog-0.8.3/setup.py
```

### Comparing `metacatalog-0.8.2/LICENSE` & `metacatalog-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/PKG-INFO` & `metacatalog-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metacatalog
-Version: 0.8.2
+Version: 0.8.3
 Summary: Metadata model management module.
 Author: Mirko Mälicke
 Author-email: mirko.maelicke@kit.edu
 License: GPL v3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `metacatalog-0.8.2/README.md` & `metacatalog-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/__init__.py` & `metacatalog-0.8.3/metacatalog/__init__.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/api/__init__.py` & `metacatalog-0.8.3/metacatalog/api/__init__.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/api/_mapping.py` & `metacatalog-0.8.3/metacatalog/api/_mapping.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/api/add.py` & `metacatalog-0.8.3/metacatalog/api/add.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/api/catalog.py` & `metacatalog-0.8.3/metacatalog/api/catalog.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/api/db.py` & `metacatalog-0.8.3/metacatalog/api/db.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/api/find.py` & `metacatalog-0.8.3/metacatalog/api/find.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/api/io.py` & `metacatalog-0.8.3/metacatalog/api/io.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/api/show.py` & `metacatalog-0.8.3/metacatalog/api/show.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/cmd/_util.py` & `metacatalog-0.8.3/metacatalog/cmd/_util.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/cmd/add.py` & `metacatalog-0.8.3/metacatalog/cmd/add.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/cmd/catalog.py` & `metacatalog-0.8.3/metacatalog/cmd/catalog.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/cmd/connection.py` & `metacatalog-0.8.3/metacatalog/cmd/connection.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/cmd/find.py` & `metacatalog-0.8.3/metacatalog/cmd/find.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/cmd/migration.py` & `metacatalog-0.8.3/metacatalog/cmd/migration.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/cmd/show.py` & `metacatalog-0.8.3/metacatalog/cmd/show.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/command_line.py` & `metacatalog-0.8.3/metacatalog/command_line.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/data/datatypes.csv` & `metacatalog-0.8.3/metacatalog/data/datatypes.csv`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/data/entrygroup_types.csv` & `metacatalog-0.8.3/metacatalog/data/entrygroup_types.csv`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/data/keywords.csv` & `metacatalog-0.8.3/metacatalog/data/keywords.csv`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/data/licenses.csv` & `metacatalog-0.8.3/metacatalog/data/licenses.csv`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/data/person_roles.csv` & `metacatalog-0.8.3/metacatalog/data/person_roles.csv`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/data/units.csv` & `metacatalog-0.8.3/metacatalog/data/units.csv`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/data/variables.csv` & `metacatalog-0.8.3/metacatalog/data/variables.csv`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/migration.py` & `metacatalog-0.8.3/metacatalog/db/migration.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev0.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev0.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev1.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev1.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev10.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev10.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev11.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev11.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev12.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev12.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev13.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev13.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev14.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev14.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev2.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev2.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev3.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev3.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev4.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev4.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev5.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev5.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev6.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev6.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev7.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev7.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev8.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev8.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/revisions/rev9.py` & `metacatalog-0.8.3/metacatalog/db/revisions/rev9.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/db/session.py` & `metacatalog-0.8.3/metacatalog/db/session.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/ext/__init__.py` & `metacatalog-0.8.3/metacatalog/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/ext/base.py` & `metacatalog-0.8.3/metacatalog/ext/base.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/ext/export/extension.py` & `metacatalog-0.8.3/metacatalog/ext/export/extension.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/ext/io/appender.py` & `metacatalog-0.8.3/metacatalog/ext/io/appender.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/ext/io/deleter.py` & `metacatalog-0.8.3/metacatalog/ext/io/deleter.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/ext/io/extension.py` & `metacatalog-0.8.3/metacatalog/ext/io/extension.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/ext/io/importer.py` & `metacatalog-0.8.3/metacatalog/ext/io/importer.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/ext/io/interface.py` & `metacatalog-0.8.3/metacatalog/ext/io/interface.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/ext/io/reader.py` & `metacatalog-0.8.3/metacatalog/ext/io/reader.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/ext/standards_export/extension.py` & `metacatalog-0.8.3/metacatalog/ext/standards_export/extension.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sqlalchemy.orm import Session
 from sqlalchemy.orm.exc import NoResultFound
 import xml.etree.ElementTree as ET
 from tqdm import tqdm
 
 
 from metacatalog.ext import MetacatalogExtensionInterface
-from metacatalog.ext.standards_export.util import _parse_iso_information, _init_jinja, _validate_xml
+from metacatalog.ext.standards_export.util import _parse_export_information, _init_jinja, _validate_xml
 from metacatalog import api
 from metacatalog.models import Entry
 from metacatalog.util.results import ImmutableResultSet
 from metacatalog.cmd._util import connect, cprint
 
 
 # default dictionary with the expected structure and keys and dummy values
@@ -41,69 +41,84 @@
 # default template_path to the iso19115 jinja template, can be overwritten in functions with parameter template_path
 TEMPLATE_PATH = os.path.abspath(os.path.join(os.path.dirname(__file__), 'schemas', 'iso19115', 'iso19115-2.j2'))
 
 
 class StandardsExportExtension(MetacatalogExtensionInterface):
     r"""
     Extension to export Entries in standard format.
-    Currently, ISO 19115 export is implemented.
+    ISO 19115 and DataCite metadata standard formats
+    are supported.
+    The exported standard is determined by the jinja
+    template passed to the extension functions as 
+    parameter ``template_path``.
 
     Adds the method standards_export to :class:`Entry <metacatalog.models.Entry>`
-    which creates the metadata standard XML for the :class:`ImmutableResultSet <metacatalog.utils.results.ImmutableResultSet>`
+    which returns the metadata standard as a Python 
+    XML ElementTree representation for the :class:`ImmutableResultSet <metacatalog.utils.results.ImmutableResultSet>`
     of the Entry.
-    The method standards_export is added to the API
-    (metacatalog.api.catalog). This method can be
-    used to export Entries / ImmutableResultSets
+    The method ``create_standards_xml`` is added to the 
+    API (metacatalog.api.catalog), which is used to 
+    export Entries / ImmutableResultSets
     in the database session and write the XML files
     to the folder location specified in ``path``.
+    Additionally, the command ``standards-export`` is
+    added to the metacatalog CLI. The command is used to
+    export one or more Entries via the command line.
+
+    .. versionchanged:: 0.8.3
+    Support for DataCite export added.
 
     """
     @classmethod
     def init_extension(cls):
         # wrapper which calls StandardsExportExtension.standards_export
-        def wrapper_entry(self: Entry, config_dict: dict = {}, template_path: str = TEMPLATE_PATH) -> ET.ElementTree:  
-            return StandardsExportExtension.standards_export(entry_or_resultset=self, config_dict=config_dict, template_path=template_path)
+        def wrapper_entry(self: Entry, config_dict: dict = {}, template_path: str = TEMPLATE_PATH, strict:bool = False) -> ET.ElementTree:
+            return StandardsExportExtension.standards_export(entry_or_resultset=self, config_dict=config_dict, template_path=template_path, strict=strict)
         
         # standards_export docstring and name for wrapper function
         wrapper_entry.__doc__ = StandardsExportExtension.standards_export.__doc__
         wrapper_entry.__name__ = StandardsExportExtension.standards_export.__name__
         
         # add wrapper to Entry model
         Entry.standards_export = wrapper_entry
 
         # add function create_iso19115 to api.catalog
-        def wrapper_api(session: Session, id_or_uuid: Union[int, str], config_dict: dict = {}, path: str = None, template_path: str = TEMPLATE_PATH):
-            return StandardsExportExtension.create_iso19115_xml(session, id_or_uuid, config_dict, path, template_path)
+        def wrapper_api(session: Session, id_or_uuid: Union[int, str], config_dict: dict = {}, path: str = None, template_path: str = TEMPLATE_PATH, strict: bool = False):
+            return StandardsExportExtension.create_standards_xml(session=session, id_or_uuid=id_or_uuid, config_dict=config_dict, path=path, template_path=template_path, strict=strict)
 
-        wrapper_api.__doc__ = StandardsExportExtension.create_iso19115_xml.__doc__
-        wrapper_api.__name__ = StandardsExportExtension.create_iso19115_xml.__name__
+        wrapper_api.__doc__ = StandardsExportExtension.create_standards_xml.__doc__
+        wrapper_api.__name__ = StandardsExportExtension.create_standards_xml.__name__
 
         # add wrapper to api.catalog
-        api.catalog.create_iso19115_xml = wrapper_api
+        api.catalog.create_standards_xml = wrapper_api
 
 
     @classmethod
     def init_cli(cls, subparsers, defaults):
+        """
+        Add the parser ``standards-export`` to the metacatalog CLI and register
+        arguments.
+        
+        """
         myparser = subparsers.add_parser('standards-export', parents=[defaults], help="Export metadata in standard format as .xml files.")
         myparser.add_argument('entries', nargs='*', help='ID(s) or UUID(s) of Entries to export.')
-        myparser.add_argument('--format', choices=['iso19115'], type=str, nargs='?', const='iso19115', default='iso19115', help="Metadata standard format.")
+        myparser.add_argument('--format', choices=['iso19115', 'datacite'], type=str, nargs='?', const='iso19115', default='iso19115', help="Metadata standard format.")
         myparser.add_argument('--path', type=str, help="Directory to save XML file(s) to, `if not specified, the current folder is used.")
         myparser.add_argument('--all', action='store_true', help="Export all entries in the session to ISO 19115, cannot be used together with --id or --uuid.")
+        myparser.add_argument('--strict', action='store_true', help="Only generate syntactically (well-formed) and content validated XML files.")
         myparser.set_defaults(func=StandardsExportExtension.cli_create_standards_xml)
 
 
     @classmethod
-    def standards_export(cls, entry_or_resultset: Union[Entry, ImmutableResultSet], config_dict: dict = {}, template_path: str = TEMPLATE_PATH) -> ET.ElementTree:
+    def standards_export(cls, entry_or_resultset: Union[Entry, ImmutableResultSet], config_dict: dict = {}, template_path: str = TEMPLATE_PATH, strict:bool = False) -> ET.ElementTree:
         """
         Export a :class:`Entry <metacatalog.models.Entry>` or 
         :class:`ImmutableResultSet <metacatalog.util.results.ImmutableResultSet>` to XML.
-        The metadata standard is dependent on the jinja2 template passed to this function
-        in template_path.
-        Repeatable information input is always a list, as we can loop over the lists in the
-        jinja2 template.
+        The metadata standard is determined by the jinja2 template passed to this function
+        as paramter ``template_path``.
         Always returns an :class:`ElementTree <xml.etree.ElementTree.ElementTree>` object.
 
         This function is added as a method to :class:`Entry <metacatalog.models.Entry>`
         when the extension is activated. 
 
         .. versionadded:: 0.7.7
 
@@ -112,182 +127,220 @@
         entry_or_resultset : Union[Entry, ImmutableResultSet]
             The entry instance to be exported
         config_dict : dict
             Configuration dictionary, containing information about the data provider.
             The following keys and their values are expected when rendering the 
             jinja template:
 
-            .. code-block:: Python
+            .. code-block:: python
 
-            dict(
-                contact = dict(
-                    organisationName = '',
-                    deliveryPoint = '',
-                    city = '',
-                    administrativeArea = '',
-                    postalCode = '',
-                    country = '',
-                    electronicMailAddress = ['', ''],
-                    linkage = '',
-                    linkage_name = '',
-                    linkage_description = ''
-                ),
-                publisher = dict(
-                    organisation_name = ''
-                ))
+                dict(
+                    contact = dict(
+                        organisationName = '',
+                        deliveryPoint = '',
+                        city = '',
+                        administrativeArea = '',
+                        postalCode = '',
+                        country = '',
+                        electronicMailAddress = ['', ''],
+                        linkage = '',
+                        linkage_name = '',
+                        linkage_description = ''
+                    ),
+                    publisher = dict(
+                        organisation_name = ''
+                    )
+                    )
             
-            It is also possible to create a .json file ``iso19115_contact.json`` containing the
-            contact information and add the path to this file to the metacatalog CONFIGFILE under 
-            the top level key ``extra``:
+            It is also possible to create a .json file ``standards_export_contact.json`` 
+            containing the contact information and add the path to this file to the 
+            metacatalog CONFIGFILE under the top level key ``extra``:
 
             .. code-block:: json
 
-            "extra":{
-    	        "iso19115_contact": "/path/to/iso19115_contact.json"
-                }
+                "extra":{
+                    "standards_export_contact": "/path/to/standards_export_contact.json"
+                    }
 
-            This is the only way to add the contact information if you use the metacatalog CLI
-            for the export of metadata standards.
         template_path : str
             Full path (including the template name) to the jinja2 template for 
-            metadata export.  
-            Currently defaults to the ISO 19115 template.
+            metadata export. This determines the metadata standard for export.
+            Defaults to ISO 19115 template.
+        strict : bool
+            .. versionadded:: 0.8.3
+            
+            If strict is True, only syntactically (well-formed) and content validated 
+            XML files are generated.  
+            Note that in version ``v0.8.3``, DataCite XML files are never valid in terms of
+            content, as metacatalog does currently not provice DOIs for its datasets.  
+            In the case of ISO 19115, content is currently not validated and a 
+            ``NotImplementedError`` is raised.  
+            Defaults to False.
         
         Returns
         ----------
         xml_etree : xml.etree.ElementTree.ElementTree
             The :class:`ElementTree <xml.etree.ElementTree.ElementTree>` object
             representing the XML ElementTree in Python.
 
         Notes
         -----
-        The content of the file will be created using a 
-        :class:`ImmutableResultSet <metacatalog.utils.results.ImmutableResultSet>`.
+        The content of the file is created using a :class:`ImmutableResultSet <metacatalog.utils.results.ImmutableResultSet>`.
         This will lazy-load sibling Entries and parent groups as needed for
-        a useful Metadata export.
+        a useful metadata export.
 
         """
         from metacatalog import CONFIGFILE
 
         # use dummy values for contact as default
         contact_config = DEFAULT_CONTACT.copy()
 
         # get contact config from metacatalog CONFIGFILE if specified
         with open(CONFIGFILE, 'r') as f:
             config = json.load(f)
 
             # get base_config path from CONFIGFILE: path to user generated .json with contact info
-            base_config_path = config.get('extra', {}).get('iso19115_contact', '')
+            base_config_path = config.get('extra', {}).get('standards_export_contact', '')
 
             if base_config_path:
                 with open(base_config_path, 'r') as f:
                     base_config = json.load(f)
             else:
                 base_config = {}
 
         # update default config with contact info from CONFIGFILE
         contact_config.update(base_config)
 
         # update config with config passed to this function in config_dict
         contact_config.update(config_dict)
 
-        # get necessary input parameters from ImmutableResultSet for ISO export
-        iso_input = _parse_iso_information(entry_or_resultset)
+        # get necessary input parameters from ImmutableResultSet for export
+        export_information = _parse_export_information(entry_or_resultset)
 
         # get initialized jinja template
         template = _init_jinja(template_path)
 
         # render template with entry_dict
-        xml_str = template.render(**iso_input, **contact_config)
-
-        # check whether xml is well-formed
-        assert _validate_xml(xml_str)
+        xml_str = template.render(**export_information, **contact_config)
 
+        # strict mode
+        if strict:
+            # check whether xml is well-formed
+            assert _validate_xml(xml_str)
+
+            if 'iso19115' in template_path.lower():
+                raise NotImplementedError("You want to use strict mode for the generation of ISO 19115 metadata, the generated XML structure is well-formed but its content currently cannot be validated.")
+            elif 'datacite' in template_path.lower():
+                raise ValueError("You want to use strict mode for the generation of DataCite metadata, as metacatalog currently does not provide DOIs, the content of the generated XML file is not valid, as the DOI field is empty. Set strict=False to generate the XML nevertheless.")
+            
         # register namespaces for ElementTree representation of XML
-        ET.register_namespace('gmi', 'http://www.isotc211.org/2005/gmi')
-        ET.register_namespace('gco', 'http://www.isotc211.org/2005/gco')
-        ET.register_namespace('gmd', 'http://www.isotc211.org/2005/gmd')
-        ET.register_namespace('gml', 'http://www.opengis.net/gml/3.2')
-        ET.register_namespace('xlink', 'http://www.w3.org/1999/xlink')
+        if 'iso19115' in template_path.lower():
+            ET.register_namespace('gmi', 'http://www.isotc211.org/2005/gmi')
+            ET.register_namespace('', 'http://www.isotc211.org/2005/gmi')
+            ET.register_namespace('gco', 'http://www.isotc211.org/2005/gco')
+            ET.register_namespace('gmd', 'http://www.isotc211.org/2005/gmd')
+            ET.register_namespace('gml', 'http://www.opengis.net/gml/3.2')
+            ET.register_namespace('gmx', 'http://www.isotc211.org/2005/gmx')
+            ET.register_namespace('gsr', 'http://www.isotc211.org/2005/gsr')
+            ET.register_namespace('gss', 'http://www.isotc211.org/2005/gss')
+            ET.register_namespace('gts', 'http://www.isotc211.org/2005/gts')
+            ET.register_namespace('xlink', 'http://www.w3.org/1999/xlink')
+            ET.register_namespace('xsi', 'http://www.w3.org/2001/XMLSchema-instance')
+
+        elif 'datacite' in template_path.lower():
+            ET.register_namespace('', 'http://datacite.org/schema/kernel-4')
+            ET.register_namespace('xsi', 'http://www.w3.org/2001/XMLSchema-instance')
 
         # convert to ElementTree and return
         return ET.ElementTree(ET.fromstring(xml_str))
 
     @overload
-    def create_iso19115_xml(path: str) -> None: ...
+    def create_standards_xml(path: str) -> None: ...
     @overload
-    def create_iso19115_xml(path: Literal[None]) -> ET.ElementTree: ...
-    def create_iso19115_xml(session: Session, id_or_uuid: Union[int, str], config_dict: dict = {}, path: str = None, template_path: str = TEMPLATE_PATH) -> ET.ElementTree | None:
+    def create_standards_xml(path: Literal[None]) -> ET.ElementTree: ...
+    def create_standards_xml(session: Session, id_or_uuid: Union[int, str], config_dict: dict = {}, path: str = None, template_path: str = TEMPLATE_PATH, strict: bool = False) -> ET.ElementTree | None:
         """
         This function can be imported from metacatalog.api.catalog
 
-        Create ISO 19115 standard metadata XML file for an entry, which is 
-        found by its id or uuid.
+        Create standard metadata XML file for an entry, which is found by 
+        its id or uuid.
         The XML file is saved to the folder given in ``path``. If ``path``
         does not end with '.xml', the name of the XML file is generated 
-        with the uuid of the used ImmutableResultSet: 
-        f"iso19115_{irs_uuid}.xml".
+        with the uuid of the used ImmutableResultSet, depending on the 
+        exported standard: 
+        * ``f"iso19115_{irs_uuid}.xml"``.
+        * ``f"datacite_{irs_uuid}.xml``"
         If no ``path`` is given, the ``ElementTree`` XML representation
-        is returned instead. 
+        is returned. 
 
         .. versionadded:: 0.8.1
 
         Parameters
         ----------
         session : sqlalchemy.Session
             SQLAlchemy session connected to the database.
         id_or_uuid : Union[int, str]
             id or uuid of the Entry to be exported.
         config_dict : dict
             Configuration dictionary, containing information about the data provider.
             The following keys and their values are expected when rendering the 
             jinja template:
 
-            .. code-block:: Python
+            .. code-block:: python
 
-            dict(
-                contact = dict(
-                    organisationName = '',
-                    deliveryPoint = '',
-                    city = '',
-                    administrativeArea = '',
-                    postalCode = '',
-                    country = '',
-                    electronicMailAddress = ['', ''],
-                    linkage = '',
-                    linkage_name = '',
-                    linkage_description = ''
-                ),
-                publisher = dict(
-                    organisation_name = ''
-                ))
+                dict(
+                    contact = dict(
+                        organisationName = '',
+                        deliveryPoint = '',
+                        city = '',
+                        administrativeArea = '',
+                        postalCode = '',
+                        country = '',
+                        electronicMailAddress = ['', ''],
+                        linkage = '',
+                        linkage_name = '',
+                        linkage_description = ''
+                    ),
+                    publisher = dict(
+                        organisation_name = ''
+                    ))
 
         path : str
-            Location where the ISO19115 XML file is saved to.
+            Location where the .xml file is saved to.
             If path ends with the name of the XML file (i.e. ends with '.xml'), the file is
             named as given.
             If path is a folder location, the name of the XML file is auto-generated with
-            the uuid of the ImmutableResultSet of the entry: ``f"iso19115_{uuid}.xml".
-            If no path is given, the class:`ElementTree <xml.etree.ElementTree.ElementTree>` object
-            representing the XML ElementTree is returned.
+            the uuid of the ImmutableResultSet of the entry and the exported standard.
+            If no path is given, the class:`ElementTree <xml.etree.ElementTree.ElementTree>` 
+            XML object is returned.
         template_path : str
             Full path (including the template name) to the jinja2 template for 
-            metadata export.  
-            Currently defaults to the ISO 19115 template.
+            metadata export. This determines the metadata standard for export.
+            Defaults to ISO 19115 template.
+        strict:
+            .. versionadded:: 0.8.3
+            
+            If strict is True, only syntactically (well-formed) and content validated 
+            XML files are generated.  
+            Note that in this version, DataCite XML files are never valid in terms of
+            content, as metacatalog does currently not provice DOIs for its datasets.  
+            In the case of ISO 19115, content is currently not validated and a 
+            ``NotImplementedError`` is raised.  
+            Defaults to False.
 
         Returns
         ----------
         xml_etree : Union[ElementTree, None]
             If no path is given, the :class:`ElementTree <xml.etree.ElementTree.ElementTree>` object
             representing the XML ElementTree in Python is returned.
-            If a path is given, None is returned.
+            If a path is given, the .xml is created and ``None`` is returned.
         
         Notes
         ----------
-        The content of the file will be created using a 
+        The content of the file is created using a 
         :class:`ImmutableResultSet <metacatalog.utils.results.ImmutableResultSet>`.
         This will lazy-load sibling Entries and parent groups as needed for
         a useful Metadata export.  
 
         """
         # find the entry by id
         if isinstance(id_or_uuid, int):
@@ -299,76 +352,80 @@
         # find the entry by uuid
         elif isinstance(id_or_uuid, str):
             entry = api.find_entry(session, uuid=id_or_uuid)
             # raise error if no entry was found
             if not entry:
                 raise NoResultFound(f"No entry with uuid={id_or_uuid} was found.")
 
-        # export entry to ISO 19115
-        xml_etree = entry.standards_export(config_dict=config_dict, template_path=template_path)
+        # create xml etree entry, standard
+        xml_etree = entry.standards_export(config_dict=config_dict, template_path=template_path, strict=strict)
 
         if not path:
             return xml_etree
 
-        # if path is given: write XML file
+        # if path is given: create XML file
         else:
-            # get the uuid of the ImmutableResultSet that is written to ISO19115 XML (rs.group.uuid or rs.get('uuid'))
+            # get the uuid of the ImmutableResultSet that is written to XML (rs.group.uuid or rs.get('uuid'))
             irs_uuid = ImmutableResultSet(entry).uuid
 
             # use absolute path
             path = os.path.abspath(path)
 
             # if path does not end with .xml: auto-generate XML filename
             if not path.endswith('.xml'):
-                path += f"/iso19115_{irs_uuid}.xml"
+                if 'iso19115' in template_path.lower():
+                    path += f"/iso19115_{irs_uuid}.xml"
+                elif 'datacite' in template_path.lower():
+                    path += f"/datacite_{irs_uuid}.xml"
 
             # write XML file
             with open(path, 'wb') as f:
                 xml_etree.write(f, encoding='utf-8')
 
 
     @classmethod
     def cli_create_standards_xml(cls, args):
         """
-        Function that determines which metadata standard to use and which 
-        executes the appropriate cli_create_*_xml() function based on the 
-        ``--format`` argument.
-
-        .. versionadded:: 0.8.2
-        
-        """
-        if args.format == 'iso19115':
-            StandardsExportExtension.cli_create_iso19115_xml(args)
-
-
-    @classmethod
-    def cli_create_iso19115_xml(cls, args):
-        """
-        Adds functionality to the metacatalog CLI to enable ISO 19115
-        XML export.
+        Adds functionality to the metacatalog CLI to export metadata of 
+        Entries in standard format as .xml files.
         Export one or more Entries, which are identified by positional
         argument entries. Entries can be identified by ID or UUID and  
-        are exported in ISO 19115 format. The produced .xml file is saved 
-        to the location specified with argument --path.
+        are exported in standard format. The metadata standard is specified
+        with argument --format.
+        The produced .xml file is saved to the location specified with 
+        argument --path.
         If no path is given, the .xml file is saved to the current
         working directory.
         Use the flag --all to export all entries in the given metacatalog
         connection.
+        Use the flag --strict to only export well-formed and content
+        validated XML files (defaults to False).
 
         .. versionadded:: 0.8.2
 
+
+        Example
+        ----------
+        With the following command, ISO 19115 XML files for the entries with
+        id=10 and id=20 in the default database session are created under the
+        specified path:
+
+        .. code-block:: bash
+            
+            $ python -m metacatalog standards-export 10 20 --format iso19115 --path /path/to/store/xmls --connection default
+
         Notes
         ----------
         The content of the xml files will be created using a 
         :class:`ImmutableResultSet <metacatalog.utils.results.ImmutableResultSet>`.
         This will lazy-load sibling Entries and parent groups as needed for
         a useful Metadata export.  
 
         """
-        from metacatalog.api.catalog import create_iso19115_xml
+        from metacatalog.api.catalog import create_standards_xml
 
         # get the session
         session = connect(args)
 
         # check path (mandatory)
         if args.path:
             path = args.path
@@ -380,23 +437,32 @@
             cprint(args, "Please provide the ID(s) or UUID(s) of Entries to be exported or use flag --all to export all Entries in the database session.")
             exit(0)
 
         if args.entries and args.all:
             cprint(args, "Flag --all cannot be used together with an ID or UUID.")
             exit(0)
 
+        # get jinja template, depending on --format
+        if args.format.lower() == 'iso19115':
+            template_path = os.path.abspath(os.path.join(os.path.dirname(__file__), 'schemas', 'iso19115', 'iso19115-2.j2'))
+        elif args.format.lower() == 'datacite':
+            template_path = os.path.abspath(os.path.join(os.path.dirname(__file__), 'schemas', 'datacite', 'datacite.j2'))
+
         # get entries to be exported
         if args.entries:
             # if '-' in x -> uuid, else id
             id_or_uuids = [str(x) if '-' in x else int(x) for x in args.entries]
 
         # flag --all: all entry ids
         elif args.all:
             id_or_uuids = [entry.id for entry in api.find_entry(session)]
 
+        # switch strict mode
+        strict = True if args.strict else False
+
         # run API ISO 19115 export function
         if args.verbose:
             for id_or_uuid in tqdm(id_or_uuids):
-                create_iso19115_xml(session=session, id_or_uuid=id_or_uuid, config_dict={}, path=path)
+                create_standards_xml(session=session, id_or_uuid=id_or_uuid, config_dict={}, path=path, template_path=template_path, strict=strict)
         else:
             for id_or_uuid in id_or_uuids:
-                create_iso19115_xml(session=session, id_or_uuid=id_or_uuid, config_dict={}, path=path)
+                create_standards_xml(session=session, id_or_uuid=id_or_uuid, config_dict={}, path=path, template_path=template_path, strict=strict)
```

### Comparing `metacatalog-0.8.2/metacatalog/ext/standards_export/util.py` & `metacatalog-0.8.3/metacatalog/ext/standards_export/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,31 +60,36 @@
     Returns the uuid of the base group (if exists). If no base group
     exists in the ImmutableResultSet, the uuid of the (single) member 
     is returned.
 
     Returns
     ----------
     uuid : str
-        Used for field <gmd:fileIdentifier> and field <gmd:identifier>, not repeatable.
+
+        * ISO19115: ``<gmd:fileIdentifier>`` and field ``<gmd:identifier>``, not repeatable.
 
     """
     return rs.uuid
 
 
 def _get_lastUpdate(rs: ImmutableResultSet) -> str:
     """
     Returns lastUpdate of ImmutableResultSet.  
     Returns the uuid of the base group (if exists) or the latest value of lastUpdate of 
     all members.
 
     Returns
     ----------
     lastUpdate : str
-        Used for field <gmd:dateStamp> and field <gmd:date> with <gmd:dateType> 'revision'
-        and field <gmd:editionDate>, str in ISO-date-format, not repeatable.
+        Character string in ISO-date-format.
+
+        * ISO 19115: ``<gmd:dateStamp>`` and field ``<gmd:date>`` with ``<gmd:dateType>`` 'revision'
+        and field ``<gmd:editionDate>``, not repeatable.
+
+        * DataCite: ``<date dateType="Updated">``
 
     """
     # if a base group exists, use the title of the base group
     if rs.group:
         lastUpdate = rs.group.lastUpdate.date().isoformat()
 
     # if there is only one lastUpdate / entry in the ImmutableResultSet, use its lastUpdate
@@ -103,27 +108,34 @@
     Returns title of ImmutableResultSet.  
     Returns the title of the base group (if exists) or the concatenated titles of all 
     members.
 
     Returns
     ----------
     title : str
-        Used for field <gmd:title>, not repeatable.
+
+        * ISO 19115: ``<gmd:title>``, not repeatable
+
+        * DataCite: ``<title>``
 
     """
+    title = ''
+
     # if a base group exists, use the title of the base group
     if rs.group:
         title = rs.group.title
 
     # if there is only one title / entry in the ImmutableResultSet, use its title
-    elif isinstance(rs.get('title'), str):
+    # also do this if title is None, as rs.group.title can be None
+    if isinstance(rs.get('title'), str) and not title:
         title = rs.get('title')
 
     # if there are more titles in ImmutableResultSet, a dict is returned, concatenate titles
-    elif isinstance(rs.get('title'), dict):
+    # also do this if title is None, as rs.group.title can be None
+    elif isinstance(rs.get('title'), dict) and not title:
         title = ''
         for i, _title in enumerate(rs.get('title').values()):
             title += f"Title {i+1}: {_title}\n"
     # TODO: sort titles?? sort everything? (like uuid) -> uuid as 'index'?
     return title
 
 
@@ -132,16 +144,19 @@
     Returns publication date of ImmutableResultSet.  
     Returns the title of the base group (if exists) or the latest value of publication of 
     all members.
 
     Returns
     ----------
     publication : str
-        Used for field <gmd:date> with <gmd:dateType> 'creation', 
-        str in ISO-datae-formate, not repeatable.
+        Character string in ISO-date-format, not repeatable.
+
+        * ISO 19115: ``<gmd:date>`` with ``<gmd:dateType>`` 'creation', 
+
+        * DataCite: ``<publicationYear>`` & ``<date dateType="Created">``
 
     """
     # if a base group exists, use the publication date of the base group
     if rs.group:
         publication = rs.group.publication.date().isoformat()
 
     # if there is only one publication / entry in the ImmutableResultSet, use its publication
@@ -159,15 +174,18 @@
     """
     Returns version number of ImmutableResultSet.  
     Returns the maximal version number of all members.
 
     Returns
     ----------
     version: int
-        Used for field <gmd:edition>, not repeatable.
+
+        * ISO 19115: ``<gmd:edition>``, not repeatable.
+
+        * DataCite: ``<version>``
 
     """
     # if there is only one version in the ImmutableResultSet, use it
     if isinstance(rs.get('version'), int):
         version = rs.get('version')
 
     # if there are more than one version in ImmutableResultSet, us latest
@@ -180,17 +198,21 @@
 def _get_authors(rs: ImmutableResultSet) -> List[Dict]:
     """
     Returns all authors and coauthors of the ImmutableResultSet.
 
     Returns
     ----------
     authors: list[dict]
-        Used for field <gmd:CI_ResponsibleParty>, list of dictionaries containing the 
-        information about authors: mandatory keys are `first_name`, `last_name` and
-        `organisation_name`, repeatable.
+        List of dictionaries containing information about authors: 
+        mandatory keys are ``first_name``, ``last_name`` and ``organisation_name``.
+
+        * ISO 19115: ``<gmd:CI_ResponsibleParty>``, repeatable.
+
+        * DataCite: ``<creators>`` & ``<contributor contributorType="ContactPerson">``, only 
+        first author in ``<contributors>``
 
     """
     # rs.get('authors') gives the first author and all coAuthors
     # if there is only one entry in the ImmutableResultSet, a list of authors is returned by rs.get('authors')
     if isinstance(rs.get('authors'), list):
         authors = []
         for author_dict in rs.get('authors'):
@@ -203,32 +225,35 @@
     # if there is more than one entry in the ImmutableResultSet, a entry_uuid-indexed dictionary of authors is returned
     elif isinstance(rs.get('authors'), dict):
         for entry_uuid, entry_authors in rs.get('authors').items():
             authors = []
             for author_dict in entry_authors:
                 authors.append(
                     {
-                    'first_name': author_dict['first_name'],
-                    'last_name': author_dict['last_name'],
-                    'organisation_name': author_dict['organisation_name']
+                    'first_name': author_dict.get('first_name'),
+                    'last_name': author_dict.get('last_name'),
+                    'organisation_name': author_dict.get('organisation_name')
                 })
     
     return authors
 
 
 def _get_abstract(rs: ImmutableResultSet) -> str:
     """
     Returns abstract of ImmutableResultSet.
     If there is more than one abstract in the ImmutableResultSet, abstracts are
     concatenated.
 
     Returns
     ----------
     abstract: str
-        Used for field <gmd:abstract>, not repeatable.
+
+        * ISO 19115: ``<gmd:abstract>``, not repeatable.
+
+        * DataCite: ``<description descriptionType="Abstract">``
 
     """
     abstract = ''
     # if there is only one entry in the ImmutableResultSet, use its abstract
     if isinstance(rs.get('abstract'), str):
         abstract = rs.get('abstract')
 
@@ -246,30 +271,85 @@
     Returns the details of the ImmutableResultSet.
     Details are currently written to XML as Markdown tables along the abstracts 
     of ImmutableResultSet members.
 
     Returns
     ----------
     details: list[str]
-        Details as a markdown table, currently also in field <gmd:abstract>, not repeatable.
+
+        * ISO 19115: ``<gmd:supplementalInformation>``, repeatable.
+
+    """
+    # create list with details_table for all entries in ImmutableResultSet
+    details_list = []
+
+    # if there is only one entry in the ImmutableResultSet, a list details is returned by rs.get('details')
+    if isinstance(rs.get('details'), list):
+        for detail_dict in rs.get('details'):
+            # nested details
+                if isinstance(detail_dict['value'], dict):
+                    # include top-level key of nested detail
+                    details_list.append(f"{detail_dict['key']}: nested")
+
+                    # go for nested details
+                    for k, v in detail_dict['value'].items():
+                        details_list.append(f"{detail_dict['key']}.{k}: {v}")
+                # flat details
+                else:
+                    details_list.append(f"{detail_dict['key']}: {detail_dict['value']}")
+
+    # if there are more than one entries in the ImmutableResultSet, a entry_uuid-indexed dictionary of details is returned
+    elif isinstance(rs.get('details'), dict):
+        for entry_uuid, entry_details_list in rs.get('details').items():
+            for detail_dict in entry_details_list:
+                # nested details
+                if isinstance(detail_dict['value'], dict):
+                    # include top-level key of nested detail
+                    details_list.append(f"{detail_dict['key']}: nested")
+
+                    # go for nested details
+                    for k, v in detail_dict['value'].items():
+                        details_list.append(f"{detail_dict['key']}.{k}: {v}")
+                # flat details
+                else:
+                    details_list.append(f"{detail_dict['key']}: {detail_dict['value']}")
+
+    # remove duplicate details, without changing the order (keep top level keys of nested details on top)
+    details_list = list(dict.fromkeys(details_list).keys())
+
+    return details_list
+
+
+def _get_details_table(rs: ImmutableResultSet) -> List[str]:
+    """
+    Returns the details of the ImmutableResultSet as markdown tables.
+    Details are written to XML as Markdown tables along the abstracts 
+    of ImmutableResultSet members.
+
+    Returns
+    ----------
+    details_tables: list[str]
+        Details as a markdown table.
+
+        * DataCite: ``<description descriptionType="Abstract">``
 
     """
     # create list with details_table for all entries in ImmutableResultSet
-    details = []
+    details_tables = []
     _details = {}
 
     # if there is only one entry in the ImmutableResultSet, a list details is returned by rs.get('authors')
     if isinstance(rs.get('details'), list):
         for detail_dict in rs.get('details'):
             # nested details
                 if isinstance(detail_dict['value'], dict):
                     # include top-level detail of nested detail
                     _details[detail_dict['key']] = detail_dict.copy()
                     _details[detail_dict['key']]['value'] = 'nested'
-                    
+
                     # remove unwanted key-value pairs
                     _details[detail_dict['key']] = {key: val for key, val in _details[detail_dict['key']].items() if key in ['value', 'key', 'entry_uuid', 'description']}
 
                     # go for nested details
                     for k, v in detail_dict['value'].items():
                         expand = {
                             f"{detail_dict['key']}.{k}": dict(
@@ -286,26 +366,26 @@
                     # remove unwanted key-value pairs
                     _details[detail_dict['key']] = {key: val for key, val in _details[detail_dict['key']].items() if key in ['value', 'key', 'entry_uuid', 'description']}
 
         # turn into a transposed dataframe
         df = pd.DataFrame(_details).T
 
         # append markdown table to details
-        details.append(df.to_markdown())
+        details_tables.append(df.to_markdown())
 
     # if there are more than one entries in the ImmutableResultSet, a entry_uuid-indexed dictionary of details is returned
     elif isinstance(rs.get('details'), dict):
         for entry_uuid, entry_details_list in rs.get('details').items():
             for detail_dict in entry_details_list:
                 # nested details
                 if isinstance(detail_dict['value'], dict):
                     # include top-level detail of nested detail
                     _details[detail_dict['key']] = detail_dict.copy()
                     _details[detail_dict['key']]['value'] = 'nested'
-                    
+
                     # remove unwanted key-value pairs
                     _details[detail_dict['key']] = {key: val for key, val in _details[detail_dict['key']].items() if key in ['value', 'key', 'entry_uuid', 'description']}
 
                     # go for nested details
                     for k, v in detail_dict['value'].items():
                         expand = {
                             f"{detail_dict['key']}.{k}": dict(
@@ -322,31 +402,35 @@
                     # remove unwanted key-value pairs
                     _details[detail_dict['key']] = {key: val for key, val in _details[detail_dict['key']].items() if key in ['value', 'key', 'entry_uuid', 'description']}
 
             # turn into a transposed dataframe
             df = pd.DataFrame(_details).T
 
             # append markdown table to details
-            details.append(df.to_markdown())
+            details_tables.append(df.to_markdown())
 
-    return details
+    return details_tables
 
 
 def _get_keywords(rs: ImmutableResultSet) -> List[Dict]:
     """
     Returns the keywords of the ImmutableResultSet.
     If the variables of the ImmutableResultSet are linked to a thesaurus, the thesaurus
     keywords are also returned along the keywords that are linked to the ImmutableResultSet
     members.
 
     Returns
     ----------
     keywords: list[dict]
-        Used for field <gmd:MD_Keywords>, list of dictionaries containing information about
-        associated keywords, mandatory keys are `full_path` and `thesaurusName`.
+        List of dictionaries containing information about associated keywords, mandatory 
+        keys are ``full_path`` and ``thesaurusName``.
+
+        * ISO 19115: ``<gmd:MD_Keywords>``
+
+        * DataCite: ``<subjects>``
 
     """
     keywords = []
 
     # go for keyword linked to variable first
     variable_dict = rs.get('variable')
 
@@ -410,16 +494,20 @@
 def _get_licenses(rs: ImmutableResultSet) -> List[Dict]:
     """
     Returns the licenses of the ImmutableResultSet.
 
     Returns
     ----------
     licenses: list[dict]
-        Used for field <gmd:resourceConstraints>, list of dictionaries containing information about
-        associated licenses, mandatory keys are `link` and `short_title`.
+        List of dictionaries containing information about associated licenses, 
+        mandatory keys are ``link`` and ``short_title``.
+
+        * ISO 19115: ``<gmd:resourceConstraints>``
+
+        * DataCite: ``<rightsList>``
 
     """
     licenses = []
     # if there is only one license in the ImmutableResultSet, there are no nested dicts
     if not any(isinstance(val, dict) for val in rs.get('license').values()):
         link = rs.get('license')['link']
         short_title = rs.get('license')['short_title']
@@ -439,35 +527,49 @@
                 'link': link,
                 'short_title': short_title
             })
 
     return licenses
 
 
-def _get_datasource_information(rs: ImmutableResultSet) -> Tuple[List[Dict], List[Dict], List[int]]:
+def _get_datasource_information(rs: ImmutableResultSet) -> Tuple[List[Dict], List[Dict], List[List[Tuple]], List[int]]:
     """
     Returns the temporal scales, the location as a bounding box and the spatial resolution 
     of the data of the ImmutableResultSet.
 
     Returns
     ----------
     temporal_scales: list[dict]
-        Used for field <gmd:temporalElement>, list of dictionaries containing information
-        about the temporal scale(s), mandatory keys are `temporal_extent_start`, 
-        `temporal_extent_end` and `temporal_resolution`, repeatable.
+        List of dictionaries containing information about the temporal scale(s), mandatory 
+        keys are ``temporal_extent_start``, 
+        ``temporal_extent_end`` and ``temporal_resolution``
+
+        * ISO 19115: ``<gmd:temporalElement>``,  repeatable.
+
     bbox_locations: list[dict]
-        Used for field <gmd:geographicElement>, list of dictionaries containing the support
-        points of the bounding box(es), mandatory keys are `min_lon`, `min_lat`, `max_lon`
-        and `max_lat`, repeatable.
+        List of dictionaries containing the support points of the bounding box(es), mandatory 
+        keys are ``min_lon``, ``min_lat``, ``max_lon`` and ``max_lat``.
+
+        * ISO 19115: ``<gmd:geographicElement>``, repeatable.
+
+        * DataCite: ``<geoLocationPoint>``, only used if not polygon_locations.
+
+    polygon_locations: list[list[tuple]]
+        List of tuples of Polygon coordinates.
+
+        * DataCite: ``<geoLocationPolygon>``
+
     spatial_resolutions: list[int]
-        Used for field <gmd:spatialResolution>, list of integers [m], repeatable.
+
+        * ISO 19115: ``<gmd:spatialResolution>``, list of integers [m], repeatable.
 
     """
     temporal_scales = []
     bbox_locations = []
+    polygon_locations = []
     spatial_resolutions = []
     # datasource can be empty / no datasource associated
     if not rs.get('datasource'):
         pass
     
     # if there is only one datasource in the ImmutableResultSet, use its values
     elif not all(isinstance(val, dict) for val in rs.get('datasource').values()):
@@ -482,23 +584,26 @@
 
             temporal_scales = [{
                 "temporal_extent_start": temporal_extent_start,
                 "temporal_extent_end": temporal_extent_end,
                 "temporal_resolution": temporal_resolution
                 }]
 
-        # spatial extent, always as a bounding box
+        # spatial extent, bounding box for ISO export, polygon for datacite export
         # go for spatial_scale in datasource first
         if 'spatial_scale' in rs.get('datasource').keys():
             location = rs.get('datasource')['spatial_scale']['extent']
             
             # convert wkt to shapely shape to infer coordinates
             P = shapely.wkt.loads(location)
+
+            # save polygon points for datacite export
+            polygon_locations.append(list(P.exterior.coords))
             
-            # get support points of polygon
+            # get bounding box points of polygon
             min_lon, min_lat = P.exterior.coords[0][0], P.exterior.coords[0][1]
             max_lon, max_lat = P.exterior.coords[2][0], P.exterior.coords[2][1]
             
             # save as list(dict)
             bbox_locations = [{'min_lon': min_lon, 'min_lat': min_lat, 'max_lon': max_lon, 'max_lat': max_lat}]
 
             # spatial_resolution
@@ -517,20 +622,23 @@
                 temporal_resolution = pd.to_timedelta(temporal_resolution).total_seconds()
 
                 temporal_scales.append({
                     "temporal_extent_start": temporal_extent_start,
                     "temporal_extent_end": temporal_extent_end,
                     "temporal_resolution": temporal_resolution
                 })
-            # spatial_scale / bbox_location & spatial_resolution
+            # spatial_scale / bbox_location, polygon_location & spatial_resolution
             if ds_dict.get('spatial_scale'):
                 location = ds_dict['spatial_scale']['extent']
         
                 # convert wkt to shapely shape to infer coordinates
                 P = shapely.wkt.loads(location)
+
+                # save polygon points for datacite export
+                polygon_locations.append(list(P.exterior.coords))
         
                 # get support points of polygon
                 min_lon, min_lat = P.exterior.coords[0][0], P.exterior.coords[0][1]
                 max_lon, max_lat = P.exterior.coords[2][0], P.exterior.coords[2][1]
                 
                 # save as list(dict)
                 bbox_locations.append({'min_lon': min_lon, 'min_lat': min_lat, 'max_lon': max_lon, 'max_lat': max_lat})
@@ -569,31 +677,31 @@
                 # append to bbox_location
                 bbox_locations.append({'min_lon': min_lon, 'min_lat': min_lat, 'max_lon': max_lon, 'max_lat': max_lat})
 
     # raise ValueError if location is neither specified in datasource.spatial_scale nor in Entry.location
     if not bbox_locations:
         raise ValueError("No location information associated with instance to be exported.")
 
-    return temporal_scales, bbox_locations, spatial_resolutions
+    return temporal_scales, bbox_locations, polygon_locations, spatial_resolutions
 
 
-def _parse_iso_information(entry_or_resultset: Union[Entry, ImmutableResultSet]) -> Dict:
+def _parse_export_information(entry_or_resultset: Union[Entry, ImmutableResultSet]) -> Dict:
     """
     Loads the ImmutableResultSet of the input Entry (if not already an ImmutableResultSet) 
-    and extracts the information necessary for ISO export.
+    and extracts the information necessary for ISO 19115 and DataCite export.
 
     Parameters
     ----------
     entry_or_resultset : Union[Entry, ImmutableResultSet]
         The entry instance to be exported
     
     Returns
     ----------
-    iso_input: dict
-        Dictionary of information 
+    export_information: dict
+        Dictionary of metadata information necessary to export metadata standards. 
 
     """
     if not isinstance(entry_or_resultset, ImmutableResultSet):
         # get ImmutableResultSet
         rs = ImmutableResultSet(entry_or_resultset)
     else:
         rs = entry_or_resultset
@@ -615,34 +723,38 @@
 
     # authors (last_name, first_name, organisation_name, role), always as list of dicts
     authors = _get_authors(rs)
 
     # abstract
     abstract = _get_abstract(rs)
 
-    # details_table, put details into field <abstract> as markdown table for now
+    # details
     details = _get_details(rs)
 
+    # details_tables
+    details_tables = _get_details_table(rs)
+
     # keywords (full_path, thesaurusName.title)
     keywords = _get_keywords(rs)
 
     ### licenses (link, short_title)
     licenses = _get_licenses(rs)
 
     ### datasource (spatial_scale.resolution, spatial_scale.extent/bbox_location, temporal_scale.extent, temporal_scale.resolution)
-    temporal_scales, bbox_locations, spatial_resolutions = _get_datasource_information(rs)
+    temporal_scales, bbox_locations, polygon_locations, spatial_resolutions = _get_datasource_information(rs)
 
-    # save everything in dict
-    iso_input = {
+    # save everything to dict
+    export_information = {
         'uuid': uuid, 'lastUpdate': lastUpdate, 'publication': publication, 'version': version, 'title': title, 
-        'authors': authors, 'abstract': abstract, 'details': details, 'keywords': keywords, 'licenses': licenses,
-        'temporal_scales': temporal_scales, 'bbox_locations': bbox_locations, 'spatial_resolutions': spatial_resolutions
+        'authors': authors, 'abstract': abstract, 'details': details, 'details_tables': details_tables,
+        'keywords': keywords, 'licenses': licenses, 'temporal_scales': temporal_scales, 
+        'bbox_locations': bbox_locations, 'polygon_locations': polygon_locations, 'spatial_resolutions': spatial_resolutions
         }
 
-    return iso_input
+    return export_information
 
 
 def _validate_xml(xml: str) -> bool:
     """
     Checks whether the input XML is well-formed (correct syntax).
     Currently, it is not checked whether the input XML is also a 
     valid ISO19115 XML.
```

### Comparing `metacatalog-0.8.2/metacatalog/models/__init__.py` & `metacatalog-0.8.3/metacatalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/models/config.py` & `metacatalog-0.8.3/metacatalog/models/config.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/models/datasource.py` & `metacatalog-0.8.3/metacatalog/models/datasource.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/models/details.py` & `metacatalog-0.8.3/metacatalog/models/details.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/models/entry.py` & `metacatalog-0.8.3/metacatalog/models/entry.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/models/entrygroup.py` & `metacatalog-0.8.3/metacatalog/models/entrygroup.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/models/generic_data.py` & `metacatalog-0.8.3/metacatalog/models/generic_data.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/models/geometry_data.py` & `metacatalog-0.8.3/metacatalog/models/geometry_data.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/models/keyword.py` & `metacatalog-0.8.3/metacatalog/models/keyword.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/models/license.py` & `metacatalog-0.8.3/metacatalog/models/license.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/models/person.py` & `metacatalog-0.8.3/metacatalog/models/person.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/models/timeseries.py` & `metacatalog-0.8.3/metacatalog/models/timeseries.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/models/timeseries_legacy.py` & `metacatalog-0.8.3/metacatalog/models/timeseries_legacy.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/models/variable.py` & `metacatalog-0.8.3/metacatalog/models/variable.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/__init__.py` & `metacatalog-0.8.3/metacatalog/test/__init__.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/_util.py` & `metacatalog-0.8.3/metacatalog/test/_util.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_api_add_find.py` & `metacatalog-0.8.3/metacatalog/test/test_api_add_find.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_api_install.py` & `metacatalog-0.8.3/metacatalog/test/test_api_install.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_api_location.py` & `metacatalog-0.8.3/metacatalog/test/test_api_location.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_array_type_data.py` & `metacatalog-0.8.3/metacatalog/test/test_array_type_data.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_cli_find.py` & `metacatalog-0.8.3/metacatalog/test/test_cli_find.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_db_migrations.py` & `metacatalog-0.8.3/metacatalog/test/test_db_migrations.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_export_extension.py` & `metacatalog-0.8.3/metacatalog/test/test_export_extension.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_groups_projects.py` & `metacatalog-0.8.3/metacatalog/test/test_groups_projects.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_logging.py` & `metacatalog-0.8.3/metacatalog/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_models_data.py` & `metacatalog-0.8.3/metacatalog/test/test_models_data.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_pg_install.py` & `metacatalog-0.8.3/metacatalog/test/test_pg_install.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_result_set.py` & `metacatalog-0.8.3/metacatalog/test/test_result_set.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_todict_fromdict.py` & `metacatalog-0.8.3/metacatalog/test/test_todict_fromdict.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/test/test_utility.py` & `metacatalog-0.8.3/metacatalog/test/test_utility.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/util/dict_functions.py` & `metacatalog-0.8.3/metacatalog/util/dict_functions.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/util/location.py` & `metacatalog-0.8.3/metacatalog/util/location.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/util/logging.py` & `metacatalog-0.8.3/metacatalog/util/logging.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog/util/results.py` & `metacatalog-0.8.3/metacatalog/util/results.py`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/metacatalog.egg-info/PKG-INFO` & `metacatalog-0.8.3/metacatalog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metacatalog
-Version: 0.8.2
+Version: 0.8.3
 Summary: Metadata model management module.
 Author: Mirko Mälicke
 Author-email: mirko.maelicke@kit.edu
 License: GPL v3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `metacatalog-0.8.2/metacatalog.egg-info/SOURCES.txt` & `metacatalog-0.8.3/metacatalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metacatalog-0.8.2/setup.py` & `metacatalog-0.8.3/setup.py`

 * *Files identical despite different names*

