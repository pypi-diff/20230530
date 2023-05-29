# Comparing `tmp/jesth-0.0.7.tar.gz` & `tmp/jesth-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jesth-0.0.7.tar", last modified: Thu May 18 16:37:22 2023, max compression
+gzip compressed data, was "dist/jesth-0.0.8.tar", last modified: Mon May 29 22:09:44 2023, max compression
```

## Comparing `jesth-0.0.7.tar` & `jesth-0.0.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 16:37:22.149441 jesth-0.0.7/
--rw-rw-r--   0 alex      (1002) alex      (1003)     1082 2023-01-27 15:42:40.000000 jesth-0.0.7/LICENSE
--rw-rw-r--   0 alex      (1002) alex      (1003)       67 2022-05-20 19:23:56.000000 jesth-0.0.7/MANIFEST.in
--rw-rw-r--   0 alex      (1002) alex      (1003)    29916 2023-05-18 16:37:22.149441 jesth-0.0.7/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)    29223 2023-05-18 16:17:45.000000 jesth-0.0.7/README.md
--rw-rw-r--   0 alex      (1002) alex      (1003)        5 2023-02-25 01:39:20.000000 jesth-0.0.7/VERSION
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 16:37:22.101441 jesth-0.0.7/jesth/
--rw-rw-r--   0 alex      (1002) alex      (1003)      518 2023-05-01 13:03:42.000000 jesth-0.0.7/jesth/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      140 2022-05-21 09:50:04.000000 jesth-0.0.7/jesth/__main__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 16:37:22.149441 jesth-0.0.7/jesth/box/
--rw-rw-r--   0 alex      (1002) alex      (1003)     1429 2023-05-01 07:48:28.000000 jesth-0.0.7/jesth/box/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 16:37:22.149441 jesth-0.0.7/jesth/const/
--rw-rw-r--   0 alex      (1002) alex      (1003)      234 2023-05-09 11:22:33.000000 jesth-0.0.7/jesth/const/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 16:37:22.149441 jesth-0.0.7/jesth/converter/
--rw-rw-r--   0 alex      (1002) alex      (1003)    42404 2023-05-11 09:04:01.000000 jesth-0.0.7/jesth/converter/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 16:37:22.149441 jesth-0.0.7/jesth/document/
--rw-rw-r--   0 alex      (1002) alex      (1003)     7458 2023-05-01 13:03:42.000000 jesth-0.0.7/jesth/document/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 16:37:22.149441 jesth-0.0.7/jesth/error/
--rw-rw-r--   0 alex      (1002) alex      (1003)      298 2023-05-01 11:22:47.000000 jesth-0.0.7/jesth/error/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 16:37:22.149441 jesth-0.0.7/jesth/misc/
--rw-rw-r--   0 alex      (1002) alex      (1003)     7867 2023-05-01 13:03:42.000000 jesth-0.0.7/jesth/misc/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 16:37:22.149441 jesth-0.0.7/jesth/parser/
--rw-rw-r--   0 alex      (1002) alex      (1003)     4075 2023-05-01 15:41:06.000000 jesth-0.0.7/jesth/parser/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 16:37:22.149441 jesth-0.0.7/jesth/renderer/
--rw-rw-r--   0 alex      (1002) alex      (1003)     2199 2023-05-09 12:13:04.000000 jesth-0.0.7/jesth/renderer/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 16:37:22.149441 jesth-0.0.7/jesth/section/
--rw-rw-r--   0 alex      (1002) alex      (1003)     4286 2023-05-04 12:19:56.000000 jesth-0.0.7/jesth/section/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 16:37:22.149441 jesth-0.0.7/jesth.egg-info/
--rw-rw-r--   0 alex      (1002) alex      (1003)    29916 2023-05-18 16:37:22.000000 jesth-0.0.7/jesth.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)      704 2023-05-18 16:37:22.000000 jesth-0.0.7/jesth.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-05-18 16:37:22.000000 jesth-0.0.7/jesth.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       47 2023-05-18 16:37:22.000000 jesth-0.0.7/jesth.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2022-05-20 19:25:34.000000 jesth-0.0.7/jesth.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1002) alex      (1003)       12 2023-05-18 16:37:22.000000 jesth-0.0.7/jesth.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:23:56.000000 jesth-0.0.7/pyproject.toml
--rw-rw-r--   0 alex      (1002) alex      (1003)      878 2023-05-18 16:37:22.153441 jesth-0.0.7/setup.cfg
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:23:56.000000 jesth-0.0.7/setup.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 16:37:22.149441 jesth-0.0.7/tests/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-05-20 19:23:56.000000 jesth-0.0.7/tests/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     1362 2023-05-01 07:48:28.000000 jesth-0.0.7/tests/test_box.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    11551 2023-05-17 14:24:54.000000 jesth-0.0.7/tests/test_converter.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     7103 2023-05-01 15:43:57.000000 jesth-0.0.7/tests/test_document.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     8157 2023-05-01 07:48:28.000000 jesth-0.0.7/tests/test_misc.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     3181 2023-05-01 07:48:28.000000 jesth-0.0.7/tests/test_parser.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     1692 2023-05-01 07:48:28.000000 jesth-0.0.7/tests/test_renderer.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      541 2023-05-01 07:48:28.000000 jesth-0.0.7/tests/test_root_imports.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     4086 2023-05-02 21:25:17.000000 jesth-0.0.7/tests/test_section.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-29 22:09:44.777376 jesth-0.0.8/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1082 2023-01-27 15:42:40.000000 jesth-0.0.8/LICENSE
+-rw-rw-r--   0 alex      (1002) alex      (1003)       67 2022-05-20 19:23:56.000000 jesth-0.0.8/MANIFEST.in
+-rw-rw-r--   0 alex      (1002) alex      (1003)    30821 2023-05-29 22:09:44.777376 jesth-0.0.8/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)    30128 2023-05-29 11:55:46.000000 jesth-0.0.8/README.md
+-rw-rw-r--   0 alex      (1002) alex      (1003)        5 2023-05-18 16:37:22.000000 jesth-0.0.8/VERSION
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-29 22:09:44.677375 jesth-0.0.8/jesth/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      522 2023-05-28 07:40:29.000000 jesth-0.0.8/jesth/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      140 2022-05-21 09:50:04.000000 jesth-0.0.8/jesth/__main__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-29 22:09:44.721376 jesth-0.0.8/jesth/box/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1429 2023-05-01 07:48:28.000000 jesth-0.0.8/jesth/box/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-29 22:09:44.737376 jesth-0.0.8/jesth/const/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      139 2023-05-25 21:12:27.000000 jesth-0.0.8/jesth/const/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-29 22:09:44.737376 jesth-0.0.8/jesth/converter/
+-rw-rw-r--   0 alex      (1002) alex      (1003)    42450 2023-05-29 18:15:40.000000 jesth-0.0.8/jesth/converter/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-29 22:09:44.737376 jesth-0.0.8/jesth/document/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     8961 2023-05-29 11:55:46.000000 jesth-0.0.8/jesth/document/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-29 22:09:44.737376 jesth-0.0.8/jesth/error/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      298 2023-05-01 11:22:47.000000 jesth-0.0.8/jesth/error/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-29 22:09:44.749376 jesth-0.0.8/jesth/misc/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     8891 2023-05-28 21:43:09.000000 jesth-0.0.8/jesth/misc/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-29 22:09:44.749376 jesth-0.0.8/jesth/parser/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4075 2023-05-01 15:41:06.000000 jesth-0.0.8/jesth/parser/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-29 22:09:44.749376 jesth-0.0.8/jesth/renderer/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2199 2023-05-09 12:13:04.000000 jesth-0.0.8/jesth/renderer/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-29 22:09:44.749376 jesth-0.0.8/jesth/section/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4566 2023-05-29 11:30:46.000000 jesth-0.0.8/jesth/section/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-29 22:09:44.721376 jesth-0.0.8/jesth.egg-info/
+-rw-rw-r--   0 alex      (1002) alex      (1003)    30821 2023-05-29 22:09:44.000000 jesth-0.0.8/jesth.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)      704 2023-05-29 22:09:44.000000 jesth-0.0.8/jesth.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-05-29 22:09:44.000000 jesth-0.0.8/jesth.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       47 2023-05-29 22:09:44.000000 jesth-0.0.8/jesth.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2022-05-20 19:25:34.000000 jesth-0.0.8/jesth.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1002) alex      (1003)       12 2023-05-29 22:09:44.000000 jesth-0.0.8/jesth.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:23:56.000000 jesth-0.0.8/pyproject.toml
+-rw-rw-r--   0 alex      (1002) alex      (1003)      878 2023-05-29 22:09:44.777376 jesth-0.0.8/setup.cfg
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:23:56.000000 jesth-0.0.8/setup.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-29 22:09:44.777376 jesth-0.0.8/tests/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-05-20 19:23:56.000000 jesth-0.0.8/tests/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1362 2023-05-01 07:48:28.000000 jesth-0.0.8/tests/test_box.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    11555 2023-05-28 07:40:30.000000 jesth-0.0.8/tests/test_converter.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     8799 2023-05-29 11:31:10.000000 jesth-0.0.8/tests/test_document.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     9156 2023-05-28 21:45:51.000000 jesth-0.0.8/tests/test_misc.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3181 2023-05-01 07:48:28.000000 jesth-0.0.8/tests/test_parser.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1692 2023-05-01 07:48:28.000000 jesth-0.0.8/tests/test_renderer.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      543 2023-05-28 07:40:29.000000 jesth-0.0.8/tests/test_root_imports.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4465 2023-05-28 10:23:44.000000 jesth-0.0.8/tests/test_section.py
```

### Comparing `jesth-0.0.7/LICENSE` & `jesth-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jesth-0.0.7/PKG-INFO` & `jesth-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jesth
-Version: 0.0.7
+Version: 0.0.8
 Summary: Next-level human-readable data serialization format
 Home-page: https://github.com/pyrustic/jesth
 Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com
 Maintainer: Pyrustic Evangelist
 Maintainer-email: rusticalex@yahoo.com
 License: MIT
@@ -15,17 +15,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- Cover -->
 <div align="center">
-    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/jesth/cover.png" alt="Demo" width="1380">
+    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/jesth/cover.png" alt="Demo" width="650">
     <p align="center">
-    Jesthfile with 1 top anonymous section, and 2 'user' sections
+    JesthFile with 1 anonymous top section, and 2 'user' sections
     </p>
 </div>
 
 
 <!-- Intro Text -->
 # Jesth
 <b> Next-level human-readable data serialization format </b>
@@ -33,60 +33,62 @@
 This project is part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
 > [Installation](#installation) &nbsp; &nbsp; [Demo](#demo) &nbsp; &nbsp; [Latest](https://github.com/pyrustic/jesth/tags) &nbsp; &nbsp; [Modules](https://github.com/pyrustic/jesth/tree/master/docs/modules#readme)
 
 
 ## Table of contents
 
 - [Overview](#overview)
-- [Why not TOML, YAML, or JSON ?](#why_not_toml_yaml_or_json )
-- [Why use Jesth ?](#why_use_jesth_)
+- [Why not TOML, YAML, or JSON ?](#why-not-toml-yaml-or-json-)
+- [Why use Jesth ?](#why-use-jesth-)
 - [Demo](#demo)
-- [Code snippets for everyday scenarios](#code_snippets_for_everyday_scenarios)
-- [Anatomy of a Section](#anatomy_of_a_Section)
-    - [Base section](#base_section)
-    - [Dict section](#dict_section)
-    - [Section family](#section_family)
-- [Specs of the Dict Section](#specs_of_the_dict_section)
+- [Code snippets for everyday scenarios](#code-snippets-for-everyday-scenarios)
+- [Anatomy of a Section](#anatomy-of-a-section)
+    - [Base section](#base-section)
+    - [Dict section](#dict-section)
+    - [Section family](#section-family)
+- [Specs of the Dict Section](#specs-of-the-dict-section)
     - [Scalars](#scalars)
-    - [Null value](#null_value)
-    - [Single-line strings](#single-line_strings)
-    - [Multi-line strings](#multi-line_strings)
-    - [Date and time](#date_and_time)
-    - [Embedded binary data](#embedded_binary_data)
-    - [Comments and whitespace](#comments_and_whitespace)
-    - [Collections (nested dict and list)](#collections_nested_dict_and_list)
-- [Application programming interface](#application_programming_interface)
-- [Jesth Schema for data validation](#jesth_schema_for_data_validation)
-- [Available implementations](#available_implementations)
+    - [Null value](#null-value)
+    - [Single-line strings](#single-line-strings)
+    - [Multi-line strings](#multi-line-strings)
+    - [Date and time](#date-and-time)
+    - [Embedded binary data](#embedded-binary-data)
+    - [Comments and whitespaces](#comments-and-whitespaces)
+    - [Collections (nested dict and list)](#collections-nested-dict-and-list)
+- [Application programming interface](#application-programming-interface)
+- [Jesth Schema for data validation](#jesth-schema-for-data-validation)
+- [Available implementations](#available-implementations)
 - [Miscellaneous](#miscellaneous)
 - [Contributing](#contributing)
 - [Installation](#installation)
     
 
 # Overview
-**Jesth**, which stands for **Just Extract Sections Then Hack**, is a human-readable data serialization format whose reference parser is an eponymous lightweight Python library available on [PyPI](#installation).
+**Jesth** (pronounced [/dʒest/](https://dictionary.cambridge.org/pronunciation/english/jest)), which stands for **Just Extract Sections Then Hack'em**, is a human-readable data serialization format whose reference parser is an eponymous lightweight [Python](https://www.python.org/) library available on [PyPI](#installation).
+
+> Read the **backstory** in this [HN discussion](https://news.ycombinator.com/item?id=35991018) !
 
 ## Versatile serialization format
 A Jesth **document** is made up of **sections**, each defined by a **header** (between two square brackets) and a **body** which is just lines of text. 
 
 Instead of interpreting these lines upstream after extracting the sections, the Jesth parser lays low and lets the programmer decide which hack to apply to them.
 
 Because of this parsing policy, a single Jesth document can contain an **eclectic set of sections** representing a poem, server configs, help text, [prompts](https://github.com/f/awesome-chatgpt-prompts) for a chatbot, [directed graph](https://en.wikipedia.org/wiki/Directed_graph), [ascii artwork](https://en.wikipedia.org/wiki/ASCII_art), and more.
 
 ## Shipped with a proper and extensively tested hack
-For convenience, the Jesth library includes a proper and extensively tested hack to convert a compatible section into a [dictionary](https://en.wikipedia.org/wiki/Associative_array) data structure. In such a section that allows comments, one can encode strings (single or multi-line), scalars (integer, float, decimal float, complex, booleans), date and time, null value, binary data and nested collections (list and dictionary).
+For convenience, the Jesth library includes a proper and extensively tested [hack]((https://en.wikipedia.org/wiki/Hacker_culture)) to convert a compatible section to a [dictionary](https://en.wikipedia.org/wiki/Associative_array) data structure. In such a section that allows comments, one can encode **strings** (single or multi-line), **scalars** (integer, float, decimal float, complex, booleans), **date** and **time**, **null** value, **binary** data and nested **collections** (list and dictionary).
 
 Therefore, Jesth can be used for configuration files, to create a [scripting language](https://github.com/pyrustic/backstage), to act as a markup language to write [docstrings](https://en.wikipedia.org/wiki/Docstring#Python) so that a tool can generate reference documentation after parsing them, etc.
 
 In the next few sections, we'll dive deep into Jesth, but first, why not [TOML](https://en.wikipedia.org/wiki/TOML), [YAML](https://fr.wikipedia.org/wiki/YAML), or [JSON](https://en.wikipedia.org/wiki/JSON) ?
 
 # Why not TOML, YAML, or JSON ?
 Jesth offers a high level of **versatility** that allows the programmer to freely decide what a section can contain and how to interpret its contents. 
 
-Moreover, whenever the programmer decides to adopt a dictionary as a data structure to formalize some or all sections of a Jesth document, he/she is offered a [very readable and strict syntax](#specs_of_the_dict_section) to encode the data. 
+Moreover, whenever the programmer decides to adopt a dictionary as a data structure to formalize some or all sections of a Jesth document, he/she is offered a [very readable and strict syntax](#specs-of-the-dict-section) to encode the data. 
 
 The library exposes an intuitive API for loading and dumping Dict sections with an option to preserve comments and whitespaces.
 
 The following subsections will briefly compare **TOML**, **YAML**, and **JSON** to **Jesth's dictionary data structure support**.
 
 ## Why not TOML ?
 Jesth shares with **TOML** the use of square brackets to define sections (or tables in TOML terminology), therefore, among other formats, the TOML syntax is closest to Jesth. However, when dealing with nested structures, TOML becomes very confusing, revealing the limitations of its syntax.
@@ -100,23 +102,23 @@
 **JSON** is great because it mimics the way we define data structures in source code. Therefore, it can be minified and is also a reasonable choice for machine-to-machine communication, but it cannot beat the readability of formats that natively support line breaks and/or indentation. In comparison to Jesth, JSON has fewer native data types and no native support for comments.
 
 # Why use Jesth ?
 Jesth is ideal for configuration files, whether intended for use by a standard application or by a chatbot/AI. Personal notes can also benefit from being entered into a Jesth file, so they can be parsed later. As mentioned in the [Overview](#overview) section, Jesth was used to design a [scripting language](https://github.com/pyrustic/backstage) and currently serves as the markup language for [docstrings](https://en.wikipedia.org/wiki/Docstring#Python) in all projects that are part of the [Pyrustic ecosystem](https://pyrustic.github.io).
 
 Loading a Jesth document is stress-free because exceptions are only thrown when you try to convert a non-compatible section to a dictionary. But even that is the strict default behavior of the dictionary converter since you can customize the converter to string invalid values. This specific customization is as simple as this: `value_converter.fallback_decoder = str`
 
-There's more to say, for example the syntax for encoding a dictionary into a JesthFile is text editor/IDE-friendly, so it may benefit from supporting some cool features like the folding mechanism.
+There's more to say, for example the Jesth Dict Section syntax is text editor/IDE-friendly, so it may benefit from supporting some cool features like the folding mechanism.
 
 # Demo
-The demo is a clonable repository containing a Jesthfile and a Python script to load its contents. 
+The demo is a clonable repository containing a JesthFile and a Python script to load its contents. 
 
 > [Open the Demo](https://github.com/pyrustic/jesth-demo#readme) !
 
 # Code snippets for everyday scenarios
-**Load a Jesthfile:**
+**Load a JesthFile:**
 ```python
 from jesth import read
 
 path = "/home/alex/jesthfile"
 document = read(path)
 ```
 
@@ -129,36 +131,40 @@
 
 # get the list of all "user" sections
 user_sections = document.get_all("user")
 
 # show the body of a section
 print(config_section.body)  # list of lines
 
+# show the body as a text (concatenated lines)
+print(config_section.to_text())
+
 # update the body of a section
 new_body = [r"# comment", 
             r"server1 = '1.1.1.1'",
             r"port = 80"]
 config_section.update(new_body)
 ```
 
 **Convert a compatible section into a Python Dict:**
+
 ```python
 ...
 
-# will raise an exception if the section can't be converted into dict
-dict_object = section.make_dict()
+# won't raise an exception if the section can't be converted to dict
+dict_object = section.to_dict()
 
-# won't raise an exception if the section can't be converted into dict
-dict_object = section.get_dict()
+# will raise an exception if the section can't be converted to dict
+dict_object = section.create_dict()
 
-# Note that `.make_dict` accepts `default` and `strict` arguments
+# Note that `.create_dict` accepts `default` and `strict` arguments
 # If the body can be converted to a dict but is empty, you get `default`
 # Set True to `strict` to preserve comments and whitespaces
 
-# Note that `.get_dict` accepts `default`, `strict`, and `fallback`
+# Note that `.to_dict` accepts `default`, `strict`, and `fallback`
 # If the body can't be converted to a dict, you get `fallback`
 ```
 
 **Edit a document:**
 ```python
 ...
 
@@ -174,15 +180,15 @@
 ```
 
 **Save a document:**
 ```python
 from jesth import write
 ...
 
-# if the document is linked to a Jesthfile, call its `save` method
+# if the document is linked to a JesthFile, call its `save` method
 document.save()
 
 # or save to a new path
 document.save_to(path)
 
 # Under the hood, the Document class actually uses the `write` function
 write(document, path)
@@ -190,15 +196,15 @@
 
 **Render a document:**
 ```python
 from jesth import render
 ...
 
 # return the string representation of the data
-# this jesth text can be stored as it in a Jesthfile
+# this jesth text can be stored as it in a JesthFile
 jesth_text = document.render()
 
 # Under the hood, the Document class actually uses the `render` function
 jesth_text = render(document)
 ```
 
 # Anatomy of a Section
@@ -241,38 +247,38 @@
 Is called Base section a section as defined in the document, without any transformation, i.e., just text lines. From the source code perspective, the body of such section is represented by default as a list of lines (string). 
 
 The alternative representation of such body is just a concatenated version of this list.
 
 ## Dict section
 Is called Dict section, a section that is intended to be converted into a dictionary object by the parser. 
 
-By default, the library uses the `OrderedDict` class to represent the body of such section, thus, the order of key/value is preserved. This default behavior can be customized through the `ValueConverter` object.
+By default, the library uses the regular `dict` type to represent the body of such section. This default behavior can be customized through the `ValueConverter` object.
 
 ## Section family
-Different sections can have the same header. In this case, they belong to a section family. By default, the `.get(header)` method from the `Document` class returns the last defined section with the given header argument. This method actually accepts an `index` argument which is set to `-1` by default to align with Python convention to access the last item of a sequence.
+Different sections can have the same header. In this case, they belong to a **section family**. By default, the `.get(header)` method from the `Document` class returns the first defined section with the given header argument. This method actually accepts a `sub_index` argument which is set to `0` by default to access the first item of the section family.
 
 **Get the 2nd section in the 'user' section family:**
 
 ```python
 ...
 
-section = document.get("user", index=1)
+section = document.get("user", sub_index=1)
 ```
 
 **Get the list of all sections in the 'user' section family:**
 ```python
 ...
 
 sections = document.get_all("user")
 ```
 
 # Specs of the Dict Section
 The specs for a Dictionary Section are mostly aligned with Python specs. For example, a Jesth Integer follows exactly the definition of Python Integer. 
 
-> **Note:** The Jesth library allows the customization of each type of data as well in the context of parsing or in the context of rendering. This customization is made via the [ValueConverter](#the_valueconverter_object) object
+> **Note:** The Jesth library allows the customization of each type of data as well in the context of parsing or in the context of rendering. This customization is made via the [ValueConverter](#the-valueconverter-object) object
 
 ## Scalars
 Jesth supports integers (base 10, hexadecimal, octal, binary), float (approximate binary floating-point, fixed-precision decimal floating-point), complex numbers, and booleans.
 
 > **Note:** Jesth Scalars specs are aligned with their respective Python equivalent specs.
 
 ### Integer
@@ -455,15 +461,15 @@
 
 |Jesth|Python|
 |---|---|
 |bin (base64)|`bytes`|
 
 
 ## Comments and whitespaces
-Jesth Dict Section supports comments which are strings starting with `#`. Comments and Whitespaces can be preserved while converting a Jesth Dict Section into a Python Dictionary (OrderedDict to be precise).
+Jesth Dict Section supports comments which are strings starting with `#`. Comments and Whitespaces can be preserved while converting a Jesth Dict Section into a Python Dictionary.
 **Example with comments and whitespaces:**
 ```
 # this is a comment
 key = "value"
 
 # another comment
 number = 42
@@ -496,18 +502,18 @@
         (dict)
             project = "jesth"
             number = 42
 ```
 
 **Mapping with actual Python objects:**
 
-|Jesth|Python|
-|---|---|
-|dict|`collections.OrderedDict`|
-|list|`list`|
+|Jesth| Python |
+|---|--------|
+|dict| `dict` |
+|list| `list` |
 
 # Application programming interface
 The library exposes functions and classes to load and dump Jesth document with optional customization at each stage. Loaded documents and their sections are encapsulated into classes exposing methods and properties with a high emphasis on ergonomy.
 
 ## Loading Jesth
 To load Jesth data, one may use the `jesth.parser.read` function when the source is a file (file-like object, path string, or pathlib.Path object), or `jesth.parser.parse` function when the source is a string.
 
@@ -576,52 +582,56 @@
 > **Properties:** `path`, `sections`, `value_converter`, and `headers`. 
 
 
 ### Edit a document
 The document object exposes `append`, `insert`, `remove`, and `remove_all` methods to add and remove sections.
 
 **Example:**
+
 ```python
 from jesth import read
 
 path = "/path/to/jestfile"
 document = read(path)
 
 # append a new section to the document
 body = ["line 1", "line 2", "line 3"]
 document.append("header", body=body)  # body may be a dict or string
 
 # insert an empty section at a specific index
 document.insert(0, "header")  # therefore, first section
+# override the first section with a new empty one
+document.set(0, "header")  # 'body' is still set to None here
 
 # remove the last section with a specific header
-document.remove("header")  # index defaults to -1
+document.remove("header")  # sub_index defaults to -1
 # remove the first section with a specific header
-document.remove("header", index=0)
+document.remove("header", sub_index=0)
 # note that the index argument is meant to be relative
 # to this 'section family', i.e., sections with same header.
 
 # remove all sections by header
 document.remove_all("header")
 ```
 
 ### Query a document
 The document object exposes `get`, `get_all`, and `count` methods to retrieve sections or their count.
 
 **Example:**
+
 ```python
 from jesth import read
 
 path = "/path/to/jestfile"
 document = read(path)
 
-# get the last section with a specific header
-section = document.get("header")  # the index arg defaults to -1
 # get the first section with a specific header
-section = document.get("header", index=0) 
+section = document.get("header")  # the index arg defaults to 0
+# get the last section with a specific header
+section = document.get("header", sub_index=-1)
 # note that the index argument is meant to be relative
 # to this 'section family', i.e., sections with same header.
 
 # get all sections with a specific header
 sections = document.get_all("header")
 
 # count the number of sections sharing a specific header
@@ -631,33 +641,37 @@
 ## The Section object
 The Section object contains the header and the body of a section. The body is stored as a list of string that may be converted on demand, if compatible, into a Python dictionary.
 
 > **Properties:** `header`, `body`, and `value_converter`.
 
 
 **Example:**
+
 ```python
 from jesth import read
 
 path = "/path/to/jestfile"
 document = read(path)
 section = document.get("header")
 
 # Convert the body of this section into a dict then return it.
+# Beware, this method won't raise an exception at all
+# instead, it may return a fallback value
+data = section.to_dict()  # accepts "default", "fallback", "strict"
+
+# Concatenate the lines of the body to form a text string
+data = section.to_text()
+
+# Convert the body of this section into a dict then return it.
 # Beware, this method will raise an exception if the conversion fails
-data = section.make_dict()  # accepts "default" and "strict"
+data = section.create_dict()  # accepts "default" and "strict"
 # the default parameter is for default data if the new created dict
 # is empty. The strict parameter is to tell whether comment/whitespace
 # should be preserved and inserted in the new dict !
 
-# Convert the body of this section into a dict then return it.
-# Beware, this method won't raise an exception at all
-# instead, it may return a fallback value
-data = section.get_dict()  # accepts "default", "fallback", "strict"
-
 # update the body of this section
 body = ["line 1", "line 2", "line 3"]
 section.update(body)  # here, body may be a string or a dict
 ```
 
 ## The ValueConverter object
 This object has methods to encode and decode values, and also properties to customize conversion types. 
@@ -665,15 +679,15 @@
 Most time, you won't need to set or edit this object. The encode and decode methods of this object are only useful for test purpose.
 
 **Parameters:**
 - **dict_type**: the Python type in which a Jesth Dict should be converted into. Defaults to Python dict type.
 
 - **list_type**: the Python type in which a Jesth List should be converted into. Defaults to Python list type.
 
-- **XXX_types**: this represents a group of parameters. Here, XXX is a placeholder for a Jesth data type. Valid types are: dict, list, bin, bool, complex, date, datetime, float, integer, raw, string, text, time. Examples: dict_types, float_types, and time_types. Use this parameter to set a list of Python types that may be encoded in the Jesth type (the same used as prefix). Example: dict_types defaults to [OrderedDict, dict], i.e., while encoding some Python data, an OrderedDict instance or a regular dict instance will be encoded as a Jesth dict.
+- **XXX_types**: this represents a group of parameters. Here, XXX is a placeholder for a Jesth data type. Valid types are: dict, list, bin, bool, complex, date, datetime, float, integer, raw, string, text, time. Examples: dict_types, float_types, and time_types. Use this parameter to set a list of Python types that may be encoded in the Jesth type (the same used as prefix). Example: dict_types defaults to [dict, OrderedDict], i.e., while encoding some Python data, an OrderedDict instance or a regular dict instance will be encoded as a Jesth dict.
 
 - **XXX_encoder**: this represents a group of parameters. Here, XXX is a placeholder for one of: bin, bool, complex, date, datetime, float, integer, null, raw, string, text, time, fallback. Use these parameters to set a callable to encode Python values into Jesth values. Example: float_encoder = decimal.Decimal
 
 - **XXX_decoder**: this represents a group of parameters. Here, XXX is a placeholder for one of: bin, bool, complex, date, datetime, float, integer, null, raw, string, text, time, fallback. Use these parameters to set a callable to decode Jesth values into Python values. Example: integer_decoder = int
 
 > **Note:** the parameters of ValueConverter are mirrored as read and write properties.
 
@@ -685,15 +699,15 @@
 For the moment, the only available implementation of Jesth is this reference library written in Python. 
 If you are interested into writing a Jesth library for another language (Rust, C#, Java, JavaScript, PHP, etc), feel free to get in touch with [me](https://pyrustic.github.io/#contact) for any question !
 
 # Miscellaneous
 Collection of miscellaneous notes.
 
 ## Acronymy
-Jesth stands for Just Extract Sections Then Hack.
+Jesth stands for **Just Extract Sections Then Hack'em**. Here, the word `hack` is a direct reference to the [Hacker culture](https://en.wikipedia.org/wiki/Hacker_culture).
 
 ## End of document
 To tell the parser to stop parsing a document, input in the document the `[[END]]` (case-insensitive) tag on its own line.
 
 ## Opening square bracket at the beginning of a line
 You must escape the opening square brackets at the start of a line of a body with a backslash `\` character. And whenever your line needs to start with `n` backslash(es) followed by an opening square bracket, you need to prepend an extra backslash to the line, resulting in `n+1` backslash(es).
 
@@ -712,14 +726,15 @@
 
 ## Beautiful cover image
 The beautiful cover image is made with the amazing [carbon app](https://carbon.now.sh).
 
 # Contributing
 Feel free to open an issue to report a bug, suggest some changes, show some useful code snippets, or discuss anything related to this project. You can also directly email [me](https://pyrustic.github.io/#contact).
 
+> **Note:** I would like to automate a decent Git workflow (branching, merging patches, all the basic cool things cool kids do) with [Backstage](https://github.com/pyrustic/backstage). In the meantime, I will manually incorporate the fixes into the only existing branch (`master`). Thank you for your understanding !
 
 ## Setup your development environment
 Following are instructions to setup your development environment
 
 ```bash
 # create and activate a virtual environment
 python -m venv venv
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jesth-0.0.7/README.md` & `jesth-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!-- Cover -->
 <div align="center">
-    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/jesth/cover.png" alt="Demo" width="1380">
+    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/jesth/cover.png" alt="Demo" width="650">
     <p align="center">
-    Jesthfile with 1 top anonymous section, and 2 'user' sections
+    JesthFile with 1 anonymous top section, and 2 'user' sections
     </p>
 </div>
 
 
 <!-- Intro Text -->
 # Jesth
 <b> Next-level human-readable data serialization format </b>
@@ -14,60 +14,62 @@
 This project is part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
 > [Installation](#installation) &nbsp; &nbsp; [Demo](#demo) &nbsp; &nbsp; [Latest](https://github.com/pyrustic/jesth/tags) &nbsp; &nbsp; [Modules](https://github.com/pyrustic/jesth/tree/master/docs/modules#readme)
 
 
 ## Table of contents
 
 - [Overview](#overview)
-- [Why not TOML, YAML, or JSON ?](#why_not_toml_yaml_or_json )
-- [Why use Jesth ?](#why_use_jesth_)
+- [Why not TOML, YAML, or JSON ?](#why-not-toml-yaml-or-json-)
+- [Why use Jesth ?](#why-use-jesth-)
 - [Demo](#demo)
-- [Code snippets for everyday scenarios](#code_snippets_for_everyday_scenarios)
-- [Anatomy of a Section](#anatomy_of_a_Section)
-    - [Base section](#base_section)
-    - [Dict section](#dict_section)
-    - [Section family](#section_family)
-- [Specs of the Dict Section](#specs_of_the_dict_section)
+- [Code snippets for everyday scenarios](#code-snippets-for-everyday-scenarios)
+- [Anatomy of a Section](#anatomy-of-a-section)
+    - [Base section](#base-section)
+    - [Dict section](#dict-section)
+    - [Section family](#section-family)
+- [Specs of the Dict Section](#specs-of-the-dict-section)
     - [Scalars](#scalars)
-    - [Null value](#null_value)
-    - [Single-line strings](#single-line_strings)
-    - [Multi-line strings](#multi-line_strings)
-    - [Date and time](#date_and_time)
-    - [Embedded binary data](#embedded_binary_data)
-    - [Comments and whitespace](#comments_and_whitespace)
-    - [Collections (nested dict and list)](#collections_nested_dict_and_list)
-- [Application programming interface](#application_programming_interface)
-- [Jesth Schema for data validation](#jesth_schema_for_data_validation)
-- [Available implementations](#available_implementations)
+    - [Null value](#null-value)
+    - [Single-line strings](#single-line-strings)
+    - [Multi-line strings](#multi-line-strings)
+    - [Date and time](#date-and-time)
+    - [Embedded binary data](#embedded-binary-data)
+    - [Comments and whitespaces](#comments-and-whitespaces)
+    - [Collections (nested dict and list)](#collections-nested-dict-and-list)
+- [Application programming interface](#application-programming-interface)
+- [Jesth Schema for data validation](#jesth-schema-for-data-validation)
+- [Available implementations](#available-implementations)
 - [Miscellaneous](#miscellaneous)
 - [Contributing](#contributing)
 - [Installation](#installation)
     
 
 # Overview
-**Jesth**, which stands for **Just Extract Sections Then Hack**, is a human-readable data serialization format whose reference parser is an eponymous lightweight Python library available on [PyPI](#installation).
+**Jesth** (pronounced [/dʒest/](https://dictionary.cambridge.org/pronunciation/english/jest)), which stands for **Just Extract Sections Then Hack'em**, is a human-readable data serialization format whose reference parser is an eponymous lightweight [Python](https://www.python.org/) library available on [PyPI](#installation).
+
+> Read the **backstory** in this [HN discussion](https://news.ycombinator.com/item?id=35991018) !
 
 ## Versatile serialization format
 A Jesth **document** is made up of **sections**, each defined by a **header** (between two square brackets) and a **body** which is just lines of text. 
 
 Instead of interpreting these lines upstream after extracting the sections, the Jesth parser lays low and lets the programmer decide which hack to apply to them.
 
 Because of this parsing policy, a single Jesth document can contain an **eclectic set of sections** representing a poem, server configs, help text, [prompts](https://github.com/f/awesome-chatgpt-prompts) for a chatbot, [directed graph](https://en.wikipedia.org/wiki/Directed_graph), [ascii artwork](https://en.wikipedia.org/wiki/ASCII_art), and more.
 
 ## Shipped with a proper and extensively tested hack
-For convenience, the Jesth library includes a proper and extensively tested hack to convert a compatible section into a [dictionary](https://en.wikipedia.org/wiki/Associative_array) data structure. In such a section that allows comments, one can encode strings (single or multi-line), scalars (integer, float, decimal float, complex, booleans), date and time, null value, binary data and nested collections (list and dictionary).
+For convenience, the Jesth library includes a proper and extensively tested [hack]((https://en.wikipedia.org/wiki/Hacker_culture)) to convert a compatible section to a [dictionary](https://en.wikipedia.org/wiki/Associative_array) data structure. In such a section that allows comments, one can encode **strings** (single or multi-line), **scalars** (integer, float, decimal float, complex, booleans), **date** and **time**, **null** value, **binary** data and nested **collections** (list and dictionary).
 
 Therefore, Jesth can be used for configuration files, to create a [scripting language](https://github.com/pyrustic/backstage), to act as a markup language to write [docstrings](https://en.wikipedia.org/wiki/Docstring#Python) so that a tool can generate reference documentation after parsing them, etc.
 
 In the next few sections, we'll dive deep into Jesth, but first, why not [TOML](https://en.wikipedia.org/wiki/TOML), [YAML](https://fr.wikipedia.org/wiki/YAML), or [JSON](https://en.wikipedia.org/wiki/JSON) ?
 
 # Why not TOML, YAML, or JSON ?
 Jesth offers a high level of **versatility** that allows the programmer to freely decide what a section can contain and how to interpret its contents. 
 
-Moreover, whenever the programmer decides to adopt a dictionary as a data structure to formalize some or all sections of a Jesth document, he/she is offered a [very readable and strict syntax](#specs_of_the_dict_section) to encode the data. 
+Moreover, whenever the programmer decides to adopt a dictionary as a data structure to formalize some or all sections of a Jesth document, he/she is offered a [very readable and strict syntax](#specs-of-the-dict-section) to encode the data. 
 
 The library exposes an intuitive API for loading and dumping Dict sections with an option to preserve comments and whitespaces.
 
 The following subsections will briefly compare **TOML**, **YAML**, and **JSON** to **Jesth's dictionary data structure support**.
 
 ## Why not TOML ?
 Jesth shares with **TOML** the use of square brackets to define sections (or tables in TOML terminology), therefore, among other formats, the TOML syntax is closest to Jesth. However, when dealing with nested structures, TOML becomes very confusing, revealing the limitations of its syntax.
@@ -81,23 +83,23 @@
 **JSON** is great because it mimics the way we define data structures in source code. Therefore, it can be minified and is also a reasonable choice for machine-to-machine communication, but it cannot beat the readability of formats that natively support line breaks and/or indentation. In comparison to Jesth, JSON has fewer native data types and no native support for comments.
 
 # Why use Jesth ?
 Jesth is ideal for configuration files, whether intended for use by a standard application or by a chatbot/AI. Personal notes can also benefit from being entered into a Jesth file, so they can be parsed later. As mentioned in the [Overview](#overview) section, Jesth was used to design a [scripting language](https://github.com/pyrustic/backstage) and currently serves as the markup language for [docstrings](https://en.wikipedia.org/wiki/Docstring#Python) in all projects that are part of the [Pyrustic ecosystem](https://pyrustic.github.io).
 
 Loading a Jesth document is stress-free because exceptions are only thrown when you try to convert a non-compatible section to a dictionary. But even that is the strict default behavior of the dictionary converter since you can customize the converter to string invalid values. This specific customization is as simple as this: `value_converter.fallback_decoder = str`
 
-There's more to say, for example the syntax for encoding a dictionary into a JesthFile is text editor/IDE-friendly, so it may benefit from supporting some cool features like the folding mechanism.
+There's more to say, for example the Jesth Dict Section syntax is text editor/IDE-friendly, so it may benefit from supporting some cool features like the folding mechanism.
 
 # Demo
-The demo is a clonable repository containing a Jesthfile and a Python script to load its contents. 
+The demo is a clonable repository containing a JesthFile and a Python script to load its contents. 
 
 > [Open the Demo](https://github.com/pyrustic/jesth-demo#readme) !
 
 # Code snippets for everyday scenarios
-**Load a Jesthfile:**
+**Load a JesthFile:**
 ```python
 from jesth import read
 
 path = "/home/alex/jesthfile"
 document = read(path)
 ```
 
@@ -110,36 +112,40 @@
 
 # get the list of all "user" sections
 user_sections = document.get_all("user")
 
 # show the body of a section
 print(config_section.body)  # list of lines
 
+# show the body as a text (concatenated lines)
+print(config_section.to_text())
+
 # update the body of a section
 new_body = [r"# comment", 
             r"server1 = '1.1.1.1'",
             r"port = 80"]
 config_section.update(new_body)
 ```
 
 **Convert a compatible section into a Python Dict:**
+
 ```python
 ...
 
-# will raise an exception if the section can't be converted into dict
-dict_object = section.make_dict()
+# won't raise an exception if the section can't be converted to dict
+dict_object = section.to_dict()
 
-# won't raise an exception if the section can't be converted into dict
-dict_object = section.get_dict()
+# will raise an exception if the section can't be converted to dict
+dict_object = section.create_dict()
 
-# Note that `.make_dict` accepts `default` and `strict` arguments
+# Note that `.create_dict` accepts `default` and `strict` arguments
 # If the body can be converted to a dict but is empty, you get `default`
 # Set True to `strict` to preserve comments and whitespaces
 
-# Note that `.get_dict` accepts `default`, `strict`, and `fallback`
+# Note that `.to_dict` accepts `default`, `strict`, and `fallback`
 # If the body can't be converted to a dict, you get `fallback`
 ```
 
 **Edit a document:**
 ```python
 ...
 
@@ -155,15 +161,15 @@
 ```
 
 **Save a document:**
 ```python
 from jesth import write
 ...
 
-# if the document is linked to a Jesthfile, call its `save` method
+# if the document is linked to a JesthFile, call its `save` method
 document.save()
 
 # or save to a new path
 document.save_to(path)
 
 # Under the hood, the Document class actually uses the `write` function
 write(document, path)
@@ -171,15 +177,15 @@
 
 **Render a document:**
 ```python
 from jesth import render
 ...
 
 # return the string representation of the data
-# this jesth text can be stored as it in a Jesthfile
+# this jesth text can be stored as it in a JesthFile
 jesth_text = document.render()
 
 # Under the hood, the Document class actually uses the `render` function
 jesth_text = render(document)
 ```
 
 # Anatomy of a Section
@@ -222,38 +228,38 @@
 Is called Base section a section as defined in the document, without any transformation, i.e., just text lines. From the source code perspective, the body of such section is represented by default as a list of lines (string). 
 
 The alternative representation of such body is just a concatenated version of this list.
 
 ## Dict section
 Is called Dict section, a section that is intended to be converted into a dictionary object by the parser. 
 
-By default, the library uses the `OrderedDict` class to represent the body of such section, thus, the order of key/value is preserved. This default behavior can be customized through the `ValueConverter` object.
+By default, the library uses the regular `dict` type to represent the body of such section. This default behavior can be customized through the `ValueConverter` object.
 
 ## Section family
-Different sections can have the same header. In this case, they belong to a section family. By default, the `.get(header)` method from the `Document` class returns the last defined section with the given header argument. This method actually accepts an `index` argument which is set to `-1` by default to align with Python convention to access the last item of a sequence.
+Different sections can have the same header. In this case, they belong to a **section family**. By default, the `.get(header)` method from the `Document` class returns the first defined section with the given header argument. This method actually accepts a `sub_index` argument which is set to `0` by default to access the first item of the section family.
 
 **Get the 2nd section in the 'user' section family:**
 
 ```python
 ...
 
-section = document.get("user", index=1)
+section = document.get("user", sub_index=1)
 ```
 
 **Get the list of all sections in the 'user' section family:**
 ```python
 ...
 
 sections = document.get_all("user")
 ```
 
 # Specs of the Dict Section
 The specs for a Dictionary Section are mostly aligned with Python specs. For example, a Jesth Integer follows exactly the definition of Python Integer. 
 
-> **Note:** The Jesth library allows the customization of each type of data as well in the context of parsing or in the context of rendering. This customization is made via the [ValueConverter](#the_valueconverter_object) object
+> **Note:** The Jesth library allows the customization of each type of data as well in the context of parsing or in the context of rendering. This customization is made via the [ValueConverter](#the-valueconverter-object) object
 
 ## Scalars
 Jesth supports integers (base 10, hexadecimal, octal, binary), float (approximate binary floating-point, fixed-precision decimal floating-point), complex numbers, and booleans.
 
 > **Note:** Jesth Scalars specs are aligned with their respective Python equivalent specs.
 
 ### Integer
@@ -436,15 +442,15 @@
 
 |Jesth|Python|
 |---|---|
 |bin (base64)|`bytes`|
 
 
 ## Comments and whitespaces
-Jesth Dict Section supports comments which are strings starting with `#`. Comments and Whitespaces can be preserved while converting a Jesth Dict Section into a Python Dictionary (OrderedDict to be precise).
+Jesth Dict Section supports comments which are strings starting with `#`. Comments and Whitespaces can be preserved while converting a Jesth Dict Section into a Python Dictionary.
 **Example with comments and whitespaces:**
 ```
 # this is a comment
 key = "value"
 
 # another comment
 number = 42
@@ -477,18 +483,18 @@
         (dict)
             project = "jesth"
             number = 42
 ```
 
 **Mapping with actual Python objects:**
 
-|Jesth|Python|
-|---|---|
-|dict|`collections.OrderedDict`|
-|list|`list`|
+|Jesth| Python |
+|---|--------|
+|dict| `dict` |
+|list| `list` |
 
 # Application programming interface
 The library exposes functions and classes to load and dump Jesth document with optional customization at each stage. Loaded documents and their sections are encapsulated into classes exposing methods and properties with a high emphasis on ergonomy.
 
 ## Loading Jesth
 To load Jesth data, one may use the `jesth.parser.read` function when the source is a file (file-like object, path string, or pathlib.Path object), or `jesth.parser.parse` function when the source is a string.
 
@@ -557,52 +563,56 @@
 > **Properties:** `path`, `sections`, `value_converter`, and `headers`. 
 
 
 ### Edit a document
 The document object exposes `append`, `insert`, `remove`, and `remove_all` methods to add and remove sections.
 
 **Example:**
+
 ```python
 from jesth import read
 
 path = "/path/to/jestfile"
 document = read(path)
 
 # append a new section to the document
 body = ["line 1", "line 2", "line 3"]
 document.append("header", body=body)  # body may be a dict or string
 
 # insert an empty section at a specific index
 document.insert(0, "header")  # therefore, first section
+# override the first section with a new empty one
+document.set(0, "header")  # 'body' is still set to None here
 
 # remove the last section with a specific header
-document.remove("header")  # index defaults to -1
+document.remove("header")  # sub_index defaults to -1
 # remove the first section with a specific header
-document.remove("header", index=0)
+document.remove("header", sub_index=0)
 # note that the index argument is meant to be relative
 # to this 'section family', i.e., sections with same header.
 
 # remove all sections by header
 document.remove_all("header")
 ```
 
 ### Query a document
 The document object exposes `get`, `get_all`, and `count` methods to retrieve sections or their count.
 
 **Example:**
+
 ```python
 from jesth import read
 
 path = "/path/to/jestfile"
 document = read(path)
 
-# get the last section with a specific header
-section = document.get("header")  # the index arg defaults to -1
 # get the first section with a specific header
-section = document.get("header", index=0) 
+section = document.get("header")  # the index arg defaults to 0
+# get the last section with a specific header
+section = document.get("header", sub_index=-1)
 # note that the index argument is meant to be relative
 # to this 'section family', i.e., sections with same header.
 
 # get all sections with a specific header
 sections = document.get_all("header")
 
 # count the number of sections sharing a specific header
@@ -612,33 +622,37 @@
 ## The Section object
 The Section object contains the header and the body of a section. The body is stored as a list of string that may be converted on demand, if compatible, into a Python dictionary.
 
 > **Properties:** `header`, `body`, and `value_converter`.
 
 
 **Example:**
+
 ```python
 from jesth import read
 
 path = "/path/to/jestfile"
 document = read(path)
 section = document.get("header")
 
 # Convert the body of this section into a dict then return it.
+# Beware, this method won't raise an exception at all
+# instead, it may return a fallback value
+data = section.to_dict()  # accepts "default", "fallback", "strict"
+
+# Concatenate the lines of the body to form a text string
+data = section.to_text()
+
+# Convert the body of this section into a dict then return it.
 # Beware, this method will raise an exception if the conversion fails
-data = section.make_dict()  # accepts "default" and "strict"
+data = section.create_dict()  # accepts "default" and "strict"
 # the default parameter is for default data if the new created dict
 # is empty. The strict parameter is to tell whether comment/whitespace
 # should be preserved and inserted in the new dict !
 
-# Convert the body of this section into a dict then return it.
-# Beware, this method won't raise an exception at all
-# instead, it may return a fallback value
-data = section.get_dict()  # accepts "default", "fallback", "strict"
-
 # update the body of this section
 body = ["line 1", "line 2", "line 3"]
 section.update(body)  # here, body may be a string or a dict
 ```
 
 ## The ValueConverter object
 This object has methods to encode and decode values, and also properties to customize conversion types. 
@@ -646,15 +660,15 @@
 Most time, you won't need to set or edit this object. The encode and decode methods of this object are only useful for test purpose.
 
 **Parameters:**
 - **dict_type**: the Python type in which a Jesth Dict should be converted into. Defaults to Python dict type.
 
 - **list_type**: the Python type in which a Jesth List should be converted into. Defaults to Python list type.
 
-- **XXX_types**: this represents a group of parameters. Here, XXX is a placeholder for a Jesth data type. Valid types are: dict, list, bin, bool, complex, date, datetime, float, integer, raw, string, text, time. Examples: dict_types, float_types, and time_types. Use this parameter to set a list of Python types that may be encoded in the Jesth type (the same used as prefix). Example: dict_types defaults to [OrderedDict, dict], i.e., while encoding some Python data, an OrderedDict instance or a regular dict instance will be encoded as a Jesth dict.
+- **XXX_types**: this represents a group of parameters. Here, XXX is a placeholder for a Jesth data type. Valid types are: dict, list, bin, bool, complex, date, datetime, float, integer, raw, string, text, time. Examples: dict_types, float_types, and time_types. Use this parameter to set a list of Python types that may be encoded in the Jesth type (the same used as prefix). Example: dict_types defaults to [dict, OrderedDict], i.e., while encoding some Python data, an OrderedDict instance or a regular dict instance will be encoded as a Jesth dict.
 
 - **XXX_encoder**: this represents a group of parameters. Here, XXX is a placeholder for one of: bin, bool, complex, date, datetime, float, integer, null, raw, string, text, time, fallback. Use these parameters to set a callable to encode Python values into Jesth values. Example: float_encoder = decimal.Decimal
 
 - **XXX_decoder**: this represents a group of parameters. Here, XXX is a placeholder for one of: bin, bool, complex, date, datetime, float, integer, null, raw, string, text, time, fallback. Use these parameters to set a callable to decode Jesth values into Python values. Example: integer_decoder = int
 
 > **Note:** the parameters of ValueConverter are mirrored as read and write properties.
 
@@ -666,15 +680,15 @@
 For the moment, the only available implementation of Jesth is this reference library written in Python. 
 If you are interested into writing a Jesth library for another language (Rust, C#, Java, JavaScript, PHP, etc), feel free to get in touch with [me](https://pyrustic.github.io/#contact) for any question !
 
 # Miscellaneous
 Collection of miscellaneous notes.
 
 ## Acronymy
-Jesth stands for Just Extract Sections Then Hack.
+Jesth stands for **Just Extract Sections Then Hack'em**. Here, the word `hack` is a direct reference to the [Hacker culture](https://en.wikipedia.org/wiki/Hacker_culture).
 
 ## End of document
 To tell the parser to stop parsing a document, input in the document the `[[END]]` (case-insensitive) tag on its own line.
 
 ## Opening square bracket at the beginning of a line
 You must escape the opening square brackets at the start of a line of a body with a backslash `\` character. And whenever your line needs to start with `n` backslash(es) followed by an opening square bracket, you need to prepend an extra backslash to the line, resulting in `n+1` backslash(es).
 
@@ -693,14 +707,15 @@
 
 ## Beautiful cover image
 The beautiful cover image is made with the amazing [carbon app](https://carbon.now.sh).
 
 # Contributing
 Feel free to open an issue to report a bug, suggest some changes, show some useful code snippets, or discuss anything related to this project. You can also directly email [me](https://pyrustic.github.io/#contact).
 
+> **Note:** I would like to automate a decent Git workflow (branching, merging patches, all the basic cool things cool kids do) with [Backstage](https://github.com/pyrustic/backstage). In the meantime, I will manually incorporate the fixes into the only existing branch (`master`). Thank you for your understanding !
 
 ## Setup your development environment
 Following are instructions to setup your development environment
 
 ```bash
 # create and activate a virtual environment
 python -m venv venv
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jesth-0.0.7/jesth/__init__.py` & `jesth-0.0.8/jesth/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """For convenience, this module exposes main classes and functions of the library"""
 from jesth.document import Document
 from jesth.section import Section
 from jesth.parser import read, parse, Parser
 from jesth.renderer import render, write
-from jesth.converter import make_dict, flatten_dict, ValueConverter
+from jesth.converter import create_dict, flatten_dict, ValueConverter
 from jesth.misc import split_key_value
 
 
 __all__ = ["Document", "Section", "parse", "render", "read", "write",
-           "make_dict", "flatten_dict", "ValueConverter", "split_key_value",
+           "create_dict", "flatten_dict", "ValueConverter", "split_key_value",
            "Parser"]
```

### Comparing `jesth-0.0.7/jesth/box/__init__.py` & `jesth-0.0.8/jesth/box/__init__.py`

 * *Files identical despite different names*

### Comparing `jesth-0.0.7/jesth/converter/__init__.py` & `jesth-0.0.8/jesth/converter/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from decimal import Decimal
 from collections import OrderedDict, namedtuple
 from jesth import error, misc, const
 from jesth.box import HexInt, OctInt, BinInt, RawString,\
     Text, RawText, CommentID, Comment, WhitespaceID, Whitespace
 
 
-def make_dict(body, value_converter=None, strict=True):
+def create_dict(body, value_converter=None, strict=True):
     """
     Convert a section body into a Python dict
 
     [parameters]
     - body: string or list of strings
     - value_converter: instance of ValueConverter to customize value encoding
     - strict: when strict is True, comments and whitespaces aren't preserved
 
     [return]
-    Returns a Python dict (OrderedDict by default, customizable with ValueConverter)
+    Returns a Python dict (type customizable with ValueConverter)
 
     [exceptions]
     - jesth.error.ConversionError: raised when an error occured while doing conversion
     """
     value_converter = value_converter if value_converter else ValueConverter()
     # base form (as a regular string)
     if isinstance(body, str):
@@ -31,44 +31,43 @@
 
 
 def flatten_dict(data, value_converter=None):
     """
     Convert a Python dict into a list of strings (section body in the base form)
 
     [parameters]
-    - data: Python dict (I do recommend an OrderedDict)
+    - data: Python dict
     - value_converter: instance of ValueConverter to customize value encoding
 
     [return]
     Returns a list of strings
     """
     value_converter = value_converter if value_converter else ValueConverter()
     return DictToBase.run(data, value_converter)
 
 
 class BaseToDict:
     @staticmethod
     def run(lines, value_converter=None, strict=True):
         value_converter = value_converter if value_converter else ValueConverter()
         stack = list()
-        #root_container = OrderedDict()
         root_container = value_converter.dict_type()
         root_context = Context("dict", root_container, 0)
         stack.append(root_context)
         for lineno, line in enumerate(lines):
             # remove line breaks
             line = line.replace("\n", "\\n")
             context = stack[-1]
             line, indents = BaseToDict._prepare_line(line, context)
             # same indent
             if indents == context.indents:
                 pass
             # lower indent
             elif indents < context.indents:
-                BaseToDict._cleanup_stack(stack, value_converter, indents)
+                BaseToDict._cleanup_stack(stack, value_converter, indents, strict)
             # exaggerated forward indent
             else:
                 msg = "Expected {} or less indents at line '{}'"
                 msg = msg.format(context.indents, line)
                 raise error.IndentError(msg)
             # process line
             try:
@@ -77,15 +76,15 @@
             except Exception as e:
                 msg = "Error on line {}: {}{}"
                 str_e = str(e)
                 str_e = ": " + str_e if str_e else str_e
                 msg = msg.format(lineno+1, type(e).__name__, str_e)
                 raise type(e)(msg)
         # cleanup stack
-        BaseToDict._cleanup_stack(stack, value_converter, 0)
+        BaseToDict._cleanup_stack(stack, value_converter, 0, strict)
         # end
         #return BaseToDict._finalize_root_dict(root_context, value_converter)
         return root_container
 
     @staticmethod
     def _prepare_line(line, context):
         indent_width = const.INDENT_WIDTH
@@ -176,66 +175,66 @@
     @staticmethod
     def _update_stack(stack, container_name,
                       container, indents):
         new_context = Context(container_name, container, indents)
         stack.append(new_context)
 
     @staticmethod
-    def _cleanup_stack(stack, value_converter, indents):
+    def _cleanup_stack(stack, value_converter, indents, strict):
         if not stack:
             return
         while True:
             if len(stack) == 1:
                 break
             context = stack[-1]
             parent_context = stack[-2]
             if indents >= context.indents:
                 break
             # bin
             if context.name == "bin":
                 BaseToDict._finalize_bin(parent_context, context,
-                                         value_converter)
+                                         value_converter, strict)
             # dict
             #elif context.name == "dict":
             #    BaseToDict._finalize_dict(parent_context, context,
             #                              value_converter)
             # list
             #elif context.name == "list":
             #    BaseToDict._finalize_list(parent_context, context,
             #                              value_converter)
             # raw
             elif context.name == "raw":
                 BaseToDict._finalize_raw(parent_context, context,
-                                         value_converter)
+                                         value_converter, strict)
             # text
             elif context.name == "text":
                 BaseToDict._finalize_text(parent_context, context,
-                                          value_converter)
+                                          value_converter, strict)
             # delete the latest context
             del stack[-1]
 
     @staticmethod
     def _finalize_root_dict(root_context, value_converter):
         default_dict_type = value_converter.dict_type
         collection = root_context.collection
         if type(collection) is default_dict_type:
             return collection
         return default_dict_type(collection)
 
     @staticmethod
-    def _finalize_bin(parent_context, context, value_converter):
+    def _finalize_bin(parent_context, context, value_converter, strict):
         bin_block, whitespace_block = BaseToDict._split_block(context.collection)
         value = [item.strip() for item in bin_block if item]
         bin_data = value_converter.bin_decoder(value)
         #default_bin_type = value_converter.bin_type
         #if type(bin_data) is not default_bin_type:
         #    bin_data = default_bin_type(bin_data)
         BaseToDict._update_parent_context(parent_context, bin_data)
         for line in whitespace_block:
-            BaseToDict._add_whitespace_to_parent_context(parent_context, line)
+            BaseToDict._add_whitespace_to_parent_context(parent_context, line, strict)
     """
     @staticmethod
     def _finalize_dict(parent_context, context, value_converter):
         default_dict_type = value_converter.dict_type
         box = context.box
         if type(box) is default_dict_type:
             return
@@ -249,44 +248,44 @@
         if type(box) is default_raw_type:
             return
         box = default_raw_type(box)
         BaseToDict._update_parent_context(parent_context, box)
     """
 
     @staticmethod
-    def _finalize_raw(parent_context, context, value_converter):
+    def _finalize_raw(parent_context, context, value_converter, strict):
         # concatenate text lines
         raw_block, whitespace_block = BaseToDict._split_block(context.collection)
         text = value_converter.raw_decoder(raw_block)
 
         #default_raw_type = value_converter.raw_type
         #if type(text) is not default_raw_type:
         #    text = default_raw_type(text)
         BaseToDict._update_parent_context(parent_context, text)
         for line in whitespace_block:
-            BaseToDict._add_whitespace_to_parent_context(parent_context, line)
+            BaseToDict._add_whitespace_to_parent_context(parent_context, line, strict)
         return
         #default_raw_type = value_converter.raw_type
         #box = context.box
         #if type(box) is default_raw_type:
         #    return
         #box = default_raw_type(box)
         #BaseToDict._update_parent_context(parent_context, box)
 
     @staticmethod
-    def _finalize_text(parent_context, context, value_converter):
+    def _finalize_text(parent_context, context, value_converter, strict):
         # concatenate text lines
         text_block, whitespace_block = BaseToDict._split_block(context.collection)
         text = value_converter.text_decoder(text_block)
         #default_text_type = value_converter.text_type
         #if type(text) is not default_text_type:
         #    text = default_text_type(text)
         BaseToDict._update_parent_context(parent_context, text)
         for line in whitespace_block:
-            BaseToDict._add_whitespace_to_parent_context(parent_context, line)
+            BaseToDict._add_whitespace_to_parent_context(parent_context, line, strict)
 
     @staticmethod
     def _split_block(block):
         x, y = block, list()
         for i, line in enumerate(reversed(block)):
             if line.rstrip() == "---":
                 n = len(block)
@@ -305,15 +304,17 @@
             parent_context.collection[-1] = data
         else:
             msg = "Invalid parent name '{}'"
             msg = msg.format(parent_context.name)
             raise error.Error(msg)
 
     @staticmethod
-    def _add_whitespace_to_parent_context(parent_context, data):
+    def _add_whitespace_to_parent_context(parent_context, data, strict):
+        if strict:
+            return
         whitespace = Whitespace(data)
         if parent_context.name == "dict":
             whitespace_id = WhitespaceID()
             parent_context.collection[whitespace_id] = whitespace
         elif parent_context.name == "list":
             parent_context.collection[-1] = whitespace
         else:
@@ -531,27 +532,27 @@
 
         [parameters]
 
         - dict_type: the Python type in which a Jesth Dict should be converted into. Defaults to Python dict type.
 
         - list_type: the Python type in which a Jesth List should be converted into. Defaults to Python list type.
 
-        - XXX_types: this represents a group of parameters. Here, XXX is a placeholder for a Jesth data type. Valid types are: dict, list, bin, bool, complex, date, datetime, float, integer, raw, string, text, time. Examples: dict_types, float_types, and time_types. Use this parameter to set a list of Python types that may be encoded in the Jesth type (the same used as prefix). Example: dict_types defaults to [OrderedDict, dict], i.e., while encoding some Python data, an OrderedDict instance or a regular dict instance will be encoded as a Jesth dict.
+        - XXX_types: this represents a group of parameters. Here, XXX is a placeholder for a Jesth data type. Valid types are: dict, list, bin, bool, complex, date, datetime, float, integer, raw, string, text, time. Examples: dict_types, float_types, and time_types. Use this parameter to set a list of Python types that may be encoded in the Jesth type (the same used as prefix). Example: dict_types defaults to [dict, OrderedDict], i.e., while encoding some Python data, an OrderedDict instance or a regular dict instance will be encoded as a Jesth dict.
 
         - XXX_encoder: this represents a group of parameters. Here, XXX is a placeholder for one of: bin, bool, complex, date, datetime, float, integer, null, raw, string, text, time, fallback. Use these parameters to set a callable to encode Python values into Jesth values. Example: float_encoder = decimal.Decimal
 
         - XXX_decoder: this represents a group of parameters. Here, XXX is a placeholder for one of: bin, bool, complex, date, datetime, float, integer, null, raw, string, text, time, fallback. Use these parameters to set a callable to decode Jesth values into Python values. Example: integer_decoder = int
         """
 
         # default types for dict and list containers
-        self._dict_type = dict_type if dict_type else OrderedDict
+        self._dict_type = dict_type if dict_type else dict
         self._list_type = list_type if list_type else list
 
         # types for containers
-        self._dict_types = dict_types if dict_types else [OrderedDict, dict]
+        self._dict_types = dict_types if dict_types else [dict, OrderedDict]
         self._list_types = list_types if list_types else [list, tuple, set]
 
         # data types
         self._bin_types = bin_types if bin_types else [bytes]
         self._bool_types = bool_types if bool_types else [bool]
         self._complex_types = complex_types if complex_types else [complex]
         self._date_types = date_types if date_types else [datetime.date]
```

### Comparing `jesth-0.0.7/jesth/document/__init__.py` & `jesth-0.0.8/jesth/document/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Document class for creating model for Jesth data or to interacting with a Jesthfile"""
 import pathlib
-from collections import OrderedDict
 from jesth import misc
 from jesth.section import Section
 from jesth.renderer import write, render
 from jesth.converter import ValueConverter
 
 
 class Document:
@@ -98,45 +97,76 @@
         """
         Create a new section then append it to the end of this document
 
         [parameters]
         - header: the header (string) of the new section
         - body: the body of this section as a string or a list of strings
         """
-        self._insert(len(self._sections), header, body)
+        n = len(self._sections)
+        self._insert(n, header, body)
 
     def insert(self, index, header, body=None):
         """
         Create a new section then insert it in the document at a specific index
 
         [parameters]
         - index: integer index (absolute index). Accepts -1 to mimic the "append" method
         - header: the header (string) of the new section
         - body: the body of this section as a string or a list of strings
         """
-        index = len(self._sections) if index == -1 else index
+        n = len(self._sections)
+        index = misc.correct_index(index, n,
+                                   ignore_upper_bound=True) if n else 0
         self._insert(index, header, body)
 
-    def get(self, header, index=-1):
+    def set(self, index, header, body=None):
+        """
+        Set a section at a specific index of the document
+
+        [parameters]
+        - index: the index integer
+        - header: the header string of the section
+        - body: the body of the section, may be a list of string, a dictionary,
+          or a text string
+        """
+        n = len(self._sections)
+        index = misc.correct_index(index, n) if n else 0
+        # find section at same index then remove it
+        cache = self._find_section_to_remove(index)
+        if cache:
+            h, i = cache
+            self.remove(header=h, sub_index=i)
+        # insert new section
+        self._insert(index, header, body)
+
+    def get(self, header, sub_index=0):
         """
         Get X named section object located at Y index relatively to others sections with same header
 
         [parameters]
         - header: the header (string) of the section
         - index: integer index, relatively to the section
         family (sections sharing this same header).
-        Defaults to -1, thus will be returned, the last section with this header relatively
+        Defaults to 0, thus will be returned, the first section with this header relatively
         to this header family.
 
         [return]
         Returns a section or None
         """
-        if header not in self._model:
+        try:
+            n = len(self._model[header])
+        except KeyError:
             return None
-        return self._model[header][index]
+        sub_index = misc.correct_index(sub_index, n) if n else 0
+        section = None
+        try:
+            section = self._model[header][sub_index]
+        except IndexError:
+            pass
+        return section
 
     def get_all(self, header):
         """
         Get all sections sharing same header
 
         [parameters]
         - header: the header (string) of the sections
@@ -157,37 +187,45 @@
         [return]
         Returns the integer number of sections matching with the `header` parameter
         """
         if header not in self._model:
             return 0
         return len(self._model[header])
 
-    def remove(self, header, index=-1):
+    def remove(self, header, sub_index=-1):
         """
         Remove a section from this document
 
         [parameters]
         - header: the header of the section to remove
         - index: the index (integer) of the section relatively to
         its family (sections sharing same header).
         Defaults to -1, thus the last section of the given header family will be removed
         from the document
         """
-        if header not in self._model:
+        try:
+            n = len(self._model[header])
+        except KeyError:
             return
-        if self._model[header]:
-            del self._model[header][index]
-        else:
+        sub_index = misc.correct_index(sub_index, n)
+        if n == 0:
             del self._model[header]
-        index = len(self._sections) if index == -1 else index
-        i = len(self._sections) - 1
-        for _ in reversed(self._sections):
-            if i == index:
-                del self._sections[i]
-                break
+        else:
+            try:
+                del self._model[header][sub_index]
+            except IndexError:
+                pass
+        i1 = i2 = 0
+        for section in self._sections:
+            if section.header == header:
+                if i2 == sub_index:
+                    del self._sections[i1]
+                    break
+                i2 += 1
+            i1 += 1
 
     def remove_all(self, header):
         """
         Remove all sections with this specific header
 
         [parameters]
         - header: the header of the section to remove
@@ -201,28 +239,40 @@
                 del self._sections[i]
             i -= 1
 
     def _setup(self):
         self._create_model()
 
     def _create_model(self):
-        self._model = OrderedDict()
+        self._model = dict()
         for section in self._sections:
             header = section.header
             if header not in self._model:
                 self._model[header] = list()
             self._model[header].append(section)
 
     def _insert(self, index, header, body):
         section = Section(header, body=body,
                           value_converter=self._value_converter)
-        if index == 0 or index == len(self._sections):
-            self._sections.insert(index, section)
-            self._update_model(header, index, section)
-        else:
-            self._sections.insert(index, section)
-            self._create_model()
+        self._sections.insert(index, section)
+        self._update_model(header, index, section)
 
     def _update_model(self, header, index, section):
         if header not in self._model:
             self._model[header] = list()
         self._model[header].insert(index, section)
+
+    def _find_section_to_remove(self, index):
+        # find section at same index (the section to remove)
+        header = None
+        for i, section in enumerate(self._sections):
+            if i == index:
+                header = section.header
+        if header is None:
+            return
+        i1 = i2 = 0
+        for section in self._sections:
+            if i1 == index:
+                return header, i2
+            if section.header == header:
+                i2 += 1
+            i1 += 1
```

### Comparing `jesth-0.0.7/jesth/misc/__init__.py` & `jesth-0.0.8/jesth/misc/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,14 +38,46 @@
         msg = "Missing value in '{}'".format(line)
         raise error.Error(msg)
     if strip_whitespace:
         key, value = key.strip(), value.strip()
     return key, value
 
 
+def correct_index(index, size, ignore_upper_bound=False):
+    """
+    Correct an index given to access an item in a list
+
+    [parameter]
+    - index: the integer representing the index of a list.
+      This number may be positive or negative. A too big number is corrected down to
+      the end index of the list.
+      A negative number from -1 accesses the list from the end. A too small number
+      is corrected up to 0.
+      Example: give 5 the size of the list.
+      Index -1 will be corrected to 4 and index 6 will be corrected to 4.
+      Index -4 will be corrected to 0 same as index -10
+    - size: an integer representing the size of the list
+
+    [return]
+    Return a corrected index integer
+    """
+    index = int(index)
+    negative_size = -size
+    end_index = size - 1
+    if index >= size:
+        if ignore_upper_bound:
+            return index
+        return end_index
+    if index < negative_size:
+        index = negative_size
+    if index < 0:
+        index = size - abs(index)
+    return index
+
+
 def ensure_parent_dir(path):
     """Make sure that parent dir exists (create it if isn't yet created)"""
     parent = os.path.dirname(path)
     try:
         os.makedirs(parent)
     except FileExistsError as e:
         pass
```

### Comparing `jesth-0.0.7/jesth/parser/__init__.py` & `jesth-0.0.8/jesth/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `jesth-0.0.7/jesth/renderer/__init__.py` & `jesth-0.0.8/jesth/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `jesth-0.0.7/jesth/section/__init__.py` & `jesth-0.0.8/jesth/section/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Definition of the Section class"""
-from collections import OrderedDict
 from jesth import converter, error
 from jesth.converter import ValueConverter
 
 
 class Section:
     """A section is the main unit of a jesthFile. It's composed of a header and a body"""
     def __init__(self, header, body=None, *, value_converter=None):
@@ -33,54 +32,68 @@
         """The body in its base form, i.e., a list of strings !"""
         return self._body
 
     @property
     def value_converter(self):
         return self._value_converter
 
-    def get_dict(self, default=None, fallback=None, *, strict=True):
+    def to_dict(self, default=None, fallback=None, *, strict=True):
         """
-        Try to convert the body of this section into a dict.
-        Return fallback if failed to convert
+        Try to convert the body of this section to a dict.
+        Return a fallback value if failed to convert
 
         [parameters]
-        - default: Value to return if the body has been successfully converted into an empty dict.
-        Note that `default` will be updated to contain an empty OrderedDict if you leave it set to None.
+        - default: Value to return if the body has been successfully
+          converted into a dict but empty. Note that `default` will be
+          updated to contain an empty dict (from ValueConverter.dict_type)
+          if you leave it set to None.
         - fallback: Value to return if the attempt to convert the body into a dict failed
         - strict: set True if you don't want to preserve comments and whitespaces
 
         [return]
-        If everything is ok, a dict (OrderedDict) will be returned.
+        If everything is ok, a dict will be returned.
         Else the value of `default` or `fallback` will be returned.
         """
-        default = OrderedDict() if default is None else default
+        default = self._value_converter.dict_type() if default is None else default
         try:
-            return self.make_dict(default=default, strict=strict)
+            return self.create_dict(default=default, strict=strict)
         except Exception as e:
             return fallback
 
-    def make_dict(self, default=None, *, strict=True):
+    def to_text(self):
         """
-        Try to convert the body of this section into a dict (OrderedDict).
+        Return the body (list of lines) as a text string.
+
+        [return]
+        Return a string built with: `"\n".join(self._body)`
+        """
+        return "\n".join(self._body)
+
+    def create_dict(self, default=None, *, strict=True):
+        """
+        Try to build a dict object out of the body of this section.
         Raise an exception if an error occurs !
         Return `default` if the body has been created but is empty
 
         [parameters]
-        - default: Value to return if the body has been successfully converted into an empty dict. 
-        Note that `default` will be updated to contain an empty OrderedDict if you leave it set to None.
+        - default: Value to return if the body has been successfully
+          converted into an empty dict.
+          Note that `default` will be updated to contain
+          an empty dict (from ValueConverter.dict_type)
+          if you leave it set to None.
         - strict: set True if you don't want to preserve comments and whitespaces
 
         [return]
-        If everything is ok, a dict (OrderedDict) will be returned or the value of `default`
+        If everything is ok, a dict will be returned or the value of `default`
         Exceptions will be raised whenever a problem will arise !
         """
-        default = OrderedDict() if default is None else default
-        data = converter.make_dict(self._body,
-                                   value_converter=self._value_converter,
-                                   strict=strict)
+        default = self._value_converter.dict_type() if default is None else default
+        data = converter.create_dict(self._body,
+                                     value_converter=self._value_converter,
+                                     strict=strict)
         return data if data else default
 
     def update(self, body):
         """Update the entire body. The new body may be string, list of strings or a dict.
         Beware, if the body is a dict, instantiating this class may raise exceptions.
         For example, if the body contains circular references, an exception will be raised."""
         self._body = ensure_body(body,
@@ -91,14 +104,14 @@
     """Convert the body in the canonical base form: a list of string."""
     body = body if body else list()
     # string
     if isinstance(body, str):
         lines = body.split("\n")
         return lines
     # dict
-    if isinstance(body, dict):  # OrderedDict subclasses dict
+    if isinstance(body, dict):
         return converter.flatten_dict(body, value_converter=value_converter)
     # list
     if isinstance(body, list):
         body = [line.replace("\n", "\\n") for line in body]
         return body
     raise error.ConversionError
```

### Comparing `jesth-0.0.7/jesth.egg-info/PKG-INFO` & `jesth-0.0.8/jesth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jesth
-Version: 0.0.7
+Version: 0.0.8
 Summary: Next-level human-readable data serialization format
 Home-page: https://github.com/pyrustic/jesth
 Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com
 Maintainer: Pyrustic Evangelist
 Maintainer-email: rusticalex@yahoo.com
 License: MIT
@@ -15,17 +15,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- Cover -->
 <div align="center">
-    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/jesth/cover.png" alt="Demo" width="1380">
+    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/jesth/cover.png" alt="Demo" width="650">
     <p align="center">
-    Jesthfile with 1 top anonymous section, and 2 'user' sections
+    JesthFile with 1 anonymous top section, and 2 'user' sections
     </p>
 </div>
 
 
 <!-- Intro Text -->
 # Jesth
 <b> Next-level human-readable data serialization format </b>
@@ -33,60 +33,62 @@
 This project is part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
 > [Installation](#installation) &nbsp; &nbsp; [Demo](#demo) &nbsp; &nbsp; [Latest](https://github.com/pyrustic/jesth/tags) &nbsp; &nbsp; [Modules](https://github.com/pyrustic/jesth/tree/master/docs/modules#readme)
 
 
 ## Table of contents
 
 - [Overview](#overview)
-- [Why not TOML, YAML, or JSON ?](#why_not_toml_yaml_or_json )
-- [Why use Jesth ?](#why_use_jesth_)
+- [Why not TOML, YAML, or JSON ?](#why-not-toml-yaml-or-json-)
+- [Why use Jesth ?](#why-use-jesth-)
 - [Demo](#demo)
-- [Code snippets for everyday scenarios](#code_snippets_for_everyday_scenarios)
-- [Anatomy of a Section](#anatomy_of_a_Section)
-    - [Base section](#base_section)
-    - [Dict section](#dict_section)
-    - [Section family](#section_family)
-- [Specs of the Dict Section](#specs_of_the_dict_section)
+- [Code snippets for everyday scenarios](#code-snippets-for-everyday-scenarios)
+- [Anatomy of a Section](#anatomy-of-a-section)
+    - [Base section](#base-section)
+    - [Dict section](#dict-section)
+    - [Section family](#section-family)
+- [Specs of the Dict Section](#specs-of-the-dict-section)
     - [Scalars](#scalars)
-    - [Null value](#null_value)
-    - [Single-line strings](#single-line_strings)
-    - [Multi-line strings](#multi-line_strings)
-    - [Date and time](#date_and_time)
-    - [Embedded binary data](#embedded_binary_data)
-    - [Comments and whitespace](#comments_and_whitespace)
-    - [Collections (nested dict and list)](#collections_nested_dict_and_list)
-- [Application programming interface](#application_programming_interface)
-- [Jesth Schema for data validation](#jesth_schema_for_data_validation)
-- [Available implementations](#available_implementations)
+    - [Null value](#null-value)
+    - [Single-line strings](#single-line-strings)
+    - [Multi-line strings](#multi-line-strings)
+    - [Date and time](#date-and-time)
+    - [Embedded binary data](#embedded-binary-data)
+    - [Comments and whitespaces](#comments-and-whitespaces)
+    - [Collections (nested dict and list)](#collections-nested-dict-and-list)
+- [Application programming interface](#application-programming-interface)
+- [Jesth Schema for data validation](#jesth-schema-for-data-validation)
+- [Available implementations](#available-implementations)
 - [Miscellaneous](#miscellaneous)
 - [Contributing](#contributing)
 - [Installation](#installation)
     
 
 # Overview
-**Jesth**, which stands for **Just Extract Sections Then Hack**, is a human-readable data serialization format whose reference parser is an eponymous lightweight Python library available on [PyPI](#installation).
+**Jesth** (pronounced [/dʒest/](https://dictionary.cambridge.org/pronunciation/english/jest)), which stands for **Just Extract Sections Then Hack'em**, is a human-readable data serialization format whose reference parser is an eponymous lightweight [Python](https://www.python.org/) library available on [PyPI](#installation).
+
+> Read the **backstory** in this [HN discussion](https://news.ycombinator.com/item?id=35991018) !
 
 ## Versatile serialization format
 A Jesth **document** is made up of **sections**, each defined by a **header** (between two square brackets) and a **body** which is just lines of text. 
 
 Instead of interpreting these lines upstream after extracting the sections, the Jesth parser lays low and lets the programmer decide which hack to apply to them.
 
 Because of this parsing policy, a single Jesth document can contain an **eclectic set of sections** representing a poem, server configs, help text, [prompts](https://github.com/f/awesome-chatgpt-prompts) for a chatbot, [directed graph](https://en.wikipedia.org/wiki/Directed_graph), [ascii artwork](https://en.wikipedia.org/wiki/ASCII_art), and more.
 
 ## Shipped with a proper and extensively tested hack
-For convenience, the Jesth library includes a proper and extensively tested hack to convert a compatible section into a [dictionary](https://en.wikipedia.org/wiki/Associative_array) data structure. In such a section that allows comments, one can encode strings (single or multi-line), scalars (integer, float, decimal float, complex, booleans), date and time, null value, binary data and nested collections (list and dictionary).
+For convenience, the Jesth library includes a proper and extensively tested [hack]((https://en.wikipedia.org/wiki/Hacker_culture)) to convert a compatible section to a [dictionary](https://en.wikipedia.org/wiki/Associative_array) data structure. In such a section that allows comments, one can encode **strings** (single or multi-line), **scalars** (integer, float, decimal float, complex, booleans), **date** and **time**, **null** value, **binary** data and nested **collections** (list and dictionary).
 
 Therefore, Jesth can be used for configuration files, to create a [scripting language](https://github.com/pyrustic/backstage), to act as a markup language to write [docstrings](https://en.wikipedia.org/wiki/Docstring#Python) so that a tool can generate reference documentation after parsing them, etc.
 
 In the next few sections, we'll dive deep into Jesth, but first, why not [TOML](https://en.wikipedia.org/wiki/TOML), [YAML](https://fr.wikipedia.org/wiki/YAML), or [JSON](https://en.wikipedia.org/wiki/JSON) ?
 
 # Why not TOML, YAML, or JSON ?
 Jesth offers a high level of **versatility** that allows the programmer to freely decide what a section can contain and how to interpret its contents. 
 
-Moreover, whenever the programmer decides to adopt a dictionary as a data structure to formalize some or all sections of a Jesth document, he/she is offered a [very readable and strict syntax](#specs_of_the_dict_section) to encode the data. 
+Moreover, whenever the programmer decides to adopt a dictionary as a data structure to formalize some or all sections of a Jesth document, he/she is offered a [very readable and strict syntax](#specs-of-the-dict-section) to encode the data. 
 
 The library exposes an intuitive API for loading and dumping Dict sections with an option to preserve comments and whitespaces.
 
 The following subsections will briefly compare **TOML**, **YAML**, and **JSON** to **Jesth's dictionary data structure support**.
 
 ## Why not TOML ?
 Jesth shares with **TOML** the use of square brackets to define sections (or tables in TOML terminology), therefore, among other formats, the TOML syntax is closest to Jesth. However, when dealing with nested structures, TOML becomes very confusing, revealing the limitations of its syntax.
@@ -100,23 +102,23 @@
 **JSON** is great because it mimics the way we define data structures in source code. Therefore, it can be minified and is also a reasonable choice for machine-to-machine communication, but it cannot beat the readability of formats that natively support line breaks and/or indentation. In comparison to Jesth, JSON has fewer native data types and no native support for comments.
 
 # Why use Jesth ?
 Jesth is ideal for configuration files, whether intended for use by a standard application or by a chatbot/AI. Personal notes can also benefit from being entered into a Jesth file, so they can be parsed later. As mentioned in the [Overview](#overview) section, Jesth was used to design a [scripting language](https://github.com/pyrustic/backstage) and currently serves as the markup language for [docstrings](https://en.wikipedia.org/wiki/Docstring#Python) in all projects that are part of the [Pyrustic ecosystem](https://pyrustic.github.io).
 
 Loading a Jesth document is stress-free because exceptions are only thrown when you try to convert a non-compatible section to a dictionary. But even that is the strict default behavior of the dictionary converter since you can customize the converter to string invalid values. This specific customization is as simple as this: `value_converter.fallback_decoder = str`
 
-There's more to say, for example the syntax for encoding a dictionary into a JesthFile is text editor/IDE-friendly, so it may benefit from supporting some cool features like the folding mechanism.
+There's more to say, for example the Jesth Dict Section syntax is text editor/IDE-friendly, so it may benefit from supporting some cool features like the folding mechanism.
 
 # Demo
-The demo is a clonable repository containing a Jesthfile and a Python script to load its contents. 
+The demo is a clonable repository containing a JesthFile and a Python script to load its contents. 
 
 > [Open the Demo](https://github.com/pyrustic/jesth-demo#readme) !
 
 # Code snippets for everyday scenarios
-**Load a Jesthfile:**
+**Load a JesthFile:**
 ```python
 from jesth import read
 
 path = "/home/alex/jesthfile"
 document = read(path)
 ```
 
@@ -129,36 +131,40 @@
 
 # get the list of all "user" sections
 user_sections = document.get_all("user")
 
 # show the body of a section
 print(config_section.body)  # list of lines
 
+# show the body as a text (concatenated lines)
+print(config_section.to_text())
+
 # update the body of a section
 new_body = [r"# comment", 
             r"server1 = '1.1.1.1'",
             r"port = 80"]
 config_section.update(new_body)
 ```
 
 **Convert a compatible section into a Python Dict:**
+
 ```python
 ...
 
-# will raise an exception if the section can't be converted into dict
-dict_object = section.make_dict()
+# won't raise an exception if the section can't be converted to dict
+dict_object = section.to_dict()
 
-# won't raise an exception if the section can't be converted into dict
-dict_object = section.get_dict()
+# will raise an exception if the section can't be converted to dict
+dict_object = section.create_dict()
 
-# Note that `.make_dict` accepts `default` and `strict` arguments
+# Note that `.create_dict` accepts `default` and `strict` arguments
 # If the body can be converted to a dict but is empty, you get `default`
 # Set True to `strict` to preserve comments and whitespaces
 
-# Note that `.get_dict` accepts `default`, `strict`, and `fallback`
+# Note that `.to_dict` accepts `default`, `strict`, and `fallback`
 # If the body can't be converted to a dict, you get `fallback`
 ```
 
 **Edit a document:**
 ```python
 ...
 
@@ -174,15 +180,15 @@
 ```
 
 **Save a document:**
 ```python
 from jesth import write
 ...
 
-# if the document is linked to a Jesthfile, call its `save` method
+# if the document is linked to a JesthFile, call its `save` method
 document.save()
 
 # or save to a new path
 document.save_to(path)
 
 # Under the hood, the Document class actually uses the `write` function
 write(document, path)
@@ -190,15 +196,15 @@
 
 **Render a document:**
 ```python
 from jesth import render
 ...
 
 # return the string representation of the data
-# this jesth text can be stored as it in a Jesthfile
+# this jesth text can be stored as it in a JesthFile
 jesth_text = document.render()
 
 # Under the hood, the Document class actually uses the `render` function
 jesth_text = render(document)
 ```
 
 # Anatomy of a Section
@@ -241,38 +247,38 @@
 Is called Base section a section as defined in the document, without any transformation, i.e., just text lines. From the source code perspective, the body of such section is represented by default as a list of lines (string). 
 
 The alternative representation of such body is just a concatenated version of this list.
 
 ## Dict section
 Is called Dict section, a section that is intended to be converted into a dictionary object by the parser. 
 
-By default, the library uses the `OrderedDict` class to represent the body of such section, thus, the order of key/value is preserved. This default behavior can be customized through the `ValueConverter` object.
+By default, the library uses the regular `dict` type to represent the body of such section. This default behavior can be customized through the `ValueConverter` object.
 
 ## Section family
-Different sections can have the same header. In this case, they belong to a section family. By default, the `.get(header)` method from the `Document` class returns the last defined section with the given header argument. This method actually accepts an `index` argument which is set to `-1` by default to align with Python convention to access the last item of a sequence.
+Different sections can have the same header. In this case, they belong to a **section family**. By default, the `.get(header)` method from the `Document` class returns the first defined section with the given header argument. This method actually accepts a `sub_index` argument which is set to `0` by default to access the first item of the section family.
 
 **Get the 2nd section in the 'user' section family:**
 
 ```python
 ...
 
-section = document.get("user", index=1)
+section = document.get("user", sub_index=1)
 ```
 
 **Get the list of all sections in the 'user' section family:**
 ```python
 ...
 
 sections = document.get_all("user")
 ```
 
 # Specs of the Dict Section
 The specs for a Dictionary Section are mostly aligned with Python specs. For example, a Jesth Integer follows exactly the definition of Python Integer. 
 
-> **Note:** The Jesth library allows the customization of each type of data as well in the context of parsing or in the context of rendering. This customization is made via the [ValueConverter](#the_valueconverter_object) object
+> **Note:** The Jesth library allows the customization of each type of data as well in the context of parsing or in the context of rendering. This customization is made via the [ValueConverter](#the-valueconverter-object) object
 
 ## Scalars
 Jesth supports integers (base 10, hexadecimal, octal, binary), float (approximate binary floating-point, fixed-precision decimal floating-point), complex numbers, and booleans.
 
 > **Note:** Jesth Scalars specs are aligned with their respective Python equivalent specs.
 
 ### Integer
@@ -455,15 +461,15 @@
 
 |Jesth|Python|
 |---|---|
 |bin (base64)|`bytes`|
 
 
 ## Comments and whitespaces
-Jesth Dict Section supports comments which are strings starting with `#`. Comments and Whitespaces can be preserved while converting a Jesth Dict Section into a Python Dictionary (OrderedDict to be precise).
+Jesth Dict Section supports comments which are strings starting with `#`. Comments and Whitespaces can be preserved while converting a Jesth Dict Section into a Python Dictionary.
 **Example with comments and whitespaces:**
 ```
 # this is a comment
 key = "value"
 
 # another comment
 number = 42
@@ -496,18 +502,18 @@
         (dict)
             project = "jesth"
             number = 42
 ```
 
 **Mapping with actual Python objects:**
 
-|Jesth|Python|
-|---|---|
-|dict|`collections.OrderedDict`|
-|list|`list`|
+|Jesth| Python |
+|---|--------|
+|dict| `dict` |
+|list| `list` |
 
 # Application programming interface
 The library exposes functions and classes to load and dump Jesth document with optional customization at each stage. Loaded documents and their sections are encapsulated into classes exposing methods and properties with a high emphasis on ergonomy.
 
 ## Loading Jesth
 To load Jesth data, one may use the `jesth.parser.read` function when the source is a file (file-like object, path string, or pathlib.Path object), or `jesth.parser.parse` function when the source is a string.
 
@@ -576,52 +582,56 @@
 > **Properties:** `path`, `sections`, `value_converter`, and `headers`. 
 
 
 ### Edit a document
 The document object exposes `append`, `insert`, `remove`, and `remove_all` methods to add and remove sections.
 
 **Example:**
+
 ```python
 from jesth import read
 
 path = "/path/to/jestfile"
 document = read(path)
 
 # append a new section to the document
 body = ["line 1", "line 2", "line 3"]
 document.append("header", body=body)  # body may be a dict or string
 
 # insert an empty section at a specific index
 document.insert(0, "header")  # therefore, first section
+# override the first section with a new empty one
+document.set(0, "header")  # 'body' is still set to None here
 
 # remove the last section with a specific header
-document.remove("header")  # index defaults to -1
+document.remove("header")  # sub_index defaults to -1
 # remove the first section with a specific header
-document.remove("header", index=0)
+document.remove("header", sub_index=0)
 # note that the index argument is meant to be relative
 # to this 'section family', i.e., sections with same header.
 
 # remove all sections by header
 document.remove_all("header")
 ```
 
 ### Query a document
 The document object exposes `get`, `get_all`, and `count` methods to retrieve sections or their count.
 
 **Example:**
+
 ```python
 from jesth import read
 
 path = "/path/to/jestfile"
 document = read(path)
 
-# get the last section with a specific header
-section = document.get("header")  # the index arg defaults to -1
 # get the first section with a specific header
-section = document.get("header", index=0) 
+section = document.get("header")  # the index arg defaults to 0
+# get the last section with a specific header
+section = document.get("header", sub_index=-1)
 # note that the index argument is meant to be relative
 # to this 'section family', i.e., sections with same header.
 
 # get all sections with a specific header
 sections = document.get_all("header")
 
 # count the number of sections sharing a specific header
@@ -631,33 +641,37 @@
 ## The Section object
 The Section object contains the header and the body of a section. The body is stored as a list of string that may be converted on demand, if compatible, into a Python dictionary.
 
 > **Properties:** `header`, `body`, and `value_converter`.
 
 
 **Example:**
+
 ```python
 from jesth import read
 
 path = "/path/to/jestfile"
 document = read(path)
 section = document.get("header")
 
 # Convert the body of this section into a dict then return it.
+# Beware, this method won't raise an exception at all
+# instead, it may return a fallback value
+data = section.to_dict()  # accepts "default", "fallback", "strict"
+
+# Concatenate the lines of the body to form a text string
+data = section.to_text()
+
+# Convert the body of this section into a dict then return it.
 # Beware, this method will raise an exception if the conversion fails
-data = section.make_dict()  # accepts "default" and "strict"
+data = section.create_dict()  # accepts "default" and "strict"
 # the default parameter is for default data if the new created dict
 # is empty. The strict parameter is to tell whether comment/whitespace
 # should be preserved and inserted in the new dict !
 
-# Convert the body of this section into a dict then return it.
-# Beware, this method won't raise an exception at all
-# instead, it may return a fallback value
-data = section.get_dict()  # accepts "default", "fallback", "strict"
-
 # update the body of this section
 body = ["line 1", "line 2", "line 3"]
 section.update(body)  # here, body may be a string or a dict
 ```
 
 ## The ValueConverter object
 This object has methods to encode and decode values, and also properties to customize conversion types. 
@@ -665,15 +679,15 @@
 Most time, you won't need to set or edit this object. The encode and decode methods of this object are only useful for test purpose.
 
 **Parameters:**
 - **dict_type**: the Python type in which a Jesth Dict should be converted into. Defaults to Python dict type.
 
 - **list_type**: the Python type in which a Jesth List should be converted into. Defaults to Python list type.
 
-- **XXX_types**: this represents a group of parameters. Here, XXX is a placeholder for a Jesth data type. Valid types are: dict, list, bin, bool, complex, date, datetime, float, integer, raw, string, text, time. Examples: dict_types, float_types, and time_types. Use this parameter to set a list of Python types that may be encoded in the Jesth type (the same used as prefix). Example: dict_types defaults to [OrderedDict, dict], i.e., while encoding some Python data, an OrderedDict instance or a regular dict instance will be encoded as a Jesth dict.
+- **XXX_types**: this represents a group of parameters. Here, XXX is a placeholder for a Jesth data type. Valid types are: dict, list, bin, bool, complex, date, datetime, float, integer, raw, string, text, time. Examples: dict_types, float_types, and time_types. Use this parameter to set a list of Python types that may be encoded in the Jesth type (the same used as prefix). Example: dict_types defaults to [dict, OrderedDict], i.e., while encoding some Python data, an OrderedDict instance or a regular dict instance will be encoded as a Jesth dict.
 
 - **XXX_encoder**: this represents a group of parameters. Here, XXX is a placeholder for one of: bin, bool, complex, date, datetime, float, integer, null, raw, string, text, time, fallback. Use these parameters to set a callable to encode Python values into Jesth values. Example: float_encoder = decimal.Decimal
 
 - **XXX_decoder**: this represents a group of parameters. Here, XXX is a placeholder for one of: bin, bool, complex, date, datetime, float, integer, null, raw, string, text, time, fallback. Use these parameters to set a callable to decode Jesth values into Python values. Example: integer_decoder = int
 
 > **Note:** the parameters of ValueConverter are mirrored as read and write properties.
 
@@ -685,15 +699,15 @@
 For the moment, the only available implementation of Jesth is this reference library written in Python. 
 If you are interested into writing a Jesth library for another language (Rust, C#, Java, JavaScript, PHP, etc), feel free to get in touch with [me](https://pyrustic.github.io/#contact) for any question !
 
 # Miscellaneous
 Collection of miscellaneous notes.
 
 ## Acronymy
-Jesth stands for Just Extract Sections Then Hack.
+Jesth stands for **Just Extract Sections Then Hack'em**. Here, the word `hack` is a direct reference to the [Hacker culture](https://en.wikipedia.org/wiki/Hacker_culture).
 
 ## End of document
 To tell the parser to stop parsing a document, input in the document the `[[END]]` (case-insensitive) tag on its own line.
 
 ## Opening square bracket at the beginning of a line
 You must escape the opening square brackets at the start of a line of a body with a backslash `\` character. And whenever your line needs to start with `n` backslash(es) followed by an opening square bracket, you need to prepend an extra backslash to the line, resulting in `n+1` backslash(es).
 
@@ -712,14 +726,15 @@
 
 ## Beautiful cover image
 The beautiful cover image is made with the amazing [carbon app](https://carbon.now.sh).
 
 # Contributing
 Feel free to open an issue to report a bug, suggest some changes, show some useful code snippets, or discuss anything related to this project. You can also directly email [me](https://pyrustic.github.io/#contact).
 
+> **Note:** I would like to automate a decent Git workflow (branching, merging patches, all the basic cool things cool kids do) with [Backstage](https://github.com/pyrustic/backstage). In the meantime, I will manually incorporate the fixes into the only existing branch (`master`). Thank you for your understanding !
 
 ## Setup your development environment
 Following are instructions to setup your development environment
 
 ```bash
 # create and activate a virtual environment
 python -m venv venv
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jesth-0.0.7/jesth.egg-info/SOURCES.txt` & `jesth-0.0.8/jesth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jesth-0.0.7/setup.cfg` & `jesth-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `jesth-0.0.7/tests/test_box.py` & `jesth-0.0.8/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `jesth-0.0.7/tests/test_converter.py` & `jesth-0.0.8/tests/test_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import decimal
 import unittest
 import datetime
 from decimal import Decimal
 from jesth import box, error
-from jesth.converter import ValueConverter, make_dict, flatten_dict
+from jesth.converter import ValueConverter, create_dict, flatten_dict
 
 
 BODY = r"""
 # strings
 string = "Hello "World" ! \\ \n \\n \\u000A ˫"
 raw_string = 'Hello 'World' ! \n \\n \u000A ˫'
 empty_string = ""
@@ -86,15 +86,15 @@
 """
 
 
 class TestConversionFuncs(unittest.TestCase):
 
     def test(self):
         # Make a dict from BODY
-        dict_body = make_dict(BODY, strict=False)
+        dict_body = create_dict(BODY, strict=False)
         # Flatten the dict
         flat_body = flatten_dict(dict_body)
         # Make text from flatten body then compare with BODY
         text = "\n".join(flat_body)
         self.assertEqual(BODY, text)
```

### Comparing `jesth-0.0.7/tests/test_document.py` & `jesth-0.0.8/tests/test_document.py`

 * *Files 20% similar despite different names*

```diff
@@ -147,27 +147,43 @@
         r = document.render("", "info", "user")
         expected = RAW_DOCUMENT
         self.assertEqual(expected, r)
 
 
 class TestDocumentDataInsertionMethods(unittest.TestCase):
 
+    def test_set_section_at_begin(self):
+        text = "[section1]\n\n[section2]"
+        # insert at begin
+        document = parse(text)
+        document.set(0, "new_section")
+        expected = "[new_section]\n\n[section2]"
+        self.assertEqual(expected, document.render())
+
+    def test_set_section_at_end(self):
+        text = "[section1]\n\n[section2]"
+        # insert at the end
+        document = parse(text)
+        document.set(-1, "new_section")
+        expected = "[section1]\n\n[new_section]"
+        self.assertEqual(expected, document.render())
+
     def test_insert_at_begin(self):
         text = "[section1]\n\n[section2]"
         # insert at 0
         document = parse(text)
         document.insert(0, "new_section")
         expected = "[new_section]\n\n" + text
         self.assertEqual(expected, document.render())
 
     def test_insert_at_end(self):
         text = "[section1]\n\n[section2]"
         # insert at the end
         document = parse(text)
-        document.insert(-1, "new_section")
+        document.insert(2, "new_section")
         expected = text + "\n\n[new_section]"
         self.assertEqual(expected, document.render())
 
     def test_insert_at_middle(self):
         text = "[section1]\n\n[section2]"
         # insert at the middle
         document = parse(text)
@@ -184,19 +200,23 @@
 
 class TestDocumentDataRetrivalMethods(unittest.TestCase):
 
     def test_get_method(self):
         # default
         document = parse(USER_ONLY)
         user = document.get("user")
+        expected_body = ["id = 1", "name = 'alex'"]
+        self.assertEqual(expected_body, user.body)
+        # specific index
+        user = document.get("user", 1)
         expected_body = ["id = 2", "name = 'rustic'"]
         self.assertEqual(expected_body, user.body)
         # specific index
-        user = document.get("user", 0)
-        expected_body = ["id = 1", "name = 'alex'"]
+        user = document.get("user", -1)
+        expected_body = ["id = 2", "name = 'rustic'"]
         self.assertEqual(expected_body, user.body)
 
     def test_get_all_method(self):
         document = parse(USER_ONLY)
         users = document.get_all("user")
         expected_bodies = (["id = 1", "name = 'alex'"],
                            ["id = 2", "name = 'rustic'"])
@@ -214,28 +234,52 @@
         document = parse(USER_ONLY)
         self.assertEqual(2, document.count("user"))
         document.remove("user")
         user = document.get("user")
         expected_body = ["id = 1", "name = 'alex'"]
         self.assertEqual(expected_body, user.body)
         self.assertEqual(1, document.count("user"))
+        self.assertEqual(1, count_sections(document, "user"))
 
     def test_remove_section_at_relative_index(self):
+        # remove first item
         document = parse(USER_ONLY)
         self.assertEqual(2, document.count("user"))
         document.remove("user", 0)
         user = document.get("user")
         expected_body = ["id = 2", "name = 'rustic'"]
         self.assertEqual(expected_body, user.body)
         self.assertEqual(1, document.count("user"))
+        self.assertEqual(1, count_sections(document, "user"))
+        # remove second item
+        document = parse(USER_ONLY)
+        document.remove("user", 1)
+        user = document.get("user")
+        expected_body = ["id = 1", "name = 'alex'"]
+        self.assertEqual(expected_body, user.body)
+        self.assertEqual(1, document.count("user"))
+        self.assertEqual(1, count_sections(document, "user"))
 
     def test_remove_all_method(self):
         document = parse(USER_AND_INFO)
         self.assertEqual(2, document.count("user"))
+        self.assertEqual(2, count_sections(document, "user"))
         self.assertEqual(1, document.count("info"))
+        self.assertEqual(1, count_sections(document, "info"))
         document.remove_all("user")
         self.assertEqual(0, document.count("user"))
+        self.assertEqual(0, count_sections(document, "user"))
         self.assertEqual(1, document.count("info"))
+        self.assertEqual(1, count_sections(document, "info"))
+
+
+def count_sections(document, header):
+    """Count sections in a document with a specific header"""
+    i = 0
+    for s in document.sections:
+        if s.header == header:
+            i += 1
+    return i
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `jesth-0.0.7/tests/test_misc.py` & `jesth-0.0.8/tests/test_misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,46 @@
     def test_with_colon_as_separator(self):
         line = " key : 'value here' "
         r = misc.split_key_value(line, sep=":")
         expected = ("key", "'value here'")
         self.assertEqual(expected, r)
 
 
+class TestCorrectIndexFunc(unittest.TestCase):
+
+    def test_with_positive_index(self):
+        # correct index
+        size = 5
+        for i in range(size):
+            r = misc.correct_index(index=i, size=size)
+            expected = i
+            self.assertEqual(expected, r)
+        # out of bound index
+        r = misc.correct_index(index=7, size=6)
+        expected = 5
+        self.assertEqual(expected, r)
+        # out of bound index + ignore upper bound
+        r = misc.correct_index(index=7, size=6, ignore_upper_bound=True)
+        expected = 7
+        self.assertEqual(expected, r)
+
+    def test_with_negative_index(self):
+        # correct index
+        size = 5
+        expected = 0
+        for i in range(-size, 0):
+            r = misc.correct_index(index=i, size=size)
+            self.assertEqual(expected, r)
+            expected += 1
+        # out of bound index
+        r = misc.correct_index(index=-7, size=6)
+        expected = 0
+        self.assertEqual(expected, r)
+
+
 class TestUpdateCachedRefsFunc(unittest.TestCase):
 
     def test(self):
         cached_refs = list()
         misc.update_cached_refs(1, cached_refs)
         self.assertEqual(1, len(cached_refs))
         with self.assertRaises(error.Error):
@@ -254,9 +286,10 @@
         expected_right_mantissa = "14653898075720390738"
         expected_exponent = "-5"
         self.assertEqual(expected_left_mantissa, info.left_mantissa)
         self.assertEqual(expected_right_mantissa, info.right_mantissa)
         self.assertEqual(expected_exponent, info.exponent)
 
 
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `jesth-0.0.7/tests/test_parser.py` & `jesth-0.0.8/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `jesth-0.0.7/tests/test_renderer.py` & `jesth-0.0.8/tests/test_renderer.py`

 * *Files identical despite different names*

### Comparing `jesth-0.0.7/tests/test_root_imports.py` & `jesth-0.0.8/tests/test_root_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def test(self):
         jesth.Document
         jesth.Section
         jesth.parse
         jesth.render
         jesth.read
         jesth.write
-        jesth.make_dict
+        jesth.create_dict
         jesth.flatten_dict
         jesth.ValueConverter
         jesth.split_key_value
         jesth.Parser
         self.assertTrue(True)
```

### Comparing `jesth-0.0.7/tests/test_section.py` & `jesth-0.0.8/tests/test_section.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,63 +59,77 @@
     def test_update_body(self):
         section = Section("header")
         invalid_base_body = 3.14
         with self.assertRaises(error.ConversionError):
             # body should be a list of string, a dict, or a string
             section.update(invalid_base_body)
 
-    def test_make_dict_body(self):
+    def test_create_dict(self):
         # test with empty body
         section = Section("")
-        r = section.make_dict()
+        r = section.create_dict()
         self.assertEqual(OrderedDict(), r)
         # empty body + default parameter set
         default = {"is_empty": True}
-        r = section.make_dict(default)
+        r = section.create_dict(default)
         self.assertIs(default, r)
         # == test with existent and compatible body
         section.update(BASE_BODY)
         # compact_mode = true
-        r = section.make_dict(strict=True)
+        r = section.create_dict(strict=True)
         self.assertIsNotNone(r)
         self.assertFalse(_find_comment(r))
         # compact_mode = false
-        r = section.make_dict(strict=False)
+        r = section.create_dict(strict=False)
         self.assertIsNotNone(r)
         self.assertTrue(_find_comment(r))
 
-    def test_make_dict_body_with_incompatible_body(self):
+    def test_create_dict_with_incompatible_body(self):
         section = Section("", ["hello world"])
         with self.assertRaises(Exception):
-            section.make_dict()
+            section.create_dict()
 
-    def test_get_dict_body(self):
+    def test_to_text(self):
+        # non-empty body
+        section = Section("", ["hello", "world"])
+        r = section.to_text()
+        expected = "hello\nworld"
+        self.assertEqual(expected, r)
+
+    def test_to_text_with_empty_body(self):
+        # empty body
+        section = Section("")
+        r = section.to_text()
+        expected = ""
+        self.assertEqual(expected, r)
+
+    def test_to_dict(self):
         # test with empty body
         section = Section("")
-        r = section.get_dict()
+        r = section.to_dict()
         self.assertEqual(OrderedDict(), r)
         # empty body + default parameter set
         default = {"is_empty": True}
-        r = section.get_dict(default)
+        r = section.to_dict(default)
         self.assertIs(default, r)
         # == test with existent and compatible body
         section.update(BASE_BODY)
         # compact_mode = true
-        r = section.get_dict(strict=True)
+        r = section.to_dict(strict=True)
         self.assertIsNotNone(r)
         self.assertFalse(_find_comment(r))
         # compact_mode = false
-        r = section.get_dict(strict=False)
+        r = section.to_dict(strict=False)
         self.assertIsNotNone(r)
         self.assertTrue(_find_comment(r))
 
-    def test_get_dict_body_with_incompatible_body(self):
+    def test_to_dict_with_incompatible_body(self):
         section = Section("", ["hello world"])
         fallback = {"something_wrong": True}
-        r = section.get_dict(fallback=fallback)
+        r = section.to_dict(fallback=fallback)
         self.assertEqual(fallback, r)
 
 
 def _find_comment(body, comment="# welcome"):
     for key, val in body.items():
         if val == comment:
             return True
```

