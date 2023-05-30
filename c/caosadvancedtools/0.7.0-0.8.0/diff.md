# Comparing `tmp/caosadvancedtools-0.7.0.tar.gz` & `tmp/caosadvancedtools-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caosadvancedtools-0.7.0.tar", last modified: Thu Mar  9 13:39:06 2023, max compression
+gzip compressed data, was "caosadvancedtools-0.8.0.tar", last modified: Tue May 30 10:54:47 2023, max compression
```

## Comparing `caosadvancedtools-0.7.0.tar` & `caosadvancedtools-0.8.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-09 13:39:06.974143 caosadvancedtools-0.7.0/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    34283 2021-06-28 12:58:26.000000 caosadvancedtools-0.7.0/LICENSE.md
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2420 2023-03-09 13:39:06.974143 caosadvancedtools-0.7.0/PKG-INFO
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2102 2023-01-20 12:51:13.000000 caosadvancedtools-0.7.0/README.md
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      106 2023-03-09 13:39:06.974143 caosadvancedtools-0.7.0/setup.cfg
--rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6020 2023-03-09 08:58:02.000000 caosadvancedtools-0.7.0/setup.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-09 13:39:06.960809 caosadvancedtools-0.7.0/src/
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-09 13:39:06.967476 caosadvancedtools-0.7.0/src/caosadvancedtools/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-11-02 16:30:12.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/__init__.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-09 13:39:06.967476 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      159 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6576 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/bloxberg.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-09 13:39:06.967476 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1287 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/__init__.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-09 13:39:06.967476 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/api/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      195 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/api/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5531 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/api/certificate_api.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5282 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/api/pdf_api.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    24792 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/api_client.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     8020 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/configuration.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-09 13:39:06.970809 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/models/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      864 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/models/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7893 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/models/batch.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    12267 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_pdf_json_certificate.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13035 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_unsigned_certificate_json_certificate.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3184 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/models/http_validation_error.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4461 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/models/validation_error.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13216 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/rest.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13681 2022-10-11 12:58:29.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/cache.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    28487 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/cfood.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-09 13:39:06.970809 caosadvancedtools-0.7.0/src/caosadvancedtools/cfoods/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      873 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/cfoods/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    10328 2022-09-05 11:41:03.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/cfoods/h5.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3522 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/collect_datamodel.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-09 13:39:06.970809 caosadvancedtools-0.7.0/src/caosadvancedtools/converter/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-06-28 12:58:26.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/converter/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5903 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/converter/labfolder_api.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7147 2021-06-28 12:58:26.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/converter/labfolder_export.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    31129 2023-03-09 08:58:02.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/crawler.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1064 2021-11-02 16:30:12.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/datainconsistency.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3643 2021-11-02 16:30:12.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/datamodel_problems.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1605 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/example_cfood.py
--rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4885 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/export_related.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2079 2021-11-02 16:30:12.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/guard.py
--rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3629 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/import_from_xml.py
--rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    10427 2023-03-09 08:58:02.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/loadFiles.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-09 13:39:06.970809 caosadvancedtools-0.7.0/src/caosadvancedtools/models/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       47 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/models/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     9272 2023-01-20 12:51:13.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/models/data_model.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    30024 2022-09-05 11:41:03.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/models/parser.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7225 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/pandoc_header_tools.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3975 2021-06-28 12:58:26.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/read_md_header.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-09 13:39:06.974143 caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      273 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5287 2021-11-02 16:30:12.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/analysis_cfood.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3995 2022-07-15 11:33:25.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/experiment_cfood.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1528 2021-11-02 16:30:12.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/generic_pattern.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4433 2021-11-02 16:30:12.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/publication_cfood.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3620 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/result_table_cfood.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4738 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/simulation_cfood.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4779 2021-11-02 16:30:12.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/software_cfood.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6969 2021-11-02 16:30:12.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/utils.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    10013 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/withreadme.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-09 13:39:06.974143 caosadvancedtools-0.7.0/src/caosadvancedtools/serverside/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-11-02 16:30:12.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/serverside/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7145 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/serverside/generic_analysis.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13742 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/serverside/helper.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2381 2021-11-02 16:30:12.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/serverside/logging.py
--rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      217 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/serverside/sync.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4916 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/structure_mapping.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3135 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/suppressKnown.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3295 2021-06-28 12:58:26.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/table_converter.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    12578 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/table_export.py
--rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    16110 2022-06-14 14:35:20.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/table_importer.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7144 2023-03-09 08:58:02.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/utils.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      242 2023-03-09 13:39:05.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/version.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3400 2021-11-02 16:30:12.000000 caosadvancedtools-0.7.0/src/caosadvancedtools/webui_formatter.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-09 13:39:06.967476 caosadvancedtools-0.7.0/src/caosadvancedtools.egg-info/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2420 2023-03-09 13:39:06.000000 caosadvancedtools-0.7.0/src/caosadvancedtools.egg-info/PKG-INFO
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3186 2023-03-09 13:39:06.000000 caosadvancedtools-0.7.0/src/caosadvancedtools.egg-info/SOURCES.txt
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        1 2023-03-09 13:39:06.000000 caosadvancedtools-0.7.0/src/caosadvancedtools.egg-info/dependency_links.txt
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      158 2023-03-09 13:39:06.000000 caosadvancedtools-0.7.0/src/caosadvancedtools.egg-info/requires.txt
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       18 2023-03-09 13:39:06.000000 caosadvancedtools-0.7.0/src/caosadvancedtools.egg-info/top_level.txt
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    34283 2021-06-28 12:58:26.000000 caosadvancedtools-0.8.0/LICENSE.md
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2419 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/PKG-INFO
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2102 2023-01-20 12:51:13.000000 caosadvancedtools-0.8.0/README.md
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      106 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/setup.cfg
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6056 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/setup.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.959383 caosadvancedtools-0.8.0/src/
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.962716 caosadvancedtools-0.8.0/src/caosadvancedtools/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/__init__.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.962716 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      159 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6576 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/bloxberg.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.962716 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1287 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/__init__.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.962716 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      195 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5531 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api/certificate_api.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5282 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api/pdf_api.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    24792 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api_client.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     8020 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/configuration.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      864 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7893 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/batch.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    12267 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_pdf_json_certificate.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13035 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_unsigned_certificate_json_certificate.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3184 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/http_validation_error.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4461 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/validation_error.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13216 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/rest.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13688 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/cache.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    28483 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/cfood.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/src/caosadvancedtools/cfoods/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      873 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/cfoods/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    10328 2022-09-05 11:41:03.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/cfoods/h5.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3522 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/collect_datamodel.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/src/caosadvancedtools/converter/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-06-28 12:58:26.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/converter/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5903 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/converter/labfolder_api.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7147 2021-06-28 12:58:26.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/converter/labfolder_export.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    31105 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/crawler.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1064 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/datainconsistency.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3643 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/datamodel_problems.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1605 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/example_cfood.py
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4892 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/export_related.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2079 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/guard.py
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3629 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/import_from_xml.py
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    10427 2023-03-09 08:58:02.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/loadFiles.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/src/caosadvancedtools/models/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       47 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/models/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     9272 2023-01-20 12:51:13.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/models/data_model.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    36974 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/models/parser.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7225 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/pandoc_header_tools.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3975 2021-06-28 12:58:26.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/read_md_header.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      273 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5287 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/analysis_cfood.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3995 2022-07-15 11:33:25.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/experiment_cfood.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1528 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/generic_pattern.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4433 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/publication_cfood.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3620 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/result_table_cfood.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4738 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/simulation_cfood.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4779 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/software_cfood.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6965 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/utils.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    10013 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/withreadme.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7145 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/generic_analysis.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13742 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/helper.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2381 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/logging.py
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      217 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/sync.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4916 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/structure_mapping.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3135 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/suppressKnown.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3291 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/table_converter.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    12578 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/table_export.py
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    17103 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/table_importer.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7144 2023-03-09 08:58:02.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/utils.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      242 2023-05-30 10:54:47.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/version.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3400 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/webui_formatter.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.962716 caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2419 2023-05-30 10:54:47.000000 caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/PKG-INFO
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3186 2023-05-30 10:54:47.000000 caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/SOURCES.txt
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        1 2023-05-30 10:54:47.000000 caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/dependency_links.txt
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      165 2023-05-30 10:54:47.000000 caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/requires.txt
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       18 2023-05-30 10:54:47.000000 caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/top_level.txt
```

### Comparing `caosadvancedtools-0.7.0/LICENSE.md` & `caosadvancedtools-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/PKG-INFO` & `caosadvancedtools-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: caosadvancedtools
-Version: 0.7.0
+Version: 0.8.0
 Summary: advanced utilities for caosdb
 Author: Henrik tom Wörden
 Author-email: h.tomwoerden@indiscale.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: h5-crawler
-Provides-Extra: gitignore-parser 
+Provides-Extra: gitignore-parser
 License-File: LICENSE.md
 
 # README
 
 ## Welcome
 
 This is the **CaosDB Advanced User Tools** repository and a part of the
```

### Comparing `caosadvancedtools-0.7.0/README.md` & `caosadvancedtools-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/setup.py` & `caosadvancedtools-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 # DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 # THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ########################################################################
 
 MAJOR = 0
-MINOR = 7
+MINOR = 8
 MICRO = 0
 PRE = ""  # e.g. rc0, alpha.1, 0.beta-23
 ISRELEASED = True
 
 if PRE:
     VERSION = "{}.{}.{}-{}".format(MAJOR, MINOR, MICRO, PRE)
 else:
@@ -152,22 +152,23 @@
         description='advanced utilities for caosdb',
         long_description=long_description,
         long_description_content_type="text/markdown",
         author='Henrik tom Wörden',
         author_email='h.tomwoerden@indiscale.com',
         python_requires='>=3.7',
         install_requires=["caosdb>=0.11.0",
+                          "jsonref",
                           "jsonschema>=4.4.0",
                           "numpy>=1.17.3",
                           "openpyxl>=3.0.7",
                           "pandas>=1.2.0",
                           "xlrd>=2.0",
                           ],
         extras_require={"h5-crawler": ["h5py>=3.3.0", ],
-                        "gitignore-parser ": ["gitignore-parser >=0.1.0", ],
+                        "gitignore-parser": ["gitignore-parser >=0.1.0", ],
                         },
         packages=find_packages('src'),
         package_dir={'': 'src'},
         setup_requires=["pytest-runner>=2.0,<3dev"],
         tests_require=["pytest", "pytest-pythonpath", "pytest-cov", "coverage>=4.4.2"],
     )
     try:
```

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/bloxberg.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/bloxberg.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/__init__.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/api/certificate_api.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api/certificate_api.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/api/pdf_api.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api/pdf_api.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/api_client.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/configuration.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/models/__init__.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/models/batch.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/batch.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_pdf_json_certificate.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_pdf_json_certificate.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_unsigned_certificate_json_certificate.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_unsigned_certificate_json_certificate.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/models/http_validation_error.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/models/validation_error.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/bloxberg/swagger_client/rest.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/cache.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
     def get_previous_version(cont):
         """ Retrieve the current, unchanged version of the entities that shall
         be updated, i.e. the version before the update """
 
         old_ones = db.Container()
 
         for ent in cont:
-            old_ones.append(db.execute_query("FIND {}".format(ent.id),
+            old_ones.append(db.execute_query("FIND ENTITY {}".format(ent.id),
                                              unique=True))
 
         return old_ones
 
     def insert(self, cont, run_id, insert=False):
         """Insert a pending, unauthorized insert or update
```

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/cfood.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/cfood.py`

 * *Files 0% similar despite different names*

```diff
@@ -803,15 +803,15 @@
         for col in self.unique_cols:
             rec.add_property(col, self.item.loc[col])
         self.identifiables.append(rec)
 
     def update_identifiables(self):
         rec = self.identifiables[0]
 
-        for key, value in self.item.iteritems():
+        for key, value in self.item.items():
             if key in self.unique_cols:
                 continue
             assure_property_is(rec, key,
                                value,
                                to_be_updated=self.to_be_updated)
```

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/cfoods/__init__.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/cfoods/__init__.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/cfoods/h5.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/cfoods/h5.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/collect_datamodel.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/collect_datamodel.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/converter/labfolder_api.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/converter/labfolder_api.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/converter/labfolder_export.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/converter/labfolder_export.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/crawler.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,40 +208,39 @@
         all_updates = 0
         for _, _, _, new, _ in inserts:
             new_cont = db.Container()
             new_cont = new_cont.from_xml(new)
             new_cont.insert(unique=False)
             logger.info("Successfully inserted {} records!".format(len(new_cont)))
             all_inserts += len(new_cont)
-        logger.info("Finished with authorized updates.")
+        logger.info("Finished with authorized inserts.")
 
         changes = cache.get_updates(run_id)
 
         for _, _, old, new, _ in changes:
-            new_cont = db.Container()
-            new_cont = new_cont.from_xml(new)
+            new_cont = db.Container.from_xml(new)
             ids = []
-            tmp = []
+            tmp = db.Container()
             update_incomplete = False
             # remove duplicate entities
             for el in new_cont:
                 if el.id not in ids:
                     ids.append(el.id)
                     tmp.append(el)
                 else:
                     update_incomplete = True
             new_cont = tmp
-            if new[0].version:
+            if new_cont[0].version:
                 valids = db.Container()
                 nonvalids = db.Container()
 
                 for ent in new_cont:
                     remote_ent = db.Entity(id=ent.id).retrieve()
                     if ent.version == remote_ent.version:
-                        valids.append(remote_ent)
+                        valids.append(ent)
                     else:
                         update_incomplete = True
                         nonvalids.append(remote_ent)
                 valids.update(unique=False)
                 logger.info("Successfully updated {} records!".format(
                     len(valids)))
                 logger.info("{} Records were not updated because the version in the server "
```

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/datainconsistency.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/datainconsistency.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/datamodel_problems.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/datamodel_problems.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/example_cfood.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/example_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/export_related.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/export_related.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 def invert_ids(entities):
     apply_to_ids(entities, lambda x: x*-1)
 
 
 def export_related_to(rec_id, directory="."):
     if not isinstance(rec_id, int):
         raise ValueError("rec_id needs to be an integer")
-    ent = db.execute_query("FIND {}".format(rec_id), unique=True)
+    ent = db.execute_query("FIND ENTITY {}".format(rec_id), unique=True)
     cont = recursively_collect_related(ent)
     export(cont, directory=directory)
 
 
 def export(cont, directory="."):
     directory = os.path.abspath(directory)
     dl_dir = os.path.join(directory, "downloads")
```

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/guard.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/guard.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/import_from_xml.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/import_from_xml.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/loadFiles.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/loadFiles.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/models/data_model.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/models/data_model.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/models/parser.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/models/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,16 +31,17 @@
 and will be added with the respective importance. These properties can be
 RecordTypes or Properties and can be defined right there.
 Every Property or RecordType only needs to be defined once anywhere. When it is
 not defined, simply the name can be supplied with no value.
 Parents can be provided under the 'inherit_from_xxxx' keywords. The value needs
 to be a list with the names. Here, NO NEW entities can be defined.
 """
-import json
 import argparse
+import json
+import jsonref
 import re
 import sys
 import yaml
 
 from typing import List
 from warnings import warn
 
@@ -72,15 +73,16 @@
     "unit",
 ]
 
 JSON_SCHEMA_ATOMIC_TYPES = [
     "string",
     "boolean",
     "integer",
-    "number"
+    "number",
+    "null"
 ]
 
 
 def _get_listdatatype(dtype):
     """matches a string to check whether the type definition is a list
 
     returns the type within the list or None, if it cannot be matched with a
@@ -148,21 +150,37 @@
 def parse_model_from_string(string):
     """Shortcut if the Parser object is not needed."""
     parser = Parser()
 
     return parser.parse_model_from_string(string)
 
 
-def parse_model_from_json_schema(filename: str):
+def parse_model_from_json_schema(
+        filename: str,
+        top_level_recordtype: bool = True,
+        types_for_missing_array_items: dict = {},
+        ignore_unspecified_array_items: bool = False
+):
     """Return a datamodel parsed from a json schema definition.
 
     Parameters
     ----------
     filename : str
         The path of the json schema file that is to be parsed
+    top_level_recordtype : bool, optional
+        Whether there is a record type defined at the top level of the
+        schema. Default is true.
+    types_for_missing_array_items : dict, optional
+        dictionary containing fall-back types for json entries with `type:
+        array` but without `items` specification. Default is an empty dict.
+    ignore_unspecified_array_items : bool, optional
+        Whether to ignore `type: array` entries the type of which is not
+        specified by their `items` property or given in
+        `types_for_missing_array_items`. An error is raised if they are not
+        ignored. Default is False.
 
     Returns
     -------
     out : Datamodel
         The datamodel generated from the input schema which then can be used for
         synchronizing with CaosDB.
 
@@ -170,18 +188,18 @@
     ----
     This is an experimental feature, see ``JsonSchemaParser`` for information
     about the limitations of the current implementation.
 
     """
     # @author Florian Spreckelsen
     # @date 2022-02-17
-    # @review Daniel Hornung 2022-02-18
-    parser = JsonSchemaParser()
+    # @review Timm Fitschen 2023-05-25
+    parser = JsonSchemaParser(types_for_missing_array_items, ignore_unspecified_array_items)
 
-    return parser.parse_model_from_json_schema(filename)
+    return parser.parse_model_from_json_schema(filename, top_level_recordtype)
 
 
 class Parser(object):
     def __init__(self):
         """Initialize an empty parser object and initialize the dictionary of entities and the list of
         treated elements.
 
@@ -254,17 +272,17 @@
             ymlmodel["extern"] = []
 
         for name in ymlmodel["extern"]:
             if name in CAOSDB_INTERNAL_PROPERTIES:
                 self.model[name] = db.Property(name=name).retrieve()
                 continue
             for role in ("Property", "RecordType", "Record", "File"):
-                if db.execute_query("COUNT {} {}".format(role, name)) > 0:
+                if db.execute_query("COUNT {} \"{}\"".format(role, name)) > 0:
                     self.model[name] = db.execute_query(
-                        "FIND {} WITH name={}".format(role, name), unique=True)
+                        f"FIND {role} WITH name=\"{name}\"", unique=True)
                     break
             else:
                 raise Exception("Did not find {}".format(name))
 
         ymlmodel.pop("extern")
 
         # add all names to ymlmodel; initialize properties
@@ -596,130 +614,176 @@
             if value is None:
                 self.model[key] = db.RecordType(name=key)
 
 
 class JsonSchemaParser(Parser):
     """Extends the yaml parser to read in datamodels defined in a json schema.
 
-    **EXPERIMENTAL:** While this calss can already be used to create data models
+    **EXPERIMENTAL:** While this class can already be used to create data models
     from basic json schemas, there are the following limitations and missing
     features:
 
     * Due to limitations of json-schema itself, we currently do not support
       inheritance in the imported data models
     * The same goes for suggested properties of RecordTypes
-    * Currently, ``$defs`` and ``$ref`` in the input schema are not resolved.
     * Already defined RecordTypes and (scalar) Properties can't be re-used as
       list properties
     * Reference properties that are different from the referenced RT. (Although
       this is possible for list of references)
     * Values
     * Roles
     * The extern keyword from the yaml parser
-    * Currently, a json-schema cannot be transformed into a data model if its
-      root element isn't a RecordType (or Property) with ``title`` and ``type``.
 
     """
     # @author Florian Spreckelsen
     # @date 2022-02-17
-    # @review Timm Fitschen 2022-02-30
+    # @review Timm Fitschen 2023-05-25
 
-    def parse_model_from_json_schema(self, filename: str):
+    def __init__(self, types_for_missing_array_items={}, ignore_unspecified_array_items=False):
+        super().__init__()
+        self.types_for_missing_array_items = types_for_missing_array_items
+        self.ignore_unspecified_array_items = ignore_unspecified_array_items
+
+    def parse_model_from_json_schema(self, filename: str, top_level_recordtype: bool = True):
         """Return a datamodel created from the definition in the json schema in
         `filename`.
 
         Parameters
         ----------
         filename : str
             The path to the json-schema file containing the datamodel definition
+        top_level_recordtype : bool, optional
+            Whether there is a record type defined at the top level of the
+            schema. Default is true.
 
         Returns
         -------
         out : DataModel
             The created DataModel
         """
         # @author Florian Spreckelsen
         # @date 2022-02-17
-        # @review Timm Fitschen 2022-02-30
+        # @review Timm Fitschen 2023-05-25
         with open(filename, 'r') as schema_file:
-            model_dict = json.load(schema_file)
+            model_dict = jsonref.load(schema_file)
 
-        return self._create_model_from_dict(model_dict)
+        return self._create_model_from_dict(model_dict, top_level_recordtype=top_level_recordtype)
 
-    def _create_model_from_dict(self, model_dict: [dict, List[dict]]):
+    def _create_model_from_dict(self, model_dict: [dict, List[dict]], top_level_recordtype: bool = True):
         """Parse a dictionary and return the Datamodel created from it.
 
         The dictionary was typically created from the model definition in a json schema file.
 
         Parameters
         ----------
         model_dict : dict or list[dict]
             One or several dictionaries read in from a json-schema file
+        top_level_recordtype : bool, optional
+            Whether there is a record type defined at the top level of the
+            schema. Default is true.
 
         Returns
         -------
         our : DataModel
             The datamodel defined in `model_dict`
         """
-        # @review Timm Fitschen 2022-02-30
+        # @review Timm Fitschen 2023-05-25
         if isinstance(model_dict, dict):
             model_dict = [model_dict]
 
         for ii, elt in enumerate(model_dict):
-            if "title" not in elt:
-                raise JsonSchemaDefinitionError(
-                    f"Object {ii+1} is lacking the `title` key word")
-            if "type" not in elt:
-                raise JsonSchemaDefinitionError(
-                    f"Object {ii+1} is lacking the `type` key word")
-            # Check if this is a valid Json Schema
             try:
                 jsonschema.Draft202012Validator.check_schema(elt)
             except jsonschema.SchemaError as err:
+                key = elt["title"] if "title" in elt else f"element {ii}"
                 raise JsonSchemaDefinitionError(
-                    f"Json Schema error in {elt['title']}:\n{str(err)}") from err
-            name = self._stringify(elt["title"], context=elt)
-            self._treat_element(elt, name)
+                    f"Json Schema error in {key}:\n{str(err)}") from err
+
+            if top_level_recordtype:
+                if "title" not in elt:
+                    raise JsonSchemaDefinitionError(
+                        f"Object {ii+1} is lacking the `title` key word")
+                if "type" not in elt:
+                    raise JsonSchemaDefinitionError(
+                        f"Object {ii+1} is lacking the `type` key word")
+                # Check if this is a valid Json Schema
+                name = self._stringify(elt["title"], context=elt)
+                self._treat_element(elt, name)
+            elif "properties" in elt or "patternProperties" in elt:
+                # No top-level type but there are entities
+                if "properties" in elt:
+                    for key, prop in elt["properties"].items():
+                        name = self._get_name_from_property(key, prop)
+                        self._treat_element(prop, name)
+                if "patternProperties" in elt:
+                    # See also treatment in ``_treat_record_type``. Since here,
+                    # there is no top-level RT we use the prefix `__Pattern`,
+                    # i.e., the resulting Record Types will be called
+                    # `__PatternElement`.
+                    self._treat_pattern_properties(
+                        elt["patternProperties"], name_prefix="__Pattern")
+            else:
+                # Neither RecordType itself, nor further properties in schema,
+                # so nothing to do here. Maybe add something in the future.
+                continue
 
         return DataModel(self.model.values())
 
+    def _get_name_from_property(self, key: str, prop: dict):
+        # @review Timm Fitschen 2023-05-25
+        if "title" in prop:
+            name = self._stringify(prop["title"])
+        else:
+            name = self._stringify(key)
+
+        return name
+
     def _get_atomic_datatype(self, elt):
-        # @review Timm Fitschen 2022-02-30
+        # @review Timm Fitschen 2023-05-25
         if elt["type"] == "string":
             if "format" in elt and elt["format"] in ["date", "date-time"]:
                 return db.DATETIME
             else:
                 return db.TEXT
         elif elt["type"] == "integer":
             return db.INTEGER
         elif elt["type"] == "number":
             return db.DOUBLE
         elif elt["type"] == "boolean":
             return db.BOOLEAN
+        elif elt["type"] == "null":
+            # This could be any datatype since a valid json will never have a
+            # value in a null property. We use TEXT for convenience.
+            return db.TEXT
         else:
             raise JsonSchemaDefinitionError(f"Unkown atomic type in {elt}.")
 
     def _treat_element(self, elt: dict, name: str):
-        # @review Timm Fitschen 2022-02-30
+        # @review Timm Fitschen 2023-05-25
         force_list = False
         if name in self.model:
             return self.model[name], force_list
         if "type" not in elt:
             # Each element must have a specific type
             raise JsonSchemaDefinitionError(
                 f"`type` is missing in element {name}.")
         if name == "name":
             # This is identified with the CaosDB name property as long as the
             # type is correct.
-            if not elt["type"] == "string":
+            if not elt["type"] == "string" and "string" not in elt["type"]:
                 raise JsonSchemaDefinitionError(
                     "The 'name' property must be string-typed, otherwise it cannot "
                     "be identified with CaosDB's name property."
                 )
             return None, force_list
+        # LinkAhead suports null for all types, so in the very special case of
+        # `"type": ["null", "<other_type>"]`, only consider the other type:
+        if isinstance(elt["type"], list) and len(elt["type"]) == 2 and "null" in elt["type"]:
+            elt["type"].remove("null")
+            elt["type"] = elt["type"][0]
         if "enum" in elt:
             ent = self._treat_enum(elt, name)
         elif elt["type"] in JSON_SCHEMA_ATOMIC_TYPES:
             ent = db.Property(
                 name=name, datatype=self._get_atomic_datatype(elt))
         elif elt["type"] == "object":
             ent = self._treat_record_type(elt, name)
@@ -729,43 +793,52 @@
             raise NotImplementedError(
                 f"Cannot parse items of type '{elt['type']}' (yet).")
         if "description" in elt and ent.description is None:
             # There is a description and it hasn't been set by another
             # treat_something function
             ent.description = elt["description"]
 
-        self.model[name] = ent
+        if ent is not None:
+            self.model[name] = ent
         return ent, force_list
 
     def _treat_record_type(self, elt: dict, name: str):
-        # @review Timm Fitschen 2022-02-30
+        # @review Timm Fitschen 2023-05-25
         rt = db.RecordType(name=name)
         if "required" in elt:
             required = elt["required"]
         else:
             required = []
         if "properties" in elt:
             for key, prop in elt["properties"].items():
-                if "title" in prop:
-                    name = self._stringify(prop["title"])
-                else:
-                    name = self._stringify(key)
+                name = self._get_name_from_property(key, prop)
                 prop_ent, force_list = self._treat_element(prop, name)
                 if prop_ent is None:
                     # Nothing to be appended since the property has to be
                     # treated specially.
                     continue
                 importance = db.OBLIGATORY if key in required else db.RECOMMENDED
                 if not force_list:
                     rt.add_property(prop_ent, importance=importance)
                 else:
                     # Special case of rt used as a list property
                     rt.add_property(prop_ent, importance=importance,
                                     datatype=db.LIST(prop_ent))
 
+        if "patternProperties" in elt:
+
+            pattern_property_rts = self._treat_pattern_properties(
+                elt["patternProperties"], name_prefix=name)
+            for ppr in pattern_property_rts:
+                # add reference to pattern property type. These can never be
+                # obligatory since pattern properties cannot be required in the
+                # original schema (since their actual names are not known a
+                # priori).
+                rt.add_property(ppr)
+
         if "description" in elt:
             rt.description = elt["description"]
         return rt
 
     def _treat_enum(self, elt: dict, name: str):
         # @review Timm Fitschen 2022-02-30
         if "type" in elt and elt["type"] == "integer":
@@ -779,36 +852,104 @@
             rec = db.Record(name=self._stringify(enum_elt))
             rec.add_parent(rt)
             self.model[enum_elt] = rec
 
         return rt
 
     def _treat_list(self, elt: dict, name: str):
-        # @review Timm Fitschen 2022-02-30
+        # @review Timm Fitschen 2023-05-25
 
-        if "items" not in elt:
+        if "items" not in elt and name not in self.types_for_missing_array_items:
+            if self.ignore_unspecified_array_items:
+                return None, False
             raise JsonSchemaDefinitionError(
                 f"The definition of the list items is missing in {elt}.")
-        items = elt["items"]
-        if "enum" in items:
-            return self._treat_enum(items, name), True
-        if items["type"] in JSON_SCHEMA_ATOMIC_TYPES:
-            datatype = db.LIST(self._get_atomic_datatype(items))
+        if "items" in elt:
+            items = elt["items"]
+            if "enum" in items:
+                return self._treat_enum(items, name), True
+            if items["type"] in JSON_SCHEMA_ATOMIC_TYPES:
+                datatype = db.LIST(self._get_atomic_datatype(items))
+                return db.Property(name=name, datatype=datatype), False
+            if items["type"] == "object":
+                if "title" not in items or self._stringify(items["title"]) == name:
+                    # Property is RecordType
+                    return self._treat_record_type(items, name), True
+                else:
+                    # List property will be an entity of its own with a name
+                    # different from the referenced RT
+                    ref_rt = self._treat_record_type(
+                        items, self._stringify(items["title"]))
+                    self.model[ref_rt.name] = ref_rt
+                    return db.Property(name=name, datatype=db.LIST(ref_rt)), False
+        else:
+            # Use predefined type:
+            datatype = db.LIST(self.types_for_missing_array_items[name])
             return db.Property(name=name, datatype=datatype), False
-        if items["type"] == "object":
-            if "title" not in items or self._stringify(items["title"]) == name:
-                # Property is RecordType
-                return self._treat_record_type(items, name), True
+
+    def _get_pattern_prop(self):
+        # @review Timm Fitschen 2023-05-25
+        if "__pattern_property_pattern_property" in self.model:
+            return self.model["__pattern_property_pattern_property"]
+        pp = db.Property(name="__matched_pattern", datatype=db.TEXT)
+        self.model["__pattern_property_pattern_property"] = pp
+        return pp
+
+    def _treat_pattern_properties(self, pattern_elements, name_prefix=""):
+        """Special Treatment for pattern properties: A RecordType is created for
+        each pattern property. In case of a `type: object` PatternProperty, the
+        remaining properties of the JSON entry are appended to the new
+        RecordType; in case of an atomic type PatternProperty, a single value
+        Property is added to the RecordType.
+
+        Raises
+        ------
+        NotImplementedError
+            In case of patternProperties with non-object, non-atomic type, e.g.,
+            array.
+
+        """
+        # @review Timm Fitschen 2023-05-25
+        num_patterns = len(pattern_elements)
+        pattern_prop = self._get_pattern_prop()
+        returns = []
+        for ii, (key, element) in enumerate(pattern_elements.items()):
+            if "title" not in element:
+                name_suffix = f"_{ii+1}" if num_patterns > 1 else ""
+                name = name_prefix + "Entry" + name_suffix
+            else:
+                name = element["title"]
+            if element["type"] == "object":
+                # simple, is already an object, so can be treated like any other
+                # record type.
+                pattern_type = self._treat_record_type(element, name)
+            elif element["type"] in JSON_SCHEMA_ATOMIC_TYPES:
+                # create a property that stores the actual value of the pattern
+                # property.
+                propname = f"{name}_value"
+                prop = db.Property(name=propname, datatype=self._get_atomic_datatype(element))
+                self.model[propname] = prop
+                pattern_type = db.RecordType(name=name)
+                pattern_type.add_property(prop)
+            else:
+                raise NotImplementedError(
+                    "Pattern properties are currently only supported for types " +
+                    ", ".join(JSON_SCHEMA_ATOMIC_TYPES) + ", and object.")
+
+            # Add pattern property and description
+            pattern_type.add_property(pattern_prop, importance=db.OBLIGATORY)
+            if pattern_type.description:
+                pattern_type.description += f"\n\npattern: {key}"
             else:
-                # List property will be an entity of its own with a name
-                # different from the referenced RT
-                ref_rt = self._treat_record_type(
-                    items, self._stringify(items["title"]))
-                self.model[ref_rt.name] = ref_rt
-                return db.Property(name=name, datatype=db.LIST(ref_rt)), False
+                pattern_type.description = f"pattern: {key}"
+
+            self.model[name] = pattern_type
+            returns.append(pattern_type)
+
+        return returns
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description=__doc__,
                                      formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument("data_model",
                         help="Path name of the data model file (yaml or json) to be used.")
```

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/pandoc_header_tools.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/pandoc_header_tools.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/read_md_header.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/read_md_header.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/analysis_cfood.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/analysis_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/experiment_cfood.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/experiment_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/generic_pattern.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/publication_cfood.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/publication_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/result_table_cfood.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/result_table_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/simulation_cfood.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/simulation_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/software_cfood.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/software_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/utils.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                                      datatype=db.LIST(db.REFERENCE))
 
 
 def create_files_list(df, ftype):
     files = []
 
     for indx, src in df.loc[ftype,
-                            pd.notnull(df.loc[ftype])].iteritems():
+                            pd.notnull(df.loc[ftype])].items():
         desc = df.loc[ftype+" description", indx]
 
         if pd.notnull(desc):
             files.append({'file': src, 'description': desc})
         else:
             files.append(src)
```

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/scifolder/withreadme.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/withreadme.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/serverside/generic_analysis.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/generic_analysis.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/serverside/helper.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/helper.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/serverside/logging.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/logging.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/structure_mapping.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/structure_mapping.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/suppressKnown.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/suppressKnown.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/table_converter.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/table_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     """ parses a pandas DataFrame to a list of records """
     records = db.Container()
 
     for idx, row in spreadsheet.iterrows():
         rec = db.Record()
         rec.add_parent(name=recordtype)
 
-        for key, value in row.iteritems():
+        for key, value in row.items():
             if key.lower() == "description":
                 rec.description = value
                 continue
 
             if (pd.notnull(value) and
                     (not isinstance(value, str) or value.strip() != "")):
                 regexp = r"(.*)\[(.*)\].*"
```

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/table_export.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/table_export.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/table_importer.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/table_importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -206,52 +206,61 @@
 
 
 class TableImporter():
     """Abstract base class for importing data from tables.
     """
 
     def __init__(self, converters, obligatory_columns=None, unique_keys=None,
-                 datatypes=None):
+                 datatypes=None, existing_columns=None):
         """
         Parameters
         ----------
         converters : dict
           Dict with column names as keys and converter functions as values. This dict also defines
           what columns are required to exist throught the existing keys. The converter functions are
           applied to the cell values. They should also check for ValueErrors, such that a separate
           value check is not necessary.
 
         obligatory_columns : list, optional
-          List of column names, each listed column must not have missing values.
+          List of column names that (if they exist) must not have missing values.
 
         unique_keys : list, optional
           List of column names that in combination must be unique: each row has a unique
           combination of values in those columns.
 
         datatypes : dict, optional
           Dict with column names as keys and datatypes as values.  All non-null values will be
           checked whether they have the provided datatype.  This dict also defines what columns are
           required to exist throught the existing keys.
 
+        existing_columns : list, optional
+          List of column names that must exist but may have missing (NULL) values
         """
 
         if converters is None:
             converters = {}
+        self.converters = converters
+
+        if obligatory_columns is None:
+            obligatory_columns = []
+        self.obligatory_columns = obligatory_columns
+
+        if unique_keys is None:
+            unique_keys = []
+        self.unique_keys = unique_keys
 
         if datatypes is None:
             datatypes = {}
+        self.datatypes = datatypes
+
+        if existing_columns is None:
+            existing_columns = []
+        self.existing_columns = existing_columns
 
         self.sup = SuppressKnown()
-        self.required_columns = list(converters.keys())+list(datatypes.keys())
-        self.obligatory_columns = ([]
-                                   if obligatory_columns is None
-                                   else obligatory_columns)
-        self.unique_keys = [] if unique_keys is None else unique_keys
-        self.converters = converters
-        self.datatypes = datatypes
 
     def read_file(self, filename, **kwargs):
         raise NotImplementedError()
 
     def check_columns(self, df, filename=None):
         """Check whether all required columns exist.
 
@@ -259,15 +268,15 @@
 
         Raises
         ------
         DataInconsistencyError
 
         """
 
-        for col in self.required_columns:
+        for col in self.existing_columns:
             if col not in df.columns:
                 errmsg = "Column '{}' missing in ".format(col)
                 errmsg += ("\n{}.\n".format(filename) if filename
                            else "the file.")
                 errmsg += "Stopping to treat this file..."
                 logger.warning(
                     errmsg,
@@ -319,26 +328,27 @@
         ----------
 
         strict: boolean, optional
           If False (the default), try to convert columns, otherwise raise an error.
 
         """
         for key, datatype in self.datatypes.items():
+            if key not in df.columns:
+                continue
             # Check for castable numeric types first: We unconditionally cast int to the default
             # float, because CaosDB does not have different sizes anyway.
             col_dtype = df.dtypes[key]
             if not strict and not np.issubdtype(col_dtype, datatype):
                 issub = np.issubdtype
                 #  These special cases should be fine.
                 if issub(col_dtype, np.integer) and issub(datatype, np.floating):
                     df[key] = df[key].astype(datatype)
 
             # Now check each element
-            for idx, val in df.loc[
-                    pd.notnull(df.loc[:, key]), key].iteritems():
+            for idx, val in df.loc[pd.notnull(df.loc[:, key]), key].items():
 
                 if not isinstance(val, datatype):
                     msg = (
                         "In row no. {rn} and column '{c}' of file '{fi}' the "
                         "datatype was {was} but it should be "
                         "{expected}".format(rn=idx, c=key, fi=filename,
                                             was=str(type(val)).strip("<>"),
@@ -359,30 +369,28 @@
         out : pandas.DataFrame
           The input DataFrame with incomplete rows removed.
         """
         df = df.copy()
 
         for index, row in df.iterrows():
             # if none of the relevant information is given, skip
-
-            if np.array([pd.isnull(row.loc[key]) for key in
-                         self.obligatory_columns]).all():
-
+            if pd.isnull(row.loc[[key for key in self.obligatory_columns if key in df.columns]]).all():
                 df = df.drop(index)
 
                 continue
 
             # if any of the relevant information is missing, report it
-
             i = 0
             okay = True
 
             while okay and i < len(self.obligatory_columns):
                 key = self.obligatory_columns[i]
                 i += 1
+                if key not in df.columns:
+                    continue
 
                 if pd.isnull(row.loc[key]):
                     errmsg = (
                         "Required information is missing ({}) in {}. row"
                         " (without header) of "
                         "file:\n{}".format(key, index+1, filename))
 
@@ -445,15 +453,18 @@
         if len(xls_file.sheet_names) > 1:
             # Multiple sheets is the default now. Only show in debug
             logger.debug(
                 "Excel file {} contains multiple sheets. "
                 "All but the first are being ignored.".format(filename))
 
         try:
-            df = xls_file.parse(converters=self.converters, **kwargs)
+            tmpdf = xls_file.parse(**kwargs)
+            applicable_converters = {k: v for k, v in self.converters.items()
+                                     if k in tmpdf.columns}
+            df = xls_file.parse(converters=applicable_converters, **kwargs)
         except Exception as e:
             logger.warning(
                 "Cannot parse {}.\n{}".format(filename, e),
                 extra={'identifier': str(filename),
                        'category': "inconsistency"})
             raise DataInconsistencyError(*e.args)
 
@@ -461,15 +472,19 @@
 
         return df
 
 
 class CSVImporter(TableImporter):
     def read_file(self, filename, sep=",", **kwargs):
         try:
-            df = pd.read_csv(filename, sep=sep, converters=self.converters,
+            tmpdf = pd.read_csv(filename, sep=sep, converters=self.converters,
+                                **kwargs)
+            applicable_converters = {k: v for k, v in self.converters.items()
+                                     if k in tmpdf.columns}
+            df = pd.read_csv(filename, sep=sep, converters=applicable_converters,
                              **kwargs)
         except ValueError as ve:
             logger.warning(
                 "Cannot parse {}.\n{}".format(filename, ve),
                 extra={'identifier': str(filename),
                        'category': "inconsistency"})
             raise DataInconsistencyError(*ve.args)
@@ -478,14 +493,18 @@
 
         return df
 
 
 class TSVImporter(TableImporter):
     def read_file(self, filename, **kwargs):
         try:
+            tmpdf = pd.read_csv(filename, sep="\t", converters=self.converters,
+                                **kwargs)
+            applicable_converters = {k: v for k, v in self.converters.items()
+                                     if k in tmpdf.columns}
             df = pd.read_csv(filename, sep="\t", converters=self.converters,
                              **kwargs)
         except ValueError as ve:
             logger.warning(
                 "Cannot parse {}.\n{}".format(filename, ve),
                 extra={'identifier': str(filename),
                        'category': "inconsistency"})
```

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/utils.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/utils.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools/webui_formatter.py` & `caosadvancedtools-0.8.0/src/caosadvancedtools/webui_formatter.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools.egg-info/PKG-INFO` & `caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: caosadvancedtools
-Version: 0.7.0
+Version: 0.8.0
 Summary: advanced utilities for caosdb
 Author: Henrik tom Wörden
 Author-email: h.tomwoerden@indiscale.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: h5-crawler
-Provides-Extra: gitignore-parser 
+Provides-Extra: gitignore-parser
 License-File: LICENSE.md
 
 # README
 
 ## Welcome
 
 This is the **CaosDB Advanced User Tools** repository and a part of the
```

### Comparing `caosadvancedtools-0.7.0/src/caosadvancedtools.egg-info/SOURCES.txt` & `caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

