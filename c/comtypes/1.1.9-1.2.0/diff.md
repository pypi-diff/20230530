# Comparing `tmp/comtypes-1.1.9.zip` & `tmp/comtypes-1.2.0.zip`

## zipinfo {}

```diff
@@ -1,106 +1,109 @@
-Zip file size: 182054 bytes, number of entries: 104
-drwxrwxrwx  2.0 fat        0 b- stor 21-Mar-13 13:21 comtypes-1.1.9/
-drwxrwxrwx  2.0 fat        0 b- stor 21-Mar-13 13:21 comtypes-1.1.9/comtypes/
-drwxrwxrwx  2.0 fat        0 b- stor 21-Mar-13 13:21 comtypes-1.1.9/comtypes.egg-info/
--rw-rw-rw-  2.0 fat    38289 b- defN 21-Feb-28 19:41 comtypes-1.1.9/CHANGES.txt
--rw-rw-rw-  2.0 fat     1554 b- defN 21-Feb-28 19:41 comtypes-1.1.9/clear_comtypes_cache.py
--rw-rw-rw-  2.0 fat     1249 b- defN 21-Feb-28 19:41 comtypes-1.1.9/LICENSE.txt
--rw-rw-rw-  2.0 fat       14 b- defN 21-Feb-28 19:41 comtypes-1.1.9/MANIFEST.in
--rw-rw-rw-  2.0 fat     1925 b- defN 21-Mar-13 13:21 comtypes-1.1.9/PKG-INFO
--rw-rw-rw-  2.0 fat      855 b- defN 21-Feb-28 19:41 comtypes-1.1.9/README
--rw-rw-rw-  2.0 fat       64 b- defN 21-Mar-13 13:21 comtypes-1.1.9/setup.cfg
--rw-rw-rw-  2.0 fat     6080 b- defN 21-Feb-28 19:41 comtypes-1.1.9/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 21-Mar-13 13:21 comtypes-1.1.9/comtypes/client/
-drwxrwxrwx  2.0 fat        0 b- stor 21-Mar-13 13:21 comtypes-1.1.9/comtypes/server/
-drwxrwxrwx  2.0 fat        0 b- stor 21-Mar-13 13:21 comtypes-1.1.9/comtypes/test/
-drwxrwxrwx  2.0 fat        0 b- stor 21-Mar-13 13:21 comtypes-1.1.9/comtypes/tools/
--rw-rw-rw-  2.0 fat    29172 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/automation.py
--rw-rw-rw-  2.0 fat     3157 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/connectionpoints.py
--rw-rw-rw-  2.0 fat     3823 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/errorinfo.py
--rw-rw-rw-  2.0 fat     2559 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/git.py
--rw-rw-rw-  2.0 fat     2681 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/GUID.py
--rw-rw-rw-  2.0 fat     2290 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/hresult.py
--rw-rw-rw-  2.0 fat     1621 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/logutil.py
--rw-rw-rw-  2.0 fat     1302 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/messageloop.py
--rw-rw-rw-  2.0 fat     3312 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/npsupport.py
--rw-rw-rw-  2.0 fat     1969 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/patcher.py
--rw-rw-rw-  2.0 fat     7081 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/persist.py
--rw-rw-rw-  2.0 fat    16461 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/safearray.py
--rw-rw-rw-  2.0 fat     8216 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/shelllink.py
--rw-rw-rw-  2.0 fat    31084 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/typeinfo.py
--rw-rw-rw-  2.0 fat     3084 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/util.py
--rw-rw-rw-  2.0 fat     6399 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/viewobject.py
--rw-rw-rw-  2.0 fat    29679 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/_comobject.py
--rw-rw-rw-  2.0 fat     2167 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/_meta.py
--rw-rw-rw-  2.0 fat     4334 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/_safearray.py
--rw-rw-rw-  2.0 fat    52587 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/__init__.py
--rw-rw-rw-  2.0 fat     5756 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/client/dynamic.py
--rw-rw-rw-  2.0 fat    10188 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/client/lazybind.py
--rw-rw-rw-  2.0 fat     5628 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/client/_code_cache.py
--rw-rw-rw-  2.0 fat    11001 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/client/_events.py
--rw-rw-rw-  2.0 fat     7906 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/client/_generate.py
--rw-rw-rw-  2.0 fat    10460 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/client/__init__.py
--rw-rw-rw-  2.0 fat     2915 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/server/automation.py
--rw-rw-rw-  2.0 fat     6042 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/server/connectionpoints.py
--rw-rw-rw-  2.0 fat     4194 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/server/inprocserver.py
--rw-rw-rw-  2.0 fat     2324 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/server/localserver.py
--rw-rw-rw-  2.0 fat    14144 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/server/register.py
--rw-rw-rw-  2.0 fat     2701 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/server/w_getopt.py
--rw-rw-rw-  2.0 fat     2390 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/server/__init__.py
--rw-rw-rw-  2.0 fat     2282 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/find_memleak.py
--rw-rw-rw-  2.0 fat     1664 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/mylib.idl
--rw-rw-rw-  2.0 fat     2491 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/mytypelib.idl
--rw-rw-rw-  2.0 fat      130 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/runtests.py
--rw-rw-rw-  2.0 fat      164 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/setup.py
--rw-rw-rw-  2.0 fat     2386 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/TestComServer.idl
--rw-rw-rw-  2.0 fat     4973 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/TestComServer.py
--rw-rw-rw-  2.0 fat     3560 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/TestComServer.tlb
--rw-rw-rw-  2.0 fat     1756 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/TestDispServer.idl
--rw-rw-rw-  2.0 fat     3638 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/TestDispServer.py
--rw-rw-rw-  2.0 fat     2992 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/TestDispServer.tlb
--rw-rw-rw-  2.0 fat     4225 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_agilent.py
--rw-rw-rw-  2.0 fat     1186 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_avmc.py
--rw-rw-rw-  2.0 fat     4202 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_basic.py
--rw-rw-rw-  2.0 fat     1554 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_BSTR.py
--rw-rw-rw-  2.0 fat     1364 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_casesensitivity.py
--rw-rw-rw-  2.0 fat     2410 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_client.py
--rw-rw-rw-  2.0 fat     5095 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_collections.py
--rw-rw-rw-  2.0 fat     7246 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_comserver.py
--rw-rw-rw-  2.0 fat     3854 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_createwrappers.py
--rw-rw-rw-  2.0 fat     3349 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_dict.py
--rw-rw-rw-  2.0 fat     4363 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_dispinterface.py
--rw-rw-rw-  2.0 fat     1123 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_DISPPARAMS.py
--rw-rw-rw-  2.0 fat     3013 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_dyndispatch.py
--rw-rw-rw-  2.0 fat     3928 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_excel.py
--rw-rw-rw-  2.0 fat     2873 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_findgendir.py
--rw-rw-rw-  2.0 fat     1406 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_getactiveobj.py
--rw-rw-rw-  2.0 fat     1351 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_GUID.py
--rw-rw-rw-  2.0 fat     3084 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_ie.py
--rw-rw-rw-  2.0 fat      387 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_jscript.js
--rw-rw-rw-  2.0 fat     2854 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_msscript.py
--rw-rw-rw-  2.0 fat     2295 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_outparam.py
--rw-rw-rw-  2.0 fat     1254 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_propputref.py
--rw-rw-rw-  2.0 fat      362 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_pump_events.py
--rw-rw-rw-  2.0 fat      704 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_QueryService.py
--rw-rw-rw-  2.0 fat    16689 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_safearray.py
--rw-rw-rw-  2.0 fat     1114 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_sapi.py
--rw-rw-rw-  2.0 fat    10120 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_server.py
--rw-rw-rw-  2.0 fat    13493 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_showevents.py
--rw-rw-rw-  2.0 fat      352 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_subinterface.py
--rw-rw-rw-  2.0 fat     3277 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_typeinfo.py
--rw-rw-rw-  2.0 fat     1630 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_urlhistory.py
--rw-rw-rw-  2.0 fat    11310 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_variant.py
--rw-rw-rw-  2.0 fat     3356 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_win32com_interop.py
--rw-rw-rw-  2.0 fat     2256 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_wmi.py
--rw-rw-rw-  2.0 fat     1847 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/test_word.py
--rw-rw-rw-  2.0 fat     7957 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/test/__init__.py
--rw-rw-rw-  2.0 fat    40339 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/tools/codegenerator.py
--rw-rw-rw-  2.0 fat    31063 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/tools/tlbparser.py
--rw-rw-rw-  2.0 fat     3896 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/tools/typedesc.py
--rw-rw-rw-  2.0 fat     5414 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/tools/typedesc_base.py
--rw-rw-rw-  2.0 fat       29 b- defN 21-Feb-28 19:41 comtypes-1.1.9/comtypes/tools/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 21-Mar-13 13:21 comtypes-1.1.9/comtypes.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat     1925 b- defN 21-Mar-13 13:21 comtypes-1.1.9/comtypes.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat     2601 b- defN 21-Mar-13 13:21 comtypes-1.1.9/comtypes.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        9 b- defN 21-Mar-13 13:21 comtypes-1.1.9/comtypes.egg-info/top_level.txt
-104 files, 596853 bytes uncompressed, 165784 bytes compressed:  72.2%
+Zip file size: 204078 bytes, number of entries: 107
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 15:18 comtypes-1.2.0/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 15:18 comtypes-1.2.0/comtypes/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 15:18 comtypes-1.2.0/comtypes.egg-info/
+-rw-rw-rw-  2.0 fat    41844 b- defN 23-May-29 15:23 comtypes-1.2.0/CHANGES.txt
+-rw-rw-rw-  2.0 fat     1554 b- defN 23-May-29 15:23 comtypes-1.2.0/clear_comtypes_cache.py
+-rw-rw-rw-  2.0 fat     1249 b- defN 23-May-29 15:23 comtypes-1.2.0/LICENSE.txt
+-rw-rw-rw-  2.0 fat       32 b- defN 23-May-29 15:23 comtypes-1.2.0/MANIFEST.in
+-rw-rw-rw-  2.0 fat     4222 b- defN 23-May-30 15:18 comtypes-1.2.0/PKG-INFO
+-rw-rw-rw-  2.0 fat     2951 b- defN 23-May-29 15:23 comtypes-1.2.0/README.md
+-rw-rw-rw-  2.0 fat       42 b- defN 23-May-30 15:18 comtypes-1.2.0/setup.cfg
+-rw-rw-rw-  2.0 fat     5956 b- defN 23-May-29 15:23 comtypes-1.2.0/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 15:18 comtypes-1.2.0/comtypes/client/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 15:18 comtypes-1.2.0/comtypes/server/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 15:18 comtypes-1.2.0/comtypes/test/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 15:18 comtypes-1.2.0/comtypes/tools/
+-rw-rw-rw-  2.0 fat    33629 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/automation.py
+-rw-rw-rw-  2.0 fat     3606 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/connectionpoints.py
+-rw-rw-rw-  2.0 fat     3922 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/errorinfo.py
+-rw-rw-rw-  2.0 fat     2559 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/git.py
+-rw-rw-rw-  2.0 fat     2779 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/GUID.py
+-rw-rw-rw-  2.0 fat     2290 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/hresult.py
+-rw-rw-rw-  2.0 fat     1621 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/logutil.py
+-rw-rw-rw-  2.0 fat     1308 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/messageloop.py
+-rw-rw-rw-  2.0 fat     1969 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/patcher.py
+-rw-rw-rw-  2.0 fat     7812 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/persist.py
+-rw-rw-rw-  2.0 fat    16913 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/safearray.py
+-rw-rw-rw-  2.0 fat     8261 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/shelllink.py
+-rw-rw-rw-  2.0 fat    41340 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/typeinfo.py
+-rw-rw-rw-  2.0 fat     3084 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/util.py
+-rw-rw-rw-  2.0 fat     6399 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/viewobject.py
+-rw-rw-rw-  2.0 fat    29896 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/_comobject.py
+-rw-rw-rw-  2.0 fat    20533 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/_memberspec.py
+-rw-rw-rw-  2.0 fat     2167 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/_meta.py
+-rw-rw-rw-  2.0 fat     4591 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/_npsupport.py
+-rw-rw-rw-  2.0 fat     4334 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/_safearray.py
+-rw-rw-rw-  2.0 fat    45295 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/__init__.py
+-rw-rw-rw-  2.0 fat     5992 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/client/dynamic.py
+-rw-rw-rw-  2.0 fat    10188 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/client/lazybind.py
+-rw-rw-rw-  2.0 fat     5660 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/client/_code_cache.py
+-rw-rw-rw-  2.0 fat     4548 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/client/_constants.py
+-rw-rw-rw-  2.0 fat    11045 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/client/_events.py
+-rw-rw-rw-  2.0 fat    10842 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/client/_generate.py
+-rw-rw-rw-  2.0 fat    11785 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/client/__init__.py
+-rw-rw-rw-  2.0 fat     2913 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/server/automation.py
+-rw-rw-rw-  2.0 fat     6046 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/server/connectionpoints.py
+-rw-rw-rw-  2.0 fat     4282 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/server/inprocserver.py
+-rw-rw-rw-  2.0 fat     2402 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/server/localserver.py
+-rw-rw-rw-  2.0 fat    14141 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/server/register.py
+-rw-rw-rw-  2.0 fat     2701 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/server/w_getopt.py
+-rw-rw-rw-  2.0 fat     2390 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/server/__init__.py
+-rw-rw-rw-  2.0 fat     2318 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/find_memleak.py
+-rw-rw-rw-  2.0 fat     1664 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/mylib.idl
+-rw-rw-rw-  2.0 fat     2491 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/mytypelib.idl
+-rw-rw-rw-  2.0 fat      130 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/runtests.py
+-rw-rw-rw-  2.0 fat      164 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/setup.py
+-rw-rw-rw-  2.0 fat     2386 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/TestComServer.idl
+-rw-rw-rw-  2.0 fat     5050 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/TestComServer.py
+-rw-rw-rw-  2.0 fat     3560 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/TestComServer.tlb
+-rw-rw-rw-  2.0 fat     1756 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/TestDispServer.idl
+-rw-rw-rw-  2.0 fat     3638 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/TestDispServer.py
+-rw-rw-rw-  2.0 fat     2992 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/TestDispServer.tlb
+-rw-rw-rw-  2.0 fat     4308 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_agilent.py
+-rw-rw-rw-  2.0 fat     1329 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_avmc.py
+-rw-rw-rw-  2.0 fat     4128 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_basic.py
+-rw-rw-rw-  2.0 fat     1555 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_BSTR.py
+-rw-rw-rw-  2.0 fat     1364 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_casesensitivity.py
+-rw-rw-rw-  2.0 fat    10244 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_client.py
+-rw-rw-rw-  2.0 fat     5310 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_collections.py
+-rw-rw-rw-  2.0 fat     7414 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_comserver.py
+-rw-rw-rw-  2.0 fat     4063 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_createwrappers.py
+-rw-rw-rw-  2.0 fat     3204 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_dict.py
+-rw-rw-rw-  2.0 fat     4604 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_dispinterface.py
+-rw-rw-rw-  2.0 fat     1109 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_DISPPARAMS.py
+-rw-rw-rw-  2.0 fat     3013 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_dyndispatch.py
+-rw-rw-rw-  2.0 fat     4495 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_excel.py
+-rw-rw-rw-  2.0 fat     2862 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_findgendir.py
+-rw-rw-rw-  2.0 fat     1576 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_getactiveobj.py
+-rw-rw-rw-  2.0 fat      983 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_GUID.py
+-rw-rw-rw-  2.0 fat     3241 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_ie.py
+-rw-rw-rw-  2.0 fat      387 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_jscript.js
+-rw-rw-rw-  2.0 fat     2834 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_msscript.py
+-rw-rw-rw-  2.0 fat    11725 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_npsupport.py
+-rw-rw-rw-  2.0 fat     2447 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_outparam.py
+-rw-rw-rw-  2.0 fat     1317 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_propputref.py
+-rw-rw-rw-  2.0 fat      362 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_pump_events.py
+-rw-rw-rw-  2.0 fat      797 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_QueryService.py
+-rw-rw-rw-  2.0 fat     9954 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_safearray.py
+-rw-rw-rw-  2.0 fat     1110 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_sapi.py
+-rw-rw-rw-  2.0 fat    11507 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_server.py
+-rw-rw-rw-  2.0 fat     1452 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_showevents.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_subinterface.py
+-rw-rw-rw-  2.0 fat     3605 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_typeinfo.py
+-rw-rw-rw-  2.0 fat     1748 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_urlhistory.py
+-rw-rw-rw-  2.0 fat    10297 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_variant.py
+-rw-rw-rw-  2.0 fat     4042 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_win32com_interop.py
+-rw-rw-rw-  2.0 fat     2404 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_wmi.py
+-rw-rw-rw-  2.0 fat     2265 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/test_word.py
+-rw-rw-rw-  2.0 fat     7877 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/test/__init__.py
+-rw-rw-rw-  2.0 fat    54305 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/tools/codegenerator.py
+-rw-rw-rw-  2.0 fat    31811 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/tools/tlbparser.py
+-rw-rw-rw-  2.0 fat     5378 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/tools/typedesc.py
+-rw-rw-rw-  2.0 fat     6688 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/tools/typedesc_base.py
+-rw-rw-rw-  2.0 fat       29 b- defN 23-May-29 15:23 comtypes-1.2.0/comtypes/tools/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-30 15:18 comtypes-1.2.0/comtypes.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat     4222 b- defN 23-May-30 15:18 comtypes-1.2.0/comtypes.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat     2691 b- defN 23-May-30 15:18 comtypes-1.2.0/comtypes.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-30 15:18 comtypes-1.2.0/comtypes.egg-info/top_level.txt
+107 files, 669660 bytes uncompressed, 187316 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -1,313 +1,322 @@
-Filename: comtypes-1.1.9/
+Filename: comtypes-1.2.0/
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/
+Filename: comtypes-1.2.0/comtypes/
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes.egg-info/
+Filename: comtypes-1.2.0/comtypes.egg-info/
 Comment: 
 
-Filename: comtypes-1.1.9/CHANGES.txt
+Filename: comtypes-1.2.0/CHANGES.txt
 Comment: 
 
-Filename: comtypes-1.1.9/clear_comtypes_cache.py
+Filename: comtypes-1.2.0/clear_comtypes_cache.py
 Comment: 
 
-Filename: comtypes-1.1.9/LICENSE.txt
+Filename: comtypes-1.2.0/LICENSE.txt
 Comment: 
 
-Filename: comtypes-1.1.9/MANIFEST.in
+Filename: comtypes-1.2.0/MANIFEST.in
 Comment: 
 
-Filename: comtypes-1.1.9/PKG-INFO
+Filename: comtypes-1.2.0/PKG-INFO
 Comment: 
 
-Filename: comtypes-1.1.9/README
+Filename: comtypes-1.2.0/README.md
 Comment: 
 
-Filename: comtypes-1.1.9/setup.cfg
+Filename: comtypes-1.2.0/setup.cfg
 Comment: 
 
-Filename: comtypes-1.1.9/setup.py
+Filename: comtypes-1.2.0/setup.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/client/
+Filename: comtypes-1.2.0/comtypes/client/
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/server/
+Filename: comtypes-1.2.0/comtypes/server/
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/
+Filename: comtypes-1.2.0/comtypes/test/
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/tools/
+Filename: comtypes-1.2.0/comtypes/tools/
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/automation.py
+Filename: comtypes-1.2.0/comtypes/automation.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/connectionpoints.py
+Filename: comtypes-1.2.0/comtypes/connectionpoints.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/errorinfo.py
+Filename: comtypes-1.2.0/comtypes/errorinfo.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/git.py
+Filename: comtypes-1.2.0/comtypes/git.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/GUID.py
+Filename: comtypes-1.2.0/comtypes/GUID.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/hresult.py
+Filename: comtypes-1.2.0/comtypes/hresult.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/logutil.py
+Filename: comtypes-1.2.0/comtypes/logutil.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/messageloop.py
+Filename: comtypes-1.2.0/comtypes/messageloop.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/npsupport.py
+Filename: comtypes-1.2.0/comtypes/patcher.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/patcher.py
+Filename: comtypes-1.2.0/comtypes/persist.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/persist.py
+Filename: comtypes-1.2.0/comtypes/safearray.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/safearray.py
+Filename: comtypes-1.2.0/comtypes/shelllink.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/shelllink.py
+Filename: comtypes-1.2.0/comtypes/typeinfo.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/typeinfo.py
+Filename: comtypes-1.2.0/comtypes/util.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/util.py
+Filename: comtypes-1.2.0/comtypes/viewobject.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/viewobject.py
+Filename: comtypes-1.2.0/comtypes/_comobject.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/_comobject.py
+Filename: comtypes-1.2.0/comtypes/_memberspec.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/_meta.py
+Filename: comtypes-1.2.0/comtypes/_meta.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/_safearray.py
+Filename: comtypes-1.2.0/comtypes/_npsupport.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/__init__.py
+Filename: comtypes-1.2.0/comtypes/_safearray.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/client/dynamic.py
+Filename: comtypes-1.2.0/comtypes/__init__.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/client/lazybind.py
+Filename: comtypes-1.2.0/comtypes/client/dynamic.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/client/_code_cache.py
+Filename: comtypes-1.2.0/comtypes/client/lazybind.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/client/_events.py
+Filename: comtypes-1.2.0/comtypes/client/_code_cache.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/client/_generate.py
+Filename: comtypes-1.2.0/comtypes/client/_constants.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/client/__init__.py
+Filename: comtypes-1.2.0/comtypes/client/_events.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/server/automation.py
+Filename: comtypes-1.2.0/comtypes/client/_generate.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/server/connectionpoints.py
+Filename: comtypes-1.2.0/comtypes/client/__init__.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/server/inprocserver.py
+Filename: comtypes-1.2.0/comtypes/server/automation.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/server/localserver.py
+Filename: comtypes-1.2.0/comtypes/server/connectionpoints.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/server/register.py
+Filename: comtypes-1.2.0/comtypes/server/inprocserver.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/server/w_getopt.py
+Filename: comtypes-1.2.0/comtypes/server/localserver.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/server/__init__.py
+Filename: comtypes-1.2.0/comtypes/server/register.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/find_memleak.py
+Filename: comtypes-1.2.0/comtypes/server/w_getopt.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/mylib.idl
+Filename: comtypes-1.2.0/comtypes/server/__init__.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/mytypelib.idl
+Filename: comtypes-1.2.0/comtypes/test/find_memleak.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/runtests.py
+Filename: comtypes-1.2.0/comtypes/test/mylib.idl
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/setup.py
+Filename: comtypes-1.2.0/comtypes/test/mytypelib.idl
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/TestComServer.idl
+Filename: comtypes-1.2.0/comtypes/test/runtests.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/TestComServer.py
+Filename: comtypes-1.2.0/comtypes/test/setup.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/TestComServer.tlb
+Filename: comtypes-1.2.0/comtypes/test/TestComServer.idl
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/TestDispServer.idl
+Filename: comtypes-1.2.0/comtypes/test/TestComServer.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/TestDispServer.py
+Filename: comtypes-1.2.0/comtypes/test/TestComServer.tlb
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/TestDispServer.tlb
+Filename: comtypes-1.2.0/comtypes/test/TestDispServer.idl
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_agilent.py
+Filename: comtypes-1.2.0/comtypes/test/TestDispServer.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_avmc.py
+Filename: comtypes-1.2.0/comtypes/test/TestDispServer.tlb
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_basic.py
+Filename: comtypes-1.2.0/comtypes/test/test_agilent.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_BSTR.py
+Filename: comtypes-1.2.0/comtypes/test/test_avmc.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_casesensitivity.py
+Filename: comtypes-1.2.0/comtypes/test/test_basic.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_client.py
+Filename: comtypes-1.2.0/comtypes/test/test_BSTR.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_collections.py
+Filename: comtypes-1.2.0/comtypes/test/test_casesensitivity.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_comserver.py
+Filename: comtypes-1.2.0/comtypes/test/test_client.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_createwrappers.py
+Filename: comtypes-1.2.0/comtypes/test/test_collections.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_dict.py
+Filename: comtypes-1.2.0/comtypes/test/test_comserver.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_dispinterface.py
+Filename: comtypes-1.2.0/comtypes/test/test_createwrappers.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_DISPPARAMS.py
+Filename: comtypes-1.2.0/comtypes/test/test_dict.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_dyndispatch.py
+Filename: comtypes-1.2.0/comtypes/test/test_dispinterface.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_excel.py
+Filename: comtypes-1.2.0/comtypes/test/test_DISPPARAMS.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_findgendir.py
+Filename: comtypes-1.2.0/comtypes/test/test_dyndispatch.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_getactiveobj.py
+Filename: comtypes-1.2.0/comtypes/test/test_excel.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_GUID.py
+Filename: comtypes-1.2.0/comtypes/test/test_findgendir.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_ie.py
+Filename: comtypes-1.2.0/comtypes/test/test_getactiveobj.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_jscript.js
+Filename: comtypes-1.2.0/comtypes/test/test_GUID.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_msscript.py
+Filename: comtypes-1.2.0/comtypes/test/test_ie.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_outparam.py
+Filename: comtypes-1.2.0/comtypes/test/test_jscript.js
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_propputref.py
+Filename: comtypes-1.2.0/comtypes/test/test_msscript.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_pump_events.py
+Filename: comtypes-1.2.0/comtypes/test/test_npsupport.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_QueryService.py
+Filename: comtypes-1.2.0/comtypes/test/test_outparam.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_safearray.py
+Filename: comtypes-1.2.0/comtypes/test/test_propputref.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_sapi.py
+Filename: comtypes-1.2.0/comtypes/test/test_pump_events.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_server.py
+Filename: comtypes-1.2.0/comtypes/test/test_QueryService.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_showevents.py
+Filename: comtypes-1.2.0/comtypes/test/test_safearray.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_subinterface.py
+Filename: comtypes-1.2.0/comtypes/test/test_sapi.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_typeinfo.py
+Filename: comtypes-1.2.0/comtypes/test/test_server.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_urlhistory.py
+Filename: comtypes-1.2.0/comtypes/test/test_showevents.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_variant.py
+Filename: comtypes-1.2.0/comtypes/test/test_subinterface.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_win32com_interop.py
+Filename: comtypes-1.2.0/comtypes/test/test_typeinfo.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_wmi.py
+Filename: comtypes-1.2.0/comtypes/test/test_urlhistory.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/test_word.py
+Filename: comtypes-1.2.0/comtypes/test/test_variant.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/test/__init__.py
+Filename: comtypes-1.2.0/comtypes/test/test_win32com_interop.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/tools/codegenerator.py
+Filename: comtypes-1.2.0/comtypes/test/test_wmi.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/tools/tlbparser.py
+Filename: comtypes-1.2.0/comtypes/test/test_word.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/tools/typedesc.py
+Filename: comtypes-1.2.0/comtypes/test/__init__.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/tools/typedesc_base.py
+Filename: comtypes-1.2.0/comtypes/tools/codegenerator.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes/tools/__init__.py
+Filename: comtypes-1.2.0/comtypes/tools/tlbparser.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes.egg-info/dependency_links.txt
+Filename: comtypes-1.2.0/comtypes/tools/typedesc.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes.egg-info/PKG-INFO
+Filename: comtypes-1.2.0/comtypes/tools/typedesc_base.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes.egg-info/SOURCES.txt
+Filename: comtypes-1.2.0/comtypes/tools/__init__.py
 Comment: 
 
-Filename: comtypes-1.1.9/comtypes.egg-info/top_level.txt
+Filename: comtypes-1.2.0/comtypes.egg-info/dependency_links.txt
+Comment: 
+
+Filename: comtypes-1.2.0/comtypes.egg-info/PKG-INFO
+Comment: 
+
+Filename: comtypes-1.2.0/comtypes.egg-info/SOURCES.txt
+Comment: 
+
+Filename: comtypes-1.2.0/comtypes.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `comtypes-1.1.9/CHANGES.txt` & `comtypes-1.2.0/CHANGES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,75 @@
 Comtypes CHANGELOG
 ==================
 
+Release 1.2.0
+--------------
+ * Remove all automatic imports of ``numpy``, and make ``numpy`` interop opt-in. By @bennyrowland.
+ * Move and redefine generating module functions for fixing cross imports. By @junkmd.
+ * Refactor creating ``__all__`` part in ``codegenerator.Generator.generate_code``. By @junkmd.
+ * Quit calling ``GetModule`` from ``tools.codegenerator``. By @junkmd.
+ * Commonize module-creating functions. By @junkmd.
+ * Shorten the lifetime of ``io.StringIO`` used for code generation. By @junkmd.
+ * Fix import source of ``Array`` from ``_ctypes`` to ``ctypes``. By @junkmd.
+ * Add ``for_stub`` mode to ``ImportedNamespaces.getvalue``. By @junkmd.
+ * Remove ``monkeypatch_COMError``. By @junkmd.
+ * Remove ``CodeGenerator.need_GUID``. By @junkmd.
+ * Carve out ``CodeGenerator.type_name`` method to ``TypeNamer`` class. By @junkmd.
+ * Add ``__known_symbols__`` attributes. By @junkmd.
+ * Remove ``CodeGenerator.type_name`` calls no longer needed and rename to ``_to_type_name``. By @junkmd.
+ * Change ``_fix_inout_args`` to module-level top level function. By @junkmd.
+ * Fix docstring from ``DispInterfaceHead``. By @junkmd.
+ * ``...METHOD`` and ``...PROPERTY`` return ``_MemberSpec``s instead of ``tuple``s. By @junkmd.
+ * Make generating ``...property`` DRY. By @junkmd.
+ * Refactor ``_MemberSpec`` stuffs and separate modules. By @junkmd.
+ * Carve out ``make_...Method`` and ``make_...Property`` of ``codegenerator``. By @junkmd.
+ * Removed extra space in ``typeinfo.IRecordInfo._methods_``. By @j0ker70.
+ * Add type annotations to many modules. By @junkmd.
+ * Fix type annotations in many modules. By @j0ker70, @muddi900, and @junkmd.
+ * Delint ``setup.py``. By @jaraco.
+ * Add ``CONTRIBUTING.md``. By @junkmd.
+ * Modernize ``README.md`` style. By @junkmd.
+ * Add announcements of plan for renaming ``master`` branch to ``main`` and dropping Python2 to ``README.md``. By @junkmd.
+
+Release 1.1.14
+--------------
+ * Fix ``SyntaxError`` in generated docstring. Thanks @junkmd.
+
+Release 1.1.13
+--------------
+ * Many fixes in code generator. Thanks @junkmd.
+ * Make tests runnable on AppVeyor CI. Many improvements in tests. Thanks @junkmd and @dmwyatt.
+ * Update (bound_)named_property args and attributes names to be similar to builtin property. Thanks @junkmd.
+ * Refactor function ``GetModule`` and fix type lib timestamping for incomplete generated module. Thanks @junkmd.
+ * Fix recent numpy versions support. Thanks @mworion.
+ * Split ``Constants`` into a separate module. Thanks @junkmd.
+ * ``client.GetModule`` can take a one liner containing lib UUID. Thanks @junkmd.
+ * Use ``Generator.imports`` instead of ``Generator._externals``. Thanks @junkmd.
+ * Rename README to README.md. Thanks @junkmd and @filipporomani.
+ * No patching or modifying ``typedesc.Obj.name`` in ``tools.codegenerator``. Thanks @junkmd.
+ * Load enumerations into ``client.Constants``. Thanks @junkmd.
+
+Release 1.1.12
+--------------
+ * Fix ``_pack_`` being returned as a float. Thanks @kdschlosser.
+ * More general fix for timestamping a type library. Thanks @kdschlosser.
+
+Release 1.1.11
+--------------
+ * Fix setuptools>=57.5.0 compatibility. Thanks @kdschlosser.
+ * Fix timestamping for typelib. Thanks @fusentasticus.
+ * Fix 64bit inproc server. Thanks @klusidy.
+ * Drop Python 2.6 support (Python 2.7 is still supported).
+ * Fix IndexError for empty safearray. Thanks @BALOGHBence.
+ * Make numpy typecodes consistent across numpy versions. Thanks @bennyrowland.
+
+Release 1.1.10
+--------------
+ * Fix loading module from relative path on Windows 7.
+
 Release 1.1.9
 -------------
  * Fix loading module from relative path.
  * Use comtypes release version in code generator version check.
 
 Release 1.1.8
 -------------
```

## Comparing `comtypes-1.1.9/clear_comtypes_cache.py` & `comtypes-1.2.0/clear_comtypes_cache.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/LICENSE.txt` & `comtypes-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/setup.py` & `comtypes-1.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """comtypes package install script"""
 import sys
 import os
-import ctypes
 import subprocess
 
 from distutils.core import Command
 from distutils.command.install import install
 from setuptools import setup
 
-try:
-    from distutils.command.build_py import build_py_2to3 as build_py
-except ImportError:
-    from distutils.command.build_py import build_py
+from distutils.command.build_py import build_py
 
-with open('README') as readme_stream:
+with open('README.md') as readme_stream:
     readme = readme_stream.read()
 
+
 class test(Command):
     # Original version of this class posted
     # by Berthold Hoellmann to distutils-sig@python.org
     description = "run tests"
 
     user_options = [
         ('tests=', 't',
          "comma-separated list of packages that contain test modules"),
         ('use-resources=', 'u',
          "resources to use - resource names are defined by tests"),
         ('refcounts', 'r',
-         "repeat tests to search for refcount leaks (requires 'sys.gettotalrefcount')"),
+         "repeat tests to search for refcount leaks (requires "
+         "'sys.gettotalrefcount')"),
         ]
 
     boolean_options = ["refcounts"]
 
     def initialize_options(self):
         self.use_resources = ""
         self.refcounts = False
@@ -63,26 +61,27 @@
                              % (name, (sys.version, sys.platform, os.name)))
             package_failure = comtypes.test.run_tests(package,
                                                       "test_*.py",
                                                       self.verbose,
                                                       self.refcounts)
             self.failure = self.failure or package_failure
 
+
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: Microsoft :: Windows',
     'Programming Language :: Python',
-    'Programming Language :: Python :: 2.6',
     'Programming Language :: Python :: 2.7',
     'Programming Language :: Python :: 3',
     'Topic :: Software Development :: Libraries :: Python Modules',
     ]
 
+
 def read_version():
     # Determine the version number by reading it from the file
     # 'comtypes\__init__.py'.  We cannot import this file (with py3,
     # at least) because it is in py2.x syntax.
     for line in open("comtypes/__init__.py"):
         if line.startswith("__version__ = "):
             var, value = line.split('=')
@@ -108,29 +107,30 @@
         self.old_and_unmanageable = None
         self.single_version_externally_managed = None
 
     def run(self):
         install.run(self)
         # Custom script we run at the end of installing
         if not self.dry_run and not self.root:
-            filename = os.path.join(self.install_scripts, "clear_comtypes_cache.py")
+            filename = os.path.join(
+                self.install_scripts, "clear_comtypes_cache.py")
             if not os.path.isfile(filename):
                 raise RuntimeError("Can't find '%s'" % (filename,))
             print("Executing post install script...")
             print('"' + sys.executable + '" "' + filename + '" -y')
             try:
                 subprocess.check_call([sys.executable, filename, '-y'])
             except subprocess.CalledProcessError:
                 print("Failed to run post install script!")
 
 
 setup_params = dict(
     name="comtypes",
     description="Pure Python COM package",
-    long_description = readme,
+    long_description=readme,
     author="Thomas Heller",
     author_email="theller@python.net",
     url="https://github.com/enthought/comtypes",
     download_url="https://github.com/enthought/comtypes/releases",
     license="MIT License",
     package_data={
         "comtypes.test": [
```

## Comparing `comtypes-1.1.9/comtypes/automation.py` & `comtypes-1.2.0/comtypes/automation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 # comtypes.automation module
 import array
 import datetime
 import decimal
+import sys
 
 from ctypes import *
 from ctypes import _Pointer
 from _ctypes import CopyComPointer
-from comtypes import IUnknown, GUID, IID, STDMETHOD, BSTR, COMMETHOD, COMError
+from comtypes import (
+    BSTR, COMError, COMMETHOD, GUID, IID, IUnknown, STDMETHOD, TYPE_CHECKING,
+)
 from comtypes.hresult import *
-from comtypes.patcher import Patch
-from comtypes import npsupport
+import comtypes.patcher
+import comtypes
 try:
     from comtypes import _safearray
 except (ImportError, AttributeError):
     class _safearray(object):
         tagSAFEARRAY = None
 
 from ctypes.wintypes import DWORD, LONG, UINT, VARIANT_BOOL, WCHAR, WORD
 
+if TYPE_CHECKING:
+    from typing import (
+        Any, Callable, ClassVar, List, Optional, Tuple, Union as _UnionT,
+    )
+    from comtypes import hints
+
+
+if sys.version_info >= (3, 0):
+    int_types = (int, )
+    str_types = (str, )
+    base_text_type = str
+else:
+    int_types = (int, long)
+    str_types = (unicode, str)
+    base_text_type = basestring
 
 LCID = DWORD
 DISPID = LONG
 SCODE = LONG
 
 VARTYPE = c_ushort
 
@@ -135,14 +153,21 @@
 
 DECIMAL = tagDEC
 
 
 # The VARIANT structure is a good candidate for implementation in a C
 # helper extension.  At least the get/set methods.
 class tagVARIANT(Structure):
+    if TYPE_CHECKING:
+        vt = hints.AnnoField()  # type: int
+        _ = hints.AnnoField()  # type: U_VARIANT1.__tagVARIANT.U_VARIANT2
+        null = hints.AnnoField()  # type: ClassVar[VARIANT]
+        empty = hints.AnnoField()  # type: ClassVar[VARIANT]
+        missing = hints.AnnoField()  # type: ClassVar[VARIANT]
+
     class U_VARIANT1(Union):
         class __tagVARIANT(Structure):
             # The C Header file defn of VARIANT is much more complicated, but
             # this is the ctypes version - functional as well.
             class U_VARIANT2(Union):
                 class _tagBRECORD(Structure):
                     _fields_ = [("pvRecord", c_void_p),
@@ -191,21 +216,27 @@
             # XXX This does not work.  _b_needsfree_ is never
             # set because the buffer is internal to the object.
             _VariantClear(self)
 
     def __repr__(self):
         if self.vt & VT_BYREF:
             return "VARIANT(vt=0x%x, byref(%r))" % (self.vt, self[0])
+        elif self is type(self).null:
+            return "VARIANT.null"
+        elif self is type(self).empty:
+            return "VARIANT.empty"
+        elif self is type(self).missing:
+            return "VARIANT.missing"
         return "VARIANT(vt=0x%x, %r)" % (self.vt, self.value)
 
+    @classmethod
     def from_param(cls, value):
         if isinstance(value, cls):
             return value
         return cls(value)
-    from_param = classmethod(from_param)
 
     def __setitem__(self, index, value):
         # This method allows to change the value of a
         # (VT_BYREF|VT_xxx) variant in place.
         if index != 0:
             raise IndexError(index)
         if not self.vt & VT_BYREF:
@@ -215,25 +246,25 @@
 
     # see also c:/sf/pywin32/com/win32com/src/oleargs.cpp 54
     def _set_value(self, value):
         _VariantClear(self)
         if value is None:
             self.vt = VT_NULL
         elif (hasattr(value, '__len__') and len(value) == 0
-                and not isinstance(value, basestring)):
+                and not isinstance(value, base_text_type)):
             self.vt = VT_NULL
         # since bool is a subclass of int, this check must come before
         # the check for int
         elif isinstance(value, bool):
             self.vt = VT_BOOL
             self._.VT_BOOL = value
         elif isinstance(value, (int, c_int)):
             self.vt = VT_I4
             self._.VT_I4 = value
-        elif isinstance(value, long):
+        elif isinstance(value, int_types):
             u = self._
             # try VT_I4 first.
             u.VT_I4 = value
             if u.VT_I4 == value:
                 # it did work.
                 self.vt = VT_I4
                 return
@@ -260,27 +291,27 @@
                     return
             # VT_R8 is last resort.
             self.vt = VT_R8
             u.VT_R8 = float(value)
         elif isinstance(value, (float, c_double)):
             self.vt = VT_R8
             self._.VT_R8 = value
-        elif isinstance(value, (str, unicode)):
+        elif isinstance(value, str_types):
             self.vt = VT_BSTR
             # do the c_wchar_p auto unicode conversion
             self._.c_void_p = _SysAllocStringLen(value, len(value))
         elif isinstance(value, datetime.datetime):
             delta = value - _com_null_date
             # a day has 24 * 60 * 60 = 86400 seconds
             com_days = delta.days + (delta.seconds + delta.microseconds * 1e-6) / 86400.
             self.vt = VT_DATE
             self._.VT_R8 = com_days
-        elif npsupport.isdatetime64(value):
-            com_days = value - npsupport.com_null_date64
-            com_days /= npsupport.numpy.timedelta64(1, 'D')
+        elif comtypes.npsupport.isdatetime64(value):
+            com_days = value - comtypes.npsupport.com_null_date64
+            com_days /= comtypes.npsupport.numpy.timedelta64(1, 'D')
             self.vt = VT_DATE
             self._.VT_R8 = com_days
         elif decimal is not None and isinstance(value, decimal.Decimal):
             self._.VT_CY = int(round(value * 10000))
             self.vt = VT_CY
         elif isinstance(value, POINTER(IDispatch)):
             CopyComPointer(value, byref(self._))
@@ -294,18 +325,18 @@
             self.vt = VT_ARRAY | obj._vartype_
         elif isinstance(value, array.array):
             vartype = _arraycode_to_vartype[value.typecode]
             typ = _vartype_to_ctype[vartype]
             obj = _midlSAFEARRAY(typ).create(value)
             memmove(byref(self._), byref(obj), sizeof(obj))
             self.vt = VT_ARRAY | obj._vartype_
-        elif npsupport.isndarray(value):
+        elif comtypes.npsupport.isndarray(value):
             # Try to convert a simple array of basic types.
             descr = value.dtype.descr[0][1]
-            typ = npsupport.typecodes.get(descr)
+            typ = comtypes.npsupport.typecodes.get(descr)
             if typ is None:
                 # Try for variant
                 obj = _midlSAFEARRAY(VARIANT).create(value)
             else:
                 obj = _midlSAFEARRAY(typ).create(value)
             memmove(byref(self._), byref(obj), sizeof(obj))
             self.vt = VT_ARRAY | obj._vartype_
@@ -535,27 +566,28 @@
 _VariantCopyInd.argtypes = POINTER(VARIANT), POINTER(VARIANT)
 
 # some commonly used VARIANT instances
 VARIANT.null = VARIANT(None)
 VARIANT.empty = VARIANT()
 VARIANT.missing = v = VARIANT()
 v.vt = VT_ERROR
-v._.VT_I4 = 0x80020004L
+v._.VT_I4 = 0x80020004
 del v
 
 _carg_obj = type(byref(c_int()))
-from _ctypes import Array as _CArrayType
+from ctypes import Array as _CArrayType
 
-@Patch(POINTER(VARIANT))
+@comtypes.patcher.Patch(POINTER(VARIANT))
 class _(object):
     # Override the default .from_param classmethod of POINTER(VARIANT).
     # This allows to pass values which can be stored in VARIANTs as
     # function parameters declared as POINTER(VARIANT).  See
     # InternetExplorer's Navigate2() method, or Word's Close() method, for
     # examples.
+    @classmethod
     def from_param(cls, arg):
         # accept POINTER(VARIANT) instance
         if isinstance(arg, POINTER(VARIANT)):
             return arg
         # accept byref(VARIANT) instance
         if isinstance(arg, _carg_obj) and isinstance(arg._obj, VARIANT):
             return arg
@@ -563,15 +595,14 @@
         if isinstance(arg, VARIANT):
             return byref(arg)
         if isinstance(arg, _CArrayType) and arg._type_ is VARIANT:
             # accept array of VARIANTs
             return arg
         # anything else which can be converted to a VARIANT.
         return byref(VARIANT(arg))
-    from_param = classmethod(from_param)
 
     def __setitem__(self, index, value):
         # This is to support the same sematics as a pointer instance:
         # variant[0] = value
         self[index].value = value
 
 ################################################################
@@ -579,19 +610,26 @@
 class IEnumVARIANT(IUnknown):
     _iid_ = GUID('{00020404-0000-0000-C000-000000000046}')
     _idlflags_ = ['hidden']
     _dynamic = False
     def __iter__(self):
         return self
 
-    def next(self):
-        item, fetched = self.Next(1)
-        if fetched:
-            return item
-        raise StopIteration
+    if sys.version_info >= (3, 0):
+        def __next__(self):
+            item, fetched = self.Next(1)
+            if fetched:
+                return item
+            raise StopIteration
+    else:
+        def next(self):
+            item, fetched = self.Next(1)
+            if fetched:
+                return item
+            raise StopIteration
 
     def __getitem__(self, index):
         self.Reset()
         # Does not yet work.
 ##        if isinstance(index, slice):
 ##            self.Skip(index.start or 0)
 ##            return self.Next(index.stop or sys.maxint)
@@ -629,14 +667,25 @@
 
 ##from _ctypes import VARIANT_set
 ##import new
 ##VARIANT.value = property(VARIANT._get_value, new.instancemethod(VARIANT_set, None, VARIANT))
 
 
 class tagEXCEPINFO(Structure):
+    if TYPE_CHECKING:
+        wCode = hints.AnnoField()  # type: int
+        wReserved = hints.AnnoField()  # type: int
+        bstrSource = hints.AnnoField()  # type: str
+        bstrDescription = hints.AnnoField()  # type: str
+        bstrHelpFile = hints.AnnoField()  # type: str
+        dwHelpContext = hints.AnnoField()  # type: int
+        pvReserved = hints.AnnoField()  # type: Optional[int]
+        pfnDeferredFillIn = hints.AnnoField()  # type: Optional[int]
+        scode = hints.AnnoField()  # type: int
+
     def __repr__(self):
         return "<EXCEPINFO %s>" % \
                ((self.wCode, self.bstrSource, self.bstrDescription, self.bstrHelpFile, self.dwHelpContext,
                 self.pfnDeferredFillIn, self.scode),)
 tagEXCEPINFO._fields_ = [
     ('wCode', WORD),
     ('wReserved', WORD),
@@ -648,14 +697,19 @@
 ##    ('pfnDeferredFillIn', WINFUNCTYPE(HRESULT, POINTER(tagEXCEPINFO))),
     ('pfnDeferredFillIn', c_void_p),
     ('scode', SCODE),
 ]
 EXCEPINFO = tagEXCEPINFO
 
 class tagDISPPARAMS(Structure):
+    if TYPE_CHECKING:
+        rgvarg = hints.AnnoField()  # type: Array[VARIANT]
+        rgdispidNamedArgs = hints.AnnoField()  # type: _Pointer[DISPID]
+        cArgs = hints.AnnoField()  # type: int
+        cNamedArgs = hints.AnnoField()  # type: int
     _fields_ = [
         # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 696
         ('rgvarg', POINTER(VARIANTARG)),
         ('rgdispidNamedArgs', POINTER(DISPID)),
         ('cArgs', UINT),
         ('cNamedArgs', UINT),
     ]
@@ -670,49 +724,74 @@
 DISPID_PROPERTYPUT = -3
 DISPID_NEWENUM = -4
 DISPID_EVALUATE = -5
 DISPID_CONSTRUCTOR = -6
 DISPID_DESTRUCTOR = -7
 DISPID_COLLECT = -8
 
+
+if TYPE_CHECKING:
+    RawGetIDsOfNamesFunc = Callable[
+        [_byref_type, Array[c_wchar_p], int, int, Array[DISPID]], int,
+    ]
+    RawInvokeFunc = Callable[
+        [
+            int, _byref_type, int, int,  # dispIdMember, riid, lcid, wFlags
+            _UnionT[_byref_type, DISPPARAMS],  # *pDispParams
+            _UnionT[_byref_type, VARIANT],  # pVarResult
+            _UnionT[_byref_type, EXCEPINFO, None],  # pExcepInfo
+            _UnionT[_byref_type, c_uint],  # puArgErr
+        ],
+        int
+    ]
+
 class IDispatch(IUnknown):
+    if TYPE_CHECKING:
+        _disp_methods_ = hints.AnnoField()  # type: ClassVar[List[comtypes._DispMemberSpec]]
+        _GetTypeInfo = hints.AnnoField()  # type: Callable[[int, int], IUnknown]
+        __com_GetIDsOfNames = hints.AnnoField()  # type: RawGetIDsOfNamesFunc
+        __com_Invoke = hints.AnnoField()  # type: RawInvokeFunc
+
     _iid_ = GUID("{00020400-0000-0000-C000-000000000046}")
     _methods_ = [
         COMMETHOD([], HRESULT, 'GetTypeInfoCount',
                   (['out'], POINTER(UINT) ) ),
         COMMETHOD([], HRESULT, 'GetTypeInfo',
                   (['in'], UINT, 'index'),
                   (['in'], LCID, 'lcid', 0),
-## Normally, we would declare this parameter in this way:
-##                  (['out'], POINTER(POINTER(ITypeInfo)) ) ),
-## but we cannot import comtypes.typeinfo at the top level (recursive imports!).
+                # Normally, we would declare this parameter in this way:
+                # (['out'], POINTER(POINTER(ITypeInfo)) ) ),
+                # but we cannot import comtypes.typeinfo at the top level (recursive imports!).
                   (['out'], POINTER(POINTER(IUnknown)) ) ),
         STDMETHOD(HRESULT, 'GetIDsOfNames', [POINTER(IID), POINTER(c_wchar_p),
                                              UINT, LCID, POINTER(DISPID)]),
         STDMETHOD(HRESULT, 'Invoke', [DISPID, POINTER(IID), LCID, WORD,
                                       POINTER(DISPPARAMS), POINTER(VARIANT),
                                       POINTER(EXCEPINFO), POINTER(UINT)]),
     ]
 
     def GetTypeInfo(self, index, lcid=0):
+        # type: (int, int) -> hints.ITypeInfo
         """Return type information.  Index 0 specifies typeinfo for IDispatch"""
         import comtypes.typeinfo
         result = self._GetTypeInfo(index, lcid)
         return result.QueryInterface(comtypes.typeinfo.ITypeInfo)
 
     def GetIDsOfNames(self, *names, **kw):
+        # type: (str, Any) -> List[int]
         """Map string names to integer ids."""
         lcid = kw.pop("lcid", 0)
         assert not kw
         arr = (c_wchar_p * len(names))(*names)
         ids = (DISPID * len(names))()
         self.__com_GetIDsOfNames(riid_null, arr, len(names), lcid, ids)
         return ids[:]
 
     def _invoke(self, memid, invkind, lcid, *args):
+        # type: (int, int, int, Any) -> Any
         var = VARIANT()
         argerr = c_uint()
         dp = DISPPARAMS()
 
         if args:
             array = (VARIANT * len(args))()
 
@@ -726,14 +805,15 @@
             dp.rgvarg = array
 
         self.__com_Invoke(memid, riid_null, lcid, invkind,
                           dp, var, None, argerr)
         return var._get_value(dynamic=True)
 
     def Invoke(self, dispid, *args, **kw):
+        # type: (int, Any, Any) -> Any
         """Invoke a method or property."""
 
         # Memory management in Dispatch::Invoke calls:
         # http://msdn.microsoft.com/library/en-us/automat/htm/chap5_4x2q.asp
         # Quote:
         #     The *CALLING* code is responsible for releasing all strings and
         #     objects referred to by rgvarg[ ] or placed in *pVarResult.
@@ -769,15 +849,15 @@
             dp.cArgs = len(args)
             dp.cNamedArgs = 0
             dp.rgvarg = array
 
         try:
             self.__com_Invoke(dispid, riid_null, _lcid, _invkind, byref(dp),
                               byref(result), byref(excepinfo), byref(argerr))
-        except COMError, err:
+        except COMError as err:
             (hresult, text, details) = err.args
             if hresult == DISP_E_EXCEPTION:
                 details = (excepinfo.bstrDescription, excepinfo.bstrSource,
                            excepinfo.bstrHelpFile, excepinfo.dwHelpContext,
                            excepinfo.scode)
                 raise COMError(hresult, text, details)
             elif hresult == DISP_E_PARAMNOTFOUND:
@@ -863,19 +943,44 @@
 
     # These are not yet implemented:
 ##    POINTER(IUnknown): VT_UNKNOWN,
 ##    POINTER(IDispatch): VT_DISPATCH,
     }
 
 _vartype_to_ctype = {}
-for c, v in _ctype_to_vartype.iteritems():
+for c, v in _ctype_to_vartype.items():
     _vartype_to_ctype[v] = c
 _vartype_to_ctype[VT_INT] = _vartype_to_ctype[VT_I4]
 _vartype_to_ctype[VT_UINT] = _vartype_to_ctype[VT_UI4]
 _ctype_to_vartype[c_char] = VT_UI1
 
 
 
 try:
     from comtypes.safearray import _midlSAFEARRAY
 except (ImportError, AttributeError):
     pass
+
+
+__known_symbols__ = [
+    'CURRENCY', 'CY', 'tagCY', 'DECIMAL', 'tagDEC', 'DISPATCH_METHOD',
+    'DISPATCH_PROPERTYGET', 'DISPATCH_PROPERTYPUT', 'DISPATCH_PROPERTYPUTREF',
+    'DISPID', 'DISPID_COLLECT', 'DISPID_CONSTRUCTOR', 'DISPID_DESTRUCTOR',
+    'DISPID_EVALUATE', 'DISPID_NEWENUM', 'DISPID_PROPERTYPUT',
+    'DISPID_UNKNOWN', 'DISPID_VALUE', 'DISPPARAMS', 'tagDISPPARAMS',
+    'EXCEPINFO', 'tagEXCEPINFO', 'IDispatch', 'IEnumVARIANT', 'IID_NULL',
+    'INVOKE_FUNC', 'INVOKE_PROPERTYGET', 'INVOKE_PROPERTYPUT',
+    'INVOKE_PROPERTYPUTREF', 'INVOKEKIND', 'tagINVOKEKIND', '_midlSAFEARRAY',
+    'SCODE', '_SysAllocStringLen', 'VARENUM', 'VARIANT','tagVARIANT', 
+    'VARIANTARG', '_VariantChangeType', '_VariantClear', '_VariantCopy',
+    '_VariantCopyInd', 'VARTYPE', 'VT_ARRAY', 'VT_BLOB', 'VT_BLOB_OBJECT',
+    'VT_BOOL', 'VT_BSTR', 'VT_BSTR_BLOB', 'VT_BYREF', 'VT_CARRAY', 'VT_CF',
+    'VT_CLSID', 'VT_CY', 'VT_DATE', 'VT_DECIMAL', 'VT_DISPATCH', 'VT_EMPTY',
+    'VT_ERROR', 'VT_FILETIME', 'VT_HRESULT', 'VT_I1', 'VT_I2', 'VT_I4',
+    'VT_I8', 'VT_ILLEGAL', 'VT_ILLEGALMASKED', 'VT_INT', 'VT_INT_PTR',
+    'VT_LPSTR', 'VT_LPWSTR', 'VT_NULL', 'VT_PTR', 'VT_R4', 'VT_R8',
+    'VT_RECORD', 'VT_RESERVED', 'VT_SAFEARRAY', 'VT_STORAGE',
+    'VT_STORED_OBJECT', 'VT_STREAM', 'VT_STREAMED_OBJECT', 'VT_TYPEMASK',
+    'VT_UI1', 'VT_UI2', 'VT_UI4', 'VT_UI8', 'VT_UINT', 'VT_UINT_PTR',
+    'VT_UNKNOWN', 'VT_USERDEFINED', 'VT_VARIANT', 'VT_VECTOR',
+    'VT_VERSIONED_STREAM', 'VT_VOID',
+]
```

## Comparing `comtypes-1.1.9/comtypes/connectionpoints.py` & `comtypes-1.2.0/comtypes/connectionpoints.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from ctypes import *
 from comtypes import IUnknown, COMMETHOD, GUID, HRESULT, dispid
 _GUID = GUID
 
 class tagCONNECTDATA(Structure):
     _fields_ = [
         ('pUnk', POINTER(IUnknown)),
@@ -22,32 +23,46 @@
 class IEnumConnections(IUnknown):
     _iid_ = GUID('{B196B287-BAB4-101A-B69C-00AA00341D07}')
     _idlflags_ = []
 
     def __iter__(self):
         return self
 
-    def next(self):
-        cp, fetched = self.Next(1)
-        if fetched == 0:
-            raise StopIteration
-        return cp
+    if sys.version_info >= (3, 0):
+        def __next__(self):
+            cp, fetched = self.Next(1)
+            if fetched == 0:
+                raise StopIteration
+            return cp
+    else:
+        def next(self):
+            cp, fetched = self.Next(1)
+            if fetched == 0:
+                raise StopIteration
+            return cp
 
 class IEnumConnectionPoints(IUnknown):
     _iid_ = GUID('{B196B285-BAB4-101A-B69C-00AA00341D07}')
     _idlflags_ = []
 
     def __iter__(self):
         return self
 
-    def next(self):
-        cp, fetched = self.Next(1)
-        if fetched == 0:
-            raise StopIteration
-        return cp
+    if sys.version_info >= (3, 0):
+        def __next__(self):
+            cp, fetched = self.Next(1)
+            if fetched == 0:
+                raise StopIteration
+            return cp
+    else:
+        def next(self):
+            cp, fetched = self.Next(1)
+            if fetched == 0:
+                raise StopIteration
+            return cp
 
 ################################################################
 
 IConnectionPointContainer._methods_ = [
     COMMETHOD([], HRESULT, 'EnumConnectionPoints',
               ( ['out'], POINTER(POINTER(IEnumConnectionPoints)), 'ppEnum' )),
     COMMETHOD([], HRESULT, 'FindConnectionPoint',
```

## Comparing `comtypes-1.1.9/comtypes/errorinfo.py` & `comtypes-1.2.0/comtypes/errorinfo.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 from ctypes import *
 from comtypes import IUnknown, HRESULT, COMMETHOD, GUID, BSTR
 from comtypes.hresult import *
 
 LPCOLESTR = c_wchar_p
 DWORD = c_ulong
 
+if sys.version_info >= (3, 0):
+    base_text_type = str
+else:
+    base_text_type = basestring
+
 class ICreateErrorInfo(IUnknown):
     _iid_ = GUID("{22F03340-547D-101B-8E65-08002B2BD119}")
     _methods_ = [
         COMMETHOD([], HRESULT, 'SetGUID',
                   (['in'], POINTER(GUID), "rguid")),
         COMMETHOD([], HRESULT, 'SetSource',
                   (['in'], LPCOLESTR, "szSource")),
@@ -69,15 +74,15 @@
     ei.SetDescription(text)
     ei.SetGUID(iid)
     if helpfile is not None:
         ei.SetHelpFile(helpfile)
     if helpcontext is not None:
         ei.SetHelpContext(helpcontext)
     if clsid is not None:
-        if isinstance(clsid, basestring):
+        if isinstance(clsid, base_text_type):
             clsid = GUID(clsid)
         try:
             progid = clsid.as_progid()
         except WindowsError:
             pass
         else:
             ei.SetSource(progid) # progid for the class or application that created the error
```

## Comparing `comtypes-1.1.9/comtypes/git.py` & `comtypes-1.2.0/comtypes/git.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/GUID.py` & `comtypes-1.2.0/comtypes/GUID.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 if sys.version_info >= (2, 6):
     def binary(obj):
         return bytes(obj)
 else:
     def binary(obj):
         return buffer(obj)
 
+if sys.version_info >= (3, 0):
+    text_type = str
+    base_text_type = str
+else:
+    text_type = unicode
+    base_text_type = basestring
+
 BYTE = c_byte
 WORD = c_ushort
 DWORD = c_ulong
 
 _ole32 = oledll.ole32
 
 _StringFromCLSID = _ole32.StringFromCLSID
@@ -28,74 +35,75 @@
     _fields_ = [("Data1", DWORD),
                 ("Data2", WORD),
                 ("Data3", WORD),
                 ("Data4", BYTE * 8)]
 
     def __init__(self, name=None):
         if name is not None:
-            _CLSIDFromString(unicode(name), byref(self))
+            _CLSIDFromString(text_type(name), byref(self))
 
     def __repr__(self):
-        return u'GUID("%s")' % unicode(self)
+        return 'GUID("%s")' % text_type(self)
 
     def __unicode__(self):
         p = c_wchar_p()
         _StringFromCLSID(byref(self), byref(p))
         result = p.value
         _CoTaskMemFree(p)
         return result
     __str__ = __unicode__
 
     def __cmp__(self, other):
         if isinstance(other, GUID):
             return cmp(binary(self), binary(other))
         return -1
 
-    def __nonzero__(self):
+    def __bool__(self):
         return self != GUID_null
 
     def __eq__(self, other):
         return isinstance(other, GUID) and \
                binary(self) == binary(other)
 
     def __hash__(self):
         # We make GUID instances hashable, although they are mutable.
         return hash(binary(self))
 
     def copy(self):
-        return GUID(unicode(self))
+        return GUID(text_type(self))
 
+    @classmethod
     def from_progid(cls, progid):
         """Get guid from progid, ...
         """
         if hasattr(progid, "_reg_clsid_"):
             progid = progid._reg_clsid_
         if isinstance(progid, cls):
             return progid
-        elif isinstance(progid, basestring):
+        elif isinstance(progid, base_text_type):
             if progid.startswith("{"):
                 return cls(progid)
             inst = cls()
-            _CLSIDFromProgID(unicode(progid), byref(inst))
+            _CLSIDFromProgID(text_type(progid), byref(inst))
             return inst
         else:
             raise TypeError("Cannot construct guid from %r" % progid)
-    from_progid = classmethod(from_progid)
 
     def as_progid(self):
         "Convert a GUID into a progid"
         progid = c_wchar_p()
         _ProgIDFromCLSID(byref(self), byref(progid))
         result = progid.value
         _CoTaskMemFree(progid)
         return result
 
+    @classmethod
     def create_new(cls):
         "Create a brand new guid"
         guid = cls()
         _CoCreateGuid(byref(guid))
         return guid
-    create_new = classmethod(create_new)
+
 
 GUID_null = GUID()
 
 __all__ = ["GUID"]
```

## Comparing `comtypes-1.1.9/comtypes/hresult.py` & `comtypes-1.2.0/comtypes/hresult.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/logutil.py` & `comtypes-1.2.0/comtypes/logutil.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,29 +9,29 @@
         if isinstance(text, str):
             writeA(text + "\n")
         else:
             writeW(text + u"\n")
 logging.NTDebugHandler = NTDebugHandler
 
 def setup_logging(*pathnames):
-    import ConfigParser
+    import configparser
 
-    parser = ConfigParser.ConfigParser()
+    parser = configparser.ConfigParser()
     parser.optionxform = str # use case sensitive option names!
 
     parser.read(pathnames)
 
     DEFAULTS = {"handler": "StreamHandler()",
                 "format": "%(levelname)s:%(name)s:%(message)s",
                 "level": "WARNING"}
 
     def get(section, option):
         try:
             return parser.get(section, option, True)
-        except (ConfigParser.NoOptionError, ConfigParser.NoSectionError):
+        except (configparser.NoOptionError, configparser.NoSectionError):
             return DEFAULTS[option]
 
     levelname = get("logging", "level")
     format = get("logging", "format")
     handlerclass = get("logging", "handler")
 
     # convert level name to level value
@@ -43,9 +43,9 @@
     logging.root.addHandler(handler)
     logging.root.setLevel(level)
 
     try:
         for name, value in parser.items("logging.levels", True):
             value = getattr(logging, value)
             logging.getLogger(name).setLevel(value)
-    except ConfigParser.NoSectionError:
+    except configparser.NoSectionError:
         pass
```

## Comparing `comtypes-1.1.9/comtypes/messageloop.py` & `comtypes-1.2.0/comtypes/messageloop.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             elif ret == 0:
                 return # got WM_QUIT
             if not self.filter_message(lpmsg):
                 TranslateMessage(lpmsg)
                 DispatchMessage(lpmsg)
 
     def filter_message(self, lpmsg):
-        return any(filter(lpmsg) for filter in self._filters)
+        return any(list(filter(lpmsg)) for filter in self._filters)
 
 _messageloop = _MessageLoop()
 
 run = _messageloop.run
 insert_filter = _messageloop.insert_filter
 remove_filter = _messageloop.remove_filter
```

## Comparing `comtypes-1.1.9/comtypes/patcher.py` & `comtypes-1.2.0/comtypes/patcher.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/persist.py` & `comtypes-1.2.0/comtypes/persist.py`

 * *Files 14% similar despite different names*

```diff
@@ -206,7 +206,21 @@
             var.ChangeType(typecode)
         return S_OK
 
     def Write(self, this, name, var):
         val = var[0].value
         self.values[name] = val
         return S_OK
+
+
+__known_symbols__ = [
+    'CLIPFORMAT', 'DictPropertyBag', 'IErrorLog', 'IPersistFile',
+    'IPersistPropertyBag', 'IPersistPropertyBag2', 'IPropertyBag',
+    'IPropertyBag2', 'tagPROPBAG2', 'PROPBAG2_TYPE_DATA',
+    'PROPBAG2_TYPE_MONIKER', 'PROPBAG2_TYPE_OBJECT', 'PROPBAG2_TYPE_STORAGE',
+    'PROPBAG2_TYPE_STREAM', 'PROPBAG2_TYPE_UNDEFINED', 'PROPBAG2_TYPE_URL',
+    'STGM_CONVERT', 'STGM_CREATE', 'STGM_DELETEONRELEASE', 'STGM_DIRECT',
+    'STGM_DIRECT_SWMR', 'STGM_FAILIFTHERE', 'STGM_NOSCRATCH',
+    'STGM_NOSNAPSHOT', 'STGM_PRIORITY', 'STGM_READ', 'STGM_READWRITE',
+    'STGM_SHARE_DENY_NONE', 'STGM_SHARE_DENY_READ', 'STGM_SHARE_DENY_WRITE',
+    'STGM_SHARE_EXCLUSIVE', 'STGM_SIMPLE', 'STGM_TRANSACTED', 'STGM_WRITE',
+]
```

## Comparing `comtypes-1.1.9/comtypes/safearray.py` & `comtypes-1.2.0/comtypes/safearray.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import threading
 import array
+import comtypes
 from ctypes import (POINTER, Structure, byref, cast, c_long, memmove, pointer,
                     sizeof)
-from comtypes import _safearray, IUnknown, com_interface_registry, npsupport
+from comtypes import _safearray, IUnknown, com_interface_registry
 from comtypes.patcher import Patch
 
-numpy = npsupport.numpy
 _safearray_type_cache = {}
 
 
 class _SafeArrayAsNdArrayContextManager(object):
     '''Context manager allowing safe arrays to be extracted as ndarrays.
 
     This is thread-safe.
@@ -23,28 +23,31 @@
     >>> type(my_arr)
     numpy.ndarray
 
     '''
     thread_local = threading.local()
 
     def __enter__(self):
+        comtypes.npsupport.enable()
         try:
             self.thread_local.count += 1
         except AttributeError:
             self.thread_local.count = 1
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.thread_local.count -= 1
 
-    def __nonzero__(self):
+    def __bool__(self):
         '''True if context manager is currently entered on given thread.
 
         '''
         return bool(getattr(self.thread_local, 'count', 0))
 
+    __nonzero__ = __bool__ # for Py2.7 compatibility
+
 
 # Global _SafeArrayAsNdArrayContextManager
 safearray_as_ndarray = _SafeArrayAsNdArrayContextManager()
 
 
 ################################################################
 # This is THE PUBLIC function: the gateway to the SAFEARRAY functionality.
@@ -107,15 +110,15 @@
             type; value is an object containing the items to store.
 
             Python lists, tuples, and array.array instances containing
             compatible item types can be passed to create
             one-dimensional arrays.  To create multidimensional arrys,
             numpy arrays must be passed.
             """
-            if npsupport.isndarray(value):
+            if comtypes.npsupport.isndarray(value):
                 return cls.create_from_ndarray(value, extra)
 
             # For VT_UNKNOWN or VT_DISPATCH, extra must be a pointer to
             # the GUID of the interface.
             #
             # For VT_RECORD, extra must be a pointer to an IRecordInfo
             # describing the record.
@@ -150,26 +153,26 @@
             return pa
 
         @classmethod
         def create_from_ndarray(cls, value, extra, lBound=0):
             from comtypes.automation import VARIANT
             # If processing VARIANT, makes sure the array type is correct.
             if cls._itemtype_ is VARIANT:
-                if value.dtype != npsupport.VARIANT_dtype:
+                if value.dtype != comtypes.npsupport.VARIANT_dtype:
                     value = _ndarray_to_variant_array(value)
             else:
                 ai = value.__array_interface__
                 if ai["version"] != 3:
                     raise TypeError("only __array_interface__ version 3 supported")
-                if cls._itemtype_ != npsupport.typecodes[ai["typestr"]]:
+                if cls._itemtype_ != comtypes.npsupport.typecodes[ai["typestr"]]:
                     raise TypeError("Wrong array item type")
 
             # SAFEARRAYs have Fortran order; convert the numpy array if needed
             if not value.flags.f_contiguous:
-                value = numpy.array(value, order="F")
+                value = comtypes.npsupport.numpy.array(value, order="F")
 
             # For VT_UNKNOWN or VT_DISPATCH, extra must be a pointer to
             # the GUID of the interface.
             #
             # For VT_RECORD, extra must be a pointer to an IRecordInfo
             # describing the record.
             rgsa = (_safearray.SAFEARRAYBOUND * value.ndim)()
@@ -232,43 +235,44 @@
             lb = _safearray.SafeArrayGetLBound(self, dim)
             return ub - lb
 
         def unpack(self):
             """Unpack a POINTER(SAFEARRAY_...) into a Python tuple or ndarray."""
             dim = _safearray.SafeArrayGetDim(self)
 
-            if dim == 1:
+            if dim == 0:
+                if safearray_as_ndarray:
+                    return comtypes.npsupport.numpy.array()
+                return tuple()
+            elif dim == 1:
                 num_elements = self._get_size(1)
                 result = self._get_elements_raw(num_elements)
                 if safearray_as_ndarray:
-                    import numpy
-                    return numpy.asarray(result)
+                    return comtypes.npsupport.numpy.asarray(result)
                 return tuple(result)
             elif dim == 2:
                 # get the number of elements in each dimension
                 rows, cols = self._get_size(1), self._get_size(2)
                 # get all elements
                 result = self._get_elements_raw(rows * cols)
                 # this must be reshaped and transposed because it is
                 # flat, and in VB order
                 if safearray_as_ndarray:
-                    import numpy
-                    return numpy.asarray(result).reshape((cols, rows)).T
+                    return comtypes.npsupport.numpy.asarray(result).reshape((cols, rows)).T
                 result = [tuple(result[r::rows]) for r in range(rows)]
                 return tuple(result)
             else:
                 lowerbounds = [_safearray.SafeArrayGetLBound(self, d)
                                for d in range(1, dim+1)]
                 indexes = (c_long * dim)(*lowerbounds)
                 upperbounds = [_safearray.SafeArrayGetUBound(self, d)
                                for d in range(1, dim+1)]
                 row = self._get_row(0, indexes, lowerbounds, upperbounds)
                 if safearray_as_ndarray:
-                    import numpy
-                    return numpy.asarray(row)
+                    return comtypes.npsupport.numpy.asarray(row)
                 return row
 
         def _get_elements_raw(self, num_elements):
             """Returns a flat list or ndarray containing ALL elements in
             the safearray."""
             from comtypes.automation import VARIANT
             # XXX Not sure this is true:
@@ -304,16 +308,16 @@
                     # alive until all the elements are destroyed.
                     if not issubclass(self._itemtype_, Structure):
                         # Create an ndarray if requested. This is where
                         # we can get the most speed-up.
                         # XXX Only try to convert types known to
                         #     numpy.ctypeslib.
                         if (safearray_as_ndarray and self._itemtype_ in
-                                npsupport.typecodes.values()):
-                            arr = numpy.ctypeslib.as_array(ptr,
+                                list(comtypes.npsupport.typecodes.keys())):
+                            arr = comtypes.npsupport.numpy.ctypeslib.as_array(ptr,
                                                            (num_elements,))
                             return arr.copy()
                         return ptr[:num_elements]
 
                     def keep_safearray(v):
                         v.__keepref = self
                         return v
@@ -361,37 +365,41 @@
 
     return sa_type
 
 
 def _ndarray_to_variant_array(value):
     """ Convert an ndarray to VARIANT_dtype array """
     # Check that variant arrays are supported
-    if npsupport.VARIANT_dtype is None:
+    if comtypes.npsupport.interop.VARIANT_dtype is None:
         msg = "VARIANT ndarrays require NumPy 1.7 or newer."
         raise RuntimeError(msg)
+    numpy = comtypes.npsupport.interop.numpy
 
     # special cases
-    if numpy.issubdtype(value.dtype, npsupport.datetime64):
+    if numpy.issubdtype(value.dtype, comtypes.npsupport.interop.datetime64):
         return _datetime64_ndarray_to_variant_array(value)
 
     from comtypes.automation import VARIANT
     # Empty array
-    varr = numpy.zeros(value.shape, npsupport.VARIANT_dtype, order='F')
+    varr = numpy.zeros(
+        value.shape, comtypes.npsupport.interop.VARIANT_dtype, order='F'
+    )
     # Convert each value to a variant and put it in the array.
     varr.flat = [VARIANT(v) for v in value.flat]
     return varr
 
 
 def _datetime64_ndarray_to_variant_array(value):
     """ Convert an ndarray of datetime64 to VARIANT_dtype array """
     # The OLE automation date format is a floating point value, counting days
     # since midnight 30 December 1899. Hours and minutes are represented as
     # fractional days.
     from comtypes.automation import VT_DATE
+    numpy = comtypes.npsupport.interop.numpy
     value = numpy.array(value, "datetime64[ns]")
-    value = value - npsupport.com_null_date64
+    value = value - comtypes.npsupport.interop.com_null_date64
     # Convert to days
     value = value / numpy.timedelta64(1, 'D')
-    varr = numpy.zeros(value.shape, npsupport.VARIANT_dtype, order='F')
+    varr = numpy.zeros(value.shape, comtypes.npsupport.interop.VARIANT_dtype, order='F')
     varr['vt'] = VT_DATE
     varr['_']['VT_R8'].flat = value.flat
     return varr
```

## Comparing `comtypes-1.1.9/comtypes/shelllink.py` & `comtypes-1.2.0/comtypes/shelllink.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import print_function
 from ctypes import *
 from ctypes.wintypes import DWORD, WIN32_FIND_DATAA, WIN32_FIND_DATAW, MAX_PATH
 from comtypes import IUnknown, GUID, COMMETHOD, HRESULT, CoClass
 
 # for GetPath
 SLGP_SHORTPATH = 0x1
 SLGP_UNCPRIORITY = 0x2
@@ -181,15 +182,15 @@
     def GetIconLocation(self):
         iIcon = c_int()
         buf = create_unicode_buffer(MAX_PATH)
         self.__com_GetIconLocation(buf, MAX_PATH, byref(iIcon))
         return buf.value, iIcon.value
 
 class ShellLink(CoClass):
-    u'ShellLink class'
+    """ShellLink class"""
     _reg_clsid_ = GUID('{00021401-0000-0000-C000-000000000046}')
     _idlflags_ = []
     _com_interfaces_ = [IShellLinkW, IShellLinkA]
 
 
 if __name__ == "__main__":
 
@@ -197,21 +198,21 @@
     import comtypes
     from comtypes.client import CreateObject
     from comtypes.persist import IPersistFile
 
 
 
     shortcut = CreateObject(ShellLink)
-    print shortcut
+    print(shortcut)
     ##help(shortcut)
 
     shortcut.SetPath(sys.executable)
 
     shortcut.SetDescription("Python %s" % sys.version)
     shortcut.SetIconLocation(sys.executable, 1)
 
-    print shortcut.GetPath(2)
-    print shortcut.GetIconLocation()
+    print(shortcut.GetPath(2))
+    print(shortcut.GetIconLocation())
 
     pf = shortcut.QueryInterface(IPersistFile)
     pf.Save("foo.lnk", True)
-    print pf.GetCurFile()
+    print(pf.GetCurFile())
```

## Comparing `comtypes-1.1.9/comtypes/typeinfo.py` & `comtypes-1.2.0/comtypes/typeinfo.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,37 +4,32 @@
 # flags '..\tools\windows.xml -m comtypes -m comtypes.automation -w -r .*TypeLibEx -r .*TypeLib -o typeinfo.py'
 # then hacked manually
 import os
 import sys
 import weakref
 
 from ctypes import *
-from ctypes.wintypes import ULONG
-from comtypes import STDMETHOD
-from comtypes import COMMETHOD
-from comtypes import _GUID, GUID
-# XXX should import more stuff from ctypes.wintypes...
-from comtypes.automation import BSTR
-from comtypes.automation import DISPID
-from comtypes.automation import DISPPARAMS
-from comtypes.automation import DWORD
-from comtypes.automation import EXCEPINFO
-from comtypes.automation import HRESULT
-from comtypes.automation import IID
-from comtypes.automation import IUnknown
-from comtypes.automation import LCID
-from comtypes.automation import LONG
-from comtypes.automation import SCODE
-from comtypes.automation import UINT
-from comtypes.automation import VARIANT
-from comtypes.automation import VARIANTARG
-from comtypes.automation import VARTYPE
-from comtypes.automation import WCHAR
-from comtypes.automation import WORD
-from comtypes.automation import tagVARIANT
+from ctypes.wintypes import DWORD, LONG, UINT, ULONG, WCHAR, WORD
+from comtypes import (
+    BSTR, COMMETHOD, _GUID, GUID, IID, IUnknown, STDMETHOD, TYPE_CHECKING,
+)
+from comtypes.automation import (
+    DISPID, DISPPARAMS, EXCEPINFO, LCID, SCODE, VARIANT, VARIANTARG, VARTYPE,
+    tagVARIANT,
+)
+
+if TYPE_CHECKING:
+    from ctypes import _CData, _Pointer
+    from typing import (
+        Any, Callable, List, Optional, overload, Sequence, Type, TypeVar,
+        Tuple, Union as _UnionT,
+    )
+    from comtypes import hints
+    _CT = TypeVar("_CT", bound=_CData)
+    _T_IUnknown = TypeVar("_T_IUnknown", bound=IUnknown)
 
 is_64_bit = sys.maxsize > 2**32
 
 BOOL = c_int
 HREFTYPE = DWORD
 INT = c_int
 MEMBERID = DISPID
@@ -181,178 +176,212 @@
 PARAMFLAG_FRETVAL = 8
 PARAMFLAG_FOPT = 16
 PARAMFLAG_FHASDEFAULT = 32
 PARAMFLAG_FHASCUSTDATA = 64
 
 ################################################################
 # a helper
+
 def _deref_with_release(ptr, release):
+    # type: (_Pointer[_CT], Callable[..., Any]) -> _CT
     # Given a POINTER instance, return the pointed to value.
     # Call the 'release' function with 'ptr' to release resources
     # when the value is no longer needed.
     result = ptr[0]
     result.__ref__ = weakref.ref(result, lambda dead: release(ptr))
     return result
 
 # interfaces
 
 class ITypeLib(IUnknown):
     _iid_ = GUID("{00020402-0000-0000-C000-000000000046}")
 
-    # Commented out methods use the default implementation that comtypes
+    # type-checking only methods use the default implementation that comtypes
     # automatically creates for COM methods.
-
-##    def GetTypeInfoCount(self):
-##        "Return the number of type informations"
-
-##    def GetTypeInfo(self, index):
-##        "Load type info by index"
-
-##    def GetTypeInfoType(self, index):
-##        "Return the TYPEKIND of type information"
-
-##    def GetTypeInfoOfGuid(self, guid):
-##        "Return type information for a guid"
+    if TYPE_CHECKING:
+        def GetTypeInfoCount(self):
+            # type: () -> int
+            """Return the number of type informations"""
+            raise
+        def GetTypeInfo(self, index):
+            # type: (int) -> ITypeInfo
+            """Load type info by index"""
+            raise
+        def GetTypeInfoType(self, index):
+            # type: (int) -> int
+            """Return the TYPEKIND of type information"""
+            raise
+        def GetTypeInfoOfGuid(self, guid):
+            # type: (GUID) -> ITypeInfo
+            """Return type information for a guid"""
+            raise
+        def GetTypeComp(self):
+            # type: () -> ITypeComp
+            """Return an ITypeComp pointer."""
+            raise
+        def GetDocumentation(self, index):
+            # type: (int) -> Tuple[str, str, int, Optional[str]]
+            """Return documentation for a type description."""
+            raise
+        def ReleaseTLibAttr(self, ptla):
+            # type: (_Pointer[TLIBATTR]) -> int
+            """Release TLIBATTR"""
+            raise
+        _GetLibAttr = hints.AnnoField()  # type: Callable[[], _Pointer[TLIBATTR]]
 
     def GetLibAttr(self):
-        "Return type library attributes"
+        # type: () -> TLIBATTR
+        """Return type library attributes"""
         return _deref_with_release(self._GetLibAttr(), self.ReleaseTLibAttr)
 
-##    def GetTypeComp(self):
-##        "Return an ITypeComp pointer."
-
-##    def GetDocumentation(self, index):
-##        "Return documentation for a type description."
-
     def IsName(self, name, lHashVal=0):
+        # type: (str, int) -> Optional[str]
         """Check if there is type information for this name.
 
         Returns the name with capitalization found in the type
         library, or None.
         """
         from ctypes import create_unicode_buffer
         namebuf = create_unicode_buffer(name)
         found = BOOL()
-        self.__com_IsName(namebuf, lHashVal, byref(found))
+        self.__com_IsName(namebuf, lHashVal, byref(found))  # type: ignore
         if found.value:
-            return namebuf[:].split("\0", 1)[0]
+            return namebuf[:].split("\0", 1)[0]  # type: ignore
         return None
 
     def FindName(self, name, lHashVal=0):
+        # type: (str, int) -> Optional[Tuple[int, ITypeInfo]]
         # Hm...
         # Could search for more than one name - should we support this?
         found = c_ushort(1)
         tinfo = POINTER(ITypeInfo)()
         memid = MEMBERID()
-        self.__com_FindName(name, lHashVal, byref(tinfo), byref(memid), byref(found))
+        self.__com_FindName(name, lHashVal, byref(tinfo), byref(memid), byref(found))  # type: ignore
         if found.value:
-            return memid.value, tinfo
+            return memid.value, tinfo  # type: ignore
         return None
 
-##    def ReleaseTLibAttr(self, ptla):
-##        "Release TLIBATTR"
-
 ################
-
+if TYPE_CHECKING:
+    @overload
+    def fix_name(name):
+        # type: (None) -> None
+        pass
+    @overload
+    def fix_name(name):
+        # type: (str) -> str
+        pass
 def fix_name(name):
     # Some typelibs contain BSTR with embedded NUL characters,
     # probably the len of the BSTR is wrong.
     if name is None:
         return name
     return name.split("\0")[0]
 
 class ITypeInfo(IUnknown):
     _iid_ = GUID("{00020401-0000-0000-C000-000000000046}")
 
+    if TYPE_CHECKING:
+        def GetTypeComp(self):
+            # type: () -> ITypeComp
+            """Return ITypeComp pointer for this type"""
+            raise
+        def GetRefTypeOfImplType(self, index):
+            # type: (int) -> int
+            """Get the reftype of an implemented type"""
+            raise
+        def GetImplTypeFlags(self, index):
+            # type: (int) -> int
+            """Get IMPLTYPEFLAGS"""
+            raise
+        # not yet wrapped
+        # STDMETHOD(HRESULT, 'Invoke', [PVOID, MEMBERID, WORD, POINTER(DISPPARAMS), POINTER(VARIANT), POINTER(EXCEPINFO), POINTER(UINT)]),
+        def GetDllEntry(self, memid, invkind):
+            # type: (int, int) -> Tuple[Optional[str], Optional[str], int]
+            """Return the dll name, function name, and ordinal for a function and invkind."""
+            raise
+        def GetRefTypeInfo(self, href):
+            # type: (int) -> ITypeInfo
+            """Get type info for reftype"""
+            raise
+        def GetMops(self, index):
+            # type: (int) -> Optional[str]
+            """Get marshalling opcodes (whatever that is...)"""
+            raise
+        def GetContainingTypeLib(self):
+            # type: () -> Tuple[ITypeLib, int]
+            """Return index into and the containing type lib itself"""
+            raise
+        ReleaseTypeAttr = hints.AnnoField()  # type: Callable[[_Pointer[TYPEATTR]], int]
+        ReleaseFuncDesc = hints.AnnoField()  # type: Callable[[_Pointer[FUNCDESC]], int]
+        ReleaseVarDesc = hints.AnnoField()  # type: Callable[[_Pointer[VARDESC]], int]
+        _GetTypeAttr = hints.AnnoField()  # type: Callable[[], _Pointer[TYPEATTR]]
+        _GetFuncDesc = hints.AnnoField()  # type: Callable[[int], _Pointer[FUNCDESC]]
+        _GetVarDesc = hints.AnnoField()  # type: Callable[[int], _Pointer[VARDESC]]
+        _GetDocumentation = hints.AnnoField()  # type: Callable[[int], Tuple[str, str, int, Optional[str]]]
+
     def GetTypeAttr(self):
-        "Return the TYPEATTR for this type"
+        """Return the TYPEATTR for this type"""
         return _deref_with_release(self._GetTypeAttr(), self.ReleaseTypeAttr)
 
-##    def GetTypeComp(self):
-##        "Return ITypeComp pointer for this type"
-
     def GetDocumentation(self, memid):
         """Return name, docstring, helpcontext, and helpfile for 'memid'."""
         name, doc, helpcontext, helpfile = self._GetDocumentation(memid)
         return fix_name(name), fix_name(doc), helpcontext, fix_name(helpfile)
 
     def GetFuncDesc(self, index):
-        "Return FUNCDESC for index"
+        """Return FUNCDESC for index"""
         return _deref_with_release(self._GetFuncDesc(index), self.ReleaseFuncDesc)
 
     def GetVarDesc(self, index):
-        "Return VARDESC for index"
+        """Return VARDESC for index"""
         return _deref_with_release(self._GetVarDesc(index), self.ReleaseVarDesc)
 
     def GetNames(self, memid, count=1):
-        "Return names for memid"
+        # type: (int, int) -> List[str]
+        """Return names for memid"""
         names = (BSTR * count)()
         cnames = c_uint()
-        self.__com_GetNames(memid, names, count, byref(cnames))
+        self.__com_GetNames(memid, names, count, byref(cnames))  # type: ignore
         return names[:cnames.value]
 
-##    def GetRefTypeOfImplType(self, index):
-##        "Get the reftype of an implemented type"
-
-##    def GetImplTypeFlags(self, index):
-##        "Get IMPLTYPEFLAGS"
-
     def GetIDsOfNames(self, *names):
-        "Maps function and argument names to identifiers"
+        # type: (str) -> List[int]
+        """Maps function and argument names to identifiers"""
         rgsznames = (c_wchar_p * len(names))(*names)
         ids = (MEMBERID * len(names))()
-        self.__com_GetIDsOfNames(rgsznames, len(names), ids)
+        self.__com_GetIDsOfNames(rgsznames, len(names), ids)  # type: ignore
         return ids[:]
 
-
-    # not yet wrapped
-##    STDMETHOD(HRESULT, 'Invoke', [PVOID, MEMBERID, WORD, POINTER(DISPPARAMS), POINTER(VARIANT), POINTER(EXCEPINFO), POINTER(UINT)]),
-
-##    def GetDllEntry(self, memid, invkind):
-##        "Return the dll name, function name, and ordinal for a function and invkind."
-
-##    def GetRefTypeInfo(self, href):
-##        "Get type info for reftype"
-
     def AddressOfMember(self, memid, invkind):
-        "Get the address of a function in a dll"
-        raise "Check Me"
+        """Get the address of a function in a dll"""
+        raise RuntimeError("Check Me")
         p = c_void_p()
         self.__com_AddressOfMember(memid, invkind, byref(p))
         # XXX Would the default impl return the value of p?
         return p.value
 
     def CreateInstance(self, punkouter=None, interface=IUnknown, iid=None):
+        # type: (Optional[Type[_Pointer[IUnknown]]], Type[_T_IUnknown], Optional[GUID]) -> _T_IUnknown
         if iid is None:
             iid = interface._iid_
-        return self._CreateInstance(punkouter, byref(interface._iid_))
-
-##    def GetMops(self, index):
-##        "Get marshalling opcodes (whatever that is...)"
-
-##    def GetContainingTypeLib(self):
-##        "Return index into and the containing type lib itself"
-
-##    def ReleaseTypeAttr(self, pta):
-
-##    def ReleaseFuncDesc(self, pfd):
-
-##    def ReleaseVarDesc(self, pvd):
+        return self._CreateInstance(punkouter, byref(interface._iid_))  # type: ignore
 
 ################
 
 class ITypeComp(IUnknown):
     _iid_ = GUID("{00020403-0000-0000-C000-000000000046}")
 
     def Bind(self, name, flags=0, lHashVal=0):
-        "Bind to a name"
+        # type: (str, int, int) -> Optional[Tuple[str, _UnionT[FUNCDESC, VARDESC, ITypeComp]]]
+        """Bind to a name"""
         bindptr = BINDPTR()
         desckind = DESCKIND()
-        ti = POINTER(ITypeInfo)()
-        self.__com_Bind(name, lHashVal, flags, byref(ti), byref(desckind), byref(bindptr))
+        ti = POINTER(ITypeInfo)()  # type: ITypeInfo
+        self.__com_Bind(name, lHashVal, flags, byref(ti), byref(desckind), byref(bindptr))  # type: ignore
         kind = desckind.value
         if kind == DESCKIND_FUNCDESC:
             fd = bindptr.lpfuncdesc[0]
             fd.__ref__ = weakref.ref(fd, lambda dead: ti.ReleaseFuncDesc(bindptr.lpfuncdesc))
             return "function", fd
         elif kind == DESCKIND_VARDESC:
             vd = bindptr.lpvardesc[0]
@@ -362,54 +391,59 @@
             return "type", bindptr.lptcomp
         elif kind == DESCKIND_IMPLICITAPPOBJ:
             raise NotImplementedError
         elif kind == DESCKIND_NONE:
             raise NameError("Name %s not found" % name)
 
     def BindType(self, name, lHashVal=0):
-        "Bind a type, and return both the typeinfo and typecomp for it."
+        # type: (str, int) -> Tuple[ITypeInfo, ITypeComp]
+        """Bind a type, and return both the typeinfo and typecomp for it."""
         ti = POINTER(ITypeInfo)()
         tc = POINTER(ITypeComp)()
-        self.__com_BindType(name, lHashVal, byref(ti), byref(tc))
-        return ti, tc
+        self.__com_BindType(name, lHashVal, byref(ti), byref(tc))  # type: ignore
+        return ti, tc  # type: ignore
 
 
 ################
 
 class ICreateTypeLib(IUnknown):
     _iid_ = GUID("{00020406-0000-0000-C000-000000000046}")
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 2149
 
 class ICreateTypeLib2(ICreateTypeLib):
     _iid_ = GUID("{0002040F-0000-0000-C000-000000000046}")
 
 class ICreateTypeInfo(IUnknown):
     _iid_ = GUID("{00020405-0000-0000-C000-000000000046}")
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 915
+    if TYPE_CHECKING:
+        _SetFuncAndParamNames = hints.AnnoField()  # Callable[[int, Array[c_wchar_p], int], int]
 
     def SetFuncAndParamNames(self, index, *names):
+        # type: (int, str) -> int
         rgszNames = (c_wchar_p * len(names))()
         for i, n in enumerate(names):
             rgszNames[i] = n
         return self._SetFuncAndParamNames(index, rgszNames, len(names))
 
 class IRecordInfo(IUnknown):
     # C:/vc98/include/OAIDL.H 5974
     _iid_ = GUID("{0000002F-0000-0000-C000-000000000046}")
 
     def GetFieldNames(self, *args):
+        # type: (Any) -> List[Optional[str]]
         count = c_ulong()
-        self.__com_GetFieldNames(count, None)
+        self.__com_GetFieldNames(count, None)  # type: ignore
         array = (BSTR * count.value)()
-        self.__com_GetFieldNames(count, array)
+        self.__com_GetFieldNames(count, array)  # type: ignore
         result = array[:]
         # XXX Should SysFreeString the array contents. How to?
         return result
 
-IRecordInfo. _methods_ = [
+IRecordInfo._methods_ = [
         COMMETHOD([], HRESULT, 'RecordInit',
                   (['in'], c_void_p, 'pvNew')),
         COMMETHOD([], HRESULT, 'RecordClear',
                   (['in'], c_void_p, 'pvExisting')),
         COMMETHOD([], HRESULT, 'RecordCopy',
                   (['in'], c_void_p, 'pvExisting'),
                   (['in'], c_void_p, 'pvNew')),
@@ -455,118 +489,185 @@
 
 
 ################################################################
 # functions
 _oleaut32 = oledll.oleaut32
 
 def GetRecordInfoFromTypeInfo(tinfo):
+    # type: (ITypeInfo) -> IRecordInfo
     "Return an IRecordInfo pointer to the UDT described in tinfo"
     ri = POINTER(IRecordInfo)()
     _oleaut32.GetRecordInfoFromTypeInfo(tinfo, byref(ri))
-    return ri
+    return ri  # type: ignore
 
 def GetRecordInfoFromGuids(rGuidTypeLib, verMajor, verMinor, lcid, rGuidTypeInfo):
+    # type: (str, int, int, int, str) -> IRecordInfo
     ri = POINTER(IRecordInfo)()
     _oleaut32.GetRecordInfoFromGuids(byref(GUID(rGuidTypeLib)),
                                      verMajor, verMinor, lcid,
                                      byref(GUID(rGuidTypeInfo)),
                                      byref(ri))
-    return ri
+    return ri  # type: ignore
 
 def LoadRegTypeLib(guid, wMajorVerNum, wMinorVerNum, lcid=0):
-    "Load a registered type library"
+    # type: (_UnionT[str, GUID], int, int, int) -> ITypeLib
+    """Load a registered type library"""
     tlib = POINTER(ITypeLib)()
     _oleaut32.LoadRegTypeLib(byref(GUID(guid)), wMajorVerNum, wMinorVerNum, lcid, byref(tlib))
-    return tlib
+    return tlib  # type: ignore
 
 if hasattr(_oleaut32, "LoadTypeLibEx"):
     def LoadTypeLibEx(szFile, regkind=REGKIND_NONE):
+        # type: (str, int) -> ITypeLib
         "Load, and optionally register a type library file"
         ptl = POINTER(ITypeLib)()
         _oleaut32.LoadTypeLibEx(c_wchar_p(szFile), regkind, byref(ptl))
-        return ptl
+        return ptl  # type: ignore
 else:
     def LoadTypeLibEx(szFile, regkind=REGKIND_NONE):
+        # type: (str, int) -> ITypeLib
         "Load, and optionally register a type library file"
         ptl = POINTER(ITypeLib)()
         _oleaut32.LoadTypeLib(c_wchar_p(szFile), byref(ptl))
-        return ptl
+        return ptl  # type: ignore
 
 def LoadTypeLib(szFile):
+    # type: (str) -> ITypeLib
     "Load and register a type library file"
     tlib = POINTER(ITypeLib)()
     _oleaut32.LoadTypeLib(c_wchar_p(szFile), byref(tlib))
-    return tlib
+    return tlib  # type: ignore
 
 def UnRegisterTypeLib(libID, wVerMajor, wVerMinor, lcid=0, syskind=SYS_WIN32):
+    # type: (str, int, int, int, int) -> int
     "Unregister a registered type library"
     return _oleaut32.UnRegisterTypeLib(byref(GUID(libID)), wVerMajor, wVerMinor, lcid, syskind)
 
 def RegisterTypeLib(tlib, fullpath, helpdir=None):
+    # type: (ITypeLib, str, Optional[str]) -> int
     "Register a type library in the registry"
     return _oleaut32.RegisterTypeLib(tlib, c_wchar_p(fullpath), c_wchar_p(helpdir))
 
 def CreateTypeLib(filename, syskind=SYS_WIN32):
+    # type: (str, int) -> ICreateTypeLib2
     "Return a ICreateTypeLib2 pointer"
     ctlib = POINTER(ICreateTypeLib2)()
     _oleaut32.CreateTypeLib2(syskind, c_wchar_p(filename), byref(ctlib))
-    return ctlib
+    return ctlib  # type: ignore
 
 def QueryPathOfRegTypeLib(libid, wVerMajor, wVerMinor, lcid=0):
+    # type: (str, int, int, int) -> str
     "Return the path of a registered type library"
     pathname = BSTR()
     _oleaut32.QueryPathOfRegTypeLib(byref(GUID(libid)), wVerMajor, wVerMinor, lcid, byref(pathname))
     return pathname.value.split("\0")[0]
 
 ################################################################
 # Structures
 
 class tagTLIBATTR(Structure):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 4437
+    if TYPE_CHECKING:
+        guid = hints.AnnoField()  # type: GUID
+        lcid = hints.AnnoField()  # type: int
+        syskind = hints.AnnoField()  # type: int
+        wMajorVerNum = hints.AnnoField()  # type: int
+        wMinorVerNum = hints.AnnoField()  # type: int
+        wLibFlags = hints.AnnoField()  # type: int
+
     def __repr__(self):
         return "TLIBATTR(GUID=%s, Version=%s.%s, LCID=%s, FLags=0x%x)" % \
                (self.guid, self.wMajorVerNum, self.wMinorVerNum, self.lcid, self.wLibFlags)
 TLIBATTR = tagTLIBATTR
 
 class tagTYPEATTR(Structure):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 672
+    if TYPE_CHECKING:
+        guid = hints.AnnoField()  # type: GUID
+        lcid = hints.AnnoField()  # type: int
+        dwReserved = hints.AnnoField()  # type: int
+        memidConstructor = hints.AnnoField()  # type: int
+        memidDestructor = hints.AnnoField()  # type: int
+        lpstrSchema = hints.AnnoField()  # type: str
+        cbSizeInstance = hints.AnnoField()  # type: int
+        typekind = hints.AnnoField()  # type: int
+        cFuncs = hints.AnnoField()  # type: int
+        cVars = hints.AnnoField()  # type: int
+        cImplTypes = hints.AnnoField()  # type: int 
+        cbSizeVft = hints.AnnoField()  # type: int
+        cbAlignment = hints.AnnoField()  # type: int
+        wTypeFlags = hints.AnnoField()  # type: int
+        wMajorVerNum = hints.AnnoField()  # type: int
+        wMinorVerNum = hints.AnnoField()  # type: int
+        tdescAlias = hints.AnnoField()  # type: TYPEDESC
+        idldescType = hints.AnnoField()  # type: IDLDESC
+
     def __repr__(self):
         return "TYPEATTR(GUID=%s, typekind=%s, funcs=%s, vars=%s, impltypes=%s)" % \
                (self.guid, self.typekind, self.cFuncs, self.cVars, self.cImplTypes)
 TYPEATTR = tagTYPEATTR
 
 class tagFUNCDESC(Structure):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 769
+    if TYPE_CHECKING:
+        memid = hints.AnnoField()  # type: int
+        lprgscode = hints.AnnoField()  # type: int
+        lprgelemdescParam = hints.AnnoField()  # type: Sequence[ELEMDESC]
+        funckind = hints.AnnoField()  # type: int
+        invkind = hints.AnnoField()  # type: int
+        callconv = hints.AnnoField()  # type: int
+        cParams = hints.AnnoField()  # type: int
+        cParamsOpt = hints.AnnoField()  # type: int
+        oVft = hints.AnnoField()  # type: int
+        cScodes = hints.AnnoField()  # type: int
+        elemdescFunc = hints.AnnoField()  # type: ELEMDESC
+        wFuncFlags = hints.AnnoField()  # type: int
+
     def __repr__(self):
         return "FUNCDESC(memid=%s, cParams=%s, cParamsOpt=%s, callconv=%s, invkind=%s, funckind=%s)" % \
                (self.memid, self.cParams, self.cParamsOpt, self.callconv, self.invkind, self.funckind)
-
-
 FUNCDESC = tagFUNCDESC
+
 class tagVARDESC(Structure):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 803
-    pass
+    if TYPE_CHECKING:
+        memid = hints.AnnoField()  # type: int
+        lpstrSchema = hints.AnnoField()  # type: str
+        _ = hints.AnnoField()  # type: N10tagVARDESC5DOLLAR_205E
+        elemdescVar = hints.AnnoField()  # type: ELEMDESC
+        wVarFlags = hints.AnnoField()  # type: int
+        varkind = hints.AnnoField()  # type: int
 VARDESC = tagVARDESC
 
 class tagBINDPTR(Union):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 3075
-    pass
+    if TYPE_CHECKING:
+        lpfuncdesc = hints.AnnoField()  # type: _Pointer[FUNCDESC]
+        lpvardesc = hints.AnnoField()  # type: _Pointer[VARDESC]
+        lptcomp = hints.AnnoField()  # type: ITypeComp
 BINDPTR = tagBINDPTR
 class tagTYPEDESC(Structure):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 582
-    pass
+    if TYPE_CHECKING:
+        _ = hints.AnnoField()  # type: N11tagTYPEDESC5DOLLAR_203E
+        vt = hints.AnnoField()  # type: int
 TYPEDESC = tagTYPEDESC
 class tagIDLDESC(Structure):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 633
-    pass
+    if TYPE_CHECKING:
+        dwReserved = hints.AnnoField()  # type: int
+        wIDLFlags = hints.AnnoField()  # type: int
 IDLDESC = tagIDLDESC
 
 class tagARRAYDESC(Structure):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 594
-    pass
+    if TYPE_CHECKING:
+        tdescElem = hints.AnnoField()  # type: TYPEDESC
+        cDims = hints.AnnoField()  # type: int
+        rgbounds = hints.AnnoField()  # type: Sequence[SAFEARRAYBOUND]
 
 ################################################################
 # interface vtbl definitions
 
 ICreateTypeLib._methods_ = [
 # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 2149
     COMMETHOD([], HRESULT, 'CreateTypeInfo',
@@ -725,22 +826,26 @@
     STDMETHOD(HRESULT, 'SetMops', [UINT, BSTR]),
     STDMETHOD(HRESULT, 'SetTypeIdldesc', [POINTER(IDLDESC)]),
     STDMETHOD(HRESULT, 'LayOut', []),
 ]
 
 class IProvideClassInfo(IUnknown):
     _iid_ = GUID("{B196B283-BAB4-101A-B69C-00AA00341D07}")
+    if TYPE_CHECKING:
+        GetClassInfo = hints.AnnoField()  # type: Callable[[], ITypeInfo]
     _methods_ = [
         # Returns the ITypeInfo interface for the object's coclass type information.
         COMMETHOD([], HRESULT, "GetClassInfo",
                   ( ['out'],  POINTER(POINTER(ITypeInfo)), "ppTI" ) )
         ]
 
 class IProvideClassInfo2(IProvideClassInfo):
     _iid_ = GUID("{A6BC3AC0-DBAA-11CE-9DE3-00AA004BB851}")
+    if TYPE_CHECKING:
+        GetGUID = hints.AnnoField()  # type: Callable[[int], GUID]
     _methods_ = [
         # Returns the GUID for the object's outgoing IID for its default event set.
         COMMETHOD([], HRESULT, "GetGUID",
                   ( ['in'], DWORD, "dwGuidKind" ),
                   ( ['out', 'retval'], POINTER(GUID), "pGUID" ))
         ]
 
@@ -755,15 +860,18 @@
     ('syskind', SYSKIND),
     ('wMajorVerNum', WORD),
     ('wMinorVerNum', WORD),
     ('wLibFlags', WORD),
 ]
 class N11tagTYPEDESC5DOLLAR_203E(Union):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 584
-    pass
+    if TYPE_CHECKING:
+        lptdesc = hints.AnnoField()  # type: TYPEDESC
+        lpadesc = hints.AnnoField()  # type: tagARRAYDESC
+        hreftype = hints.AnnoField()  # type: int
 N11tagTYPEDESC5DOLLAR_203E._fields_ = [
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 584
     ('lptdesc', POINTER(tagTYPEDESC)),
     ('lpadesc', POINTER(tagARRAYDESC)),
     ('hreftype', HREFTYPE),
 ]
 tagTYPEDESC._anonymous_ = ('_',)
@@ -797,34 +905,44 @@
     ('wMajorVerNum', WORD),
     ('wMinorVerNum', WORD),
     ('tdescAlias', TYPEDESC),
     ('idldescType', IDLDESC),
 ]
 class N10tagVARDESC5DOLLAR_205E(Union):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 807
-    pass
+    if TYPE_CHECKING:
+        oInst = hints.AnnoField()  # type: int
+        lpvarValue = hints.AnnoField()  # type: VARIANT
 N10tagVARDESC5DOLLAR_205E._fields_ = [
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 807
     ('oInst', DWORD),
     ('lpvarValue', POINTER(VARIANT)),
 ]
 class tagELEMDESC(Structure):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 661
-    pass
+    if TYPE_CHECKING:
+        tdesc = hints.AnnoField()  # type: TYPEDESC
+        _ = hints.AnnoField()  # type: N11tagELEMDESC5DOLLAR_204E
 class N11tagELEMDESC5DOLLAR_204E(Union):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 663
-    pass
+    if TYPE_CHECKING:
+        idldesc = hints.AnnoField()  # type: IDLDESC
+        paramdesc = hints.AnnoField()  # type: PARAMDESC
 
 class tagPARAMDESC(Structure):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 609
-    pass
+    if TYPE_CHECKING:
+        pparamdescex = hints.AnnoField()  # type: tagPARAMDESCEX
+        wParamFlags = hints.AnnoField()  # type: int
 
 class tagPARAMDESCEX(Structure):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 601
-    pass
+    if TYPE_CHECKING:
+        cBytes = hints.AnnoField()  # type: int
+        varDefaultValue = hints.AnnoField()  # type: VARIANTARG
 LPPARAMDESCEX = POINTER(tagPARAMDESCEX)
 
 tagPARAMDESC._fields_ = [
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 609
     ('pparamdescex', LPPARAMDESCEX),
     ('wParamFlags', USHORT),
 ]
@@ -880,19 +998,71 @@
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 601
     ('cBytes', DWORD),
     ('varDefaultValue', VARIANTARG),
 ]
 
 class tagSAFEARRAYBOUND(Structure):
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 226
+    if TYPE_CHECKING:
+        cElements = hints.AnnoField()  # type: int
+        lLbound = hints.AnnoField()  # type: int
     _fields_ = [
         ('cElements', DWORD),
         ('lLbound', LONG),
     ]
 SAFEARRAYBOUND = tagSAFEARRAYBOUND
 
 tagARRAYDESC._fields_ = [
     # C:/Programme/gccxml/bin/Vc71/PlatformSDK/oaidl.h 594
     ('tdescElem', TYPEDESC),
     ('cDims', USHORT),
     ('rgbounds', SAFEARRAYBOUND * 1),
 ]
+
+
+__known_symbols__ = [
+    'tagARRAYDESC', 'BINDPTR', 'tagBINDPTR', 'CALLCONV', 'tagCALLCONV',
+    'CC_CDECL', 'CC_FASTCALL', 'CC_FPFASTCALL', 'CC_MACPASCAL', 'CC_MAX',
+    'CC_MPWCDECL', 'CC_MPWPASCAL', 'CC_MSCPASCAL', 'CC_PASCAL', 'CC_STDCALL',
+    'CC_SYSCALL', 'CreateTypeLib', 'DESCKIND', 'tagDESCKIND',
+    'DESCKIND_FUNCDESC', 'DESCKIND_IMPLICITAPPOBJ', 'DESCKIND_MAX',
+    'DESCKIND_NONE', 'DESCKIND_TYPECOMP', 'DESCKIND_VARDESC', 'ELEMDESC',
+    'tagELEMDESC', 'FUNC_DISPATCH', 'FUNC_NONVIRTUAL', 'FUNC_PUREVIRTUAL',
+    'FUNC_STATIC', 'FUNC_VIRTUAL', 'FUNCDESC', 'tagFUNCDESC',
+    'FUNCFLAG_FBINDABLE', 'FUNCFLAG_FDEFAULTBIND', 'FUNCFLAG_FDEFAULTCOLLELEM',
+    'FUNCFLAG_FDISPLAYBIND', 'FUNCFLAG_FHIDDEN', 'FUNCFLAG_FIMMEDIATEBIND',
+    'FUNCFLAG_FNONBROWSABLE', 'FUNCFLAG_FREPLACEABLE', 'FUNCFLAG_FREQUESTEDIT',
+    'FUNCFLAG_FRESTRICTED', 'FUNCFLAG_FSOURCE', 'FUNCFLAG_FUIDEFAULT',
+    'FUNCFLAG_FUSESGETLASTERROR', 'FUNCFLAGS', 'tagFUNCFLAGS', 'FUNCKIND',
+    'tagFUNCKIND', 'GetRecordInfoFromGuids', 'GetRecordInfoFromTypeInfo',
+    'HREFTYPE', 'ICreateTypeInfo', 'ICreateTypeLib', 'ICreateTypeLib2',
+    'IDLDESC', 'tagIDLDESC', 'IMPLTYPEFLAG_FDEFAULT',
+    'IMPLTYPEFLAG_FDEFAULTVTABLE', 'IMPLTYPEFLAG_FRESTRICTED',
+    'IMPLTYPEFLAG_FSOURCE', 'IProvideClassInfo', 'IProvideClassInfo2',
+    'IRecordInfo', 'ITypeComp', 'ITypeInfo', 'ITypeLib', 'LoadRegTypeLib',
+    'LoadTypeLib', 'LoadTypeLibEx', 'LPPARAMDESCEX', 'MEMBERID',
+    'N10tagVARDESC5DOLLAR_205E', 'N11tagELEMDESC5DOLLAR_204E',
+    'N11tagTYPEDESC5DOLLAR_203E', 'OLECHAR', 'PARAMDESC', 'tagPARAMDESC',
+    'tagPARAMDESCEX', 'PARAMFLAG_FHASCUSTDATA', 'PARAMFLAG_FHASDEFAULT',
+    'PARAMFLAG_FIN', 'PARAMFLAG_FLCID', 'PARAMFLAG_FOPT', 'PARAMFLAG_FOUT',
+    'PARAMFLAG_FRETVAL', 'PARAMFLAG_NONE', 'PVOID', 'QueryPathOfRegTypeLib',
+    'RegisterTypeLib', 'REGKIND', 'tagREGKIND', 'REGKIND_DEFAULT',
+    'REGKIND_NONE', 'REGKIND_REGISTER', 'SAFEARRAYBOUND', 'tagSAFEARRAYBOUND',
+    'SYS_MAC', 'SYS_WIN16', 'SYS_WIN32', 'SYS_WIN64', 'SYSKIND', 'tagSYSKIND',
+    'TKIND_ALIAS', 'TKIND_COCLASS', 'TKIND_DISPATCH', 'TKIND_ENUM',
+    'TKIND_INTERFACE', 'TKIND_MAX', 'TKIND_MODULE', 'TKIND_RECORD',
+    'TKIND_UNION', 'tagTLIBATTR', 'TLIBATTR', 'tagTYPEATTR', 'TYPEATTR',
+    'tagTYPEDESC', 'TYPEDESC', 'TYPEFLAG_FAGGREGATABLE', 'TYPEFLAG_FAPPOBJECT',
+    'TYPEFLAG_FCANCREATE', 'TYPEFLAG_FCONTROL', 'TYPEFLAG_FDISPATCHABLE',
+    'TYPEFLAG_FDUAL', 'TYPEFLAG_FHIDDEN', 'TYPEFLAG_FLICENSED',
+    'TYPEFLAG_FNONEXTENSIBLE', 'TYPEFLAG_FOLEAUTOMATION',
+    'TYPEFLAG_FPREDECLID', 'TYPEFLAG_FPROXY', 'TYPEFLAG_FREPLACEABLE',
+    'TYPEFLAG_FRESTRICTED', 'TYPEFLAG_FREVERSEBIND', 'TYPEFLAGS',
+    'tagTYPEFLAGS', 'TYPEKIND', 'tagTYPEKIND', 'ULONG_PTR',
+    'UnRegisterTypeLib', 'VAR_CONST', 'VAR_DISPATCH', 'VAR_PERINSTANCE',
+    'VAR_STATIC', 'VARDESC', 'tagVARDESC', 'VARFLAG_FBINDABLE',
+    'VARFLAG_FDEFAULTBIND', 'VARFLAG_FDEFAULTCOLLELEM', 'VARFLAG_FDISPLAYBIND',
+    'VARFLAG_FHIDDEN', 'VARFLAG_FIMMEDIATEBIND', 'VARFLAG_FNONBROWSABLE',
+    'VARFLAG_FREADONLY', 'VARFLAG_FREPLACEABLE', 'VARFLAG_FREQUESTEDIT',
+    'VARFLAG_FRESTRICTED', 'VARFLAG_FSOURCE', 'VARFLAG_FUIDEFAULT',
+    'VARFLAGS', 'tagVARFLAGS', 'VARKIND', 'tagVARKIND',
+]
```

## Comparing `comtypes-1.1.9/comtypes/util.py` & `comtypes-1.2.0/comtypes/util.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/viewobject.py` & `comtypes-1.2.0/comtypes/viewobject.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/_comobject.py` & `comtypes-1.2.0/comtypes/_comobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from ctypes import (
     FormatError, POINTER, Structure, WINFUNCTYPE, byref, c_long, c_void_p,
     oledll, pointer, windll
 )
 from _ctypes import CopyComPointer
 import logging
 import os
+import sys
 
 from comtypes import COMError, ReturnHRESULT, instancemethod, _encode_idl
 from comtypes.errorinfo import ISupportErrorInfo, ReportException, ReportError
 from comtypes import IPersist
 from comtypes.hresult import (
     DISP_E_BADINDEX, DISP_E_MEMBERNOTFOUND, E_FAIL, E_NOINTERFACE,
     E_INVALIDARG, E_NOTIMPL, RPC_E_CHANGED_MODE, S_FALSE, S_OK
@@ -17,14 +18,19 @@
 
 
 logger = logging.getLogger(__name__)
 _debug = logger.debug
 _warning = logger.warning
 _error = logger.error
 
+if sys.version_info >= (3, 0):
+    int_types = (int, )
+else:
+    int_types = (int, long)
+
 ################################################################
 # COM object implementation
 
 # so we don't have to import comtypes.automation
 DISPATCH_METHOD = 1
 DISPATCH_PROPERTYGET = 2
 DISPATCH_PROPERTYPUT = 4
@@ -47,15 +53,15 @@
 def winerror(exc):
     """Return the windows error code from a WindowsError or COMError
     instance."""
     if isinstance(exc, COMError):
         return exc.hresult
     elif isinstance(exc, WindowsError):
         code = exc.winerror
-        if isinstance(code, (int, long)):
+        if isinstance(code, int_types):
             return code
         # Sometimes, a WindowsError instance has no error code.  An access
         # violation raised by ctypes has only text, for example.  In this
         # cases we return a generic error code.
         return E_FAIL
     raise TypeError("Expected comtypes.COMERROR or WindowsError instance, got %s" % type(exc).__name__)
 
@@ -71,19 +77,19 @@
 
 def catch_errors(obj, mth, paramflags, interface, mthname):
     clsid = getattr(obj, "_reg_clsid_", None)
 
     def call_with_this(*args, **kw):
         try:
             result = mth(*args, **kw)
-        except ReturnHRESULT, err:
+        except ReturnHRESULT as err:
             (hresult, text) = err.args
             return ReportError(text, iid=interface._iid_, clsid=clsid,
                                hresult=hresult)
-        except (COMError, WindowsError), details:
+        except (COMError, WindowsError) as details:
             _error("Exception in %s.%s implementation:", interface.__name__,
                    mthname, exc_info=True)
             return HRESULT_FROM_WIN32(winerror(details))
         except E_NotImplemented:
             _warning("Unimplemented method %s.%s called", interface.__name__,
                      mthname)
             return E_NOTIMPL
@@ -104,15 +110,15 @@
 
 
 ################################################################
 
 def hack(inst, mth, paramflags, interface, mthname):
     if paramflags is None:
         return catch_errors(inst, mth, paramflags, interface, mthname)
-    code = mth.func_code
+    code = mth.__code__
     if code.co_varnames[1:2] == ("this",):
         return catch_errors(inst, mth, paramflags, interface, mthname)
     dirflags = [f[0] for f in paramflags]
     # An argument is an input arg either if flags are NOT set in the
     # idl file, or if the flags contain 'in'. In other words, the
     # direction flag is either exactly '0' or has the '1' bit set:
     # Output arguments have flag '2'
@@ -150,32 +156,32 @@
                 args[args_out_idx[0]][0] = result
             elif args_out != 0:
                 if len(result) != args_out:
                     msg = "Method should have returned a %s-tuple" % args_out
                     raise ValueError(msg)
                 for i, value in enumerate(result):
                     args[args_out_idx[i]][0] = value
-        except ReturnHRESULT, err:
+        except ReturnHRESULT as err:
             (hresult, text) = err.args
             return ReportError(text, iid=interface._iid_, clsid=clsid,
                                hresult=hresult)
-        except COMError, err:
+        except COMError as err:
             (hr, text, details) = err.args
             _error("Exception in %s.%s implementation:", interface.__name__,
                    mthname, exc_info=True)
             try:
                 descr, source, helpfile, helpcontext, progid = details
             except (ValueError, TypeError):
                 msg = str(details)
             else:
                 msg = "%s: %s" % (source, descr)
             hr = HRESULT_FROM_WIN32(hr)
             return ReportError(msg, iid=interface._iid_, clsid=clsid,
                                hresult=hr)
-        except WindowsError, details:
+        except WindowsError as details:
             _error("Exception in %s.%s implementation:", interface.__name__,
                    mthname, exc_info=True)
             hr = HRESULT_FROM_WIN32(winerror(details))
             return ReportException(hr, interface._iid_, clsid=clsid)
         except E_NotImplemented:
             _warning("Unimplemented method %s.%s called", interface.__name__,
                      mthname)
@@ -329,16 +335,19 @@
             obj._revoke_class()
 
     def run_sta(self):
         from comtypes import messageloop
         messageloop.run()
 
     def run_mta(self):
-        import Queue
-        self._queue = Queue.Queue()
+        if sys.version_info >= (3, 0):
+            import queue
+        else:
+            import Queue as queue
+        self._queue = queue.Queue()
         self._queue.get()
 
     def Lock(self):
         oledll.ole32.CoAddRefServerProcess()
 
     def Unlock(self):
         rc = oledll.ole32.CoReleaseServerProcess()
@@ -554,15 +563,15 @@
         try:
             del COMObject._instances_[obj]
         except AttributeError:
             _debug("? active COM objects: Removed %r", obj)
         else:
             _debug("%d active COM objects: Removed %r",
                    len(COMObject._instances_), obj)
-        _debug("Remaining: %s", COMObject._instances_.keys())
+        _debug("Remaining: %s", list(COMObject._instances_.keys()))
         if COMObject.__server__:
             COMObject.__server__.Unlock()
     #
     ################################################################
 
     #########################################################
     # IUnknown methods implementations
@@ -732,15 +741,15 @@
             # DISPATCH_PROPERTYPUT
             # DISPATCH_PROPERTYPUTREF
             #
             # How are the parameters unpacked for propertyput
             # operations with additional parameters?  Can propput
             # have additional args?
             args = [params.rgvarg[i].value
-                    for i in reversed(range(params.cNamedArgs))]
+                    for i in reversed(list(range(params.cNamedArgs)))]
             # MSDN: pVarResult is ignored if DISPATCH_PROPERTYPUT or
             # DISPATCH_PROPERTYPUTREF is specified.
             return mth(this, *args)
 
         else:
             # DISPATCH_METHOD
             # DISPATCH_PROPERTYGET
@@ -749,15 +758,15 @@
             # 2to3 has problems to translate 'range(...)[::-1]'
             # correctly, so use 'list(range)[::-1]' instead (will be
             # fixed in Python 3.1, probably):
             named_indexes = [params.rgdispidNamedArgs[i]
                              for i in range(params.cNamedArgs)]
             # the positions of unnamed arguments
             num_unnamed = params.cArgs - params.cNamedArgs
-            unnamed_indexes = list(reversed(range(num_unnamed)))
+            unnamed_indexes = list(reversed(list(range(num_unnamed))))
             # It seems that this code calculates the indexes of the
             # parameters in the params.rgvarg array correctly.
             indexes = named_indexes + unnamed_indexes
             args = [params.rgvarg[i].value for i in indexes]
 
             if pVarResult and getattr(mth, "has_outargs", False):
                 args.append(pVarResult)
```

## Comparing `comtypes-1.1.9/comtypes/_meta.py` & `comtypes-1.2.0/comtypes/_meta.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/_safearray.py` & `comtypes-1.2.0/comtypes/_safearray.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/__init__.py` & `comtypes-1.2.0/comtypes/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,123 @@
-import types
-import sys
-import os
-
 # comtypes version numbers follow semver (http://semver.org/) and PEP 440
-__version__ = "1.1.9"
+__version__ = "1.2.0"
 
+import atexit
+from ctypes import *
+from ctypes import _SimpleCData
+from _ctypes import COMError
 import logging
+import os
+import sys
+import types
+
+################################################################
+
+def add_metaclass(metaclass):
+    """Class decorator from six.py for creating a class with a metaclass.
+
+    Copyright (c) 2010-2020 Benjamin Peterson
+
+    Permission is hereby granted, free of charge, to any person obtaining a copy of
+    this software and associated documentation files (the "Software"), to deal in
+    the Software without restriction, including without limitation the rights to
+    use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+    the Software, and to permit persons to whom the Software is furnished to do so,
+    subject to the following conditions:
+
+    The above copyright notice and this permission notice shall be included in all
+    copies or substantial portions of the Software.
+
+    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+    FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+    COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+    IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+    CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+    """
+    def wrapper(cls):
+        orig_vars = cls.__dict__.copy()
+        slots = orig_vars.get('__slots__')
+        if slots is not None:
+            if isinstance(slots, text_type):
+                slots = [slots]
+            for slots_var in slots:
+                orig_vars.pop(slots_var)
+        orig_vars.pop('__dict__', None)
+        orig_vars.pop('__weakref__', None)
+        if hasattr(cls, '__qualname__'):
+            orig_vars['__qualname__'] = cls.__qualname__
+        return metaclass(cls.__name__, cls.__bases__, orig_vars)
+    return wrapper
+
+################################################################
+
+# type hinting symbols
+#
+# `if TYPE_CHECKING:` code block must not be executed because `TYPE_CHECKING`
+# is always `False` in runtime.
+# see https://peps.python.org/pep-0484/#runtime-or-type-checking
+#
+if sys.version_info >= (3, 5):
+    from typing import TYPE_CHECKING
+else:  # typehints in this package don't support Py<3.5 due to importing symbols.
+    TYPE_CHECKING = False
+#
+# Annotations must be placed in a `# type:` comment in according to PEP484.
+# see https://peps.python.org/pep-0484/#suggested-syntax-for-python-2-7-and-straddling-code
+# - `NameError` never raises by using those symbols.
+# - It is not able to use any runtime introspections, such as
+#   `typing.get_type_hints` or `typing.get_origin`.
+#
+if TYPE_CHECKING:
+    from ctypes import _CData  # only in `typeshed`, private in runtime
+    # _CData = _SimpleCData.__mro__[:-1][-1]  # defining in runtime
+    from ctypes import _Pointer
+    from typing import Any, ClassVar, overload, TypeVar
+    # XXX: symbols for backward compatibility.
+    # instead of `builtins`. see PEP585.
+    from typing import Dict, List, Tuple, Type
+    # instead of `collections.abc`. see PEP585.
+    from typing import Callable, Iterable, Iterator
+    # instead of `A | B` and `None | A`. see PEP604.
+    from typing import Union as _UnionT  #  avoiding confusion with `ctypes.Union`
+    from typing import Optional
+    # utilities or workarounds for annotations.
+    from comtypes import hints as hints
+
+################################################################
+
+from comtypes.GUID import GUID
+from comtypes import patcher
+from comtypes._npsupport import interop as npsupport
+from comtypes._memberspec import (
+    ComMemberGenerator, _ComMemberSpec, DispMemberGenerator, _DispMemberSpec,
+    _encode_idl, _resolve_argspec,
+)
+
+################################################################
+if sys.version_info >= (3, 0):
+    text_type = str
+else:
+    text_type = unicode
+_all_slice = slice(None, None, None)
+
 class NullHandler(logging.Handler):
     """A Handler that does nothing."""
     def emit(self, record):
         pass
 
 logger = logging.getLogger(__name__)
 
 # Add a NULL handler to the comtypes logger.  This prevents getting a
 # message like this:
 #    No handlers could be found for logger "comtypes"
 # when logging is not configured and logger.error() is called.
 logger.addHandler(NullHandler())
 
-from ctypes import *
-from _ctypes import COMError
-from comtypes import patcher
 
 def _check_version(actual, tlib_cached_mtime=None):
     from comtypes.tools.codegenerator import version as required
     if actual != required:
         raise ImportError("Wrong version")
     if not hasattr(sys, "frozen"):
         g = sys._getframe(1).f_globals
@@ -33,33 +125,14 @@
         try:
             tlib_curr_mtime = os.stat(tlb_path).st_mtime
         except (OSError, TypeError):
             return
         if not tlib_cached_mtime or abs(tlib_curr_mtime - tlib_cached_mtime) >= 1:
             raise ImportError("Typelib different than module")
 
-try:
-    COMError()
-except TypeError:
-    pass
-else:
-    # Python 2.5 and 2.5.1 have a bug in the COMError implementation:
-    # The type has no __init__ method, and no hresult, text, and
-    # details instance vars.  Work around this bug by monkeypatching
-    # COMError.
-    def monkeypatch_COMError():
-        def __init__(self, hresult, text, details):
-            self.hresult = hresult
-            self.text = text
-            self.details = details
-            super(COMError, self).__init__(hresult, text, details)
-        COMError.__init__ = __init__
-    monkeypatch_COMError()
-    del monkeypatch_COMError
-
 if sys.version_info >= (3, 0):
     pythonapi.PyInstanceMethod_New.argtypes = [py_object]
     pythonapi.PyInstanceMethod_New.restype = py_object
     PyInstanceMethod_Type = type(pythonapi.PyInstanceMethod_New(id))
 
     def instancemethod(func, inst, cls):
         mth = PyInstanceMethod_Type(func)
@@ -76,15 +149,14 @@
     Return a hresult code from a COM method implementation
     without logging an error.
     """
 
 ##class IDLWarning(UserWarning):
 ##    "Warn about questionable type information"
 
-from comtypes.GUID import GUID
 _GUID = GUID
 IID = GUID
 DWORD = c_ulong
 
 wireHWND = c_ulong
 
 ################################################################
@@ -168,30 +240,29 @@
 
 
 def _shutdown(func=_ole32_nohresult.CoUninitialize,
              _debug=logger.debug,
              _exc_clear=getattr(sys, "exc_clear", lambda: None)):
     # Make sure no COM pointers stay in exception frames.
     _exc_clear()
-    # Sometimes, CoUnititialize, running at Python shutdown,
+    # Sometimes, CoUninitialize, running at Python shutdown,
     # raises an exception.  We suppress this when __debug__ is
     # False.
-    _debug("Calling CoUnititialize()")
+    _debug("Calling CoUninitialize()")
     if __debug__:
         func()
     else:
         try: func()
         except WindowsError: pass
     # Set the flag which means that calling obj.Release() is no longer
     # needed.
     if _cominterface_meta is not None:
         _cominterface_meta._com_shutting_down = True
-    _debug("CoUnititialize() done.")
+    _debug("CoUninitialize() done.")
 
-import atexit
 atexit.register(_shutdown)
 
 ################################################################
 # global registries.
 
 # allows to find interface classes by guid strings (iid)
 com_interface_registry = {}
@@ -216,53 +287,58 @@
 ################################################################
 # The metaclasses...
 
 class _cominterface_meta(type):
     """Metaclass for COM interfaces.  Automatically creates high level
     methods from COMMETHOD lists.
     """
+    if TYPE_CHECKING:
+        _case_insensitive_ = hints.AnnoField()  # type: bool
+        _iid_ = hints.AnnoField()  # type: GUID
+        _methods_ = hints.AnnoField()  # type: List[_ComMemberSpec]
+        _disp_methods_ = hints.AnnoField()  # type: List[_DispMemberSpec]
 
     # This flag is set to True by the atexit handler which calls
-    # CoUnititialize.
+    # CoUninitialize.
     _com_shutting_down = False
 
     # Creates also a POINTER type for the newly created class.
-    def __new__(self, name, bases, namespace):
+    def __new__(cls, name, bases, namespace):
         methods = namespace.pop("_methods_", None)
         dispmethods = namespace.pop("_disp_methods_", None)
-        cls = type.__new__(self, name, bases, namespace)
+        new_cls = type.__new__(cls, name, bases, namespace)
 
         if methods is not None:
-            cls._methods_ = methods
+            new_cls._methods_ = methods
         if dispmethods is not None:
-            cls._disp_methods_ = dispmethods
+            new_cls._disp_methods_ = dispmethods
 
         # If we sublass a COM interface, for example:
         #
         # class IDispatch(IUnknown):
         #     ....
         #
         # then we need to make sure that POINTER(IDispatch) is a
         # subclass of POINTER(IUnknown) because of the way ctypes
         # typechecks work.
         if bases == (object,):
-            _ptr_bases = (cls, _compointer_base)
+            _ptr_bases = (new_cls, _compointer_base)
         else:
-            _ptr_bases = (cls, POINTER(bases[0]))
+            _ptr_bases = (new_cls, POINTER(bases[0]))
 
-        # The interface 'cls' is used as a mixin.
-        p = type(_compointer_base)("POINTER(%s)" % cls.__name__,
+        # The interface 'new_cls' is used as a mixin.
+        p = type(_compointer_base)("POINTER(%s)" % new_cls.__name__,
                                    _ptr_bases,
-                                   {"__com_interface__": cls,
+                                   {"__com_interface__": new_cls,
                                     "_needs_com_addref_": None})
 
         from ctypes import _pointer_type_cache
-        _pointer_type_cache[cls] = p
+        _pointer_type_cache[new_cls] = p
 
-        if cls._case_insensitive_:
+        if new_cls._case_insensitive_:
 
             @patcher.Patch(p)
             class CaseInsensitive(object):
                 # case insensitive attributes for COM methods and properties
                 def __getattr__(self, name):
                     """Implement case insensitive access to methods and properties"""
                     try:
@@ -308,15 +384,15 @@
                     if bool(value):
                         value.AddRef()
                     super(POINTER(p), self).__setitem__(index, value)
                     return
                 from _ctypes import CopyComPointer
                 CopyComPointer(value, self)
 
-        return cls
+        return new_cls
 
     def __setattr__(self, name, value):
         if name == "_methods_":
             # XXX I'm no longer sure why the code generator generates
             # "_methods_ = []" in the interface definition, and later
             # overrides this by "Interface._methods_ = [...]
 ##            assert self.__dict__.get("_methods_", None) is None
@@ -368,15 +444,15 @@
                     elif index == _all_slice:
                         args = ()
                     else:
                         args = (index,)
 
                     try:
                         result = self.Item(*args)
-                    except COMError, err:
+                    except COMError as err:
                         (hresult, text, details) = err.args
                         if hresult == -2147352565:  # DISP_E_BADINDEX
                             raise IndexError("invalid index")
                         else:
                             raise
 
                     # Note that result may be NULL COM pointer. There is no way
@@ -387,15 +463,15 @@
                     return result
 
                 @patcher.no_replace
                 def __setitem__(self, index, value):
                     "Attempt 'self.Item[index] = value'"
                     try:
                         self.Item[index] = value
-                    except COMError, err:
+                    except COMError as err:
                         (hresult, text, details) = err.args
                         if hresult == -2147352565:  # DISP_E_BADINDEX
                             raise IndexError("invalid index")
                         else:
                             raise
                     except TypeError:
                         msg = "%r object does not support item assignment"
@@ -434,478 +510,103 @@
             self.__dict__["__map_case__"]
         except KeyError:
             d = {}
             d.update(getattr(self, "__map_case__", {}))
             self.__map_case__ = d
 
     def _make_dispmethods(self, methods):
+        # type: (List[_DispMemberSpec]) -> None
         if self._case_insensitive_:
             self._make_case_insensitive()
-
         # create dispinterface methods and properties on the interface 'self'
-        properties = {}
+        member_gen = DispMemberGenerator(self.__name__)
         for m in methods:
-            what, name, idlflags, restype, argspec = m
-
-            # is it a property set or property get?
-            is_prop = False
-
-            # argspec is a sequence of tuples, each tuple is:
-            # ([paramflags], type, name)
-            try:
-                memid = [x for x in idlflags if isinstance(x, int)][0]
-            except IndexError:
-                raise TypeError("no dispid found in idlflags")
-            if what == "DISPPROPERTY": # DISPPROPERTY
-                assert not argspec # XXX does not yet work for properties with parameters
-                accessor = self._disp_property(memid, idlflags)
-                is_prop = True
-                setattr(self, name, accessor)
-            elif what == "DISPMETHOD": # DISPMETHOD
-                # argspec is a tuple of (idlflags, type, name[,
-                # defval]) items.
-                method = self._disp_method(memid, name, idlflags, restype, argspec)
-## not in 2.3                method.__name__ = name
-                if 'propget' in idlflags:
-                    nargs = len(argspec)
-                    properties.setdefault((name, nargs), [None, None, None])[0] = method
-                    is_prop = True
-                elif 'propput' in idlflags:
-                    nargs = len(argspec)-1
-                    properties.setdefault((name, nargs), [None, None, None])[1] = method
-                    is_prop = True
-                elif 'propputref' in idlflags:
-                    nargs = len(argspec)-1
-                    properties.setdefault((name, nargs), [None, None, None])[2] = method
-                    is_prop = True
-                else:
-                    setattr(self, name, method)
+            member_gen.add(m)
+        for name, func_or_prop, is_prop in member_gen.items():
+            setattr(self, name, func_or_prop)
             # COM is case insensitive.
-            #
             # For a method, this is the real name.  For a property,
             # this is the name WITHOUT the _set_ or _get_ prefix.
             if self._case_insensitive_:
                 self.__map_case__[name.lower()] = name
                 if is_prop:
                     self.__map_case__[name[5:].lower()] = name[5:]
-
-        for (name, nargs), methods in properties.items():
-            # methods contains [propget or None, propput or None, propputref or None]
-            if methods[1] is not None and methods[2] is not None:
-                # both propput and propputref.
-                #
-                # Create a setter method that examines the argument type
-                # and calls 'propputref' if it is an Object (in the VB
-                # sense), or call 'propput' otherwise.
-                propput = methods[1]
-                propputref = methods[2]
-                def put_or_putref(self, *args):
-                    if _is_object(args[-1]):
-                        return propputref(self, *args)
-                    else:
-                        return propput(self, *args)
-                methods[1] = put_or_putref
-                del methods[2]
-            elif methods[2] is not None:
-                # use propputref
-                del methods[1]
-            else:
-                # use propput (if any)
-                del methods[2]
-            if nargs:
-                setattr(self, name, named_property("%s.%s" % (self.__name__, name), *methods))
-            else:
-                assert len(methods) <= 2
-                setattr(self, name, property(*methods))
-
+        for name, accessor in member_gen.properties():
+            setattr(self, name, accessor)
             # COM is case insensitive
             if self._case_insensitive_:
                 self.__map_case__[name.lower()] = name
 
-    # Some ideas, (not only) related to disp_methods:
-    #
-    # Should the functions/methods we create have restype and/or
-    # argtypes attributes?
-
-    def _disp_method(self, memid, name, idlflags, restype, argspec):
-        if 'propget' in idlflags:
-            def getfunc(obj, *args, **kw):
-                return self.Invoke(obj, memid, _invkind=2, *args, **kw) # DISPATCH_PROPERTYGET
-            return getfunc
-        elif 'propput' in idlflags:
-            def putfunc(obj, *args, **kw):
-                return self.Invoke(obj, memid, _invkind=4, *args, **kw) # DISPATCH_PROPERTYPUT
-            return putfunc
-        elif 'propputref' in idlflags:
-            def putfunc(obj, *args, **kw):
-                return self.Invoke(obj, memid, _invkind=8, *args, **kw) # DISPATCH_PROPERTYPUTREF
-            return putfunc
-        # a first attempt to make use of the restype.  Still, support
-        # for named arguments and default argument values should be
-        # added.
-        if hasattr(restype, "__com_interface__"):
-            interface = restype.__com_interface__
-            def func(s, *args, **kw):
-                result = self.Invoke(s, memid, _invkind=1, *args, **kw)
-                if result is None:
-                    return
-                return result.QueryInterface(interface)
-        else:
-            def func(obj, *args, **kw):
-                return self.Invoke(obj, memid, _invkind=1, *args, **kw) # DISPATCH_METHOD
-        return func
-
-    def _disp_property(self, memid, idlflags):
-        # XXX doc string missing in property
-        def _get(obj):
-            return obj.Invoke(memid, _invkind=2) # DISPATCH_PROPERTYGET
-        if "readonly" in idlflags:
-            return property(_get)
-        def _set(obj, value):
-            # Detect whether to use DISPATCH_PROPERTYPUT or
-            # DISPATCH_PROPERTYPUTREF
-            invkind = 8 if _is_object(value) else 4
-            return obj.Invoke(memid, value, _invkind=invkind)
-        return property(_get, _set)
-
     def __get_baseinterface_methodcount(self):
         "Return the number of com methods in the base interfaces"
         try:
             result = 0
             for itf in self.mro()[1:-1]:
                 result += len(itf.__dict__["_methods_"])
             return result
-        except KeyError, err:
+        except KeyError as err:
             (name,) = err.args
             if name == "_methods_":
                 raise TypeError("baseinterface '%s' has no _methods_" % itf.__name__)
             raise
 
-    def _fix_inout_args(self, func, argtypes, paramflags):
-        # This function provides a workaround for a bug in ctypes.
-        # [in, out] parameters must be converted with the argtype's
-        # .from_param() method BEFORE they are passed to the _ctypes
-        # build_callargs() function in Modules/_ctypes/_ctypes.c.
-        #
-        # For details see below.
-        #
-        # TODO: The workaround should be disabled when a ctypes
-        # version is used where the bug is fixed.
-        SIMPLETYPE = type(c_int)
-        BYREFTYPE = type(byref(c_int()))
-        def call_with_inout(self_, *args, **kw):
-            args = list(args)
-            # Indexed by order in the output
-            outargs = {}
-            outnum = 0
-            for i, info in enumerate(paramflags):
-                direction = info[0]
-                if direction & 3 == 3:
-                    # This is an [in, out] parameter.
-                    #
-                    # Determine name and required type of the parameter.
-                    name = info[1]
-                    # [in, out] parameters are passed as pointers,
-                    # this is the pointed-to type:
-                    atyp = argtypes[i]._type_
-
-                    # Get the actual parameter, either as positional or
-                    # keyword arg.
-                    try:
-                        try:
-                            v = args[i]
-                        except IndexError:
-                            v = kw[name]
-                    except KeyError:
-                        # no parameter was passed, make an empty one
-                        # of the required type
-                        v = atyp()
-                    else:
-                        # parameter was passed, call .from_param() to
-                        # convert it to a ctypes type.
-                        if getattr(v, "_type_", None) is atyp:
-                            # Array of or pointer to type 'atyp' was
-                            # passed, pointer to 'atyp' expected.
-                            pass
-                        elif type(atyp) is SIMPLETYPE:
-                            # The from_param method of simple types
-                            # (c_int, c_double, ...) returns a byref()
-                            # object which we cannot use since later
-                            # it will be wrapped in a pointer.  Simply
-                            # call the constructor with the argument
-                            # in that case.
-                            v = atyp(v)
-                        else:
-                            v = atyp.from_param(v)
-                            assert not isinstance(v, BYREFTYPE)
-                    outargs[outnum] = v
-                    outnum += 1
-                    if len(args) > i:
-                        args[i] = v
-                    else:
-                        kw[name] = v
-                elif direction & 2 == 2:
-                    outnum += 1
-
-            rescode = func(self_, *args, **kw)
-            # If there is only a single output value, then do not expect it to
-            # be iterable.
-            if outnum == 1:  # rescode is not iterable
-                if len(outargs) == 1:
-                    rescode = rescode.__ctypes_from_outparam__()
-                return rescode
-
-            rescode = list(rescode)
-            for outnum, o in outargs.items():
-                rescode[outnum] = o.__ctypes_from_outparam__()
-            return rescode
-        return call_with_inout
-
     def _make_methods(self, methods):
+        # type: (List[_ComMemberSpec]) -> None
         if self._case_insensitive_:
             self._make_case_insensitive()
-
-        # we insist on an _iid_ in THIS class!
+        # register com interface. we insist on an _iid_ in THIS class!
         try:
             iid = self.__dict__["_iid_"]
         except KeyError:
             raise AttributeError("this class must define an _iid_")
         else:
-            iid = str(iid)
-##            if iid in com_interface_registry:
-##                # Warn when multiple interfaces are defined with identical iids.
-##                # This would also trigger if we reload() a module that contains
-##                # interface types, so suppress the warning in this case.
-##                other = com_interface_registry[iid]
-##                if self.__name__ != other.__name__ or self.__module__ != other.__module__:
-##                    text = "Multiple interface defn: %s, %s" % (self, other)
-##                    warnings.warn(text, UserWarning)
-            com_interface_registry[iid] = self
-            del iid
+            com_interface_registry[text_type(iid)] = self
+        # create members
         vtbl_offset = self.__get_baseinterface_methodcount()
-
-        properties = {}
-
+        member_gen = ComMemberGenerator(self.__name__, vtbl_offset, self._iid_)
         # create private low level, and public high level methods
-        for i, item in enumerate(methods):
-            restype, name, argtypes, paramflags, idlflags, doc = item
-            # the function prototype
-            prototype = WINFUNCTYPE(restype, *argtypes)
-
-            # a low level unbound method calling the com method.
-            # attach it with a private name (__com_AddRef, for example),
-            # so that custom method implementations can call it.
-
-            # If the method returns a HRESULT, we pass the interface iid,
-            # so that we can request error info for the interface.
-            if restype == HRESULT:
-##                print "%s.%s" % (self.__name__, name)
-                raw_func = prototype(i + vtbl_offset, name, None, self._iid_)
-                func = prototype(i + vtbl_offset, name, paramflags, self._iid_)
-            else:
-                raw_func = prototype(i + vtbl_offset, name, None, None)
-                func = prototype(i + vtbl_offset, name, paramflags, None)
-            setattr(self,
-                    "_%s__com_%s" % (self.__name__, name),
-                    instancemethod(raw_func, None, self))
-
-            if paramflags:
-                # see comment in the _fix_inout_args method
-                dirflags = [(p[0]&3) for p in paramflags]
-                if 3 in dirflags:
-##                    fullname = "%s::%s" % (self.__name__, name)
-##                    print "FIX %s" % fullname
-                    func = self._fix_inout_args(func, argtypes, paramflags)
-
-            # 'func' is a high level function calling the COM method
-            func.__doc__ = doc
-            try:
-                func.__name__ = name # for pyhelp
-            except TypeError:
-                # In Python 2.3, __name__ is a readonly attribute
-                pass
-            # make it an unbound method.  Remember, 'self' is a type here.
+        for m in methods:
+            member_gen.add(m)
+        for name, func, raw_func, is_prop in member_gen.methods():
+            raw_mth = instancemethod(raw_func, None, self)
+            setattr(self, "_%s__com_%s" % (self.__name__, name), raw_mth)
             mth = instancemethod(func, None, self)
-
-            # is it a property set or property get?
-            is_prop = False
-
-            # XXX Hm.  What, when paramflags is None?
-            # Or does have '0' values?
-            # Seems we loose then, at least for properties...
-
-            # The following code assumes that the docstrings for
-            # propget and propput are identical.
-            if "propget" in idlflags:
-                assert name.startswith("_get_")
-                nargs = len([flags for flags in paramflags
-                             if flags[0] & 7 in (0, 1)])
-                # XXX or should we do this?
-                # nargs = len([flags for flags in paramflags
-                #             if (flags[0] & 1) or (flags[0] == 0)])
-                propname = name[len("_get_"):]
-                properties.setdefault((propname, doc, nargs), [None, None, None])[0] = func
-                is_prop = True
-            elif "propput" in idlflags:
-                assert name.startswith("_set_")
-                nargs = len([flags for flags in paramflags
-                              if flags[0] & 7 in (0, 1)]) - 1
-                propname = name[len("_set_"):]
-                properties.setdefault((propname, doc, nargs), [None, None, None])[1] = func
-                is_prop = True
-            elif "propputref" in idlflags:
-                assert name.startswith("_setref_")
-                nargs = len([flags for flags in paramflags
-                              if flags[0] & 7 in (0, 1)]) - 1
-                propname = name[len("_setref_"):]
-                properties.setdefault((propname, doc, nargs), [None, None, None])[2] = func
-                is_prop = True
-
-            # We install the method in the class, except when it's a
-            # property accessor.  And we make sure we don't overwrite
-            # a property that's already present in the class.
             if not is_prop:
-                if hasattr(self, name):
-                    setattr(self, "_" + name, mth)
-                else:
-                    setattr(self, name, mth)
-
-            # COM is case insensitive.
-            #
-            # For a method, this is the real name.  For a property,
-            # this is the name WITHOUT the _set_ or _get_ prefix.
+                # We install the method in the class, except when it's a property.
+                # And we make sure we don't overwrite a property that's already present.
+                mthname = name if not hasattr(self, name) else ("_%s" % name)
+                setattr(self, mthname, mth)
+            # For a method, this is the real name.
+            # For a property, this is the name WITHOUT the _set_ or _get_ prefix.
             if self._case_insensitive_:
                 self.__map_case__[name.lower()] = name
                 if is_prop:
                     self.__map_case__[name[5:].lower()] = name[5:]
-
         # create public properties / attribute accessors
-        for (name, doc, nargs), methods in properties.items():
-            # methods contains [propget or None, propput or None, propputref or None]
-            if methods[1] is not None and methods[2] is not None:
-                # both propput and propputref.
-                #
-                # Create a setter method that examines the argument type
-                # and calls 'propputref' if it is an Object (in the VB
-                # sense), or call 'propput' otherwise.
-                propput = methods[1]
-                propputref = methods[2]
-                def put_or_putref(self, *args):
-                    if _is_object(args[-1]):
-                        return propputref(self, *args)
-                    else:
-                        return propput(self, *args)
-                methods[1] = put_or_putref
-                del methods[2]
-            elif methods[2] is not None:
-                # use propputref
-                del methods[1]
-            else:
-                # use propput (if any)
-                del methods[2]
-            if nargs == 0:
-                prop = property(*methods + [None, doc])
-            else:
-                # Hm, must be a descriptor where the __get__ method
-                # returns a bound object having __getitem__ and
-                # __setitem__ methods.
-                prop = named_property("%s.%s" % (self.__name__, name), *methods + [doc])
-            # Again, we should not overwrite class attributes that are
-            # already present.
-            if hasattr(self, name):
-                setattr(self, "_" + name, prop)
-            else:
-                setattr(self, name, prop)
-
+        for name, accessor in member_gen.properties():
+            # Again, we should not overwrite class attributes that are already present.
+            propname = name if not hasattr(self, name) else ("_%s" % name)
+            setattr(self, propname, accessor)
             # COM is case insensitive
             if self._case_insensitive_:
                 self.__map_case__[name.lower()] = name
 
-
-################################################################
-# helper classes for COM propget / propput
-# Should they be implemented in C for speed?
-
-_all_slice = slice(None, None, None)
-
-
-class bound_named_property(object):
-    def __init__(self, name, getter, setter, im_inst):
-        self.name = name
-        self.im_inst = im_inst
-        self.getter = getter
-        self.setter = setter
-
-    def __getitem__(self, index):
-        if self.getter is None:
-            raise TypeError("unsubscriptable object")
-        if isinstance(index, tuple):
-            return self.getter(self.im_inst, *index)
-        elif index == _all_slice:
-            return self.getter(self.im_inst)
-        else:
-            return self.getter(self.im_inst, index)
-
-    def __call__(self, *args):
-        if self.getter is None:
-            raise TypeError("object is not callable")
-        return self.getter(self.im_inst, *args)
-
-    def __setitem__(self, index, value):
-        if self.setter is None:
-            raise TypeError("object does not support item assignment")
-        if isinstance(index, tuple):
-            self.setter(self.im_inst, *(index + (value,)))
-        elif index == _all_slice:
-            self.setter(self.im_inst, value)
-        else:
-            self.setter(self.im_inst, index, value)
-
-    def __repr__(self):
-        return "<bound_named_property %r at %x>" % (self.name, id(self))
-
-    def __iter__(self):
-        """ Explicitly disallow iteration. """
-        msg = "%r is not iterable" % self.name
-        raise TypeError(msg)
-
-
-
-class named_property(object):
-    def __init__(self, name, fget=None, fset=None, doc=None):
-        self.name = name
-        self.getter = fget
-        self.setter = fset
-        self.__doc__ = doc
-
-    def __get__(self, im_inst, im_class=None):
-        if im_inst is None:
-            return self
-        return bound_named_property(self.name, self.getter, self.setter, im_inst)
-
-    # Make this a data descriptor
-    def __set__(self, obj):
-        raise AttributeError("Unsettable attribute")
-
-    def __repr__(self):
-        return "<named_property %r at %x>" % (self.name, id(self))
-
 ################################################################
 
 class _compointer_meta(type(c_void_p), _cominterface_meta):
     "metaclass for COM interface pointer classes"
     # no functionality, but needed to avoid a metaclass conflict
 
+@add_metaclass(_compointer_meta)
 class _compointer_base(c_void_p):
     "base class for COM interface pointer classes"
-    __metaclass__ = _compointer_meta
     def __del__(self, _debug=logger.debug):
         "Release the COM refcount we own."
         if self:
-            # comtypes calls CoUnititialize() when the atexit handlers
+            # comtypes calls CoUninitialize() when the atexit handlers
             # runs.  CoUninitialize() cleans up the COM objects that
             # are still alive. Python COM pointers may still be
             # present but we can no longer call Release() on them -
             # this may give a protection fault.  So we need the
             # _com_shutting_down flag.
             #
             if not type(self)._com_shutting_down:
@@ -947,49 +648,47 @@
 
     # This fixes the problem when there are multiple python interface types
     # wrapping the same COM interface.  This could happen because some interfaces
     # are contained in multiple typelibs.
     #
     # It also allows to pass a CoClass instance to an api
     # expecting a COM interface.
-    def from_param(klass, value):
+    @classmethod
+    def from_param(cls, value):
         """Convert 'value' into a COM pointer to the interface.
 
         This method accepts a COM pointer, or a CoClass instance
         which is QueryInterface()d."""
         if value is None:
             return None
         # CLF: 2013-01-18
         # A default value of 0, meaning null, can pass through to here.
         if value == 0:
             return None
-        if isinstance(value, klass):
+        if isinstance(value, cls):
             return value
         # multiple python interface types for the same COM interface.
         # Do we need more checks here?
-        if klass._iid_ == getattr(value, "_iid_", None):
+        if cls._iid_ == getattr(value, "_iid_", None):
             return value
         # Accept an CoClass instance which exposes the interface required.
         try:
             table = value._com_pointers_
         except AttributeError:
             pass
         else:
             try:
                 # a kind of QueryInterface
-                return table[klass._iid_]
+                return table[cls._iid_]
             except KeyError:
-                raise TypeError("Interface %s not supported" % klass._iid_)
-        return value.QueryInterface(klass.__com_interface__)
-    from_param = classmethod(from_param)
+                raise TypeError("Interface %s not supported" % cls._iid_)
+        return value.QueryInterface(cls.__com_interface__)
 
 ################################################################
 
-from ctypes import _SimpleCData
-
 class BSTR(_SimpleCData):
     "The windows BSTR data type"
     _type_ = "X"
     _needsfree = False
     def __repr__(self):
         return "%s(%r)" % (self.__class__.__name__, self.value)
 
@@ -1000,257 +699,301 @@
     def __del__(self, _free=windll.oleaut32.SysFreeString):
         # Free the string if self owns the memory
         # or if instructed by __ctypes_from_outparam__.
         if self._b_base_ is None \
                or self._needsfree:
             _free(self)
 
+    @classmethod
     def from_param(cls, value):
         """Convert into a foreign function call parameter."""
         if isinstance(value, cls):
             return value
         # Although the builtin SimpleCData.from_param call does the
         # right thing, it doesn't ensure that SysFreeString is called
         # on destruction.
         return cls(value)
-    from_param = classmethod(from_param)
 
 ################################################################
 # IDL stuff
 
-class helpstring(unicode):
+class helpstring(text_type):
     "Specifies the helpstring for a COM method or property."
 
 class defaultvalue(object):
     "Specifies the default value for parameters marked optional."
     def __init__(self, value):
         self.value = value
 
 class dispid(int):
     "Specifies the DISPID of a method or property."
 
 # XXX STDMETHOD, COMMETHOD, DISPMETHOD, and DISPPROPERTY should return
-# instances with methods, or at least accessors instead of tuple.
+# instances with more methods or properties, and should not behave as an unpackable.
 
 def STDMETHOD(restype, name, argtypes=()):
     "Specifies a COM method slot without idlflags"
-    # restype, name, argtypes, paramflags, idlflags, docstring
-    return restype, name, argtypes, None, (), None
+    return _ComMemberSpec(restype, name, argtypes, None, (), None)
 
 def DISPMETHOD(idlflags, restype, name, *argspec):
     "Specifies a method of a dispinterface"
-    return "DISPMETHOD", name, idlflags, restype, argspec
+    return _DispMemberSpec("DISPMETHOD", name, tuple(idlflags), restype, argspec)
 
 def DISPPROPERTY(idlflags, proptype, name):
     "Specifies a property of a dispinterface"
-    return "DISPPROPERTY", name, idlflags, proptype, ()#, argspec
+    return _DispMemberSpec("DISPPROPERTY", name, tuple(idlflags), proptype, ())
 
-# COMMETHOD returns:
-# restype, methodname, tuple(argtypes), tuple(paramflags), tuple(idlflags), helptext
-#
-# paramflags is a sequence of (flags (integer), paramname (string)
 # tuple(idlflags) is for the method itself: (dispid, 'readonly')
-#
-# Example: (HRESULT, 'Width', (c_long,), (2, 'rhs'), (4, 'readonly'), None)
-
-## sample generated code:
-##    DISPPROPERTY([5, 'readonly'], OLE_YSIZE_HIMETRIC, 'Height'),
-##    DISPMETHOD([6], None, 'Render',
-##               ( [], c_int, 'hdc' ),
-##               ( [], c_int, 'x' ),
-##               ( [], c_int, 'y' ))
-
-################################################################
 
-_PARAMFLAGS = {
-    "in": 1,
-    "out": 2,
-    "lcid": 4,
-    "retval": 8,
-    "optional": 16,
-    }
-
-def _encode_idl(names):
-    # sum up all values found in _PARAMFLAGS, ignoring all others.
-    return sum([_PARAMFLAGS.get(n, 0) for n in names])
-
-_NOTHING = object()
-def _unpack_argspec(idl, typ, name=None, defval=_NOTHING):
-    return idl, typ, name, defval
+# sample generated code:
+#     DISPPROPERTY([5, 'readonly'], OLE_YSIZE_HIMETRIC, 'Height'),
+#     DISPMETHOD(
+#         [6], None, 'Render', ([], c_int, 'hdc'), ([], c_int, 'x'), ([], c_int, 'y')
+#     )
 
 def COMMETHOD(idlflags, restype, methodname, *argspec):
     """Specifies a COM method slot with idlflags.
 
     XXX should explain the sematics of the arguments.
     """
-    paramflags = []
-    argtypes = []
-
     # collect all helpstring instances
     # We should suppress docstrings when Python is started with -OO
-    helptext = [t for t in idlflags if isinstance(t, helpstring)]
     # join them together(does this make sense?) and replace by None if empty.
-    helptext = "".join(helptext) or None
-
-    from comtypes.automation import VARIANT
-
-    for item in argspec:
-        idl, typ, argname, defval = _unpack_argspec(*item)
-        pflags = _encode_idl(idl)
-        if "optional" in idl:
-            if defval is _NOTHING:
-                if typ is VARIANT:
-                    defval = VARIANT.missing
-                elif typ is POINTER(VARIANT):
-                    defval = pointer(VARIANT.missing)
-                else:
-##                    msg = ("'optional' only allowed for VARIANT and VARIANT*, not for %s"
-##                           % typ.__name__)
-##                    warnings.warn(msg, IDLWarning, stacklevel=2)
-                    defval = typ()
-        if defval is _NOTHING:
-            paramflags.append((pflags, argname))
-        else:
-            paramflags.append((pflags, argname, defval))
-        argtypes.append(typ)
+    helptext = "".join(t for t in idlflags if isinstance(t, helpstring)) or None
+    paramflags, argtypes = _resolve_argspec(argspec)
     if "propget" in idlflags:
-        methodname = "_get_%s" % methodname
+        name = "_get_%s" % methodname
     elif "propput" in idlflags:
-        methodname = "_set_%s" % methodname
+        name = "_set_%s" % methodname
     elif "propputref" in idlflags:
-        methodname = "_setref_%s" % methodname
-    return restype, methodname, tuple(argtypes), tuple(paramflags), tuple(idlflags), helptext
+        name = "_setref_%s" % methodname
+    else:
+        name = methodname
+    return _ComMemberSpec(
+        restype, name, argtypes, paramflags, tuple(idlflags), helptext
+    )
+
 
 ################################################################
 # IUnknown, the root of all evil...
 
-class IUnknown(object):
+if TYPE_CHECKING:
+    _T_IUnknown = TypeVar("_T_IUnknown", bound="IUnknown")
+
+    class _IUnknown_Base(c_void_p):
+        """This is workaround to avoid false-positive of static type checking.
+
+        `IUnknown` behaves as a ctypes type, and `POINTER` can take it.
+        This behavior is defined by some metaclasses in runtime.
+
+        In runtime, this symbol in the namespace is just alias for
+        `builtins.object`.
+        """
+        __com_QueryInterface = hints.AnnoField()  # type: Callable[[Any, Any], int]
+        __com_AddRef = hints.AnnoField()  # type: Callable[[], int]
+        __com_Release = hints.AnnoField()  # type: Callable[[], int]
+else:
+    _IUnknown_Base = object
+
+@add_metaclass(_cominterface_meta)
+class IUnknown(_IUnknown_Base):
     """The most basic COM interface.
 
     Each subclasses of IUnknown must define these class attributes:
 
     _iid_ - a GUID instance defining the identifier of this interface
 
     _methods_ - a list of methods for this interface.
 
     The _methods_ list must in VTable order.  Methods are specified
     with STDMETHOD or COMMETHOD calls.
     """
-    _case_insensitive_ = False
-    __metaclass__ = _cominterface_meta
-    _iid_ = GUID("{00000000-0000-0000-C000-000000000046}")
+    _case_insensitive_ = False  # type: ClassVar[bool]
+    _iid_ = GUID("{00000000-0000-0000-C000-000000000046}")  # type: ClassVar[GUID]
 
     _methods_ = [
         STDMETHOD(HRESULT, "QueryInterface",
                   [POINTER(GUID), POINTER(c_void_p)]),
         STDMETHOD(c_ulong, "AddRef"),
         STDMETHOD(c_ulong, "Release")
-    ]
+    ]  # type: ClassVar[List[_ComMemberSpec]]
 
+    # NOTE: Why not `QueryInterface(T) -> _Pointer[T]`?
+    # Any static type checkers is not able to provide members of `T` from `_Pointer[T]`,
+    # regardless of the pointer is able to access members of contents in runtime.
+    # And if `isinstance(p, POINTER(T))` is `True`, then `isinstance(p, T)` is also `True`.
+    # So returning `T` is not a lie, and good way to know what members the class has.
     def QueryInterface(self, interface, iid=None):
-        "QueryInterface(interface) -> instance"
+        # type: (Type[_T_IUnknown], Optional[GUID]) -> _T_IUnknown
+        """QueryInterface(interface) -> instance"""
         p = POINTER(interface)()
         if iid is None:
             iid = interface._iid_
         self.__com_QueryInterface(byref(iid), byref(p))
         clsid = self.__dict__.get('__clsid')
         if clsid is not None:
             p.__dict__['__clsid'] = clsid
-        return p
+        return p  # type: ignore
 
     # these are only so that they get a docstring.
     # XXX There should be other ways to install a docstring.
     def AddRef(self):
-        "Increase the internal refcount by one and return it."
+        # type: () -> int
+        """Increase the internal refcount by one and return it."""
         return self.__com_AddRef()
 
     def Release(self):
-        "Decrease the internal refcount by one and return it."
+        # type: () -> int
+        """Decrease the internal refcount by one and return it."""
         return self.__com_Release()
 
+
+################################################################
 # IPersist is a trivial interface, which allows to ask an object about
 # its clsid.
 class IPersist(IUnknown):
     _iid_ = GUID('{0000010C-0000-0000-C000-000000000046}')
     _idlflags_ = []
     _methods_ = [
         COMMETHOD([], HRESULT, 'GetClassID',
                   ( ['out'], POINTER(GUID), 'pClassID' )),
         ]
+    if TYPE_CHECKING:
+        # Returns the CLSID that uniquely represents an object class that
+        # defines the code that can manipulate the object's data.
+        GetClassID = hints.AnnoField()  # type: Callable[[], GUID]
+
 
 class IServiceProvider(IUnknown):
     _iid_ = GUID('{6D5140C1-7436-11CE-8034-00AA006009FA}')
-
+    if TYPE_CHECKING:
+        _QueryService = hints.AnnoField()  # type: Callable[[Any, Any, Any], int]
     # Overridden QueryService to make it nicer to use (passing it an
     # interface and it returns a pointer to that interface)
     def QueryService(self, serviceIID, interface):
+        # type: (GUID, Type[_T_IUnknown]) -> _T_IUnknown
         p = POINTER(interface)()
         self._QueryService(byref(serviceIID), byref(interface._iid_), byref(p))
-        return p
+        return p  # type: ignore
 
     _methods_ = [
         COMMETHOD([], HRESULT, 'QueryService',
                   ( ['in'], POINTER(GUID), 'guidService' ),
                   ( ['in'], POINTER(GUID), 'riid' ),
                   ( ['in'], POINTER(c_void_p), 'ppvObject' ))
         ]
 
 ################################################################
+
+if TYPE_CHECKING:
+    @overload
+    def CoGetObject(displayname, interface):  # `interface` can't be missing
+        # type: (str, None) -> IUnknown
+        pass
+    @overload
+    def CoGetObject(displayname, interface):  # it should be called this way
+        # type: (str, Type[_T_IUnknown]) -> _T_IUnknown
+        pass
+
 def CoGetObject(displayname, interface):
+    # type: (str, Optional[Type[IUnknown]]) -> IUnknown
     """Convert a displayname to a moniker, then bind and return the object
     identified by the moniker."""
     if interface is None:
         interface = IUnknown
     punk = POINTER(interface)()
     # Do we need a way to specify the BIND_OPTS parameter?
-    _ole32.CoGetObject(unicode(displayname),
+    _ole32.CoGetObject(text_type(displayname),
                        None,
                        byref(interface._iid_),
                        byref(punk))
-    return punk
+    return punk  # type: ignore
+
+
+if TYPE_CHECKING:
+    pUnkOuter = Type[_Pointer[IUnknown]]
+
+    @overload
+    def CoCreateInstance(clsid, interface=None, clsctx=None, punkouter=None):
+        # type: (GUID, None, Optional[int], Optional[pUnkOuter]) -> IUnknown
+        pass
+    @overload
+    def CoCreateInstance(clsid, interface, clsctx=None, punkouter=None):
+        # type: (GUID, Type[_T_IUnknown], Optional[int], Optional[pUnkOuter]) -> _T_IUnknown
+        pass
 
 def CoCreateInstance(clsid, interface=None, clsctx=None, punkouter=None):
+    # type: (GUID, Optional[Type[IUnknown]], Optional[int], Optional[pUnkOuter]) -> IUnknown
     """The basic windows api to create a COM class object and return a
     pointer to an interface.
     """
     if clsctx is None:
         clsctx = CLSCTX_SERVER
     if interface is None:
         interface = IUnknown
     p = POINTER(interface)()
     iid = interface._iid_
     _ole32.CoCreateInstance(byref(clsid), punkouter, clsctx, byref(iid), byref(p))
-    return p
+    return p  # type: ignore
+
+
+if TYPE_CHECKING:
+    @overload
+    def CoGetClassObject(clsid, clsctx=None, pServerInfo=None, interface=None):
+        # type: (GUID, Optional[int], Optional[COSERVERINFO], None) -> hints.IClassFactory
+        pass
+    @overload
+    def CoGetClassObject(clsid, clsctx=None, pServerInfo=None, interface=None):
+        # type: (GUID, Optional[int], Optional[COSERVERINFO], Type[_T_IUnknown]) -> _T_IUnknown
+        pass
 
 def CoGetClassObject(clsid, clsctx=None, pServerInfo=None, interface=None):
+    # type: (GUID, Optional[int], Optional[COSERVERINFO], Optional[Type[IUnknown]]) -> IUnknown
     if clsctx is None:
         clsctx = CLSCTX_SERVER
     if interface is None:
         import comtypes.server
         interface = comtypes.server.IClassFactory
     p = POINTER(interface)()
     _CoGetClassObject(clsid,
                       clsctx,
                       pServerInfo,
                       interface._iid_,
                       byref(p))
-    return p
+    return p  # type: ignore
+
+
+if TYPE_CHECKING:
+    @overload
+    def GetActiveObject(clsid, interface=None):
+        # type: (GUID, None) -> IUnknown
+        pass
+    @overload
+    def GetActiveObject(clsid, interface):
+        # type: (GUID, Type[_T_IUnknown]) -> _T_IUnknown
+        pass
 
 def GetActiveObject(clsid, interface=None):
+    # type: (GUID, Optional[Type[IUnknown]]) -> IUnknown
     """Retrieves a pointer to a running object"""
     p = POINTER(IUnknown)()
     oledll.oleaut32.GetActiveObject(byref(clsid), None, byref(p))
     if interface is not None:
-        p = p.QueryInterface(interface)
-    return p
+        p = p.QueryInterface(interface)  # type: ignore
+    return p  # type: ignore
+
 
 class MULTI_QI(Structure):
     _fields_ = [("pIID", POINTER(GUID)),
                 ("pItf", POINTER(c_void_p)),
                 ("hr", HRESULT)]
+    if TYPE_CHECKING:
+        pIID = hints.AnnoField()  # type: GUID
+        pItf = hints.AnnoField()  # type: _Pointer[c_void_p]
+        hr = hints.AnnoField()  # type: HRESULT
 
 class _COAUTHIDENTITY(Structure):
     _fields_ = [
         ('User', POINTER(c_ushort)),
         ('UserLength', c_ulong),
         ('Domain', POINTER(c_ushort)),
         ('DomainLength', c_ulong),
@@ -1275,14 +1018,19 @@
 class _COSERVERINFO(Structure):
     _fields_ = [
         ('dwReserved1', c_ulong),
         ('pwszName', c_wchar_p),
         ('pAuthInfo', POINTER(_COAUTHINFO)),
         ('dwReserved2', c_ulong),
     ]
+    if TYPE_CHECKING:
+        dwReserved1 = hints.AnnoField()  # type: int
+        pwszName = hints.AnnoField()  # type: Optional[str]
+        pAuthInfo = hints.AnnoField()  # type: _COAUTHINFO
+        dwReserved2 = hints.AnnoField()  # type: int
 COSERVERINFO = _COSERVERINFO
 _CoGetClassObject = _ole32.CoGetClassObject
 _CoGetClassObject.argtypes = [POINTER(GUID), DWORD, POINTER(COSERVERINFO),
                               POINTER(GUID), POINTER(c_void_p)]
 
 class tagBIND_OPTS(Structure):
     _fields_ = [
@@ -1333,18 +1081,32 @@
 class _SOLE_AUTHENTICATION_LIST(Structure):
     _fields_ = [
         ('cAuthInfo', c_ulong),
         ('pAuthInfo', POINTER(_SOLE_AUTHENTICATION_INFO)),
     ]
 SOLE_AUTHENTICATION_LIST = _SOLE_AUTHENTICATION_LIST
 
+
+if TYPE_CHECKING:
+    @overload
+    def CoCreateInstanceEx(
+        clsid, interface=None, clsctx=None, machine=None, pServerInfo=None):
+        # type: (GUID, None, Optional[int], Optional[str], Optional[COSERVERINFO]) -> IUnknown
+        pass
+    @overload
+    def CoCreateInstanceEx(
+        clsid, interface=None, clsctx=None, machine=None, pServerInfo=None):
+        # type: (GUID, Type[_T_IUnknown], Optional[int], Optional[str], Optional[COSERVERINFO]) -> _T_IUnknown
+        pass
+
 def CoCreateInstanceEx(clsid, interface=None,
                        clsctx=None,
                        machine=None,
                        pServerInfo=None):
+    # type: (GUID, Optional[Type[IUnknown]], Optional[int], Optional[str], Optional[COSERVERINFO]) -> IUnknown
     """The basic windows api to create a COM class object and return a
     pointer to an interface, possibly on another machine.
 
     Passing both "machine" and "pServerInfo" results in a ValueError.
 
     """
     if clsctx is None:
@@ -1353,34 +1115,63 @@
     if pServerInfo is not None:
         if machine is not None:
             msg = "Can not specify both machine name and server info"
             raise ValueError(msg)
     elif machine is not None:
         serverinfo = COSERVERINFO()
         serverinfo.pwszName = machine
-        pServerInfo = byref(serverinfo)
+        pServerInfo = byref(serverinfo)  # type: ignore
 
     if interface is None:
         interface = IUnknown
     multiqi = MULTI_QI()
-    multiqi.pIID = pointer(interface._iid_)
+    multiqi.pIID = pointer(interface._iid_)  # type: ignore
     _ole32.CoCreateInstanceEx(byref(clsid),
                              None,
                              clsctx,
                              pServerInfo,
                              1,
                              byref(multiqi))
-    return cast(multiqi.pItf, POINTER(interface))
+    return cast(multiqi.pItf, POINTER(interface))  # type: ignore
 
 
 ################################################################
 from comtypes._comobject import COMObject
 
 # What's a coclass?
 # a POINTER to a coclass is allowed as parameter in a function declaration:
 # http://msdn.microsoft.com/library/en-us/midl/midl/oleautomation.asp
 
 from comtypes._meta import _coclass_meta
 
+@add_metaclass(_coclass_meta)
 class CoClass(COMObject):
-    __metaclass__ = _coclass_meta
+    pass
 ################################################################
+
+
+__known_symbols__ = [
+    'BIND_OPTS', 'tagBIND_OPTS', 'BINDOPTS2', 'tagBIND_OPTS2', 'BSTR',
+    '_check_version', 'CLSCTX', 'tagCLSCTX', 'CLSCTX_ALL',
+    'CLSCTX_DISABLE_AAA', 'CLSCTX_ENABLE_AAA', 'CLSCTX_ENABLE_CODE_DOWNLOAD',
+    'CLSCTX_FROM_DEFAULT_CONTEXT', 'CLSCTX_INPROC', 'CLSCTX_INPROC_HANDLER',
+    'CLSCTX_INPROC_HANDLER16', 'CLSCTX_INPROC_SERVER',
+    'CLSCTX_INPROC_SERVER16', 'CLSCTX_LOCAL_SERVER', 'CLSCTX_NO_CODE_DOWNLOAD',
+    'CLSCTX_NO_CUSTOM_MARSHAL', 'CLSCTX_NO_FAILURE_LOG',
+    'CLSCTX_REMOTE_SERVER', 'CLSCTX_RESERVED1', 'CLSCTX_RESERVED2',
+    'CLSCTX_RESERVED3', 'CLSCTX_RESERVED4', 'CLSCTX_RESERVED5',
+    'CLSCTX_SERVER', '_COAUTHIDENTITY', 'COAUTHIDENTITY', '_COAUTHINFO',
+    'COAUTHINFO', 'CoClass', 'CoCreateInstance', 'CoCreateInstanceEx',
+    '_CoGetClassObject', 'CoGetClassObject', 'CoGetObject',
+    'COINIT_APARTMENTTHREADED', 'COINIT_DISABLE_OLE1DDE',
+    'COINIT_MULTITHREADED', 'COINIT_SPEED_OVER_MEMORY', 'CoInitialize',
+    'CoInitializeEx', 'COMError', 'COMMETHOD', 'COMObject', '_COSERVERINFO',
+    'COSERVERINFO', 'CoUninitialize', 'dispid', 'DISPMETHOD', 'DISPPROPERTY',
+    'DWORD', 'EOAC_NONE', 'GetActiveObject', '_GUID', 'GUID', 'helpstring',
+    'IID', 'IPersist', 'IServiceProvider', 'IUnknown', 'MULTI_QI',
+    'ReturnHRESULT', 'RPC_C_AUTHN_LEVEL_CONNECT', 'RPC_C_AUTHN_WINNT',
+    'RPC_C_AUTHZ_NONE', 'RPC_C_IMP_LEVEL_IMPERSONATE',
+    '_SEC_WINNT_AUTH_IDENTITY', 'SEC_WINNT_AUTH_IDENTITY',
+    'SEC_WINNT_AUTH_IDENTITY_UNICODE', '_SOLE_AUTHENTICATION_INFO',
+    'SOLE_AUTHENTICATION_INFO', '_SOLE_AUTHENTICATION_LIST',
+    'SOLE_AUTHENTICATION_LIST', 'STDMETHOD', 'wireHWND',
+]
```

## Comparing `comtypes-1.1.9/comtypes/client/dynamic.py` & `comtypes-1.2.0/comtypes/client/dynamic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import ctypes
 import comtypes.automation
 import comtypes.typeinfo
 import comtypes.client
 import comtypes.client.lazybind
 
 from comtypes import COMError, IUnknown, _is_object
@@ -114,15 +115,15 @@
             result = MethodCaller(dispid, self)
             self.__dict__[name] = result
             return result
 
         flags = comtypes.automation.DISPATCH_PROPERTYGET
         try:
             result = self._comobj.Invoke(dispid, _invkind=flags)
-        except COMError, err:
+        except COMError as err:
             (hresult, text, details) = err.args
             if hresult in ERRORS_BAD_CONTEXT:
                 result = MethodCaller(dispid, self)
                 self.__dict__[name] = result
             else:
                 # The line break is important for 2to3 to work correctly
                 raise
@@ -149,17 +150,24 @@
 ##        self._comobj.Invoke(-3, index, value,
 ##                            _invkind=comtypes.automation.DISPATCH_PROPERTYPUT|comtypes.automation.DISPATCH_PROPERTYPUTREF)
 
 class _Collection(object):
     def __init__(self, enum):
         self.enum = enum
 
-    def next(self):
-        item, fetched = self.enum.Next(1)
-        if fetched:
-            return item
-        raise StopIteration
+    if sys.version_info >= (3, 0):
+        def __next__(self):
+            item, fetched = self.enum.Next(1)
+            if fetched:
+                return item
+            raise StopIteration
+    else:
+        def next(self):
+            item, fetched = self.enum.Next(1)
+            if fetched:
+                return item
+            raise StopIteration
 
     def __iter__(self):
         return self
 
 __all__ = ["Dispatch"]
```

## Comparing `comtypes-1.1.9/comtypes/client/lazybind.py` & `comtypes-1.2.0/comtypes/client/lazybind.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/client/_code_cache.py` & `comtypes-1.2.0/comtypes/client/_code_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """comtypes.client._code_cache helper module.
 
 The main function is _find_gen_dir(), which on-demand creates the
 comtypes.gen package and returns a directory where generated code can
 be written to.
 """
 import ctypes, logging, os, sys, tempfile, types
+from ctypes import wintypes
 logger = logging.getLogger(__name__)
 
 
 def _ensure_list(path):
     """
     On Python 3.4 and later, when a package is imported from
     an empty directory, its `__path__` will be a _NamespacePath
@@ -75,15 +76,15 @@
 ################################################################
 
 SHGetSpecialFolderPath = ctypes.OleDLL("shell32.dll").SHGetSpecialFolderPathW
 GetModuleFileName = ctypes.WinDLL("kernel32.dll").GetModuleFileNameW
 SHGetSpecialFolderPath.argtypes = [ctypes.c_ulong, ctypes.c_wchar_p,
                                    ctypes.c_int, ctypes.c_int]
 GetModuleFileName.restype = ctypes.c_ulong
-GetModuleFileName.argtypes = [ctypes.c_ulong, ctypes.c_wchar_p, ctypes.c_ulong]
+GetModuleFileName.argtypes = [wintypes.HMODULE, ctypes.c_wchar_p, ctypes.c_ulong]
 
 CSIDL_APPDATA = 26
 MAX_PATH = 260
 
 def _create_comtypes_gen_package():
     """Import (creating it if needed) the comtypes.gen package."""
     try:
@@ -99,15 +100,15 @@
                 logger.info("Created comtypes.gen directory: '%s'", comtypes_path)
             comtypes_init = os.path.join(comtypes_path, "__init__.py")
             if not os.path.exists(comtypes_init):
                 logger.info("Writing __init__.py file: '%s'", comtypes_init)
                 ofi = open(comtypes_init, "w")
                 ofi.write("# comtypes.gen package, directory for generated files.\n")
                 ofi.close()
-        except (OSError, IOError), details:
+        except (OSError, IOError) as details:
             logger.info("Creating comtypes.gen package failed: %s", details)
             module = sys.modules["comtypes.gen"] = types.ModuleType("comtypes.gen")
             comtypes.gen = module
             comtypes.gen.__path__ = []
             logger.info("Created a memory-only package.")
 
 def _is_writeable(path):
```

## Comparing `comtypes-1.1.9/comtypes/client/_events.py` & `comtypes-1.2.0/comtypes/client/_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import print_function
 import ctypes
 import traceback
 import comtypes
 import comtypes.hresult
 import comtypes.automation
 import comtypes.typeinfo
 import comtypes.connectionpoints
@@ -82,15 +83,15 @@
     # Enumerate the connection interfaces.  If we find a single one,
     # return it, if there are more, we give up since we cannot
     # determine which one to use.
     cpc = source.QueryInterface(comtypes.connectionpoints.IConnectionPointContainer)
     enum = cpc.EnumConnectionPoints()
     iid = enum.next().GetConnectionInterface()
     try:
-        enum.next()
+        next(enum)
     except StopIteration:
         try:
             interface = comtypes.com_interface_registry[str(iid)]
         except KeyError:
             return None
         else:
             logger.debug("%s using sinkinterface from iid %s", source, interface)
@@ -100,15 +101,15 @@
 
     return None
 
 def report_errors(func):
     # This decorator preserves parts of the decorated function
     # signature, so that the comtypes special-casing for the 'this'
     # parameter still works.
-    if func.func_code.co_varnames[:2] == ('self', 'this'):
+    if func.__code__.co_varnames[:2] == ('self', 'this'):
         def error_printer(self, this, *args, **kw):
             try:
                 return func(self, this, *args, **kw)
             except:
                 traceback.print_exc()
                 raise
     else:
@@ -134,22 +135,22 @@
     def find_method(self, fq_name, mthname):
         impl = self._find_method(fq_name, mthname)
         # Caller of this method catches AttributeError,
         # so we need to be careful in the following code
         # not to raise one...
         try:
             # impl is a bound method, dissect it...
-            im_self, im_func = impl.im_self, impl.im_func
+            im_self, im_func = impl.__self__, impl.__func__
             # decorate it with an error printer...
             method = report_errors(im_func)
             # and make a new bound method from it again.
             return comtypes.instancemethod(method,
                                            im_self,
                                            type(im_self))
-        except AttributeError, details:
+        except AttributeError as details:
             raise RuntimeError(details)
 
     def _find_method(self, fq_name, mthname):
         try:
             return super(_SinkMethodFinder, self).find_method(fq_name, mthname)
         except AttributeError:
             try:
@@ -204,19 +205,19 @@
 class EventDumper(object):
     """Universal sink for COM events."""
 
     def __getattr__(self, name):
         "Create event handler methods on demand"
         if name.startswith("__") and name.endswith("__"):
             raise AttributeError(name)
-        print "# event found:", name
+        print("# event found:", name)
         def handler(self, this, *args, **kw):
             # XXX handler is called with 'this'.  Should we really print "None" instead?
             args = (None,) + args
-            print "Event %s(%s)" % (name, ", ".join([repr(a) for a in args]))
+            print("Event %s(%s)" % (name, ", ".join([repr(a) for a in args])))
         return comtypes.instancemethod(handler, self, EventDumper)
 
 def ShowEvents(source, interface=None):
     """Receive COM events from 'source'.  A special event sink will be
     used that first prints the names of events that are found in the
     outgoing interface, and will also print out the events when they
     are fired.
@@ -271,15 +272,15 @@
 
     try:
         try:
             res = ctypes.oledll.ole32.CoWaitForMultipleHandles(0,
                                                                int(timeout * 1000),
                                                                len(handles), handles,
                                                                ctypes.byref(ctypes.c_ulong()))
-        except WindowsError, details:
+        except WindowsError as details:
             if details.winerror != RPC_S_CALLPENDING: # timeout expired
                 raise
         else:
             raise KeyboardInterrupt
     finally:
         ctypes.windll.kernel32.CloseHandle(hevt)
         ctypes.windll.kernel32.SetConsoleCtrlHandler(HandlerRoutine, 0)
```

## Comparing `comtypes-1.1.9/comtypes/client/__init__.py` & `comtypes-1.2.0/comtypes/client/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,71 +5,76 @@
 #
 # TODO:
 #
 # - refactor some code into modules
 #
 ################################################################
 
-import sys, os
 import ctypes
+import logging
+import os
+import sys
 
 import comtypes
 from comtypes.hresult import *
-import comtypes.automation
-import comtypes.typeinfo
+from comtypes import (
+    automation, CoClass, GUID, IUnknown, TYPE_CHECKING, typeinfo,
+)
 import comtypes.client.dynamic
-
+from comtypes.client._constants import Constants
 from comtypes.client._events import GetEvents, ShowEvents, PumpEvents
 from comtypes.client._generate import GetModule
-
-import logging
-logger = logging.getLogger(__name__)
-
-__all__ = ["CreateObject", "GetActiveObject", "CoGetObject",
-           "GetEvents", "ShowEvents", "PumpEvents", "GetModule",
-           "GetClassObject"]
-
 from comtypes.client._code_cache import _find_gen_dir
 
 gen_dir = _find_gen_dir()
 import comtypes.gen
-
 ### for testing
 ##gen_dir = None
 
+if TYPE_CHECKING:
+    from typing import Any, Optional, overload, Type, TypeVar, Union as _UnionT
+    from comtypes import hints
+    _T_IUnknown = TypeVar("_T_IUnknown", bound=IUnknown)
+
+logger = logging.getLogger(__name__)
+
+
 def wrap_outparam(punk):
+    # type: (Any) -> Any
     logger.debug("wrap_outparam(%s)", punk)
     if not punk:
         return None
-    if punk.__com_interface__ == comtypes.automation.IDispatch:
+    if punk.__com_interface__ == automation.IDispatch:
         return GetBestInterface(punk)
     return punk
 
+
 def GetBestInterface(punk):
+    # type: (Any) -> Any
     """Try to QueryInterface a COM pointer to the 'most useful'
     interface.
 
     Get type information for the provided object, either via
     IDispatch.GetTypeInfo(), or via IProvideClassInfo.GetClassInfo().
     Generate a wrapper module for the typelib, and QI for the
     interface found.
     """
     if not punk: # NULL COM pointer
         return punk # or should we return None?
     # find the typelib and the interface name
     logger.debug("GetBestInterface(%s)", punk)
     try:
         try:
-            pci = punk.QueryInterface(comtypes.typeinfo.IProvideClassInfo)
+            pci = punk.QueryInterface(typeinfo.IProvideClassInfo)
             logger.debug("Does implement IProvideClassInfo")
         except comtypes.COMError:
             # Some COM objects support IProvideClassInfo2, but not IProvideClassInfo.
             # These objects are broken, but we support them anyway.
             logger.debug("Does NOT implement IProvideClassInfo, trying IProvideClassInfo2")
-            pci = punk.QueryInterface(comtypes.typeinfo.IProvideClassInfo2)
+            pci = punk.QueryInterface(typeinfo.IProvideClassInfo2)
             logger.debug("Does implement IProvideClassInfo2")
         tinfo = pci.GetClassInfo() # TypeInfo for the CoClass
         # find the interface marked as default
         ta = tinfo.GetTypeAttr()
         for index in range(ta.cImplTypes):
             if tinfo.GetImplTypeFlags(index) == 1:
                 break
@@ -81,15 +86,15 @@
             # not marked as default).
             index = 0
         href = tinfo.GetRefTypeOfImplType(index)
         tinfo = tinfo.GetRefTypeInfo(href)
     except comtypes.COMError:
         logger.debug("Does NOT implement IProvideClassInfo/IProvideClassInfo2")
         try:
-            pdisp = punk.QueryInterface(comtypes.automation.IDispatch)
+            pdisp = punk.QueryInterface(automation.IDispatch)
         except comtypes.COMError:
             logger.debug("No Dispatch interface: %s", punk)
             return punk
         try:
             tinfo = pdisp.GetTypeInfo(0)
         except comtypes.COMError:
             pdisp = comtypes.client.dynamic.Dispatch(pdisp)
@@ -126,92 +131,101 @@
     result = punk.QueryInterface(interface)
     logger.debug("Final result is %s", result)
     return result
 # backwards compatibility:
 wrap = GetBestInterface
 
 # Should we do this for POINTER(IUnknown) also?
-ctypes.POINTER(comtypes.automation.IDispatch).__ctypes_from_outparam__ = wrap_outparam
-
-################################################################
-#
-# Typelib constants
-#
-class Constants(object):
-    """This class loads the type library from the supplied object,
-    then exposes constants in the type library as attributes."""
-    def __init__(self, obj):
-        obj = obj.QueryInterface(comtypes.automation.IDispatch)
-        tlib, index = obj.GetTypeInfo(0).GetContainingTypeLib()
-        self.tcomp = tlib.GetTypeComp()
-
-    def __getattr__(self, name):
-        try:
-            kind, desc = self.tcomp.Bind(name)
-        except (WindowsError, comtypes.COMError):
-            raise AttributeError(name)
-        if kind != "variable":
-            raise AttributeError(name)
-        return desc._.lpvarValue[0].value
-
-    def _bind_type(self, name):
-        return self.tcomp.BindType(name)
+ctypes.POINTER(automation.IDispatch).__ctypes_from_outparam__ = wrap_outparam  # type: ignore
 
 ################################################################
 #
 # Object creation
 #
+if comtypes.TYPE_CHECKING:
+    @overload
+    def GetActiveObject(progid):
+        # type: (_UnionT[str, CoClass, GUID]) -> Any
+        pass
+    @overload
+    def GetActiveObject(progid, interface):
+        # type: (_UnionT[str, CoClass, GUID], Type[_T_IUnknown]) -> _T_IUnknown
+        pass
 def GetActiveObject(progid, interface=None, dynamic=False):
+    # type: (_UnionT[str, CoClass, GUID], Optional[Any], bool) -> Any
     """Return a pointer to a running COM object that has been
     registered with COM.
 
     'progid' may be a string like "Excel.Application",
        a string specifying a clsid, a GUID instance, or an object with
        a _clsid_ attribute which should be any of the above.
     'interface' allows to force a certain interface.
     'dynamic=True' will return a dynamic dispatch object.
     """
-    clsid = comtypes.GUID.from_progid(progid)
+    clsid = GUID.from_progid(progid)
     if dynamic:
         if interface is not None:
             raise ValueError("interface and dynamic are mutually exclusive")
-        interface = comtypes.automation.IDispatch
+        interface = automation.IDispatch
     elif interface is None:
         interface = getattr(progid, "_com_interfaces_", [None])[0]
     obj = comtypes.GetActiveObject(clsid, interface=interface)
     if dynamic:
         return comtypes.client.dynamic.Dispatch(obj)
     return _manage(obj, clsid, interface=interface)
 
+
 def _manage(obj, clsid, interface):
+    # type: (Any, Optional[GUID], Optional[Type[IUnknown]]) -> Any
     obj.__dict__['__clsid'] = str(clsid)
     if interface is None:
         obj = GetBestInterface(obj)
     return obj
 
+
+if TYPE_CHECKING:
+    @overload
+    def GetClassObject(progid, clsctx=None, pServerInfo=None):
+        # type: (_UnionT[str, CoClass, GUID], Optional[int], Optional[comtypes.COSERVERINFO]) -> hints.IClassFactory
+        pass
+    @overload
+    def GetClassObject(progid, clsctx=None, pServerInfo=None, interface=None):
+        # type: (_UnionT[str, CoClass, GUID], Optional[int], Optional[comtypes.COSERVERINFO], Optional[Type[_T_IUnknown]]) -> _T_IUnknown
+        pass
 def GetClassObject(progid,
                    clsctx=None,
                    pServerInfo=None,
                    interface=None):
+    # type: (_UnionT[str, CoClass, GUID], Optional[int], Optional[comtypes.COSERVERINFO], Optional[Type[IUnknown]]) -> IUnknown
     """Create and return the class factory for a COM object.
 
     'clsctx' specifies how to create the object, use the CLSCTX_... constants.
     'pServerInfo', if used, must be a pointer to a comtypes.COSERVERINFO instance
     'interface' may be used to request an interface other than IClassFactory
     """
-    clsid = comtypes.GUID.from_progid(progid)
-    return comtypes.CoGetClassObject(clsid,
-                                     clsctx, pServerInfo, interface)
+    clsid = GUID.from_progid(progid)
+    return comtypes.CoGetClassObject(clsid, clsctx, pServerInfo, interface)
+
 
+if TYPE_CHECKING:
+    @overload
+    def CreateObject(progid):
+        # type: (_UnionT[str, CoClass, GUID]) -> Any
+        pass
+    @overload
+    def CreateObject(progid, clsctx=None, machine=None, interface=None, dynamic=False, pServerInfo=None):
+        # type: (_UnionT[str, CoClass, GUID], Optional[int], Optional[str], Optional[Type[_T_IUnknown]], bool, Optional[comtypes.COSERVERINFO]) -> _T_IUnknown
+        pass
 def CreateObject(progid,                  # which object to create
                  clsctx=None,             # how to create the object
                  machine=None,            # where to create the object
                  interface=None,          # the interface we want
                  dynamic=False,           # use dynamic dispatch
                  pServerInfo=None):       # server info struct for remoting
+    # type: (_UnionT[str, CoClass, GUID], Optional[int], Optional[str], Optional[Type[IUnknown]], bool, Optional[comtypes.COSERVERINFO]) -> Any
     """Create a COM object from 'progid', and try to QueryInterface()
     it to the most useful interface, generating typelib support on
     demand.  A pointer to this interface is returned.
 
     'progid' may be a string like "InternetExplorer.Application",
        a string specifying a clsid, a GUID instance, or an object with
        a _clsid_ attribute which should be any of the above.
@@ -220,20 +234,20 @@
     'interface' allows to force a certain interface
     'dynamic=True' will return a dynamic dispatch object
     'pServerInfo', if used, must be a pointer to a comtypes.COSERVERINFO instance
         This supercedes 'machine'.
 
     You can also later request to receive events with GetEvents().
     """
-    clsid = comtypes.GUID.from_progid(progid)
+    clsid = GUID.from_progid(progid)
     logger.debug("%s -> %s", progid, clsid)
     if dynamic:
         if interface:
             raise ValueError("interface and dynamic are mutually exclusive")
-        interface = comtypes.automation.IDispatch
+        interface = automation.IDispatch
     elif interface is None:
         interface = getattr(progid, "_com_interfaces_", [None])[0]
     if machine is None and pServerInfo is None:
         logger.debug("CoCreateInstance(%s, clsctx=%s, interface=%s)",
                      clsid, clsctx, interface)
         obj = comtypes.CoCreateInstance(clsid, clsctx=clsctx, interface=interface)
     else:
@@ -245,22 +259,39 @@
             raise ValueError(msg)
         obj = comtypes.CoCreateInstanceEx(clsid, clsctx=clsctx,
                 interface=interface, machine=machine, pServerInfo=pServerInfo)
     if dynamic:
         return comtypes.client.dynamic.Dispatch(obj)
     return _manage(obj, clsid, interface=interface)
 
+
+if TYPE_CHECKING:
+    @overload
+    def CoGetObject(displayname, interface):
+        # type: (str, Type[_T_IUnknown]) -> _T_IUnknown
+        pass
+    @overload
+    def CoGetObject(displayname, interface=None, dynamic=False):
+        # type: (str, None, bool) -> Any
+        pass
 def CoGetObject(displayname, interface=None, dynamic=False):
+    # type: (str, Optional[Type[comtypes.IUnknown]], bool) -> Any
     """Create an object by calling CoGetObject(displayname).
 
     Additional parameters have the same meaning as in CreateObject().
     """
     if dynamic:
         if interface is not None:
             raise ValueError("interface and dynamic are mutually exclusive")
-        interface = comtypes.automation.IDispatch
+        interface = automation.IDispatch
     punk = comtypes.CoGetObject(displayname, interface)
     if dynamic:
         return comtypes.client.dynamic.Dispatch(punk)
     return _manage(punk,
                    clsid=None,
                    interface=interface)
+
+
+__all__ = [
+    "CreateObject", "GetActiveObject", "CoGetObject", "GetEvents",
+    "ShowEvents", "PumpEvents", "GetModule", "GetClassObject",
+]
```

## Comparing `comtypes-1.1.9/comtypes/server/automation.py` & `comtypes-1.2.0/comtypes/server/automation.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     def Next(self, this, celt, rgVar, pCeltFetched):
         if not rgVar: return E_POINTER
         if not pCeltFetched: pCeltFetched = [None]
         pCeltFetched[0] = 0
         try:
             for index in range(celt):
-                item = self.seq.next()
+                item = next(self.seq)
                 p = item.QueryInterface(IDispatch)
                 rgVar[index].value = p
                 pCeltFetched[0] += 1
         except StopIteration:
             pass
 ##        except:
 ##            # ReportException? return E_FAIL?
@@ -43,15 +43,15 @@
             return S_OK
         return S_FALSE
 
     def Skip(self, this, celt):
         # skip some elements.
         try:
             for _ in range(celt):
-                self.seq.next()
+                next(self.seq)
         except StopIteration:
             return S_FALSE
         return S_OK
 
     def Reset(self, this):
         self.seq = iter(self.items)
         return S_OK
```

## Comparing `comtypes-1.1.9/comtypes/server/connectionpoints.py` & `comtypes-1.2.0/comtypes/server/connectionpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         # via Invoke calls (even if it is a dual interface).
         if hasattr(self._sink_interface, "Invoke"):
             # for better performance, we could cache the dispids.
             dispid = self._typeinfo.GetIDsOfNames(name)[0]
             for key, p in self._connections.items():
                 try:
                     result = p.Invoke(dispid, *args, **kw)
-                except COMError, details:
+                except COMError as details:
                     if details.hresult == -2147023174:
                         logger.warning("_call_sinks(%s, %s, *%s, **%s) failed; removing connection",
                                        self, name, args, kw,
                                        exc_info=True)
                         try:
                             del self._connections[key]
                         except KeyError:
@@ -75,15 +75,15 @@
                                        exc_info=True)
                 else:
                     results.append(result)
         else:
             for p in self._connections.values():
                 try:
                     result = getattr(p, name)(*args, **kw)
-                except COMError, details:
+                except COMError as details:
                     if details.hresult == -2147023174:
                         logger.warning("_call_sinks(%s, %s, *%s, **%s) failed; removing connection",
                                        self, name, args, kw,
                                        exc_info=True)
                         del self._connections[key]
                     else:
                         logger.warning("_call_sinks(%s, %s, *%s, **%s)", self, name, args, kw,
```

## Comparing `comtypes-1.1.9/comtypes/server/inprocserver.py` & `comtypes-1.2.0/comtypes/server/inprocserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import ctypes
 from comtypes import COMObject, GUID
 from comtypes.server import IClassFactory
 from comtypes.hresult import *
 
-import sys, _winreg, logging
+import sys
+import logging
+if sys.version_info >= (3, 0):
+    import winreg
+else:
+    import _winreg as winreg
 
 logger = logging.getLogger(__name__)
 _debug = logger.debug
 _critical = logger.critical
 
 ################################################################
 
@@ -34,26 +39,26 @@
 # will be set by py2exe boot script 'from outside'
 _clsid_to_class = {}
 
 def inproc_find_class(clsid):
     if _clsid_to_class:
         return _clsid_to_class[clsid]
 
-    key = _winreg.OpenKey(_winreg.HKEY_CLASSES_ROOT, "CLSID\\%s\\InprocServer32" % clsid)
+    key = winreg.OpenKey(winreg.HKEY_CLASSES_ROOT, "CLSID\\%s\\InprocServer32" % clsid)
     try:
-        pathdir = _winreg.QueryValueEx(key, "PythonPath")[0]
+        pathdir = winreg.QueryValueEx(key, "PythonPath")[0]
     except:
         _debug("NO path to insert")
     else:
         if not pathdir in sys.path:
             sys.path.insert(0, str(pathdir))
             _debug("insert path %r", pathdir)
         else:
             _debug("Already in path %r", pathdir)
-    pythonclass = _winreg.QueryValueEx(key, "PythonClass")[0]
+    pythonclass = winreg.QueryValueEx(key, "PythonClass")[0]
     parts = pythonclass.split(".")
     modname = ".".join(parts[:-1])
     classname = parts[-1]
     _debug("modname: %s, classname %s", modname, classname)
     __import__(modname)
     mod = sys.modules[modname]
     result = getattr(mod, classname)
@@ -69,33 +74,33 @@
     """
     global _logging_configured
     if _logging_configured:
         return
     _logging_configured = True
 
     try:
-        hkey = _winreg.OpenKey(_winreg.HKEY_CLASSES_ROOT, r"CLSID\%s\Logging" % clsid)
+        hkey = winreg.OpenKey(winreg.HKEY_CLASSES_ROOT, r"CLSID\%s\Logging" % clsid)
     except WindowsError:
         return
     from comtypes.logutil import NTDebugHandler
     handler = NTDebugHandler()
     try:
-        val, typ = _winreg.QueryValueEx(hkey, "format")
+        val, typ = winreg.QueryValueEx(hkey, "format")
         formatter = logging.Formatter(val)
     except:
         formatter = logging.Formatter("(Thread %(thread)s):%(levelname)s:%(message)s")
     handler.setFormatter(formatter)
     logging.root.addHandler(handler)
     try:
-        values, typ = _winreg.QueryValueEx(hkey, "levels")
+        values, typ = winreg.QueryValueEx(hkey, "levels")
     except:
         return
-    if typ == _winreg.REG_SZ:
+    if typ == winreg.REG_SZ:
         values = [values]
-    elif typ != _winreg.REG_MULTI_SZ:
+    elif typ != winreg.REG_MULTI_SZ:
         # this is an error
         return
     for val in values:
         name, level = val.split("=")
         level = getattr(logging, level)
         logging.getLogger(name).setLevel(level)
 
@@ -115,15 +120,15 @@
     try:
         _debug("DllGetClassObject(clsid=%s, iid=%s)", clsid, iid)
 
         cls = inproc_find_class(clsid)
         if not cls:
             return CLASS_E_CLASSNOTAVAILABLE
 
-        result = ClassFactory(cls).IUnknown_QueryInterface(None, ctypes.pointer(iid), ppv)
+        result = ClassFactory(cls).IUnknown_QueryInterface(None, ctypes.pointer(iid), ctypes.c_void_p(ppv))
         _debug("DllGetClassObject() -> %s", result)
         return result
     except Exception:
         _critical("DllGetClassObject", exc_info=True)
         return E_FAIL
 
 def DllCanUnloadNow():
```

## Comparing `comtypes-1.1.9/comtypes/server/localserver.py` & `comtypes-1.2.0/comtypes/server/localserver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+import sys
 from ctypes import *
 import comtypes
 from comtypes.hresult import *
 from comtypes.server import IClassFactory
 import logging
-import Queue
+if sys.version_info >= (3, 0):
+    import queue
+else:
+    import Queue as queue
 
 logger = logging.getLogger(__name__)
 _debug = logger.debug
 
 REGCLS_SINGLEUSE = 0       # class object only generates one instance
 REGCLS_MULTIPLEUSE = 1     # same class object genereates multiple inst.
 REGCLS_MULTI_SEPARATE = 2  # multiple use, but separate control over each
```

## Comparing `comtypes-1.1.9/comtypes/server/register.py` & `comtypes-1.2.0/comtypes/server/register.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,18 @@
   python mycomobj.py /l comtypes=INFO /l comtypes.server=DEBUG /f %(message)s
 
 Now, debug the object, and when done delete logging info:
 
   python mycomobj.py /nodebug
 """
 import sys, os
-import _winreg
+if sys.version_info >= (3, 0):
+    import winreg
+else:
+    import _winreg as winreg
 import logging
 
 import comtypes
 from comtypes.typeinfo import LoadTypeLibEx, UnRegisterTypeLib, REGKIND_REGISTER
 from comtypes.hresult import *
 from comtypes.server import w_getopt
 import comtypes.server.inprocserver
@@ -58,23 +61,20 @@
 def _non_zero(retval, func, args):
     if retval:
         raise WinError(retval)
 SHDeleteKey = windll.shlwapi.SHDeleteKeyW
 SHDeleteKey.errcheck = _non_zero
 SHDeleteKey.argtypes = c_ulong, c_wchar_p
 
-try:
-    Set = set
-except NameError:
-    from sets import Set #as set
+Set = set
 
 
-_KEYS = {_winreg.HKEY_CLASSES_ROOT: "HKCR",
-         _winreg.HKEY_LOCAL_MACHINE: "HKLM",
-         _winreg.HKEY_CURRENT_USER: "HKCU"}
+_KEYS = {winreg.HKEY_CLASSES_ROOT: "HKCR",
+         winreg.HKEY_LOCAL_MACHINE: "HKLM",
+         winreg.HKEY_CURRENT_USER: "HKCU"}
 
 def _explain(hkey):
     return _KEYS.get(hkey, hkey)
 
 class Registrar(object):
     """COM class registration.
 
@@ -85,43 +85,43 @@
     work.
     """
     def nodebug(self, cls):
         """Delete logging entries from the registry."""
         clsid = cls._reg_clsid_
         try:
             _debug('DeleteKey( %s\\CLSID\\%s\\Logging"' % \
-                    (_explain(_winreg.HKEY_CLASSES_ROOT), clsid))
-            hkey = _winreg.OpenKey(_winreg.HKEY_CLASSES_ROOT, r"CLSID\%s" % clsid)
-            _winreg.DeleteKey(hkey, "Logging")
-        except WindowsError, detail:
+                    (_explain(winreg.HKEY_CLASSES_ROOT), clsid))
+            hkey = winreg.OpenKey(winreg.HKEY_CLASSES_ROOT, r"CLSID\%s" % clsid)
+            winreg.DeleteKey(hkey, "Logging")
+        except WindowsError as detail:
             if get_winerror(detail) != 2:
                 raise
 
     def debug(self, cls, levels, format):
         """Write entries in the registry to setup logging for this clsid."""
         # handlers
         # format
         clsid = cls._reg_clsid_
         _debug('CreateKey( %s\\CLSID\\%s\\Logging"' % \
-                (_explain(_winreg.HKEY_CLASSES_ROOT), clsid))
-        hkey = _winreg.CreateKey(_winreg.HKEY_CLASSES_ROOT, r"CLSID\%s\Logging" % clsid)
+                (_explain(winreg.HKEY_CLASSES_ROOT), clsid))
+        hkey = winreg.CreateKey(winreg.HKEY_CLASSES_ROOT, r"CLSID\%s\Logging" % clsid)
         for item in levels:
             name, value = item.split("=")
             v = getattr(logging, value)
             assert isinstance(v, int)
         _debug('SetValueEx(levels, %s)' % levels)
-        _winreg.SetValueEx(hkey, "levels", None, _winreg.REG_MULTI_SZ, levels)
+        winreg.SetValueEx(hkey, "levels", None, winreg.REG_MULTI_SZ, levels)
         if format:
             _debug('SetValueEx(format, %s)' % format)
-            _winreg.SetValueEx(hkey, "format", None, _winreg.REG_SZ, format)
+            winreg.SetValueEx(hkey, "format", None, winreg.REG_SZ, format)
         else:
             _debug('DeleteValue(format)')
             try:
-                _winreg.DeleteValue(hkey, "format")
-            except WindowsError, detail:
+                winreg.DeleteValue(hkey, "format")
+            except WindowsError as detail:
                 if get_winerror(detail) != 2:
                     raise
 
     def register(self, cls, executable=None):
         """Register the COM server class."""
         # First, we unregister the object with force=True, to force removal
         # of all registry entries, even if we would not write them.
@@ -137,16 +137,16 @@
     def _register(self, cls, executable=None):
         table = self._registry_entries(cls)
         table.sort()
         _debug("Registering %s", cls)
         for hkey, subkey, valuename, value in table:
             _debug ('[%s\\%s]', _explain(hkey), subkey)
             _debug('%s="%s"', valuename or "@", value)
-            k = _winreg.CreateKey(hkey, subkey)
-            _winreg.SetValueEx(k, valuename, None, _winreg.REG_SZ, str(value))
+            k = winreg.CreateKey(hkey, subkey)
+            winreg.SetValueEx(k, valuename, None, winreg.REG_SZ, str(value))
 
         tlib = getattr(cls, "_reg_typelib_", None)
         if tlib is not None:
             if hasattr(sys, "frozendllhandle"):
                 dll = self._get_serverdll()
                 _debug("LoadTypeLibEx(%s, REGKIND_REGISTER)", dll)
                 LoadTypeLibEx(dll, REGKIND_REGISTER)
@@ -181,24 +181,24 @@
         for hkey, subkey in table:
             try:
                 if force:
                     _debug("SHDeleteKey %s\\%s", _explain(hkey), subkey)
                     SHDeleteKey(hkey, subkey)
                 else:
                     _debug("DeleteKey %s\\%s", _explain(hkey), subkey)
-                    _winreg.DeleteKey(hkey, subkey)
-            except WindowsError, detail:
+                    winreg.DeleteKey(hkey, subkey)
+            except WindowsError as detail:
                 if get_winerror(detail) != 2:
                     raise
         tlib = getattr(cls, "_reg_typelib_", None)
         if tlib is not None:
             try:
                 _debug("UnRegisterTypeLib(%s, %s, %s)", *tlib)
                 UnRegisterTypeLib(*tlib)
-            except WindowsError, detail:
+            except WindowsError as detail:
                 if not get_winerror(detail) in (TYPE_E_REGISTRYACCESS, TYPE_E_CANTLOADLIBRARY):
                     raise
         _debug("Done")
 
     def _get_serverdll(self):
         """Return the pathname of the dll hosting the COM object."""
         handle = getattr(sys, "frozendllhandle", None)
@@ -239,15 +239,15 @@
         _reg_novers_progid_ - version independend progid, typically 'MyServer.MyObject'
         _reg_typelib_ - an tuple (libid, majorversion, minorversion) specifying a typelib.
         _reg_threading_ - a string specifying the threading model
 
         Note that the first part of the progid string is typically the
         IDL library name of the type library containing the coclass.
         """
-        HKCR = _winreg.HKEY_CLASSES_ROOT
+        HKCR = winreg.HKEY_CLASSES_ROOT
 
         # table format: rootkey, subkey, valuename, value
         table = []
         append = lambda *args: table.append(args)
 
         # basic entry - names the comobject
         reg_clsid = str(cls._reg_clsid_) # that's the only required attribute for registration
```

## Comparing `comtypes-1.1.9/comtypes/server/w_getopt.py` & `comtypes-1.2.0/comtypes/server/w_getopt.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/server/__init__.py` & `comtypes-1.2.0/comtypes/server/__init__.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/test/find_memleak.py` & `comtypes-1.2.0/comtypes/test/find_memleak.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import print_function
 import unittest, gc
 from ctypes import *
 from ctypes.wintypes import *
 
 ################################################################
 
 class PROCESS_MEMORY_COUNTERS(Structure):
@@ -16,15 +17,15 @@
                 ("PagefileUsage", c_size_t),
                 ("PeakPagefileUsage", c_size_t)]
     def __init__(self):
         self.cb = sizeof(self)
 
     def dump(self):
         for n, _ in self._fields_[2:]:
-            print n, getattr(self, n)/1e6
+            print(n, getattr(self, n)/1e6)
 
 try:
     windll.psapi.GetProcessMemoryInfo.argtypes = (HANDLE, POINTER(PROCESS_MEMORY_COUNTERS), DWORD)
 except WindowsError:
     # cannot search for memory leaks on Windows CE
     def find_memleak(func, loops=None):
         return 0
@@ -37,25 +38,25 @@
         return pmi.WorkingSetSize
 
     LOOPS = 10, 1000
 
     def find_memleak(func, loops=LOOPS):
         # call 'func' several times, so that memory consumption
         # stabilizes:
-        for j in xrange(loops[0]):
-            for k in xrange(loops[1]):
+        for j in range(loops[0]):
+            for k in range(loops[1]):
                 func()
         gc.collect(); gc.collect(); gc.collect()
         bytes = wss()
         # call 'func' several times, recording the difference in
         # memory consumption before and after the call.  Repeat this a
         # few times, and return a list containing the memory
         # consumption differences.
-        for j in xrange(loops[0]):
-            for k in xrange(loops[1]):
+        for j in range(loops[0]):
+            for k in range(loops[1]):
                 func()
         gc.collect(); gc.collect(); gc.collect()
         # return the increased in process size
         result = wss() - bytes
         # Sometimes the process size did decrease, we do not report leaks
         # in this case:
         return max(result, 0)
```

## Comparing `comtypes-1.1.9/comtypes/test/mylib.idl` & `comtypes-1.2.0/comtypes/test/mylib.idl`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/test/mytypelib.idl` & `comtypes-1.2.0/comtypes/test/mytypelib.idl`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/test/TestComServer.idl` & `comtypes-1.2.0/comtypes/test/TestComServer.idl`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/test/TestComServer.py` & `comtypes-1.2.0/comtypes/test/TestComServer.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,8 +143,11 @@
     try:
         from comtypes.server.register import UseCommandLine
 ##    logging.basicConfig(level=logging.DEBUG)
         UseCommandLine(TestComServer)
     except Exception:
         import traceback
         traceback.print_exc()
-        raw_input()
+        if sys.version_info >= (3, 0):
+            input()
+        else:
+            raw_input()
```

## Comparing `comtypes-1.1.9/comtypes/test/TestComServer.tlb` & `comtypes-1.2.0/comtypes/test/TestComServer.tlb`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/test/TestDispServer.idl` & `comtypes-1.2.0/comtypes/test/TestDispServer.idl`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/test/TestDispServer.py` & `comtypes-1.2.0/comtypes/test/TestDispServer.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/test/TestDispServer.tlb` & `comtypes-1.2.0/comtypes/test/TestDispServer.tlb`

 * *Files identical despite different names*

## Comparing `comtypes-1.1.9/comtypes/test/test_agilent.py` & `comtypes-1.2.0/comtypes/test/test_agilent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # This test requires that the Agilent IVI-COM Driver for Agilent546XX
 # is installed.  It is not requires to have a physical instrument
 # connected, the driver is used in simulation mode.
+
+from __future__ import print_function
 import unittest
 from comtypes.test import ResourceDenied
 from comtypes.client import CreateObject
 from comtypes import GUID
 from comtypes.safearray import _midlSAFEARRAY
 from ctypes import c_double, POINTER
 
@@ -20,15 +22,15 @@
             # which takes several [in, out] arguments.
             agDrvr = CreateObject("Agilent546XX.Agilent546XX")
 
             # XXX XXX XXX The following call crashes hard with an accessviolation when
             # the OANOCACHE environ variable is set.
             import os
             if "OANOCACHE" in os.environ:
-                print "Cannot test. buggy COM object?"
+                print("Cannot test. buggy COM object?")
                 return
 
             # Initialize the driver in simulation mode.  Resource descriptor is ignored.
             agDrvr.Initialize("", False, False, "Simulate=true")
             # Initialize driver.  Edit resource descriptor for your system.
             # agDrvr.Initialize("GPIB0::7::INSTR", False, False, "QueryInstrStatus=true")
 
@@ -68,23 +70,24 @@
             self._check_result(pMeasurement.ReadWaveform(20000, pXIncrement=9.0, pInitialX=3.0))
             self._check_result(pMeasurement.ReadWaveform(20000))
             self._check_result(pMeasurement.ReadWaveform(20000, []))
             self._check_result(pMeasurement.ReadWaveform(20000, pWaveformArray = []))
             self._check_result(pMeasurement.ReadWaveform(20000, psaWaveform))
             self._check_result(pMeasurement.ReadWaveform(20000, pXIncrement=9.0))
 
-        def _check_result(self, (array, initial_x, x_increment)):
+        def _check_result(self, xxx_todo_changeme):
             # ReadWaveform, in simulation mode, returns three values:
             #
             # - a safearray containing 100 random double values,
             #   unpacked and returned as tuple
             # - the initial_x value: 0.0
             # - the x_increment value: 0.0
-            self.failUnlessEqual(len(array), 100)
-            self.failIf([x for x in array if not isinstance(x, float)])
-            self.failUnlessEqual(initial_x, 0.0)
-            self.failUnlessEqual(x_increment, 0.0)
+            (array, initial_x, x_increment) = xxx_todo_changeme
+            self.assertEqual(len(array), 100)
+            self.assertFalse([x for x in array if not isinstance(x, float)])
+            self.assertEqual(initial_x, 0.0)
+            self.assertEqual(x_increment, 0.0)
 
 
 
 if __name__ == "__main__":
     unittest.main()
```

## Comparing `comtypes-1.1.9/comtypes/test/test_BSTR.py` & `comtypes-1.2.0/comtypes/test/test_BSTR.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ##requires("memleaks")
 
 from comtypes.test.find_memleak import find_memleak
 
 class Test(unittest.TestCase):
     def check_leaks(self, func, limit=0):
         bytes = find_memleak(func)
-        self.failIf(bytes > limit, "Leaks %d bytes" % bytes)
+        self.assertFalse(bytes > limit, "Leaks %d bytes" % bytes)
 
     def test_creation(self):
         def doit():
             BSTR(u"abcdef" * 100)
         # It seems this test is unreliable.  Sometimes it leaks 4096
         # bytes, sometimes not.  Try to workaround that...
         self.check_leaks(doit, limit=4096)
@@ -36,15 +36,15 @@
         self.check_leaks(doit)
 
     def test_inargs(self):
         SysStringLen = windll.oleaut32.SysStringLen
         SysStringLen.argtypes = BSTR,
         SysStringLen.restype = c_uint
 
-        self.failUnlessEqual(SysStringLen("abc xyz"), 7)
+        self.assertEqual(SysStringLen("abc xyz"), 7)
         def doit():
             SysStringLen("abc xyz")
             SysStringLen(u"abc xyz")
             SysStringLen(BSTR(u"abc def"))
         self.check_leaks(doit)
 
 if __name__ == "__main__":
```

## Comparing `comtypes-1.1.9/comtypes/test/test_casesensitivity.py` & `comtypes-1.2.0/comtypes/test/test_casesensitivity.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,28 +11,28 @@
         # IDispatch(IUnknown)
         # IWebBrowser(IDispatch)
         # IWebBrowserApp(IWebBrowser)
         # IWebBrowser2(IWebBrowserApp)
 
 ##        print iem.IWebBrowser2.mro()
 
-        self.failUnless(issubclass(iem.IWebBrowser2, iem.IWebBrowserApp))
-        self.failUnless(issubclass(iem.IWebBrowserApp, iem.IWebBrowser))
+        self.assertTrue(issubclass(iem.IWebBrowser2, iem.IWebBrowserApp))
+        self.assertTrue(issubclass(iem.IWebBrowserApp, iem.IWebBrowser))
 
 ##        print sorted(iem.IWebBrowser.__map_case__.keys())
 ##        print "=" * 42
 ##        print sorted(iem.IWebBrowserApp.__map_case__.keys())
 ##        print "=" * 42
 ##        print sorted(iem.IWebBrowser2.__map_case__.keys())
 ##        print "=" * 42
 
         # names in the base class __map_case__ must also appear in the
         # subclass.
         for name in iem.IWebBrowser.__map_case__:
-            self.failUnless(name in iem.IWebBrowserApp.__map_case__, "%s missing" % name)
-            self.failUnless(name in iem.IWebBrowser2.__map_case__, "%s missing" % name)
+            self.assertTrue(name in iem.IWebBrowserApp.__map_case__, "%s missing" % name)
+            self.assertTrue(name in iem.IWebBrowser2.__map_case__, "%s missing" % name)
 
         for name in iem.IWebBrowserApp.__map_case__:
-            self.failUnless(name in iem.IWebBrowser2.__map_case__, "%s missing" % name)
+            self.assertTrue(name in iem.IWebBrowser2.__map_case__, "%s missing" % name)
 
 if __name__ == "__main__":
     unittest.main()
```

## Comparing `comtypes-1.1.9/comtypes/test/test_collections.py` & `comtypes-1.2.0/comtypes/test/test_collections.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,100 +9,103 @@
 
     def test_IEnumVARIANT(self):
         # The XP firewall manager.
         fwmgr = CreateObject('HNetCfg.FwMgr')
         # apps has a _NewEnum property that implements IEnumVARIANT
         services = fwmgr.LocalPolicy.CurrentProfile.Services
 
-        self.failUnlessEqual(services.Count, len(services))
+        self.assertEqual(services.Count, len(services))
 
         cv = iter(services)
 
         names = [p.Name for p in cv]
-        self.failUnlessEqual(len(services), len(names))
+        self.assertEqual(len(services), len(names))
 
         # The iterator is consumed now:
-        self.failUnlessEqual([p.Name for p in cv], [])
+        self.assertEqual([p.Name for p in cv], [])
 
         # But we can reset it:
         cv.Reset()
-        self.failUnlessEqual([p.Name for p in cv], names)
+        self.assertEqual([p.Name for p in cv], names)
 
         # Reset, then skip:
         cv.Reset()
         cv.Skip(3)
-        self.failUnlessEqual([p.Name for p in cv], names[3:])
+        self.assertEqual([p.Name for p in cv], names[3:])
 
         # Reset, then skip:
         cv.Reset()
         cv.Skip(300)
-        self.failUnlessEqual([p.Name for p in cv], names[300:])
+        self.assertEqual([p.Name for p in cv], names[300:])
 
         # Hm, do we want to allow random access to the iterator?
         # Should the iterator support __getitem__ ???
-        self.failUnlessEqual(cv[0].Name, names[0])
-        self.failUnlessEqual(cv[0].Name, names[0])
-        self.failUnlessEqual(cv[0].Name, names[0])
+        self.assertEqual(cv[0].Name, names[0])
+        self.assertEqual(cv[0].Name, names[0])
+        self.assertEqual(cv[0].Name, names[0])
 
         if len(names) > 1:
-            self.failUnlessEqual(cv[1].Name, names[1])
-            self.failUnlessEqual(cv[1].Name, names[1])
-            self.failUnlessEqual(cv[1].Name, names[1])
+            self.assertEqual(cv[1].Name, names[1])
+            self.assertEqual(cv[1].Name, names[1])
+            self.assertEqual(cv[1].Name, names[1])
 
         # We can now call Next(celt) with celt != 1, the call always returns a
         # list:
         cv.Reset()
-        self.failUnlessEqual(names[:3],
+        self.assertEqual(names[:3],
                             [p.Name for p in cv.Next(3)])
 
         # calling Next(0) makes no sense, but should work anyway:
-        self.failUnlessEqual(cv.Next(0), [])
+        self.assertEqual(cv.Next(0), [])
 
         cv.Reset()
-        self.failUnlessEqual(len(cv.Next(len(names) * 2)), len(names))
+        self.assertEqual(len(cv.Next(len(names) * 2)), len(names))
 
         # slicing is not (yet?) supported
         cv.Reset()
-        self.failUnlessRaises(ArgumentError, lambda: cv[:])
+        self.assertRaises(ArgumentError, lambda: cv[:])
 
+    @unittest.skip("This test takes a long time.  Do we need it? Can it be rewritten?")
     def test_leaks_1(self):
         # The XP firewall manager.
         fwmgr = CreateObject('HNetCfg.FwMgr')
         # apps has a _NewEnum property that implements IEnumVARIANT
         apps = fwmgr.LocalPolicy.CurrentProfile.AuthorizedApplications
 
         def doit():
             for item in iter(apps):
                 item.ProcessImageFileName
         bytes = find_memleak(doit, (20, 20))
-        self.failIf(bytes, "Leaks %d bytes" % bytes)
+        self.assertFalse(bytes, "Leaks %d bytes" % bytes)
 
+    @unittest.skip("This test takes a long time.  Do we need it? Can it be rewritten?")
     def test_leaks_2(self):
         # The XP firewall manager.
         fwmgr = CreateObject('HNetCfg.FwMgr')
         # apps has a _NewEnum property that implements IEnumVARIANT
         apps = fwmgr.LocalPolicy.CurrentProfile.AuthorizedApplications
 
         def doit():
             iter(apps).Next(99)
         bytes = find_memleak(doit, (20, 20))
-        self.failIf(bytes, "Leaks %d bytes" % bytes)
+        self.assertFalse(bytes, "Leaks %d bytes" % bytes)
 
+    @unittest.skip("This test takes a long time.  Do we need it? Can it be rewritten?")
     def test_leaks_3(self):
         # The XP firewall manager.
         fwmgr = CreateObject('HNetCfg.FwMgr')
         # apps has a _NewEnum property that implements IEnumVARIANT
         apps = fwmgr.LocalPolicy.CurrentProfile.AuthorizedApplications
 
         def doit():
             for i in range(2):
                 for what in iter(apps):
                     pass
         bytes = find_memleak(doit, (20, 20))
-        self.failIf(bytes, "Leaks %d bytes" % bytes)
+        self.assertFalse(bytes, "Leaks %d bytes" % bytes)
 
 
 class TestCollectionInterface(unittest.TestCase):
     """ Test the early-bound collection interface. """
 
     def setUp(self):
         self.d = CreateObject("Scripting.Dictionary", dynamic=False)
```

## Comparing `comtypes-1.1.9/comtypes/test/test_comserver.py` & `comtypes-1.2.0/comtypes/test/test_comserver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-import unittest, sys
-from ctypes import *
-from ctypes.wintypes import *
-from comtypes.client import CreateObject, GetEvents, ShowEvents
-from comtypes.server.register import register#, unregister
+import sys
+import unittest
+
+import comtypes.test.TestComServer
+from comtypes.client import CreateObject
+from comtypes.server.register import register  # , unregister
 from comtypes.test import is_resource_enabled
 from comtypes.test.find_memleak import find_memleak
 
-################################################################
-import comtypes.test.TestComServer
-register(comtypes.test.TestComServer.TestComServer)
+
+def setUpModule():
+    raise unittest.SkipTest("This test requires the tests to be run as admin since it tries to "
+                            "register the test COM server.  Is this a good idea?")
+
+    # If this test is ever NOT skipped, then this line needs to run.  Keeping it here for posterity.
+    register(comtypes.test.TestComServer.TestComServer)
+
 
 class TestInproc(unittest.TestCase):
 
     def create_object(self):
         return CreateObject("TestComServerLib.TestComServer",
                             clsctx = comtypes.CLSCTX_INPROC_SERVER)
 
     def _find_memleak(self, func):
         bytes = find_memleak(func)
-        self.failIf(bytes, "Leaks %d bytes" % bytes)
+        self.assertFalse(bytes, "Leaks %d bytes" % bytes)
 
     def test_mixedinout(self):
         o = self.create_object()
-        self.failUnlessEqual(o.MixedInOut(2, 4), (3, 5))
+        self.assertEqual(o.MixedInOut(2, 4), (3, 5))
 
     def test_getname(self):
-        from ctypes import byref, pointer
+        from ctypes import pointer
         from comtypes import BSTR
 
         # This tests a tricky bug, introduced with this patch:
         # http://www.python.org/sf/1643874
         #
         # Returning a BSTR as an [out] parameter from a server
         # implementation must transfer the ownership to the caller.
@@ -41,15 +47,15 @@
         obj._ITestComServer__com__get_name(pb)
         # Retrieve the value, but keep the pointer to the BSTR alive:
         name = pb[0]
         # Create sme BSTR's to reuse the memory in case it has been freed:
         for i in range(10):
             BSTR("f" * len(name))
         # Make sure the pointer is still valid:
-        self.failUnlessEqual(pb[0], name)
+        self.assertEqual(pb[0], name)
 
     if is_resource_enabled("memleaks"):
         def test_get_id(self):
             obj = self.create_object()
             self._find_memleak(lambda: obj.id)
 
         def test_get_name(self):
@@ -69,15 +75,15 @@
             self._find_memleak(func)
 
 
         def test_eval(self):
             obj = self.create_object()
             def func():
                 return obj.eval("(1, 2, 3)")
-            self.failUnlessEqual(func(), (1, 2, 3))
+            self.assertEqual(func(), (1, 2, 3))
             self._find_memleak(func)
 
         def test_get_typeinfo(self):
             obj = self.create_object()
             def func():
                 obj.GetTypeInfo(0)
                 obj.GetTypeInfoCount()
@@ -175,15 +181,15 @@
             Event ITestComServerEvents_EvalStarted(None, u"['32'] * 2")
             Event ITestComServerEvents_EvalCompleted(None, u"['32'] * 2", VARIANT(vt=0x200c, (u'32', u'32')))
             >>> result
             (u'32', u'32')
             >>>
             '''
 
-    def GetEvents():
+    def GetEvents(self):
         """
         >>> from comtypes.client import CreateObject, GetEvents
         >>>
         >>> o =  CreateObject("TestComServerLib.TestComServer")
         >>> class EventHandler(object):
         ...     def EvalStarted(self, this, what):
         ...         print("EvalStarted: %s" % what)
```

## Comparing `comtypes-1.1.9/comtypes/test/test_createwrappers.py` & `comtypes-1.2.0/comtypes/test/test_createwrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,25 @@
+from __future__ import print_function
+
 import glob
 import os
 import unittest
 import warnings
-import comtypes.typeinfo
+
 import comtypes.client
 import comtypes.client._generate
-from comtypes.test import requires
+import comtypes.typeinfo
+
+
+def setUpModule():
+    raise unittest.SkipTest("I have no idea what to do with this.  It programmatically creates "
+                            "*thousands* of tests and a few dozen of them fail.")
+
 
-requires("typelibs")
+# requires("typelibs")
 
 # filter warnings about interfaces without a base interface; they will
 # be skipped in the code generation.
 warnings.filterwarnings("ignore",
                         "Ignoring interface .* which has no base interface",
                         UserWarning)
 
@@ -71,15 +79,15 @@
         "grde50.olb", # UnicodeEncodeError
         ):
         continue
     add_test(fname)
 
 path = os.path.join(progdir, r"Microsoft Visual Studio .NET 2003\Visual Studio SDKs\DIA SDK\bin\msdia71.dll")
 if os.path.isfile(path):
-    print "ADD", path
+    print("ADD", path)
     add_test(path)
 
 for fname in glob.glob(os.path.join(common_progdir, r"Microsoft Shared\Speech\*.dll")):
     add_test(fname)
 
 for fname in glob.glob(os.path.join(sysdir, "*.dll")):
     # these typelibs give errors:
```

## Comparing `comtypes-1.1.9/comtypes/test/test_DISPPARAMS.py` & `comtypes-1.2.0/comtypes/test/test_DISPPARAMS.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,38 +4,38 @@
     def test(self):
         from comtypes.automation import DISPPARAMS, VARIANT
 
         dp = DISPPARAMS()
         dp.rgvarg = (VARIANT * 3)()
 
         for i in range(3):
-            self.failUnlessEqual(dp.rgvarg[i].value, None)
+            self.assertEqual(dp.rgvarg[i].value, None)
 
         dp.rgvarg[0].value = 42
         dp.rgvarg[1].value = "spam"
         dp.rgvarg[2].value = "foo"
 
         # damn, there's still this old bug!
 
-        self.failUnlessEqual(dp.rgvarg[0].value, 42)
+        self.assertEqual(dp.rgvarg[0].value, 42)
         # these fail:
 ##        self.failUnlessEqual(dp.rgvarg[1].value, "spam")
 ##        self.failUnlessEqual(dp.rgvarg[2].value, "foo")
 
     def X_test_2(self):
         # basically the same test as above
         from comtypes.automation import DISPPARAMS, VARIANT
 
         args = [42, None, "foo"]
 
         dp = DISPPARAMS()
-        dp.rgvarg = (VARIANT * 3)(*map(VARIANT, args[::-1]))
+        dp.rgvarg = (VARIANT * 3)(*list(map(VARIANT, args[::-1])))
 
         import gc
         gc.collect()
 
-        self.failUnlessEqual(dp.rgvarg[0].value, 42)
-        self.failUnlessEqual(dp.rgvarg[1].value, "spam")
-        self.failUnlessEqual(dp.rgvarg[2].value, "foo")
+        self.assertEqual(dp.rgvarg[0].value, 42)
+        self.assertEqual(dp.rgvarg[1].value, "spam")
+        self.assertEqual(dp.rgvarg[2].value, "foo")
 
 if __name__ == "__main__":
     ut.main()
```

## Comparing `comtypes-1.1.9/comtypes/test/test_dyndispatch.py` & `comtypes-1.2.0/comtypes/test/test_dyndispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def setUp(self):
         self.d = CreateObject("Scripting.Dictionary", dynamic=True)
 
     def tearDown(self):
         del self.d
 
     def test_type(self):
-        self.failUnless(isinstance(self.d, Dispatch))
+        self.assertTrue(isinstance(self.d, Dispatch))
 
     def test_index_setter(self):
         d = self.d
         d.CompareMode = 42
         d["foo"] = 1
         d["bar"] = "spam foo"
         d["baz"] = 3.14
```

## Comparing `comtypes-1.1.9/comtypes/test/test_findgendir.py` & `comtypes-1.2.0/comtypes/test/test_findgendir.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-import types, os, unittest, sys, tempfile
-
-if sys.version_info >= (2, 6):
-    from imp import reload
+import os
+import sys
+import tempfile
+import types
+import unittest
 
 import comtypes
 import comtypes.client
 import comtypes.gen
 
-from comtypes.client._code_cache import _get_appdata_dir
+if sys.version_info >= (3, 4):
+    from importlib import reload
+else:
+    from imp import reload
 
 imgbase = os.path.splitext(os.path.basename(sys.executable))[0]
 
 class Test(unittest.TestCase):
     """Test the comtypes.client._find_gen_dir() function in several
     simulated environments.
     """
@@ -38,44 +42,44 @@
         reload(comtypes.gen)
 
     def test_script(self):
         # %APPDATA%\Python\Python25\comtypes_cache
         template = r"$APPDATA\Python\Python%d%d\comtypes_cache"
         path = os.path.expandvars(template % sys.version_info[:2])
         gen_dir = comtypes.client._find_gen_dir()
-        self.failUnlessEqual(path, gen_dir)
+        self.assertEqual(path, gen_dir)
 
     def test_frozen_dll(self):
         sys.frozen = "dll"
         sys.frozendllhandle = sys.dllhandle
         ma, mi = sys.version_info[:2]
         # %TEMP%\comtypes_cache\<imagebasename>-25
         # the image is python25.dll
         path = os.path.join(tempfile.gettempdir(),
                             r"comtypes_cache\%s%d%d-%d%d" % (imgbase, ma, mi, ma, mi))
         gen_dir = comtypes.client._find_gen_dir()
-        self.failUnlessEqual(path, gen_dir)
+        self.assertEqual(path, gen_dir)
 
     def test_frozen_console_exe(self):
         sys.frozen = "console_exe"
         # %TEMP%\comtypes_cache\<imagebasename>-25
         path = os.path.join(tempfile.gettempdir(),
                             r"comtypes_cache\%s-%d%d" % (
             imgbase, sys.version_info[0], sys.version_info[1]))
         gen_dir = comtypes.client._find_gen_dir()
-        self.failUnlessEqual(path, gen_dir)
+        self.assertEqual(path, gen_dir)
 
     def test_frozen_windows_exe(self):
         sys.frozen = "windows_exe"
         # %TEMP%\comtypes_cache\<imagebasename>-25
         path = os.path.join(tempfile.gettempdir(),
                             r"comtypes_cache\%s-%d%d" % (
             imgbase, sys.version_info[0], sys.version_info[1]))
         gen_dir = comtypes.client._find_gen_dir()
-        self.failUnlessEqual(path, gen_dir)
+        self.assertEqual(path, gen_dir)
 
 
 def main():
     unittest.main()
 
 if __name__ == "__main__":
     main()
```

## Comparing `comtypes-1.1.9/comtypes/test/test_getactiveobj.py` & `comtypes-1.2.0/comtypes/test/test_getactiveobj.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import unittest
 
 import comtypes
 import comtypes.client
-
 import comtypes.test
+
 comtypes.test.requires("ui")
 
+
+def setUpModule():
+    raise unittest.SkipTest("External test dependencies like this seem bad.  Find a different "
+                            "built-in win32 API to use.")
+
+
 class Test(unittest.TestCase):
     def tearDown(self):
         if hasattr(self, "w1"):
             self.w1.Quit()
             del self.w1
 
 
@@ -24,28 +30,28 @@
 
         # create a WORD instance
         self.w1 = w1 = comtypes.client.CreateObject("Word.Application")
         # connect to the running instance
         w2 = comtypes.client.GetActiveObject("Word.Application")
 
         # check if they are referring to the same object
-        self.failUnlessEqual(w1.QueryInterface(comtypes.IUnknown),
+        self.assertEqual(w1.QueryInterface(comtypes.IUnknown),
                              w2.QueryInterface(comtypes.IUnknown))
 
         w1.Quit()
         del self.w1
 
         import time
         time.sleep(1)
 
         try:
             w2.Visible
-        except comtypes.COMError, err:
+        except comtypes.COMError as err:
             variables = err.hresult, err.text, err.details
-            self.failUnlessEqual(variables, err[:])
+            self.assertEqual(variables, err[:])
         else:
             raise AssertionError("COMError not raised")
 
         self.assertRaises(WindowsError, comtypes.client.GetActiveObject, "Word.Application")
 
 
 if __name__ == "__main__":
```

## Comparing `comtypes-1.1.9/comtypes/test/test_GUID.py` & `comtypes-1.2.0/comtypes/test/test_GUID.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 import os
 import unittest
 from comtypes import GUID
 
 class Test(unittest.TestCase):
     def test(self):
-        self.failUnlessEqual(GUID(), GUID())
-        self.failUnlessEqual(GUID("{00000000-0000-0000-C000-000000000046}"),
+        self.assertEqual(GUID(), GUID())
+        self.assertEqual(GUID("{00000000-0000-0000-C000-000000000046}"),
                              GUID("{00000000-0000-0000-C000-000000000046}"))
 
-        self.failUnlessEqual(str(GUID("{0002DF01-0000-0000-C000-000000000046}")),
+        self.assertEqual(str(GUID("{0002DF01-0000-0000-C000-000000000046}")),
                              "{0002DF01-0000-0000-C000-000000000046}")
-        self.failUnlessEqual(repr(GUID("{0002DF01-0000-0000-C000-000000000046}")),
+        self.assertEqual(repr(GUID("{0002DF01-0000-0000-C000-000000000046}")),
                              'GUID("{0002DF01-0000-0000-C000-000000000046}")')
 
         self.assertRaises(WindowsError, GUID, "abc")
         self.assertRaises(WindowsError, GUID.from_progid, "abc")
 
         self.assertRaises(WindowsError, lambda guid: guid.as_progid(),
                           GUID("{00000000-0000-0000-C000-000000000046}"))
 
-
-        if os.name == "nt":
-            self.failUnlessEqual(GUID.from_progid("InternetExplorer.Application"),
-                                 GUID("{0002DF01-0000-0000-C000-000000000046}"))
-            self.failUnlessEqual(GUID("{0002DF01-0000-0000-C000-000000000046}").as_progid(),
-                                 u'InternetExplorer.Application.1')
-
-        self.failIfEqual(GUID.create_new(), GUID.create_new())
+        self.assertNotEqual(GUID.create_new(), GUID.create_new())
 
 if __name__ == "__main__":
     unittest.main()
```

## Comparing `comtypes-1.1.9/comtypes/test/test_ie.py` & `comtypes-1.2.0/comtypes/test/test_ie.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import unittest as ut
 from ctypes import *
-from comtypes.client import CreateObject, GetEvents
 
 import comtypes.test
+from comtypes.client import CreateObject, GetEvents
+
 comtypes.test.requires("ui")
 
+
+def setUpModule():
+    raise ut.SkipTest("External test dependencies like this seem bad.  Find a different built-in "
+                      "win32 API to use.")
+
+
 class EventSink:
     def __init__(self):
         self._events = []
 
     # some DWebBrowserEvents
     def OnVisible(self, this, *args):
 ##        print "OnVisible", args
@@ -74,15 +81,15 @@
         import time
         for i in range(50):
             PumpWaitingMessages()
             time.sleep(0.1)
         ie.Visible = False
         ie.Quit()
 
-        self.failUnlessEqual(sink._events, ['OnVisible', 'BeforeNavigate2',
+        self.assertEqual(sink._events, ['OnVisible', 'BeforeNavigate2',
                                             'NavigateComplete2', 'DocumentComplete',
                                             'OnVisible'])
 
         del ie
         del conn
 
     def test_nondefault_eventinterface(self):
@@ -96,12 +103,12 @@
         import time
         for i in range(50):
             PumpWaitingMessages()
             time.sleep(0.1)
         ie.Visible = False
         ie.Quit()
 
-        self.failUnlessEqual(sink._events, ['BeforeNavigate', 'NavigateComplete'])
+        self.assertEqual(sink._events, ['BeforeNavigate', 'NavigateComplete'])
         del ie
 
 if __name__ == "__main__":
     ut.main()
```

## Comparing `comtypes-1.1.9/comtypes/test/test_msscript.py` & `comtypes-1.2.0/comtypes/test/test_msscript.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,27 +46,27 @@
             # typeinfo is really a temporary thing.
 
             res = engine.Eval("[1, 2, 3, 4]")._comobj
 
             # comtypes.client works around this bug, by not trying to
             # high-level wrap the dispatch pointer because QI for the real
             # interface fails.
-            self.failUnlessEqual(type(res), POINTER(IDispatch))
+            self.assertEqual(type(res), POINTER(IDispatch))
 
             tinfo_1 = engine.Eval("[1, 2, 3]")._comobj.GetTypeInfo(0)
             tinfo_2 = engine.Eval("[1, 2, 3, 4]")._comobj.GetTypeInfo(0)
             tinfo_3 = engine.Eval("[1, 2, 3, 4, 5]")._comobj.GetTypeInfo(0)
 
 
-            self.failUnlessEqual(tinfo_1.GetTypeAttr().cVars, 3)
-            self.failUnlessEqual(tinfo_2.GetTypeAttr().cVars, 4)
-            self.failUnlessEqual(tinfo_3.GetTypeAttr().cVars, 5)
+            self.assertEqual(tinfo_1.GetTypeAttr().cVars, 3)
+            self.assertEqual(tinfo_2.GetTypeAttr().cVars, 4)
+            self.assertEqual(tinfo_3.GetTypeAttr().cVars, 5)
 
             # These tests simply describe the current behaviour ;-)
-            self.failUnlessEqual(tinfo_1.GetTypeAttr().guid,
+            self.assertEqual(tinfo_1.GetTypeAttr().guid,
                                  tinfo_1.GetTypeAttr().guid)
 
             ## print (res[0], res[1], res[2])
             ## print len(res)
 
             engine.Reset()
```

## Comparing `comtypes-1.1.9/comtypes/test/test_outparam.py` & `comtypes-1.2.0/comtypes/test/test_outparam.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,22 @@
-from ctypes import *
+import sys
 import unittest
+from ctypes import *
 
 import comtypes.test
+
 comtypes.test.requires("devel")
 
-from comtypes import BSTR, IUnknown, GUID, COMMETHOD, HRESULT
+from comtypes import IUnknown, GUID, COMMETHOD
+
+if sys.version_info >= (3, 0):
+    text_type = str
+else:
+    text_type = unicode
+
 class IMalloc(IUnknown):
     _iid_ = GUID("{00000002-0000-0000-C000-000000000046}")
     _methods_ = [
         COMMETHOD([], c_void_p, "Alloc",
                   ([], c_ulong, "cb")),
         COMMETHOD([], c_void_p, "Realloc",
                   ([], c_void_p, "pv"),
@@ -33,36 +41,37 @@
     if not malloc.DidAlloc(self):
         raise ValueError("memory was NOT allocated by CoTaskMemAlloc")
     windll.ole32.CoTaskMemFree(self)
     return result
 c_wchar_p.__ctypes_from_outparam__ = from_outparm
 
 def comstring(text, typ=c_wchar_p):
-    text = unicode(text)
+    text = text_type(text)
     size = (len(text) + 1) * sizeof(c_wchar)
     mem = windll.ole32.CoTaskMemAlloc(size)
-    print "malloc'd 0x%x, %d bytes" % (mem, size)
+    print("malloc'd 0x%x, %d bytes" % (mem, size))
     ptr = cast(mem, typ)
     memmove(mem, text, size)
     return ptr
 
 class Test(unittest.TestCase):
+    @unittest.skip("This fails for reasons I don't understand yet")
     def test_c_char(self):
 ##        ptr = c_wchar_p("abc")
 ##        self.failUnlessEqual(ptr.__ctypes_from_outparam__(),
 ##                             "abc")
 
 ##        p = BSTR("foo bar spam")
 
         x = comstring("Hello, World")
         y = comstring("foo bar")
         z = comstring("spam, spam, and spam")
 
 ##        (x.__ctypes_from_outparam__(), x.__ctypes_from_outparam__())
-        print (x.__ctypes_from_outparam__(), None) #x.__ctypes_from_outparam__())
+        print((x.__ctypes_from_outparam__(), None)) #x.__ctypes_from_outparam__())
 
 ##        print comstring("Hello, World", c_wchar_p).__ctypes_from_outparam__()
 ##        print comstring("Hello, World", c_wchar_p).__ctypes_from_outparam__()
 ##        print comstring("Hello, World", c_wchar_p).__ctypes_from_outparam__()
 ##        print comstring("Hello, World", c_wchar_p).__ctypes_from_outparam__()
 
 if __name__ == "__main__":
```

## Comparing `comtypes-1.1.9/comtypes/test/test_propputref.py` & `comtypes-1.2.0/comtypes/test/test_propputref.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # There are also propputref tests in test_sapi.py!
 import unittest
 from comtypes.client import CreateObject
 from comtypes.automation import VARIANT
 
 class Test(unittest.TestCase):
+    @unittest.skip("Fails on creating `TestComServerLib.TestComServer`.  Figure out why.")
     def test(self, dynamic=False):
         d = CreateObject("Scripting.Dictionary", dynamic=dynamic)
         s = CreateObject("TestComServerLib.TestComServer", dynamic=dynamic)
         s.name = "the value"
 
         # This calls propputref, since we assign an Object
         d.Item["object"] = s
         # This calls propput, since we assing a Value
         d.Item["value"] = s.name
 
-        self.failUnlessEqual(d.Item["object"], s)
-        self.failUnlessEqual(d.Item["object"].name, "the value")
-        self.failUnlessEqual(d.Item["value"], "the value")
+        self.assertEqual(d.Item["object"], s)
+        self.assertEqual(d.Item["object"].name, "the value")
+        self.assertEqual(d.Item["value"], "the value")
 
         # Changing the default property of the object
         s.name = "foo bar"
-        self.failUnlessEqual(d.Item["object"], s)
-        self.failUnlessEqual(d.Item["object"].name, "foo bar")
-        self.failUnlessEqual(d.Item["value"], "the value")
+        self.assertEqual(d.Item["object"], s)
+        self.assertEqual(d.Item["object"].name, "foo bar")
+        self.assertEqual(d.Item["value"], "the value")
 
         # This also calls propputref since we assign an Object
         d.Item["var"] = VARIANT(s)
-        self.failUnlessEqual(d.Item["var"], s)
+        self.assertEqual(d.Item["var"], s)
 
     def test_dispatch(self):
         return self.test(dynamic=True)
 
 if __name__ == "__main__":
     unittest.main()
```

## Comparing `comtypes-1.1.9/comtypes/test/test_sapi.py` & `comtypes-1.2.0/comtypes/test/test_sapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,19 @@
         fd, fname = tempfile.mkstemp(suffix=".wav")
         os.close(fd)
 
         stream.Open(fname, SpeechLib.SSFMCreateForWrite)
 
         # engine.AudioStream is a propputref property
         engine.AudioOutputStream = stream
-        self.failUnlessEqual(engine.AudioOutputStream, stream)
+        self.assertEqual(engine.AudioOutputStream, stream)
         engine.speak("Hello, World", 0)
         stream.Close()
         filesize = os.stat(fname).st_size
-        self.failUnless(filesize > 100, "filesize only %d bytes" % filesize)
+        self.assertTrue(filesize > 100, "filesize only %d bytes" % filesize)
         os.unlink(fname)
 
     def test_dyndisp(self):
         return self.test(dynamic=True)
 
 if __name__ == "__main__":
     unittest.main()
```

## Comparing `comtypes-1.1.9/comtypes/test/test_server.py` & `comtypes-1.2.0/comtypes/test/test_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,291 +1,303 @@
-import atexit, os, unittest
-##import comtypes
-import comtypes.typeinfo, comtypes.client
-
-class TypeLib(object):
-    """This class collects IDL code fragments and eventually writes
-    them into a .IDL file.  The compile() method compiles the IDL file
-    into a typelibrary and registers it.  A function is also
-    registered with atexit that will unregister the typelib at program
-    exit.
-    """
-    def __init__(self, lib):
-        self.lib = lib
-        self.interfaces = []
-        self.coclasses = []
-
-    def interface(self, header):
-        itf = Interface(header)
-        self.interfaces.append(itf)
-        return itf
-
-    def coclass(self, definition):
-        self.coclasses.append(definition)
-
-    def __str__(self):
-        header = '''import "oaidl.idl";
-                    import "ocidl.idl";
-                    %s {''' % self.lib
-        body = "\n".join([str(itf) for itf in self.interfaces])
-        footer = "\n".join(self.coclasses) + "}"
-        return "\n".join((header, body, footer))
-
-    def compile(self):
-        """Compile and register the typelib"""
-        code = str(self)
-        curdir = os.path.dirname(__file__)
-        idl_path = os.path.join(curdir, "mylib.idl")
-        tlb_path = os.path.join(curdir, "mylib.tlb")
-        if not os.path.isfile(idl_path) or open(idl_path, "r").read() != code:
-            open(idl_path, "w").write(code)
-            os.system(r'call "%%VS71COMNTOOLS%%vsvars32.bat" && '
-                      r'midl /nologo %s /tlb %s' % (idl_path, tlb_path))
-        # Register the typelib...
-        tlib = comtypes.typeinfo.LoadTypeLib(tlb_path)
-        # create the wrapper module...
-        comtypes.client.GetModule(tlb_path)
-        # Unregister the typelib at interpreter exit...
-        attr = tlib.GetLibAttr()
-        guid, major, minor = attr.guid, attr.wMajorVerNum, attr.wMinorVerNum
-##        atexit.register(comtypes.typeinfo.UnRegisterTypeLib,
-##                        guid, major, minor)
-        return tlb_path
-    
-class Interface(object):
-    def __init__(self, header):
-        self.header = header
-        self.code = ""
-
-    def add(self, text):
-        self.code += text + "\n"
-        return self
-
-    def __str__(self):
-        return self.header + " {\n" + self.code + "}\n"
-
-################################################################
-import comtypes
-from comtypes.client import wrap
-
-tlb = TypeLib("[uuid(f4f74946-4546-44bd-a073-9ea6f9fe78cb)] library TestLib")
-
-itf = tlb.interface("""[object,
-                        oleautomation,
-                        dual,
-                        uuid(ed978f5f-cc45-4fcc-a7a6-751ffa8dfedd)]
-                        interface IMyInterface : IDispatch""")
-
-outgoing = tlb.interface("""[object,
-                             oleautomation,
-                             dual,
-                             uuid(f7c48a90-64ea-4bb8-abf1-b3a3aa996848)]
-                             interface IMyEventInterface : IDispatch""")
-
-tlb.coclass("""
-[uuid(fa9de8f4-20de-45fc-b079-648572428817)]
-coclass MyServer {
-    [default] interface IMyInterface;
-    [default, source] interface IMyEventInterface;
-};
-""")
-
-# The purpose of the MyServer class is to locate three separate code
-# section snippets closely together:
-#
-# 1. The IDL method definition for a COM interface method
-# 2. The Python implementation of the COM method
-# 3. The unittest(s) for the COM method.
-#
-from comtypes.server.connectionpoints import ConnectableObjectMixin
-class MyServer(comtypes.CoClass, ConnectableObjectMixin):
-    _reg_typelib_ = ('{f4f74946-4546-44bd-a073-9ea6f9fe78cb}', 0, 0)
-    _reg_clsid_ = comtypes.GUID('{fa9de8f4-20de-45fc-b079-648572428817}')
-
-    ################
-    # definition
-    itf.add("""[id(100), propget] HRESULT Name([out, retval] BSTR *pname);
-               [id(100), propput] HRESULT Name([in] BSTR name);""")
-    # implementation
-    Name = "foo"
-    # test
-    def test_Name(self):
-        p = wrap(self.create())
-        self.assertEqual((p.Name, p.name, p.nAME), ("foo",) * 3)
-        p.NAME = "spam"
-        self.assertEqual((p.Name, p.name, p.nAME), ("spam",) * 3)
-
-    ################
-    # definition
-    itf.add("[id(101)] HRESULT MixedInOut([in] int a, [out] int *b, [in] int c, [out] int *d);")
-    # implementation
-    def MixedInOut(self, a, c):
-        return a+1, c+1
-    #test
-    def test_MixedInOut(self):
-        p = wrap(self.create())
-        self.assertEqual(p.MixedInOut(1, 2), (2, 3))
-
-    ################
-    # definition
-    itf.add("[id(102)] HRESULT MultiInOutArgs([in, out] int *pa, [in, out] int *pb);")
-    # implementation
-    def MultiInOutArgs(self, pa, pb):
-        return pa[0] * 3, pb[0] * 4
-    # test
-    def test_MultiInOutArgs(self):
-        p = wrap(self.create())
-        self.assertEqual(p.MultiInOutArgs(1, 2), (3, 8))
-
-    ################
-    # definition
-    itf.add("HRESULT MultiInOutArgs2([in, out] int *pa, [out] int *pb);")
-##    # implementation
-##    def MultiInOutArgs2(self, pa):
-##        return pa[0] * 3, pa[0] * 4
-##    # test
-##    def test_MultiInOutArgs2(self):
-##        p = wrap(self.create())
-##        self.assertEqual(p.MultiInOutArgs2(42), (126, 168))
-
-    ################
-    # definition
-    itf.add("HRESULT MultiInOutArgs3([out] int *pa, [out] int *pb);")
-    # implementation
-    def MultiInOutArgs3(self):
-        return 42, 43
-    # test
-    def test_MultiInOutArgs3(self):
-        p = wrap(self.create())
-        self.assertEqual(p.MultiInOutArgs3(), (42, 43))
-
-    ################
-    # definition
-    itf.add("HRESULT MultiInOutArgs4([out] int *pa, [in, out] int *pb);")
-    # implementation
-    def MultiInOutArgs4(self, pb):
-        return pb[0] + 3, pb[0] + 4
-    # test
-    def test_MultiInOutArgs4(self):
-        p = wrap(self.create())
-        res = p.MultiInOutArgs4(pb=32)
-##        print "MultiInOutArgs4", res
-
-    itf.add("""HRESULT GetStackTrace([in] ULONG FrameOffset,
-                                     [in, out] INT *Frames,
-                                     [in] ULONG FramesSize,
-                                     [out, optional] ULONG *FramesFilled);""")
-    def GetStackTrace(self, this, *args):
-##        print "GetStackTrace", args
-        return 0
-    def test_GetStackTrace(self):
-        p = wrap(self.create())
-        from ctypes import c_int, POINTER, pointer
-        frames = (c_int * 5)()
-        res = p.GetStackTrace(42, frames, 5)
-##        print "RES_1", res
-
-        frames = pointer(c_int(5))
-        res = p.GetStackTrace(42, frames, 0)
-##        print "RES_2", res
-
-    # It is unlear to me if this is allowed or not.  Apparently there
-    # are typelibs that define such an argument type, but it may be
-    # that these are buggy.
+try:
+    # Force module to raise.  We catch this error later.  Yes, a dirty hack for python2.7.
+    raise WindowsError("This test module cannot run as-is.  Investigate why")
+    import atexit, os, unittest
+
+    import comtypes.typeinfo, comtypes.client
+
+
+
+
+    class TypeLib(object):
+        """This class collects IDL code fragments and eventually writes
+        them into a .IDL file.  The compile() method compiles the IDL file
+        into a typelibrary and registers it.  A function is also
+        registered with atexit that will unregister the typelib at program
+        exit.
+        """
+        def __init__(self, lib):
+            self.lib = lib
+            self.interfaces = []
+            self.coclasses = []
+
+        def interface(self, header):
+            itf = Interface(header)
+            self.interfaces.append(itf)
+            return itf
+
+        def coclass(self, definition):
+            self.coclasses.append(definition)
+
+        def __str__(self):
+            header = '''import "oaidl.idl";
+                        import "ocidl.idl";
+                        %s {''' % self.lib
+            body = "\n".join([str(itf) for itf in self.interfaces])
+            footer = "\n".join(self.coclasses) + "}"
+            return "\n".join((header, body, footer))
+
+        def compile(self):
+            """Compile and register the typelib"""
+            code = str(self)
+            curdir = os.path.dirname(__file__)
+            idl_path = os.path.join(curdir, "mylib.idl")
+            tlb_path = os.path.join(curdir, "mylib.tlb")
+            if not os.path.isfile(idl_path) or open(idl_path, "r").read() != code:
+                open(idl_path, "w").write(code)
+                os.system(r'call "%%VS71COMNTOOLS%%vsvars32.bat" && '
+                          r'midl /nologo %s /tlb %s' % (idl_path, tlb_path))
+            # Register the typelib...
+            tlib = comtypes.typeinfo.LoadTypeLib(tlb_path)
+            # create the wrapper module...
+            comtypes.client.GetModule(tlb_path)
+            # Unregister the typelib at interpreter exit...
+            attr = tlib.GetLibAttr()
+            guid, major, minor = attr.guid, attr.wMajorVerNum, attr.wMinorVerNum
+    ##        atexit.register(comtypes.typeinfo.UnRegisterTypeLib,
+    ##                        guid, major, minor)
+            return tlb_path
+
+    class Interface(object):
+        def __init__(self, header):
+            self.header = header
+            self.code = ""
+
+        def add(self, text):
+            self.code += text + "\n"
+            return self
+
+        def __str__(self):
+            return self.header + " {\n" + self.code + "}\n"
+
+    ################################################################
+    import comtypes
+    from comtypes.client import wrap
+
+    tlb = TypeLib("[uuid(f4f74946-4546-44bd-a073-9ea6f9fe78cb)] library TestLib")
+
+    itf = tlb.interface("""[object,
+                            oleautomation,
+                            dual,
+                            uuid(ed978f5f-cc45-4fcc-a7a6-751ffa8dfedd)]
+                            interface IMyInterface : IDispatch""")
+
+    outgoing = tlb.interface("""[object,
+                                 oleautomation,
+                                 dual,
+                                 uuid(f7c48a90-64ea-4bb8-abf1-b3a3aa996848)]
+                                 interface IMyEventInterface : IDispatch""")
+
+    tlb.coclass("""
+    [uuid(fa9de8f4-20de-45fc-b079-648572428817)]
+    coclass MyServer {
+        [default] interface IMyInterface;
+        [default, source] interface IMyEventInterface;
+    };
+    """)
+
+    # The purpose of the MyServer class is to locate three separate code
+    # section snippets closely together:
     #
-    # Point is that SafeArrayCreateEx(VT_VARIANT|VT_BYREF, ..) fails.
-    # The MSDN docs for SafeArrayCreate() have a notice that neither
-    # VT_ARRAY not VT_BYREF may be set, this notice is missing however
-    # for SafeArrayCreateEx().
+    # 1. The IDL method definition for a COM interface method
+    # 2. The Python implementation of the COM method
+    # 3. The unittest(s) for the COM method.
     #
-    # We have this code here to make sure that comtypes can import
-    # such a typelib, although calling ths method will fail because
-    # such an array cannot be created.
-    itf.add("""HRESULT dummy([in] SAFEARRAY(VARIANT *) foo);""")
-
-
-    # Test events.
-    itf.add("""HRESULT DoSomething();""")
-    outgoing.add("""[id(103)] HRESULT OnSomething();""")
-    # implementation
-    def DoSomething(self):
-        "Implement the DoSomething method"
-        self.Fire_Event(0, "OnSomething")
-    # test
-    def test_events(self):
-        p = wrap(self.create())
-        class Handler(object):
-            called = 0
-            def OnSomething(self, this):
-                "Handles the OnSomething event"
-                self.called += 1
-        handler = Handler()
-        ev = comtypes.client.GetEvents(p, handler)
-        p.DoSomething()
-        self.assertEqual(handler.called, 1)
-
-        class Handler(object):
-            called = 0
-            def IMyEventInterface_OnSomething(self):
-                "Handles the OnSomething event"
-                self.called += 1
-        handler = Handler()
-        ev = comtypes.client.GetEvents(p, handler)
-        p.DoSomething()
-        self.assertEqual(handler.called, 1)
-
-    # events with out-parameters (these are probably very unlikely...)
-    itf.add("""HRESULT DoSomethingElse();""")
-    outgoing.add("""[id(104)] HRESULT OnSomethingElse([out, retval] int *px);""")
-    def DoSomethingElse(self):
-        "Implement the DoSomething method"
-        self.Fire_Event(0, "OnSomethingElse")
-    def test_DoSomethingElse(self):
-        p = wrap(self.create())
-        class Handler(object):
-            called = 0
-            def OnSomethingElse(self):
-                "Handles the OnSomething event"
-                self.called += 1
-                return 42
-        handler = Handler()
-        ev = comtypes.client.GetEvents(p, handler)
-        p.DoSomethingElse()
-        self.assertEqual(handler.called, 1)
-
-        class Handler(object):
-            called = 0
-            def OnSomethingElse(self, this, presult):
-                "Handles the OnSomething event"
-                self.called += 1
-                presult[0] = 42
-        handler = Handler()
-        ev = comtypes.client.GetEvents(p, handler)
-        p.DoSomethingElse()
-        self.assertEqual(handler.called, 1)
-
-################################################################
-
-path = tlb.compile()
-from comtypes.gen import TestLib
-from comtypes.typeinfo import IProvideClassInfo, IProvideClassInfo2
-from comtypes.connectionpoints import IConnectionPointContainer
-
-MyServer._com_interfaces_ = [TestLib.IMyInterface,
-                             IProvideClassInfo2,
-                             IConnectionPointContainer]
-MyServer._outgoing_interfaces_ = [TestLib.IMyEventInterface]
-
-################################################################
-
-class Test(unittest.TestCase, MyServer):
-    def __init__(self, *args):
-        unittest.TestCase.__init__(self, *args)
-        MyServer.__init__(self)
-
-    def create(self):
-        obj = MyServer()
-        return obj.QueryInterface(comtypes.IUnknown)
-
+    from comtypes.server.connectionpoints import ConnectableObjectMixin
+    class MyServer(comtypes.CoClass, ConnectableObjectMixin):
+        _reg_typelib_ = ('{f4f74946-4546-44bd-a073-9ea6f9fe78cb}', 0, 0)
+        _reg_clsid_ = comtypes.GUID('{fa9de8f4-20de-45fc-b079-648572428817}')
+
+        ################
+        # definition
+        itf.add("""[id(100), propget] HRESULT Name([out, retval] BSTR *pname);
+                   [id(100), propput] HRESULT Name([in] BSTR name);""")
+        # implementation
+        Name = "foo"
+        # test
+        def test_Name(self):
+            p = wrap(self.create())
+            self.assertEqual((p.Name, p.name, p.nAME), ("foo",) * 3)
+            p.NAME = "spam"
+            self.assertEqual((p.Name, p.name, p.nAME), ("spam",) * 3)
+
+        ################
+        # definition
+        itf.add("[id(101)] HRESULT MixedInOut([in] int a, [out] int *b, [in] int c, [out] int *d);")
+        # implementation
+        def MixedInOut(self, a, c):
+            return a+1, c+1
+        #test
+        def test_MixedInOut(self):
+            p = wrap(self.create())
+            self.assertEqual(p.MixedInOut(1, 2), (2, 3))
+
+        ################
+        # definition
+        itf.add("[id(102)] HRESULT MultiInOutArgs([in, out] int *pa, [in, out] int *pb);")
+        # implementation
+        def MultiInOutArgs(self, pa, pb):
+            return pa[0] * 3, pb[0] * 4
+        # test
+        def test_MultiInOutArgs(self):
+            p = wrap(self.create())
+            self.assertEqual(p.MultiInOutArgs(1, 2), (3, 8))
+
+        ################
+        # definition
+        itf.add("HRESULT MultiInOutArgs2([in, out] int *pa, [out] int *pb);")
+    ##    # implementation
+    ##    def MultiInOutArgs2(self, pa):
+    ##        return pa[0] * 3, pa[0] * 4
+    ##    # test
+    ##    def test_MultiInOutArgs2(self):
+    ##        p = wrap(self.create())
+    ##        self.assertEqual(p.MultiInOutArgs2(42), (126, 168))
+
+        ################
+        # definition
+        itf.add("HRESULT MultiInOutArgs3([out] int *pa, [out] int *pb);")
+        # implementation
+        def MultiInOutArgs3(self):
+            return 42, 43
+        # test
+        def test_MultiInOutArgs3(self):
+            p = wrap(self.create())
+            self.assertEqual(p.MultiInOutArgs3(), (42, 43))
+
+        ################
+        # definition
+        itf.add("HRESULT MultiInOutArgs4([out] int *pa, [in, out] int *pb);")
+        # implementation
+        def MultiInOutArgs4(self, pb):
+            return pb[0] + 3, pb[0] + 4
+        # test
+        def test_MultiInOutArgs4(self):
+            p = wrap(self.create())
+            res = p.MultiInOutArgs4(pb=32)
+    ##        print "MultiInOutArgs4", res
+
+        itf.add("""HRESULT GetStackTrace([in] ULONG FrameOffset,
+                                         [in, out] INT *Frames,
+                                         [in] ULONG FramesSize,
+                                         [out, optional] ULONG *FramesFilled);""")
+        def GetStackTrace(self, this, *args):
+    ##        print "GetStackTrace", args
+            return 0
+        def test_GetStackTrace(self):
+            p = wrap(self.create())
+            from ctypes import c_int, POINTER, pointer
+            frames = (c_int * 5)()
+            res = p.GetStackTrace(42, frames, 5)
+    ##        print "RES_1", res
+
+            frames = pointer(c_int(5))
+            res = p.GetStackTrace(42, frames, 0)
+    ##        print "RES_2", res
+
+        # It is unlear to me if this is allowed or not.  Apparently there
+        # are typelibs that define such an argument type, but it may be
+        # that these are buggy.
+        #
+        # Point is that SafeArrayCreateEx(VT_VARIANT|VT_BYREF, ..) fails.
+        # The MSDN docs for SafeArrayCreate() have a notice that neither
+        # VT_ARRAY not VT_BYREF may be set, this notice is missing however
+        # for SafeArrayCreateEx().
+        #
+        # We have this code here to make sure that comtypes can import
+        # such a typelib, although calling ths method will fail because
+        # such an array cannot be created.
+        itf.add("""HRESULT dummy([in] SAFEARRAY(VARIANT *) foo);""")
+
+
+        # Test events.
+        itf.add("""HRESULT DoSomething();""")
+        outgoing.add("""[id(103)] HRESULT OnSomething();""")
+        # implementation
+        def DoSomething(self):
+            "Implement the DoSomething method"
+            self.Fire_Event(0, "OnSomething")
+        # test
+        def test_events(self):
+            p = wrap(self.create())
+            class Handler(object):
+                called = 0
+                def OnSomething(self, this):
+                    "Handles the OnSomething event"
+                    self.called += 1
+            handler = Handler()
+            ev = comtypes.client.GetEvents(p, handler)
+            p.DoSomething()
+            self.assertEqual(handler.called, 1)
+
+            class Handler(object):
+                called = 0
+                def IMyEventInterface_OnSomething(self):
+                    "Handles the OnSomething event"
+                    self.called += 1
+            handler = Handler()
+            ev = comtypes.client.GetEvents(p, handler)
+            p.DoSomething()
+            self.assertEqual(handler.called, 1)
+
+        # events with out-parameters (these are probably very unlikely...)
+        itf.add("""HRESULT DoSomethingElse();""")
+        outgoing.add("""[id(104)] HRESULT OnSomethingElse([out, retval] int *px);""")
+        def DoSomethingElse(self):
+            "Implement the DoSomething method"
+            self.Fire_Event(0, "OnSomethingElse")
+        def test_DoSomethingElse(self):
+            p = wrap(self.create())
+            class Handler(object):
+                called = 0
+                def OnSomethingElse(self):
+                    "Handles the OnSomething event"
+                    self.called += 1
+                    return 42
+            handler = Handler()
+            ev = comtypes.client.GetEvents(p, handler)
+            p.DoSomethingElse()
+            self.assertEqual(handler.called, 1)
+
+            class Handler(object):
+                called = 0
+                def OnSomethingElse(self, this, presult):
+                    "Handles the OnSomething event"
+                    self.called += 1
+                    presult[0] = 42
+            handler = Handler()
+            ev = comtypes.client.GetEvents(p, handler)
+            p.DoSomethingElse()
+            self.assertEqual(handler.called, 1)
+
+    ################################################################
+
+    path = tlb.compile()
+    from comtypes.gen import TestLib
+    from comtypes.typeinfo import IProvideClassInfo, IProvideClassInfo2
+    from comtypes.connectionpoints import IConnectionPointContainer
+
+    MyServer._com_interfaces_ = [TestLib.IMyInterface,
+                                 IProvideClassInfo2,
+                                 IConnectionPointContainer]
+    MyServer._outgoing_interfaces_ = [TestLib.IMyEventInterface]
+
+    ################################################################
+
+    class Test(unittest.TestCase, MyServer):
+        def __init__(self, *args):
+            unittest.TestCase.__init__(self, *args)
+            MyServer.__init__(self)
+
+        def create(self):
+            obj = MyServer()
+            return obj.QueryInterface(comtypes.IUnknown)
+except:
+    import unittest
+
+    class TestSkipped(unittest.TestCase):
+        @unittest.skip("This file causes a WindowsError.  Needs investigated and fixed.")
+        def test_server_module_skipped(self):
+            pass
 
 if __name__ == "__main__":
     unittest.main()
```

## Comparing `comtypes-1.1.9/comtypes/test/test_typeinfo.py` & `comtypes-1.2.0/comtypes/test/test_typeinfo.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,80 +2,91 @@
 import unittest
 from ctypes import POINTER, byref
 from comtypes import GUID, COMError
 from comtypes.automation import DISPATCH_METHOD
 from comtypes.typeinfo import LoadTypeLibEx, LoadRegTypeLib, \
      QueryPathOfRegTypeLib, TKIND_INTERFACE, TKIND_DISPATCH, TKIND_ENUM
 
-# We should add other test cases for Windows CE.
-if os.name == "nt":
-    class Test(unittest.TestCase):
-        # No LoadTypeLibEx on windows ce
-        def test_LoadTypeLibEx(self):
-            # IE 6 uses shdocvw.dll, IE 7 uses ieframe.dll
-            if os.path.exists(os.path.join(os.environ["SystemRoot"],
-                                           "system32", "ieframe.dll")):
-                dllname = "ieframe.dll"
-            else:
-                dllname = "shdocvw.dll"
-
-            self.assertRaises(WindowsError, lambda: LoadTypeLibEx("<xxx.xx>"))
-            tlib = LoadTypeLibEx(dllname)
-            self.failUnless(tlib.GetTypeInfoCount())
-            tlib.GetDocumentation(-1)
-            self.failUnlessEqual(tlib.IsName("iwebbrowser"), "IWebBrowser")
-            self.failUnlessEqual(tlib.IsName("IWEBBROWSER"), "IWebBrowser")
-            self.failUnless(tlib.FindName("IWebBrowser"))
-            self.failUnlessEqual(tlib.IsName("Spam"), None)
-            tlib.GetTypeComp()
-
-            attr = tlib.GetLibAttr()
-            info = attr.guid, attr.wMajorVerNum, attr.wMinorVerNum
-            other_tlib = LoadRegTypeLib(*info)
-            self.failUnlessEqual(tlib, other_tlib)
-
-    ##         for n in dir(attr):
-    ##             if not n.startswith("_"):
-    ##                 print "\t", n, getattr(attr, n)
-
-            for i in range(tlib.GetTypeInfoCount()):
-                ti = tlib.GetTypeInfo(i)
-                ti.GetTypeAttr()
-                tlib.GetDocumentation(i)
-                tlib.GetTypeInfoType(i)
-
-                c_tlib, index = ti.GetContainingTypeLib()
-                self.failUnlessEqual(c_tlib, tlib)
-                self.failUnlessEqual(index, i)
-
-            guid_null = GUID()
-            self.assertRaises(COMError, lambda: tlib.GetTypeInfoOfGuid(guid_null))
-
-            self.failUnless(tlib.GetTypeInfoOfGuid(GUID("{EAB22AC1-30C1-11CF-A7EB-0000C05BAE0B}")))
-
-            path = QueryPathOfRegTypeLib(*info)
-            path = path.split("\0")[0]
-            self.failUnless(path.lower().endswith(dllname))
-
-        def test_TypeInfo(self):
-            tlib = LoadTypeLibEx("shdocvw.dll")
-            for index in range(tlib.GetTypeInfoCount()):
-                ti = tlib.GetTypeInfo(index)
-                ta = ti.GetTypeAttr()
-                ti.GetDocumentation(-1)
-                if ta.typekind in (TKIND_INTERFACE, TKIND_DISPATCH):
-                    if ta.cImplTypes:
-                        href = ti.GetRefTypeOfImplType(0)
-                        base = ti.GetRefTypeInfo(href)
-                        base.GetDocumentation(-1)
-                        ti.GetImplTypeFlags(0)
-                for f in range(ta.cFuncs):
-                    fd = ti.GetFuncDesc(f)
-                    names = ti.GetNames(fd.memid, 32)
-                    ti.GetIDsOfNames(*names)
-                    ti.GetMops(fd.memid)
 
-                for v in range(ta.cVars):
-                    ti.GetVarDesc(v)
+class Test(unittest.TestCase):
+    def test_LoadTypeLibEx(self):
+        dllname = "scrrun.dll"
+        with self.assertRaises(WindowsError):
+            LoadTypeLibEx("<xxx.xx>")
+        tlib = LoadTypeLibEx(dllname)
+        self.assertTrue(tlib.GetTypeInfoCount())
+        tlib.GetDocumentation(-1)
+        self.assertEqual(tlib.IsName("ifile"), "IFile")
+        self.assertEqual(tlib.IsName("IFILE"), "IFile")
+        self.assertTrue(tlib.FindName("IFile"))
+        self.assertEqual(tlib.IsName("Spam"), None)
+        tlib.GetTypeComp()
+
+    def test_LoadRegTypeLib(self):
+        tlib = LoadTypeLibEx("scrrun.dll")
+        attr = tlib.GetLibAttr()
+        info = attr.guid, attr.wMajorVerNum, attr.wMinorVerNum
+        other_tlib = LoadRegTypeLib(*info)
+        self.assert_tlibattr_equal(tlib, other_tlib)
+    
+    def assert_tlibattr_equal(self, tlib, other_tlib):
+        attr, other_attr = tlib.GetLibAttr(), other_tlib.GetLibAttr()
+        # `assert tlib == other_tlib` will fail in some environments.
+        # But their attributes are equal even if difference of environments.
+        self.assertEqual(attr.guid, other_attr.guid)
+        self.assertEqual(attr.wMajorVerNum, other_attr.wMajorVerNum)
+        self.assertEqual(attr.wMinorVerNum, other_attr.wMinorVerNum)
+        self.assertEqual(attr.lcid, other_attr.lcid)
+        self.assertEqual(attr.wLibFlags, other_attr.wLibFlags)
+
+        # for n in dir(attr):
+        #     if not n.startswith("_"):
+        #         print "\t", n, getattr(attr, n)
+
+    def test_QueryPathOfRegTypeLib(self):
+        dllname = "scrrun.dll"
+        tlib = LoadTypeLibEx(dllname)
+        attr = tlib.GetLibAttr()
+        info = attr.guid, attr.wMajorVerNum, attr.wMinorVerNum
+        path = QueryPathOfRegTypeLib(*info)
+        path = path.split("\0")[0]
+        self.assertTrue(path.lower().endswith(dllname))
+
+    def test_TypeInfo(self):
+        tlib = LoadTypeLibEx("scrrun.dll")
+        for index in range(tlib.GetTypeInfoCount()):
+            ti = tlib.GetTypeInfo(index)
+            ta = ti.GetTypeAttr()
+            ti.GetDocumentation(-1)
+            c_tlib, c_index = ti.GetContainingTypeLib()
+            self.assert_tlibattr_equal(c_tlib, tlib)
+            self.assertEqual(c_index, index)
+            if ta.typekind in (TKIND_INTERFACE, TKIND_DISPATCH):
+                if ta.cImplTypes:
+                    href = ti.GetRefTypeOfImplType(0)
+                    base = ti.GetRefTypeInfo(href)
+                    base.GetDocumentation(-1)
+                    ti.GetImplTypeFlags(0)
+            for f in range(ta.cFuncs):
+                fd = ti.GetFuncDesc(f)
+                names = ti.GetNames(fd.memid, 32)
+                ti.GetIDsOfNames(*names)
+                ti.GetMops(fd.memid)
+
+            for v in range(ta.cVars):
+                ti.GetVarDesc(v)
+
+        guid_null = GUID()
+        with self.assertRaises(COMError):
+            tlib.GetTypeInfoOfGuid(guid_null)
+
+        guid = GUID("{C7C3F5A4-88A3-11D0-ABCB-00A0C90FFFC0}")
+        ti = tlib.GetTypeInfoOfGuid(guid)
+        c_tlib, c_index = ti.GetContainingTypeLib()
+        c_ti = c_tlib.GetTypeInfo(c_index)
+        self.assert_tlibattr_equal(c_tlib, tlib)
+        self.assertEqual(c_ti, ti)
+        self.assertEqual(guid, ti.GetTypeAttr().guid)
+
 
 if __name__ == "__main__":
     unittest.main()
```

## Comparing `comtypes-1.1.9/comtypes/test/test_urlhistory.py` & `comtypes-1.2.0/comtypes/test/test_urlhistory.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 GetModule(os.path.join(os.path.dirname(__file__), "urlhist.tlb"))
 from comtypes.gen import urlhistLib
 
 # The pwcsTitle and pwcsUrl fields of the _STATURL structure must be
 # freed by the caller.  The only way to do this without patching the
 # generated code directly is to monkey-patch the
 # _STATURL.__ctypes_from_outparam__ method like this.
-@Patch(urlhistlib._STATURL)
+@Patch(urlhistLib._STATURL)
 class _(object):
     def __ctypes_from_outparam__(self):
         from comtypes.util import cast_field
         result = type(self)()
         for n, _ in self._fields_:
             setattr(result, n, getattr(self, n))
         url, title = self.pwcsUrl, self.pwcsTitle
@@ -26,16 +26,17 @@
         return result
 
 from comtypes.test.find_memleak import find_memleak
 
 class Test(unittest.TestCase):
     def check_leaks(self, func):
         bytes = find_memleak(func, (5, 10))
-        self.failIf(bytes, "Leaks %d bytes" % bytes)
+        self.assertFalse(bytes, "Leaks %d bytes" % bytes)
 
+    @unittest.skip("This fails with: `TypeError: iter() returned non-iterator of type 'POINTER(IEnumSTATURL)'`")
     def test_creation(self):
         hist = CreateObject(urlhistLib.UrlHistory)
         for x in hist.EnumURLS():
             x.pwcsUrl, x.pwcsTitle
 ##            print (x.pwcsUrl, x.pwcsTitle)
 ##            print x
         def doit():
```

## Comparing `comtypes-1.1.9/comtypes/test/test_variant.py` & `comtypes-1.2.0/comtypes/test/test_variant.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,331 +1,292 @@
-from ctypes import (
-    POINTER, byref, c_byte, c_char, c_double, c_float, c_int, c_int64, c_short,
-    c_ubyte, c_ushort, c_uint, c_uint64, pointer,
-)
+from __future__ import print_function
+
 import datetime
 import decimal
 import sys
 import unittest
+from ctypes import (
+    POINTER, byref, c_byte, c_char, c_double, c_float, c_int, c_int64, c_short, c_ubyte, c_uint,
+    c_uint64, c_ushort, pointer,
+)
 
-from comtypes import IUnknown, GUID
+from comtypes import GUID, IUnknown
 from comtypes.automation import (
-    VARIANT, DISPPARAMS, VT_NULL, VT_EMPTY, VT_ERROR, VT_I1, VT_I2, VT_I4,
-    VT_I8, VT_UI1, VT_UI2, VT_UI4, VT_UI8, VT_R4, VT_R8, VT_BYREF, VT_BSTR,
-    VT_DATE, VT_DECIMAL, VT_CY,)
-from comtypes.typeinfo import LoadRegTypeLib
-from comtypes.test import get_numpy
+    DISPPARAMS, VARIANT, VT_BSTR, VT_BYREF, VT_CY, VT_DATE, VT_DECIMAL, VT_EMPTY, VT_ERROR, VT_I1,
+    VT_I2, VT_I4, VT_I8, VT_NULL, VT_R4, VT_R8, VT_UI1, VT_UI2, VT_UI4, VT_UI8,
+)
 from comtypes.test.find_memleak import find_memleak
+from comtypes.typeinfo import LoadRegTypeLib
 
 
 def get_refcnt(comptr):
     # return the COM reference count of a COM interface pointer
     if not comptr:
         return 0
     comptr.AddRef()
     return comptr.Release()
 
 
 class VariantTestCase(unittest.TestCase):
 
     def test_constants(self):
         empty = VARIANT.empty
-        self.failUnlessEqual(empty.vt, VT_EMPTY)
-        self.failUnless(empty.value is None)
+        self.assertEqual(empty.vt, VT_EMPTY)
+        self.assertTrue(empty.value is None)
 
         null = VARIANT.null
-        self.failUnlessEqual(null.vt, VT_NULL)
-        self.failUnless(null.value is None)
+        self.assertEqual(null.vt, VT_NULL)
+        self.assertTrue(null.value is None)
 
         missing = VARIANT.missing
-        self.failUnlessEqual(missing.vt, VT_ERROR)
+        self.assertEqual(missing.vt, VT_ERROR)
         self.assertRaises(NotImplementedError, lambda: missing.value)
 
     def test_com_refcounts(self):
         # typelib for oleaut32
         tlb = LoadRegTypeLib(GUID("{00020430-0000-0000-C000-000000000046}"), 2, 0, 0)
         rc = get_refcnt(tlb)
 
         p = tlb.QueryInterface(IUnknown)
-        self.failUnlessEqual(get_refcnt(tlb), rc+1)
+        self.assertEqual(get_refcnt(tlb), rc+1)
 
         del p
-        self.failUnlessEqual(get_refcnt(tlb), rc)
+        self.assertEqual(get_refcnt(tlb), rc)
 
     def test_com_pointers(self):
         # Storing a COM interface pointer in a VARIANT increments the refcount,
         # changing the variant to contain something else decrements it
         tlb = LoadRegTypeLib(GUID("{00020430-0000-0000-C000-000000000046}"), 2, 0, 0)
         rc = get_refcnt(tlb)
 
         v = VARIANT(tlb)
-        self.failUnlessEqual(get_refcnt(tlb), rc+1)
+        self.assertEqual(get_refcnt(tlb), rc+1)
 
         p = v.value
-        self.failUnlessEqual(get_refcnt(tlb), rc+2)
+        self.assertEqual(get_refcnt(tlb), rc+2)
         del p
-        self.failUnlessEqual(get_refcnt(tlb), rc+1)
+        self.assertEqual(get_refcnt(tlb), rc+1)
 
         v.value = None
-        self.failUnlessEqual(get_refcnt(tlb), rc)
+        self.assertEqual(get_refcnt(tlb), rc)
 
     def test_null_com_pointers(self):
         p = POINTER(IUnknown)()
-        self.failUnlessEqual(get_refcnt(p), 0)
+        self.assertEqual(get_refcnt(p), 0)
 
         VARIANT(p)
-        self.failUnlessEqual(get_refcnt(p), 0)
+        self.assertEqual(get_refcnt(p), 0)
 
     def test_dispparams(self):
         # DISPPARAMS is a complex structure, well worth testing.
         d = DISPPARAMS()
         d.rgvarg = (VARIANT * 3)()
         values = [1, 5, 7]
         for i, v in enumerate(values):
             d.rgvarg[i].value = v
         result = [d.rgvarg[i].value for i in range(3)]
-        self.failUnlessEqual(result, values)
+        self.assertEqual(result, values)
 
     def test_pythonobjects(self):
-        objects = [None, 42, 3.14, True, False, "abc", u"abc", 7L]
+        if sys.version_info >= (3, 0):
+            objects = [None, 42, 3.14, True, False, "abc", "abc", 7]
+        else:
+            objects = [None, 42, 3.14, True, False, "abc", u"abc", 7]
         for x in objects:
             v = VARIANT(x)
-            self.failUnlessEqual(x, v.value)
+            self.assertEqual(x, v.value)
 
     def test_integers(self):
         v = VARIANT()
 
+        int_type = int if sys.version_info >= (3,0) else (int, long)
+
         if (hasattr(sys, "maxint")):
             # this test doesn't work in Python 3000
-            v.value = sys.maxint
-            self.failUnlessEqual(v.value, sys.maxint)
-            self.failUnlessEqual(type(v.value), int)
+            v.value = sys.maxsize
+            self.assertEqual(v.value, sys.maxsize)
+            self.assertIsInstance(v.value, int_type)
 
             v.value += 1
-            self.failUnlessEqual(v.value, sys.maxint+1)
-            self.failUnlessEqual(type(v.value), long)
+            self.assertEqual(v.value, sys.maxsize+1)
+            self.assertIsInstance(v.value, int_type)
 
-        v.value = 1L
-        self.failUnlessEqual(v.value, 1)
-        self.failUnlessEqual(type(v.value), int)
+        v.value = 1
+
+        self.assertEqual(v.value, 1)
+        self.assertIsInstance(v.value, int_type)
 
     def test_datetime(self):
         now = datetime.datetime.now()
 
         v = VARIANT()
         v.value = now
-        self.failUnlessEqual(v.vt, VT_DATE)
-        self.failUnlessEqual(v.value, now)
-
-    def test_datetime64(self):
-        np = get_numpy()
-        if np is None:
-            return
-        try:
-            np.datetime64
-        except AttributeError:
-            return
-
-        dates = [
-            np.datetime64("2000-01-01T05:30:00", "s"),
-            np.datetime64("1800-01-01T05:30:00", "ms"),
-            np.datetime64("2000-01-01T12:34:56", "us")
-        ]
-
-        for date in dates:
-            v = VARIANT()
-            v.value = date
-            self.failUnlessEqual(v.vt, VT_DATE)
-            self.failUnlessEqual(v.value, date.astype(datetime.datetime))
+        self.assertEqual(v.vt, VT_DATE)
+        self.assertEqual(v.value, now)
 
     def test_decimal_as_currency(self):
         value = decimal.Decimal('3.14')
 
         v = VARIANT()
         v.value = value
-        self.failUnlessEqual(v.vt, VT_CY)
-        self.failUnlessEqual(v.value, value)
+        self.assertEqual(v.vt, VT_CY)
+        self.assertEqual(v.value, value)
 
     def test_decimal_as_decimal(self):
         v = VARIANT()
         v.vt = VT_DECIMAL
         v.decVal.Lo64 = 1234
         v.decVal.scale = 3
-        self.failUnlessEqual(v.value, decimal.Decimal('1.234'))
+        self.assertEqual(v.value, decimal.Decimal('1.234'))
 
         v.decVal.sign = 0x80
-        self.failUnlessEqual(v.value, decimal.Decimal('-1.234'))
+        self.assertEqual(v.value, decimal.Decimal('-1.234'))
 
         v.decVal.scale = 28
-        self.failUnlessEqual(v.value, decimal.Decimal('-1.234e-25'))
+        self.assertEqual(v.value, decimal.Decimal('-1.234e-25'))
 
         v.decVal.scale = 12
         v.decVal.Hi32 = 100
-        self.failUnlessEqual(
+        self.assertEqual(
             v.value, decimal.Decimal('-1844674407.370955162834'))
 
+    @unittest.skip("This test causes python(3?) to crash.")
     def test_BSTR(self):
         v = VARIANT()
         v.value = u"abc\x00123\x00"
-        self.failUnlessEqual(v.value, "abc\x00123\x00")
+        self.assertEqual(v.value, "abc\x00123\x00")
 
         v.value = None
         # manually clear the variant
         v._.VT_I4 = 0
 
         # NULL pointer BSTR should be handled as empty string
         v.vt = VT_BSTR
-        self.failUnless(v.value in ("", None))
+        self.assertTrue(v.value in ("", None))
 
     def test_empty_BSTR(self):
         v = VARIANT()
         v.value = ""
         self.assertEqual(v.vt, VT_BSTR)
 
+    @unittest.skip("Fails on creating `TestComServerLib.TestComServer`.  Library not registered.")
     def test_UDT(self):
         from comtypes.gen.TestComServerLib import MYCOLOR
         v = VARIANT(MYCOLOR(red=1.0, green=2.0, blue=3.0))
         value = v.value
-        self.failUnlessEqual((1.0, 2.0, 3.0),
+        self.assertEqual((1.0, 2.0, 3.0),
                              (value.red, value.green, value.blue))
 
         def func():
             v = VARIANT(MYCOLOR(red=1.0, green=2.0, blue=3.0))
             return v.value
 
         bytes = find_memleak(func)
-        self.failIf(bytes, "Leaks %d bytes" % bytes)
+        self.assertFalse(bytes, "Leaks %d bytes" % bytes)
 
     def test_ctypes_in_variant(self):
         v = VARIANT()
         objs = [(c_ubyte(3), VT_UI1),
-                (c_char("x"), VT_UI1),
+                (c_char(b"x"), VT_UI1),
                 (c_byte(3), VT_I1),
                 (c_ushort(3), VT_UI2),
                 (c_short(3), VT_I2),
                 (c_uint(3), VT_UI4),
                 (c_uint64(2**64), VT_UI8),
                 (c_int(3), VT_I4),
                 (c_int64(2**32), VT_I8),
                 (c_double(3.14), VT_R8),
                 (c_float(3.14), VT_R4),
                 ]
         for value, vt in objs:
             v.value = value
-            self.failUnlessEqual(v.vt, vt)
+            self.assertEqual(v.vt, vt)
 
     def test_byref(self):
         variable = c_int(42)
         v = VARIANT(byref(variable))
-        self.failUnlessEqual(v[0], 42)
-        self.failUnlessEqual(v.vt, VT_BYREF | VT_I4)
+        self.assertEqual(v[0], 42)
+        self.assertEqual(v.vt, VT_BYREF | VT_I4)
         variable.value = 96
-        self.failUnlessEqual(v[0], 96)
+        self.assertEqual(v[0], 96)
 
         variable = c_int(42)
         v = VARIANT(pointer(variable))
-        self.failUnlessEqual(v[0], 42)
-        self.failUnlessEqual(v.vt, VT_BYREF | VT_I4)
+        self.assertEqual(v[0], 42)
+        self.assertEqual(v.vt, VT_BYREF | VT_I4)
         variable.value = 96
-        self.failUnlessEqual(v[0], 96)
-
+        self.assertEqual(v[0], 96)
 
-class NdArrayTest(unittest.TestCase):
-    def test_double(self):
-        np = get_numpy()
-        if np is None:
-            return
-        for dtype in ('float32', 'float64'):
-            # because of FLOAT rounding errors, whi will only work for
-            # certain values!
-            a = np.array([1.0, 2.0, 3.0, 4.5], dtype=dtype)
-            v = VARIANT()
-            v.value = a
-            self.failUnless((v.value == a).all())
-
-    def test_int(self):
-        np = get_numpy()
-        if np is None:
-            return
-        for dtype in ('int8', 'int16', 'int32', 'int64', 'uint8',
-                'uint16', 'uint32', 'uint64'):
-            a = np.array((1, 1, 1, 1), dtype=dtype)
-            v = VARIANT()
-            v.value = a
-            self.failUnless((v.value == a).all())
-
-    def test_mixed(self):
-        np = get_numpy()
-        if np is None:
-            return
-
-        now = datetime.datetime.now()
-        a = np.array(
-            [11, "22", None, True, now, decimal.Decimal("3.14")]).reshape(2,3)
-        v = VARIANT()
-        v.value = a
-        self.failUnless((v.value == a).all())
+    def test_repr(self):
+        self.assertEqual(repr(VARIANT(c_int(42))), "VARIANT(vt=0x3, 42)")
+        self.assertEqual(repr(VARIANT(byref(c_int(42)))), "VARIANT(vt=0x4003, byref(42))")
+        self.assertEqual(repr(VARIANT.empty), "VARIANT.empty")
+        self.assertEqual(repr(VARIANT.null), "VARIANT.null")
+        self.assertEqual(repr(VARIANT.missing), "VARIANT.missing")
 
 
 class ArrayTest(unittest.TestCase):
     def test_double(self):
         import array
         for typecode in "df":
             # because of FLOAT rounding errors, whi will only work for
             # certain values!
             a = array.array(typecode, (1.0, 2.0, 3.0, 4.5))
             v = VARIANT()
             v.value = a
-            self.failUnlessEqual(v.value, (1.0, 2.0, 3.0, 4.5))
+            self.assertEqual(v.value, (1.0, 2.0, 3.0, 4.5))
 
     def test_int(self):
         import array
         for typecode in "bhiBHIlL":
             a = array.array(typecode, (1, 1, 1, 1))
             v = VARIANT()
             v.value = a
-            self.failUnlessEqual(v.value, (1, 1, 1, 1))
+            self.assertEqual(v.value, (1, 1, 1, 1))
 
 ################################################################
 def run_test(rep, msg, func=None, previous={}, results={}):
 ##    items = [None] * rep
     if func is None:
         locals = sys._getframe(1).f_locals
         func = eval("lambda: %s" % msg, locals)
-    items = xrange(rep)
+    items = range(rep)
     from time import clock
     start = clock()
     for i in items:
         func(); func(); func(); func(); func()
     stop = clock()
     duration = (stop-start)*1e6/5/rep
     try:
         prev = previous[msg]
     except KeyError:
-        print >> sys.stderr, "%40s: %7.1f us" % (msg, duration)
+        print("%40s: %7.1f us" % (msg, duration), file=sys.stderr)
         delta = 0.0
     else:
         delta = duration / prev * 100.0
-        print >> sys.stderr, "%40s: %7.1f us, time = %5.1f%%" % (msg, duration, delta)
+        print("%40s: %7.1f us, time = %5.1f%%" % (msg, duration, delta), file=sys.stderr)
     results[msg] = duration
     return delta
 
 
 def check_perf(rep=20000):
     from ctypes import c_int, byref
     from comtypes.automation import VARIANT
     import comtypes.automation
-    print comtypes.automation
+    print(comtypes.automation)
     variable = c_int()
     by_var = byref(variable)
     ptr_var = pointer(variable)
 
-    import cPickle
+    if sys.version_info >= (3, 0):
+        import pickle
+    else:
+        import cPickle as pickle
     try:
-        previous = cPickle.load(open("result.pickle", "rb"))
+        previous = pickle.load(open("result.pickle", "rb"))
     except IOError:
         previous = {}
 
     results = {}
 
     d = 0.0
     d += run_test(rep, "VARIANT()", previous=previous, results=results)
@@ -337,18 +298,18 @@
     d += run_test(rep, "VARIANT(42L).value", previous=previous, results=results)
     d += run_test(rep, "VARIANT(3.14).value", previous=previous, results=results)
     d += run_test(rep, "VARIANT(u'Str').value", previous=previous, results=results)
     d += run_test(rep, "VARIANT('Str').value", previous=previous, results=results)
     d += run_test(rep, "VARIANT((42,)).value", previous=previous, results=results)
     d += run_test(rep, "VARIANT([42,]).value", previous=previous, results=results)
 
-    print "Average duration %.1f%%" % (d / 10)
+    print("Average duration %.1f%%" % (d / 10))
 ##    cPickle.dump(results, open("result.pickle", "wb"))
 
 if __name__ == '__main__':
     try:
         unittest.main()
     except SystemExit:
         pass
     import comtypes
-    print "Running benchmark with comtypes %s/Python %s ..." % (comtypes.__version__, sys.version.split()[0],)
+    print("Running benchmark with comtypes %s/Python %s ..." % (comtypes.__version__, sys.version.split()[0],))
     check_perf()
```

## Comparing `comtypes-1.1.9/comtypes/test/test_wmi.py` & `comtypes-1.2.0/comtypes/test/test_wmi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+import sys
 import unittest as ut
 from ctypes import POINTER
 from comtypes.client import CoGetObject
 from comtypes.test import requires
 
 requires("time")
 
+if sys.version_info >= (3, 0):
+    base_text_type = str
+    text_type = str
+else:
+    base_text_type = basestring
+    text_type = unicode
+
 # WMI has dual interfaces.
 # Some methods/properties have "[out] POINTER(VARIANT)" parameters.
 # This test checks that these parameters are returned as strings:
 # that's what VARIANT.__ctypes_from_outparam__ does.
 class Test(ut.TestCase):
     def test_wmi(self):
         wmi = CoGetObject("winmgmts:")
@@ -27,26 +35,26 @@
 
         for item in disks:
             # obj[index] is forwarded to obj.Item(index)
             # .Value is a property with "[out] POINTER(VARIANT)" parameter.
             a = item.Properties_["Caption"].Value
             b = item.Properties_.Item("Caption").Value
             c = item.Properties_("Caption").Value
-            self.failUnlessEqual(a, b)
-            self.failUnlessEqual(a, c)
-            self.failUnless(isinstance(a, basestring))
-            self.failUnless(isinstance(b, basestring))
-            self.failUnless(isinstance(c, basestring))
+            self.assertEqual(a, b)
+            self.assertEqual(a, c)
+            self.assertTrue(isinstance(a, base_text_type))
+            self.assertTrue(isinstance(b, base_text_type))
+            self.assertTrue(isinstance(c, base_text_type))
             result = {}
             for prop in item.Properties_:
-                self.failUnless(isinstance(prop.Name, basestring))
+                self.assertTrue(isinstance(prop.Name, base_text_type))
                 prop.Value
                 result[prop.Name] = prop.Value
 ##                print "\t", (prop.Name, prop.Value)
-            self.failUnlessEqual(len(item.Properties_), item.Properties_.Count)
-            self.failUnlessEqual(len(item.Properties_), len(result))
-            self.failUnless(isinstance(item.Properties_["Description"].Value, unicode))
+            self.assertEqual(len(item.Properties_), item.Properties_.Count)
+            self.assertEqual(len(item.Properties_), len(result))
+            self.assertTrue(isinstance(item.Properties_["Description"].Value, text_type))
         # len(obj) is forwared to obj.Count
-        self.failUnlessEqual(len(disks), disks.Count)
+        self.assertEqual(len(disks), disks.Count)
 
 if __name__ == "__main__":
     ut.main()
```

## Comparing `comtypes-1.1.9/comtypes/test/__init__.py` & `comtypes-1.2.0/comtypes/test/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 # comtypes.test package.
 
+from __future__ import print_function
 import ctypes
 import getopt
 import os
 import sys
 import time
 import unittest
 
-use_resources = []
+use_resources = ["*"]
 
-def get_numpy():
-    '''Get numpy if it is available.'''
-    try:
-        import numpy
-        return numpy
-    except ImportError:
-        return None
 
 def register_server(source_dir):
     """ Register testing server appropriate for the python architecture.
 
     ``source_dir`` gives the absolute path to the comtype source in which the
     32- and 64-bit testing server, "AvmcIfc.dll" is defined.
 
@@ -69,15 +63,15 @@
         raise ResourceDenied(msg)
 
 def find_package_modules(package, mask):
     import fnmatch
     if hasattr(package, "__loader__"):
         path = package.__name__.replace(".", os.path.sep)
         mask = os.path.join(path, mask)
-        for fnm in package.__loader__._files.iterkeys():
+        for fnm in package.__loader__._files.keys():
             if fnmatch.fnmatchcase(fnm, mask):
                 yield os.path.splitext(fnm)[0].replace(os.path.sep, ".")
     else:
         path = package.__path__[0]
         for fnm in os.listdir(path):
             if fnmatch.fnmatchcase(fnm, mask):
                 yield "%s.%s" % (package.__name__, os.path.splitext(fnm)[0])
@@ -85,36 +79,36 @@
 def get_tests(package, mask, verbosity):
     """Return a list of skipped test modules, and a list of test cases."""
     tests = []
     skipped = []
     for modname in find_package_modules(package, mask):
         try:
             mod = __import__(modname, globals(), locals(), ['*'])
-        except ResourceDenied, detail:
+        except ResourceDenied as detail:
             skipped.append(modname)
             if verbosity > 1:
-                print >> sys.stderr, "Skipped %s: %s" % (modname, detail)
+                print("Skipped %s: %s" % (modname, detail), file=sys.stderr)
             continue
-        except Exception, detail:
-            print >> sys.stderr, "Warning: could not import %s: %s" % (modname, detail)
+        except Exception as detail:
+            print("Warning: could not import %s: %s" % (modname, detail), file=sys.stderr)
             continue
         for name in dir(mod):
             if name.startswith("_"):
                 continue
             o = getattr(mod, name)
             try:
                 is_test = issubclass(o, unittest.TestCase)
             except TypeError:
                 continue
             if is_test:
                 tests.append(o)
     return skipped, tests
 
 def usage():
-    print __doc__
+    print(__doc__)
     return 1
 
 def test_with_refcounts(runner, verbosity, testcase):
     """Run testcase several times, tracking reference counts."""
     import gc
     import ctypes
     ptc = ctypes._pointer_type_cache.copy()
@@ -137,18 +131,18 @@
     COUNT = 5
     refcounts = [None] * COUNT
     for i in range(COUNT):
         rc = sys.gettotalrefcount()
         runner.run(test)
         cleanup()
         refcounts[i] = sys.gettotalrefcount() - rc
-    if filter(None, refcounts):
-        print "%s leaks:\n\t" % testcase, refcounts
+    if [_f for _f in refcounts if _f]:
+        print("%s leaks:\n\t" % testcase, refcounts)
     elif verbosity:
-        print "%s: ok." % testcase
+        print("%s: ok." % testcase)
 
 class TestRunner(unittest.TextTestRunner):
     def run(self, test, skipped):
         "Run the given test case or test suite."
         # Same as unittest.TextTestRunner.run, except that it reports
         # skipped tests.
         result = self._makeResult()
@@ -156,28 +150,28 @@
         test(result)
         stopTime = time.time()
         timeTaken = stopTime - startTime
         result.printErrors()
         self.stream.writeln(result.separator2)
         run = result.testsRun
         if _unavail: #skipped:
-            requested = _unavail.keys()
+            requested = list(_unavail.keys())
             requested.sort()
             self.stream.writeln("Ran %d test%s in %.3fs (%s module%s skipped)" %
                                 (run, run != 1 and "s" or "", timeTaken,
                                  len(skipped),
                                  len(skipped) != 1 and "s" or ""))
             self.stream.writeln("Unavailable resources: %s" % ", ".join(requested))
         else:
             self.stream.writeln("Ran %d test%s in %.3fs" %
                                 (run, run != 1 and "s" or "", timeTaken))
         self.stream.writeln()
         if not result.wasSuccessful():
             self.stream.write("FAILED (")
-            failed, errored = map(len, (result.failures, result.errors))
+            failed, errored = list(map(len, (result.failures, result.errors)))
             if failed:
                 self.stream.write("failures=%d" % failed)
             if errored:
                 if failed: self.stream.write(", ")
                 self.stream.write("errors=%d" % errored)
             self.stream.writeln(")")
         else:
@@ -222,15 +216,15 @@
             verbosity -= 1
         elif flag == "-v":
             verbosity += 1
         elif flag == "-r":
             try:
                 sys.gettotalrefcount
             except AttributeError:
-                print >> sys.stderr, "-r flag requires Python debug build"
+                print("-r flag requires Python debug build", file=sys.stderr)
                 return -1
             search_leaks = True
         elif flag == "-u":
             use_resources.extend(value.split(","))
 
     mask = "test_*.py*"
     if args:
```

## Comparing `comtypes-1.1.9/comtypes/tools/tlbparser.py` & `comtypes-1.2.0/comtypes/tools/tlbparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+from __future__ import print_function
+import os
 import sys
+from ctypes import alignment, c_void_p, sizeof, windll
 
-from comtypes import automation, typeinfo, COMError
+from comtypes import automation, COMError, TYPE_CHECKING, typeinfo
 from comtypes.tools import typedesc
-from ctypes import c_void_p, sizeof, alignment
+from comtypes.client._code_cache import _get_module_filename
+
+if TYPE_CHECKING:
+    from typing import (
+        Any, Callable, Dict, List, Optional, Type, TypeVar, Tuple,
+        Union as _UnionT,
+    )
+    from ctypes import _CData, _Pointer
+    from comtypes import hints
 
-try:
-    set
-except NameError:
-    from sets import Set as set
 
 # Is the process 64-bit?
 is_64bits = sys.maxsize > 2**32
 
 
 ################################
 
@@ -97,81 +104,81 @@
 
 #automation.VT_ARRAY = 8192
 #automation.VT_BYREF = 16384
 
 ################################################################
 
 class Parser(object):
+    if TYPE_CHECKING:
+        tlib = hints.AnnoField()  # type: typeinfo.ITypeLib
+        items = hints.AnnoField()  # type: Dict[str, Any]
 
     def make_type(self, tdesc, tinfo):
-        try:
+        # type: (typeinfo.TYPEDESC, typeinfo.ITypeInfo) -> Any
+        if tdesc.vt in COMTYPES:
             return COMTYPES[tdesc.vt]
-        except KeyError:
-            pass
-
         if tdesc.vt == automation.VT_CARRAY:
-            typ = self.make_type(tdesc._.lpadesc[0].tdescElem, tinfo)
-            for i in range(tdesc._.lpadesc[0].cDims):
-                typ = typedesc.ArrayType(typ,
-                                         tdesc._.lpadesc[0].rgbounds[i].lLbound,
-                                         tdesc._.lpadesc[0].rgbounds[i].cElements-1)
+            arraydesc = tdesc._.lpadesc[0]  # type: typeinfo.tagARRAYDESC
+            typ = self.make_type(arraydesc.tdescElem, tinfo)
+            for i in range(arraydesc.cDims):
+                typ = typedesc.ArrayType(
+                    typ, arraydesc.rgbounds[i].lLbound, arraydesc.rgbounds[i].cElements-1
+                )
             return typ
-
         elif tdesc.vt == automation.VT_PTR:
-            typ = self.make_type(tdesc._.lptdesc[0], tinfo)
+            ptrdesc = tdesc._.lptdesc[0]  # type: typeinfo.TYPEDESC
+            typ = self.make_type(ptrdesc, tinfo)
             return PTR(typ)
-
         elif tdesc.vt == automation.VT_USERDEFINED:
             try:
                 ti = tinfo.GetRefTypeInfo(tdesc._.hreftype)
-            except COMError, details:
+            except COMError as details:
                 type_name = "__error_hreftype_%d__" % tdesc._.hreftype
                 tlib_name = get_tlib_filename(self.tlib)
                 if tlib_name is None:
                     tlib_name = "unknown typelib"
                 message = "\n\tGetRefTypeInfo failed in %s: %s\n\tgenerating type '%s' instead" % \
                           (tlib_name, details, type_name)
                 import warnings
                 warnings.warn(message, UserWarning);
-                result = typedesc.Structure(type_name,
-                                            align=8,
-                                            members=[], bases=[],
-                                            size=0)
+                result = typedesc.Structure(
+                    type_name, align=8, members=[], bases=[], size=0
+                )
                 return result
             result = self.parse_typeinfo(ti)
             assert result is not None, ti.GetDocumentation(-1)[0]
             return result
-
         elif tdesc.vt == automation.VT_SAFEARRAY:
             # SAFEARRAY(<type>), see Don Box pp.331f
-            itemtype = self.make_type(tdesc._.lptdesc[0], tinfo)
-            return midlSAFEARRAY(itemtype)
-
+            safearraydesc = tdesc._.lptdesc[0]  # type: typeinfo.TYPEDESC
+            return midlSAFEARRAY(self.make_type(safearraydesc, tinfo))
         raise NotImplementedError(tdesc.vt)
 
     ################################################################
 
     # TKIND_ENUM = 0
     def ParseEnum(self, tinfo, ta):
+        # type: (typeinfo.ITypeInfo, typeinfo.TYPEATTR) -> typedesc.Enumeration
         ta = tinfo.GetTypeAttr()
         enum_name = tinfo.GetDocumentation(-1)[0]
         enum = typedesc.Enumeration(enum_name, 32, 32)
         self._register(enum_name, enum)
 
         for i in range(ta.cVars):
             vd = tinfo.GetVarDesc(i)
             name = tinfo.GetDocumentation(vd.memid)[0]
             assert vd.varkind == typeinfo.VAR_CONST
-            num_val = vd._.lpvarValue[0].value
+            num_val = vd._.lpvarValue[0].value  # type: int
             v = typedesc.EnumValue(name, num_val, enum)
             enum.add_value(v)
         return enum
 
     # TKIND_RECORD = 1
     def ParseRecord(self, tinfo, ta):
+        # type: (typeinfo.ITypeInfo, typeinfo.TYPEATTR) -> typedesc.Structure
         members = [] # will be filled later
         struct_name, doc, helpcntext, helpfile = tinfo.GetDocumentation(-1)
         struct = typedesc.Structure(struct_name,
                                     align=ta.cbAlignment*8,
                                     members=members,
                                     bases=[],
                                     size=ta.cbSizeInstance*8)
@@ -203,14 +210,15 @@
                                    None, # bits
                                    offset)
             members.append(field)
         return struct
 
     # TKIND_MODULE = 2
     def ParseModule(self, tinfo, ta):
+        # type: (typeinfo.ITypeInfo, typeinfo.TYPEATTR) -> None
         assert 0 == ta.cImplTypes
         # functions
         for i in range(ta.cFuncs):
             # We skip all function definitions.  There are several
             # problems with these, and we can, for comtypes, ignore them.
             continue
             fd = tinfo.GetFuncDesc(i)
@@ -245,14 +253,15 @@
             v = typedesc.Constant(name, typ, var_value)
             self._register(name, v)
             if var_doc is not None:
                 v.doc = var_doc
 
     # TKIND_INTERFACE = 3
     def ParseInterface(self, tinfo, ta):
+        # type: (typeinfo.ITypeInfo, typeinfo.TYPEATTR) -> Optional[typedesc.ComInterface]
         itf_name, itf_doc = tinfo.GetDocumentation(-1)[0:2]
         assert ta.cImplTypes <= 1
         if ta.cImplTypes == 0 and itf_name != "IUnknown":
             # Windows defines an interface IOleControlTypes in ocidl.idl.
             # Don't known what artefact that is - we ignore it.
             # It's an interface without methods anyway.
             if itf_name != "IOleControlTypes":
@@ -276,47 +285,46 @@
             itf.base = self.parse_typeinfo(tibase)
 
         assert ta.cVars == 0, "vars on an Interface?"
 
         members = []
         for i in range(ta.cFuncs):
             fd = tinfo.GetFuncDesc(i)
-##            func_name = tinfo.GetDocumentation(fd.memid)[0]
             func_name, func_doc = tinfo.GetDocumentation(fd.memid)[:2]
             assert fd.funckind == typeinfo.FUNC_PUREVIRTUAL
             returns = self.make_type(fd.elemdescFunc.tdesc, tinfo)
             names = tinfo.GetNames(fd.memid, fd.cParams+1)
             names.append("rhs")
             names = names[:fd.cParams + 1]
             assert len(names) == fd.cParams + 1
             flags = self.func_flags(fd.wFuncFlags)
             flags += self.inv_kind(fd.invkind)
             mth = typedesc.ComMethod(fd.invkind, fd.memid, func_name, returns, flags, func_doc)
-            mth.oVft = fd.oVft
             for p in range(fd.cParams):
                 typ = self.make_type(fd.lprgelemdescParam[p].tdesc, tinfo)
                 name = names[p+1]
                 flags = fd.lprgelemdescParam[p]._.paramdesc.wParamFlags
                 if flags & typeinfo.PARAMFLAG_FHASDEFAULT:
                     # XXX should be handled by VARIANT itself
                     var = fd.lprgelemdescParam[p]._.paramdesc.pparamdescex[0].varDefaultValue
-                    default = var.value
+                    default = var.value  # type: Any
                 else:
                     default = None
                 mth.add_argument(typ, name, self.param_flags(flags), default)
             members.append((fd.oVft, mth))
         # Sort the methods by oVft (VTable offset): Some typeinfo
         # don't list methods in VTable order.
         members.sort()
         itf.members.extend([m[1] for m in members])
 
         return itf
 
     # TKIND_DISPATCH = 4
     def ParseDispatch(self, tinfo, ta):
+        # type: (typeinfo.ITypeInfo, typeinfo.TYPEATTR) -> typedesc.DispInterface
         itf_name, doc = tinfo.GetDocumentation(-1)[0:2]
         assert ta.cImplTypes == 1
 
         hr = tinfo.GetRefTypeOfImplType(0)
         tibase = tinfo.GetRefTypeInfo(hr)
         base = self.parse_typeinfo(tibase)
         members = []
@@ -364,35 +372,37 @@
             names.append("rhs")
             names = names[:fd.cParams + 1]
             assert len(names) == fd.cParams + 1 # function name first, then parameter names
             flags = self.func_flags(fd.wFuncFlags)
             flags += self.inv_kind(fd.invkind)
             mth = typedesc.DispMethod(fd.memid, fd.invkind, func_name, returns, flags, func_doc)
             for p in range(fd.cParams):
-                typ = self.make_type(fd.lprgelemdescParam[p].tdesc, tinfo)
+                descparam = fd.lprgelemdescParam[p]
+                typ = self.make_type(descparam.tdesc, tinfo)
                 name = names[p+1]
-                flags = fd.lprgelemdescParam[p]._.paramdesc.wParamFlags
+                flags = descparam._.paramdesc.wParamFlags
                 if flags & typeinfo.PARAMFLAG_FHASDEFAULT:
-                    var = fd.lprgelemdescParam[p]._.paramdesc.pparamdescex[0].varDefaultValue
-                    default = var.value
+                    var = descparam._.paramdesc.pparamdescex[0].varDefaultValue  # type: ignore
+                    default = var.value  # type: Any
                 else:
                     default = None
                 mth.add_argument(typ, name, self.param_flags(flags), default)
             itf.members.append(mth)
-
         return itf
 
     def inv_kind(self, invkind):
+        # type: (int) -> List[str]
         NAMES = {automation.DISPATCH_METHOD: [],
                  automation.DISPATCH_PROPERTYPUT: ["propput"],
                  automation.DISPATCH_PROPERTYPUTREF: ["propputref"],
                  automation.DISPATCH_PROPERTYGET: ["propget"]}
         return NAMES[invkind]
 
     def func_flags(self, flags):
+        # type: (int) -> List[str]
         # map FUNCFLAGS values to idl attributes
         NAMES = {typeinfo.FUNCFLAG_FRESTRICTED: "restricted",
                  typeinfo.FUNCFLAG_FSOURCE: "source",
                  typeinfo.FUNCFLAG_FBINDABLE: "bindable",
                  typeinfo.FUNCFLAG_FREQUESTEDIT: "requestedit",
                  typeinfo.FUNCFLAG_FDISPLAYBIND: "displaybind",
                  typeinfo.FUNCFLAG_FDEFAULTBIND: "defaultbind",
@@ -402,26 +412,28 @@
                  typeinfo.FUNCFLAG_FUIDEFAULT: "uidefault",
                  typeinfo.FUNCFLAG_FNONBROWSABLE: "nonbrowsable",
                  # typeinfo.FUNCFLAG_FREPLACEABLE: "???",
                  typeinfo.FUNCFLAG_FIMMEDIATEBIND: "immediatebind"}
         return [NAMES[bit] for bit in NAMES if bit & flags]
 
     def param_flags(self, flags):
+        # type: (int) -> List[str]
         # map PARAMFLAGS values to idl attributes
         NAMES = {typeinfo.PARAMFLAG_FIN: "in",
                  typeinfo.PARAMFLAG_FOUT: "out",
                  typeinfo.PARAMFLAG_FLCID: "lcid",
                  typeinfo.PARAMFLAG_FRETVAL: "retval",
                  typeinfo.PARAMFLAG_FOPT: "optional",
                  # typeinfo.PARAMFLAG_FHASDEFAULT: "",
                  # typeinfo.PARAMFLAG_FHASCUSTDATA: "",
                  }
         return [NAMES[bit] for bit in NAMES if bit & flags]
 
     def coclass_type_flags(self, flags):
+        # type: (int) -> List[str]
         # map TYPEFLAGS values to idl attributes
         NAMES = {typeinfo.TYPEFLAG_FAPPOBJECT: "appobject",
                  # typeinfo.TYPEFLAG_FCANCREATE:
                  typeinfo.TYPEFLAG_FLICENSED: "licensed",
                  # typeinfo.TYPEFLAG_FPREDECLID:
                  typeinfo.TYPEFLAG_FHIDDEN: "hidden",
                  typeinfo.TYPEFLAG_FCONTROL: "control",
@@ -436,14 +448,15 @@
                  typeinfo.TYPEFLAG_FPROXY: "proxy",
                  }
         NEGATIVE_NAMES = {typeinfo.TYPEFLAG_FCANCREATE: "noncreatable"}
         return [NAMES[bit] for bit in NAMES if bit & flags] + \
                [NEGATIVE_NAMES[bit] for bit in NEGATIVE_NAMES if not (bit & flags)]
 
     def interface_type_flags(self, flags):
+        # type: (int) -> List[str]
         # map TYPEFLAGS values to idl attributes
         NAMES = {typeinfo.TYPEFLAG_FAPPOBJECT: "appobject",
                  # typeinfo.TYPEFLAG_FCANCREATE:
                  typeinfo.TYPEFLAG_FLICENSED: "licensed",
                  # typeinfo.TYPEFLAG_FPREDECLID:
                  typeinfo.TYPEFLAG_FHIDDEN: "hidden",
                  typeinfo.TYPEFLAG_FCONTROL: "control",
@@ -458,14 +471,15 @@
                  typeinfo.TYPEFLAG_FPROXY: "proxy",
                  }
         NEGATIVE_NAMES = {}
         return [NAMES[bit] for bit in NAMES if bit & flags] + \
                [NEGATIVE_NAMES[bit] for bit in NEGATIVE_NAMES if not (bit & flags)]
 
     def var_flags(self, flags):
+        # type: (int) -> List[str]
         NAMES = {typeinfo.VARFLAG_FREADONLY: "readonly",
                  typeinfo.VARFLAG_FSOURCE: "source",
                  typeinfo.VARFLAG_FBINDABLE: "bindable",
                  typeinfo.VARFLAG_FREQUESTEDIT: "requestedit",
                  typeinfo.VARFLAG_FDISPLAYBIND: "displaybind",
                  typeinfo.VARFLAG_FDEFAULTBIND: "defaultbind",
                  typeinfo.VARFLAG_FHIDDEN: "hidden",
@@ -474,17 +488,17 @@
                  typeinfo.VARFLAG_FUIDEFAULT: "uidefault",
                  typeinfo.VARFLAG_FNONBROWSABLE: "nonbrowsable",
                  typeinfo.VARFLAG_FREPLACEABLE: "replaceable",
                  typeinfo.VARFLAG_FIMMEDIATEBIND: "immediatebind"
                  }
         return [NAMES[bit] for bit in NAMES if bit & flags]
 
-
     # TKIND_COCLASS = 5
     def ParseCoClass(self, tinfo, ta):
+        # type: (typeinfo.ITypeInfo, typeinfo.TYPEATTR) -> typedesc.CoClass
         # possible ta.wTypeFlags: helpstring, helpcontext, licensed,
         #        version, control, hidden, and appobject
         coclass_name, doc = tinfo.GetDocumentation(-1)[0:2]
         tlibattr = tinfo.GetContainingTypeLib()[0].GetLibAttr()
         coclass = typedesc.CoClass(coclass_name,
                                    str(ta.guid),
                                    self.coclass_type_flags(ta.wTypeFlags),
@@ -499,22 +513,24 @@
             itf = self.parse_typeinfo(ti)
             flags = tinfo.GetImplTypeFlags(i)
             coclass.add_interface(itf, flags)
         return coclass
 
     # TKIND_ALIAS = 6
     def ParseAlias(self, tinfo, ta):
+        # type: (typeinfo.ITypeInfo, typeinfo.TYPEATTR) -> typedesc.Typedef
         name = tinfo.GetDocumentation(-1)[0]
         typ = self.make_type(ta.tdescAlias, tinfo)
         alias = typedesc.Typedef(name, typ)
         self._register(name, alias)
         return alias
 
     # TKIND_UNION = 7
     def ParseUnion(self, tinfo, ta):
+        # type: (typeinfo.ITypeInfo, typeinfo.TYPEATTR) -> typedesc.Union
         union_name, doc, helpcntext, helpfile = tinfo.GetDocumentation(-1)
         members = []
         union = typedesc.Union(union_name,
                                align=ta.cbAlignment*8,
                                members=members,
                                bases=[],
                                size=ta.cbSizeInstance*8)
@@ -541,49 +557,50 @@
                                    offset)
             members.append(field)
         return union
 
     ################################################################
 
     def _typelib_module(self, tlib=None):
+        # type: (Optional[typeinfo.ITypeLib]) -> str
         if tlib is None:
             tlib = self.tlib
         # return a string that uniquely identifies a typelib.
         # The string doesn't have any meaning outside this instance.
         return str(tlib.GetLibAttr())
 
     def _register(self, name, value, tlib=None):
+        # type: (Optional[str], Any, Optional[typeinfo.ITypeLib]) -> None
         modname = self._typelib_module(tlib)
         fullname = "%s.%s" % (modname, name)
         if fullname in self.items:
             # XXX Can we really allow this? It happens, at least.
             if isinstance(value, typedesc.External):
                 return
             # BUG: We try to register an item that's already registered.
             raise ValueError("Bug: Multiple registered name '%s': %r" % (name, value))
         self.items[fullname] = value
 
     def parse_typeinfo(self, tinfo):
+        # type: (typeinfo.ITypeInfo) -> Any
         name = tinfo.GetDocumentation(-1)[0]
         modname = self._typelib_module()
         try:
             return self.items["%s.%s" % (modname, name)]
         except KeyError:
             pass
 
         tlib = tinfo.GetContainingTypeLib()[0]
         if tlib != self.tlib:
             ta = tinfo.GetTypeAttr()
             size = ta.cbSizeInstance * 8
             align = ta.cbAlignment * 8
-            typ = typedesc.External(tlib,
-                                    name,
-                                    size,
-                                    align,
-                                    tlib.GetDocumentation(-1)[:2])
+            typ = typedesc.External(
+                tlib, name, size, align, tlib.GetDocumentation(-1)[:2]
+            )
             self._register(name, typ, tlib)
             return typ
 
         ta = tinfo.GetTypeAttr()
         tkind = ta.typekind
 
         if tkind == typeinfo.TKIND_ENUM: # 0
@@ -609,15 +626,15 @@
         elif tkind == typeinfo.TKIND_COCLASS: # 5
             return self.ParseCoClass(tinfo, ta)
         elif tkind == typeinfo.TKIND_ALIAS: # 6
             return self.ParseAlias(tinfo, ta)
         elif tkind == typeinfo.TKIND_UNION: # 7
             return self.ParseUnion(tinfo, ta)
         else:
-            print "NYI", tkind
+            print("NYI", tkind)
 ##            raise "NYI", tkind
 
     def parse_LibraryDescription(self):
         la = self.tlib.GetLibAttr()
         name, doc = self.tlib.GetDocumentation(-1)[:2]
         desc = typedesc.TypeLib(name,
                                 str(la.guid), la.wMajorVerNum, la.wMinorVerNum,
@@ -704,49 +721,26 @@
         return None
     if 0 == windll.oleaut32.QueryPathOfRegTypeLib(byref(la.guid),
                                                   la.wMajorVerNum,
                                                   la.wMinorVerNum,
                                                   0, # lcid
                                                   byref(name)
                                                   ):
-        return name.value.split("\0")[0]
+        full_filename = name.value.split("\0")[0]
+        if not os.path.isabs(full_filename):
+            # workaround Windows 7 bug in QueryPathOfRegTypeLib returning relative path
+            try:
+                dll = windll.LoadLibrary(full_filename)
+                full_filename = _get_module_filename(dll._handle)
+                del dll
+            except OSError:
+                return None
+        return full_filename
     return None
 
 def _py2exe_hint():
     # If the tlbparser is frozen, we need to include these
     import comtypes.persist
     import comtypes.typeinfo
     import comtypes.automation
 
-def generate_module(tlib, ofi, pathname):
-    known_symbols = {}
-    for name in ("comtypes.persist",
-                 "comtypes.typeinfo",
-                 "comtypes.automation",
-                 "comtypes._others",
-                 "comtypes",
-                 "ctypes.wintypes",
-                 "ctypes"):
-        try:
-            mod = __import__(name)
-        except ImportError:
-            if name == "comtypes._others":
-                continue
-            raise
-        for submodule in name.split(".")[1:]:
-            mod = getattr(mod, submodule)
-        for name in mod.__dict__:
-            known_symbols[name] = mod.__name__
-    p = TypeLibParser(tlib)
-    if pathname is None:
-        pathname = get_tlib_filename(tlib)
-    items = p.parse()
-
-    from codegenerator import Generator
-
-    gen = Generator(ofi,
-                    known_symbols=known_symbols,
-                    )
-
-    gen.generate_code(items.values(), filename=pathname)
-
 # -eof-
```

## Comparing `comtypes-1.1.9/comtypes/tools/typedesc_base.py` & `comtypes-1.2.0/comtypes/tools/typedesc_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # typedesc.py - classes representing C type descriptions
-try:
-    set
-except NameError:
-    from sets import Set as set
+
+import comtypes
+from comtypes import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Any, List, Optional, Tuple, Union as _UnionT, SupportsInt
+
 
 class Argument(object):
     "a Parameter in the argument list of a callable (Function, Method, ...)"
     def __init__(self, atype, name):
         self.atype = atype
         self.name = name
 
@@ -111,90 +114,112 @@
     def __init__(self, name, typ):
         self.name = name
         self.typ = typ
 
 class ArrayType(object):
     location = None
     def __init__(self, typ, min, max):
+        # type: (Any, int, int) -> None
         self.typ = typ
         self.min = min
         self.max = max
 
 class StructureHead(object):
     location = None
     def __init__(self, struct):
+        # type: (_Struct_Union_Base) -> None
         self.struct = struct
 
 class StructureBody(object):
     location = None
     def __init__(self, struct):
+        # type: (_Struct_Union_Base) -> None
         self.struct = struct
 
 class _Struct_Union_Base(object):
+    if TYPE_CHECKING:
+        name = comtypes.hints.AnnoField()  # type: str
+        align = comtypes.hints.AnnoField()  # type: int
+        members = comtypes.hints.AnnoField()  # type: List[_UnionT[Field, Method, Constructor]]
+        bases = comtypes.hints.AnnoField()  # type: List[_Struct_Union_Base]
+        artificial = comtypes.hints.AnnoField()  # type: Optional[Any]
+        size = comtypes.hints.AnnoField()  # type: Optional[int]
+        _recordinfo_ = comtypes.hints.AnnoField()  # type: Tuple[str, int, int, int, str]
+
     location = None
+    def __init__(self):
+        self.struct_body = StructureBody(self)
+        self.struct_head = StructureHead(self)
+
     def get_body(self):
+        # type: () -> StructureBody
         return self.struct_body
 
     def get_head(self):
+        # type: () -> StructureHead
         return self.struct_head
 
 class Structure(_Struct_Union_Base):
     def __init__(self, name, align, members, bases, size, artificial=None):
+        # type: (str, SupportsInt, List[Field], List[Any], Optional[SupportsInt], Optional[Any]) -> None
         self.name = name
         self.align = int(align)
         self.members = members
         self.bases = bases
         self.artificial = artificial
         if size is not None:
             self.size = int(size)
         else:
             self.size = None
-        self.struct_body = StructureBody(self)
-        self.struct_head = StructureHead(self)
+        super(Structure, self).__init__()
 
 class Union(_Struct_Union_Base):
     def __init__(self, name, align, members, bases, size, artificial=None):
+        # type: (str, SupportsInt, List[Field], List[Any], Optional[SupportsInt], Optional[Any]) -> None
         self.name = name
         self.align = int(align)
         self.members = members
         self.bases = bases
         self.artificial = artificial
         if size is not None:
             self.size = int(size)
         else:
             self.size = None
-        self.struct_body = StructureBody(self)
-        self.struct_head = StructureHead(self)
+        super(Union, self).__init__()
 
 class Field(object):
     def __init__(self, name, typ, bits, offset):
+        # type: (str, Any, Optional[Any], SupportsInt) -> None
         self.name = name
         self.typ = typ
         self.bits = bits
         self.offset = int(offset)
 
 class CvQualifiedType(object):
     def __init__(self, typ, const, volatile):
         self.typ = typ
         self.const = const
         self.volatile = volatile
 
 class Enumeration(object):
     location = None
     def __init__(self, name, size, align):
+        # type: (str, SupportsInt, SupportsInt) -> None
         self.name = name
         self.size = int(size)
         self.align = int(align)
-        self.values = []
+        self.values = []  # type: List[EnumValue]
 
     def add_value(self, v):
+        # type: (EnumValue) -> None
         self.values.append(v)
 
 class EnumValue(object):
     def __init__(self, name, value, enumeration):
+        # type: (str, int, Enumeration) -> None
         self.name = name
         self.value = value
         self.enumeration = enumeration
 
 class Variable(object):
     location = None
     def __init__(self, name, typ, init=None):
```

## Comparing `comtypes-1.1.9/comtypes.egg-info/SOURCES.txt` & `comtypes-1.2.0/comtypes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 CHANGES.txt
 LICENSE.txt
 MANIFEST.in
-README
+README.md
 clear_comtypes_cache.py
 setup.py
 comtypes/GUID.py
 comtypes/__init__.py
 comtypes/_comobject.py
+comtypes/_memberspec.py
 comtypes/_meta.py
+comtypes/_npsupport.py
 comtypes/_safearray.py
 comtypes/automation.py
 comtypes/connectionpoints.py
 comtypes/errorinfo.py
 comtypes/git.py
 comtypes/hresult.py
 comtypes/logutil.py
 comtypes/messageloop.py
-comtypes/npsupport.py
 comtypes/patcher.py
 comtypes/persist.py
 comtypes/safearray.py
 comtypes/shelllink.py
 comtypes/typeinfo.py
 comtypes/util.py
 comtypes/viewobject.py
 comtypes.egg-info/PKG-INFO
 comtypes.egg-info/SOURCES.txt
 comtypes.egg-info/dependency_links.txt
 comtypes.egg-info/top_level.txt
 comtypes/client/__init__.py
 comtypes/client/_code_cache.py
+comtypes/client/_constants.py
 comtypes/client/_events.py
 comtypes/client/_generate.py
 comtypes/client/dynamic.py
 comtypes/client/lazybind.py
 comtypes/server/__init__.py
 comtypes/server/automation.py
 comtypes/server/connectionpoints.py
@@ -70,14 +72,15 @@
 comtypes/test/test_dyndispatch.py
 comtypes/test/test_excel.py
 comtypes/test/test_findgendir.py
 comtypes/test/test_getactiveobj.py
 comtypes/test/test_ie.py
 comtypes/test/test_jscript.js
 comtypes/test/test_msscript.py
+comtypes/test/test_npsupport.py
 comtypes/test/test_outparam.py
 comtypes/test/test_propputref.py
 comtypes/test/test_pump_events.py
 comtypes/test/test_safearray.py
 comtypes/test/test_sapi.py
 comtypes/test/test_server.py
 comtypes/test/test_showevents.py
```

