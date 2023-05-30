# Comparing `tmp/thipster-0.13.1.tar.gz` & `tmp/thipster-0.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.13.1.tar", last modified: Tue May 30 14:54:10 2023, max compression
+gzip compressed data, was "thipster-0.13.2.tar", last modified: Tue May 30 15:43:47 2023, max compression
```

## Comparing `thipster-0.13.1.tar` & `thipster-0.13.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:10.551723 thipster-0.13.1/
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-30 14:54:07.000000 thipster-0.13.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-30 14:54:10.551723 thipster-0.13.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2697 2023-05-30 14:54:07.000000 thipster-0.13.1/README.md
--rw-r--r--   0 root         (0) root         (0)      868 2023-05-30 14:54:07.000000 thipster-0.13.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      117 2023-05-30 14:54:07.000000 thipster-0.13.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 14:54:10.551723 thipster-0.13.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-30 14:54:08.000000 thipster-0.13.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:10.547723 thipster-0.13.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:10.547723 thipster-0.13.1/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3218 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:10.547723 thipster-0.13.1/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:10.547723 thipster-0.13.1/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15546 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13247 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      861 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4154 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4682 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     4008 2023-05-30 14:54:07.000000 thipster-0.13.1/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:10.547723 thipster-0.13.1/thipster/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:10.551723 thipster-0.13.1/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)     1239 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/auth/Google.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/auth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:10.551723 thipster-0.13.1/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)     2273 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/engine/Engine.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/engine/I_Auth.py
--rw-r--r--   0 root         (0) root         (0)      668 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/engine/I_Parser.py
--rw-r--r--   0 root         (0) root         (0)      332 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/engine/I_Repository.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/engine/I_Terraform.py
--rw-r--r--   0 root         (0) root         (0)     6123 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/engine/ParsedFile.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/engine/ResourceModel.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:10.551723 thipster-0.13.1/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)     2342 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/parser/ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     6169 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/parser/YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:10.551723 thipster-0.13.1/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)    10350 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/parser/dsl_parser/AST.py
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/parser/dsl_parser/DSLExceptions.py
--rw-r--r--   0 root         (0) root         (0)     2064 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/parser/dsl_parser/DSLParser.py
--rw-r--r--   0 root         (0) root         (0)    13788 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/parser/dsl_parser/Interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17548 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/parser/dsl_parser/Lexer.py
--rw-r--r--   0 root         (0) root         (0)     4770 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/parser/dsl_parser/LexerPosition.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/parser/dsl_parser/Token.py
--rw-r--r--   0 root         (0) root         (0)    19857 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/parser/dsl_parser/TokenParser.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/parser/dsl_parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:10.551723 thipster-0.13.1/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/repository/GithubRepo.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/repository/JSONRepo.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/repository/LocalRepo.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/repository/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:10.551723 thipster-0.13.1/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)    11680 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/terraform/CDK.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:54:07.000000 thipster-0.13.1/thipster/terraform/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:10.547723 thipster-0.13.1/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-30 14:54:10.000000 thipster-0.13.1/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1629 2023-05-30 14:54:10.000000 thipster-0.13.1/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 14:54:10.000000 thipster-0.13.1/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      205 2023-05-30 14:54:10.000000 thipster-0.13.1/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-30 14:54:10.000000 thipster-0.13.1/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.025070 thipster-0.13.2/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-30 15:43:43.000000 thipster-0.13.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-05-30 15:43:47.025070 thipster-0.13.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-05-30 15:43:43.000000 thipster-0.13.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      867 2023-05-30 15:43:43.000000 thipster-0.13.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      117 2023-05-30 15:43:43.000000 thipster-0.13.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 15:43:47.025070 thipster-0.13.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-05-30 15:43:44.000000 thipster-0.13.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.013070 thipster-0.13.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.013070 thipster-0.13.2/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3218 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/engine/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.013070 thipster-0.13.2/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.013070 thipster-0.13.2/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15546 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13247 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      861 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4154 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4682 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     4008 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/test_e2e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.017070 thipster-0.13.2/thipster/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.017070 thipster-0.13.2/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/auth/Google.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/auth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.021070 thipster-0.13.2/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/Engine.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/I_Auth.py
+-rw-r--r--   0 root         (0) root         (0)      668 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/I_Parser.py
+-rw-r--r--   0 root         (0) root         (0)      332 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/I_Repository.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/I_Terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/ParsedFile.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/ResourceModel.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.021070 thipster-0.13.2/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     6169 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.021070 thipster-0.13.2/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)    10350 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/AST.py
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/DSLExceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/DSLParser.py
+-rw-r--r--   0 root         (0) root         (0)    13788 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/Interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17548 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/Lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4770 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/LexerPosition.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/Token.py
+-rw-r--r--   0 root         (0) root         (0)    19857 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/TokenParser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.025070 thipster-0.13.2/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/repository/GithubRepo.py
+-rw-r--r--   0 root         (0) root         (0)     4664 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/repository/JSONRepo.py
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/repository/LocalRepo.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/repository/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.025070 thipster-0.13.2/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)    11680 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/terraform/CDK.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/terraform/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.017070 thipster-0.13.2/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-05-30 15:43:46.000000 thipster-0.13.2/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-05-30 15:43:47.000000 thipster-0.13.2/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 15:43:46.000000 thipster-0.13.2/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      205 2023-05-30 15:43:46.000000 thipster-0.13.2/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-30 15:43:46.000000 thipster-0.13.2/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.13.1/README.md` & `thipster-0.13.2/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/pyproject.toml` & `thipster-0.13.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
-
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 
 testpaths = [
     "tests",
     "integration",
```

### Comparing `thipster-0.13.1/tests/engine/test_engine.py` & `thipster-0.13.2/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.13.2/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/tests/parser/dsl_parser/test_ast.py` & `thipster-0.13.2/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.13.2/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/tests/parser/dsl_parser/test_token.py` & `thipster-0.13.2/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.13.2/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/tests/parser/test_ParserFactory.py` & `thipster-0.13.2/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/tests/parser/test_YAMLParser.py` & `thipster-0.13.2/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/tests/parser/test_parsedfile.py` & `thipster-0.13.2/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/tests/test_e2e.py` & `thipster-0.13.2/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/auth/Google.py` & `thipster-0.13.2/thipster/auth/Google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/engine/Engine.py` & `thipster-0.13.2/thipster/engine/Engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/engine/I_Parser.py` & `thipster-0.13.2/thipster/engine/I_Parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/engine/I_Terraform.py` & `thipster-0.13.2/thipster/engine/I_Terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/engine/ParsedFile.py` & `thipster-0.13.2/thipster/engine/ParsedFile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/engine/ResourceModel.py` & `thipster-0.13.2/thipster/engine/ResourceModel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/parser/ParserFactory.py` & `thipster-0.13.2/thipster/parser/ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/parser/YAMLParser.py` & `thipster-0.13.2/thipster/parser/YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/parser/dsl_parser/AST.py` & `thipster-0.13.2/thipster/parser/dsl_parser/AST.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/parser/dsl_parser/DSLParser.py` & `thipster-0.13.2/thipster/parser/dsl_parser/DSLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/parser/dsl_parser/Interpreter.py` & `thipster-0.13.2/thipster/parser/dsl_parser/Interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/parser/dsl_parser/Lexer.py` & `thipster-0.13.2/thipster/parser/dsl_parser/Lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/parser/dsl_parser/LexerPosition.py` & `thipster-0.13.2/thipster/parser/dsl_parser/LexerPosition.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/parser/dsl_parser/Token.py` & `thipster-0.13.2/thipster/parser/dsl_parser/Token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/parser/dsl_parser/TokenParser.py` & `thipster-0.13.2/thipster/parser/dsl_parser/TokenParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/repository/GithubRepo.py` & `thipster-0.13.2/thipster/repository/GithubRepo.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/repository/JSONRepo.py` & `thipster-0.13.2/thipster/repository/JSONRepo.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster/terraform/CDK.py` & `thipster-0.13.2/thipster/terraform/CDK.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.1/thipster.egg-info/SOURCES.txt` & `thipster-0.13.2/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

