# Comparing `tmp/thipster-0.12.3.tar.gz` & `tmp/thipster-0.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.12.3.tar", last modified: Tue May 30 14:08:34 2023, max compression
+gzip compressed data, was "thipster-0.13.0.tar", last modified: Tue May 30 13:46:15 2023, max compression
```

## Comparing `thipster-0.12.3.tar` & `thipster-0.13.0.tar`

### file list

```diff
@@ -1,74 +1,52 @@
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:34.012536 thipster-0.12.3/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)       80 2023-05-30 12:37:23.000000 thipster-0.12.3/MANIFEST.in
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      114 2023-05-30 14:08:34.012536 thipster-0.12.3/PKG-INFO
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     2697 2023-05-15 08:47:22.000000 thipster-0.12.3/README.md
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      868 2023-05-30 14:06:54.000000 thipster-0.12.3/pyproject.toml
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      117 2023-05-30 12:14:30.000000 thipster-0.12.3/requirements.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)       38 2023-05-30 14:08:34.012536 thipster-0.12.3/setup.cfg
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      582 2023-05-30 14:08:28.000000 thipster-0.12.3/setup.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:33.992536 thipster-0.12.3/tests/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-26 14:12:09.000000 thipster-0.12.3/tests/__init__.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:33.992536 thipster-0.12.3/tests/engine/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-20 08:57:48.000000 thipster-0.12.3/tests/engine/__init__.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     3161 2023-05-30 12:20:19.000000 thipster-0.12.3/tests/engine/test_engine.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:33.992536 thipster-0.12.3/tests/parser/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-20 08:57:48.000000 thipster-0.12.3/tests/parser/__init__.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:33.992536 thipster-0.12.3/tests/parser/dsl_parser/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-21 13:59:54.000000 thipster-0.12.3/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    15501 2023-05-25 08:45:48.000000 thipster-0.12.3/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1330 2023-05-25 08:45:48.000000 thipster-0.12.3/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    13229 2023-05-25 08:45:48.000000 thipster-0.12.3/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      843 2023-05-25 08:45:48.000000 thipster-0.12.3/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     3451 2023-05-25 08:45:48.000000 thipster-0.12.3/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     3005 2023-05-05 15:19:18.000000 thipster-0.12.3/tests/parser/test_ParserFactory.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4136 2023-05-15 08:47:22.000000 thipster-0.12.3/tests/parser/test_YAMLParser.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4673 2023-05-05 15:19:18.000000 thipster-0.12.3/tests/parser/test_parsedfile.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     3680 2023-05-30 12:20:19.000000 thipster-0.12.3/tests/test_e2e.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:34.002536 thipster-0.12.3/thipster/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 07:31:34.000000 thipster-0.12.3/thipster/__init__.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:34.002536 thipster-0.12.3/thipster/auth/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-18 12:21:13.000000 thipster-0.12.3/thipster/auth/__init__.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:34.002536 thipster-0.12.3/thipster/engine/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     2263 2023-05-30 12:20:19.000000 thipster-0.12.3/thipster/engine/Engine.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      435 2023-05-30 12:20:19.000000 thipster-0.12.3/thipster/engine/I_Auth.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      659 2023-05-15 08:47:22.000000 thipster-0.12.3/thipster/engine/I_Parser.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      323 2023-05-10 12:33:34.000000 thipster-0.12.3/thipster/engine/I_Repository.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1610 2023-05-25 08:45:48.000000 thipster-0.12.3/thipster/engine/I_Terraform.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     6123 2023-05-22 13:28:55.000000 thipster-0.12.3/thipster/engine/ParsedFile.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4124 2023-05-25 08:45:48.000000 thipster-0.12.3/thipster/engine/ResourceModel.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-18 12:21:13.000000 thipster-0.12.3/thipster/engine/__init__.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      129 2023-05-10 12:33:34.000000 thipster-0.12.3/thipster/helpers.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:34.002536 thipster-0.12.3/thipster/parser/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     2306 2023-05-15 08:47:22.000000 thipster-0.12.3/thipster/parser/ParserFactory.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     6199 2023-05-15 08:47:22.000000 thipster-0.12.3/thipster/parser/YAMLParser.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-18 12:21:13.000000 thipster-0.12.3/thipster/parser/__init__.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:34.002536 thipster-0.12.3/thipster/parser/dsl_parser/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    10332 2023-05-25 08:45:48.000000 thipster-0.12.3/thipster/parser/dsl_parser/AST.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      399 2023-05-05 15:19:18.000000 thipster-0.12.3/thipster/parser/dsl_parser/DSLExceptions.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     2010 2023-05-25 08:45:48.000000 thipster-0.12.3/thipster/parser/dsl_parser/DSLParser.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    13743 2023-05-25 08:45:48.000000 thipster-0.12.3/thipster/parser/dsl_parser/Interpreter.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    17503 2023-05-25 08:45:48.000000 thipster-0.12.3/thipster/parser/dsl_parser/Lexer.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4761 2023-05-25 08:45:48.000000 thipster-0.12.3/thipster/parser/dsl_parser/LexerPosition.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     2279 2023-05-25 08:45:48.000000 thipster-0.12.3/thipster/parser/dsl_parser/Token.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    19839 2023-05-25 08:45:48.000000 thipster-0.12.3/thipster/parser/dsl_parser/TokenParser.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-21 13:59:54.000000 thipster-0.12.3/thipster/parser/dsl_parser/__init__.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:34.002536 thipster-0.12.3/thipster/repository/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1152 2023-05-10 12:33:34.000000 thipster-0.12.3/thipster/repository/GithubRepo.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4646 2023-05-30 07:31:23.000000 thipster-0.12.3/thipster/repository/JSONRepo.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      360 2023-05-09 15:24:53.000000 thipster-0.12.3/thipster/repository/LocalRepo.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-20 08:57:48.000000 thipster-0.12.3/thipster/repository/__init__.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:34.002536 thipster-0.12.3/thipster/terraform/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    11986 2023-05-30 12:20:19.000000 thipster-0.12.3/thipster/terraform/CDK.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-18 12:21:13.000000 thipster-0.12.3/thipster/terraform/__init__.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:34.002536 thipster-0.12.3/thipster/thipster.egg-info/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1265 2023-05-30 13:56:10.000000 thipster-0.12.3/thipster/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        1 2023-05-30 13:56:10.000000 thipster-0.12.3/thipster/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)       44 2023-05-30 13:56:10.000000 thipster-0.12.3/thipster/thipster.egg-info/entry_points.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      205 2023-05-30 13:56:10.000000 thipster-0.12.3/thipster/thipster.egg-info/requires.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)       57 2023-05-30 13:56:10.000000 thipster-0.12.3/thipster/thipster.egg-info/top_level.txt
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-05-30 14:08:34.002536 thipster-0.12.3/thipster.egg-info/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      114 2023-05-30 14:08:33.000000 thipster-0.12.3/thipster.egg-info/PKG-INFO
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1817 2023-05-30 14:08:33.000000 thipster-0.12.3/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        1 2023-05-30 14:08:33.000000 thipster-0.12.3/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      205 2023-05-30 14:08:33.000000 thipster-0.12.3/thipster.egg-info/requires.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)       15 2023-05-30 14:08:33.000000 thipster-0.12.3/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:15.716524 thipster-0.13.0/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-30 13:46:13.000000 thipster-0.13.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-30 13:46:15.716524 thipster-0.13.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-05-30 13:46:13.000000 thipster-0.13.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      779 2023-05-30 13:46:13.000000 thipster-0.13.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      117 2023-05-30 13:46:13.000000 thipster-0.13.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 13:46:15.716524 thipster-0.13.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      639 2023-05-30 13:46:13.000000 thipster-0.13.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:15.712524 thipster-0.13.0/thipster/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:15.712524 thipster-0.13.0/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/auth/Google.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/auth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:15.712524 thipster-0.13.0/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/engine/Engine.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/engine/I_Auth.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/engine/I_Parser.py
+-rw-r--r--   0 root         (0) root         (0)      323 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/engine/I_Repository.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/engine/I_Terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/engine/ParsedFile.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/engine/ResourceModel.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:15.712524 thipster-0.13.0/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)     2306 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/parser/ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     6199 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/parser/YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:15.716524 thipster-0.13.0/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)    10332 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/parser/dsl_parser/AST.py
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/parser/dsl_parser/DSLExceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/parser/dsl_parser/DSLParser.py
+-rw-r--r--   0 root         (0) root         (0)    13743 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/parser/dsl_parser/Interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17503 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/parser/dsl_parser/Lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4761 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/parser/dsl_parser/LexerPosition.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/parser/dsl_parser/Token.py
+-rw-r--r--   0 root         (0) root         (0)    19839 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/parser/dsl_parser/TokenParser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/parser/dsl_parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:15.716524 thipster-0.13.0/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/repository/GithubRepo.py
+-rw-r--r--   0 root         (0) root         (0)     4646 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/repository/JSONRepo.py
+-rw-r--r--   0 root         (0) root         (0)      360 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/repository/LocalRepo.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/repository/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:15.716524 thipster-0.13.0/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)    11635 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/terraform/CDK.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 13:46:13.000000 thipster-0.13.0/thipster/terraform/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:15.716524 thipster-0.13.0/thipster/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-30 13:46:15.000000 thipster-0.13.0/thipster/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-05-30 13:46:15.000000 thipster-0.13.0/thipster/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 13:46:15.000000 thipster-0.13.0/thipster/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-30 13:46:15.000000 thipster-0.13.0/thipster/thipster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      205 2023-05-30 13:46:15.000000 thipster-0.13.0/thipster/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-30 13:46:15.000000 thipster-0.13.0/thipster/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.12.3/README.md` & `thipster-0.13.0/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/pyproject.toml` & `thipster-0.13.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 
 testpaths = [
     "tests",
     "integration",
```

### Comparing `thipster-0.12.3/setup.py` & `thipster-0.13.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from setuptools import setup, find_packages  
+from setuptools import setup
 
-__version__ = '0.12.3'
+__version__ = '0.13.0'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='thipster',
     version=__version__,
+    package_dir={'': 'thipster'},
     install_requires=required,
-    packages=find_packages(
-        exclude=['packages'],  
-    ),
     extras_require={
         'test': [
             'pytest',
             'pytest-mock',
         ],
         'dev': [
             'pytest',
@@ -23,8 +21,13 @@
             'dagger.io',
             'pre-commit',
         ],
         'doc': [
             'sphinx',
         ],
     },
+    entry_points={
+        'console_scripts': [
+            'thipster-demo = demo:demo',
+        ],
+    },
 )
```

### Comparing `thipster-0.12.3/thipster/engine/Engine.py` & `thipster-0.13.0/thipster/engine/Engine.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from engine.I_Repository import I_Repository
 from engine.I_Auth import I_Auth
 from engine.I_Terraform import I_Terraform
 import engine.ParsedFile as pf
 
 
 class Engine():
-    """Class representing the engine of thipster
+    """The engine of thipster
 
     The core of the application, it is used to call and link all
     interfaces together.
 
     Methods
     -------
     run(filename: str)
@@ -74,16 +74,14 @@
         print("Parsed:", end - start)
         start = time.time()
 
         # Get needed models
         types = [r.type for r in file.resources]
         models = self.__repository.get(types)
 
-        # self.__auth.run()
-
         # Generate Terraform files
-        dirs = self.__terraform.generate(file, models)
+        dirs = self.__terraform.generate(file, models, self.__auth)
 
         self.__terraform.init()
         print(self.__terraform.plan())
 
         return dirs
```

### Comparing `thipster-0.12.3/thipster/engine/I_Parser.py` & `thipster-0.13.0/thipster/engine/I_Parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/engine/I_Terraform.py` & `thipster-0.13.0/thipster/engine/I_Terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/engine/ParsedFile.py` & `thipster-0.13.0/thipster/engine/ParsedFile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/engine/ResourceModel.py` & `thipster-0.13.0/thipster/engine/ResourceModel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/parser/ParserFactory.py` & `thipster-0.13.0/thipster/parser/ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/parser/YAMLParser.py` & `thipster-0.13.0/thipster/parser/YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/parser/dsl_parser/AST.py` & `thipster-0.13.0/thipster/parser/dsl_parser/AST.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/parser/dsl_parser/DSLParser.py` & `thipster-0.13.0/thipster/parser/dsl_parser/DSLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/parser/dsl_parser/Interpreter.py` & `thipster-0.13.0/thipster/parser/dsl_parser/Interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/parser/dsl_parser/Lexer.py` & `thipster-0.13.0/thipster/parser/dsl_parser/Lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/parser/dsl_parser/LexerPosition.py` & `thipster-0.13.0/thipster/parser/dsl_parser/LexerPosition.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/parser/dsl_parser/Token.py` & `thipster-0.13.0/thipster/parser/dsl_parser/Token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/parser/dsl_parser/TokenParser.py` & `thipster-0.13.0/thipster/parser/dsl_parser/TokenParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/repository/GithubRepo.py` & `thipster-0.13.0/thipster/repository/GithubRepo.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/repository/JSONRepo.py` & `thipster-0.13.0/thipster/repository/JSONRepo.py`

 * *Files identical despite different names*

### Comparing `thipster-0.12.3/thipster/terraform/CDK.py` & `thipster-0.13.0/thipster/terraform/CDK.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import copy
 import shutil
 import subprocess
 import sys
 import os
 import importlib
 import uuid
+from engine.I_Auth import I_Auth
 
 from python_terraform import Terraform
 from constructs import Construct
 from cdktf import App, TerraformStack, TerraformOutput
 
 import engine.ResourceModel as rm
 import engine.ParsedFile as pf
-from cdktf_cdktf_provider_google.provider import GoogleProvider
 from engine.I_Terraform import I_Terraform
 from helpers import createLogger as Logger
 
 
 class CDKException(Exception):
     @property
     def message(self):
@@ -78,15 +78,18 @@
             If method is not implemented in inheriting classes
 
         """
         t = Terraform()
         _, stdout, stderr = t.apply()
         return stdout + stderr
 
-    def generate(self, file: pf.ParsedFile, models: dict[str, rm.ResourceModel]):
+    def generate(
+        self, file: pf.ParsedFile, models: dict[str, rm.ResourceModel],
+        _auth: I_Auth,
+    ):
 
         CDK._models = models
         # Init CDK
         app = App()
 
         f_position = file.resources[0].position
         file_name = f_position.fileName if f_position else 'thipster_infrastructure'
@@ -94,25 +97,15 @@
         CDK._logger.debug('Creating tf code for file %s', file_name)
 
         # Declare new stack in CDK
         class _ResourceStack(TerraformStack):
             def __init__(self, scope: Construct, ns: str):
                 super().__init__(scope, ns)
 
-                GoogleProvider(
-                    self, f"{file_name}_google",
-                    project="rcattin-sandbox",
-                    credentials=os.path.join(
-                        os.getcwd(),
-                        "rcattin-sandbox-credentials.json",
-                    ),
-
-                    region="europe-west1",
-                    zone="europe-west1-b",
-                )
+                _auth.authenticate(self)
 
                 for resource in file.resources:
                     res = CDK._create_resource_from_resource(
                         self,
                         resource=resource,
                     )
```

### Comparing `thipster-0.12.3/thipster/thipster.egg-info/SOURCES.txt` & `thipster-0.13.0/thipster/thipster.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
-tests/test_e2e.py
 thipster/__init__.py
 thipster/helpers.py
+thipster/auth/Google.py
 thipster/auth/__init__.py
 thipster/engine/Engine.py
 thipster/engine/I_Auth.py
 thipster/engine/I_Parser.py
 thipster/engine/I_Repository.py
 thipster/engine/I_Terraform.py
 thipster/engine/ParsedFile.py
```

