# Comparing `tmp/saspy-5.1.2.tar.gz` & `tmp/saspy-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saspy-5.1.2.tar", last modified: Fri Apr 28 14:58:16 2023, max compression
+gzip compressed data, was "saspy-5.2.0.tar", last modified: Tue May 30 15:47:11 2023, max compression
```

## Comparing `saspy-5.1.2.tar` & `saspy-5.2.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.845075 saspy-5.1.2/
--rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2023-04-28 14:58:04.000000 saspy-5.1.2/LICENSE.md
--rw-r--r--   0 sastpw     (894) r&d        (100)       18 2023-04-28 14:58:04.000000 saspy-5.1.2/MANIFEST.in
--rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-04-28 14:58:16.845075 saspy-5.1.2/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2023-04-28 14:58:04.000000 saspy-5.1.2/README.md
--rw-r--r--   0 sastpw     (894) r&d        (100)      173 2023-04-28 14:58:04.000000 saspy-5.1.2/pyproject.toml
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.819074 saspy-5.1.2/saspy/
--rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/SASLogLexer.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/__init__.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/autocfg.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.821074 saspy-5.1.2/saspy/java/
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.832074 saspy-5.1.2/saspy/java/iomclient/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/log4j-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/log4j-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/log4j-core-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/log4j-core-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/sas.core.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/sas.security.sspi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/sas.svc.connection.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.836075 saspy-5.1.2/saspy/java/pyiom/
--rw-r--r--   0 sastpw     (894) r&d        (100)    17665 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/pyiom/saspy2j.class
--rw-r--r--   0 sastpw     (894) r&d        (100)    32061 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/pyiom/saspy2j.java
--rw-r--r--   0 sastpw     (894) r&d        (100)    18548 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/saspyiom.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.844076 saspy-5.1.2/saspy/java/thirdparty/
--rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/thirdparty/NOTICE.md
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/thirdparty/glassfish-corba-internal-api.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/thirdparty/glassfish-corba-omgapi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/thirdparty/glassfish-corba-orb.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/thirdparty/pfl-basic.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/thirdparty/pfl-tf.jar
--rw-r--r--   0 sastpw     (894) r&d        (100)     3529 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/libname_gen.sas
--rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasViyaML.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sas_magic.py
--rw-r--r--   0 sastpw     (894) r&d        (100)   130256 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasbase.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10967 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sascfg.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasdata.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasdecorator.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasets.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     2418 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasexceptions.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    37669 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasiocom.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    84218 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasiohttp.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    87068 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasioiom.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    99701 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasiostdio.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasml.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    37444 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasproccommons.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasqc.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasresults.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasstat.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sastabulate.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasutil.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.844076 saspy-5.1.2/saspy/scripts/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/scripts/run_sas.py
--rw-r--r--   0 sastpw     (894) r&d        (100)       22 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/version.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.820073 saspy-5.1.2/saspy.egg-info/
--rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-04-28 14:58:16.000000 saspy-5.1.2/saspy.egg-info/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     1392 2023-04-28 14:58:16.000000 saspy-5.1.2/saspy.egg-info/SOURCES.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        1 2023-04-28 14:58:16.000000 saspy-5.1.2/saspy.egg-info/dependency_links.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       41 2023-04-28 14:58:16.000000 saspy-5.1.2/saspy.egg-info/requires.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        6 2023-04-28 14:58:16.000000 saspy-5.1.2/saspy.egg-info/top_level.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       38 2023-04-28 14:58:16.845075 saspy-5.1.2/setup.cfg
--rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2023-04-28 14:58:04.000000 saspy-5.1.2/setup.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-30 15:47:11.795040 saspy-5.2.0/
+-rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2023-05-30 15:46:52.000000 saspy-5.2.0/LICENSE.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)       18 2023-05-30 15:46:52.000000 saspy-5.2.0/MANIFEST.in
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-05-30 15:47:11.794040 saspy-5.2.0/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2023-05-30 15:46:52.000000 saspy-5.2.0/README.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)      173 2023-05-30 15:46:52.000000 saspy-5.2.0/pyproject.toml
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-30 15:47:11.774039 saspy-5.2.0/saspy/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/SASLogLexer.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/__init__.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/autocfg.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-30 15:47:11.776039 saspy-5.2.0/saspy/java/
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-30 15:47:11.786040 saspy-5.2.0/saspy/java/iomclient/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/iomclient/log4j-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/iomclient/log4j-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/iomclient/log4j-core-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/iomclient/log4j-core-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/iomclient/sas.core.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/iomclient/sas.security.sspi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/iomclient/sas.svc.connection.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-30 15:47:11.789040 saspy-5.2.0/saspy/java/pyiom/
+-rw-r--r--   0 sastpw     (894) r&d        (100)    17665 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/pyiom/saspy2j.class
+-rw-r--r--   0 sastpw     (894) r&d        (100)    32061 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/pyiom/saspy2j.java
+-rw-r--r--   0 sastpw     (894) r&d        (100)    18548 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/saspyiom.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-30 15:47:11.794040 saspy-5.2.0/saspy/java/thirdparty/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/thirdparty/NOTICE.md
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/thirdparty/glassfish-corba-orb.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/thirdparty/pfl-basic.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/java/thirdparty/pfl-tf.jar
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3529 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/libname_gen.sas
+-rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasViyaML.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sas_magic.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)   130270 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasbase.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10967 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sascfg.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasdata.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasdecorator.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasets.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2418 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasexceptions.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    37669 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasiocom.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    86926 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasiohttp.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    87068 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasioiom.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    99635 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasiostdio.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasml.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    37444 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasproccommons.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasqc.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasresults.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasstat.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sastabulate.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/sasutil.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-30 15:47:11.794040 saspy-5.2.0/saspy/scripts/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/scripts/run_sas.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)       22 2023-05-30 15:46:52.000000 saspy-5.2.0/saspy/version.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-30 15:47:11.775040 saspy-5.2.0/saspy.egg-info/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-05-30 15:47:11.000000 saspy-5.2.0/saspy.egg-info/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1392 2023-05-30 15:47:11.000000 saspy-5.2.0/saspy.egg-info/SOURCES.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        1 2023-05-30 15:47:11.000000 saspy-5.2.0/saspy.egg-info/dependency_links.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       41 2023-05-30 15:47:11.000000 saspy-5.2.0/saspy.egg-info/requires.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        6 2023-05-30 15:47:11.000000 saspy-5.2.0/saspy.egg-info/top_level.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       38 2023-05-30 15:47:11.795040 saspy-5.2.0/setup.cfg
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2023-05-30 15:46:52.000000 saspy-5.2.0/setup.py
```

### Comparing `saspy-5.1.2/LICENSE.md` & `saspy-5.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/PKG-INFO` & `saspy-5.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.1.2
+Version: 5.2.0
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.1.2/README.md` & `saspy-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/SASLogLexer.py` & `saspy-5.2.0/saspy/SASLogLexer.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/__init__.py` & `saspy-5.2.0/saspy/__init__.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/autocfg.py` & `saspy-5.2.0/saspy/autocfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar` & `saspy-5.2.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar` & `saspy-5.2.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/iomclient/log4j-api-2.12.4.jar` & `saspy-5.2.0/saspy/java/iomclient/log4j-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/iomclient/log4j-api-2.17.1.jar` & `saspy-5.2.0/saspy/java/iomclient/log4j-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/iomclient/log4j-core-2.12.4.jar` & `saspy-5.2.0/saspy/java/iomclient/log4j-core-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/iomclient/log4j-core-2.17.1.jar` & `saspy-5.2.0/saspy/java/iomclient/log4j-core-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/iomclient/sas.core.jar` & `saspy-5.2.0/saspy/java/iomclient/sas.core.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/iomclient/sas.security.sspi.jar` & `saspy-5.2.0/saspy/java/iomclient/sas.security.sspi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/iomclient/sas.svc.connection.jar` & `saspy-5.2.0/saspy/java/iomclient/sas.svc.connection.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/pyiom/saspy2j.class` & `saspy-5.2.0/saspy/java/pyiom/saspy2j.class`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/pyiom/saspy2j.java` & `saspy-5.2.0/saspy/java/pyiom/saspy2j.java`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/saspyiom.jar` & `saspy-5.2.0/saspy/java/saspyiom.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/thirdparty/NOTICE.md` & `saspy-5.2.0/saspy/java/thirdparty/NOTICE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/thirdparty/glassfish-corba-internal-api.jar` & `saspy-5.2.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/thirdparty/glassfish-corba-omgapi.jar` & `saspy-5.2.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/thirdparty/glassfish-corba-orb.jar` & `saspy-5.2.0/saspy/java/thirdparty/glassfish-corba-orb.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/thirdparty/pfl-basic.jar` & `saspy-5.2.0/saspy/java/thirdparty/pfl-basic.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/java/thirdparty/pfl-tf.jar` & `saspy-5.2.0/saspy/java/thirdparty/pfl-tf.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/libname_gen.sas` & `saspy-5.2.0/saspy/libname_gen.sas`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasViyaML.py` & `saspy-5.2.0/saspy/sasViyaML.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sas_magic.py` & `saspy-5.2.0/saspy/sas_magic.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasbase.py` & `saspy-5.2.0/saspy/sasbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
                 else:
                     cfgname = self._prompt(
                         "Please enter the name of the SAS Config you wish to run. Available Configs are: " +
                         str(configs) + " ")
 
         while cfgname not in configs:
             cfgname = self._prompt(
-                "The SAS Config name specified was not found. Please enter the SAS Config you wish to use. Available Configs are: " +
+                "The SAS Config name specified ("+cfgname+") was not found. Please enter the SAS Config you wish to use. Available Configs are: " +
                 str(configs) + " ")
             if cfgname is None:
                 raise RuntimeError("No SAS Config name provided.")
 
         self.name = cfgname
         cfg = getattr(SAScfg, cfgname)
```

### Comparing `saspy-5.1.2/saspy/sascfg.py` & `saspy-5.2.0/saspy/sascfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasdata.py` & `saspy-5.2.0/saspy/sasdata.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasdecorator.py` & `saspy-5.2.0/saspy/sasdecorator.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasets.py` & `saspy-5.2.0/saspy/sasets.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasexceptions.py` & `saspy-5.2.0/saspy/sasexceptions.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasiocom.py` & `saspy-5.2.0/saspy/sasiocom.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasiohttp.py` & `saspy-5.2.0/saspy/sasiohttp.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,17 @@
       authcode       = cfg.get('authcode', None)
       jwt            = cfg.get('jwt', None)
       self.encoding  = cfg.get('encoding', '')
       self.authkey   = cfg.get('authkey', '')
       self._prompt   = session._sb.sascfg._prompt
       self.lrecl     = cfg.get('lrecl', None)
       self.inactive  = cfg.get('inactive', 120)
+      puser          = cfg.get('proxy_user', '')
+      ppw            = cfg.get('proxy_pw', '')
+      pauthkey       = cfg.get('proxy_authkey', '')
 
       try:
          self.outopts = getattr(SAScfg, "SAS_output_options")
          self.output  = self.outopts.get('output', 'html5')
       except:
          self.output  = 'html5'
 
@@ -216,14 +219,35 @@
       inak = kwargs.get('authkey', '')
       if len(inak) > 0:
          if lock and len(self.authkey):
             logger.warning("Parameter 'authkey' passed to SAS_session was ignored due to configuration restriction.")
          else:
             self.authkey = inak
 
+      inpak = kwargs.get('proxy_authkey', '')
+      if len(inpak) > 0:
+         if lock and len(pauthkey):
+            logger.warning("Parameter 'proxy_authkey' passed to SAS_session was ignored due to configuration restriction.")
+         else:
+            pauthkey = inpak
+
+      inpuser = kwargs.get('proxy_user', '')
+      if len(inpuser) > 0:
+         if lock and len(puser):
+            logger.warning("Parameter 'proxy_user' passed to SAS_session was ignored due to configuration restriction.")
+         else:
+            puser = inpuser
+
+      inppw = kwargs.get('proxy_pw', '')
+      if len(inppw) > 0:
+         if lock and len(ppw):
+            logger.warning("Parameter 'proxy_pw' passed to SAS_session was ignored due to configuration restriction.")
+         else:
+            ppw = inppw
+
       inssl = kwargs.get('ssl', None)
       if inssl is not None:
          if lock and self.ssl:
             logger.warning("Parameter 'ssl' passed to SAS_session was ignored due to configuration restriction.")
          else:
             self.ssl = bool(inssl)
 
@@ -354,16 +378,50 @@
             hp = http[0].split(':')
 
          self.pip   = self.ip
          self.ip    = hp[0]
          self.pport = self.port
          self.port  = int(hp[1]) if len(hp) > 1 else self.port
 
-         #else:
-         #   logger.warning("Parameter 'proxy' not in recognized format. Expeting '[http[s]://]host:port'. Ignoring parameter.")
+         if pauthkey or puser:
+            if not puser:
+               found = False
+               if os.name == 'nt':
+                  pwf = os.path.expanduser('~')+os.sep+'_authinfo'
+               else:
+                  pwf = os.path.expanduser('~')+os.sep+'.authinfo'
+               try:
+                  fid = open(pwf, mode='r')
+                  for line in fid:
+                     if line.startswith(pauthkey):
+                        puser  = line.partition(' user'    )[2].lstrip().partition(' ')[0].partition('\n')[0]
+                        ppw    = line.partition(' password')[2].lstrip().partition(' ')[0].partition('\n')[0]
+                        found  = True
+                        break
+                  fid.close()
+               except OSError as e:
+                  logger.warning('Error trying to read authinfo file:'+pwf+'\n'+str(e))
+                  pass
+               except:
+                  pass
+
+               if not found:
+                  logger.warning('Did not find key '+self.authkey+' in authinfo file:'+pwf+'\n')
+
+            while len(puser) == 0:
+               puser = self._prompt("Please enter proxy_userid: ")
+               if puser is None:
+                  self._token = None
+                  raise RuntimeError("No proxy_userid provided.")
+
+            while len(ppw) == 0:
+               ppw = self._prompt("Please enter proxy_password: ", pw = True)
+               if ppw is None:
+                  self._token = None
+                  raise RuntimeError("No proxy_password provided.")
       else:
          self.pip = None
 
       # get Connections
       if self.ssl:
          sslctx = ssl.create_default_context(cafile=self.cafile)
          if   self.verify is None:
@@ -391,16 +449,23 @@
             self.REFConn  = hc.HTTPSConnection(self.ip, self.port, timeout=self.timeout, context=ssl._create_unverified_context())
             self.HTTPConn = hc.HTTPSConnection(self.ip, self.port, timeout=self.timeout, context=ssl._create_unverified_context())
       else:
          self.REFConn  = hc.HTTPConnection(self.ip, self.port, timeout=self.timeout)
          self.HTTPConn = hc.HTTPConnection(self.ip, self.port, timeout=self.timeout)
 
       if self.pip:
-         self.REFConn.set_tunnel( self.pip, self.pport)
-         self.HTTPConn.set_tunnel(self.pip, self.pport)
+         if puser and ppw:
+            uuser  = urllib.parse.quote(puser)
+            upw    = urllib.parse.quote(ppw)
+            auth   = "Basic "+base64.encodebytes((uuser+":"+upw).encode(self.encoding)).splitlines()[0].decode(self.encoding)
+            header = {"Proxy-Authorization":auth}
+         else:
+            header = None
+         self.REFConn.set_tunnel( self.pip, self.pport, header)
+         self.HTTPConn.set_tunnel(self.pip, self.pport, header)
 
       # get AuthToken
       if not self._token:
          js = self._authenticate(user, pw, authcode, client_id, client_secret, jwt)
          self._token   = js.get('access_token',  None)
          self._refresh = js.get('refresh_token', None)
```

### Comparing `saspy-5.1.2/saspy/sasioiom.py` & `saspy-5.2.0/saspy/sasioiom.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasiostdio.py` & `saspy-5.2.0/saspy/sasiostdio.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,14 +220,15 @@
             try:
                socks.gethostbyaddr(ip)
                self.hostip = ip
             except:
                pass
             x.stdout.close()
             x.terminate()
+            x.wait(1)
          except:
             pass
 
       return
 
 class SASsessionSTDIO():
    """
@@ -552,22 +553,18 @@
                except (subprocess.TimeoutExpired):
                   if self.sascfg.verbose:
                      logger.warning("SAS didn't shutdown w/in 5 seconds; killing it to be sure")
                   self.pid.kill()
                self.to.join(5)
                self.te.join(5)
             else:
-               x = 5
-               while True:
+               for i in range(5):
                   rc = os.waitpid(self.pid, os.WNOHANG)
                   if rc[0] != 0:
                      break
-                  x = x - 1
-                  if x < 1:
-                     break
                   sleep(1)
 
                if rc[0] != 0:
                   pass
                else:
                   if self.sascfg.verbose:
                      logger.warning("SAS didn't shutdown w/in 5 seconds; killing it to be sure")
@@ -1865,15 +1862,15 @@
 
          if self.sascfg.ssh:
             if not self.sascfg.tunnel:
                host = self.sascfg.hostip #socks.gethostname()
             else:
                host = 'localhost'
          else:
-            host = ''
+            host = 'localhost'
 
          try:
             sock = socks.socket()
             if self.sascfg.tunnel:
                sock.bind(('localhost', port))
             else:
                sock.bind(('', port))
```

### Comparing `saspy-5.1.2/saspy/sasml.py` & `saspy-5.2.0/saspy/sasml.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasproccommons.py` & `saspy-5.2.0/saspy/sasproccommons.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasqc.py` & `saspy-5.2.0/saspy/sasqc.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasresults.py` & `saspy-5.2.0/saspy/sasresults.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasstat.py` & `saspy-5.2.0/saspy/sasstat.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sastabulate.py` & `saspy-5.2.0/saspy/sastabulate.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/sasutil.py` & `saspy-5.2.0/saspy/sasutil.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy/scripts/run_sas.py` & `saspy-5.2.0/saspy/scripts/run_sas.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/saspy.egg-info/PKG-INFO` & `saspy-5.2.0/saspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.1.2
+Version: 5.2.0
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.1.2/saspy.egg-info/SOURCES.txt` & `saspy-5.2.0/saspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saspy-5.1.2/setup.py` & `saspy-5.2.0/setup.py`

 * *Files identical despite different names*

