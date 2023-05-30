# Comparing `tmp/tuxbake-0.4.0.tar.gz` & `tmp/tuxbake-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuxbake-0.4.0.tar", last modified: Tue May 30 12:51:27 2023, max compression
+gzip compressed data, was "tuxbake-0.4.1.tar", last modified: Tue May 30 14:47:51 2023, max compression
```

## Comparing `tuxbake-0.4.0.tar` & `tuxbake-0.4.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0       94 2023-05-30 12:51:25.692838 tuxbake-0.4.0/.gitignore
--rw-r--r--   0        0        0     2767 2023-05-30 12:51:25.692838 tuxbake-0.4.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      879 2023-05-30 12:51:25.692838 tuxbake-0.4.0/Dockerfile.ci-debian
--rw-r--r--   0        0        0      555 2023-05-30 12:51:25.692838 tuxbake-0.4.0/Dockerfile.ci-fedora
--rw-r--r--   0        0        0     1054 2023-05-30 12:51:25.692838 tuxbake-0.4.0/LICENSE
--rw-r--r--   0        0        0     1211 2023-05-30 12:51:25.692838 tuxbake-0.4.0/Makefile
--rw-r--r--   0        0        0     4869 2023-05-30 12:51:25.692838 tuxbake-0.4.0/README.md
--rw-r--r--   0        0        0      141 2023-05-30 12:51:25.692838 tuxbake-0.4.0/debian/changelog
--rw-r--r--   0        0        0      700 2023-05-30 12:51:25.692838 tuxbake-0.4.0/debian/control
--rw-r--r--   0        0        0      100 2023-05-30 12:51:25.692838 tuxbake-0.4.0/debian/gbp.conf
--rwxr-xr-x   0        0        0      594 2023-05-30 12:51:25.692838 tuxbake-0.4.0/debian/rules
--rw-r--r--   0        0        0       12 2023-05-30 12:51:25.692838 tuxbake-0.4.0/debian/source/format
--rw-r--r--   0        0        0     1051 2023-05-30 12:51:25.692838 tuxbake-0.4.0/dockerfiles/Makefile
--rw-r--r--   0        0        0     1485 2023-05-30 12:51:25.692838 tuxbake-0.4.0/dockerfiles/centos-7/Dockerfile
--rw-r--r--   0        0        0     1838 2023-05-30 12:51:25.692838 tuxbake-0.4.0/dockerfiles/centos-8/Dockerfile
--rw-r--r--   0        0        0     1823 2023-05-30 12:51:25.692838 tuxbake-0.4.0/dockerfiles/debian-bullseye/Dockerfile
--rw-r--r--   0        0        0     1821 2023-05-30 12:51:25.692838 tuxbake-0.4.0/dockerfiles/debian-buster/Dockerfile
--rw-r--r--   0        0        0     2259 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/debian-stretch/Dockerfile
--rw-r--r--   0        0        0     1803 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/fedora-33/Dockerfile
--rw-r--r--   0        0        0     1714 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/fedora-34/Dockerfile
--rw-r--r--   0        0        0     1535 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/opensuse-leap-15.1/Dockerfile
--rw-r--r--   0        0        0     1535 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/opensuse-leap-15.2/Dockerfile
--rw-r--r--   0        0        0     1564 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/ubuntu-16.04/Dockerfile
--rw-r--r--   0        0        0     1631 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/ubuntu-18.04/Dockerfile
--rw-r--r--   0        0        0     1631 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/ubuntu-20.04/Dockerfile
--rw-r--r--   0        0        0     1631 2023-05-30 12:51:25.693838 tuxbake-0.4.0/dockerfiles/ubuntu-22.04/Dockerfile
--rw-r--r--   0        0        0       76 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/README.md
--rw-r--r--   0        0        0      416 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/demo.json
--rw-r--r--   0        0        0      314 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/ledge-rpb.json
--rw-r--r--   0        0        0      894 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/lkft.json
--rw-r--r--   0        0        0      495 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/lt-qcom.json
--rw-r--r--   0        0        0      387 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/oe-rpb.json
--rw-r--r--   0        0        0      409 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/oniro.json
--rw-r--r--   0        0        0      387 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/qcom-rpb-dunfell.json
--rw-r--r--   0        0        0      388 2023-05-30 12:51:25.693838 tuxbake-0.4.0/examples/qcom-rpb-honister.json
--rw-r--r--   0        0        0      684 2023-05-30 12:51:25.694838 tuxbake-0.4.0/examples/template.json
--rw-r--r--   0        0        0      325 2023-05-30 12:51:25.694838 tuxbake-0.4.0/examples/yocto.json
--rw-r--r--   0        0        0      424 2023-05-30 12:51:25.694838 tuxbake-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       46 2023-05-30 12:51:25.694838 tuxbake-0.4.0/requirements-dev.txt
--rw-r--r--   0        0        0   594416 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/bitbake-environment
--rw-r--r--   0        0        0     6264 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/conftest.py
--rw-r--r--   0        0        0      204 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/test.xml
--rw-r--r--   0        0        0     1369 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/test_argparse.py
--rw-r--r--   0        0        0      661 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/test_build.py
--rw-r--r--   0        0        0     5156 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/test_metadata.py
--rw-r--r--   0        0        0     9748 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/test_models.py
--rw-r--r--   0        0        0     5723 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tests/unit/test_utils.py
--rw-r--r--   0        0        0     1409 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake.spec
--rw-r--r--   0        0        0      112 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/__init__.py
--rw-r--r--   0        0        0     1909 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/__main__.py
--rw-r--r--   0        0        0     2984 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/argparse.py
--rw-r--r--   0        0        0      784 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/build.py
--rw-r--r--   0        0        0      747 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/exceptions.py
--rw-r--r--   0        0        0     5014 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/helper.py
--rw-r--r--   0        0        0     1361 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata.pl
--rw-r--r--   0        0        0     7276 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata.py
--rw-r--r--   0        0        0      165 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata/hardware.ini
--rw-r--r--   0        0        0      300 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata/os.ini
--rw-r--r--   0        0        0       89 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata/resources.ini
--rw-r--r--   0        0        0     1602 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata/tools.ini
--rw-r--r--   0        0        0      190 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/metadata/uname.ini
--rw-r--r--   0        0        0    14919 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/models.py
--rw-r--r--   0        0        0     6537 2023-05-30 12:51:25.696838 tuxbake-0.4.0/tuxbake/utils.py
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 tuxbake-0.4.0/setup.py
--rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 tuxbake-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-05-30 14:47:49.328650 tuxbake-0.4.1/.gitignore
+-rw-r--r--   0        0        0     2767 2023-05-30 14:47:49.328650 tuxbake-0.4.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      879 2023-05-30 14:47:49.328650 tuxbake-0.4.1/Dockerfile.ci-debian
+-rw-r--r--   0        0        0      555 2023-05-30 14:47:49.328650 tuxbake-0.4.1/Dockerfile.ci-fedora
+-rw-r--r--   0        0        0     1054 2023-05-30 14:47:49.328650 tuxbake-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1211 2023-05-30 14:47:49.328650 tuxbake-0.4.1/Makefile
+-rw-r--r--   0        0        0     4869 2023-05-30 14:47:49.328650 tuxbake-0.4.1/README.md
+-rw-r--r--   0        0        0      141 2023-05-30 14:47:49.328650 tuxbake-0.4.1/debian/changelog
+-rw-r--r--   0        0        0      700 2023-05-30 14:47:49.328650 tuxbake-0.4.1/debian/control
+-rw-r--r--   0        0        0      100 2023-05-30 14:47:49.328650 tuxbake-0.4.1/debian/gbp.conf
+-rwxr-xr-x   0        0        0      594 2023-05-30 14:47:49.328650 tuxbake-0.4.1/debian/rules
+-rw-r--r--   0        0        0       12 2023-05-30 14:47:49.328650 tuxbake-0.4.1/debian/source/format
+-rw-r--r--   0        0        0     1051 2023-05-30 14:47:49.328650 tuxbake-0.4.1/dockerfiles/Makefile
+-rw-r--r--   0        0        0     1485 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/centos-7/Dockerfile
+-rw-r--r--   0        0        0     1838 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/centos-8/Dockerfile
+-rw-r--r--   0        0        0     1823 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/debian-bullseye/Dockerfile
+-rw-r--r--   0        0        0     1821 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/debian-buster/Dockerfile
+-rw-r--r--   0        0        0     2259 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/debian-stretch/Dockerfile
+-rw-r--r--   0        0        0     1803 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/fedora-33/Dockerfile
+-rw-r--r--   0        0        0     1714 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/fedora-34/Dockerfile
+-rw-r--r--   0        0        0     1535 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/opensuse-leap-15.1/Dockerfile
+-rw-r--r--   0        0        0     1535 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/opensuse-leap-15.2/Dockerfile
+-rw-r--r--   0        0        0     1564 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/ubuntu-16.04/Dockerfile
+-rw-r--r--   0        0        0     1631 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/ubuntu-18.04/Dockerfile
+-rw-r--r--   0        0        0     1631 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/ubuntu-20.04/Dockerfile
+-rw-r--r--   0        0        0     1631 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/ubuntu-22.04/Dockerfile
+-rw-r--r--   0        0        0       76 2023-05-30 14:47:49.329650 tuxbake-0.4.1/examples/README.md
+-rw-r--r--   0        0        0      416 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/demo.json
+-rw-r--r--   0        0        0      314 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/ledge-rpb.json
+-rw-r--r--   0        0        0      894 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/lkft.json
+-rw-r--r--   0        0        0      495 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/lt-qcom.json
+-rw-r--r--   0        0        0      387 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/oe-rpb.json
+-rw-r--r--   0        0        0      409 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/oniro.json
+-rw-r--r--   0        0        0      387 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/qcom-rpb-dunfell.json
+-rw-r--r--   0        0        0      388 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/qcom-rpb-honister.json
+-rw-r--r--   0        0        0      684 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/template.json
+-rw-r--r--   0        0        0      325 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/yocto.json
+-rw-r--r--   0        0        0      437 2023-05-30 14:47:49.330650 tuxbake-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-05-30 14:47:49.330650 tuxbake-0.4.1/requirements-dev.txt
+-rw-r--r--   0        0        0   594416 2023-05-30 14:47:49.332650 tuxbake-0.4.1/tests/unit/bitbake-environment
+-rw-r--r--   0        0        0     6264 2023-05-30 14:47:49.332650 tuxbake-0.4.1/tests/unit/conftest.py
+-rw-r--r--   0        0        0      204 2023-05-30 14:47:49.332650 tuxbake-0.4.1/tests/unit/test.xml
+-rw-r--r--   0        0        0     1369 2023-05-30 14:47:49.332650 tuxbake-0.4.1/tests/unit/test_argparse.py
+-rw-r--r--   0        0        0      661 2023-05-30 14:47:49.332650 tuxbake-0.4.1/tests/unit/test_build.py
+-rw-r--r--   0        0        0     5156 2023-05-30 14:47:49.332650 tuxbake-0.4.1/tests/unit/test_metadata.py
+-rw-r--r--   0        0        0     9748 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tests/unit/test_models.py
+-rw-r--r--   0        0        0     5723 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     1409 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake.spec
+-rw-r--r--   0        0        0      112 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/__init__.py
+-rw-r--r--   0        0        0     1909 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/__main__.py
+-rw-r--r--   0        0        0     2984 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/argparse.py
+-rw-r--r--   0        0        0      784 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/build.py
+-rw-r--r--   0        0        0      747 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/exceptions.py
+-rw-r--r--   0        0        0     5014 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/helper.py
+-rw-r--r--   0        0        0     1361 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata.pl
+-rw-r--r--   0        0        0     7276 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata.py
+-rw-r--r--   0        0        0      165 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata/hardware.ini
+-rw-r--r--   0        0        0      300 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata/os.ini
+-rw-r--r--   0        0        0       89 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata/resources.ini
+-rw-r--r--   0        0        0     1602 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata/tools.ini
+-rw-r--r--   0        0        0      190 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata/uname.ini
+-rw-r--r--   0        0        0    14919 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/models.py
+-rw-r--r--   0        0        0     6537 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/utils.py
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 tuxbake-0.4.1/setup.py
+-rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 tuxbake-0.4.1/PKG-INFO
```

### Comparing `tuxbake-0.4.0/.gitlab-ci.yml` & `tuxbake-0.4.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/Dockerfile.ci-debian` & `tuxbake-0.4.1/Dockerfile.ci-debian`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/Dockerfile.ci-fedora` & `tuxbake-0.4.1/Dockerfile.ci-fedora`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/LICENSE` & `tuxbake-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/Makefile` & `tuxbake-0.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/README.md` & `tuxbake-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/debian/control` & `tuxbake-0.4.1/debian/control`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/debian/rules` & `tuxbake-0.4.1/debian/rules`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/Makefile` & `tuxbake-0.4.1/dockerfiles/Makefile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/centos-7/Dockerfile` & `tuxbake-0.4.1/dockerfiles/centos-7/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/centos-8/Dockerfile` & `tuxbake-0.4.1/dockerfiles/centos-8/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/debian-bullseye/Dockerfile` & `tuxbake-0.4.1/dockerfiles/debian-bullseye/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/debian-buster/Dockerfile` & `tuxbake-0.4.1/dockerfiles/debian-buster/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/debian-stretch/Dockerfile` & `tuxbake-0.4.1/dockerfiles/debian-stretch/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/fedora-33/Dockerfile` & `tuxbake-0.4.1/dockerfiles/fedora-33/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/fedora-34/Dockerfile` & `tuxbake-0.4.1/dockerfiles/fedora-34/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/opensuse-leap-15.1/Dockerfile` & `tuxbake-0.4.1/dockerfiles/opensuse-leap-15.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/opensuse-leap-15.2/Dockerfile` & `tuxbake-0.4.1/dockerfiles/opensuse-leap-15.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/ubuntu-16.04/Dockerfile` & `tuxbake-0.4.1/dockerfiles/ubuntu-16.04/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/ubuntu-18.04/Dockerfile` & `tuxbake-0.4.1/dockerfiles/ubuntu-18.04/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/ubuntu-20.04/Dockerfile` & `tuxbake-0.4.1/dockerfiles/ubuntu-20.04/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/dockerfiles/ubuntu-22.04/Dockerfile` & `tuxbake-0.4.1/dockerfiles/ubuntu-22.04/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/examples/lkft.json` & `tuxbake-0.4.1/examples/lkft.json`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/examples/template.json` & `tuxbake-0.4.1/examples/template.json`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tests/unit/bitbake-environment` & `tuxbake-0.4.1/tests/unit/bitbake-environment`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tests/unit/conftest.py` & `tuxbake-0.4.1/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tests/unit/test_argparse.py` & `tuxbake-0.4.1/tests/unit/test_argparse.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tests/unit/test_build.py` & `tuxbake-0.4.1/tests/unit/test_build.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tests/unit/test_metadata.py` & `tuxbake-0.4.1/tests/unit/test_metadata.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tests/unit/test_models.py` & `tuxbake-0.4.1/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tests/unit/test_utils.py` & `tuxbake-0.4.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tuxbake.spec` & `tuxbake-0.4.1/tuxbake.spec`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name:      tuxbake
-Version:   0.4.0
+Version:   0.4.1
 Release:   0%{?dist}
 Summary:   FIXME
 License:   FIXME
 URL:       FIXME
 Source0:   %{pypi_source}
```

### Comparing `tuxbake-0.4.0/tuxbake/__main__.py` & `tuxbake-0.4.1/tuxbake/__main__.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tuxbake/argparse.py` & `tuxbake-0.4.1/tuxbake/argparse.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tuxbake/build.py` & `tuxbake-0.4.1/tuxbake/build.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tuxbake/exceptions.py` & `tuxbake-0.4.1/tuxbake/exceptions.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tuxbake/helper.py` & `tuxbake-0.4.1/tuxbake/helper.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tuxbake/metadata.pl` & `tuxbake-0.4.1/tuxbake/metadata.pl`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tuxbake/metadata.py` & `tuxbake-0.4.1/tuxbake/metadata.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tuxbake/metadata/tools.ini` & `tuxbake-0.4.1/tuxbake/metadata/tools.ini`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tuxbake/models.py` & `tuxbake-0.4.1/tuxbake/models.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/tuxbake/utils.py` & `tuxbake-0.4.1/tuxbake/utils.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.0/setup.py` & `tuxbake-0.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 packages = \
 ['tuxbake']
 
 package_data = \
 {'': ['*'], 'tuxbake': ['metadata/*']}
 
 install_requires = \
-['tuxmake >=1.2.0']
+['tuxmake >=1.2.0', 'retrying']
 
 entry_points = \
 {'console_scripts': ['tuxbake = tuxbake.__main__:main']}
 
 setup(name='tuxbake',
-      version='0.4.0',
+      version='0.4.1',
       description='Command line tool to build OpenEmbedded and Yocto images',
       author='Vishal Bhoj',
       author_email='vishal.bhoj@linaro.org',
       url='https://tuxbake.org/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

