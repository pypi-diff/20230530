# Comparing `tmp/audresample-1.2.1.tar.gz` & `tmp/audresample-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audresample-1.2.1.tar", last modified: Fri Jan 27 12:35:11 2023, max compression
+gzip compressed data, was "audresample-1.3.0.tar", last modified: Tue May 30 07:15:30 2023, max compression
```

## Comparing `audresample-1.2.1.tar` & `audresample-1.3.0.tar`

### file list

```diff
@@ -1,83 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.706442 audresample-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.698442 audresample-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.698442 audresample-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-01-27 12:34:53.000000 audresample-1.2.1/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-01-27 12:34:53.000000 audresample-1.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-01-27 12:34:53.000000 audresample-1.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-27 12:34:53.000000 audresample-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-27 12:34:53.000000 audresample-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-01-27 12:34:53.000000 audresample-1.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-01-27 12:34:53.000000 audresample-1.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-27 12:34:53.000000 audresample-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-01-27 12:35:11.706442 audresample-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-01-27 12:34:53.000000 audresample-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.698442 audresample-1.2.1/audresample/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-01-27 12:34:53.000000 audresample-1.2.1/audresample/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.702442 audresample-1.2.1/audresample/core/
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-01-27 12:34:53.000000 audresample-1.2.1/audresample/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.698442 audresample-1.2.1/audresample/core/bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.702442 audresample-1.2.1/audresample/core/bin/linux/
--rwxr-xr-x   0 runner    (1001) docker     (123)   290720 2023-01-27 12:34:53.000000 audresample-1.2.1/audresample/core/bin/linux/libaudresample.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.702442 audresample-1.2.1/audresample/core/bin/macos-intel/
--rwxr-xr-x   0 runner    (1001) docker     (123)   289712 2023-01-27 12:34:53.000000 audresample-1.2.1/audresample/core/bin/macos-intel/libaudresample.dylib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.702442 audresample-1.2.1/audresample/core/bin/macos-m1/
--rwxr-xr-x   0 runner    (1001) docker     (123)   206817 2023-01-27 12:34:53.000000 audresample-1.2.1/audresample/core/bin/macos-m1/libaudresample.dylib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.702442 audresample-1.2.1/audresample/core/bin/windows/
--rw-r--r--   0 runner    (1001) docker     (123)   361472 2023-01-27 12:34:53.000000 audresample-1.2.1/audresample/core/bin/windows/audresample.dll
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-27 12:34:53.000000 audresample-1.2.1/audresample/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-27 12:34:53.000000 audresample-1.2.1/audresample/core/define.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-01-27 12:34:53.000000 audresample-1.2.1/audresample/core/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.702442 audresample-1.2.1/audresample/define/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-27 12:34:53.000000 audresample-1.2.1/audresample/define/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.702442 audresample-1.2.1/audresample.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-01-27 12:35:10.000000 audresample-1.2.1/audresample.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-01-27 12:35:11.000000 audresample-1.2.1/audresample.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 12:35:10.000000 audresample-1.2.1/audresample.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-27 12:35:10.000000 audresample-1.2.1/audresample.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-27 12:35:10.000000 audresample-1.2.1/audresample.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.702442 audresample-1.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.698442 audresample-1.2.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.702442 audresample-1.2.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-27 12:34:53.000000 audresample-1.2.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-01-27 12:34:53.000000 audresample-1.2.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-01-27 12:34:53.000000 audresample-1.2.1/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.702442 audresample-1.2.1/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-27 12:34:53.000000 audresample-1.2.1/docs/api-src/audresample.define.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-27 12:34:53.000000 audresample-1.2.1/docs/api-src/audresample.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-27 12:34:53.000000 audresample-1.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-01-27 12:34:53.000000 audresample-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-27 12:34:53.000000 audresample-1.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-27 12:34:53.000000 audresample-1.2.1/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-01-27 12:34:53.000000 audresample-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-27 12:34:53.000000 audresample-1.2.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-27 12:34:53.000000 audresample-1.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-01-27 12:34:53.000000 audresample-1.2.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.706442 audresample-1.2.1/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-01-27 12:34:53.000000 audresample-1.2.1/misc/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-27 12:34:53.000000 audresample-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-01-27 12:35:11.710442 audresample-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-27 12:34:53.000000 audresample-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.706442 audresample-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:35:11.706442 audresample-1.2.1/tests/test-assets/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/generate_test_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/original__sr_16000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/original__sr_16000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/original__sr_44100__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/original__sr_44100__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/original__sr_8000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/original__sr_8000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test_remix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-01-27 12:34:53.000000 audresample-1.2.1/tests/test_resample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.477567 audresample-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.465567 audresample-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-30 07:15:11.000000 audresample-1.3.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-30 07:15:11.000000 audresample-1.3.0/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-30 07:15:11.000000 audresample-1.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-30 07:15:11.000000 audresample-1.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 07:15:11.000000 audresample-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 07:15:11.000000 audresample-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-30 07:15:11.000000 audresample-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-30 07:15:11.000000 audresample-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-30 07:15:11.000000 audresample-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-30 07:15:30.477567 audresample-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-30 07:15:11.000000 audresample-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/audresample/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/audresample/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/audresample/core/bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/audresample/core/bin/macosx_12_0_arm64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   206817 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/bin/macosx_12_0_arm64/libaudresample.dylib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/audresample/core/bin/macosx_12_0_x86_64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   289712 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/bin/macosx_12_0_x86_64/libaudresample.dylib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/audresample/core/bin/manylinux_2_17_aarch64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   204120 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/bin/manylinux_2_17_aarch64/libaudresample.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/audresample/core/bin/manylinux_2_17_armv7l/
+-rw-r--r--   0 runner    (1001) docker     (123)   154436 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/bin/manylinux_2_17_armv7l/libaudresample.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/audresample/core/bin/manylinux_2_17_x86_64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   290720 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/bin/manylinux_2_17_x86_64/libaudresample.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/audresample/core/bin/win_amd64/
+-rw-r--r--   0 runner    (1001) docker     (123)   361472 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/bin/win_amd64/audresample.dll
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/define.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/audresample/define/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/define/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/audresample.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-30 07:15:30.000000 audresample-1.3.0/audresample.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-30 07:15:30.000000 audresample-1.3.0/audresample.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 07:15:30.000000 audresample-1.3.0/audresample.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 07:15:30.000000 audresample-1.3.0/audresample.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 07:15:30.000000 audresample-1.3.0/audresample.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/api-src/audresample.define.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/api-src/audresample.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-30 07:15:11.000000 audresample-1.3.0/misc/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 07:15:11.000000 audresample-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-30 07:15:30.481567 audresample-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-30 07:15:11.000000 audresample-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.477567 audresample-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.477567 audresample-1.3.0/tests/test-assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/generate_test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/original__sr_16000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/original__sr_16000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/original__sr_44100__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/original__sr_44100__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/original__sr_8000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/original__sr_8000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test_remix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test_resample.py
```

### Comparing `audresample-1.2.1/.github/workflows/publish.yml` & `audresample-1.3.0/.github/workflows/publish.yml`

 * *Files 15% similar despite different names*

```diff
@@ -2,39 +2,85 @@
 
 on:
   push:
     tags:
       - 'v*' # Push events to matching v*, i.e. v1.0, v20.15.10
 
 jobs:
-  deploy:
-    runs-on: ubuntu-latest
+  build:
+
+    runs-on: 'ubuntu-latest'
+    strategy:
+      matrix:
+        platform:
+        - macosx_12_0_x86_64
+        - macosx_12_0_arm64
+        - manylinux_2_17_x86_64
+        - manylinux_2_17_armv7l
+        - manylinux_2_17_aarch64
+        - win_amd64
+
     steps:
     - uses: actions/checkout@v3
+      # Need more than a shallow clone to get version from tags
       with:
         fetch-depth: 2
 
+    - name: Set up Python 3.8
+      uses: actions/setup-python@v4
+      with:
+        python-version: '3.8'
+
+    - name: Install build dependencies
+      run: |
+        python -m pip install --upgrade pip
+        pip install build
+
+    - name: Build wheels
+      run: python -m build --wheel --outdir wheelhouse
+      env:
+        PLAT_NAME: ${{ matrix.platform }}
+
+    - name: Build source distribution
+      run: python -m build --sdist --outdir wheelhouse
+      if: matrix.platform == 'manylinux_2_17_x86_64'
+
+    - uses: actions/upload-artifact@v3
+      with:
+        path: ./wheelhouse/*
+
+  deploy:
+
+    runs-on: 'ubuntu-latest'
+    needs: [ build ]
+    
+    steps:
+
+    - name: Download dist artifacts
+      uses: actions/download-artifact@v3
+      with:
+        name: artifact
+        path: dist
+
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.8'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install setuptools wheel twine
+        pip install twine
 
     # PyPI package
-    - name: Build and publish
+    - name: Publish
       env:
         TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
         TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
-      run: |
-        python setup.py sdist bdist_wheel
-        python -m twine upload dist/*
+      run: python -m twine upload dist/*
 
     # Docuemntation
     - name: Install doc dependencies
       run: |
         pip install -r requirements.txt
         pip install -r docs/requirements.txt
```

### Comparing `audresample-1.2.1/.github/workflows/test.yml` & `audresample-1.3.0/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -39,26 +39,19 @@
       if: matrix.os == 'ubuntu-latest' || matrix.os == 'ubuntu-20.04'
 
     - name: Install dependencies
       run: |
         python -V
         python -m pip install --upgrade pip
         pip install -r requirements.txt
-        pip install -r docs/requirements.txt
         pip install -r tests/requirements.txt
 
     - name: Test with pytest
       run: |
         python -m pytest
 
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v3
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         file: ./coverage.xml
       if: matrix.os == 'ubuntu-20.04'
-
-    - name: Test building documentation
-      run: |
-        python -m sphinx docs/ docs/_build/ -b html -W
-        python -m sphinx docs/ build/sphinx/html -b linkcheck
-      if: matrix.os == 'ubuntu-20.04'
```

### Comparing `audresample-1.2.1/CHANGELOG.rst` & `audresample-1.3.0/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,34 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.3.0 (2023-05-30)
+--------------------------
+
+* Added: support for Raspberry Pi
+  64-bit (aarch64)
+  and 32-bit (armv7l)
+* Added: code example to README
+  that highlights the functionality
+  of the package
+* Changed: replace universal wheel
+  of Python package
+  by dedicated platform wheels for
+  ``macosx_12_0_arm64``,
+  ``macosx_12_0_x86_64``,
+  ``manylinux_2_17_aarch64``,
+  ``manylinux_2_17_armv7l``,
+  ``manylinux_2_17_x86_64``,
+  ``win_amd64``
+
+
 Version 1.2.1 (2023-01-27)
 --------------------------
 
 * Fixed: require ``sphinx-audeering-theme>=1.2.1``
   to ensure the correct theme is used
   for the public documentation
```

### Comparing `audresample-1.2.1/CONTRIBUTING.rst` & `audresample-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/LICENSE` & `audresample-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/README.rst` & `audresample-1.3.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 ===========
 audresample
 ===========
 
 |tests| |coverage| |docs| |python-versions| |license|
 
-Python wrapper for `audresamplelib`_
-that provides functions to
-resample and remix audio signals.
-Resampling is only supported for
-signals in single precision floating-point format.
+**audresample** remixes or resamples your signals.
+
+Resampling is supported
+for signals in single precision floating-point format,
+and based on the `soxr`_ implementation
+as provided by `audresamplelib`_.
 
 Have a look at the installation_ and usage_ instructions.
 
+.. code-block:: python
+
+    >>> import numpy as np
+    >>> import audresample
+    >>> signal = np.zeros((2, 8000), dtype='float32')
+    >>> signal.shape
+    (2, 8000)
+    >>> audresample.remix(signal, mixdown=True).shape
+    (1, 8000)
+    >>> audresample.remix(signal, channels=[0, 0, 1, 1]).shape
+    (4, 8000)
+    >>> audresample.resample(signal, 8000, 16000).shape
+    (2, 16000)
+
+.. _soxr: https://sourceforge.net/projects/soxr/
 .. _audresamplelib: https://github.com/audeering/audresamplelib
 .. _installation: https://audeering.github.io/audresample/install.html
 .. _usage: https://audeering.github.io/audresample/usage.html
 
 
 .. badges images and links:
 .. |tests| image:: https://github.com/audeering/audresample/workflows/Test/badge.svg
```

### Comparing `audresample-1.2.1/audresample/core/api.py` & `audresample-1.3.0/audresample/core/api.py`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/audresample/core/bin/linux/libaudresample.so` & `audresample-1.3.0/audresample/core/bin/manylinux_2_17_x86_64/libaudresample.so`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/audresample/core/bin/macos-intel/libaudresample.dylib` & `audresample-1.3.0/audresample/core/bin/macosx_12_0_x86_64/libaudresample.dylib`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/audresample/core/bin/macos-m1/libaudresample.dylib` & `audresample-1.3.0/audresample/core/bin/macosx_12_0_arm64/libaudresample.dylib`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/audresample/core/bin/windows/audresample.dll` & `audresample-1.3.0/audresample/core/bin/win_amd64/audresample.dll`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/audresample.egg-info/SOURCES.txt` & `audresample-1.3.0/audresample.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,35 @@
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 README.rst
 requirements.txt
 setup.cfg
 setup.py
+.github/workflows/doc.yml
 .github/workflows/flake8.yml
 .github/workflows/publish.yml
 .github/workflows/test.yml
 audresample/__init__.py
 audresample.egg-info/PKG-INFO
 audresample.egg-info/SOURCES.txt
 audresample.egg-info/dependency_links.txt
 audresample.egg-info/requires.txt
 audresample.egg-info/top_level.txt
+audresample/core/__init__.py
 audresample/core/api.py
 audresample/core/config.py
 audresample/core/define.py
 audresample/core/lib.py
-audresample/core/bin/linux/libaudresample.so
-audresample/core/bin/macos-intel/libaudresample.dylib
-audresample/core/bin/macos-m1/libaudresample.dylib
-audresample/core/bin/windows/audresample.dll
+audresample/core/bin/macosx_12_0_arm64/libaudresample.dylib
+audresample/core/bin/macosx_12_0_x86_64/libaudresample.dylib
+audresample/core/bin/manylinux_2_17_aarch64/libaudresample.so
+audresample/core/bin/manylinux_2_17_armv7l/libaudresample.so
+audresample/core/bin/manylinux_2_17_x86_64/libaudresample.so
+audresample/core/bin/win_amd64/audresample.dll
 audresample/define/__init__.py
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/genindex.rst
 docs/index.rst
 docs/install.rst
```

### Comparing `audresample-1.2.1/docs/_templates/autosummary/class.rst` & `audresample-1.3.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/docs/conf.py` & `audresample-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/docs/index.rst` & `audresample-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/docs/usage.rst` & `audresample-1.3.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/misc/icon.png` & `audresample-1.3.0/misc/icon.png`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/setup.cfg` & `audresample-1.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author_email = jwagner@audeering.com, acrespi@audeering.com, hwierstorf@audeering.com
 url = https://github.com/audeering/audresample/
 project_urls = 
 	Documentation = https://audeering.github.io/audresample/
 description = Provides functions to resample and remix a signal
 long_description = file: README.rst, CHANGELOG.rst
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 keywords = audio, dsp, resample, remix
 platforms = any
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Science/Research
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
@@ -23,16 +23,14 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 
 [options]
-packages = find:
-include_package_data = True
 install_requires = 
 	numpy
 setup_requires = 
 	setuptools_scm
 
 [tool:pytest]
 addopts =
```

### Comparing `audresample-1.2.1/tests/test-assets/generate_test_assets.py` & `audresample-1.3.0/tests/test-assets/generate_test_assets.py`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/original__sr_16000__channels_1.wav` & `audresample-1.3.0/tests/test-assets/original__sr_16000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/original__sr_16000__channels_2.wav` & `audresample-1.3.0/tests/test-assets/original__sr_16000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/original__sr_44100__channels_1.wav` & `audresample-1.3.0/tests/test-assets/original__sr_44100__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/original__sr_44100__channels_2.wav` & `audresample-1.3.0/tests/test-assets/original__sr_44100__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/original__sr_8000__channels_1.wav` & `audresample-1.3.0/tests/test-assets/original__sr_8000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/original__sr_8000__channels_2.wav` & `audresample-1.3.0/tests/test-assets/original__sr_8000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_1.wav` & `audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_2.wav` & `audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_1.wav` & `audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_2.wav` & `audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_1.wav` & `audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_2.wav` & `audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_1.wav` & `audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_2.wav` & `audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_1.wav` & `audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_2.wav` & `audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_1.wav` & `audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_2.wav` & `audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test_remix.py` & `audresample-1.3.0/tests/test_remix.py`

 * *Files identical despite different names*

### Comparing `audresample-1.2.1/tests/test_resample.py` & `audresample-1.3.0/tests/test_resample.py`

 * *Files identical despite different names*

