# Comparing `tmp/i18ndude-6.0.0.tar.gz` & `tmp/i18ndude-6.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i18ndude-6.0.0.tar", last modified: Tue May 30 14:37:40 2023, max compression
+gzip compressed data, was "i18ndude-6.0.0a1.tar", last modified: Mon May  8 20:57:57 2023, max compression
```

## Comparing `i18ndude-6.0.0.tar` & `i18ndude-6.0.0a1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 14:37:40.761724 i18ndude-6.0.0/
--rw-r--r--   0 maurits    (501) staff       (20)    14445 2023-05-30 14:37:40.000000 i18ndude-6.0.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)      136 2023-05-30 14:37:40.000000 i18ndude-6.0.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    27662 2023-05-30 14:37:40.761855 i18ndude-6.0.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1889 2023-05-30 14:37:40.000000 i18ndude-6.0.0/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 14:37:40.748355 i18ndude-6.0.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)      825 2023-05-30 14:37:40.000000 i18ndude-6.0.0/docs/COPYRIGHT
--rw-r--r--   0 maurits    (501) staff       (20)    15880 2023-05-30 14:37:40.000000 i18ndude-6.0.0/docs/ChangeLog
--rw-r--r--   0 maurits    (501) staff       (20)    12296 2023-05-30 14:37:40.000000 i18ndude-6.0.0/docs/LICENSE
--rw-r--r--   0 maurits    (501) staff       (20)      439 2023-05-30 14:37:40.000000 i18ndude-6.0.0/docs/TODO.txt
--rw-r--r--   0 maurits    (501) staff       (20)    10185 2023-05-30 14:37:40.000000 i18ndude-6.0.0/docs/command.rst
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-05-30 14:37:40.000000 i18ndude-6.0.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      293 2023-05-30 14:37:40.762297 i18ndude-6.0.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2120 2023-05-30 14:37:40.000000 i18ndude-6.0.0/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 14:37:40.744107 i18ndude-6.0.0/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 14:37:40.752349 i18ndude-6.0.0/src/i18ndude/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    32873 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)     3805 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/common.py
--rw-r--r--   0 maurits    (501) staff       (20)    20834 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/extract.py
--rw-r--r--   0 maurits    (501) staff       (20)    10947 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/generator.py
--rw-r--r--   0 maurits    (501) staff       (20)     2985 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/gsextract.py
--rw-r--r--   0 maurits    (501) staff       (20)     1831 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    22287 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/pygettext.py
--rwxr-xr-x   0 maurits    (501) staff       (20)    28016 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/script.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 14:37:40.744512 i18ndude-6.0.0/src/i18ndude/testdata/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 14:37:40.759121 i18ndude-6.0.0/src/i18ndude/testdata/input/
--rw-r--r--   0 maurits    (501) staff       (20)      522 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/chameleon.pt
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/empty-en.po
--rw-r--r--   0 maurits    (501) staff       (20)      778 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/synctest-de.po
--rw-r--r--   0 maurits    (501) staff       (20)      820 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/synctest.pot
--rw-r--r--   0 maurits    (501) staff       (20)     2361 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/test-en.po
--rw-r--r--   0 maurits    (501) staff       (20)     1375 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/test.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1917 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/test.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2779 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/test1.pt
--rw-r--r--   0 maurits    (501) staff       (20)      916 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/test2-en.po
--rw-r--r--   0 maurits    (501) staff       (20)      392 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/test2.py
--rw-r--r--   0 maurits    (501) staff       (20)      893 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/test2_expected-en.po
--rw-r--r--   0 maurits    (501) staff       (20)      728 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/test3.pt
--rw-r--r--   0 maurits    (501) staff       (20)      510 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/test4.pt
--rw-r--r--   0 maurits    (501) staff       (20)      882 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/input/test5.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 14:37:40.759402 i18ndude-6.0.0/src/i18ndude/testdata/output/
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/testdata/output/README.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 14:37:40.761527 i18ndude-6.0.0/src/i18ndude/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    34684 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/tests/test_catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)      252 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/tests/test_extract.py
--rw-r--r--   0 maurits    (501) staff       (20)     7921 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/tests/test_untranslated.py
--rw-r--r--   0 maurits    (501) staff       (20)     5558 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/tests/test_utils.py
--rwxr-xr-x   0 maurits    (501) staff       (20)     1524 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/tests/tox-check-i18ndude-command.sh
--rw-r--r--   0 maurits    (501) staff       (20)      829 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/tests/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     9723 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/untranslated.py
--rw-r--r--   0 maurits    (501) staff       (20)    11122 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     6119 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/visualisation.py
--rw-r--r--   0 maurits    (501) staff       (20)     3237 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude/zcmlextract.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 14:37:40.754651 i18ndude-6.0.0/src/i18ndude.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    27662 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1572 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      142 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       85 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2023-05-30 14:37:40.000000 i18ndude-6.0.0/src/i18ndude.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.655965 i18ndude-6.0.0a1/
+-rw-r--r--   0 maurits    (501) staff       (20)    14343 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      136 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    27562 2023-05-08 20:57:57.656198 i18ndude-6.0.0a1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1889 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.637197 i18ndude-6.0.0a1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)      825 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/docs/COPYRIGHT
+-rw-r--r--   0 maurits    (501) staff       (20)    15880 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/docs/ChangeLog
+-rw-r--r--   0 maurits    (501) staff       (20)    12296 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/docs/LICENSE
+-rw-r--r--   0 maurits    (501) staff       (20)      439 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/docs/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    10185 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/docs/command.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      397 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      293 2023-05-08 20:57:57.656996 i18ndude-6.0.0a1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2122 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.631591 i18ndude-6.0.0a1/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.643047 i18ndude-6.0.0a1/src/i18ndude/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    32873 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3805 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/common.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20834 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/extract.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10947 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/generator.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2985 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/gsextract.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1831 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    22287 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/pygettext.py
+-rwxr-xr-x   0 maurits    (501) staff       (20)    28016 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/script.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.632302 i18ndude-6.0.0a1/src/i18ndude/testdata/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.652132 i18ndude-6.0.0a1/src/i18ndude/testdata/input/
+-rw-r--r--   0 maurits    (501) staff       (20)      522 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/chameleon.pt
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/empty-en.po
+-rw-r--r--   0 maurits    (501) staff       (20)      778 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/synctest-de.po
+-rw-r--r--   0 maurits    (501) staff       (20)      820 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/synctest.pot
+-rw-r--r--   0 maurits    (501) staff       (20)     2361 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test-en.po
+-rw-r--r--   0 maurits    (501) staff       (20)     1375 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1917 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2779 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test1.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      916 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2-en.po
+-rw-r--r--   0 maurits    (501) staff       (20)      392 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2.py
+-rw-r--r--   0 maurits    (501) staff       (20)      893 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2_expected-en.po
+-rw-r--r--   0 maurits    (501) staff       (20)      728 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test3.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      510 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test4.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      882 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test5.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.652604 i18ndude-6.0.0a1/src/i18ndude/testdata/output/
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/output/README.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.655631 i18ndude-6.0.0a1/src/i18ndude/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    34684 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/test_catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)      252 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/test_extract.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7921 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/test_untranslated.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5558 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/test_utils.py
+-rwxr-xr-x   0 maurits    (501) staff       (20)     1524 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/tox-check-i18ndude-command.sh
+-rw-r--r--   0 maurits    (501) staff       (20)      829 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9723 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/untranslated.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11122 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6119 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/visualisation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3237 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/zcmlextract.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.646149 i18ndude-6.0.0a1/src/i18ndude.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    27562 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1572 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      142 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/top_level.txt
```

### Comparing `i18ndude-6.0.0/CHANGES.rst` & `i18ndude-6.0.0a1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,14 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
-6.0.0 (2023-05-30)
-------------------
-
-Bug fixes:
-
-
-- Fix pre-commit integration.
-  [gforcada] (#1)
-
-
 6.0.0a1 (2023-05-08)
 --------------------
 
 Breaking changes:
 
 
 - Drop support for Python 2.
```

### Comparing `i18ndude-6.0.0/PKG-INFO` & `i18ndude-6.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i18ndude
-Version: 6.0.0
+Version: 6.0.0a1
 Summary: i18ndude performs various tasks related to ZPT's, Python Scripts and i18n.
 Home-page: https://github.com/collective/i18ndude
 Author: Daniel Nouri
 Author-email: plone-i18n@lists.sourceforge.net
 Maintainer: Maurits van Rees
 Maintainer-email: maurits@vanrees.org
 License: GPL
@@ -386,24 +386,14 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
-6.0.0 (2023-05-30)
-------------------
-
-Bug fixes:
-
-
-- Fix pre-commit integration.
-  [gforcada] (#1)
-
-
 6.0.0a1 (2023-05-08)
 --------------------
 
 Breaking changes:
 
 
 - Drop support for Python 2.
```

### Comparing `i18ndude-6.0.0/README.rst` & `i18ndude-6.0.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/docs/COPYRIGHT` & `i18ndude-6.0.0a1/docs/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/docs/ChangeLog` & `i18ndude-6.0.0a1/docs/ChangeLog`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/docs/LICENSE` & `i18ndude-6.0.0a1/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/docs/command.rst` & `i18ndude-6.0.0a1/docs/command.rst`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/setup.py` & `i18ndude-6.0.0a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 
 from setuptools import setup, find_packages
 
-version = '6.0.0'
+version = '6.0.0a1'
 
 install_requires = [
     'lxml',
     'zope.i18nmessageid >= 3.3',
     'zope.interface >= 3.3',
     'zope.tal >= 4.3.0',
 ]
```

### Comparing `i18ndude-6.0.0/src/i18ndude/catalog.py` & `i18ndude-6.0.0a1/src/i18ndude/catalog.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/common.py` & `i18ndude-6.0.0a1/src/i18ndude/common.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/extract.py` & `i18ndude-6.0.0a1/src/i18ndude/extract.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/generator.py` & `i18ndude-6.0.0a1/src/i18ndude/generator.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/gsextract.py` & `i18ndude-6.0.0a1/src/i18ndude/gsextract.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/interfaces.py` & `i18ndude-6.0.0a1/src/i18ndude/interfaces.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/pygettext.py` & `i18ndude-6.0.0a1/src/i18ndude/pygettext.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/script.py` & `i18ndude-6.0.0a1/src/i18ndude/script.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/testdata/input/chameleon.pt` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/chameleon.pt`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/testdata/input/synctest-de.po` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/synctest-de.po`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/testdata/input/synctest.pot` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/synctest.pot`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/testdata/input/test-en.po` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test-en.po`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/testdata/input/test.xml` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test.xml`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/testdata/input/test.zcml` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test.zcml`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/testdata/input/test1.pt` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test1.pt`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/testdata/input/test2-en.po` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2-en.po`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/testdata/input/test2_expected-en.po` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2_expected-en.po`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/testdata/input/test3.pt` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test3.pt`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/testdata/input/test5.pt` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test5.pt`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/tests/test_catalog.py` & `i18ndude-6.0.0a1/src/i18ndude/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/tests/test_untranslated.py` & `i18ndude-6.0.0a1/src/i18ndude/tests/test_untranslated.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/tests/test_utils.py` & `i18ndude-6.0.0a1/src/i18ndude/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/tests/tox-check-i18ndude-command.sh` & `i18ndude-6.0.0a1/src/i18ndude/tests/tox-check-i18ndude-command.sh`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/tests/utils.py` & `i18ndude-6.0.0a1/src/i18ndude/tests/utils.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/untranslated.py` & `i18ndude-6.0.0a1/src/i18ndude/untranslated.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/utils.py` & `i18ndude-6.0.0a1/src/i18ndude/utils.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/visualisation.py` & `i18ndude-6.0.0a1/src/i18ndude/visualisation.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude/zcmlextract.py` & `i18ndude-6.0.0a1/src/i18ndude/zcmlextract.py`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0/src/i18ndude.egg-info/PKG-INFO` & `i18ndude-6.0.0a1/src/i18ndude.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i18ndude
-Version: 6.0.0
+Version: 6.0.0a1
 Summary: i18ndude performs various tasks related to ZPT's, Python Scripts and i18n.
 Home-page: https://github.com/collective/i18ndude
 Author: Daniel Nouri
 Author-email: plone-i18n@lists.sourceforge.net
 Maintainer: Maurits van Rees
 Maintainer-email: maurits@vanrees.org
 License: GPL
@@ -386,24 +386,14 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
-6.0.0 (2023-05-30)
-------------------
-
-Bug fixes:
-
-
-- Fix pre-commit integration.
-  [gforcada] (#1)
-
-
 6.0.0a1 (2023-05-08)
 --------------------
 
 Breaking changes:
 
 
 - Drop support for Python 2.
```

### Comparing `i18ndude-6.0.0/src/i18ndude.egg-info/SOURCES.txt` & `i18ndude-6.0.0a1/src/i18ndude.egg-info/SOURCES.txt`

 * *Files identical despite different names*

