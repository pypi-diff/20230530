# Comparing `tmp/audresample-1.3.1.tar.gz` & `tmp/audresample-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audresample-1.3.1.tar", last modified: Tue May 30 08:17:15 2023, max compression
+gzip compressed data, was "audresample-1.3.2.tar", last modified: Tue May 30 09:36:22 2023, max compression
```

## Comparing `audresample-1.3.1.tar` & `audresample-1.3.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.286961 audresample-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.270960 audresample-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-30 08:16:51.000000 audresample-1.3.1/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-30 08:16:51.000000 audresample-1.3.1/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-30 08:16:51.000000 audresample-1.3.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-30 08:16:51.000000 audresample-1.3.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 08:16:51.000000 audresample-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 08:16:51.000000 audresample-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-30 08:16:51.000000 audresample-1.3.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-30 08:16:51.000000 audresample-1.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-30 08:16:51.000000 audresample-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-30 08:17:15.286961 audresample-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-30 08:16:51.000000 audresample-1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/audresample/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/audresample/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/audresample/core/bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/audresample/core/bin/macosx_10_4_x86_64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   289712 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/bin/macosx_10_4_x86_64/libaudresample.dylib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/audresample/core/bin/macosx_11_0_arm64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   206817 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/bin/macosx_11_0_arm64/libaudresample.dylib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/audresample/core/bin/manylinux_2_17_aarch64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   204120 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/bin/manylinux_2_17_aarch64/libaudresample.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/audresample/core/bin/manylinux_2_17_armv7l/
--rw-r--r--   0 runner    (1001) docker     (123)   154436 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/bin/manylinux_2_17_armv7l/libaudresample.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/audresample/core/bin/manylinux_2_17_x86_64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   290720 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/bin/manylinux_2_17_x86_64/libaudresample.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/audresample/core/bin/win_amd64/
--rw-r--r--   0 runner    (1001) docker     (123)   361472 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/bin/win_amd64/audresample.dll
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/define.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/core/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/audresample/define/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 08:16:51.000000 audresample-1.3.1/audresample/define/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/audresample.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-30 08:17:15.000000 audresample-1.3.1/audresample.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-30 08:17:15.000000 audresample-1.3.1/audresample.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:17:15.000000 audresample-1.3.1/audresample.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 08:17:15.000000 audresample-1.3.1/audresample.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 08:17:15.000000 audresample-1.3.1/audresample.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.274961 audresample-1.3.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.278961 audresample-1.3.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.282961 audresample-1.3.1/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/api-src/audresample.define.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/api-src/audresample.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-30 08:16:51.000000 audresample-1.3.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.282961 audresample-1.3.1/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-30 08:16:51.000000 audresample-1.3.1/misc/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 08:16:51.000000 audresample-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-30 08:17:15.286961 audresample-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-30 08:16:51.000000 audresample-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.282961 audresample-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:17:15.286961 audresample-1.3.1/tests/test-assets/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/generate_test_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/original__sr_16000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/original__sr_16000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/original__sr_44100__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/original__sr_44100__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/original__sr_8000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/original__sr_8000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_1.wav
--rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_2.wav
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test_remix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-30 08:16:51.000000 audresample-1.3.1/tests/test_resample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.287020 audresample-1.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.263020 audresample-1.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.271020 audresample-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-30 09:36:01.000000 audresample-1.3.2/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-30 09:36:01.000000 audresample-1.3.2/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-30 09:36:01.000000 audresample-1.3.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-30 09:36:01.000000 audresample-1.3.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 09:36:01.000000 audresample-1.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 09:36:01.000000 audresample-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-30 09:36:01.000000 audresample-1.3.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-30 09:36:01.000000 audresample-1.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-30 09:36:01.000000 audresample-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-30 09:36:22.287020 audresample-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-30 09:36:01.000000 audresample-1.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.271020 audresample-1.3.2/audresample/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-30 09:36:01.000000 audresample-1.3.2/audresample/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.271020 audresample-1.3.2/audresample/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:01.000000 audresample-1.3.2/audresample/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-05-30 09:36:01.000000 audresample-1.3.2/audresample/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.263020 audresample-1.3.2/audresample/core/bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.271020 audresample-1.3.2/audresample/core/bin/macosx_10_4_x86_64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   289712 2023-05-30 09:36:01.000000 audresample-1.3.2/audresample/core/bin/macosx_10_4_x86_64/libaudresample.dylib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.275020 audresample-1.3.2/audresample/core/bin/macosx_11_0_arm64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   206817 2023-05-30 09:36:01.000000 audresample-1.3.2/audresample/core/bin/macosx_11_0_arm64/libaudresample.dylib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.275020 audresample-1.3.2/audresample/core/bin/manylinux_2_17_aarch64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   204120 2023-05-30 09:36:01.000000 audresample-1.3.2/audresample/core/bin/manylinux_2_17_aarch64/libaudresample.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.275020 audresample-1.3.2/audresample/core/bin/manylinux_2_17_armv7l/
+-rw-r--r--   0 runner    (1001) docker     (123)   154436 2023-05-30 09:36:01.000000 audresample-1.3.2/audresample/core/bin/manylinux_2_17_armv7l/libaudresample.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.275020 audresample-1.3.2/audresample/core/bin/manylinux_2_17_x86_64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   290720 2023-05-30 09:36:01.000000 audresample-1.3.2/audresample/core/bin/manylinux_2_17_x86_64/libaudresample.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.275020 audresample-1.3.2/audresample/core/bin/win_amd64/
+-rw-r--r--   0 runner    (1001) docker     (123)   361472 2023-05-30 09:36:01.000000 audresample-1.3.2/audresample/core/bin/win_amd64/audresample.dll
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 09:36:01.000000 audresample-1.3.2/audresample/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-30 09:36:01.000000 audresample-1.3.2/audresample/core/define.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-30 09:36:01.000000 audresample-1.3.2/audresample/core/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.275020 audresample-1.3.2/audresample/define/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 09:36:01.000000 audresample-1.3.2/audresample/define/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.271020 audresample-1.3.2/audresample.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-30 09:36:22.000000 audresample-1.3.2/audresample.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-30 09:36:22.000000 audresample-1.3.2/audresample.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:36:22.000000 audresample-1.3.2/audresample.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 09:36:22.000000 audresample-1.3.2/audresample.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 09:36:22.000000 audresample-1.3.2/audresample.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.279020 audresample-1.3.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.263020 audresample-1.3.2/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.279020 audresample-1.3.2/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 09:36:01.000000 audresample-1.3.2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-30 09:36:01.000000 audresample-1.3.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-30 09:36:01.000000 audresample-1.3.2/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.279020 audresample-1.3.2/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-30 09:36:01.000000 audresample-1.3.2/docs/api-src/audresample.define.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 09:36:01.000000 audresample-1.3.2/docs/api-src/audresample.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 09:36:01.000000 audresample-1.3.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-30 09:36:01.000000 audresample-1.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 09:36:01.000000 audresample-1.3.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 09:36:01.000000 audresample-1.3.2/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-30 09:36:01.000000 audresample-1.3.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-30 09:36:01.000000 audresample-1.3.2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 09:36:01.000000 audresample-1.3.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-30 09:36:01.000000 audresample-1.3.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.279020 audresample-1.3.2/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-30 09:36:01.000000 audresample-1.3.2/misc/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 09:36:01.000000 audresample-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-30 09:36:22.287020 audresample-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-30 09:36:01.000000 audresample-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.279020 audresample-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:22.287020 audresample-1.3.2/tests/test-assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/generate_test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/original__sr_16000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/original__sr_16000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/original__sr_44100__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/original__sr_44100__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/original__sr_8000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/original__sr_8000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    64044 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    88244 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   176444 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test_remix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-30 09:36:01.000000 audresample-1.3.2/tests/test_resample.py
```

### Comparing `audresample-1.3.1/.github/workflows/doc.yml` & `audresample-1.3.2/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/.github/workflows/publish.yml` & `audresample-1.3.2/.github/workflows/publish.yml`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 jobs:
   build:
 
     runs-on: 'ubuntu-latest'
     strategy:
       matrix:
         platform:
-        - macosx_12_0_x86_64
-        - macosx_12_0_arm64
+        - macosx_10_4_x86_64
+        - macosx_11_0_arm64
         - manylinux_2_17_x86_64
         - manylinux_2_17_armv7l
         - manylinux_2_17_aarch64
         - win_amd64
 
     steps:
     - uses: actions/checkout@v3
```

### Comparing `audresample-1.3.1/.github/workflows/test.yml` & `audresample-1.3.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/CHANGELOG.rst` & `audresample-1.3.2/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.3.2 (2023-05-30)
+--------------------------
+
+* Fixed: wrong version
+  in deployed MacOS wheels
+  in the ``publish`` Action on Github
+
+
 Version 1.3.1 (2023-05-30)
 --------------------------
 
 * Fixed: documentation building in deploy step
   of ``publish`` Action on Github
 * Changed: switch versions of MacOS wheel to
   ``macosx_11_0_arm64``,
```

### Comparing `audresample-1.3.1/CONTRIBUTING.rst` & `audresample-1.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/LICENSE` & `audresample-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/PKG-INFO` & `audresample-1.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audresample
-Version: 1.3.1
+Version: 1.3.2
 Summary: Provides functions to resample and remix a signal
 Home-page: https://github.com/audeering/audresample/
 Author: Johannes Wagner, Andrea Crespi, Hagen Wierstorf
 Author-email: jwagner@audeering.com, acrespi@audeering.com, hwierstorf@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audresample/
 Keywords: audio,dsp,resample,remix
@@ -81,14 +81,22 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.3.2 (2023-05-30)
+--------------------------
+
+* Fixed: wrong version
+  in deployed MacOS wheels
+  in the ``publish`` Action on Github
+
+
 Version 1.3.1 (2023-05-30)
 --------------------------
 
 * Fixed: documentation building in deploy step
   of ``publish`` Action on Github
 * Changed: switch versions of MacOS wheel to
   ``macosx_11_0_arm64``,
```

### Comparing `audresample-1.3.1/README.rst` & `audresample-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/audresample/core/api.py` & `audresample-1.3.2/audresample/core/api.py`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/audresample/core/bin/macosx_10_4_x86_64/libaudresample.dylib` & `audresample-1.3.2/audresample/core/bin/macosx_10_4_x86_64/libaudresample.dylib`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/audresample/core/bin/macosx_11_0_arm64/libaudresample.dylib` & `audresample-1.3.2/audresample/core/bin/macosx_11_0_arm64/libaudresample.dylib`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/audresample/core/bin/manylinux_2_17_aarch64/libaudresample.so` & `audresample-1.3.2/audresample/core/bin/manylinux_2_17_aarch64/libaudresample.so`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/audresample/core/bin/manylinux_2_17_armv7l/libaudresample.so` & `audresample-1.3.2/audresample/core/bin/manylinux_2_17_armv7l/libaudresample.so`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/audresample/core/bin/manylinux_2_17_x86_64/libaudresample.so` & `audresample-1.3.2/audresample/core/bin/manylinux_2_17_x86_64/libaudresample.so`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/audresample/core/bin/win_amd64/audresample.dll` & `audresample-1.3.2/audresample/core/bin/win_amd64/audresample.dll`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/audresample/core/lib.py` & `audresample-1.3.2/audresample/core/lib.py`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/audresample.egg-info/PKG-INFO` & `audresample-1.3.2/audresample.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audresample
-Version: 1.3.1
+Version: 1.3.2
 Summary: Provides functions to resample and remix a signal
 Home-page: https://github.com/audeering/audresample/
 Author: Johannes Wagner, Andrea Crespi, Hagen Wierstorf
 Author-email: jwagner@audeering.com, acrespi@audeering.com, hwierstorf@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audresample/
 Keywords: audio,dsp,resample,remix
@@ -81,14 +81,22 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.3.2 (2023-05-30)
+--------------------------
+
+* Fixed: wrong version
+  in deployed MacOS wheels
+  in the ``publish`` Action on Github
+
+
 Version 1.3.1 (2023-05-30)
 --------------------------
 
 * Fixed: documentation building in deploy step
   of ``publish`` Action on Github
 * Changed: switch versions of MacOS wheel to
   ``macosx_11_0_arm64``,
```

### Comparing `audresample-1.3.1/audresample.egg-info/SOURCES.txt` & `audresample-1.3.2/audresample.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/docs/_templates/autosummary/class.rst` & `audresample-1.3.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/docs/conf.py` & `audresample-1.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/docs/index.rst` & `audresample-1.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/docs/usage.rst` & `audresample-1.3.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/misc/icon.png` & `audresample-1.3.2/misc/icon.png`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/setup.cfg` & `audresample-1.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/setup.py` & `audresample-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/generate_test_assets.py` & `audresample-1.3.2/tests/test-assets/generate_test_assets.py`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/original__sr_16000__channels_1.wav` & `audresample-1.3.2/tests/test-assets/original__sr_16000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/original__sr_16000__channels_2.wav` & `audresample-1.3.2/tests/test-assets/original__sr_16000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/original__sr_44100__channels_1.wav` & `audresample-1.3.2/tests/test-assets/original__sr_44100__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/original__sr_44100__channels_2.wav` & `audresample-1.3.2/tests/test-assets/original__sr_44100__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/original__sr_8000__channels_1.wav` & `audresample-1.3.2/tests/test-assets/original__sr_8000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/original__sr_8000__channels_2.wav` & `audresample-1.3.2/tests/test-assets/original__sr_8000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_1.wav` & `audresample-1.3.2/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_2.wav` & `audresample-1.3.2/tests/test-assets/resampled__sr-in_16000__sr-out_44100__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_1.wav` & `audresample-1.3.2/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_2.wav` & `audresample-1.3.2/tests/test-assets/resampled__sr-in_16000__sr-out_8000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_1.wav` & `audresample-1.3.2/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_2.wav` & `audresample-1.3.2/tests/test-assets/resampled__sr-in_44100__sr-out_16000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_1.wav` & `audresample-1.3.2/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_2.wav` & `audresample-1.3.2/tests/test-assets/resampled__sr-in_44100__sr-out_8000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_1.wav` & `audresample-1.3.2/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_2.wav` & `audresample-1.3.2/tests/test-assets/resampled__sr-in_8000__sr-out_16000__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_1.wav` & `audresample-1.3.2/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_1.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_2.wav` & `audresample-1.3.2/tests/test-assets/resampled__sr-in_8000__sr-out_44100__channels_2.wav`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test_remix.py` & `audresample-1.3.2/tests/test_remix.py`

 * *Files identical despite different names*

### Comparing `audresample-1.3.1/tests/test_resample.py` & `audresample-1.3.2/tests/test_resample.py`

 * *Files identical despite different names*

