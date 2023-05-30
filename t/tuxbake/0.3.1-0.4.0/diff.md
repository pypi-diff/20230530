# Comparing `tmp/tuxbake-0.3.1.tar.gz` & `tmp/tuxbake-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuxbake-0.3.1.tar", last modified: Mon Feb 27 09:56:29 2023, max compression
+gzip compressed data, was "tuxbake-0.4.0.tar", last modified: Tue May 30 12:51:27 2023, max compression
```

## Comparing `tuxbake-0.3.1.tar` & `tuxbake-0.4.0.tar`

### file list

```diff
@@ -1,57 +1,65 @@
--rw-r--r--   0        0        0       50 2023-02-27 09:56:27.370999 tuxbake-0.3.1/.gitignore
--rw-r--r--   0        0        0     2420 2023-02-27 09:56:27.370999 tuxbake-0.3.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      879 2023-02-27 09:56:27.370999 tuxbake-0.3.1/Dockerfile.ci-debian
--rw-r--r--   0        0        0      555 2023-02-27 09:56:27.370999 tuxbake-0.3.1/Dockerfile.ci-fedora
--rw-r--r--   0        0        0     1054 2023-02-27 09:56:27.370999 tuxbake-0.3.1/LICENSE
--rw-r--r--   0        0        0     1211 2023-02-27 09:56:27.370999 tuxbake-0.3.1/Makefile
--rw-r--r--   0        0        0     4869 2023-02-27 09:56:27.370999 tuxbake-0.3.1/README.md
--rw-r--r--   0        0        0      141 2023-02-27 09:56:27.370999 tuxbake-0.3.1/debian/changelog
--rw-r--r--   0        0        0      640 2023-02-27 09:56:27.370999 tuxbake-0.3.1/debian/control
--rw-r--r--   0        0        0      100 2023-02-27 09:56:27.370999 tuxbake-0.3.1/debian/gbp.conf
--rwxr-xr-x   0        0        0      594 2023-02-27 09:56:27.370999 tuxbake-0.3.1/debian/rules
--rw-r--r--   0        0        0       12 2023-02-27 09:56:27.370999 tuxbake-0.3.1/debian/source/format
--rw-r--r--   0        0        0     1051 2023-02-27 09:56:27.370999 tuxbake-0.3.1/dockerfiles/Makefile
--rw-r--r--   0        0        0     1485 2023-02-27 09:56:27.370999 tuxbake-0.3.1/dockerfiles/centos-7/Dockerfile
--rw-r--r--   0        0        0     1838 2023-02-27 09:56:27.370999 tuxbake-0.3.1/dockerfiles/centos-8/Dockerfile
--rw-r--r--   0        0        0     1823 2023-02-27 09:56:27.371999 tuxbake-0.3.1/dockerfiles/debian-bullseye/Dockerfile
--rw-r--r--   0        0        0     1821 2023-02-27 09:56:27.371999 tuxbake-0.3.1/dockerfiles/debian-buster/Dockerfile
--rw-r--r--   0        0        0     2259 2023-02-27 09:56:27.371999 tuxbake-0.3.1/dockerfiles/debian-stretch/Dockerfile
--rw-r--r--   0        0        0     1803 2023-02-27 09:56:27.371999 tuxbake-0.3.1/dockerfiles/fedora-33/Dockerfile
--rw-r--r--   0        0        0     1714 2023-02-27 09:56:27.371999 tuxbake-0.3.1/dockerfiles/fedora-34/Dockerfile
--rw-r--r--   0        0        0     1535 2023-02-27 09:56:27.371999 tuxbake-0.3.1/dockerfiles/opensuse-leap-15.1/Dockerfile
--rw-r--r--   0        0        0     1535 2023-02-27 09:56:27.371999 tuxbake-0.3.1/dockerfiles/opensuse-leap-15.2/Dockerfile
--rw-r--r--   0        0        0     1564 2023-02-27 09:56:27.371999 tuxbake-0.3.1/dockerfiles/ubuntu-16.04/Dockerfile
--rw-r--r--   0        0        0     1631 2023-02-27 09:56:27.371999 tuxbake-0.3.1/dockerfiles/ubuntu-18.04/Dockerfile
--rw-r--r--   0        0        0     1631 2023-02-27 09:56:27.371999 tuxbake-0.3.1/dockerfiles/ubuntu-20.04/Dockerfile
--rw-r--r--   0        0        0     1631 2023-02-27 09:56:27.371999 tuxbake-0.3.1/dockerfiles/ubuntu-22.04/Dockerfile
--rw-r--r--   0        0        0       76 2023-02-27 09:56:27.371999 tuxbake-0.3.1/examples/README.md
--rw-r--r--   0        0        0      416 2023-02-27 09:56:27.371999 tuxbake-0.3.1/examples/demo.json
--rw-r--r--   0        0        0      314 2023-02-27 09:56:27.371999 tuxbake-0.3.1/examples/ledge-rpb.json
--rw-r--r--   0        0        0      894 2023-02-27 09:56:27.371999 tuxbake-0.3.1/examples/lkft.json
--rw-r--r--   0        0        0      496 2023-02-27 09:56:27.371999 tuxbake-0.3.1/examples/lt-qcom.json
--rw-r--r--   0        0        0      387 2023-02-27 09:56:27.371999 tuxbake-0.3.1/examples/oe-rpb.json
--rw-r--r--   0        0        0      409 2023-02-27 09:56:27.371999 tuxbake-0.3.1/examples/oniro.json
--rw-r--r--   0        0        0      387 2023-02-27 09:56:27.371999 tuxbake-0.3.1/examples/qcom-rpb-dunfell.json
--rw-r--r--   0        0        0      388 2023-02-27 09:56:27.371999 tuxbake-0.3.1/examples/qcom-rpb-honister.json
--rw-r--r--   0        0        0      684 2023-02-27 09:56:27.371999 tuxbake-0.3.1/examples/template.json
--rw-r--r--   0        0        0      325 2023-02-27 09:56:27.371999 tuxbake-0.3.1/examples/yocto.json
--rw-r--r--   0        0        0      424 2023-02-27 09:56:27.372999 tuxbake-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       38 2023-02-27 09:56:27.372999 tuxbake-0.3.1/requirements-dev.txt
--rw-r--r--   0        0        0   594416 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tests/unit/bitbake-environment
--rw-r--r--   0        0        0     5957 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tests/unit/conftest.py
--rw-r--r--   0        0        0      204 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tests/unit/test.xml
--rw-r--r--   0        0        0     1369 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tests/unit/test_argparse.py
--rw-r--r--   0        0        0      661 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tests/unit/test_build.py
--rw-r--r--   0        0        0     9749 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tests/unit/test_models.py
--rw-r--r--   0        0        0     4813 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tests/unit/test_utils.py
--rw-r--r--   0        0        0     1350 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tuxbake.spec
--rw-r--r--   0        0        0      112 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tuxbake/__init__.py
--rw-r--r--   0        0        0     1909 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tuxbake/__main__.py
--rw-r--r--   0        0        0     2984 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tuxbake/argparse.py
--rw-r--r--   0        0        0      561 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tuxbake/build.py
--rw-r--r--   0        0        0      493 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tuxbake/exceptions.py
--rw-r--r--   0        0        0     5018 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tuxbake/helper.py
--rw-r--r--   0        0        0    14920 2023-02-27 09:56:27.374999 tuxbake-0.3.1/tuxbake/models.py
--rw-r--r--   0        0        0     6154 2023-02-27 09:56:27.375999 tuxbake-0.3.1/tuxbake/utils.py
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 tuxbake-0.3.1/setup.py
--rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 tuxbake-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-05-30 12:51:25.692838 tuxbake-0.4.0/.gitignore
+-rw-r--r--   0        0        0     2767 2023-05-30 12:51:25.692838 tuxbake-0.4.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      879 2023-05-30 12:51:25.692838 tuxbake-0.4.0/Dockerfile.ci-debian
+-rw-r--r--   0        0        0      555 2023-05-30 12:51:25.692838 tuxbake-0.4.0/Dockerfile.ci-fedora
+-rw-r--r--   0        0        0     1054 2023-05-30 12:51:25.692838 tuxbake-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1211 2023-05-30 12:51:25.692838 tuxbake-0.4.0/Makefile
+-rw-r--r--   0        0        0     4869 2023-05-30 12:51:25.692838 tuxbake-0.4.0/README.md
+-rw-r--r--   0        0        0      141 2023-05-30 12:51:25.692838 tuxbake-0.4.0/debian/changelog
+-rw-r--r--   0        0        0      700 2023-05-30 12:51:25.692838 tuxbake-0.4.0/debian/control
+-rw-r--r--   0        0        0      100 2023-05-30 12:51:25.692838 tuxbake-0.4.0/debian/gbp.conf
+-rwxr-xr-x   0        0        0      594 2023-05-30 12:51:25.692838 tuxbake-0.4.0/debian/rules
+-rw-r--r--   0        0        0       12 2023-05-30 12:51:25.692838 tuxbake-0.4.0/debian/source/format
+-rw-r--r--   0        0        0     1051 2023-05-30 12:51:25.692838 tuxbake-0.4.0/dockerfiles/Makefile
+-rw-r--r--   0        0        0     1485 2023-05-30 12:51:25.692838 tuxbake-0.4.0/dockerfiles/centos-7/Dockerfile
+-rw-r--r--   0        0        0     1838 2023-05-30 12:51:25.692838 tuxbake-0.4.0/dockerfiles/centos-8/Dockerfile
+-rw-r--r--   0        0        0     1823 2023-05-30 12:51:25.692838 tuxbake-0.4.0/dockerfiles/debian-bullseye/Dockerfile
+-rw-r--r--   0        0        0     1821 2023-05-30 12:51:25.692838 tuxbake-0.4.0/dockerfiles/debian-buster/Dockerfile
+-rw-r--r--   0        0        0     2259 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/debian-stretch/Dockerfile
+-rw-r--r--   0        0        0     1803 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/fedora-33/Dockerfile
+-rw-r--r--   0        0        0     1714 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/fedora-34/Dockerfile
+-rw-r--r--   0        0        0     1535 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/opensuse-leap-15.1/Dockerfile
+-rw-r--r--   0        0        0     1535 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/opensuse-leap-15.2/Dockerfile
+-rw-r--r--   0        0        0     1564 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/ubuntu-16.04/Dockerfile
+-rw-r--r--   0        0        0     1631 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/ubuntu-18.04/Dockerfile
+-rw-r--r--   0        0        0     1631 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/ubuntu-20.04/Dockerfile
+-rw-r--r--   0        0        0     1631 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/ubuntu-22.04/Dockerfile
+-rw-r--r--   0        0        0       76 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/README.md
+-rw-r--r--   0        0        0      416 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/demo.json
+-rw-r--r--   0        0        0      314 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/ledge-rpb.json
+-rw-r--r--   0        0        0      894 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/lkft.json
+-rw-r--r--   0        0        0      495 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/lt-qcom.json
+-rw-r--r--   0        0        0      387 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/oe-rpb.json
+-rw-r--r--   0        0        0      409 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/oniro.json
+-rw-r--r--   0        0        0      387 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/qcom-rpb-dunfell.json
+-rw-r--r--   0        0        0      388 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/qcom-rpb-honister.json
+-rw-r--r--   0        0        0      684 2023-05-30 12:51:25.694838 tuxbake-0.4.0/examples/template.json
+-rw-r--r--   0        0        0      325 2023-05-30 12:51:25.694838 tuxbake-0.4.0/examples/yocto.json
+-rw-r--r--   0        0        0      424 2023-05-30 12:51:25.694838 tuxbake-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-05-30 12:51:25.694838 tuxbake-0.4.0/requirements-dev.txt
+-rw-r--r--   0        0        0   594416 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/bitbake-environment
+-rw-r--r--   0        0        0     6264 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0      204 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/test.xml
+-rw-r--r--   0        0        0     1369 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/test_argparse.py
+-rw-r--r--   0        0        0      661 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/test_build.py
+-rw-r--r--   0        0        0     5156 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/test_metadata.py
+-rw-r--r--   0        0        0     9748 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/test_models.py
+-rw-r--r--   0        0        0     5723 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     1409 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake.spec
+-rw-r--r--   0        0        0      112 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/__init__.py
+-rw-r--r--   0        0        0     1909 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/__main__.py
+-rw-r--r--   0        0        0     2984 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/argparse.py
+-rw-r--r--   0        0        0      784 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/build.py
+-rw-r--r--   0        0        0      747 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/exceptions.py
+-rw-r--r--   0        0        0     5014 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/helper.py
+-rw-r--r--   0        0        0     1361 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata.pl
+-rw-r--r--   0        0        0     7276 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata.py
+-rw-r--r--   0        0        0      165 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata/hardware.ini
+-rw-r--r--   0        0        0      300 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata/os.ini
+-rw-r--r--   0        0        0       89 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata/resources.ini
+-rw-r--r--   0        0        0     1602 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata/tools.ini
+-rw-r--r--   0        0        0      190 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata/uname.ini
+-rw-r--r--   0        0        0    14919 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/models.py
+-rw-r--r--   0        0        0     6537 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/utils.py
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 tuxbake-0.4.0/setup.py
+-rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 tuxbake-0.4.0/PKG-INFO
```

### Comparing `tuxbake-0.3.1/.gitlab-ci.yml` & `tuxbake-0.4.0/.gitlab-ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -131,7 +131,21 @@
   variables:
     TARGET: ubuntu-20.04
 
 ubuntu-22.04:
   extends: .build-image
   variables:
     TARGET: ubuntu-22.04
+
+# trigger packages.tuxsuite.com on release
+trigger_tuxsuite:
+  stage: .post
+  image: docker:22.04
+  before_script:
+    - apt update
+    - apt install -y curl
+  script:
+    - "curl -X POST -F token=$TUXSUITE_PACKAGES_TRIGGER_TOKEN -F ref=master https://gitlab.com/api/v4/projects/13070238/trigger/pipeline"
+  only:
+    - tags
+  needs:
+    - pages
```

### Comparing `tuxbake-0.3.1/Dockerfile.ci-debian` & `tuxbake-0.4.0/Dockerfile.ci-debian`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/Dockerfile.ci-fedora` & `tuxbake-0.4.0/Dockerfile.ci-fedora`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/LICENSE` & `tuxbake-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/Makefile` & `tuxbake-0.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/README.md` & `tuxbake-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/debian/rules` & `tuxbake-0.4.0/debian/rules`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/Makefile` & `tuxbake-0.4.0/dockerfiles/Makefile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/centos-7/Dockerfile` & `tuxbake-0.4.0/dockerfiles/centos-7/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/centos-8/Dockerfile` & `tuxbake-0.4.0/dockerfiles/centos-8/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/debian-bullseye/Dockerfile` & `tuxbake-0.4.0/dockerfiles/debian-bullseye/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/debian-buster/Dockerfile` & `tuxbake-0.4.0/dockerfiles/debian-buster/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/debian-stretch/Dockerfile` & `tuxbake-0.4.0/dockerfiles/debian-stretch/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/fedora-33/Dockerfile` & `tuxbake-0.4.0/dockerfiles/fedora-33/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/fedora-34/Dockerfile` & `tuxbake-0.4.0/dockerfiles/fedora-34/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/opensuse-leap-15.1/Dockerfile` & `tuxbake-0.4.0/dockerfiles/opensuse-leap-15.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/opensuse-leap-15.2/Dockerfile` & `tuxbake-0.4.0/dockerfiles/opensuse-leap-15.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/ubuntu-16.04/Dockerfile` & `tuxbake-0.4.0/dockerfiles/ubuntu-16.04/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/ubuntu-18.04/Dockerfile` & `tuxbake-0.4.0/dockerfiles/ubuntu-18.04/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/ubuntu-20.04/Dockerfile` & `tuxbake-0.4.0/dockerfiles/ubuntu-20.04/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/dockerfiles/ubuntu-22.04/Dockerfile` & `tuxbake-0.4.0/dockerfiles/ubuntu-22.04/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/examples/lkft.json` & `tuxbake-0.4.0/examples/lkft.json`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/examples/template.json` & `tuxbake-0.4.0/examples/template.json`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/tests/unit/bitbake-environment` & `tuxbake-0.4.0/tests/unit/bitbake-environment`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/tests/unit/conftest.py` & `tuxbake-0.4.0/tests/unit/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import subprocess
 import sys
 import pytest
 
 # TODO this should not be needed if the tuxmake RPM manages to provide a public
 # Python module that is not tied to a specific Python version
 sys.path.append("/usr/share/tuxmake")
+from tuxmake.runtime import Runtime
 
 
 oebuild_git_params = {
     "sources": {
         "git_trees": [
             {"url": "http://git.yoctoproject.org/git/poky", "branch": "main"},
             {"url": "https://github.com/ndechesne/meta-qcom", "branch": "main"},
@@ -170,7 +171,18 @@
 
 @pytest.fixture()
 def oebuild_repo_init_object():
     from tuxbake.models import OEBuild
 
     oebuild = OEBuild(**oebuild_repo_object)
     return oebuild
+
+
+@pytest.fixture()
+def metadata_obj(oebuild_repo_init_object):
+    from tuxbake.metadata import Metadata
+
+    oebuild = oebuild_repo_init_object
+    # prepare runtime
+    runtime = Runtime.get(oebuild.runtime)
+    oebuild._runtime = runtime
+    return Metadata(oebuild)
```

### Comparing `tuxbake-0.3.1/tests/unit/test_argparse.py` & `tuxbake-0.4.0/tests/unit/test_argparse.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/tests/unit/test_build.py` & `tuxbake-0.4.0/tests/unit/test_build.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/tests/unit/test_models.py` & `tuxbake-0.4.0/tests/unit/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,14 @@
     "bblayers_conf": ["bb_conf", [1]],
     "sstate_mirror": [1, 1.4],
     "dl_dir": [1],
 }
 
 
 def test_validate(oebuild_repo_init_object):
-
     # case - similar with repo obj as it has repo instead of git_trees
     oebuild_obj = asdict(oebuild_repo_init_object)
     OEBuild.validate(oebuild_obj)
     # handling all defined test in test_map
     sources = oebuild_obj["sources"]
     for key in test_map:
         if key in ["repo", "git_trees"]:
```

### Comparing `tuxbake-0.3.1/tests/unit/test_utils.py` & `tuxbake-0.4.0/tests/unit/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,58 @@
 import pytest
 from tuxbake.exceptions import TuxbakeRunCmdError
 import os
-import shutil
+from unittest.mock import patch
 
 
 def test_run_cmd(tmp_path):
     from tuxbake.utils import run_cmd
 
     cmd = "ls nofile".split()
     run_cmd(cmd, src_dir=tmp_path, fail_ok=True)
     with pytest.raises(TuxbakeRunCmdError):
         run_cmd(cmd, src_dir=tmp_path, fail_ok=False)
 
 
 def test_git_init(oebuild_git_object, tmpdir_factory):
-
     """
     oebuild_git_object is a gobal fixture defined in conftest file.
     and we are receiving it as a tuple object (oebuild_obj, src_path_1, src_path_2, git_branch_1, git_branch_2, src_dir)
     """
     from tuxbake.utils import git_init
 
     oebuild_object = oebuild_git_object[0]
     src_dir = oebuild_object.src_dir
     git_init(oebuild_object, src_dir)
 
     # case when only url is present and not branch
     for git_obj in oebuild_object.git_trees:
-
         # adding ref also , so as to cover ref if block
         git_obj.ref = f"refs/heads/{git_obj.branch}"
         git_obj.branch = None
 
     temp_src2 = tmpdir_factory.mktemp("src2")
     git_init(oebuild_object, temp_src2)
 
     with pytest.raises((TuxbakeRunCmdError, FileNotFoundError)):
         git_init(oebuild_object, "/some/wrong/folder")
 
+    # check the retries
+    for git_obj in oebuild_object.git_trees:
+        git_obj.branch = None
+        git_obj.sha = None
+        git_obj.ref = None
+    # git_init(oebuild_object, temp_src2)
+    with patch("tuxbake.utils.run_cmd") as mock_run_cmd:
+        with patch("tuxbake.utils.git_get_sha") as patch_get_git_sha:
+            patch_get_git_sha.return_value = None
+            with pytest.raises(TuxbakeRunCmdError):
+                git_init(oebuild_object, temp_src2)
+                assert mock_run_cmd.call_count == 3
+
 
 def test_repo_init(oebuild_repo_init_object, tmpdir_factory, tmpdir):
     from tuxbake.utils import repo_init
 
     oebuild = oebuild_repo_init_object
     url, branch = oebuild.repo.url, oebuild.repo.branch
     temp_src = tmpdir_factory.mktemp("test_repo_init")
@@ -71,31 +82,39 @@
     repo_init(oebuild, tmpdir, local_manifest)
 
     # case - checking with wrong manishfest file name
     oebuild.repo.manifest = "some-wrong-name.xml"
     with pytest.raises(TuxbakeRunCmdError):
         repo_init(oebuild, temp_src)
 
+    # check the retry
+    # wrong manifest, will raise TuxbakeRunCmdError
+    oebuild.repo.manifest = "some-wrong-name.xml"
+    with patch(
+        "tuxbake.utils.run_cmd", side_effect=TuxbakeRunCmdError
+    ) as patch_run_cmd:
+        with pytest.raises(TuxbakeRunCmdError):
+            repo_init(oebuild, temp_src)
+            assert patch_run_cmd.call_count == 3
 
-def test_find_bitbake_env():
 
+def test_find_bitbake_env():
     from tuxbake.utils import find_bitbake_env
 
     path = os.path.abspath("tests/unit/bitbake-environment")
     assert find_bitbake_env(path, "DL_DIR")
     with pytest.raises(AssertionError):
         assert find_bitbake_env(path, "DUMMY_VAR")
 
     # Bitbake environment doesn't exists
     path = os.path.abspath("tests/bitbake-environment")
     assert find_bitbake_env(path, "DL_DIR") is None
 
 
 def test_handle_log(capsys, oebuild_git_object):
-
     from tuxbake.utils import handle_log, git_init
 
     logs_list = ["test", b"test-check-out", b"test-check-err"]
     handle_log(logs_list)
     out, err = capsys.readouterr()
     assert "test-check-err" in err
```

### Comparing `tuxbake-0.3.1/tuxbake.spec` & `tuxbake-0.4.0/tuxbake.spec`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name:      tuxbake
-Version:   0.3.1
+Version:   0.4.0
 Release:   0%{?dist}
 Summary:   FIXME
 License:   FIXME
 URL:       FIXME
 Source0:   %{pypi_source}
 
 
@@ -13,20 +13,22 @@
 BuildRequires: python3-flit
 BuildRequires: python3-pip
 BuildRequires: python3-pytest
 BuildRequires: python3-pytest-cov
 BuildRequires: python3-pytest-mock
 BuildRequires: tuxmake
 BuildRequires: repo
+BuildRequires: python3-retrying
 
 BuildArch: noarch
 
 Requires: python3 >= 3.6
 Requires: tuxmake
 Requires: repo
+Requires: python3-retrying
 
 %global debug_package %{nil}
 
 %description
 FIXME
 
 %prep
```

### Comparing `tuxbake-0.3.1/tuxbake/__main__.py` & `tuxbake-0.4.0/tuxbake/__main__.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/tuxbake/argparse.py` & `tuxbake-0.4.0/tuxbake/argparse.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.3.1/tuxbake/helper.py` & `tuxbake-0.4.0/tuxbake/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,14 @@
         dest,
         str,
         f"Unexpected argument for dest in git_trees object, expected string: '{dest}'",
     )
 
 
 def validate_container(container):
-
     supported_containers = [
         "ubuntu-22.04",
         "ubuntu-20.04",
         "ubuntu-18.04",
         "ubuntu-16.04",
         "centos-8",
         "debian-bullseye",
@@ -127,30 +126,28 @@
         raise TuxbakeParsingError(
             f"Unexpected argument for container: '{container}'; "
             "container not supported or is invalid!!"
         )
 
 
 def validate_local_conf(local_conf):
-
     check_instance(
         local_conf,
         list,
         f"Unexpected argument for local_conf, expected list: '{local_conf}'",
     )
     for conf in local_conf:
         check_instance(
             conf,
             str,
             f"Unexpected argument for local_conf data, expected string: '{conf}'",
         )
 
 
 def validate_bblayers_conf(bblayers_conf):
-
     check_instance(
         bblayers_conf,
         list,
         f"Unexpected argument for bblayers_conf, expected list: '{bblayers_conf}'",
     )
     for bb_conf in bblayers_conf:
         check_instance(
@@ -171,15 +168,14 @@
             artifact,
             str,
             f"Unexpected argument for artifacts data, expected string: '{artifact}'",
         )
 
 
 def validate_extraconfigs(extraconfigs):
-
     check_instance(
         extraconfigs,
         list,
         f"Unexpected argument for extraconfigs, expected list: '{extraconfigs}'",
     )
     for config in extraconfigs:
         check_instance(
```

### Comparing `tuxbake-0.3.1/tuxbake/models.py` & `tuxbake-0.4.0/tuxbake/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,14 @@
         elif self.sources.get("git_trees"):
             self.git_trees = []
             for git_entry in self.sources.get("git_trees"):
                 self.git_trees.append(self.Git(**git_entry))
 
     @staticmethod
     def validate(oebuild_data):
-
         if not oebuild_data.get("sources"):
             raise (
                 TuxbakeParsingError(
                     "Please specify either git_trees or repo in sources of build definition"
                 )
             )
```

### Comparing `tuxbake-0.3.1/tuxbake/utils.py` & `tuxbake-0.4.0/tuxbake/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 import subprocess
 import glob
 from pathlib import Path
 from tuxbake.exceptions import TuxbakeRunCmdError, TuxbakeParsingError
 from tuxmake.logging import debug
 import logging
+from retrying import retry
 
 formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
 logger = logging.getLogger(__name__)
 logger.setLevel(level=logging.INFO)
 
 
 __log_flag__ = False
@@ -32,14 +33,20 @@
 
         return value
 
     return log
 
 
 @log_handler
+@retry(
+    wait_exponential_multiplier=500,
+    wait_exponential_max=10000,
+    stop_max_attempt_number=3,
+    retry_on_exception=lambda e: isinstance(e, TuxbakeRunCmdError),
+)
 def repo_init(oebuild, src_dir, local_manifest=None, pinned_manifest=None):
     cmd = f"repo init -u {oebuild.repo.url} -b {oebuild.repo.branch} -m {oebuild.repo.manifest}".split()
     run_cmd(cmd, src_dir)
     if pinned_manifest:
         cmd = f"cp {pinned_manifest} .repo/manifests/{oebuild.repo.manifest}".split()
         run_cmd(cmd, src_dir)
 
@@ -66,14 +73,20 @@
     except TuxbakeRunCmdError:
         raise TuxbakeRunCmdError(f"Unable to fetch the 'branch' or 'ref': {branch}")
     sha = ret.out.split()[0].decode("utf-8")
     return sha
 
 
 @log_handler
+@retry(
+    wait_exponential_multiplier=500,
+    wait_exponential_max=10000,
+    stop_max_attempt_number=3,
+    retry_on_exception=lambda e: isinstance(e, TuxbakeRunCmdError),
+)
 def git_init(oebuild, src_dir):
     for git_object in oebuild.git_trees:
         url = git_object.url.rstrip("/")
         branch = git_object.branch or git_object.ref
         sha = git_object.sha or git_get_sha(branch, url)
         dest = git_object.dest
         if not (branch or sha):
```

### Comparing `tuxbake-0.3.1/setup.py` & `tuxbake-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 from distutils.core import setup
 
 packages = \
 ['tuxbake']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'tuxbake': ['metadata/*']}
 
 install_requires = \
 ['tuxmake >=1.2.0']
 
 entry_points = \
 {'console_scripts': ['tuxbake = tuxbake.__main__:main']}
 
 setup(name='tuxbake',
-      version='0.3.1',
+      version='0.4.0',
       description='Command line tool to build OpenEmbedded and Yocto images',
       author='Vishal Bhoj',
       author_email='vishal.bhoj@linaro.org',
       url='https://tuxbake.org/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

