# Comparing `tmp/aws-codeartifact-poetry-1.2.0.tar.gz` & `tmp/aws_codeartifact_poetry-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-codeartifact-poetry-1.2.0.tar", max compression
+gzip compressed data, was "aws_codeartifact_poetry-1.3.0.tar", max compression
```

## Comparing `aws-codeartifact-poetry-1.2.0.tar` & `aws_codeartifact_poetry-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-02-13 10:32:22.120100 aws-codeartifact-poetry-1.2.0/LICENSE
--rw-r--r--   0        0        0     2431 2023-02-13 10:32:22.120100 aws-codeartifact-poetry-1.2.0/README.md
--rw-r--r--   0        0        0       35 2023-02-13 10:32:22.120100 aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/__init__.py
--rw-r--r--   0        0        0       53 2023-02-13 10:32:22.120100 aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/aws/__init__.py
--rw-r--r--   0        0        0     1264 2023-02-13 10:32:22.120100 aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/aws/session.py
--rw-r--r--   0        0        0     1138 2023-02-13 10:32:22.120100 aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/cli.py
--rw-r--r--   0        0        0       51 2023-02-13 10:32:22.120100 aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/commands/__init__.py
--rw-r--r--   0        0        0     1994 2023-02-13 10:32:22.120100 aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/commands/login.py
--rw-r--r--   0        0        0       45 2023-02-13 10:32:22.120100 aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/helpers/__init__.py
--rw-r--r--   0        0        0     1087 2023-02-13 10:32:22.124100 aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/helpers/catch_exceptions.py
--rw-r--r--   0        0        0     3691 2023-02-13 10:32:22.124100 aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/helpers/cmd.py
--rw-r--r--   0        0        0     2056 2023-02-13 10:32:22.124100 aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/helpers/logging.py
--rw-r--r--   0        0        0     4244 2023-02-13 10:32:22.124100 aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/helpers/poetry.py
--rw-r--r--   0        0        0     1703 2023-02-13 10:32:22.124100 aws-codeartifact-poetry-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 aws-codeartifact-poetry-1.2.0/setup.py
--rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 aws-codeartifact-poetry-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2431 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/README.md
+-rw-r--r--   0        0        0       35 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/__init__.py
+-rw-r--r--   0        0        0       53 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/aws/__init__.py
+-rw-r--r--   0        0        0     1264 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/aws/session.py
+-rw-r--r--   0        0        0     1138 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/cli.py
+-rw-r--r--   0        0        0       51 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/commands/__init__.py
+-rw-r--r--   0        0        0     1994 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/commands/login.py
+-rw-r--r--   0        0        0       45 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/helpers/__init__.py
+-rw-r--r--   0        0        0     1087 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/helpers/catch_exceptions.py
+-rw-r--r--   0        0        0     3691 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/helpers/cmd.py
+-rw-r--r--   0        0        0     2056 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/helpers/logging.py
+-rw-r--r--   0        0        0     4244 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/helpers/poetry.py
+-rw-r--r--   0        0        0     1702 2023-05-30 13:41:14.547405 aws_codeartifact_poetry-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 aws_codeartifact_poetry-1.3.0/PKG-INFO
```

### Comparing `aws-codeartifact-poetry-1.2.0/LICENSE` & `aws_codeartifact_poetry-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-codeartifact-poetry-1.2.0/README.md` & `aws_codeartifact_poetry-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/aws/session.py` & `aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/aws/session.py`

 * *Files identical despite different names*

### Comparing `aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/cli.py` & `aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/cli.py`

 * *Files identical despite different names*

### Comparing `aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/commands/login.py` & `aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/commands/login.py`

 * *Files identical despite different names*

### Comparing `aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/helpers/catch_exceptions.py` & `aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/helpers/catch_exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/helpers/cmd.py` & `aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/helpers/cmd.py`

 * *Files identical despite different names*

### Comparing `aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/helpers/logging.py` & `aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `aws-codeartifact-poetry-1.2.0/aws_codeartifact_poetry/helpers/poetry.py` & `aws_codeartifact_poetry-1.3.0/aws_codeartifact_poetry/helpers/poetry.py`

 * *Files identical despite different names*

### Comparing `aws-codeartifact-poetry-1.2.0/pyproject.toml` & `aws_codeartifact_poetry-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-codeartifact-poetry"
-version = "1.2.0"
+version = "1.3.0"
 description = "AWS CodeArtifact Poetry CLI"
 license = "Proprietary"
 authors = [ "Lucas Vieira <lucas.vieira94@outlook.com>" ]
 maintainers = [ "Lucas Vieira <lucas.vieira94@outlook.com>" ]
 readme = "README.md"
 repository = "https://github.com/lucasvieirasilva/aws-codeartifact-poetry"
 
@@ -12,15 +12,15 @@
   include = "aws_codeartifact_poetry"
 
   [tool.poetry.scripts]
   aws-codeartifact-poetry = "aws_codeartifact_poetry.cli:cli"
 
   [tool.poetry.dependencies]
   python = ">=3.8,<3.12"
-  boto3 = "1.20.5"
+  boto3 = "^1.20"
   click = "^8.0.3"
   toml = "^0.10.2"
 
   [tool.poetry.dev-dependencies]
   flake8 = "4.0.1"
   flake8-isort = "4.1.1"
   flake8-print = "4.0.0"
```

### Comparing `aws-codeartifact-poetry-1.2.0/PKG-INFO` & `aws_codeartifact_poetry-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: aws-codeartifact-poetry
-Version: 1.2.0
+Version: 1.3.0
 Summary: AWS CodeArtifact Poetry CLI
 Home-page: https://github.com/lucasvieirasilva/aws-codeartifact-poetry
 License: Proprietary
 Author: Lucas Vieira
 Author-email: lucas.vieira94@outlook.com
 Maintainer: Lucas Vieira
 Maintainer-email: lucas.vieira94@outlook.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: boto3 (==1.20.5)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: boto3 (>=1.20,<2.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/lucasvieirasilva/aws-codeartifact-poetry
 Description-Content-Type: text/markdown
 
 # AWS CodeArtifact Poetry
```

