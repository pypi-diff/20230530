# Comparing `tmp/smartgpt-0.1.2.1.tar.gz` & `tmp/smartgpt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartgpt-0.1.2.1.tar", last modified: Mon May 15 04:28:54 2023, max compression
+gzip compressed data, was "smartgpt-0.1.3.tar", last modified: Mon May 29 22:22:25 2023, max compression
```

## Comparing `smartgpt-0.1.2.1.tar` & `smartgpt-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,94 @@
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 04:28:54.093422 smartgpt-0.1.2.1/
--rw-r--r--   0 evan       (501) staff       (20)     1067 2023-05-11 06:26:43.000000 smartgpt-0.1.2.1/LICENSE
--rw-r--r--   0 evan       (501) staff       (20)      176 2023-05-15 04:28:54.093558 smartgpt-0.1.2.1/PKG-INFO
--rw-r--r--   0 evan       (501) staff       (20)     2273 2023-05-14 20:48:56.000000 smartgpt-0.1.2.1/README.md
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 04:28:54.086255 smartgpt-0.1.2.1/bin/
--rwxrwxrwx   0 evan       (501) staff       (20)     5058 2023-05-15 03:51:22.000000 smartgpt-0.1.2.1/bin/smartgpt
--rw-r--r--   0 evan       (501) staff       (20)       62 2023-05-11 06:10:56.000000 smartgpt-0.1.2.1/pyproject.toml
--rw-r--r--   0 evan       (501) staff       (20)      103 2023-05-15 04:28:54.094391 smartgpt-0.1.2.1/setup.cfg
--rw-r--r--   0 evan       (501) staff       (20)      682 2023-05-15 04:27:39.000000 smartgpt-0.1.2.1/setup.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 04:28:54.089912 smartgpt-0.1.2.1/smartgpt/
--rw-r--r--   0 evan       (501) staff       (20)      237 2023-05-15 04:22:03.000000 smartgpt-0.1.2.1/smartgpt/__init__.py
--rw-r--r--   0 evan       (501) staff       (20)    10063 2023-05-15 03:44:52.000000 smartgpt-0.1.2.1/smartgpt/chat.py
--rw-r--r--   0 evan       (501) staff       (20)     5538 2023-05-15 03:50:20.000000 smartgpt-0.1.2.1/smartgpt/datatypes.py
--rw-r--r--   0 evan       (501) staff       (20)     1130 2023-05-15 03:44:52.000000 smartgpt-0.1.2.1/smartgpt/error.py
--rw-r--r--   0 evan       (501) staff       (20)     1510 2023-05-15 01:46:46.000000 smartgpt-0.1.2.1/smartgpt/logger.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 04:28:54.093095 smartgpt-0.1.2.1/smartgpt/prompts/
--rw-r--r--   0 evan       (501) staff       (20)      995 2023-05-14 20:45:10.000000 smartgpt-0.1.2.1/smartgpt/prompts/__init__.py
--rw-r--r--   0 evan       (501) staff       (20)     2113 2023-05-15 03:31:58.000000 smartgpt-0.1.2.1/smartgpt/repl.py
--rw-r--r--   0 evan       (501) staff       (20)     1379 2023-05-11 06:10:56.000000 smartgpt-0.1.2.1/smartgpt/strenum.py
--rw-r--r--   0 evan       (501) staff       (20)      808 2023-05-15 00:52:53.000000 smartgpt-0.1.2.1/smartgpt/user_profile.py
--rw-r--r--   0 evan       (501) staff       (20)      900 2023-05-15 03:44:53.000000 smartgpt-0.1.2.1/smartgpt/util.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 04:28:54.092712 smartgpt-0.1.2.1/smartgpt.egg-info/
--rw-r--r--   0 evan       (501) staff       (20)      176 2023-05-15 04:28:54.000000 smartgpt-0.1.2.1/smartgpt.egg-info/PKG-INFO
--rw-r--r--   0 evan       (501) staff       (20)      459 2023-05-15 04:28:54.000000 smartgpt-0.1.2.1/smartgpt.egg-info/SOURCES.txt
--rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-15 04:28:54.000000 smartgpt-0.1.2.1/smartgpt.egg-info/dependency_links.txt
--rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-15 00:27:20.000000 smartgpt-0.1.2.1/smartgpt.egg-info/not-zip-safe
--rw-r--r--   0 evan       (501) staff       (20)       42 2023-05-15 04:28:54.000000 smartgpt-0.1.2.1/smartgpt.egg-info/requires.txt
--rw-r--r--   0 evan       (501) staff       (20)        9 2023-05-15 04:28:54.000000 smartgpt-0.1.2.1/smartgpt.egg-info/top_level.txt
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.701727 smartgpt-0.1.3/
+-rw-r--r--   0 evan       (501) staff       (20)     1067 2023-05-11 06:26:43.000000 smartgpt-0.1.3/LICENSE
+-rw-r--r--   0 evan       (501) staff       (20)       38 2023-05-29 22:15:45.000000 smartgpt-0.1.3/MANIFEST.in
+-rw-r--r--   0 evan       (501) staff       (20)      174 2023-05-29 22:22:25.701938 smartgpt-0.1.3/PKG-INFO
+-rw-r--r--   0 evan       (501) staff       (20)     5098 2023-05-29 22:13:30.000000 smartgpt-0.1.3/README.md
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.632641 smartgpt-0.1.3/bin/
+-rwxrwxrwx   0 evan       (501) staff       (20)     4771 2023-05-29 21:20:34.000000 smartgpt-0.1.3/bin/smartgpt
+-rw-r--r--   0 evan       (501) staff       (20)       62 2023-05-11 06:10:56.000000 smartgpt-0.1.3/pyproject.toml
+-rw-r--r--   0 evan       (501) staff       (20)      103 2023-05-29 22:22:25.702895 smartgpt-0.1.3/setup.cfg
+-rw-r--r--   0 evan       (501) staff       (20)      698 2023-05-29 22:22:10.000000 smartgpt-0.1.3/setup.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.636418 smartgpt-0.1.3/smartgpt/
+-rw-r--r--   0 evan       (501) staff       (20)      223 2023-05-29 22:15:53.000000 smartgpt-0.1.3/smartgpt/__init__.py
+-rw-r--r--   0 evan       (501) staff       (20)     7794 2023-05-29 22:11:12.000000 smartgpt-0.1.3/smartgpt/chat.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.640998 smartgpt-0.1.3/smartgpt/data/
+-rw-r--r--   0 evan       (501) staff       (20)      775 2023-05-29 19:43:19.000000 smartgpt-0.1.3/smartgpt/data/__init__.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.697622 smartgpt-0.1.3/smartgpt/data/questions/
+-rw-r--r--   0 evan       (501) staff       (20)    17358 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/abstract_algebra_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    29844 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/anatomy_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    42999 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/astronomy_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    31394 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/business_ethics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    56562 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/clinical_knowledge_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    45351 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/college_biology_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    22314 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/college_chemistry_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    40401 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/college_computer_science_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    22429 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/college_mathematics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    78334 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/college_medicine_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    27811 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/college_physics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    24840 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/computer_security_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    34992 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/conceptual_physics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    44039 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/econometrics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    21595 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/electrical_engineering_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    61602 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/elementary_mathematics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    46929 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/formal_logic_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    16191 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/global_facts_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   102424 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_biology_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    53918 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_chemistry_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    42281 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_computer_science_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   266888 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_european_history_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    37386 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_geography_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    61553 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_government_and_politics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   108402 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_macroeconomics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    48584 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_mathematics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    70131 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_microeconomics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    56252 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_physics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   146542 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_psychology_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   105978 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_statistics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   292834 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_us_history_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   373770 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_world_history_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    40617 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/human_aging_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    29052 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/human_sexuality_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    50691 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/international_law_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    31375 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/jurisprudence_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    46290 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/logical_fallacies_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    31698 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/machine_learning_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    17457 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/management_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    57435 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/marketing_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    18520 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/medical_genetics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   129221 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/miscellaneous_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    99902 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/moral_disputes_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   361484 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/moral_scenarios_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    85926 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/nutrition_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    72820 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/philosophy_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    82193 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/prehistory_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   118484 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/professional_accounting_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)  1867637 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/professional_law_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   211585 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/professional_medicine_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   212333 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/professional_psychology_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    26236 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/public_relations_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   199745 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/security_studies_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    61540 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/sociology_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    26047 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/us_foreign_policy_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    34689 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/virology_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    21156 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/world_religions_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)      369 2023-05-15 21:55:11.000000 smartgpt-0.1.3/smartgpt/datatypes.py
+-rw-r--r--   0 evan       (501) staff       (20)     1130 2023-05-15 03:44:52.000000 smartgpt-0.1.3/smartgpt/error.py
+-rw-r--r--   0 evan       (501) staff       (20)     1510 2023-05-15 01:46:46.000000 smartgpt-0.1.3/smartgpt/logger.py
+-rw-r--r--   0 evan       (501) staff       (20)     4559 2023-05-29 22:11:05.000000 smartgpt-0.1.3/smartgpt/message.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.698465 smartgpt-0.1.3/smartgpt/prompts/
+-rw-r--r--   0 evan       (501) staff       (20)      995 2023-05-14 20:45:10.000000 smartgpt-0.1.3/smartgpt/prompts/__init__.py
+-rw-r--r--   0 evan       (501) staff       (20)     2168 2023-05-29 16:27:13.000000 smartgpt-0.1.3/smartgpt/repl.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.701223 smartgpt-0.1.3/smartgpt/settings/
+-rw-r--r--   0 evan       (501) staff       (20)      269 2023-05-15 21:27:25.000000 smartgpt-0.1.3/smartgpt/settings/__init__.py
+-rw-r--r--   0 evan       (501) staff       (20)      195 2023-05-15 21:16:04.000000 smartgpt-0.1.3/smartgpt/settings/constants.py
+-rw-r--r--   0 evan       (501) staff       (20)     1628 2023-05-29 16:11:32.000000 smartgpt-0.1.3/smartgpt/settings/credentials.py
+-rw-r--r--   0 evan       (501) staff       (20)     2435 2023-05-29 16:28:24.000000 smartgpt-0.1.3/smartgpt/settings/user.py
+-rw-r--r--   0 evan       (501) staff       (20)     1379 2023-05-11 06:10:56.000000 smartgpt-0.1.3/smartgpt/strenum.py
+-rw-r--r--   0 evan       (501) staff       (20)      900 2023-05-15 03:44:53.000000 smartgpt-0.1.3/smartgpt/util.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.640102 smartgpt-0.1.3/smartgpt.egg-info/
+-rw-r--r--   0 evan       (501) staff       (20)      174 2023-05-29 22:22:25.000000 smartgpt-0.1.3/smartgpt.egg-info/PKG-INFO
+-rw-r--r--   0 evan       (501) staff       (20)     3532 2023-05-29 22:22:25.000000 smartgpt-0.1.3/smartgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-29 22:22:25.000000 smartgpt-0.1.3/smartgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-15 00:27:20.000000 smartgpt-0.1.3/smartgpt.egg-info/not-zip-safe
+-rw-r--r--   0 evan       (501) staff       (20)       49 2023-05-29 22:22:25.000000 smartgpt-0.1.3/smartgpt.egg-info/requires.txt
+-rw-r--r--   0 evan       (501) staff       (20)        9 2023-05-29 22:22:25.000000 smartgpt-0.1.3/smartgpt.egg-info/top_level.txt
```

### Comparing `smartgpt-0.1.2.1/LICENSE` & `smartgpt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.2.1/bin/smartgpt` & `smartgpt-0.1.3/bin/smartgpt`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 #!/usr/bin/env python
 
 import argparse
-import sys
 import textwrap
 
-from smartgpt import Mode, Settings, SmartGPT, Verbosity
-from smartgpt.user_profile import SETTINGS_PATH
-from smartgpt.util import color_text
+from smartgpt.chat import SmartGPT
+from smartgpt.datatypes import Mode, Verbosity
+from smartgpt.settings.constants import SETTINGS_PATH
+from smartgpt.settings.credentials import Credentials
+from smartgpt.settings.user import UserSettings
 
 
 def main(args: argparse.Namespace) -> None:
-    if args.print_settings_file:
-        print_settings_file_and_exit()
+    settings = override_settings_with_CLI_args(UserSettings.default(), args)
+    credentials = Credentials.default()
 
-    settings = override_settings_with_CLI_args(Settings.load(SETTINGS_PATH), args)
-
-    print_settings(settings)
+    print_settings(settings, credentials)
 
     app = SmartGPT.create(settings)
     app.repl()
 
 
-def print_settings_file_and_exit() -> None:
-    print(f"The contents of {SETTINGS_PATH}:\n")
-    print(color_text(open(SETTINGS_PATH).read(), color="cyan"))
-    sys.exit()
-
-
-def print_settings(settings: Settings) -> None:
-    print(settings)
+def print_settings(settings: UserSettings, credentials: Credentials) -> None:
+    print(f"{settings}\n    {credentials}\n")
 
 
 def override_settings_with_CLI_args(
-    settings: Settings, args: argparse.Namespace
-) -> Settings:
+    settings: UserSettings, args: argparse.Namespace
+) -> UserSettings:
     """Overwrites settings attributes with those specified in CLI"""
     if args.mode is not None:
         settings.mode = args.mode
     if args.verbosity:
         settings.verbosity = args.verbosity
     if args.model:
         settings.model = args.model
@@ -119,18 +112,10 @@
         ),
     )
     parser.add_argument(
         "--model",
         required=False,
         help=("The name of the model you want (e.g. gpt-4, gpt-3.5-turbo)"),
     )
-    parser.add_argument(
-        "--print-settings-file",
-        action="store_true",
-        help=(
-            "Prints the settings file and location. Modify this file to change the "
-            "default behavior."
-        ),
-    )
     args = parser.parse_args()
 
     main(args)
```

### Comparing `smartgpt-0.1.2.1/setup.py` & `smartgpt-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 
 
 if sys.version_info < (3, 8):
     sys.exit(error_msg())
 
 setup(
     name="smartgpt",
-    version="0.1.2.1",
+    version="0.1.3",
     packages=find_packages(),
     scripts=["bin/smartgpt"],
     author_email="kiefl.evan@gmail.com",
     author="Evan Kiefl",
     url="https://github.com/ekiefl/smartgpt",
     install_requires=[
         "openai",
         "attrs",
         "cattrs",
+        "pandas",
         "pyyaml",
         "prompt_toolkit",
     ],
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `smartgpt-0.1.2.1/smartgpt/chat.py` & `smartgpt-0.1.3/smartgpt/chat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,127 +1,50 @@
-"""This module is a wrapper around OpenAI's GPT model
-
-It defines two main classes, Agent
-and SmartGPT, which together facilitate interactive sessions with the AI model. The
-module supports different modes of interaction, including zero-shot, "step-by-step"
-chain of thought prompt flavoring, and the full "SmartGPT" resolver mode.
-
-Classes:
-    Agent:
-        Represents an interface to the GPT model.
-    SmartGPT:
-        Manages interactive sessions with the AI, supporting different modes of
-        interaction.
-"""
-
 from __future__ import annotations
 
 import copy
 import logging
-import time
-from typing import Dict, List, Optional
+from typing import List, Optional
 
 import attrs
-import openai
-from openai.error import InvalidRequestError, RateLimitError
 
 from smartgpt import prompts
-from smartgpt.datatypes import (
-    Credentials,
-    GPTConfig,
-    Message,
-    Mode,
-    Response,
-    Role,
-    Settings,
-    Verbosity,
-)
-from smartgpt.logger import default_logger, get_logger
+from smartgpt.datatypes import Mode, Verbosity
+from smartgpt.logger import get_logger
+from smartgpt.message import GPTBot, Message, Role
 from smartgpt.repl import repl
-from smartgpt.user_profile import SETTINGS_PATH
+from smartgpt.settings.credentials import Credentials
+from smartgpt.settings.user import UserSettings
 
 
-@attrs.define
-class Agent:
-    """Represents an interface to the GPT model.
-
-    It encapsulates the process of sending messages to the model and receiving
-    responses. The class also handles message history.
+@attrs.define(frozen=True)
+class GPTConfig:
+    """Configuration for the GPT model.
 
     Attributes:
-        messages:
-            A list of messages sent to and received from the model.
+        model:
+            The GPT model to use (default is 'gpt-4').
         credentials:
             Credentials for accessing the model.
-        model:
-            The model to use (default is 'gpt-4').
-        temp:
-            The temperature parameter to use when generating responses.
+        mode:
+            The mode of interaction.
     """
 
-    messages: List[Dict[str, str]] = attrs.field(factory=list)
-    credentials: Credentials = attrs.field(default=Settings.default().credentials)
     model: str = attrs.field(default="gpt-4")
-    temp: float = attrs.field(default=0.5)
-
-    def append_message(self, message: Message) -> None:
-        """Appends a message to the current message history.
+    credentials: Credentials = attrs.field(default=Credentials.default())
+    mode: Mode = attrs.field(default=Mode.ZERO_SHOT)
 
-        Args:
-            message: The message to append.
-        """
-        self.messages.append(attrs.asdict(message))
-
-    def request(self) -> Response:
-        """Sends the current message history to the GPT model via an API request
-
-        The message history includes all previous interactions, which allows the model
-        to generate a response based on the entire conversation context.
-
-        Returns:
-            Response:
-                A Response object that encapsulates the model's response, which includes
-                the generated message, remaining tokens, and other metadata.
-        """
-
-        try:
-            return Response.from_openai_response(
-                openai.ChatCompletion.create(
-                    model=self.model,
-                    messages=self.messages,
-                    api_key=self.credentials.key,
-                )
-            )
-        except RateLimitError:
-            default_logger.info("Hit rate limit. Sleeping for 20 seconds...")
-            time.sleep(20)
-            return self.request()
-        except InvalidRequestError:
-            raise NotImplementedError()
-
-    def response(self, prompt: str) -> Message:
-        """Appends prompt to message history and sends request to the GPT model.
-
-        The model's response is then appended to the message history.
-
-        Args:
-            prompt:
-                The prompt to send to the model.
+    @classmethod
+    def default(cls) -> GPTConfig:
+        """Factory method to create a default GPTConfig.
 
         Returns:
-            Message:
-                The model's response encapsulated in a Message object.
+            GPTConfig:
+                A GPTConfig instance with default values.
         """
-        self.append_message(Message(Role.USER, prompt))
-
-        response = self.request()
-
-        self.append_message(response.message)
-
-        return response.message
+        return cls()
 
 
 @attrs.define
 class SmartGPT:
     """Manages interactive sessions with the AI, supports different interaction modes.
 
     In zero-shot mode, the user's prompts are sent directly to the model. In
@@ -142,26 +65,26 @@
             An agent responsible for considering the researcher's analysis and creating
             the final response.
         generators:
             A list of agents for generating responses in resolver mode.
     """
 
     config: GPTConfig
-    main: Agent
-    researcher: Agent
-    resolver: Agent
-    generators: List[Agent]
+    main: GPTBot
+    researcher: GPTBot
+    resolver: GPTBot
+    generators: List[GPTBot]
     verbosity: Verbosity = Verbosity.SOME
 
     logger: logging.Logger = attrs.field(init=False)
 
     def __attrs_post_init__(self) -> None:
         self.logger = get_logger(verbosity=self.verbosity)
 
-    def create_response(self, prompt: str) -> Message:
+    def response(self, prompt: str) -> Message:
         """
         Determines the mode of interaction based on the current configuration and
         generates a response from the model accordingly.
 
         In ZERO_SHOT mode, the prompt is sent directly to the main agent, which sends it
         to the model and returns the response.
 
@@ -228,58 +151,70 @@
 
             researcher_response = self.researcher.response(researcher_prompt)
             self.logger.debug(f"Researcher response:\n{researcher_response.content}")
 
             self.logger.info("Generating response for resolver...")
 
             resolver_prompt = prompts.you_are_a_resolver(
-                candidates, silence_rationale=(self.verbosity != Verbosity.ALL)
+                candidates, silence_rationale=True
             )
             self.logger.debug(f"Resolver prompt:\n{resolver_prompt}")
 
             self.resolver.messages = copy.deepcopy(self.researcher.messages)
             response = self.resolver.response(resolver_prompt)
+            self.logger.debug(f"Resolver response:\n{response.content}")
 
             # Add the prompt and response to the main agent
             self.main.append_message(Message(Role.USER, candidate_prompt))
             self.main.append_message(response)
 
         logging.debug("Finished generating response")
 
         return response
 
     @classmethod
-    def create(cls, settings: Optional[Settings] = None) -> SmartGPT:
+    def create(
+        cls,
+        settings: Optional[UserSettings] = None,
+        credentials: Optional[Credentials] = None,
+        mode: Optional[Mode] = None,
+    ) -> SmartGPT:
         if settings is None:
-            settings = Settings.load(SETTINGS_PATH)
+            settings = UserSettings.default()
+
+        if credentials is None:
+            credentials = Credentials.default()
+
+        if mode is not None:
+            settings.mode = mode
 
         return cls(
             config=GPTConfig(
-                credentials=settings.credentials,
+                credentials=credentials,
                 model=settings.model,
                 mode=settings.mode,
             ),
-            main=Agent(
-                credentials=settings.credentials,
+            main=GPTBot(
+                credentials=credentials,
                 model=settings.model,
                 temp=settings.resolver_temp,
             ),
-            researcher=Agent(
-                credentials=settings.credentials,
+            researcher=GPTBot(
+                credentials=credentials,
                 model=settings.model,
                 temp=settings.researcher_temp,
             ),
-            resolver=Agent(
-                credentials=settings.credentials,
+            resolver=GPTBot(
+                credentials=credentials,
                 model=settings.model,
                 temp=settings.resolver_temp,
             ),
             generators=[
-                Agent(
-                    credentials=settings.credentials,
+                GPTBot(
+                    credentials=credentials,
                     model=settings.model,
                     temp=settings.generator_temps[i],
                 )
                 for i in range(settings.num_agents)
             ],
             verbosity=settings.verbosity,
         )
```

### Comparing `smartgpt-0.1.2.1/smartgpt/error.py` & `smartgpt-0.1.3/smartgpt/error.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.2.1/smartgpt/logger.py` & `smartgpt-0.1.3/smartgpt/logger.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.2.1/smartgpt/prompts/__init__.py` & `smartgpt-0.1.3/smartgpt/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.2.1/smartgpt/repl.py` & `smartgpt-0.1.3/smartgpt/repl.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from typing import Protocol, Tuple
 
 from prompt_toolkit import PromptSession
 from prompt_toolkit.formatted_text import FormattedText
 from prompt_toolkit.history import FileHistory
 
-from smartgpt.datatypes import Message, Settings
-from smartgpt.user_profile import MAX_HISTORY, REPL_HISTORY_PATH, SETTINGS_PATH
+from smartgpt.message import Message
+from smartgpt.settings.constants import REPL_HISTORY_PATH
+from smartgpt.settings.user import UserSettings
+
+MAX_HISTORY = 3000
 
 
 class LimitedFileHistory(FileHistory):
     def __init__(self, filename, max_size):
         super().__init__(filename)
         self.max_size = max_size
 
@@ -26,53 +29,53 @@
                 f.writelines(lines[-self.max_size :])  # Keep last max_size lines
 
 
 session: PromptSession = PromptSession(
     history=LimitedFileHistory(str(REPL_HISTORY_PATH), MAX_HISTORY),
     multiline=True,
     wrap_lines=True,
-    vi_mode=Settings.load(SETTINGS_PATH).vi_mode,
+    vi_mode=UserSettings.default().vi_mode,
 )
 
 
 USER_PREFIX = FormattedText(
     [
         ("", "(To submit: press ESC, then ENTER)\n"),
         ("bold fg:ansigreen", "> "),
     ]
 )
 
 
 class Model(Protocol):
-    def create_response(self, prompt: str) -> Message:
+    def response(self, prompt: str) -> Message:
         ...
 
 
-def repl(model: Model) -> None:
+def repl(model: Model, quiet: bool = False) -> None:
     """Starts the Read-Eval-Print-Loop (REPL) for interaction with a model
 
     This function runs indefinitely until the session is manually terminated.
     """
     while True:
-        _, _ = repl_iteration(model)
+        _, _ = repl_iteration(model, quiet=quiet)
 
 
-def repl_iteration(model: Model, quiet=False) -> Tuple[str, str]:
+def repl_iteration(model: Model, quiet: bool = True) -> Tuple[str, str]:
     """Executes a single pass of the Read-Eval-Print-Loop (REPL)
 
     Args:
         quiet:
             If true, the function will not print the model's response. Default is
             False.
 
     Returns:
         Tuple[str, str]:
             The user's prompt and the model's response.
     """
     prompt = session.prompt(USER_PREFIX)
 
-    response_message = model.create_response(prompt)
+    response_message = model.response(prompt)
 
     if not quiet:
         print(f"\n{response_message.content}\n")
 
     return prompt, response_message.content
```

### Comparing `smartgpt-0.1.2.1/smartgpt/strenum.py` & `smartgpt-0.1.3/smartgpt/strenum.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.2.1/smartgpt/util.py` & `smartgpt-0.1.3/smartgpt/util.py`

 * *Files identical despite different names*

