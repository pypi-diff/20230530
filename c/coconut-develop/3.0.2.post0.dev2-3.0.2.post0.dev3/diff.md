# Comparing `tmp/coconut-develop-3.0.2.post0.dev2.tar.gz` & `tmp/coconut-develop-3.0.2.post0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coconut-develop-3.0.2.post0.dev2.tar", last modified: Tue May 30 05:06:22 2023, max compression
+gzip compressed data, was "dist/coconut-develop-3.0.2.post0.dev3.tar", last modified: Tue May 30 07:15:08 2023, max compression
```

## Comparing `coconut-develop-3.0.2.post0.dev2.tar` & `coconut-develop-3.0.2.post0.dev3.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/
--rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/FAQ.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/_coconut/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/_coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     4759 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/_coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/_coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/xontrib/
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/xontrib/coconut.py
--rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/HELP.md
--rw-r--r--   0 runner    (1001) docker     (122)   197597 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/DOCS.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/__coconut__/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/__coconut__/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    42053 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/__coconut__/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/__coconut__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/highlighter.py
--rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/constants_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_35/
--rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_35/py35_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/
--rw-r--r--   0 runner    (1001) docker     (122)    46282 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/util.coco
--rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/tutorial.coco
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/main.coco
--rw-r--r--   0 runner    (1001) docker     (122)    63026 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/primary.coco
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/__init__.coco
--rw-r--r--   0 runner    (1001) docker     (122)     5205 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/specific.coco
--rw-r--r--   0 runner    (1001) docker     (122)    42163 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/suite.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_2/
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_2/py2_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_38/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_38/py38_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_sys/
--rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_36/
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_36/py36_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_3/
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_3/py3_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/non_strict/
--rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/runner.coco
--rw-r--r--   0 runner    (1001) docker     (122)    22242 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/extras.coco
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/src/runnable.coco
--rw-r--r--   0 runner    (1001) docker     (122)    30311 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/main_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/convenience.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/convenience.py
--rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/__coconut__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/api.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/root.py
--rw-r--r--   0 runner    (1001) docker     (122)    11623 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/__coconut__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/compiler/templates/
--rw-r--r--   0 runner    (1001) docker     (122)   101374 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/compiler/templates/header.py_template
--rw-r--r--   0 runner    (1001) docker     (122)    31929 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/compiler/header.py
--rw-r--r--   0 runner    (1001) docker     (122)    93077 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/compiler/grammar.py
--rw-r--r--   0 runner    (1001) docker     (122)    58872 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/compiler/matching.py
--rw-r--r--   0 runner    (1001) docker     (122)   196422 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    48882 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/compiler/util.py
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/icoconut/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/icoconut/coconut_py3/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/icoconut/coconut_py3/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)    10729 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/icoconut/root.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/icoconut/coconut_py/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/icoconut/coconut_py/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/icoconut/embed.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/icoconut/coconut_py2/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/icoconut/coconut_py2/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/icoconut/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-30 05:06:21.000000 coconut-develop-3.0.2.post0.dev2/coconut/icoconut/coconut/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/icoconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/icoconut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/command/
--rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/command/mypy.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/command/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut/command/resources/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/command/resources/zcoconut.pth
--rw-r--r--   0 runner    (1001) docker     (122)    44133 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/command/command.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/command/command.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     8255 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/command/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    23531 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/command/util.py
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/terminal.py
--rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    36559 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/_pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/integrations.py
--rw-r--r--   0 runner    (1001) docker     (122)    11530 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6936 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut_develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-30 05:06:22.000000 coconut-develop-3.0.2.post0.dev2/coconut_develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)    13803 2023-05-30 04:06:29.000000 coconut-develop-3.0.2.post0.dev2/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/FAQ.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/_coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/_coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     4759 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/_coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/_coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/xontrib/coconut.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/HELP.md
+-rw-r--r--   0 runner    (1001) docker     (122)   197597 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/DOCS.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/__coconut__/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/__coconut__/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    42053 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/__coconut__/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/__coconut__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/constants_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_35/
+-rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_35/py35_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)    46282 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/util.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/tutorial.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/main.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    63026 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/primary.coco
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/__init__.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     5205 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/specific.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    42163 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/suite.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_2/
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_2/py2_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_38/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_38/py38_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_sys/
+-rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_36/
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_36/py36_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_3/py3_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/non_strict/
+-rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/runner.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    22242 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/extras.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/src/runnable.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    30324 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/convenience.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/__coconut__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11623 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/__coconut__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/compiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)   100801 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/compiler/templates/header.py_template
+-rw-r--r--   0 runner    (1001) docker     (122)    33279 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/compiler/header.py
+-rw-r--r--   0 runner    (1001) docker     (122)    93077 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/compiler/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58872 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/compiler/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)   196422 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48882 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/compiler/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/icoconut/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/icoconut/coconut_py3/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/icoconut/coconut_py3/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10729 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/icoconut/root.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/icoconut/coconut_py/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/icoconut/coconut_py/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/icoconut/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/icoconut/coconut_py2/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/icoconut/coconut_py2/kernel.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/icoconut/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-30 07:15:06.000000 coconut-develop-3.0.2.post0.dev3/coconut/icoconut/coconut/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/icoconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/icoconut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/command/
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/command/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/command/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut/command/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/command/resources/zcoconut.pth
+-rw-r--r--   0 runner    (1001) docker     (122)    44133 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/command/command.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     8255 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/command/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23531 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/command/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36559 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/_pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11530 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut_develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-30 07:15:08.000000 coconut-develop-3.0.2.post0.dev3/coconut_develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)    13803 2023-05-30 06:21:58.000000 coconut-develop-3.0.2.post0.dev3/CONTRIBUTING.md
```

### Comparing `coconut-develop-3.0.2.post0.dev2/README.rst` & `coconut-develop-3.0.2.post0.dev3/README.rst`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/conf.py` & `coconut-develop-3.0.2.post0.dev3/conf.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/FAQ.md` & `coconut-develop-3.0.2.post0.dev3/FAQ.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/_coconut/__init__.pyi` & `coconut-develop-3.0.2.post0.dev3/_coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/_coconut/__init__.py` & `coconut-develop-3.0.2.post0.dev3/_coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/LICENSE.txt` & `coconut-develop-3.0.2.post0.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/setup.py` & `coconut-develop-3.0.2.post0.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/xontrib/coconut.py` & `coconut-develop-3.0.2.post0.dev3/xontrib/coconut.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/HELP.md` & `coconut-develop-3.0.2.post0.dev3/HELP.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/DOCS.md` & `coconut-develop-3.0.2.post0.dev3/DOCS.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/__coconut__/__init__.pyi` & `coconut-develop-3.0.2.post0.dev3/__coconut__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/__coconut__/__init__.py` & `coconut-develop-3.0.2.post0.dev3/__coconut__/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/highlighter.py` & `coconut-develop-3.0.2.post0.dev3/coconut/highlighter.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/api.py` & `coconut-develop-3.0.2.post0.dev3/coconut/api.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/constants_test.py` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/constants_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_35/py35_test.coco` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_35/py35_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/util.coco` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/util.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/tutorial.coco` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/tutorial.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/main.coco` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/main.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/primary.coco` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/primary.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/specific.coco` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/specific.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/agnostic/suite.coco` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/agnostic/suite.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_sys/target_sys_test.coco` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_sys/target_sys_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_36/py36_test.coco` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_36/py36_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/target_3/py3_test.coco` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/target_3/py3_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/src/cocotest/non_strict/non_strict_test.coco` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/src/cocotest/non_strict/non_strict_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/src/extras.coco` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/src/extras.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/main_test.py` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/main_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -797,15 +797,15 @@
         if not WINDOWS and not PYPY:
             def test_jupyter_console(self):
                 p = spawn_cmd("coconut --jupyter console")
                 p.expect("In", timeout=120)
                 p.sendline("%load_ext coconut")
                 p.expect("In", timeout=120)
                 p.sendline("`exit`")
-                p.expect("Shutting down kernel|shutting down")
+                p.expect("Shutting down kernel|shutting down", timeout=120)
                 if p.isalive():
                     p.terminate()
 
 
 @add_test_func_names
 class TestCompilation(unittest.TestCase):
```

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/__main__.py` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/tests/__init__.py` & `coconut-develop-3.0.2.post0.dev3/coconut/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/convenience.pyi` & `coconut-develop-3.0.2.post0.dev3/coconut/convenience.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/convenience.py` & `coconut-develop-3.0.2.post0.dev3/coconut/convenience.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/__coconut__.pyi` & `coconut-develop-3.0.2.post0.dev3/coconut/__coconut__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/api.pyi` & `coconut-develop-3.0.2.post0.dev3/coconut/api.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/root.py` & `coconut-develop-3.0.2.post0.dev3/coconut/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -----------------------------------------------------------------------------------------------------------------------
 # VERSION:
 # -----------------------------------------------------------------------------------------------------------------------
 
 VERSION = "3.0.2"
 VERSION_NAME = None
 # False for release, int >= 1 for develop
-DEVELOP = 2
+DEVELOP = 3
 ALPHA = False  # for pre releases rather than post releases
 
 assert DEVELOP is False or DEVELOP >= 1, "DEVELOP must be False or an int >= 1"
 assert DEVELOP or not ALPHA, "alpha releases are only for develop"
 
 # -----------------------------------------------------------------------------------------------------------------------
 # UTILITIES:
```

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/requirements.py` & `coconut-develop-3.0.2.post0.dev3/coconut/requirements.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/main.py` & `coconut-develop-3.0.2.post0.dev3/coconut/main.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/__coconut__.py` & `coconut-develop-3.0.2.post0.dev3/coconut/__coconut__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/compiler/templates/header.py_template` & `coconut-develop-3.0.2.post0.dev3/coconut/compiler/templates/header.py_template`

 * *Files 0% similar despite different names*

```diff
@@ -1484,35 +1484,16 @@
         Equivalent to multiset[item], but additionally verifies the count is non-negative."""
         result = self[item]
         if result < 0:
             raise _coconut.ValueError("multiset has negative count for " + _coconut.repr(item))
         return result
     def __fmap__(self, func):
         return self.__class__(_coconut.dict((func(obj), num) for obj, num in self.items()))
-    def __add__(self, other):
-        out = self.copy()
-        out += other
-        return out
-    def __and__(self, other):
-        out = self.copy()
-        out &= other
-        return out
-    def __or__(self, other):
-        out = self.copy()
-        out |= other
-        return out
-    def __sub__(self, other):
-        out = self.copy()
-        out -= other
-        return out
-    def __neg__(self):
-        return self.__class__(_coconut.super({_coconut_}multiset, self).__neg__())
-    def __pos__(self):
-        return self.__class__(_coconut.super({_coconut_}multiset, self).__pos__())
-{def_total_and_comparisons}{assign_multiset_views}_coconut.abc.MutableSet.register(multiset)
+{def_multiset_ops}
+{def_total_and_comparisons}{def_py2_multiset_methods}_coconut.abc.MutableSet.register(multiset)
 def _coconut_base_makedata(data_type, args, from_fmap=False, fallback_to_init=False):
     if _coconut.hasattr(data_type, "_make") and _coconut.issubclass(data_type, _coconut.tuple):
         return data_type._make(args)
     if _coconut.issubclass(data_type, (_coconut.range, _coconut.abc.Iterator)):
         return args
     if _coconut.issubclass(data_type, _coconut.str):
         return "".join(args)
```

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/compiler/header.py` & `coconut-develop-3.0.2.post0.dev3/coconut/compiler/header.py`

 * *Files 3% similar despite different names*

```diff
@@ -472,17 +472,19 @@
             return False
         found_diff = found_diff or self[k] != v
     return found_diff
             ''',
             indent=1,
             newline=True,
         ),
-        assign_multiset_views=pycondition(
+        def_py2_multiset_methods=pycondition(
             (3,),
             if_lt='''
+def __bool__(self):
+    return _coconut.bool(_coconut.len(self))
 keys = _coconut.collections.Counter.viewkeys
 values = _coconut.collections.Counter.viewvalues
 items = _coconut.collections.Counter.viewitems
             ''',
             indent=1,
             newline=True,
         ),
@@ -672,14 +674,54 @@
         __slots__ = ()
     functools.lru_cache = you_need_to_install_backports_functools_lru_cache()
             '''.format(**format_dict),
             if_ge=None,
             indent=1,
             newline=True,
         ),
+        def_multiset_ops=pycondition(
+            (3,),
+            if_ge='''
+def __add__(self, other):
+    out = self.copy()
+    out += other
+    return out
+def __and__(self, other):
+    out = self.copy()
+    out &= other
+    return out
+def __or__(self, other):
+    out = self.copy()
+    out |= other
+    return out
+def __sub__(self, other):
+    out = self.copy()
+    out -= other
+    return out
+def __pos__(self):
+    return self.__class__(_coconut.super({_coconut_}multiset, self).__pos__())
+def __neg__(self):
+    return self.__class__(_coconut.super({_coconut_}multiset, self).__neg__())
+            '''.format(**format_dict),
+            if_lt='''
+def __add__(self, other):
+    return self.__class__(_coconut.super({_coconut_}multiset, self).__add__(other))
+def __and__(self, other):
+    return self.__class__(_coconut.super({_coconut_}multiset, self).__and__(other))
+def __or__(self, other):
+    return self.__class__(_coconut.super({_coconut_}multiset, self).__or__(other))
+def __sub__(self, other):
+    return self.__class__(_coconut.super({_coconut_}multiset, self).__sub__(other))
+def __pos__(self):
+    return self + {_coconut_}multiset()
+def __neg__(self):
+    return {_coconut_}multiset() - self
+            '''.format(**format_dict),
+            indent=1,
+        ),
     )
     format_dict.update(extra_format_dict)
 
     return format_dict
 
 
 # -----------------------------------------------------------------------------------------------------------------------
```

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/compiler/grammar.py` & `coconut-develop-3.0.2.post0.dev3/coconut/compiler/grammar.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/compiler/matching.py` & `coconut-develop-3.0.2.post0.dev3/coconut/compiler/matching.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/compiler/compiler.py` & `coconut-develop-3.0.2.post0.dev3/coconut/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/compiler/util.py` & `coconut-develop-3.0.2.post0.dev3/coconut/compiler/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/compiler/__init__.py` & `coconut-develop-3.0.2.post0.dev3/coconut/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/icoconut/root.py` & `coconut-develop-3.0.2.post0.dev3/coconut/icoconut/root.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/icoconut/embed.py` & `coconut-develop-3.0.2.post0.dev3/coconut/icoconut/embed.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/icoconut/__main__.py` & `coconut-develop-3.0.2.post0.dev3/coconut/icoconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/icoconut/__init__.py` & `coconut-develop-3.0.2.post0.dev3/coconut/icoconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/command/mypy.py` & `coconut-develop-3.0.2.post0.dev3/coconut/command/mypy.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/command/watch.py` & `coconut-develop-3.0.2.post0.dev3/coconut/command/watch.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/command/command.py` & `coconut-develop-3.0.2.post0.dev3/coconut/command/command.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/command/command.pyi` & `coconut-develop-3.0.2.post0.dev3/coconut/command/command.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/command/cli.py` & `coconut-develop-3.0.2.post0.dev3/coconut/command/cli.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/command/util.py` & `coconut-develop-3.0.2.post0.dev3/coconut/command/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/command/__init__.py` & `coconut-develop-3.0.2.post0.dev3/coconut/command/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/__init__.pyi` & `coconut-develop-3.0.2.post0.dev3/coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/terminal.py` & `coconut-develop-3.0.2.post0.dev3/coconut/terminal.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/exceptions.py` & `coconut-develop-3.0.2.post0.dev3/coconut/exceptions.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/constants.py` & `coconut-develop-3.0.2.post0.dev3/coconut/constants.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/_pyparsing.py` & `coconut-develop-3.0.2.post0.dev3/coconut/_pyparsing.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/integrations.py` & `coconut-develop-3.0.2.post0.dev3/coconut/integrations.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/util.py` & `coconut-develop-3.0.2.post0.dev3/coconut/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/__main__.py` & `coconut-develop-3.0.2.post0.dev3/coconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut/__init__.py` & `coconut-develop-3.0.2.post0.dev3/coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/PKG-INFO` & `coconut-develop-3.0.2.post0.dev3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,98 @@
 Metadata-Version: 2.1
 Name: coconut-develop
-Version: 3.0.2.post0.dev2
+Version: 3.0.2.post0.dev3
 Summary: Simple, elegant, Pythonic functional programming.
 Home-page: http://coconut-lang.org
 Author: Evan Hubinger
 Author-email: evanjhub@gmail.com
 License: Apache 2.0
+Description: |logo| Coconut
+        ==============
+        
+        ..
+            <insert toctree here>
+        
+        .. |logo| image:: https://github.com/evhub/coconut/raw/gh-pages/favicon-32x32.png
+        
+        .. image:: https://opencollective.com/coconut/backers/badge.svg
+            :alt: Backers on Open Collective
+            :target: #backers
+        .. image:: https://opencollective.com/coconut/sponsors/badge.svg
+            :alt: Sponsors on Open Collective
+            :target: #sponsors
+        .. image:: https://badges.gitter.im/evhub/coconut.svg
+            :alt: Join the chat at https://gitter.im/evhub/coconut
+            :target: https://gitter.im/evhub/coconut?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+        
+        Coconut (`coconut-lang.org`__) is a variant of Python_ that **adds on top of Python syntax** new features for simple, elegant, Pythonic **functional programming**.
+        
+        __ Coconut_
+        .. _Coconut: http://coconut-lang.org/
+        
+        Coconut is developed on GitHub_ and hosted on PyPI_. Installing Coconut is as easy as opening a command prompt and entering::
+        
+            pip install coconut
+        
+        To help you get started, check out these links for more information about Coconut:
+        
+        - Tutorial_: If you're new to Coconut, a good place to start is Coconut's **tutorial**.
+        - Documentation_: If you're looking for info about a specific feature, check out Coconut's **documentation**.
+        - `Online Interpreter`_: If you want to try Coconut in your browser, check out Coconut's **online interpreter**.
+        - FAQ_: If you have general questions about Coconut—like who Coconut is built for and whether or not you should use it—Coconut's frequently asked questions are often the best place to start.
+        - `Create a New Issue <https://github.com/evhub/coconut/issues/new>`_: If you're having a problem with Coconut, creating a new issue detailing the problem will allow it to be addressed as soon as possible.
+        - Gitter_: For any questions, concerns, or comments about anything Coconut-related, ask around at Coconut's Gitter, a GitHub-integrated chat room for Coconut developers.
+        - Releases_: Want to know what's been added in recent Coconut versions? Check out the release log for all the new features and fixes.
+        
+        .. _Python: https://www.python.org/
+        .. _PyPI: https://pypi.python.org/pypi/coconut
+        .. _Tutorial: http://coconut.readthedocs.io/en/latest/HELP.html
+        .. _Documentation: http://coconut.readthedocs.io/en/latest/DOCS.html
+        .. _`Online Interpreter`: https://cs121-team-panda.github.io/coconut-interpreter
+        .. _FAQ: http://coconut.readthedocs.io/en/latest/FAQ.html
+        .. _GitHub: https://github.com/evhub/coconut
+        .. _Gitter: https://gitter.im/evhub/coconut
+        .. _Releases: https://github.com/evhub/coconut/releases
+        
+        Credits
+        +++++++
+        
+        Contributors
+        ------------
+        
+        This project exists thanks to all the people who contribute! `Become a contributor`__.
+        
+        .. image:: https://opencollective.com/coconut/contributors.svg?width=890&button=false
+            :target: https://github.com/evhub/coconut/graphs/contributors
+        
+        __ Contributor_
+        .. _Contributor: http://coconut.readthedocs.io/en/develop/CONTRIBUTING.html
+        
+        Backers
+        -------
+        
+        Thank you to all our backers! `Become a backer`__.
+        
+        .. image:: https://opencollective.com/coconut/backers.svg?width=890
+            :target: https://opencollective.com/coconut#backers
+        
+        __ Backer_
+        .. _Backer: https://opencollective.com/coconut#backer
+        
+        Sponsors
+        --------
+        
+        Support Coconut by becoming a sponsor. Your logo will show up here with a link to your website. `Become a sponsor`__.
+        
+        .. image:: https://opencollective.com/XX/sponsor/0/avatar.svg
+            :target: https://opencollective.com/coconut/sponsor/0/website
+        
+        __ Sponsor_
+        .. _Sponsor: https://opencollective.com/coconut#sponsor
+        
 Keywords: functional,programming,language,compiler,pattern,pattern-matching,algebraic,data type,data types,lambda,lambdas,lazy,evaluation,lazy list,lazy lists,tail,recursion,call,recursive,infix,function,composition,compose,partial,application,currying,curry,pipeline,pipe,unicode,operator,operators,frozenset,literal,syntax,destructuring,assignment,fold,datamaker,prepattern,iterator,none,coalesce,coalescing,statement,lru_cache,memoization,backport,typing,embed,PEP 622,overrides,islice,itertools,functools,TYPE_CHECKING,Expected,breakpoint,help,reduce,takewhile,dropwhile,tee,count,makedata,consume,parallel_map,addpattern,recursive_iterator,concurrent_map,fmap,starmap,reiterable,scan,groupsof,memoize,zip_longest,override,flatten,ident,call,safe_call,flip,const,lift,all_equal,collectby,multi_enumerate,cartesian_product,multiset,cycle,windowsof,py_chr,py_dict,py_hex,py_input,py_int,py_map,py_object,py_oct,py_open,py_print,py_range,py_str,py_super,py_zip,py_filter,py_reversed,py_enumerate,py_raw_input,py_xrange,py_repr,py_breakpoint,_namedtuple_of,reveal_type,reveal_locals,MatchError,__fmap__,__iter_getitem__,data,match,case,cases,where,addpattern,then,operator,type,copyclosure,λ
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
@@ -48,93 +131,7 @@
 Provides-Extra: xonsh
 Provides-Extra: jupyter
 Provides-Extra: all
 Provides-Extra: ipython
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: dev
-License-File: LICENSE.txt
-
-|logo| Coconut
-==============
-
-..
-    <insert toctree here>
-
-.. |logo| image:: https://github.com/evhub/coconut/raw/gh-pages/favicon-32x32.png
-
-.. image:: https://opencollective.com/coconut/backers/badge.svg
-    :alt: Backers on Open Collective
-    :target: #backers
-.. image:: https://opencollective.com/coconut/sponsors/badge.svg
-    :alt: Sponsors on Open Collective
-    :target: #sponsors
-.. image:: https://badges.gitter.im/evhub/coconut.svg
-    :alt: Join the chat at https://gitter.im/evhub/coconut
-    :target: https://gitter.im/evhub/coconut?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-
-Coconut (`coconut-lang.org`__) is a variant of Python_ that **adds on top of Python syntax** new features for simple, elegant, Pythonic **functional programming**.
-
-__ Coconut_
-.. _Coconut: http://coconut-lang.org/
-
-Coconut is developed on GitHub_ and hosted on PyPI_. Installing Coconut is as easy as opening a command prompt and entering::
-
-    pip install coconut
-
-To help you get started, check out these links for more information about Coconut:
-
-- Tutorial_: If you're new to Coconut, a good place to start is Coconut's **tutorial**.
-- Documentation_: If you're looking for info about a specific feature, check out Coconut's **documentation**.
-- `Online Interpreter`_: If you want to try Coconut in your browser, check out Coconut's **online interpreter**.
-- FAQ_: If you have general questions about Coconut—like who Coconut is built for and whether or not you should use it—Coconut's frequently asked questions are often the best place to start.
-- `Create a New Issue <https://github.com/evhub/coconut/issues/new>`_: If you're having a problem with Coconut, creating a new issue detailing the problem will allow it to be addressed as soon as possible.
-- Gitter_: For any questions, concerns, or comments about anything Coconut-related, ask around at Coconut's Gitter, a GitHub-integrated chat room for Coconut developers.
-- Releases_: Want to know what's been added in recent Coconut versions? Check out the release log for all the new features and fixes.
-
-.. _Python: https://www.python.org/
-.. _PyPI: https://pypi.python.org/pypi/coconut
-.. _Tutorial: http://coconut.readthedocs.io/en/latest/HELP.html
-.. _Documentation: http://coconut.readthedocs.io/en/latest/DOCS.html
-.. _`Online Interpreter`: https://cs121-team-panda.github.io/coconut-interpreter
-.. _FAQ: http://coconut.readthedocs.io/en/latest/FAQ.html
-.. _GitHub: https://github.com/evhub/coconut
-.. _Gitter: https://gitter.im/evhub/coconut
-.. _Releases: https://github.com/evhub/coconut/releases
-
-Credits
-+++++++
-
-Contributors
-------------
-
-This project exists thanks to all the people who contribute! `Become a contributor`__.
-
-.. image:: https://opencollective.com/coconut/contributors.svg?width=890&button=false
-    :target: https://github.com/evhub/coconut/graphs/contributors
-
-__ Contributor_
-.. _Contributor: http://coconut.readthedocs.io/en/develop/CONTRIBUTING.html
-
-Backers
--------
-
-Thank you to all our backers! `Become a backer`__.
-
-.. image:: https://opencollective.com/coconut/backers.svg?width=890
-    :target: https://opencollective.com/coconut#backers
-
-__ Backer_
-.. _Backer: https://opencollective.com/coconut#backer
-
-Sponsors
---------
-
-Support Coconut by becoming a sponsor. Your logo will show up here with a link to your website. `Become a sponsor`__.
-
-.. image:: https://opencollective.com/XX/sponsor/0/avatar.svg
-    :target: https://opencollective.com/coconut/sponsor/0/website
-
-__ Sponsor_
-.. _Sponsor: https://opencollective.com/coconut#sponsor
-
-
```

### Comparing `coconut-develop-3.0.2.post0.dev2/coconut_develop.egg-info/SOURCES.txt` & `coconut-develop-3.0.2.post0.dev3/coconut_develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev2/CONTRIBUTING.md` & `coconut-develop-3.0.2.post0.dev3/CONTRIBUTING.md`

 * *Files identical despite different names*

