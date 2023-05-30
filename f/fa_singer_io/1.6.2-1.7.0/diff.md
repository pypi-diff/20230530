# Comparing `tmp/fa_singer_io-1.6.2.tar.gz` & `tmp/fa_singer_io-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa_singer_io-1.6.2.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
+gzip compressed data, was "fa_singer_io-1.7.0.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
```

## Comparing `fa_singer_io-1.6.2.tar` & `fa_singer_io-1.7.0.tar`

### file list

```diff
@@ -1,63 +1,67 @@
--rw-r--r--   0        0        0       85 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/.envrc
--rw-r--r--   0        0        0       59 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/.gitignore
--rw-r--r--   0        0        0     2300 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/.gitlab-ci.yml
--rw-r--r--   0        0        0      797 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/arch.cfg
--rw-r--r--   0        0        0      340 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/arch_test.cfg
--rw-r--r--   0        0        0      262 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/ci/check.nix
--rw-r--r--   0        0        0      191 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/ci/utils.sh
--rw-r--r--   0        0        0     1450 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/default.nix
--rw-r--r--   0        0        0     1376 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/deps/default.nix
--rw-r--r--   0        0        0      579 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/deps/import-linter/default.nix
--rw-r--r--   0        0        0      209 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/deps/jsonschema/stubs.nix
--rw-r--r--   0        0        0      251 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/deps/networkx.nix
--rw-r--r--   0        0        0     1767 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/deps/override_utils.nix
--rw-r--r--   0        0        0      208 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/deps/pyRFC3339/stubs.nix
--rw-r--r--   0        0        0      602 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/pkg/build.nix
--rwxr-xr-x   0        0        0      200 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/pkg/check/arch.sh
--rwxr-xr-x   0        0        0      127 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/pkg/check/tests.sh
--rwxr-xr-x   0        0        0      135 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/pkg/check/types.sh
--rw-r--r--   0        0        0      687 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/pkg/default.nix
--rw-r--r--   0        0        0      100 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/build/publish/default.nix
--rw-r--r--   0        0        0       22 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/__init__.py
--rw-r--r--   0        0        0      179 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/json_schema/__init__.py
--rw-r--r--   0        0        0     3246 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/json_schema/_factory.py
--rw-r--r--   0        0        0      274 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/json_schema/_inner.py
--rw-r--r--   0        0        0      701 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/json_schema/core.py
--rw-r--r--   0        0        0      550 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/json_schema/factory.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/py.typed
--rw-r--r--   0        0        0      354 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/__init__.py
--rw-r--r--   0        0        0      461 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/_utils.py
--rw-r--r--   0        0        0     2348 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/deserializer.py
--rw-r--r--   0        0        0      956 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/emitter.py
--rw-r--r--   0        0        0     2299 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/encoder.py
--rw-r--r--   0        0        0      177 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/errors.py
--rw-r--r--   0        0        0       75 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/record/__init__.py
--rw-r--r--   0        0        0      301 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/record/core.py
--rw-r--r--   0        0        0     1534 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/record/decoder.py
--rw-r--r--   0        0        0      698 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/record/encode.py
--rw-r--r--   0        0        0      288 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/record/factory.py
--rw-r--r--   0        0        0       75 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/schema/__init__.py
--rw-r--r--   0        0        0     3187 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/schema/core.py
--rw-r--r--   0        0        0     1827 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/schema/decoder.py
--rw-r--r--   0        0        0      921 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/schema/encode.py
--rw-r--r--   0        0        0      256 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/schema/factory.py
--rw-r--r--   0        0        0       73 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/state/__init__.py
--rw-r--r--   0        0        0      146 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/state/core.py
--rw-r--r--   0        0        0     1125 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/state/decoder.py
--rw-r--r--   0        0        0      324 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/state/encode.py
--rw-r--r--   0        0        0      325 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/singer/validate.py
--rw-r--r--   0        0        0     1451 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/fa_singer_io/time.py
--rw-r--r--   0        0        0     1596 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/flake.lock
--rw-r--r--   0        0        0     1088 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/flake.nix
--rw-r--r--   0        0        0      122 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/makes.lock.nix
--rw-r--r--   0        0        0      705 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/makes.nix
--rw-r--r--   0        0        0      740 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/mypy.ini
--rw-r--r--   0        0        0      260 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/nix.conf
--rw-r--r--   0        0        0      513 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/tests/__init__.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/tests/py.typed
--rw-r--r--   0        0        0     1207 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/tests/test_json_schema.py
--rw-r--r--   0        0        0      593 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/tests/test_record.py
--rw-r--r--   0        0        0      726 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/tests/test_schema.py
--rw-r--r--   0        0        0      459 1980-01-01 00:00:00.000000 fa_singer_io-1.6.2/tests/test_state.py
--rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 fa_singer_io-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0       83 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/.envrc
+-rw-r--r--   0        0        0       59 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/.gitignore
+-rw-r--r--   0        0        0     1976 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      262 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/ci/check.nix
+-rw-r--r--   0        0        0      191 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/ci/utils.sh
+-rw-r--r--   0        0        0      779 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/default.nix
+-rw-r--r--   0        0        0     1155 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/deps/default.nix
+-rw-r--r--   0        0        0      209 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/deps/jsonschema/stubs.nix
+-rw-r--r--   0        0        0      251 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/deps/networkx.nix
+-rw-r--r--   0        0        0     1368 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/deps/override_utils.nix
+-rw-r--r--   0        0        0      208 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/deps/pyRFC3339/stubs.nix
+-rw-r--r--   0        0        0      182 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/dev_env/default.nix
+-rwxr-xr-x   0        0        0      131 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/dev_env/hook.sh
+-rw-r--r--   0        0        0     1482 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/dev_env/vs_settings.py
+-rw-r--r--   0        0        0      210 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/generic_builder/check.nix
+-rw-r--r--   0        0        0      341 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/generic_builder/default.nix
+-rw-r--r--   0        0        0      245 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/generic_builder/env.nix
+-rw-r--r--   0        0        0      309 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/generic_builder/metadata.nix
+-rwxr-xr-x   0        0        0      127 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/generic_builder/pkg/check/tests.sh
+-rwxr-xr-x   0        0        0      160 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/generic_builder/pkg/check/types.sh
+-rw-r--r--   0        0        0      623 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/build/generic_builder/pkg/default.nix
+-rw-r--r--   0        0        0       22 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/__init__.py
+-rw-r--r--   0        0        0      179 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/json_schema/__init__.py
+-rw-r--r--   0        0        0     3246 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/json_schema/_factory.py
+-rw-r--r--   0        0        0      274 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/json_schema/_inner.py
+-rw-r--r--   0        0        0      701 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/json_schema/core.py
+-rw-r--r--   0        0        0      550 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/json_schema/factory.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/py.typed
+-rw-r--r--   0        0        0      354 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/__init__.py
+-rw-r--r--   0        0        0      461 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/_utils.py
+-rw-r--r--   0        0        0     2348 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/deserializer.py
+-rw-r--r--   0        0        0      956 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/emitter.py
+-rw-r--r--   0        0        0     2299 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/encoder.py
+-rw-r--r--   0        0        0      177 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/errors.py
+-rw-r--r--   0        0        0       75 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/record/__init__.py
+-rw-r--r--   0        0        0      301 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/record/core.py
+-rw-r--r--   0        0        0     1534 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/record/decoder.py
+-rw-r--r--   0        0        0      698 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/record/encode.py
+-rw-r--r--   0        0        0      288 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/record/factory.py
+-rw-r--r--   0        0        0       75 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/schema/__init__.py
+-rw-r--r--   0        0        0     3187 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/schema/core.py
+-rw-r--r--   0        0        0     1827 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/schema/decoder.py
+-rw-r--r--   0        0        0      921 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/schema/encode.py
+-rw-r--r--   0        0        0      256 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/schema/factory.py
+-rw-r--r--   0        0        0       73 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/state/__init__.py
+-rw-r--r--   0        0        0      146 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/state/core.py
+-rw-r--r--   0        0        0     1125 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/state/decoder.py
+-rw-r--r--   0        0        0      324 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/state/encode.py
+-rw-r--r--   0        0        0      325 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/singer/validate.py
+-rw-r--r--   0        0        0     1451 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/fa_singer_io/time.py
+-rw-r--r--   0        0        0     2626 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/flake.lock
+-rw-r--r--   0        0        0     1725 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/flake.nix
+-rw-r--r--   0        0        0      122 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/makes.lock.nix
+-rw-r--r--   0        0        0      705 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/makes.nix
+-rw-r--r--   0        0        0      740 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/mypy.ini
+-rw-r--r--   0        0        0      260 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/nix.conf
+-rw-r--r--   0        0        0      513 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/tests/arch/__init__.py
+-rw-r--r--   0        0        0     1471 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/tests/arch/arch.py
+-rw-r--r--   0        0        0     1052 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/tests/arch/test_arch.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/tests/py.typed
+-rw-r--r--   0        0        0     1207 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/tests/test_json_schema.py
+-rw-r--r--   0        0        0      593 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/tests/test_record.py
+-rw-r--r--   0        0        0      726 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/tests/test_schema.py
+-rw-r--r--   0        0        0      459 1980-01-01 00:00:00.000000 fa_singer_io-1.7.0/tests/test_state.py
+-rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 fa_singer_io-1.7.0/PKG-INFO
```

### Comparing `fa_singer_io-1.6.2/.gitlab-ci.yml` & `fa_singer_io-1.7.0/.gitlab-ci.yml`

 * *Files 22% similar despite different names*

```diff
@@ -57,60 +57,39 @@
 
 lint-bash:
   image: ghcr.io/fluidattacks/makes:21.11
   stage: lint
   <<: *in_dev_branch
   script: m . /formatBash && m . /lintBash
 
-build-runtime-env:
+build-for-python39:
   <<: *with_nix
   <<: *in_dev_branch
   stage: build
   script:
-    - build ".#python38.env.runtime"
+    - build ".#python39.pkg"
 
-build-dev-env:
+build-for-python310:
   <<: *with_nix
   <<: *in_dev_branch
   stage: build
   script:
-    - build ".#python38.env.dev"
+    - build ".#python310.pkg"
 
-arch-check:
+build-for-python311:
   <<: *with_nix
   <<: *in_dev_branch
-  stage: test
-  script:
-    - build ".#python38.check.arch"
-
-test-check:
-  <<: *with_nix
-  <<: *in_dev_branch
-  stage: test
-  script:
-    - build ".#python38.check.tests"
-
-type-check:
-  <<: *with_nix
-  <<: *in_dev_branch
-  stage: test
-  script:
-    - build ".#python38.check.types"
-
-build-for-min-python:
-  <<: *with_nix
-  <<: *new_version
   stage: build
   script:
-    - build ".#python38.pkg"
+    - build ".#python311.pkg"
 
 deploy-to-pypi:
   <<: *with_nix
   <<: *new_version
   stage: deploy
   script:
     - src=$(pwd)
     - nix develop -i
       -k FLIT_USERNAME
       -k FLIT_PASSWORD
-      ".#publish" -c
+      ".#python311.publish" -c
         flit -f "${src}/pyproject.toml" publish
```

### Comparing `fa_singer_io-1.6.2/build/deps/default.nix` & `fa_singer_io-1.7.0/build/deps/default.nix`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 {
-  lib,
-  python_pkgs,
+  nixpkgs,
+  python_version,
 }: let
+  lib = {
+    buildEnv = nixpkgs."${python_version}".buildEnv.override;
+    inherit (nixpkgs."${python_version}".pkgs) buildPythonPackage;
+    inherit (nixpkgs.python3Packages) fetchPypi;
+  };
+
   utils = import ./override_utils.nix;
   pkgs_overrides = override: python_pkgs: builtins.mapAttrs (_: override python_pkgs) python_pkgs;
 
   layer_1 = python_pkgs:
     python_pkgs
     // {
-      import-linter = import ./import-linter {
-        inherit lib;
-        click = python_pkgs.click;
-        networkx = python_pkgs.networkx;
-      };
-      jsonschema = python_pkgs.jsonschema.overridePythonAttrs (
-        old: rec {
-          version = "3.2.0";
-          SETUPTOOLS_SCM_PRETEND_VERSION = version;
-          src = lib.fetchPypi {
-            inherit version;
-            pname = old.pname;
-            sha256 = "yKhbKNN3zHc35G4tnytPRO48Dh3qxr9G3e/HGH0weXo=";
-          };
-          doCheck = false;
-        }
-      );
-      pyrsistent = python_pkgs.pyrsistent.overridePythonAttrs (
-        _: {doCheck = false;}
-      );
+      arch-lint = nixpkgs.arch-lint."${python_version}".pkg;
+      purity = nixpkgs.purity."${python_version}".pkg;
       types-jsonschema = import ./jsonschema/stubs.nix lib;
       types-pyRFC3339 = import ./pyRFC3339/stubs.nix lib;
     };
 
-  pyrsistent_override = python_pkgs: utils.replace_pkg ["pyrsistent"] python_pkgs.pyrsistent;
+  pyrsistent_override = python_pkgs:
+    utils.replace_pkg ["pyrsistent"] (
+      python_pkgs.pyrsistent.overridePythonAttrs (
+        _: {doCheck = false;}
+      )
+    );
   networkx_override = python_pkgs: utils.replace_pkg ["networkx"] (import ./networkx.nix lib python_pkgs);
   overrides = map pkgs_overrides [
     pyrsistent_override
     networkx_override
   ];
 
-  final_pkgs = utils.compose ([layer_1] ++ overrides) python_pkgs;
+  python_pkgs = utils.compose ([layer_1] ++ overrides) nixpkgs."${python_version}Packages";
 in {
-  python_pkgs = final_pkgs;
+  inherit lib python_pkgs;
 }
```

### Comparing `fa_singer_io-1.6.2/build/deps/override_utils.nix` & `fa_singer_io-1.7.0/build/deps/override_utils.nix`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             if builtins.isList value
             then map self value
             else self value)
         )
       else pkg;
 
   # no_check_override: Derivation -> Derivation
-  no_check_override = recursive_python_pkg_override (pkg: pkg ? overridePythonAttrs) (
+  no_check_override = recursive_python_pkg_override (pkg: pkg ? overridePythonAttrs && pkg ? pname) (
     pkg:
       pkg.overridePythonAttrs (
         old:
           (
             builtins.mapAttrs (_: value:
               if builtins.isList value
               then map no_check_override value
@@ -36,28 +36,11 @@
   );
 
   # replace_pkg: List[str] -> Derivation -> Derivation
   replace_pkg = names: new_pkg:
     recursive_python_pkg_override (
       x: x ? overridePythonAttrs && x ? pname && builtins.elem x.pname names
     ) (_: new_pkg);
-
-  pkg_override = is_pkg: new_pkg: let
-    override = x:
-      if is_pkg x
-      then new_pkg
-      else pkg_override is_pkg new_pkg x;
-  in
-    pkg:
-      if pkg ? overridePythonAttrs
-      then
-        pkg.overridePythonAttrs (
-          builtins.mapAttrs (_: value:
-            if builtins.isList value
-            then map override value
-            else override value)
-        )
-      else pkg;
 in {
-  inherit recursive_python_pkg_override no_check_override replace_pkg pkg_override;
+  inherit recursive_python_pkg_override no_check_override replace_pkg;
   compose = functions: val: builtins.foldl' (x: f: f x) val functions;
 }
```

### Comparing `fa_singer_io-1.6.2/fa_singer_io/json_schema/_factory.py` & `fa_singer_io-1.7.0/fa_singer_io/json_schema/_factory.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/fa_singer_io/json_schema/core.py` & `fa_singer_io-1.7.0/fa_singer_io/json_schema/core.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/fa_singer_io/json_schema/factory.py` & `fa_singer_io-1.7.0/fa_singer_io/json_schema/factory.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/fa_singer_io/singer/deserializer.py` & `fa_singer_io-1.7.0/fa_singer_io/singer/deserializer.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/fa_singer_io/singer/emitter.py` & `fa_singer_io-1.7.0/fa_singer_io/singer/emitter.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/fa_singer_io/singer/encoder.py` & `fa_singer_io-1.7.0/fa_singer_io/singer/encoder.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/fa_singer_io/singer/record/decoder.py` & `fa_singer_io-1.7.0/fa_singer_io/singer/record/decoder.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/fa_singer_io/singer/record/encode.py` & `fa_singer_io-1.7.0/fa_singer_io/singer/record/encode.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/fa_singer_io/singer/schema/core.py` & `fa_singer_io-1.7.0/fa_singer_io/singer/schema/core.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/fa_singer_io/singer/schema/decoder.py` & `fa_singer_io-1.7.0/fa_singer_io/singer/schema/decoder.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/fa_singer_io/singer/schema/encode.py` & `fa_singer_io-1.7.0/fa_singer_io/singer/schema/encode.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/fa_singer_io/singer/state/decoder.py` & `fa_singer_io-1.7.0/fa_singer_io/singer/state/decoder.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/fa_singer_io/time.py` & `fa_singer_io-1.7.0/fa_singer_io/time.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/flake.lock` & `fa_singer_io-1.7.0/flake.lock`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9389467592592592%*

 * *Differences: {"'nodes'": "{'nixpkgs': {'locked': {'lastModified': 1679793451, 'narHash': "*

 * *            "'sha256-JafTtgMDATE8dZOImBhWMA9RCn9AP8FVOpN+9K/tTlg=', 'rev': "*

 * *            "'0cd51a933d91078775b300cf0f29aa3495231aa2'}, 'original': {'rev': "*

 * *            "'0cd51a933d91078775b300cf0f29aa3495231aa2'}}, 'purity': {'locked': {'lastModified': "*

 * *            "1685212251, 'narHash': 'sha256-b/2MMuPOFcfgyJpoGJg/71lNMUhoLiv3lpN3MUAH4Ag=', 'rev': "*

 * *            "'feaa69ef3ad93ad91fd679d8169c80458457d779'}, 'original': {delete: […]*

```diff
@@ -1,9 +1,30 @@
 {
     "nodes": {
+        "arch-lint": {
+            "inputs": {
+                "nix_filter": "nix_filter",
+                "nixpkgs": [
+                    "nixpkgs"
+                ]
+            },
+            "locked": {
+                "lastModified": 1685371599,
+                "narHash": "sha256-DcOPPeAKrjdev/2K1o3pnZUL2+nggMmqa6uJ5An9IxA=",
+                "owner": "dmurciaatfluid",
+                "repo": "arch_lint",
+                "rev": "72a495bb933f052ad812292b468ca3e18fd9dde4",
+                "type": "gitlab"
+            },
+            "original": {
+                "owner": "dmurciaatfluid",
+                "repo": "arch_lint",
+                "type": "gitlab"
+            }
+        },
         "nix_filter": {
             "locked": {
                 "lastModified": 1645371475,
                 "narHash": "sha256-z2n0y5ME7yQTqzzGWnQTVd1MG5Bp1E+of7ZgA861/9E=",
                 "owner": "numtide",
                 "repo": "nix-filter",
                 "rev": "38bc843f1ce76958a9f6f0a1e4e3455221c8ecf6",
@@ -11,56 +32,72 @@
             },
             "original": {
                 "owner": "numtide",
                 "repo": "nix-filter",
                 "type": "github"
             }
         },
+        "nix_filter_2": {
+            "locked": {
+                "lastModified": 1645371475,
+                "narHash": "sha256-z2n0y5ME7yQTqzzGWnQTVd1MG5Bp1E+of7ZgA861/9E=",
+                "owner": "numtide",
+                "repo": "nix-filter",
+                "rev": "38bc843f1ce76958a9f6f0a1e4e3455221c8ecf6",
+                "type": "github"
+            },
+            "original": {
+                "owner": "numtide",
+                "repo": "nix-filter",
+                "type": "github"
+            }
+        },
         "nixpkgs": {
             "locked": {
-                "lastModified": 1679002176,
-                "narHash": "sha256-MgcwKHS1DIw0zKu8Y6u2MVnkh9GpKWVY7I7ZcyXWodY=",
+                "lastModified": 1679793451,
+                "narHash": "sha256-JafTtgMDATE8dZOImBhWMA9RCn9AP8FVOpN+9K/tTlg=",
                 "owner": "nixos",
                 "repo": "nixpkgs",
-                "rev": "421cfe4e7e1a5f91eddd1cf6a86574f8e9c8136e",
+                "rev": "0cd51a933d91078775b300cf0f29aa3495231aa2",
                 "type": "github"
             },
             "original": {
                 "owner": "nixos",
                 "repo": "nixpkgs",
+                "rev": "0cd51a933d91078775b300cf0f29aa3495231aa2",
                 "type": "github"
             }
         },
         "purity": {
             "inputs": {
                 "nix_filter": [
                     "nix_filter"
                 ],
                 "nixpkgs": [
                     "nixpkgs"
                 ]
             },
             "locked": {
-                "lastModified": 1679416217,
-                "narHash": "sha256-bEbIxdPS7IC5wMbHn9zOrkP7m4XOL25XAyWwXGTh/ZU=",
+                "lastModified": 1685212251,
+                "narHash": "sha256-b/2MMuPOFcfgyJpoGJg/71lNMUhoLiv3lpN3MUAH4Ag=",
                 "owner": "dmurciaatfluid",
                 "repo": "purity",
-                "rev": "a2fba10724f6062976d3bb3ae5a40f0addd959a5",
+                "rev": "feaa69ef3ad93ad91fd679d8169c80458457d779",
                 "type": "gitlab"
             },
             "original": {
                 "owner": "dmurciaatfluid",
-                "ref": "v1.31.0",
                 "repo": "purity",
                 "type": "gitlab"
             }
         },
         "root": {
             "inputs": {
-                "nix_filter": "nix_filter",
+                "arch-lint": "arch-lint",
+                "nix_filter": "nix_filter_2",
                 "nixpkgs": "nixpkgs",
                 "purity": "purity"
             }
         }
     },
     "root": "root",
     "version": 7
```

### Comparing `fa_singer_io-1.6.2/makes.nix` & `fa_singer_io-1.7.0/makes.nix`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/mypy.ini` & `fa_singer_io-1.7.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/pyproject.toml` & `fa_singer_io-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 name = "fa_singer_io"
 authors = [
     {name = "Product Team", email = "development@fluidattacks.com"},
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = [
     "fa-purity >=1.31.0, <2.0.0",
     "Deprecated >=1.2.12, <2.0.0",
-    "jsonschema >=3.2.0, <4.0.0",
+    "jsonschema >=3.2.0, <5.0.0",
     "pyRFC3339 >=1.1, <2.0",
 ]
 description = "Singer io SDK with strict types"
 dynamic = ["version"]
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
```

### Comparing `fa_singer_io-1.6.2/tests/test_json_schema.py` & `fa_singer_io-1.7.0/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/tests/test_record.py` & `fa_singer_io-1.7.0/tests/test_record.py`

 * *Files identical despite different names*

### Comparing `fa_singer_io-1.6.2/tests/test_schema.py` & `fa_singer_io-1.7.0/tests/test_schema.py`

 * *Files identical despite different names*

