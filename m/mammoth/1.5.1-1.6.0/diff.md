# Comparing `tmp/mammoth-1.5.1.tar.gz` & `tmp/mammoth-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mammoth-1.5.1.tar", last modified: Wed Apr  5 20:38:42 2023, max compression
+gzip compressed data, was "mammoth-1.6.0.tar", last modified: Tue May 30 10:34:12 2023, max compression
```

## Comparing `mammoth-1.5.1.tar` & `mammoth-1.6.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-04-05 20:38:42.253144 mammoth-1.5.1/
--rw-r--r--   0 mick      (1000) mick      (1000)     1307 2013-11-30 23:33:05.000000 mammoth-1.5.1/LICENSE
--rw-r--r--   0 mick      (1000) mick      (1000)    23601 2023-04-05 20:38:42.253144 mammoth-1.5.1/PKG-INFO
--rw-r--r--   0 mick      (1000) mick      (1000)    22500 2023-04-05 20:23:58.000000 mammoth-1.5.1/README
-drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-04-05 20:38:42.249143 mammoth-1.5.1/mammoth/
--rw-r--r--   0 mick      (1000) mick      (1000)     1463 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/__init__.py
--rw-r--r--   0 mick      (1000) mick      (1000)     3095 2018-11-02 20:10:04.000000 mammoth-1.5.1/mammoth/cli.py
--rw-r--r--   0 mick      (1000) mick      (1000)    13513 2021-08-01 10:06:55.000000 mammoth-1.5.1/mammoth/conversion.py
--rw-r--r--   0 mick      (1000) mick      (1000)     1864 2020-11-05 19:40:41.000000 mammoth-1.5.1/mammoth/document_matchers.py
--rw-r--r--   0 mick      (1000) mick      (1000)     6001 2021-08-01 10:06:42.000000 mammoth-1.5.1/mammoth/documents.py
-drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-04-05 20:38:42.249143 mammoth-1.5.1/mammoth/docx/
--rw-r--r--   0 mick      (1000) mick      (1000)     6342 2019-03-17 21:24:14.000000 mammoth-1.5.1/mammoth/docx/__init__.py
--rw-r--r--   0 mick      (1000) mick      (1000)    22396 2022-03-09 21:00:38.000000 mammoth-1.5.1/mammoth/docx/body_xml.py
--rw-r--r--   0 mick      (1000) mick      (1000)      849 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/docx/comments_xml.py
--rw-r--r--   0 mick      (1000) mick      (1000)      181 2021-08-01 16:19:06.000000 mammoth-1.5.1/mammoth/docx/complex_fields.py
--rw-r--r--   0 mick      (1000) mick      (1000)     1632 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/docx/content_types_xml.py
--rw-r--r--   0 mick      (1000) mick      (1000)    32817 2021-01-19 22:04:23.000000 mammoth-1.5.1/mammoth/docx/dingbats.py
--rw-r--r--   0 mick      (1000) mick      (1000)      498 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/docx/document_xml.py
--rw-r--r--   0 mick      (1000) mick      (1000)     1029 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/docx/files.py
--rw-r--r--   0 mick      (1000) mick      (1000)      979 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/docx/notes_xml.py
--rw-r--r--   0 mick      (1000) mick      (1000)     3704 2021-05-11 21:32:05.000000 mammoth-1.5.1/mammoth/docx/numbering_xml.py
--rw-r--r--   0 mick      (1000) mick      (1000)     1270 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/docx/office_xml.py
--rw-r--r--   0 mick      (1000) mick      (1000)     1194 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/docx/relationships_xml.py
--rw-r--r--   0 mick      (1000) mick      (1000)     2514 2020-11-06 19:35:22.000000 mammoth-1.5.1/mammoth/docx/style_map.py
--rw-r--r--   0 mick      (1000) mick      (1000)     2990 2019-03-17 16:51:03.000000 mammoth-1.5.1/mammoth/docx/styles_xml.py
--rw-r--r--   0 mick      (1000) mick      (1000)      289 2017-05-18 19:12:17.000000 mammoth-1.5.1/mammoth/docx/uris.py
--rw-r--r--   0 mick      (1000) mick      (1000)     3575 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/docx/xmlparser.py
-drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-04-05 20:38:42.249143 mammoth-1.5.1/mammoth/html/
--rw-r--r--   0 mick      (1000) mick      (1000)     3516 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/html/__init__.py
--rw-r--r--   0 mick      (1000) mick      (1000)     1076 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/html/nodes.py
--rw-r--r--   0 mick      (1000) mick      (1000)     1159 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/html_paths.py
--rw-r--r--   0 mick      (1000) mick      (1000)      638 2022-08-31 20:33:14.000000 mammoth-1.5.1/mammoth/images.py
--rw-r--r--   0 mick      (1000) mick      (1000)      785 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/lists.py
--rw-r--r--   0 mick      (1000) mick      (1000)     3111 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/options.py
--rw-r--r--   0 mick      (1000) mick      (1000)      435 2021-08-01 10:10:27.000000 mammoth-1.5.1/mammoth/raw_text.py
--rw-r--r--   0 mick      (1000) mick      (1000)      905 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/results.py
-drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-04-05 20:38:42.249143 mammoth-1.5.1/mammoth/styles/
--rw-r--r--   0 mick      (1000) mick      (1000)      184 2016-11-29 22:11:41.000000 mammoth-1.5.1/mammoth/styles/__init__.py
-drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-04-05 20:38:42.249143 mammoth-1.5.1/mammoth/styles/parser/
--rw-r--r--   0 mick      (1000) mick      (1000)      514 2016-11-29 22:11:41.000000 mammoth-1.5.1/mammoth/styles/parser/__init__.py
--rw-r--r--   0 mick      (1000) mick      (1000)     3868 2020-11-05 19:40:53.000000 mammoth-1.5.1/mammoth/styles/parser/document_matcher_parser.py
--rw-r--r--   0 mick      (1000) mick      (1000)       42 2016-11-29 22:11:41.000000 mammoth-1.5.1/mammoth/styles/parser/errors.py
--rw-r--r--   0 mick      (1000) mick      (1000)     2034 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/styles/parser/html_path_parser.py
--rw-r--r--   0 mick      (1000) mick      (1000)      498 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/styles/parser/style_mapping_parser.py
--rw-r--r--   0 mick      (1000) mick      (1000)     1786 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/styles/parser/token_iterator.py
--rw-r--r--   0 mick      (1000) mick      (1000)      793 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/styles/parser/token_parser.py
--rw-r--r--   0 mick      (1000) mick      (1000)     1652 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/styles/parser/tokeniser.py
--rw-r--r--   0 mick      (1000) mick      (1000)     1416 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/transforms.py
--rw-r--r--   0 mick      (1000) mick      (1000)      171 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/underline.py
-drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-04-05 20:38:42.253144 mammoth-1.5.1/mammoth/writers/
--rw-r--r--   0 mick      (1000) mick      (1000)      320 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/writers/__init__.py
--rw-r--r--   0 mick      (1000) mick      (1000)      554 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/writers/abc.py
--rw-r--r--   0 mick      (1000) mick      (1000)     1183 2019-10-31 11:00:12.000000 mammoth-1.5.1/mammoth/writers/html.py
--rw-r--r--   0 mick      (1000) mick      (1000)     5300 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/writers/markdown.py
--rw-r--r--   0 mick      (1000) mick      (1000)     1802 2018-11-02 20:01:06.000000 mammoth-1.5.1/mammoth/zips.py
-drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-04-05 20:38:42.249143 mammoth-1.5.1/mammoth.egg-info/
--rw-r--r--   0 mick      (1000) mick      (1000)    23601 2023-04-05 20:38:42.000000 mammoth-1.5.1/mammoth.egg-info/PKG-INFO
--rw-r--r--   0 mick      (1000) mick      (1000)     1464 2023-04-05 20:38:42.000000 mammoth-1.5.1/mammoth.egg-info/SOURCES.txt
--rw-r--r--   0 mick      (1000) mick      (1000)        1 2023-04-05 20:38:42.000000 mammoth-1.5.1/mammoth.egg-info/dependency_links.txt
--rw-r--r--   0 mick      (1000) mick      (1000)       45 2023-04-05 20:38:42.000000 mammoth-1.5.1/mammoth.egg-info/entry_points.txt
--rw-r--r--   0 mick      (1000) mick      (1000)       19 2023-04-05 20:38:42.000000 mammoth-1.5.1/mammoth.egg-info/requires.txt
--rw-r--r--   0 mick      (1000) mick      (1000)        8 2023-04-05 20:38:42.000000 mammoth-1.5.1/mammoth.egg-info/top_level.txt
--rw-r--r--   0 mick      (1000) mick      (1000)       81 2023-04-05 20:24:19.000000 mammoth-1.5.1/pyproject.toml
--rw-r--r--   0 mick      (1000) mick      (1000)       67 2023-04-05 20:38:42.253144 mammoth-1.5.1/setup.cfg
--rw-r--r--   0 mick      (1000) mick      (1000)     1603 2023-04-05 20:38:01.000000 mammoth-1.5.1/setup.py
-drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-04-05 20:38:42.253144 mammoth-1.5.1/tests/
--rw-r--r--   0 mick      (1000) mick      (1000)      433 2022-11-25 23:03:53.000000 mammoth-1.5.1/tests/testing.py
+drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-05-30 10:34:12.475019 mammoth-1.6.0/
+-rw-r--r--   0 mick      (1000) mick      (1000)     1307 2013-11-30 23:33:05.000000 mammoth-1.6.0/LICENSE
+-rw-r--r--   0 mick      (1000) mick      (1000)    23601 2023-05-30 10:34:12.475019 mammoth-1.6.0/PKG-INFO
+-rw-r--r--   0 mick      (1000) mick      (1000)    22500 2023-05-20 19:48:47.000000 mammoth-1.6.0/README
+drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-05-30 10:34:12.467019 mammoth-1.6.0/mammoth/
+-rw-r--r--   0 mick      (1000) mick      (1000)     1463 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/__init__.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     3095 2018-11-02 20:10:04.000000 mammoth-1.6.0/mammoth/cli.py
+-rw-r--r--   0 mick      (1000) mick      (1000)    13513 2021-08-01 10:06:55.000000 mammoth-1.6.0/mammoth/conversion.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     1864 2020-11-05 19:40:41.000000 mammoth-1.6.0/mammoth/document_matchers.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     6001 2021-08-01 10:06:42.000000 mammoth-1.6.0/mammoth/documents.py
+drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-05-30 10:34:12.471019 mammoth-1.6.0/mammoth/docx/
+-rw-r--r--   0 mick      (1000) mick      (1000)     6342 2019-03-17 21:24:14.000000 mammoth-1.6.0/mammoth/docx/__init__.py
+-rw-r--r--   0 mick      (1000) mick      (1000)    23159 2023-05-20 19:48:34.000000 mammoth-1.6.0/mammoth/docx/body_xml.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      849 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/docx/comments_xml.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      181 2021-08-01 16:19:06.000000 mammoth-1.6.0/mammoth/docx/complex_fields.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     1632 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/docx/content_types_xml.py
+-rw-r--r--   0 mick      (1000) mick      (1000)    32817 2021-01-19 22:04:23.000000 mammoth-1.6.0/mammoth/docx/dingbats.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      498 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/docx/document_xml.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     1029 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/docx/files.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      979 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/docx/notes_xml.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     3704 2021-05-11 21:32:05.000000 mammoth-1.6.0/mammoth/docx/numbering_xml.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     1270 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/docx/office_xml.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     1194 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/docx/relationships_xml.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     2514 2020-11-06 19:35:22.000000 mammoth-1.6.0/mammoth/docx/style_map.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     2990 2019-03-17 16:51:03.000000 mammoth-1.6.0/mammoth/docx/styles_xml.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      289 2017-05-18 19:12:17.000000 mammoth-1.6.0/mammoth/docx/uris.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     3140 2023-05-30 10:32:01.000000 mammoth-1.6.0/mammoth/docx/xmlparser.py
+drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-05-30 10:34:12.471019 mammoth-1.6.0/mammoth/html/
+-rw-r--r--   0 mick      (1000) mick      (1000)     3516 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/html/__init__.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     1076 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/html/nodes.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     1159 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/html_paths.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      638 2022-08-31 20:33:14.000000 mammoth-1.6.0/mammoth/images.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      785 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/lists.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     3111 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/options.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      435 2021-08-01 10:10:27.000000 mammoth-1.6.0/mammoth/raw_text.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      905 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/results.py
+drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-05-30 10:34:12.471019 mammoth-1.6.0/mammoth/styles/
+-rw-r--r--   0 mick      (1000) mick      (1000)      184 2016-11-29 22:11:41.000000 mammoth-1.6.0/mammoth/styles/__init__.py
+drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-05-30 10:34:12.475019 mammoth-1.6.0/mammoth/styles/parser/
+-rw-r--r--   0 mick      (1000) mick      (1000)      514 2016-11-29 22:11:41.000000 mammoth-1.6.0/mammoth/styles/parser/__init__.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     3868 2020-11-05 19:40:53.000000 mammoth-1.6.0/mammoth/styles/parser/document_matcher_parser.py
+-rw-r--r--   0 mick      (1000) mick      (1000)       42 2016-11-29 22:11:41.000000 mammoth-1.6.0/mammoth/styles/parser/errors.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     2034 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/styles/parser/html_path_parser.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      498 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/styles/parser/style_mapping_parser.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     1786 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/styles/parser/token_iterator.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      793 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/styles/parser/token_parser.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     1652 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/styles/parser/tokeniser.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     1416 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/transforms.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      171 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/underline.py
+drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-05-30 10:34:12.475019 mammoth-1.6.0/mammoth/writers/
+-rw-r--r--   0 mick      (1000) mick      (1000)      320 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/writers/__init__.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      554 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/writers/abc.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     1183 2019-10-31 11:00:12.000000 mammoth-1.6.0/mammoth/writers/html.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     5300 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/writers/markdown.py
+-rw-r--r--   0 mick      (1000) mick      (1000)     1802 2018-11-02 20:01:06.000000 mammoth-1.6.0/mammoth/zips.py
+drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-05-30 10:34:12.471019 mammoth-1.6.0/mammoth.egg-info/
+-rw-r--r--   0 mick      (1000) mick      (1000)    23601 2023-05-30 10:34:12.000000 mammoth-1.6.0/mammoth.egg-info/PKG-INFO
+-rw-r--r--   0 mick      (1000) mick      (1000)     1464 2023-05-30 10:34:12.000000 mammoth-1.6.0/mammoth.egg-info/SOURCES.txt
+-rw-r--r--   0 mick      (1000) mick      (1000)        1 2023-05-30 10:34:12.000000 mammoth-1.6.0/mammoth.egg-info/dependency_links.txt
+-rw-r--r--   0 mick      (1000) mick      (1000)       45 2023-05-30 10:34:12.000000 mammoth-1.6.0/mammoth.egg-info/entry_points.txt
+-rw-r--r--   0 mick      (1000) mick      (1000)       19 2023-05-30 10:34:12.000000 mammoth-1.6.0/mammoth.egg-info/requires.txt
+-rw-r--r--   0 mick      (1000) mick      (1000)        8 2023-05-30 10:34:12.000000 mammoth-1.6.0/mammoth.egg-info/top_level.txt
+-rw-r--r--   0 mick      (1000) mick      (1000)       81 2023-04-05 20:24:19.000000 mammoth-1.6.0/pyproject.toml
+-rw-r--r--   0 mick      (1000) mick      (1000)       67 2023-05-30 10:34:12.475019 mammoth-1.6.0/setup.cfg
+-rw-r--r--   0 mick      (1000) mick      (1000)     1603 2023-05-30 10:32:27.000000 mammoth-1.6.0/setup.py
+drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2023-05-30 10:34:12.475019 mammoth-1.6.0/tests/
+-rw-r--r--   0 mick      (1000) mick      (1000)      433 2022-11-25 23:03:53.000000 mammoth-1.6.0/tests/testing.py
```

### Comparing `mammoth-1.5.1/LICENSE` & `mammoth-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/PKG-INFO` & `mammoth-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mammoth
-Version: 1.5.1
+Version: 1.6.0
 Summary: Convert Word documents from docx to simple and clean HTML and Markdown
 Home-page: https://github.com/mwilliamson/python-mammoth
 Author: Michael Williamson
 Author-email: mike@zwobble.org
 License: BSD-2-Clause
 Keywords: docx word office clean html markdown md
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mammoth-1.5.1/README` & `mammoth-1.6.0/README`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/__init__.py` & `mammoth-1.6.0/mammoth/__init__.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/cli.py` & `mammoth-1.6.0/mammoth/cli.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/conversion.py` & `mammoth-1.6.0/mammoth/conversion.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/document_matchers.py` & `mammoth-1.6.0/mammoth/document_matchers.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/documents.py` & `mammoth-1.6.0/mammoth/documents.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/docx/__init__.py` & `mammoth-1.6.0/mammoth/docx/__init__.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/docx/body_xml.py` & `mammoth-1.6.0/mammoth/docx/body_xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,22 @@
 
     def read_all(self, elements):
         result = self._read_all(elements)
         return results.Result(result.elements, result.messages)
 
 
 def _create_reader(numbering, content_types, relationships, styles, docx_file, files):
+    current_instr_text = []
+    complex_field_stack = []
+
+    # When a paragraph is marked as deleted, its contents should be combined
+    # with the following paragraph. See 17.13.5.15 del (Deleted Paragraph) of
+    # ECMA-376 4th edition Part 1.
+    deleted_paragraph_contents = []
+
     _ignored_elements = set([
         "office-word:wrap",
         "v:shadow",
         "v:shapetype",
         "w:annotationRef",
         "w:bookmarkEnd",
         "w:sectPr",
@@ -127,38 +135,49 @@
         return element and element.attributes.get("w:val") not in ["false", "0"]
 
     def read_underline_element(element):
         return element and element.attributes.get("w:val") not in [None, "false", "0", "none"]
 
     def paragraph(element):
         properties = element.find_child_or_null("w:pPr")
-        alignment = properties.find_child_or_null("w:jc").attributes.get("w:val")
-        indent = _read_paragraph_indent(properties.find_child_or_null("w:ind"))
 
-        return _ReadResult.map_results(
-            _read_paragraph_style(properties),
-            _read_xml_elements(element.children),
-            lambda style, children: documents.paragraph(
-                children=children,
-                style_id=style[0],
-                style_name=style[1],
-                numbering=_read_numbering_properties(
-                    paragraph_style_id=style[0],
-                    element=properties.find_child_or_null("w:numPr"),
-                ),
-                alignment=alignment,
-                indent=indent,
-            )).append_extra()
+        is_deleted = properties.find_child_or_null("w:rPr").find_child("w:del")
+
+        if is_deleted is not None:
+            for child in element.children:
+                deleted_paragraph_contents.append(child)
+            return _empty_result
+
+        else:
+            alignment = properties.find_child_or_null("w:jc").attributes.get("w:val")
+            indent = _read_paragraph_indent(properties.find_child_or_null("w:ind"))
+
+            children_xml = element.children
+            if deleted_paragraph_contents:
+                children_xml = deleted_paragraph_contents + children_xml
+                del deleted_paragraph_contents[:]
+
+            return _ReadResult.map_results(
+                _read_paragraph_style(properties),
+                _read_xml_elements(children_xml),
+                lambda style, children: documents.paragraph(
+                    children=children,
+                    style_id=style[0],
+                    style_name=style[1],
+                    numbering=_read_numbering_properties(
+                        paragraph_style_id=style[0],
+                        element=properties.find_child_or_null("w:numPr"),
+                    ),
+                    alignment=alignment,
+                    indent=indent,
+                )).append_extra()
 
     def _read_paragraph_style(properties):
         return _read_style(properties, "w:pStyle", "Paragraph", styles.find_paragraph_style_by_id)
 
-    current_instr_text = []
-    complex_field_stack = []
-
     def current_hyperlink_kwargs():
         for complex_field in reversed(complex_field_stack):
             if isinstance(complex_field, complex_fields.Hyperlink):
                 return complex_field.kwargs
 
         return None
```

### Comparing `mammoth-1.5.1/mammoth/docx/comments_xml.py` & `mammoth-1.6.0/mammoth/docx/comments_xml.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/docx/content_types_xml.py` & `mammoth-1.6.0/mammoth/docx/content_types_xml.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/docx/dingbats.py` & `mammoth-1.6.0/mammoth/docx/dingbats.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/docx/files.py` & `mammoth-1.6.0/mammoth/docx/files.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/docx/notes_xml.py` & `mammoth-1.6.0/mammoth/docx/notes_xml.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/docx/numbering_xml.py` & `mammoth-1.6.0/mammoth/docx/numbering_xml.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/docx/office_xml.py` & `mammoth-1.6.0/mammoth/docx/office_xml.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/docx/relationships_xml.py` & `mammoth-1.6.0/mammoth/docx/relationships_xml.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/docx/style_map.py` & `mammoth-1.6.0/mammoth/docx/style_map.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/docx/styles_xml.py` & `mammoth-1.6.0/mammoth/docx/styles_xml.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/docx/xmlparser.py` & `mammoth-1.6.0/mammoth/docx/xmlparser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import xml.sax
+import xml.dom.minidom
 
 import cobble
 
 
 @cobble.data
 class XmlElement(object):
     name = cobble.field()
     attributes = cobble.field()
     children = cobble.field()
-    
+
     def find_child_or_null(self, name):
         return self.find_child(name) or _null_xml_element
-    
+
     def find_child(self, name):
         for child in self.children:
             if isinstance(child, XmlElement) and child.name == name:
                 return child
-        
-    
+
+
     def find_children(self, name):
         return XmlElementList(filter(
             lambda child: child.node_type == node_types.element and child.name == name,
             self.children
         ))
 
 
 class XmlElementList(object):
     def __init__(self, elements):
         self._elements = elements
-        
+
     def __iter__(self):
         return iter(self._elements)
-    
+
     def find_children(self, name):
         children = []
         for element in self._elements:
             for child in element.find_children(name):
                 children.append(child)
         return XmlElementList(children)
 
 
 class NullXmlElement(object):
     attributes = {}
-    
+
     def find_child_or_null(self, name):
         return self
-    
+
     def find_child(self, name):
         return None
 
 
 _null_xml_element = NullXmlElement()
 
 
@@ -75,59 +75,46 @@
 
 
 def parse_xml(fileobj, namespace_mapping=None):
     if namespace_mapping is None:
         namespace_prefixes = {}
     else:
         namespace_prefixes = dict((uri, prefix) for prefix, uri in namespace_mapping)
-    
-    handler = Handler(namespace_prefixes)
-    parser = xml.sax.make_parser()
-    parser.setFeature(xml.sax.handler.feature_namespaces, True)
-    parser.setContentHandler(handler)
-    parser.parse(fileobj)
-    return handler.root()
-
-
-class Handler(xml.sax.handler.ContentHandler):
-    def __init__(self, namespace_prefixes):
-        self._namespace_prefixes = namespace_prefixes
-        self._element_stack = [RootElement()]
-        self._character_buffer = []
-    
-    def root(self):
-        return self._element_stack[0].children[0]
-    
-    def startElementNS(self, name, qname, attrs):
-        self._flush_character_buffer()
-        attributes = dict((self._read_name(key), value) for key, value in attrs.items())
-        element = XmlElement(self._read_name(name), attributes, [])
-        self._element_stack[-1].children.append(element)
-        self._element_stack.append(element)
-    
-    def endElementNS(self, name, qname):
-        self._flush_character_buffer()
-        self._element_stack.pop()
-        
-    def characters(self, content):
-        self._character_buffer.append(content)
-
-    def _flush_character_buffer(self):
-        if self._character_buffer:
-            text = "".join(self._character_buffer)
-            self._element_stack[-1].children.append(XmlText(text))
-            self._character_buffer = []
-            
-    def _read_name(self, name):
-        uri, local_name = name
-        if uri is None:
-            return local_name
+
+    document = xml.dom.minidom.parse(fileobj)
+
+    def convert_node(node):
+        if node.nodeType == xml.dom.Node.ELEMENT_NODE:
+            return convert_element(node)
+        elif node.nodeType == xml.dom.Node.TEXT_NODE:
+            return XmlText(node.nodeValue)
+        else:
+            return None
+
+    def convert_element(element):
+        converted_name = convert_name(element)
+
+        converted_attributes = dict(
+            (convert_name(attribute), attribute.value)
+            for attribute in element.attributes.values()
+            if attribute.namespaceURI != "http://www.w3.org/2000/xmlns/"
+        )
+
+        converted_children = []
+        for child_node in element.childNodes:
+            converted_child_node = convert_node(child_node)
+            if converted_child_node is not None:
+                converted_children.append(converted_child_node)
+
+        return XmlElement(converted_name, converted_attributes, converted_children)
+
+    def convert_name(node):
+        if node.namespaceURI is None:
+            return node.localName
         else:
-            prefix = self._namespace_prefixes.get(uri)
+            prefix = namespace_prefixes.get(node.namespaceURI)
             if prefix is None:
-                return "{%s}%s" % (uri, local_name)
+                return "{%s}%s" % (node.namespaceURI, node.localName)
             else:
-                return "%s:%s" % (prefix, local_name)
+                return "%s:%s" % (prefix, node.localName)
 
-class RootElement(object):
-    def __init__(self):
-        self.children = []
+    return convert_node(document.documentElement)
```

### Comparing `mammoth-1.5.1/mammoth/html/__init__.py` & `mammoth-1.6.0/mammoth/html/__init__.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/html/nodes.py` & `mammoth-1.6.0/mammoth/html/nodes.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/html_paths.py` & `mammoth-1.6.0/mammoth/html_paths.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/images.py` & `mammoth-1.6.0/mammoth/images.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/lists.py` & `mammoth-1.6.0/mammoth/lists.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/options.py` & `mammoth-1.6.0/mammoth/options.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/results.py` & `mammoth-1.6.0/mammoth/results.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/styles/parser/__init__.py` & `mammoth-1.6.0/mammoth/styles/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/styles/parser/document_matcher_parser.py` & `mammoth-1.6.0/mammoth/styles/parser/document_matcher_parser.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/styles/parser/html_path_parser.py` & `mammoth-1.6.0/mammoth/styles/parser/html_path_parser.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/styles/parser/token_iterator.py` & `mammoth-1.6.0/mammoth/styles/parser/token_iterator.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/styles/parser/token_parser.py` & `mammoth-1.6.0/mammoth/styles/parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/styles/parser/tokeniser.py` & `mammoth-1.6.0/mammoth/styles/parser/tokeniser.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/transforms.py` & `mammoth-1.6.0/mammoth/transforms.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/writers/abc.py` & `mammoth-1.6.0/mammoth/writers/abc.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/writers/html.py` & `mammoth-1.6.0/mammoth/writers/html.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/writers/markdown.py` & `mammoth-1.6.0/mammoth/writers/markdown.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth/zips.py` & `mammoth-1.6.0/mammoth/zips.py`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/mammoth.egg-info/PKG-INFO` & `mammoth-1.6.0/mammoth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mammoth
-Version: 1.5.1
+Version: 1.6.0
 Summary: Convert Word documents from docx to simple and clean HTML and Markdown
 Home-page: https://github.com/mwilliamson/python-mammoth
 Author: Michael Williamson
 Author-email: mike@zwobble.org
 License: BSD-2-Clause
 Keywords: docx word office clean html markdown md
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mammoth-1.5.1/mammoth.egg-info/SOURCES.txt` & `mammoth-1.6.0/mammoth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mammoth-1.5.1/setup.py` & `mammoth-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='mammoth',
-    version='1.5.1',
+    version='1.6.0',
     description='Convert Word documents from docx to simple and clean HTML and Markdown',
     long_description=read("README"),
     author='Michael Williamson',
     author_email='mike@zwobble.org',
     url='https://github.com/mwilliamson/python-mammoth',
     packages=['mammoth', 'mammoth.docx', 'mammoth.html', 'mammoth.styles', 'mammoth.styles.parser', 'mammoth.writers'],
     entry_points={
```

