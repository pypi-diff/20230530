# Comparing `tmp/smartgpt-0.1.3.tar.gz` & `tmp/smartgpt-0.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartgpt-0.1.3.tar", last modified: Mon May 29 22:22:25 2023, max compression
+gzip compressed data, was "smartgpt-0.1.3.1.tar", last modified: Mon May 29 22:43:53 2023, max compression
```

## Comparing `smartgpt-0.1.3.tar` & `smartgpt-0.1.3.1.tar`

### file list

```diff
@@ -1,94 +1,97 @@
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.701727 smartgpt-0.1.3/
--rw-r--r--   0 evan       (501) staff       (20)     1067 2023-05-11 06:26:43.000000 smartgpt-0.1.3/LICENSE
--rw-r--r--   0 evan       (501) staff       (20)       38 2023-05-29 22:15:45.000000 smartgpt-0.1.3/MANIFEST.in
--rw-r--r--   0 evan       (501) staff       (20)      174 2023-05-29 22:22:25.701938 smartgpt-0.1.3/PKG-INFO
--rw-r--r--   0 evan       (501) staff       (20)     5098 2023-05-29 22:13:30.000000 smartgpt-0.1.3/README.md
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.632641 smartgpt-0.1.3/bin/
--rwxrwxrwx   0 evan       (501) staff       (20)     4771 2023-05-29 21:20:34.000000 smartgpt-0.1.3/bin/smartgpt
--rw-r--r--   0 evan       (501) staff       (20)       62 2023-05-11 06:10:56.000000 smartgpt-0.1.3/pyproject.toml
--rw-r--r--   0 evan       (501) staff       (20)      103 2023-05-29 22:22:25.702895 smartgpt-0.1.3/setup.cfg
--rw-r--r--   0 evan       (501) staff       (20)      698 2023-05-29 22:22:10.000000 smartgpt-0.1.3/setup.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.636418 smartgpt-0.1.3/smartgpt/
--rw-r--r--   0 evan       (501) staff       (20)      223 2023-05-29 22:15:53.000000 smartgpt-0.1.3/smartgpt/__init__.py
--rw-r--r--   0 evan       (501) staff       (20)     7794 2023-05-29 22:11:12.000000 smartgpt-0.1.3/smartgpt/chat.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.640998 smartgpt-0.1.3/smartgpt/data/
--rw-r--r--   0 evan       (501) staff       (20)      775 2023-05-29 19:43:19.000000 smartgpt-0.1.3/smartgpt/data/__init__.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.697622 smartgpt-0.1.3/smartgpt/data/questions/
--rw-r--r--   0 evan       (501) staff       (20)    17358 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/abstract_algebra_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    29844 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/anatomy_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    42999 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/astronomy_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    31394 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/business_ethics_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    56562 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/clinical_knowledge_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    45351 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/college_biology_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    22314 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/college_chemistry_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    40401 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/college_computer_science_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    22429 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/college_mathematics_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    78334 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/college_medicine_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    27811 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/college_physics_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    24840 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/computer_security_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    34992 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/conceptual_physics_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    44039 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/econometrics_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    21595 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/electrical_engineering_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    61602 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/elementary_mathematics_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    46929 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/formal_logic_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    16191 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/global_facts_test.csv
--rw-r--r--   0 evan       (501) staff       (20)   102424 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_biology_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    53918 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_chemistry_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    42281 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_computer_science_test.csv
--rw-r--r--   0 evan       (501) staff       (20)   266888 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_european_history_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    37386 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_geography_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    61553 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_government_and_politics_test.csv
--rw-r--r--   0 evan       (501) staff       (20)   108402 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_macroeconomics_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    48584 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_mathematics_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    70131 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_microeconomics_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    56252 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_physics_test.csv
--rw-r--r--   0 evan       (501) staff       (20)   146542 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_psychology_test.csv
--rw-r--r--   0 evan       (501) staff       (20)   105978 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_statistics_test.csv
--rw-r--r--   0 evan       (501) staff       (20)   292834 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_us_history_test.csv
--rw-r--r--   0 evan       (501) staff       (20)   373770 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/high_school_world_history_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    40617 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/human_aging_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    29052 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/human_sexuality_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    50691 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/international_law_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    31375 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/jurisprudence_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    46290 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/logical_fallacies_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    31698 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/machine_learning_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    17457 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/management_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    57435 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/marketing_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    18520 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/medical_genetics_test.csv
--rw-r--r--   0 evan       (501) staff       (20)   129221 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/miscellaneous_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    99902 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/moral_disputes_test.csv
--rw-r--r--   0 evan       (501) staff       (20)   361484 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/moral_scenarios_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    85926 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/nutrition_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    72820 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/philosophy_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    82193 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/prehistory_test.csv
--rw-r--r--   0 evan       (501) staff       (20)   118484 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/professional_accounting_test.csv
--rw-r--r--   0 evan       (501) staff       (20)  1867637 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/professional_law_test.csv
--rw-r--r--   0 evan       (501) staff       (20)   211585 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/professional_medicine_test.csv
--rw-r--r--   0 evan       (501) staff       (20)   212333 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/professional_psychology_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    26236 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/public_relations_test.csv
--rw-r--r--   0 evan       (501) staff       (20)   199745 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/security_studies_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    61540 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/sociology_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    26047 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/us_foreign_policy_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    34689 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/virology_test.csv
--rw-r--r--   0 evan       (501) staff       (20)    21156 2023-05-29 15:12:00.000000 smartgpt-0.1.3/smartgpt/data/questions/world_religions_test.csv
--rw-r--r--   0 evan       (501) staff       (20)      369 2023-05-15 21:55:11.000000 smartgpt-0.1.3/smartgpt/datatypes.py
--rw-r--r--   0 evan       (501) staff       (20)     1130 2023-05-15 03:44:52.000000 smartgpt-0.1.3/smartgpt/error.py
--rw-r--r--   0 evan       (501) staff       (20)     1510 2023-05-15 01:46:46.000000 smartgpt-0.1.3/smartgpt/logger.py
--rw-r--r--   0 evan       (501) staff       (20)     4559 2023-05-29 22:11:05.000000 smartgpt-0.1.3/smartgpt/message.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.698465 smartgpt-0.1.3/smartgpt/prompts/
--rw-r--r--   0 evan       (501) staff       (20)      995 2023-05-14 20:45:10.000000 smartgpt-0.1.3/smartgpt/prompts/__init__.py
--rw-r--r--   0 evan       (501) staff       (20)     2168 2023-05-29 16:27:13.000000 smartgpt-0.1.3/smartgpt/repl.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.701223 smartgpt-0.1.3/smartgpt/settings/
--rw-r--r--   0 evan       (501) staff       (20)      269 2023-05-15 21:27:25.000000 smartgpt-0.1.3/smartgpt/settings/__init__.py
--rw-r--r--   0 evan       (501) staff       (20)      195 2023-05-15 21:16:04.000000 smartgpt-0.1.3/smartgpt/settings/constants.py
--rw-r--r--   0 evan       (501) staff       (20)     1628 2023-05-29 16:11:32.000000 smartgpt-0.1.3/smartgpt/settings/credentials.py
--rw-r--r--   0 evan       (501) staff       (20)     2435 2023-05-29 16:28:24.000000 smartgpt-0.1.3/smartgpt/settings/user.py
--rw-r--r--   0 evan       (501) staff       (20)     1379 2023-05-11 06:10:56.000000 smartgpt-0.1.3/smartgpt/strenum.py
--rw-r--r--   0 evan       (501) staff       (20)      900 2023-05-15 03:44:53.000000 smartgpt-0.1.3/smartgpt/util.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:22:25.640102 smartgpt-0.1.3/smartgpt.egg-info/
--rw-r--r--   0 evan       (501) staff       (20)      174 2023-05-29 22:22:25.000000 smartgpt-0.1.3/smartgpt.egg-info/PKG-INFO
--rw-r--r--   0 evan       (501) staff       (20)     3532 2023-05-29 22:22:25.000000 smartgpt-0.1.3/smartgpt.egg-info/SOURCES.txt
--rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-29 22:22:25.000000 smartgpt-0.1.3/smartgpt.egg-info/dependency_links.txt
--rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-15 00:27:20.000000 smartgpt-0.1.3/smartgpt.egg-info/not-zip-safe
--rw-r--r--   0 evan       (501) staff       (20)       49 2023-05-29 22:22:25.000000 smartgpt-0.1.3/smartgpt.egg-info/requires.txt
--rw-r--r--   0 evan       (501) staff       (20)        9 2023-05-29 22:22:25.000000 smartgpt-0.1.3/smartgpt.egg-info/top_level.txt
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:43:53.191620 smartgpt-0.1.3.1/
+-rw-r--r--   0 evan       (501) staff       (20)     1067 2023-05-11 06:26:43.000000 smartgpt-0.1.3.1/LICENSE
+-rw-r--r--   0 evan       (501) staff       (20)       69 2023-05-29 22:42:28.000000 smartgpt-0.1.3.1/MANIFEST.in
+-rw-r--r--   0 evan       (501) staff       (20)      176 2023-05-29 22:43:53.191861 smartgpt-0.1.3.1/PKG-INFO
+-rw-r--r--   0 evan       (501) staff       (20)     5085 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/README.md
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:43:53.110955 smartgpt-0.1.3.1/bin/
+-rwxr-xr-x   0 evan       (501) staff       (20)     4771 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/bin/smartgpt
+-rw-r--r--   0 evan       (501) staff       (20)       62 2023-05-11 06:10:56.000000 smartgpt-0.1.3.1/pyproject.toml
+-rw-r--r--   0 evan       (501) staff       (20)      103 2023-05-29 22:43:53.192942 smartgpt-0.1.3.1/setup.cfg
+-rw-r--r--   0 evan       (501) staff       (20)      700 2023-05-29 22:42:49.000000 smartgpt-0.1.3.1/setup.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:43:53.116905 smartgpt-0.1.3.1/smartgpt/
+-rw-r--r--   0 evan       (501) staff       (20)      225 2023-05-29 22:43:08.000000 smartgpt-0.1.3.1/smartgpt/__init__.py
+-rw-r--r--   0 evan       (501) staff       (20)     7794 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/chat.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:43:53.122127 smartgpt-0.1.3.1/smartgpt/data/
+-rw-r--r--   0 evan       (501) staff       (20)      775 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/__init__.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:43:53.185269 smartgpt-0.1.3.1/smartgpt/data/questions/
+-rw-r--r--   0 evan       (501) staff       (20)    17358 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/abstract_algebra_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    29844 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/anatomy_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    42999 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/astronomy_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    31394 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/business_ethics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    56562 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/clinical_knowledge_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    45351 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/college_biology_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    22314 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/college_chemistry_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    40401 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/college_computer_science_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    22429 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/college_mathematics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    78334 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/college_medicine_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    27811 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/college_physics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    24840 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/computer_security_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    34992 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/conceptual_physics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    44039 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/econometrics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    21595 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/electrical_engineering_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    61602 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/elementary_mathematics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    46929 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/formal_logic_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    16191 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/global_facts_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   102424 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_biology_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    53918 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_chemistry_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    42281 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_computer_science_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   266888 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_european_history_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    37386 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_geography_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    61553 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_government_and_politics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   108402 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_macroeconomics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    48584 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_mathematics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    70131 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_microeconomics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    56252 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_physics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   146542 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_psychology_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   105978 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_statistics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   292834 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_us_history_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   373770 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/high_school_world_history_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    40617 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/human_aging_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    29052 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/human_sexuality_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    50691 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/international_law_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    31375 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/jurisprudence_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    46290 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/logical_fallacies_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    31698 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/machine_learning_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    17457 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/management_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    57435 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/marketing_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    18520 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/medical_genetics_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   129221 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/miscellaneous_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    99902 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/moral_disputes_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   361484 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/moral_scenarios_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    85926 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/nutrition_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    72820 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/philosophy_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    82193 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/prehistory_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   118484 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/professional_accounting_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)  1867637 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/professional_law_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   211585 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/professional_medicine_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   212333 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/professional_psychology_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    26236 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/public_relations_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)   199745 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/security_studies_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    61540 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/sociology_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    26047 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/us_foreign_policy_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    34689 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/virology_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)    21156 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/data/questions/world_religions_test.csv
+-rw-r--r--   0 evan       (501) staff       (20)      369 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/datatypes.py
+-rw-r--r--   0 evan       (501) staff       (20)     1130 2023-05-15 03:44:52.000000 smartgpt-0.1.3.1/smartgpt/error.py
+-rw-r--r--   0 evan       (501) staff       (20)     1510 2023-05-15 01:46:46.000000 smartgpt-0.1.3.1/smartgpt/logger.py
+-rw-r--r--   0 evan       (501) staff       (20)     4559 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/message.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:43:53.188002 smartgpt-0.1.3.1/smartgpt/prompts/
+-rw-r--r--   0 evan       (501) staff       (20)      995 2023-05-29 22:41:50.000000 smartgpt-0.1.3.1/smartgpt/prompts/__init__.py
+-rw-r--r--   0 evan       (501) staff       (20)      295 2023-05-14 21:13:44.000000 smartgpt-0.1.3.1/smartgpt/prompts/researcher.txt
+-rw-r--r--   0 evan       (501) staff       (20)      288 2023-05-14 20:18:41.000000 smartgpt-0.1.3.1/smartgpt/prompts/resolver.txt
+-rw-r--r--   0 evan       (501) staff       (20)      107 2023-05-12 06:44:16.000000 smartgpt-0.1.3.1/smartgpt/prompts/step_by_step.txt
+-rw-r--r--   0 evan       (501) staff       (20)     2168 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/repl.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:43:53.190974 smartgpt-0.1.3.1/smartgpt/settings/
+-rw-r--r--   0 evan       (501) staff       (20)      269 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/settings/__init__.py
+-rw-r--r--   0 evan       (501) staff       (20)      195 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/settings/constants.py
+-rw-r--r--   0 evan       (501) staff       (20)     1628 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/settings/credentials.py
+-rw-r--r--   0 evan       (501) staff       (20)     2435 2023-05-29 22:42:13.000000 smartgpt-0.1.3.1/smartgpt/settings/user.py
+-rw-r--r--   0 evan       (501) staff       (20)     1379 2023-05-11 06:10:56.000000 smartgpt-0.1.3.1/smartgpt/strenum.py
+-rw-r--r--   0 evan       (501) staff       (20)      900 2023-05-15 03:44:53.000000 smartgpt-0.1.3.1/smartgpt/util.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-29 22:43:53.121347 smartgpt-0.1.3.1/smartgpt.egg-info/
+-rw-r--r--   0 evan       (501) staff       (20)      176 2023-05-29 22:43:53.000000 smartgpt-0.1.3.1/smartgpt.egg-info/PKG-INFO
+-rw-r--r--   0 evan       (501) staff       (20)     3628 2023-05-29 22:43:53.000000 smartgpt-0.1.3.1/smartgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-29 22:43:53.000000 smartgpt-0.1.3.1/smartgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-15 00:27:20.000000 smartgpt-0.1.3.1/smartgpt.egg-info/not-zip-safe
+-rw-r--r--   0 evan       (501) staff       (20)       49 2023-05-29 22:43:53.000000 smartgpt-0.1.3.1/smartgpt.egg-info/requires.txt
+-rw-r--r--   0 evan       (501) staff       (20)        9 2023-05-29 22:43:53.000000 smartgpt-0.1.3.1/smartgpt.egg-info/top_level.txt
```

### Comparing `smartgpt-0.1.3/LICENSE` & `smartgpt-0.1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/README.md` & `smartgpt-0.1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SmartGPT
 
-<img src="assets/alg.jpg" width="600" />
+<img src="assets/alg.jpg"/>
 
 SmartGPT uses a collection of GPT-4 agents, each with specific roles, to produce demonstrably higher quality responses than vanilla GPT-4. It also leverages chain-of-thought prompt engineering to boost performance.
 
 SmartGPT was conceived by AIExplained in his video: https://www.youtube.com/watch?v=wVzuvf9D9BU.
 
 ## Explanation of the algorithm
```

### Comparing `smartgpt-0.1.3/bin/smartgpt` & `smartgpt-0.1.3.1/bin/smartgpt`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/setup.py` & `smartgpt-0.1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 if sys.version_info < (3, 8):
     sys.exit(error_msg())
 
 setup(
     name="smartgpt",
-    version="0.1.3",
+    version="0.1.3.1",
     packages=find_packages(),
     scripts=["bin/smartgpt"],
     author_email="kiefl.evan@gmail.com",
     author="Evan Kiefl",
     url="https://github.com/ekiefl/smartgpt",
     install_requires=[
         "openai",
```

### Comparing `smartgpt-0.1.3/smartgpt/chat.py` & `smartgpt-0.1.3.1/smartgpt/chat.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/__init__.py` & `smartgpt-0.1.3.1/smartgpt/data/__init__.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/abstract_algebra_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/abstract_algebra_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/anatomy_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/anatomy_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/astronomy_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/astronomy_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/business_ethics_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/business_ethics_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/clinical_knowledge_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/clinical_knowledge_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/college_biology_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/college_biology_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/college_chemistry_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/college_chemistry_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/college_computer_science_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/college_computer_science_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/college_mathematics_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/college_mathematics_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/college_medicine_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/college_medicine_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/college_physics_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/college_physics_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/computer_security_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/computer_security_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/conceptual_physics_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/conceptual_physics_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/econometrics_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/econometrics_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/electrical_engineering_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/electrical_engineering_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/elementary_mathematics_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/elementary_mathematics_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/formal_logic_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/formal_logic_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/global_facts_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/global_facts_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_biology_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_biology_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_chemistry_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_chemistry_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_computer_science_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_computer_science_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_european_history_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_european_history_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_geography_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_geography_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_government_and_politics_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_government_and_politics_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_macroeconomics_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_macroeconomics_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_mathematics_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_mathematics_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_microeconomics_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_microeconomics_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_physics_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_physics_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_psychology_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_psychology_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_statistics_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_statistics_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_us_history_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_us_history_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/high_school_world_history_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/high_school_world_history_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/human_aging_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/human_aging_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/human_sexuality_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/human_sexuality_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/international_law_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/international_law_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/jurisprudence_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/jurisprudence_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/logical_fallacies_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/logical_fallacies_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/machine_learning_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/machine_learning_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/management_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/management_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/marketing_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/marketing_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/medical_genetics_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/medical_genetics_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/miscellaneous_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/miscellaneous_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/moral_disputes_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/moral_disputes_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/moral_scenarios_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/moral_scenarios_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/nutrition_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/nutrition_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/philosophy_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/philosophy_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/prehistory_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/prehistory_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/professional_accounting_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/professional_accounting_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/professional_law_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/professional_law_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/professional_medicine_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/professional_medicine_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/professional_psychology_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/professional_psychology_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/public_relations_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/public_relations_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/security_studies_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/security_studies_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/sociology_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/sociology_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/us_foreign_policy_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/us_foreign_policy_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/virology_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/virology_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/data/questions/world_religions_test.csv` & `smartgpt-0.1.3.1/smartgpt/data/questions/world_religions_test.csv`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/error.py` & `smartgpt-0.1.3.1/smartgpt/error.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/logger.py` & `smartgpt-0.1.3.1/smartgpt/logger.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/message.py` & `smartgpt-0.1.3.1/smartgpt/message.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/prompts/__init__.py` & `smartgpt-0.1.3.1/smartgpt/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/repl.py` & `smartgpt-0.1.3.1/smartgpt/repl.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/settings/credentials.py` & `smartgpt-0.1.3.1/smartgpt/settings/credentials.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/settings/user.py` & `smartgpt-0.1.3.1/smartgpt/settings/user.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/strenum.py` & `smartgpt-0.1.3.1/smartgpt/strenum.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt/util.py` & `smartgpt-0.1.3.1/smartgpt/util.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.3/smartgpt.egg-info/SOURCES.txt` & `smartgpt-0.1.3.1/smartgpt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -75,11 +75,14 @@
 smartgpt/data/questions/public_relations_test.csv
 smartgpt/data/questions/security_studies_test.csv
 smartgpt/data/questions/sociology_test.csv
 smartgpt/data/questions/us_foreign_policy_test.csv
 smartgpt/data/questions/virology_test.csv
 smartgpt/data/questions/world_religions_test.csv
 smartgpt/prompts/__init__.py
+smartgpt/prompts/researcher.txt
+smartgpt/prompts/resolver.txt
+smartgpt/prompts/step_by_step.txt
 smartgpt/settings/__init__.py
 smartgpt/settings/constants.py
 smartgpt/settings/credentials.py
 smartgpt/settings/user.py
```

