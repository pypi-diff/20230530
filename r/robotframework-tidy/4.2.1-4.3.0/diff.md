# Comparing `tmp/robotframework-tidy-4.2.1.tar.gz` & `tmp/robotframework-tidy-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-tidy-4.2.1.tar", last modified: Wed Apr 26 08:27:57 2023, max compression
+gzip compressed data, was "robotframework-tidy-4.3.0.tar", last modified: Tue May 30 10:41:57 2023, max compression
```

## Comparing `robotframework-tidy-4.2.1.tar` & `robotframework-tidy-4.3.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:27:57.109992 robotframework-tidy-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-26 08:27:57.109992 robotframework-tidy-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:27:57.101992 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-26 08:27:57.000000 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-26 08:27:57.000000 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:27:57.000000 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 08:27:57.000000 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-26 08:27:57.000000 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 08:27:57.000000 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:27:57.105992 robotframework-tidy-4.2.1/robotidy/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:27:57.105992 robotframework-tidy-4.2.1/robotidy/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-26 08:27:56.000000 robotframework-tidy-4.2.1/robotidy/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-26 08:27:56.000000 robotframework-tidy-4.2.1/robotidy/__pycache__/version.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/disablers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/rich_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/skip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:27:57.109992 robotframework-tidy-4.2.1/robotidy/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/AddMissingEnd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/AlignKeywordsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/AlignSettingsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/AlignTemplatedTestCases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/AlignTestCasesSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/AlignVariablesSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/DiscardEmptySections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/GenerateDocumentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/IndentNestedKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/InlineIf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/MergeAndOrderSections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeAssignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeComments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeNewLines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeSectionHeaderName.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeSeparators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeSettingName.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeTags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/OrderSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/OrderSettingsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/OrderTags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/RemoveEmptySettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/RenameKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/RenameTestCases.py
--rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/RenameVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/ReplaceBreakContinue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/ReplaceEmptyValues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/ReplaceReturns.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/ReplaceRunKeywordIf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/SmartSortKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/SplitTooLongLine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/Translate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19687 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23065 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/aligners_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:27:57.109992 robotframework-tidy-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:41:57.145647 robotframework-tidy-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-30 10:41:57.145647 robotframework-tidy-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:41:57.133647 robotframework-tidy-4.3.0/robotframework_tidy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-30 10:41:57.000000 robotframework-tidy-4.3.0/robotframework_tidy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-30 10:41:57.000000 robotframework-tidy-4.3.0/robotframework_tidy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:41:57.000000 robotframework-tidy-4.3.0/robotframework_tidy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 10:41:57.000000 robotframework-tidy-4.3.0/robotframework_tidy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-30 10:41:57.000000 robotframework-tidy-4.3.0/robotframework_tidy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 10:41:57.000000 robotframework-tidy-4.3.0/robotframework_tidy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:41:57.137647 robotframework-tidy-4.3.0/robotidy/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:41:57.137647 robotframework-tidy-4.3.0/robotidy/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-30 10:41:56.000000 robotframework-tidy-4.3.0/robotidy/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-30 10:41:56.000000 robotframework-tidy-4.3.0/robotidy/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/rich_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/skip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:41:57.145647 robotframework-tidy-4.3.0/robotidy/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/AddMissingEnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/AlignKeywordsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/AlignSettingsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/AlignTemplatedTestCases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/AlignTestCasesSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/AlignVariablesSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/DiscardEmptySections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/GenerateDocumentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/IndentNestedKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/InlineIf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/MergeAndOrderSections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/NormalizeAssignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/NormalizeComments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/NormalizeNewLines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/NormalizeSectionHeaderName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/NormalizeSeparators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/NormalizeSettingName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/NormalizeTags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/OrderSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/OrderSettingsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/OrderTags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/RemoveEmptySettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/RenameKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/RenameTestCases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/RenameVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/ReplaceBreakContinue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/ReplaceEmptyValues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/ReplaceReturns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/ReplaceRunKeywordIf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/SmartSortKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/SplitTooLongLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/Translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19687 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23065 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/aligners_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/transformers/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/robotidy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:41:57.145647 robotframework-tidy-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-30 10:41:41.000000 robotframework-tidy-4.3.0/setup.py
```

### Comparing `robotframework-tidy-4.2.1/LICENSE` & `robotframework-tidy-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/PKG-INFO` & `robotframework-tidy-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-tidy
-Version: 4.2.1
+Version: 4.3.0
 Summary: Code autoformatter for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-tidy
 Author: MarketSquare - Robot Framework community
 Author-email: bartek.hirsz@gmail.com
 License: Apache License 2.0
 Keywords: robotframework
 Platform: any
```

### Comparing `robotframework-tidy-4.2.1/README.md` & `robotframework-tidy-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotframework_tidy.egg-info/PKG-INFO` & `robotframework-tidy-4.3.0/robotframework_tidy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-tidy
-Version: 4.2.1
+Version: 4.3.0
 Summary: Code autoformatter for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-tidy
 Author: MarketSquare - Robot Framework community
 Author-email: bartek.hirsz@gmail.com
 License: Apache License 2.0
 Keywords: robotframework
 Platform: any
```

### Comparing `robotframework-tidy-4.2.1/robotframework_tidy.egg-info/SOURCES.txt` & `robotframework-tidy-4.3.0/robotframework_tidy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/api.py` & `robotframework-tidy-4.3.0/robotidy/api.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/app.py` & `robotframework-tidy-4.3.0/robotidy/app.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/cli.py` & `robotframework-tidy-4.3.0/robotidy/cli.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/config.py` & `robotframework-tidy-4.3.0/robotidy/config.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/decorators.py` & `robotframework-tidy-4.3.0/robotidy/decorators.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/disablers.py` & `robotframework-tidy-4.3.0/robotidy/disablers.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/exceptions.py` & `robotframework-tidy-4.3.0/robotidy/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/files.py` & `robotframework-tidy-4.3.0/robotidy/files.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/skip.py` & `robotframework-tidy-4.3.0/robotidy/skip.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/AddMissingEnd.py` & `robotframework-tidy-4.3.0/robotidy/transformers/AddMissingEnd.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/AlignKeywordsSection.py` & `robotframework-tidy-4.3.0/robotidy/transformers/AlignKeywordsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/AlignSettingsSection.py` & `robotframework-tidy-4.3.0/robotidy/transformers/AlignSettingsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/AlignTemplatedTestCases.py` & `robotframework-tidy-4.3.0/robotidy/transformers/AlignTemplatedTestCases.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/AlignTestCasesSection.py` & `robotframework-tidy-4.3.0/robotidy/transformers/AlignTestCasesSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/AlignVariablesSection.py` & `robotframework-tidy-4.3.0/robotidy/transformers/AlignVariablesSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/DiscardEmptySections.py` & `robotframework-tidy-4.3.0/robotidy/transformers/DiscardEmptySections.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/GenerateDocumentation.py` & `robotframework-tidy-4.3.0/robotidy/transformers/GenerateDocumentation.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/IndentNestedKeywords.py` & `robotframework-tidy-4.3.0/robotidy/transformers/IndentNestedKeywords.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         separator = self.get_separator()
         new_line = get_new_line(indent)
         tokens = [indent, node.data_tokens[0], separator, *join_tokens_with_token(lines[0][1], separator)]
         comment = merge_comments_into_one(node.tokens)
         if comment:
             # need to add comments on first line for [Setup] / [Teardown] settings
             comment_sep = Token(Token.SEPARATOR, "  ")
-            tokens.extend([comment_sep, Token(Token.COMMENT, comment)])
+            tokens.extend([comment_sep, comment])
         node.tokens = self.parse_keyword_lines(lines, tokens, new_line, eol=node.tokens[-1])
         return node
 
     visit_Teardown = visit_Setup
 
     @skip_if_disabled
     def visit_KeywordCall(self, node):  # noqa
```

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/InlineIf.py` & `robotframework-tidy-4.3.0/robotidy/transformers/InlineIf.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/MergeAndOrderSections.py` & `robotframework-tidy-4.3.0/robotidy/transformers/MergeAndOrderSections.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeAssignments.py` & `robotframework-tidy-4.3.0/robotidy/transformers/NormalizeAssignments.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeComments.py` & `robotframework-tidy-4.3.0/robotidy/transformers/NormalizeComments.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeNewLines.py` & `robotframework-tidy-4.3.0/robotidy/transformers/NormalizeNewLines.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeSectionHeaderName.py` & `robotframework-tidy-4.3.0/robotidy/transformers/NormalizeSectionHeaderName.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeSeparators.py` & `robotframework-tidy-4.3.0/robotidy/transformers/NormalizeSeparators.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,19 +29,31 @@
             "skip_keyword_call_pattern",
             "skip_comments",
             "skip_block_comments",
             "skip_sections",
         }
     )
 
-    def __init__(self, flatten_lines: bool = False, skip: Skip = None):
+    def __init__(self, flatten_lines: bool = False, align_new_line: bool = False, skip: Skip = None):
         super().__init__(skip=skip)
         self.indent = 0
         self.flatten_lines = flatten_lines
         self.is_inline = False
+        self.align_new_line = align_new_line
+        self._allowed_line_length = None  # we can only retrieve it after all transformers are initialized
+
+    @property
+    def allowed_line_length(self) -> int:
+        """Get line length from SplitTooLongLine transformer or global config."""
+        if self._allowed_line_length is None:
+            if "SplitTooLongLine" in self.transformers:
+                self._allowed_line_length = self.transformers["SplitTooLongLine"].line_length
+            else:
+                self._allowed_line_length = self.formatting_config.line_length
+        return self._allowed_line_length
 
     def visit_File(self, node):  # noqa
         self.indent = 0
         return self.generic_visit(node)
 
     @skip_section_if_disabled
     def visit_Section(self, node):  # noqa
@@ -154,30 +166,48 @@
         statement.tokens = new_tokens
         self.generic_visit(statement)
         return statement
 
     def handle_spaces(self, statement, has_pipes, only_indent=False):
         new_tokens = []
         prev_token = None
+        first_col_width = 0
+        first_data_token = True
+        is_sep_after_first_data_token = False
+        align_continuation = self.align_new_line
         for line in statement.lines:
             prev_sep = False
+            line_length = 0
             for index, token in enumerate(line):
                 if token.type == Token.SEPARATOR:
                     if prev_sep:
                         continue
                     prev_sep = True
                     if index == 0 and not self.is_keyword_inside_inline_if(statement):
                         token.value = self.formatting_config.indent * self.indent
                     elif not only_indent:
                         if prev_token and prev_token.type == Token.CONTINUATION:
-                            token.value = self.formatting_config.continuation_indent
+                            if align_continuation:
+                                token.value = first_col_width * " "
+                            else:
+                                token.value = self.formatting_config.continuation_indent
                         else:
                             token.value = self.formatting_config.separator
                 else:
                     prev_sep = False
+                    if align_continuation:
+                        if first_data_token:
+                            first_col_width += max(len(token.value), 3) - 3  # remove ... token length
+                            # Check if first line is not longer than allowed line length - we cant align over limit
+                            align_continuation = align_continuation and first_col_width < self.allowed_line_length
+                            first_data_token = False
+                        elif not is_sep_after_first_data_token and token.type != Token.EOL:
+                            is_sep_after_first_data_token = True
+                            first_col_width += len(self.formatting_config.separator)
                     prev_token = token
                 if has_pipes and index == len(line) - 2:
                     token.value = token.value.rstrip()
+                line_length += len(token.value)
                 new_tokens.append(token)
         statement.tokens = new_tokens
         self.generic_visit(statement)
         return statement
```

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeSettingName.py` & `robotframework-tidy-4.3.0/robotidy/transformers/NormalizeSettingName.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeTags.py` & `robotframework-tidy-4.3.0/robotidy/transformers/NormalizeTags.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/OrderSettings.py` & `robotframework-tidy-4.3.0/robotidy/transformers/OrderSettings.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/OrderSettingsSection.py` & `robotframework-tidy-4.3.0/robotidy/transformers/OrderSettingsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/OrderTags.py` & `robotframework-tidy-4.3.0/robotidy/transformers/OrderTags.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/RemoveEmptySettings.py` & `robotframework-tidy-4.3.0/robotidy/transformers/RemoveEmptySettings.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/RenameKeywords.py` & `robotframework-tidy-4.3.0/robotidy/transformers/RenameKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/RenameTestCases.py` & `robotframework-tidy-4.3.0/robotidy/transformers/RenameTestCases.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/RenameVariables.py` & `robotframework-tidy-4.3.0/robotidy/transformers/RenameVariables.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/ReplaceBreakContinue.py` & `robotframework-tidy-4.3.0/robotidy/transformers/ReplaceBreakContinue.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/ReplaceEmptyValues.py` & `robotframework-tidy-4.3.0/robotidy/transformers/ReplaceEmptyValues.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/ReplaceReturns.py` & `robotframework-tidy-4.3.0/robotidy/transformers/ReplaceReturns.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/ReplaceRunKeywordIf.py` & `robotframework-tidy-4.3.0/robotidy/transformers/ReplaceRunKeywordIf.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/SmartSortKeywords.py` & `robotframework-tidy-4.3.0/robotidy/transformers/SmartSortKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/SplitTooLongLine.py` & `robotframework-tidy-4.3.0/robotidy/transformers/SplitTooLongLine.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/Translate.py` & `robotframework-tidy-4.3.0/robotidy/transformers/Translate.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/__init__.py` & `robotframework-tidy-4.3.0/robotidy/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/aligners_core.py` & `robotframework-tidy-4.3.0/robotidy/transformers/aligners_core.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/transformers/run_keywords.py` & `robotframework-tidy-4.3.0/robotidy/transformers/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.1/robotidy/utils.py` & `robotframework-tidy-4.3.0/robotidy/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -308,22 +308,30 @@
     return statement([indent, Token(statement.type), *tokens])
 
 
 def wrap_in_if_and_replace_statement(node, statement, default_separator):
     if len(node.data_tokens) < 2:
         return node
     condition = node.data_tokens[1]
+    separator = Token(Token.SEPARATOR, default_separator)
     indent = Token(Token.SEPARATOR, node.tokens[0].value + default_separator)
-    indented_tokens = replace_indent_in_lines(node, default_separator)
-    body = create_statement_from_tokens(statement=statement, tokens=indented_tokens[4:], indent=indent)
+    merged_comment = merge_comments_into_one(node.tokens)
+    data_tokens = join_tokens_with_token(node.data_tokens[2:], separator)
+    if data_tokens:
+        data_tokens.insert(0, separator)
+    if merged_comment:
+        data_tokens.append(Token(Token.SEPARATOR, "  "))
+        data_tokens.append(merged_comment)
+    data_tokens.append(Token(Token.EOL))
+    body = create_statement_from_tokens(statement=statement, tokens=data_tokens, indent=indent)
     header = IfHeader(
         [
             node.tokens[0],
             Token(Token.IF),
-            Token(Token.SEPARATOR, default_separator),
+            separator,
             condition,
             Token(Token.EOL),
         ]
     )
     end = End.from_params(indent=node.tokens[0].value)
     if_block = If(header=header, body=[body], orelse=None, end=end)
     return if_block
@@ -350,15 +358,15 @@
     comments = []
     for token in tokens:
         if token.type == Token.COMMENT:
             comments.append(token.value.lstrip("#").strip())
     if not comments:
         return None
     comment = " ".join(comments)
-    return f"# {comment}"
+    return Token(Token.COMMENT, f"# {comment}")
 
 
 def collect_comments_from_tokens(tokens, indent):
     comments = get_comments(tokens)
     eol = Token(Token.EOL)
     if indent:
         return [Comment([indent, comment, eol]) for comment in comments]
```

### Comparing `robotframework-tidy-4.2.1/setup.py` & `robotframework-tidy-4.3.0/setup.py`

 * *Files identical despite different names*

