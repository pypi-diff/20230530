# Comparing `tmp/file-name-attributes-0.2.4.tar.gz` & `tmp/file-name-attributes-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file-name-attributes-0.2.4.tar", last modified: Sat May 27 15:17:26 2023, max compression
+gzip compressed data, was "file-name-attributes-0.2.5.tar", last modified: Tue May 30 12:38:22 2023, max compression
```

## Comparing `file-name-attributes-0.2.4.tar` & `file-name-attributes-0.2.5.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-06 18:55:15.000000 file-name-attributes-0.2.4/LICENSE
--rw-rw-r--   0 kevin     (1001) dialout     (20)       31 2023-05-07 00:42:08.000000 file-name-attributes-0.2.4/MANIFEST.in
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5434 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4769 2023-05-25 13:38:58.000000 file-name-attributes-0.2.4/README.md
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/config/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      873 2023-05-06 03:24:15.000000 file-name-attributes-0.2.4/config/config.toml
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/doc/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2059 2023-05-22 21:45:38.000000 file-name-attributes-0.2.4/doc/configuration.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)    10407 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/doc/fna.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4121 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/doc/keys.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4432 2023-05-26 19:58:41.000000 file-name-attributes-0.2.4/pyproject.toml
--rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/setup.cfg
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/extra/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4899 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/extra/fnaffle.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4378 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/extra/make_isbn_ranges.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/file_name_attributes.egg-info/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5434 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/file_name_attributes.egg-info/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2354 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/file_name_attributes.egg-info/SOURCES.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/file_name_attributes.egg-info/dependency_links.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)       62 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/file_name_attributes.egg-info/entry_points.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)       34 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/file_name_attributes.egg-info/top_level.txt
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/fna/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3415 2023-05-22 16:11:49.000000 file-name-attributes-0.2.4/src/fna/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/util/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-22 16:12:06.000000 file-name-attributes-0.2.4/src/util/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      778 2023-05-21 18:37:39.000000 file-name-attributes-0.2.4/src/util/checksum.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      716 2023-05-21 18:37:58.000000 file-name-attributes-0.2.4/src/util/checksum_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3648 2023-05-21 20:02:21.000000 file-name-attributes-0.2.4/src/util/config.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5367 2023-05-22 13:18:46.000000 file-name-attributes-0.2.4/src/util/config_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      625 2023-05-21 19:00:38.000000 file-name-attributes-0.2.4/src/util/docsplit.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      707 2023-05-22 16:03:59.000000 file-name-attributes-0.2.4/src/util/docsplit_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     9038 2023-05-26 20:01:56.000000 file-name-attributes-0.2.4/src/util/duration.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5525 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/src/util/duration_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      102 2023-05-22 16:04:07.000000 file-name-attributes-0.2.4/src/util/error.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2181 2023-05-21 19:04:05.000000 file-name-attributes-0.2.4/src/util/escape.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2912 2023-05-21 18:38:18.000000 file-name-attributes-0.2.4/src/util/escape_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      926 2023-05-21 19:04:45.000000 file-name-attributes-0.2.4/src/util/fearmat.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      710 2023-05-06 18:49:53.000000 file-name-attributes-0.2.4/src/util/fearmat_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1857 2023-05-22 16:13:43.000000 file-name-attributes-0.2.4/src/util/io.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2033 2023-05-21 20:01:59.000000 file-name-attributes-0.2.4/src/util/io_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3535 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/util/multimap.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4661 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/util/multimap_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1063 2023-05-22 16:04:25.000000 file-name-attributes-0.2.4/src/util/pytestutil.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1738 2023-05-22 16:05:14.000000 file-name-attributes-0.2.4/src/util/registry.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      849 2023-05-21 18:38:59.000000 file-name-attributes-0.2.4/src/util/registry_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1099 2023-05-21 20:46:41.000000 file-name-attributes-0.2.4/src/util/repr.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1408 2023-05-21 18:39:13.000000 file-name-attributes-0.2.4/src/util/repr_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8073 2023-05-26 20:00:25.000000 file-name-attributes-0.2.4/src/util/sqlite.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4994 2023-05-26 19:15:36.000000 file-name-attributes-0.2.4/src/util/sqlite_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      438 2023-05-22 16:05:57.000000 file-name-attributes-0.2.4/src/util/typecheck.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1338 2023-05-06 18:49:53.000000 file-name-attributes-0.2.4/src/util/typecheck_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1788 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      401 2023-05-22 16:06:32.000000 file-name-attributes-0.2.4/src/vlju/testutil.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-22 16:15:23.000000 file-name-attributes-0.2.4/src/vlju/types/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      830 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/src/vlju/types/all.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/doi/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3999 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vlju/types/doi/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3698 2023-05-22 12:38:34.000000 file-name-attributes-0.2.4/src/vlju/types/doi/doi_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)  1136925 2023-05-22 16:07:12.000000 file-name-attributes-0.2.4/src/vlju/types/doi/org.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/ean/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1691 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/ean/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2346 2023-05-21 21:36:50.000000 file-name-attributes-0.2.4/src/vlju/types/ean/ean_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3210 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/ean/isbn.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    40480 2023-05-22 15:22:32.000000 file-name-attributes-0.2.4/src/vlju/types/ean/isbn_ranges.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2463 2023-05-21 21:38:59.000000 file-name-attributes-0.2.4/src/vlju/types/ean/isbn_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      653 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/ean/ismn.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1082 2023-05-21 21:40:39.000000 file-name-attributes-0.2.4/src/vlju/types/ean/ismn_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1281 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/ean/issn.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2198 2023-05-21 21:42:02.000000 file-name-attributes-0.2.4/src/vlju/types/ean/issn_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/file/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1967 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vlju/types/file/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1751 2023-05-21 18:40:36.000000 file-name-attributes-0.2.4/src/vlju/types/file/file_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/info/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      924 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/info/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      670 2023-05-21 18:40:36.000000 file-name-attributes-0.2.4/src/vlju/types/info/info_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2835 2023-05-22 16:07:37.000000 file-name-attributes-0.2.4/src/vlju/types/info/kinds.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/lccn/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1201 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/lccn/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1055 2023-05-21 18:40:36.000000 file-name-attributes-0.2.4/src/vlju/types/lccn/lccn_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/site/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2241 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/site/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1541 2023-05-22 16:15:47.000000 file-name-attributes-0.2.4/src/vlju/types/site/site_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2860 2023-05-22 12:18:47.000000 file-name-attributes-0.2.4/src/vlju/types/site/sites_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/timestamp/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      874 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vlju/types/timestamp/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1244 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/src/vlju/types/timestamp/timestamp_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/uri/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8357 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/uri/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     6218 2023-05-22 13:38:50.000000 file-name-attributes-0.2.4/src/vlju/types/uri/uri_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/url/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      673 2023-05-22 16:16:29.000000 file-name-attributes-0.2.4/src/vlju/types/url/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      533 2023-05-21 18:40:36.000000 file-name-attributes-0.2.4/src/vlju/types/url/url_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/urn/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1356 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/urn/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4039 2023-05-22 16:09:09.000000 file-name-attributes-0.2.4/src/vlju/types/urn/kinds.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1054 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vlju/types/urn/urn_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1760 2023-05-22 13:43:11.000000 file-name-attributes-0.2.4/src/vlju/vlju_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vljum/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8442 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vljum/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2570 2023-05-23 22:07:37.000000 file-name-attributes-0.2.4/src/vljum/m.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     9087 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vljum/m_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    10520 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/src/vljum/runner.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8326 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/src/vljum/runner_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vljumap/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1197 2023-05-22 15:35:19.000000 file-name-attributes-0.2.4/src/vljumap/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    20714 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vljumap/enc.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    10428 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vljumap/enc_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1342 2023-05-23 21:58:33.000000 file-name-attributes-0.2.4/src/vljumap/factory.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1742 2023-05-23 22:02:05.000000 file-name-attributes-0.2.4/src/vljumap/factory_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1575 2023-05-22 01:56:36.000000 file-name-attributes-0.2.4/src/vljumap/vljumap_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:22.000000 file-name-attributes-0.2.5/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-06 18:55:15.000000 file-name-attributes-0.2.5/LICENSE
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       31 2023-05-07 00:42:08.000000 file-name-attributes-0.2.5/MANIFEST.in
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5434 2023-05-30 12:38:22.000000 file-name-attributes-0.2.5/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4769 2023-05-25 13:38:58.000000 file-name-attributes-0.2.5/README.md
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/config/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1638 2023-05-27 20:42:39.000000 file-name-attributes-0.2.5/config/config.toml
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/doc/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2984 2023-05-30 12:24:39.000000 file-name-attributes-0.2.5/doc/configuration.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    10407 2023-05-25 00:54:41.000000 file-name-attributes-0.2.5/doc/fna.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4121 2023-05-25 00:54:41.000000 file-name-attributes-0.2.5/doc/keys.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4559 2023-05-30 12:25:10.000000 file-name-attributes-0.2.5/pyproject.toml
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-05-30 12:38:22.000000 file-name-attributes-0.2.5/setup.cfg
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/extra/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4899 2023-05-25 00:54:42.000000 file-name-attributes-0.2.5/src/extra/fnaffle.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4378 2023-05-25 00:54:42.000000 file-name-attributes-0.2.5/src/extra/make_isbn_ranges.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/file_name_attributes.egg-info/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5434 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/file_name_attributes.egg-info/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2354 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/file_name_attributes.egg-info/SOURCES.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/file_name_attributes.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       62 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/file_name_attributes.egg-info/entry_points.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       34 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/file_name_attributes.egg-info/top_level.txt
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/fna/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3415 2023-05-22 16:11:49.000000 file-name-attributes-0.2.5/src/fna/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/util/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-22 16:12:06.000000 file-name-attributes-0.2.5/src/util/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      778 2023-05-21 18:37:39.000000 file-name-attributes-0.2.5/src/util/checksum.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      716 2023-05-21 18:37:58.000000 file-name-attributes-0.2.5/src/util/checksum_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3648 2023-05-21 20:02:21.000000 file-name-attributes-0.2.5/src/util/config.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5367 2023-05-22 13:18:46.000000 file-name-attributes-0.2.5/src/util/config_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      625 2023-05-21 19:00:38.000000 file-name-attributes-0.2.5/src/util/docsplit.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      707 2023-05-22 16:03:59.000000 file-name-attributes-0.2.5/src/util/docsplit_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     9038 2023-05-26 20:01:56.000000 file-name-attributes-0.2.5/src/util/duration.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5525 2023-05-25 00:54:41.000000 file-name-attributes-0.2.5/src/util/duration_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      102 2023-05-22 16:04:07.000000 file-name-attributes-0.2.5/src/util/error.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2181 2023-05-21 19:04:05.000000 file-name-attributes-0.2.5/src/util/escape.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2912 2023-05-21 18:38:18.000000 file-name-attributes-0.2.5/src/util/escape_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1075 2023-05-27 18:44:17.000000 file-name-attributes-0.2.5/src/util/fearmat.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      710 2023-05-06 18:49:53.000000 file-name-attributes-0.2.5/src/util/fearmat_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1857 2023-05-22 16:13:43.000000 file-name-attributes-0.2.5/src/util/io.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2033 2023-05-21 20:01:59.000000 file-name-attributes-0.2.5/src/util/io_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3535 2023-05-25 00:54:42.000000 file-name-attributes-0.2.5/src/util/multimap.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4661 2023-05-25 00:54:42.000000 file-name-attributes-0.2.5/src/util/multimap_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1063 2023-05-22 16:04:25.000000 file-name-attributes-0.2.5/src/util/pytestutil.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1738 2023-05-22 16:05:14.000000 file-name-attributes-0.2.5/src/util/registry.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      849 2023-05-21 18:38:59.000000 file-name-attributes-0.2.5/src/util/registry_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1099 2023-05-21 20:46:41.000000 file-name-attributes-0.2.5/src/util/repr.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1408 2023-05-21 18:39:13.000000 file-name-attributes-0.2.5/src/util/repr_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8073 2023-05-26 20:00:25.000000 file-name-attributes-0.2.5/src/util/sqlite.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4994 2023-05-26 19:15:36.000000 file-name-attributes-0.2.5/src/util/sqlite_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      438 2023-05-22 16:05:57.000000 file-name-attributes-0.2.5/src/util/typecheck.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1338 2023-05-06 18:49:53.000000 file-name-attributes-0.2.5/src/util/typecheck_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/vlju/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1788 2023-05-22 15:56:18.000000 file-name-attributes-0.2.5/src/vlju/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      401 2023-05-22 16:06:32.000000 file-name-attributes-0.2.5/src/vlju/testutil.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/vlju/types/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-22 16:15:23.000000 file-name-attributes-0.2.5/src/vlju/types/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      830 2023-05-25 00:54:41.000000 file-name-attributes-0.2.5/src/vlju/types/all.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/vlju/types/doi/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3999 2023-05-25 00:54:42.000000 file-name-attributes-0.2.5/src/vlju/types/doi/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3698 2023-05-22 12:38:34.000000 file-name-attributes-0.2.5/src/vlju/types/doi/doi_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)  1136925 2023-05-22 16:07:12.000000 file-name-attributes-0.2.5/src/vlju/types/doi/org.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/vlju/types/ean/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1691 2023-05-22 15:56:18.000000 file-name-attributes-0.2.5/src/vlju/types/ean/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2346 2023-05-21 21:36:50.000000 file-name-attributes-0.2.5/src/vlju/types/ean/ean_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3210 2023-05-22 15:56:18.000000 file-name-attributes-0.2.5/src/vlju/types/ean/isbn.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    40480 2023-05-22 15:22:32.000000 file-name-attributes-0.2.5/src/vlju/types/ean/isbn_ranges.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2463 2023-05-21 21:38:59.000000 file-name-attributes-0.2.5/src/vlju/types/ean/isbn_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      653 2023-05-22 15:56:18.000000 file-name-attributes-0.2.5/src/vlju/types/ean/ismn.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1082 2023-05-21 21:40:39.000000 file-name-attributes-0.2.5/src/vlju/types/ean/ismn_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1281 2023-05-22 15:56:18.000000 file-name-attributes-0.2.5/src/vlju/types/ean/issn.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2198 2023-05-21 21:42:02.000000 file-name-attributes-0.2.5/src/vlju/types/ean/issn_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/vlju/types/file/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1967 2023-05-25 00:54:42.000000 file-name-attributes-0.2.5/src/vlju/types/file/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1751 2023-05-21 18:40:36.000000 file-name-attributes-0.2.5/src/vlju/types/file/file_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/vlju/types/info/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      924 2023-05-22 15:56:18.000000 file-name-attributes-0.2.5/src/vlju/types/info/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      670 2023-05-21 18:40:36.000000 file-name-attributes-0.2.5/src/vlju/types/info/info_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2835 2023-05-22 16:07:37.000000 file-name-attributes-0.2.5/src/vlju/types/info/kinds.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/vlju/types/lccn/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1201 2023-05-22 15:56:18.000000 file-name-attributes-0.2.5/src/vlju/types/lccn/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1055 2023-05-21 18:40:36.000000 file-name-attributes-0.2.5/src/vlju/types/lccn/lccn_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:21.000000 file-name-attributes-0.2.5/src/vlju/types/site/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3978 2023-05-27 22:20:00.000000 file-name-attributes-0.2.5/src/vlju/types/site/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1541 2023-05-22 16:15:47.000000 file-name-attributes-0.2.5/src/vlju/types/site/site_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3819 2023-05-27 22:14:01.000000 file-name-attributes-0.2.5/src/vlju/types/site/sites_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:22.000000 file-name-attributes-0.2.5/src/vlju/types/timestamp/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      874 2023-05-25 00:54:42.000000 file-name-attributes-0.2.5/src/vlju/types/timestamp/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1244 2023-05-25 00:54:41.000000 file-name-attributes-0.2.5/src/vlju/types/timestamp/timestamp_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:22.000000 file-name-attributes-0.2.5/src/vlju/types/uri/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8357 2023-05-22 15:56:18.000000 file-name-attributes-0.2.5/src/vlju/types/uri/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     6218 2023-05-22 13:38:50.000000 file-name-attributes-0.2.5/src/vlju/types/uri/uri_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:22.000000 file-name-attributes-0.2.5/src/vlju/types/url/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      673 2023-05-22 16:16:29.000000 file-name-attributes-0.2.5/src/vlju/types/url/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      533 2023-05-21 18:40:36.000000 file-name-attributes-0.2.5/src/vlju/types/url/url_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:22.000000 file-name-attributes-0.2.5/src/vlju/types/urn/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1356 2023-05-22 15:56:18.000000 file-name-attributes-0.2.5/src/vlju/types/urn/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4039 2023-05-22 16:09:09.000000 file-name-attributes-0.2.5/src/vlju/types/urn/kinds.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1054 2023-05-25 00:54:42.000000 file-name-attributes-0.2.5/src/vlju/types/urn/urn_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1760 2023-05-22 13:43:11.000000 file-name-attributes-0.2.5/src/vlju/vlju_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:22.000000 file-name-attributes-0.2.5/src/vljum/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8442 2023-05-25 00:54:42.000000 file-name-attributes-0.2.5/src/vljum/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2570 2023-05-23 22:07:37.000000 file-name-attributes-0.2.5/src/vljum/m.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     9087 2023-05-25 00:54:42.000000 file-name-attributes-0.2.5/src/vljum/m_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    10520 2023-05-25 00:54:41.000000 file-name-attributes-0.2.5/src/vljum/runner.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8326 2023-05-25 00:54:41.000000 file-name-attributes-0.2.5/src/vljum/runner_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 12:38:22.000000 file-name-attributes-0.2.5/src/vljumap/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1197 2023-05-22 15:35:19.000000 file-name-attributes-0.2.5/src/vljumap/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    20714 2023-05-25 00:54:42.000000 file-name-attributes-0.2.5/src/vljumap/enc.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    10428 2023-05-25 00:54:42.000000 file-name-attributes-0.2.5/src/vljumap/enc_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1342 2023-05-23 21:58:33.000000 file-name-attributes-0.2.5/src/vljumap/factory.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1742 2023-05-23 22:02:05.000000 file-name-attributes-0.2.5/src/vljumap/factory_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1575 2023-05-22 01:56:36.000000 file-name-attributes-0.2.5/src/vljumap/vljumap_test.py
```

### Comparing `file-name-attributes-0.2.4/LICENSE` & `file-name-attributes-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/PKG-INFO` & `file-name-attributes-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-name-attributes
-Version: 0.2.4
+Version: 0.2.5
 Summary: Manage key/value metadata in file names.
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/fna
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `file-name-attributes-0.2.4/README.md` & `file-name-attributes-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/doc/configuration.md` & `file-name-attributes-0.2.5/doc/configuration.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,39 +17,58 @@
 An `[option]` section can contain key-value pairs corresponding
 to tool command line options.
 
 ### `[site.`_key_`]`
 
 A `site` section defines a mapping from a short ‘id’,
 which is to be used as a file name attribute value, to a URL.
+Optionally, it can also define rules to extract an id from a URL.
 
 The _key_ is the attribute key associated with the site type.
 
 It contains a number of required and optional fields,
 all of which have string values.
 
 - `name`: required. A unique name, used for the Python class.
 - `scheme`: optional. The URL scheme, typically `https` or `http`.
   If absent, the scheme is `https`.
 - `host`: required. The host name of the site, e.g. `example.com`.
 - `path`: optional. Path component of a site URL, if any.
 - `query`: optional. Query component of a site URL, if any.
 - `fragment`: optional. Fragment component of a site URL, if any.
 - `normalize`: optional. Converts an attribute value to canonical form.
+- `url`: optional. Converts a URL to an attribute value.
+
+The distribution file `config/config.toml` contains some examples.
+
+#### To URL
 
 At least one of `path`, `query`, or `fragment` must be present
 in order for the URL to be useful.
 
 The `path`, `query`, `fragment`, and `normalize` strings
 take the form of Python
-[f-strings](https://docs.python.org/3/reference/lexical_analysis.html#f-strings),
-with restrictions.
-Only the following Python names are available:
-`False`, `None`, `True`,
-`abs`, `all`, `any`, `ascii`, `bin`, `bool`, `chr`, `hex`, `int`, `len`,
-`max`, `min`, `oct`, `ord`, `reversed`, `slice`, `sorted`, `str`.
-
+[f-strings](https://docs.python.org/3/reference/lexical_analysis.html#f-strings).
 In the `path`, `query`, and `fragment` strings,
-`x` contains the canonical representation of the attribute value.
-In the `normalize` string, `x` is the value read.
+`id` contains the canonical representation of the attribute value.
+In the `normalize` string, `id` is the value read.
 
-The distribution file `config/config.toml` contains some examples.
+Only the following Python names are available:
+`False`, `None`, `True`,
+`abs`, `add`, `all`, `any`, `ascii`, `bin`, `bool`, `chr`, `hex`, `int`, `len`,
+`map`, `max`, `min`, `oct`, `ord`, `reversed`, `slice`, `sorted`, `str`, `sub`.
+(Python does not provide perfect isolation, so it's possible in principle
+for a malicious configuration string to do harm, but it's not more dangerous
+than running an untrusted program in the first place.)
+
+#### From URL
+
+The optional `url` field provides regular expressions
+[using Python
+syntax](https://docs.python.org/3/library/re.html#regular-expression-syntax)
+Its value must be a list.
+Each element of the list is another list containing one or two elements:
+the first is a regular expression pattern tried against a URL,
+and the second is a substitution result used if case of a match.
+If there is no second element, the substitution result is `'\1'`,
+that is, the contents of the first match group.
+Patterns are tried in order; the first to match defines the attribute value.
```

### Comparing `file-name-attributes-0.2.4/doc/fna.md` & `file-name-attributes-0.2.5/doc/fna.md`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/doc/keys.md` & `file-name-attributes-0.2.5/doc/keys.md`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/pyproject.toml` & `file-name-attributes-0.2.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "file-name-attributes"
-version = "0.2.4"
+version = "0.2.5"
 description = "Manage key/value metadata in file names."
 license.text = "MIT License"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
@@ -143,17 +143,20 @@
 allow_multiline_lambdas = true
 allow_multiline_dictionary_keys = true
 blank_lines_around_top_level_definition = 1
 blank_lines_between_top_level_imports_and_variables = 1
 coalesce_brackets = true
 column_limit = 80
 dedent_closing_brackets = false
+each_dict_entry_on_separate_line = true
 indent_dictionary_value = true
 join_multiple_lines = false
 spaces_around_default_or_named_assign = false
 spaces_around_subscript_colon = true
 spaces_before_comment = [17, 21, 25, 29, 33, 37, 41, 45, 49, 53, 57, 61, 65, 69]
+split_all_top_level_comma_separated_values = true
 split_before_bitwise_operator = true
 split_before_arithmetic_operator = true
 split_before_dot = true
 split_before_expression_after_opening_paren = true
+split_before_logical_operator = true
 split_complex_comprehension = true
```

### Comparing `file-name-attributes-0.2.4/src/extra/fnaffle.py` & `file-name-attributes-0.2.5/src/extra/fnaffle.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/extra/make_isbn_ranges.py` & `file-name-attributes-0.2.5/src/extra/make_isbn_ranges.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/file_name_attributes.egg-info/PKG-INFO` & `file-name-attributes-0.2.5/src/file_name_attributes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-name-attributes
-Version: 0.2.4
+Version: 0.2.5
 Summary: Manage key/value metadata in file names.
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/fna
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `file-name-attributes-0.2.4/src/file_name_attributes.egg-info/SOURCES.txt` & `file-name-attributes-0.2.5/src/file_name_attributes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/fna/__init__.py` & `file-name-attributes-0.2.5/src/fna/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/checksum.py` & `file-name-attributes-0.2.5/src/util/checksum.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/checksum_test.py` & `file-name-attributes-0.2.5/src/util/checksum_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/config.py` & `file-name-attributes-0.2.5/src/util/config.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/config_test.py` & `file-name-attributes-0.2.5/src/util/config_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/docsplit.py` & `file-name-attributes-0.2.5/src/util/docsplit.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/docsplit_test.py` & `file-name-attributes-0.2.5/src/util/docsplit_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/duration.py` & `file-name-attributes-0.2.5/src/util/duration.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/duration_test.py` & `file-name-attributes-0.2.5/src/util/duration_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/escape.py` & `file-name-attributes-0.2.5/src/util/escape.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/escape_test.py` & `file-name-attributes-0.2.5/src/util/escape_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/fearmat.py` & `file-name-attributes-0.2.5/src/util/fearmat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # SPDX-License-Identifier: MIT
 """Like format, but scary."""
 
 from collections.abc import Mapping
 from typing import Any
 
+import operator
+
 import util.error
 
 ALLOWED_BUILTINS = (
     'False',
     'None',
     'True',
     'abs',
@@ -16,25 +18,36 @@
     'ascii',
     'bin',
     'bool',
     'chr',
     'hex',
     'int',
     'len',
+    'map',
     'max',
     'min',
     'oct',
     'ord',
     'reversed',
     'slice',
     'sorted',
     'str',
 )
+ALLOWED_OPERATORS = (
+    'add',
+    'sub',
+)
 
-BUILTINS = {k: globals()['__builtins__'][k] for k in ALLOWED_BUILTINS}
+BUILTINS = {
+    k: globals()['__builtins__'][k]
+    for k in ALLOWED_BUILTINS
+} | {
+    k: getattr(operator, k)
+    for k in ALLOWED_OPERATORS
+}
 
 def fearmat(template: str,
             values: Mapping[str, Any],
             builtins: Mapping[str, Any] | None = None) -> str:
     if '"""' in template:
         msg = '‘"""’ in ‘template’'
         raise util.error.Error(msg)
```

### Comparing `file-name-attributes-0.2.4/src/util/fearmat_test.py` & `file-name-attributes-0.2.5/src/util/fearmat_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/io.py` & `file-name-attributes-0.2.5/src/util/io.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/io_test.py` & `file-name-attributes-0.2.5/src/util/io_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/multimap.py` & `file-name-attributes-0.2.5/src/util/multimap.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/multimap_test.py` & `file-name-attributes-0.2.5/src/util/multimap_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/pytestutil.py` & `file-name-attributes-0.2.5/src/util/pytestutil.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/registry.py` & `file-name-attributes-0.2.5/src/util/registry.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/registry_test.py` & `file-name-attributes-0.2.5/src/util/registry_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/repr.py` & `file-name-attributes-0.2.5/src/util/repr.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/repr_test.py` & `file-name-attributes-0.2.5/src/util/repr_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/sqlite.py` & `file-name-attributes-0.2.5/src/util/sqlite.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/sqlite_test.py` & `file-name-attributes-0.2.5/src/util/sqlite_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/util/typecheck_test.py` & `file-name-attributes-0.2.5/src/util/typecheck_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/__init__.py` & `file-name-attributes-0.2.5/src/vlju/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/all.py` & `file-name-attributes-0.2.5/src/vlju/types/all.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/doi/__init__.py` & `file-name-attributes-0.2.5/src/vlju/types/doi/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/doi/doi_test.py` & `file-name-attributes-0.2.5/src/vlju/types/doi/doi_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/doi/org.py` & `file-name-attributes-0.2.5/src/vlju/types/doi/org.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/ean/__init__.py` & `file-name-attributes-0.2.5/src/vlju/types/ean/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/ean/ean_test.py` & `file-name-attributes-0.2.5/src/vlju/types/ean/ean_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/ean/isbn.py` & `file-name-attributes-0.2.5/src/vlju/types/ean/isbn.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/ean/isbn_ranges.py` & `file-name-attributes-0.2.5/src/vlju/types/ean/isbn_ranges.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/ean/isbn_test.py` & `file-name-attributes-0.2.5/src/vlju/types/ean/isbn_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/ean/ismn.py` & `file-name-attributes-0.2.5/src/vlju/types/ean/ismn.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/ean/ismn_test.py` & `file-name-attributes-0.2.5/src/vlju/types/ean/ismn_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/ean/issn.py` & `file-name-attributes-0.2.5/src/vlju/types/ean/issn.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/ean/issn_test.py` & `file-name-attributes-0.2.5/src/vlju/types/ean/issn_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/file/__init__.py` & `file-name-attributes-0.2.5/src/vlju/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/file/file_test.py` & `file-name-attributes-0.2.5/src/vlju/types/file/file_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/info/__init__.py` & `file-name-attributes-0.2.5/src/vlju/types/info/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/info/info_test.py` & `file-name-attributes-0.2.5/src/vlju/types/info/info_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/info/kinds.py` & `file-name-attributes-0.2.5/src/vlju/types/info/kinds.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/lccn/__init__.py` & `file-name-attributes-0.2.5/src/vlju/types/lccn/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/lccn/lccn_test.py` & `file-name-attributes-0.2.5/src/vlju/types/lccn/lccn_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/site/site_test.py` & `file-name-attributes-0.2.5/src/vlju/types/site/site_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/site/sites_test.py` & `file-name-attributes-0.2.5/src/vlju/types/site/sites_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # ruff: noqa: F821
 
 import pathlib
 
 import pytest
 
 from util.config import read_toml_config
+from util.error import Error
 from util.pytestutil import im2p
 from vlju.types.site import site_class
 from vlju.types.url import URL
 
 config = read_toml_config(pathlib.Path('config/config.toml'))
 assert config
 for _, v in config['site'].items():
@@ -21,62 +22,76 @@
     {
         'cls': Danbooru,
         'inp': '2077531',
         'val': '2077531',
         'scheme': 'https',
         'host': 'danbooru.donmai.us',
         'path': 'posts/2077531',
+        'url': 'https://danbooru.donmai.us/posts/2077531',
     },
     {
         'cls': Gelbooru,
-        'inp': '1',
-        'val': '1',
+        'inp': '123',
+        'val': '123',
         'scheme': 'https',
         'host': 'gelbooru.com',
-        'path': 'index.php?page=post&s=view&id=1',
+        'path': 'index.php?page=post&s=view&id=123',
+        'url': 'https://gelbooru.com/index.php?page=post&s=view&id=123',
     },
     {
-        'cls': Pixiv,
-        'inp': '90647064',
-        'val': '90647064_p0',
-        'scheme': 'https',
-        'host': 'www.pixiv.net',
-        'path': 'en/artworks/90647064',
+        'cls':
+            Pixiv,
+        'inp':
+            '90647064',
+        'val':
+            '90647064_p0',
+        'scheme':
+            'https',
+        'host':
+            'www.pixiv.net',
+        'path':
+            'en/artworks/90647064',
+        'url':
+            'https://i.pximg.net/img-original/img/2021/06/19/01/14/55/90647064_p0.jpg',
     },
     {
         'cls': Pixiv,
-        'inp': '51307116_p14',
-        'val': '51307116_p14',
+        'inp': '52112383_p4',
+        'val': '52112383_p4',
         'scheme': 'https',
         'host': 'www.pixiv.net',
-        'path': 'en/artworks/51307116#15',
+        'path': 'en/artworks/52112383#5',
+        'url': 'https://pixiv.net/en/artworks/52112383#5',
     },
     {
         'cls': Twitter,
         'inp': '1152566724341878786',
         'val': '1152566724341878786',
         'scheme': 'https',
         'host': 'twitter.com',
         'path': 'i/web/status/1152566724341878786',
+        'url': 'https://twitter.com/i/web/status/1152566724341878786',
     },
     {
         'cls': Twitter,
         'inp': 'ClariS_Staff,245010623375749121',
         'val': 'ClariS_Staff,245010623375749121',
         'scheme': 'https',
         'host': 'twitter.com',
         'path': 'ClariS_Staff/status/245010623375749121',
+        'url': 'https://twitter.com/ClariS_Staff/status/245010623375749121',
     },
     {
         'cls': YouTube,
         'inp': 'ROsmdDujDH8',
         'val': 'ROsmdDujDH8',
         'scheme': 'https',
         'host': 'www.youtube.com',
         'path': 'watch?v=ROsmdDujDH8',
+        'url': 'https://www.youtube.com/watch?v=ROsmdDujDH8',
     },
 ]
 
 @pytest.mark.parametrize(*im2p(CASES, ('cls', 'inp', 'scheme')))
 def test_scheme(cls, inp, scheme):
     assert cls(inp).scheme() == scheme
 
@@ -91,17 +106,27 @@
 @pytest.mark.parametrize(*im2p(CASES, ('cls', 'inp', 'scheme', 'host', 'path')))
 def test_url(cls, inp, scheme, host, path):
     y = cls(inp)
     url = URL(y)
     x = f'{scheme}://{host}/{path}'
     assert str(url) == x
 
+@pytest.mark.parametrize(*im2p(CASES, ('cls', 'url', 'val')))
+def test_from_url(cls, url, val):
+    u = cls.from_url(url)
+    assert isinstance(u, cls)
+    assert str(u) == val
+
+@pytest.mark.parametrize(*im2p(CASES, ('cls', 'url', 'val')))
+def test_init_from_url(cls, url, val):
+    assert str(cls(url)) == val
+
 @pytest.mark.parametrize(*im2p(CASES, ('cls', 'inp', 'scheme', 'host', 'path')))
-def test_site_bad_cast(
-        cls,
-        inp,
-        scheme,  # noqa: unused-function-argument
-        host,  # noqa: unused-function-argument
-        path):  # noqa: unused-function-argument
+def test_site_bad_cast(cls, inp, scheme, host, path):
     y = cls(inp)
     with pytest.raises(TypeError):
         _ = y.cast_params(int)
+
+@pytest.mark.parametrize(*im2p(CASES, ('cls',)))
+def test_from_url_fail(cls):
+    with pytest.raises(Error, match='not recognized'):
+        _ = cls.from_url('http://example.com/')
```

### Comparing `file-name-attributes-0.2.4/src/vlju/types/timestamp/__init__.py` & `file-name-attributes-0.2.5/src/vlju/types/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/timestamp/timestamp_test.py` & `file-name-attributes-0.2.5/src/vlju/types/timestamp/timestamp_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/uri/__init__.py` & `file-name-attributes-0.2.5/src/vlju/types/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/uri/uri_test.py` & `file-name-attributes-0.2.5/src/vlju/types/uri/uri_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/url/__init__.py` & `file-name-attributes-0.2.5/src/vlju/types/url/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/url/url_test.py` & `file-name-attributes-0.2.5/src/vlju/types/url/url_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/urn/__init__.py` & `file-name-attributes-0.2.5/src/vlju/types/urn/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/urn/kinds.py` & `file-name-attributes-0.2.5/src/vlju/types/urn/kinds.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/types/urn/urn_test.py` & `file-name-attributes-0.2.5/src/vlju/types/urn/urn_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vlju/vlju_test.py` & `file-name-attributes-0.2.5/src/vlju/vlju_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vljum/__init__.py` & `file-name-attributes-0.2.5/src/vljum/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vljum/m.py` & `file-name-attributes-0.2.5/src/vljum/m.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vljum/m_test.py` & `file-name-attributes-0.2.5/src/vljum/m_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vljum/runner.py` & `file-name-attributes-0.2.5/src/vljum/runner.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vljum/runner_test.py` & `file-name-attributes-0.2.5/src/vljum/runner_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vljumap/__init__.py` & `file-name-attributes-0.2.5/src/vljumap/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vljumap/enc.py` & `file-name-attributes-0.2.5/src/vljumap/enc.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vljumap/enc_test.py` & `file-name-attributes-0.2.5/src/vljumap/enc_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vljumap/factory.py` & `file-name-attributes-0.2.5/src/vljumap/factory.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vljumap/factory_test.py` & `file-name-attributes-0.2.5/src/vljumap/factory_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.4/src/vljumap/vljumap_test.py` & `file-name-attributes-0.2.5/src/vljumap/vljumap_test.py`

 * *Files identical despite different names*

