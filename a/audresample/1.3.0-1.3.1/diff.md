# Comparing `tmp/audresample-1.3.0.tar.gz` & `tmp/audresample-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audresample-1.3.0.tar", last modified: Tue May 30 07:15:30 2023, max compression
+gzip compressed data, was "audresample-1.3.1.tar", last modified: Tue May 30 08:17:15 2023, max compression
```

## Comparing `audresample-1.3.0.tar` & `audresample-1.3.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.477567 audresample-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.465567 audresample-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-30 07:15:11.000000 audresample-1.3.0/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-30 07:15:11.000000 audresample-1.3.0/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-30 07:15:11.000000 audresample-1.3.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-30 07:15:11.000000 audresample-1.3.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 07:15:11.000000 audresample-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 07:15:11.000000 audresample-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-30 07:15:11.000000 audresample-1.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-30 07:15:11.000000 audresample-1.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-30 07:15:11.000000 audresample-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-30 07:15:30.477567 audresample-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-30 07:15:11.000000 audresample-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/audresample/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/audresample/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/audresample/core/bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/audresample/core/bin/macosx_12_0_arm64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   206817 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/bin/macosx_12_0_arm64/libaudresample.dylib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/audresample/core/bin/macosx_12_0_x86_64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   289712 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/bin/macosx_12_0_x86_64/libaudresample.dylib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/audresample/core/bin/manylinux_2_17_aarch64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   204120 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/bin/manylinux_2_17_aarch64/libaudresample.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/audresample/core/bin/manylinux_2_17_armv7l/
--rw-r--r--   0 runner    (1001) docker     (123)   154436 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/bin/manylinux_2_17_armv7l/libaudresample.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/audresample/core/bin/manylinux_2_17_x86_64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   290720 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/bin/manylinux_2_17_x86_64/libaudresample.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/audresample/core/bin/win_amd64/
--rw-r--r--   0 runner    (1001) docker     (123)   361472 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/bin/win_amd64/audresample.dll
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/define.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/core/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/audresample/define/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 07:15:11.000000 audresample-1.3.0/audresample/define/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/audresample.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-30 07:15:30.000000 audresample-1.3.0/audresample.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-30 07:15:30.000000 audresample-1.3.0/audresample.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 07:15:30.000000 audresample-1.3.0/audresample.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 07:15:30.000000 audresample-1.3.0/audresample.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 07:15:30.000000 audresample-1.3.0/audresample.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.469567 audresample-1.3.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/api-src/audresample.define.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/api-src/audresample.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-30 07:15:11.000000 audresample-1.3.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.473567 audresample-1.3.0/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-30 07:15:11.000000 audresample-1.3.0/misc/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 07:15:11.000000 audresample-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-30 07:15:30.481567 audresample-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-30 07:15:11.000000 audresample-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.477567 audresample-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:15:30.477567 audresample-1.3.0/tests/test-assets/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/generate_test_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/original__sr_16000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/original__sr_16000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/original__sr_44100__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/original__sr_44100__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/original__sr_8000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/original__sr_8000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test_remix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-30 07:15:11.000000 audresample-1.3.0/tests/test_resample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.286961 audresample-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.270960 audresample-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-30 08:16:51.000000 audresample-1.3.1/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-30 08:16:51.000000 audresample-1.3.1/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-30 08:16:51.000000 audresample-1.3.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-30 08:16:51.000000 audresample-1.3.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 08:16:51.000000 audresample-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 08:16:51.000000 audresample-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-30 08:16:51.000000 audresample-1.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-30 08:16:51.000000 audresample-1.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-30 08:16:51.000000 audresample-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-30 08:17:15.286961 audresample-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-30 08:16:51.000000 audresample-1.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/audresample/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/audresample/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/audresample/core/bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/audresample/core/bin/macosx_10_4_x86_64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   289712 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/bin/macosx_10_4_x86_64/libaudresample.dylib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/audresample/core/bin/macosx_11_0_arm64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   206817 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/bin/macosx_11_0_arm64/libaudresample.dylib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/audresample/core/bin/manylinux_2_17_aarch64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   204120 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/bin/manylinux_2_17_aarch64/libaudresample.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/audresample/core/bin/manylinux_2_17_armv7l/
+-rw-r--r--   0 runner    (1001) docker     (123)   154436 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/bin/manylinux_2_17_armv7l/libaudresample.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/audresample/core/bin/manylinux_2_17_x86_64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   290720 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/bin/manylinux_2_17_x86_64/libaudresample.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/audresample/core/bin/win_amd64/
+-rw-r--r--   0 runner    (1001) docker     (123)   361472 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/bin/win_amd64/audresample.dll
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/define.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/audresample/define/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/define/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/audresample.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-30 08:17:15.000000 audresample-1.3.1/audresample.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-30 08:17:15.000000 audresample-1.3.1/audresample.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:17:15.000000 audresample-1.3.1/audresample.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 08:17:15.000000 audresample-1.3.1/audresample.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 08:17:15.000000 audresample-1.3.1/audresample.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.282961 audresample-1.3.1/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/api-src/audresample.define.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/api-src/audresample.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.282961 audresample-1.3.1/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-30 08:16:51.000000 audresample-1.3.1/misc/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 08:16:51.000000 audresample-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-30 08:17:15.286961 audresample-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-30 08:16:51.000000 audresample-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.282961 audresample-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.286961 audresample-1.3.1/tests/test-assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/generate_test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/original__sr_16000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/original__sr_16000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/original__sr_44100__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/original__sr_44100__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/original__sr_8000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/original__sr_8000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test_remix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test_resample.py
```

### Comparing `audresample-1.3.0/.github/workflows/doc.yml` & `audresample-1.3.1/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/.github/workflows/publish.yml` & `audresample-1.3.1/.github/workflows/publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,17 @@
   deploy:
 
     runs-on: 'ubuntu-latest'
     needs: [ build ]
     
     steps:
 
+    - name: Clone repository
+      uses: actions/checkout@v3
+
     - name: Download dist artifacts
       uses: actions/download-artifact@v3
       with:
         name: artifact
         path: dist
 
     - name: Set up Python
@@ -74,15 +77,15 @@
     # PyPI package
     - name: Publish
       env:
         TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
         TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
       run: python -m twine upload dist/*
 
-    # Docuemntation
+    # Documentation
     - name: Install doc dependencies
       run: |
         pip install -r requirements.txt
         pip install -r docs/requirements.txt
 
     - name: Build documentation
       run: |
```

### Comparing `audresample-1.3.0/.github/workflows/test.yml` & `audresample-1.3.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/CHANGELOG.rst` & `audresample-1.3.1/CHANGELOG.rst`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.3.1 (2023-05-30)
+--------------------------
+
+* Fixed: documentation building in deploy step
+  of ``publish`` Action on Github
+* Changed: switch versions of MacOS wheel to
+  ``macosx_11_0_arm64``,
+  ``macosx_10_4_x86_64``
+
+
 Version 1.3.0 (2023-05-30)
 --------------------------
 
 * Added: support for Raspberry Pi
   64-bit (aarch64)
   and 32-bit (armv7l)
 * Added: code example to README
```

### Comparing `audresample-1.3.0/CONTRIBUTING.rst` & `audresample-1.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/LICENSE` & `audresample-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/PKG-INFO` & `audresample-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audresample
-Version: 1.3.0
+Version: 1.3.1
 Summary: Provides functions to resample and remix a signal
 Home-page: https://github.com/audeering/audresample/
 Author: Johannes Wagner, Andrea Crespi, Hagen Wierstorf
 Author-email: jwagner@audeering.com, acrespi@audeering.com, hwierstorf@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audresample/
 Keywords: audio,dsp,resample,remix
@@ -81,14 +81,24 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.3.1 (2023-05-30)
+--------------------------
+
+* Fixed: documentation building in deploy step
+  of ``publish`` Action on Github
+* Changed: switch versions of MacOS wheel to
+  ``macosx_11_0_arm64``,
+  ``macosx_10_4_x86_64``
+
+
 Version 1.3.0 (2023-05-30)
 --------------------------
 
 * Added: support for Raspberry Pi
   64-bit (aarch64)
   and 32-bit (armv7l)
 * Added: code example to README
```

### Comparing `audresample-1.3.0/README.rst` & `audresample-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/audresample/core/api.py` & `audresample-1.3.1/audresample/core/api.py`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/audresample/core/bin/macosx_12_0_arm64/libaudresample.dylib` & `audresample-1.3.1/audresample/core/bin/macosx_11_0_arm64/libaudresample.dylib`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/audresample/core/bin/macosx_12_0_x86_64/libaudresample.dylib` & `audresample-1.3.1/audresample/core/bin/macosx_10_4_x86_64/libaudresample.dylib`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/audresample/core/bin/manylinux_2_17_aarch64/libaudresample.so` & `audresample-1.3.1/audresample/core/bin/manylinux_2_17_aarch64/libaudresample.so`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/audresample/core/bin/manylinux_2_17_armv7l/libaudresample.so` & `audresample-1.3.1/audresample/core/bin/manylinux_2_17_armv7l/libaudresample.so`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/audresample/core/bin/manylinux_2_17_x86_64/libaudresample.so` & `audresample-1.3.1/audresample/core/bin/manylinux_2_17_x86_64/libaudresample.so`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/audresample/core/bin/win_amd64/audresample.dll` & `audresample-1.3.1/audresample/core/bin/win_amd64/audresample.dll`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/audresample/core/lib.py` & `audresample-1.3.1/audresample/core/lib.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     Expected outcomes are:
 
     ==================== ======================
     Linux, 64-bit        manylinux_2_17_x86_64
     Raspberry Pi, 32-bit manylinux_2_17_armv7l
     Raspberry Pi, 64-bit manylinux_2_17_aarch64
     Windows              win_amd64
-    MacOS Intel          macosx_12_0_x86_64
-    MacOS M1             macosx_12_0_arm64
+    MacOS Intel          macosx_10_4_x86_64
+    MacOS M1             macosx_11_0_arm64
     ==================== ======================
 
     Under Linux the manylinux version
     can be extracted
     by inspecting the wheel
     with ``auditwheel``.
 
@@ -27,24 +27,28 @@
     .. code-block:: bash
 
         $ pip debug --verbose
 
     """
     system = platform.system()
     machine = platform.machine().lower()
-    system_mapping = {
-        'Linux': 'manylinux_2_17',
-        'Windows': 'win',
-        'Darwin': 'macosx_12_0',
-    }
 
-    if system not in system_mapping:  # pragma: no cover
+    if system == 'Linux':  # pragma: no cover
+        system = 'manylinux_2_17'
+    elif system == 'Windows':  # pragma: no cover
+        system = 'win'
+    elif system == 'Darwin':  # pragma: no cover
+        if machine == 'x86_64':
+            system = 'macosx_10_4'
+        else:
+            system = 'macosx_11_0'
+    else:  # pragma: no cover
         raise RuntimeError(f'Unsupported platform {system}')
 
-    return f'{system_mapping[system]}_{machine}'
+    return f'{system}_{machine}'
 
 
 # load library
 
 root = os.path.dirname(os.path.realpath(__file__))
 bin_path = os.path.join(root, 'bin')
```

### Comparing `audresample-1.3.0/audresample.egg-info/PKG-INFO` & `audresample-1.3.1/audresample.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audresample
-Version: 1.3.0
+Version: 1.3.1
 Summary: Provides functions to resample and remix a signal
 Home-page: https://github.com/audeering/audresample/
 Author: Johannes Wagner, Andrea Crespi, Hagen Wierstorf
 Author-email: jwagner@audeering.com, acrespi@audeering.com, hwierstorf@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audresample/
 Keywords: audio,dsp,resample,remix
@@ -81,14 +81,24 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.3.1 (2023-05-30)
+--------------------------
+
+* Fixed: documentation building in deploy step
+  of ``publish`` Action on Github
+* Changed: switch versions of MacOS wheel to
+  ``macosx_11_0_arm64``,
+  ``macosx_10_4_x86_64``
+
+
 Version 1.3.0 (2023-05-30)
 --------------------------
 
 * Added: support for Raspberry Pi
   64-bit (aarch64)
   and 32-bit (armv7l)
 * Added: code example to README
```

### Comparing `audresample-1.3.0/audresample.egg-info/SOURCES.txt` & `audresample-1.3.1/audresample.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 audresample.egg-info/requires.txt
 audresample.egg-info/top_level.txt
 audresample/core/__init__.py
 audresample/core/api.py
 audresample/core/config.py
 audresample/core/define.py
 audresample/core/lib.py
-audresample/core/bin/macosx_12_0_arm64/libaudresample.dylib
-audresample/core/bin/macosx_12_0_x86_64/libaudresample.dylib
+audresample/core/bin/macosx_10_4_x86_64/libaudresample.dylib
+audresample/core/bin/macosx_11_0_arm64/libaudresample.dylib
 audresample/core/bin/manylinux_2_17_aarch64/libaudresample.so
 audresample/core/bin/manylinux_2_17_armv7l/libaudresample.so
 audresample/core/bin/manylinux_2_17_x86_64/libaudresample.so
 audresample/core/bin/win_amd64/audresample.dll
 audresample/define/__init__.py
 docs/changelog.rst
 docs/conf.py
```

### Comparing `audresample-1.3.0/docs/_templates/autosummary/class.rst` & `audresample-1.3.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/docs/conf.py` & `audresample-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/docs/index.rst` & `audresample-1.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/docs/usage.rst` & `audresample-1.3.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/misc/icon.png` & `audresample-1.3.1/misc/icon.png`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/setup.cfg` & `audresample-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/setup.py` & `audresample-1.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 
 import setuptools
 
 
 # Include only the platform specific pre-compiled binary.
 # For sources see https://github.com/audeering/audresamplelib
 
-
 def platform_name():
     r"""Platform name used in pip tag.
 
     Expected outcomes are:
 
     ==================== ======================
     Linux, 64-bit        manylinux_2_17_x86_64
     Raspberry Pi, 32-bit manylinux_2_17_armv7l
     Raspberry Pi, 64-bit manylinux_2_17_aarch64
     Windows              win_amd64
-    MacOS Intel          macosx_12_0_x86_64
-    MacOS M1             macosx_12_0_arm64
+    MacOS Intel          macosx_10_4_x86_64
+    MacOS M1             macosx_11_0_arm64
     ==================== ======================
 
     Under Linux the manylinux version
     can be extracted
     by inspecting the wheel
     with ``auditwheel``.
 
@@ -32,24 +31,28 @@
     .. code-block:: bash
 
         $ pip debug --verbose
 
     """
     system = platform.system()
     machine = platform.machine().lower()
-    system_mapping = {
-        'Linux': 'manylinux_2_17',
-        'Windows': 'win',
-        'Darwin': 'macosx_12_0',
-    }
 
-    if system not in system_mapping:
+    if system == 'Linux':  # pragma: no cover
+        system = 'manylinux_2_17'
+    elif system == 'Windows':  # pragma: no cover
+        system = 'win'
+    elif system == 'Darwin':  # pragma: no cover
+        if machine == 'x86_64':
+            system = 'macosx_10_4'
+        else:
+            system = 'macosx_11_0'
+    else:  # pragma: no cover
         raise RuntimeError(f'Unsupported platform {system}')
 
-    return f'{system_mapping[system]}_{machine}'
+    return f'{system}_{machine}'
 
 
 # Look for enrionment variable PLAT_NAME
 # to be able to enforce
 # different platform names
 # in CI on the same runner
 plat_name = os.environ.get('PLAT_NAME', platform_name())
```

### Comparing `audresample-1.3.0/tests/test-assets/generate_test_assets.py` & `audresample-1.3.1/tests/test-assets/generate_test_assets.py`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/original__sr_16000__channels_1.wav` & `audresample-1.3.1/tests/test-assets/original__sr_16000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/original__sr_16000__channels_2.wav` & `audresample-1.3.1/tests/test-assets/original__sr_16000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/original__sr_44100__channels_1.wav` & `audresample-1.3.1/tests/test-assets/original__sr_44100__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/original__sr_44100__channels_2.wav` & `audresample-1.3.1/tests/test-assets/original__sr_44100__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/original__sr_8000__channels_1.wav` & `audresample-1.3.1/tests/test-assets/original__sr_8000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/original__sr_8000__channels_2.wav` & `audresample-1.3.1/tests/test-assets/original__sr_8000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_1.wav` & `audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_2.wav` & `audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_1.wav` & `audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_2.wav` & `audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_1.wav` & `audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_2.wav` & `audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_1.wav` & `audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_2.wav` & `audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_1.wav` & `audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_2.wav` & `audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_1.wav` & `audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_2.wav` & `audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test_remix.py` & `audresample-1.3.1/tests/test_remix.py`

 * *Files identical despite different names*

### Comparing `audresample-1.3.0/tests/test_resample.py` & `audresample-1.3.1/tests/test_resample.py`

 * *Files identical despite different names*

