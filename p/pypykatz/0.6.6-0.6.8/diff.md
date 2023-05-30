# Comparing `tmp/pypykatz-0.6.6.tar.gz` & `tmp/pypykatz-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypykatz-0.6.6.tar", last modified: Sat Mar  4 20:11:22 2023, max compression
+gzip compressed data, was "pypykatz-0.6.8.tar", last modified: Tue May 30 16:14:33 2023, max compression
```

## Comparing `pypykatz-0.6.6.tar` & `pypykatz-0.6.8.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.463306 pypykatz-0.6.6/
--rw-rw-r--   0 root         (0) root         (0)     1077 2023-03-03 12:16:53.000000 pypykatz-0.6.6/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       26 2023-03-03 12:16:53.000000 pypykatz-0.6.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      392 2023-03-04 20:11:22.463306 pypykatz-0.6.6/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8346 2023-03-03 12:16:53.000000 pypykatz-0.6.6/README.md
--rw-rw-r--   0 root         (0) root         (0)       88 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.251305 pypykatz-0.6.6/pypykatz/
--rw-rw-r--   0 root         (0) root         (0)     4146 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/__amain__.py
--rw-rw-r--   0 root         (0) root         (0)       73 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4988 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/__main__.py
--rw-rw-r--   0 root         (0) root         (0)     1250 2023-03-04 19:51:27.000000 pypykatz-0.6.6/pypykatz/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.283305 pypykatz-0.6.6/pypykatz/alsadecryptor/
--rw-rw-r--   0 root         (0) root         (0)      143 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2013 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/asbmfile.py
--rw-rw-r--   0 root         (0) root         (0)     7568 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/cmdhelper.py
--rw-rw-r--   0 root         (0) root         (0)      642 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/lsa_decryptor.py
--rw-rw-r--   0 root         (0) root         (0)    13743 2023-03-04 19:49:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/lsa_decryptor_nt5.py
--rw-rw-r--   0 root         (0) root         (0)     4002 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/lsa_decryptor_nt6.py
--rw-rw-r--   0 root         (0) root         (0)     3400 2023-03-03 23:46:37.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/lsa_template_nt5.py
--rw-rw-r--   0 root         (0) root         (0)    16955 2023-03-04 19:43:16.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/lsa_template_nt6.py
--rw-rw-r--   0 root         (0) root         (0)     1351 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/lsa_templates.py
--rw-rw-r--   0 root         (0) root         (0)     7094 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/package_commons.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.283305 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/
--rw-rw-r--   0 root         (0) root         (0)     1305 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.291305 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/cloudap/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/cloudap/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2935 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/cloudap/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)     5189 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/cloudap/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.291305 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/credman/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/credman/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15019 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/credman/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.295305 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/dpapi/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/dpapi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2374 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/dpapi/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)     3912 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/dpapi/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.295305 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/kerberos/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/kerberos/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10404 2023-03-03 23:47:58.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/kerberos/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)    68801 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/kerberos/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.295305 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/livessp/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/livessp/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2579 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/livessp/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)     3133 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/livessp/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.303305 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/msv/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/msv/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    16329 2023-03-03 21:51:02.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/msv/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)    35725 2023-03-03 21:41:23.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/msv/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.303305 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/ssp/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/ssp/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2673 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/ssp/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)     2937 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/ssp/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.307305 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/tspkg/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/tspkg/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3491 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/tspkg/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)     5017 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/tspkg/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.311305 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/wdigest/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/wdigest/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3096 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/wdigest/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)     4884 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/packages/wdigest/templates.py
--rw-rw-r--   0 root         (0) root         (0)    25656 2023-03-03 23:14:17.000000 pypykatz-0.6.6/pypykatz/alsadecryptor/win_datatypes.py
--rw-rw-r--   0 root         (0) root         (0)    11699 2023-03-03 19:47:55.000000 pypykatz-0.6.6/pypykatz/apypykatz.py
--rw-rw-r--   0 root         (0) root         (0)    11849 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/argparsertest.py
--rw-rw-r--   0 root         (0) root         (0)      395 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/argpretty.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.311305 pypykatz-0.6.6/pypykatz/commons/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14242 2023-03-03 15:00:07.000000 pypykatz-0.6.6/pypykatz/commons/common.py
--rw-rw-r--   0 root         (0) root         (0)     3014 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/filetime.py
--rw-rw-r--   0 root         (0) root         (0)     8828 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/kerberosticket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.311305 pypykatz-0.6.6/pypykatz/commons/readers/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.311305 pypykatz-0.6.6/pypykatz/commons/readers/local/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.323305 pypykatz-0.6.6/pypykatz/commons/readers/local/common/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/common/__init__.py
--rw-rw-r--   0 root         (0) root         (0)   113173 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/common/advapi32.py
--rw-rw-r--   0 root         (0) root         (0)    23500 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/common/defines.py
--rw-rw-r--   0 root         (0) root         (0)      590 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/common/fileinfo.py
--rw-rw-r--   0 root         (0) root         (0)    22801 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/common/kernel32.py
--rw-rw-r--   0 root         (0) root         (0)     6625 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/common/live_reader_ctypes.py
--rw-rw-r--   0 root         (0) root         (0)     1459 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/common/privileges.py
--rw-rw-r--   0 root         (0) root         (0)     8117 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/common/privileges_types.py
--rw-rw-r--   0 root         (0) root         (0)    13706 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/common/psapi.py
--rw-rw-r--   0 root         (0) root         (0)    36775 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/common/version.py
--rw-rw-r--   0 root         (0) root         (0)     1824 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/common/winreg.py
--rw-rw-r--   0 root         (0) root         (0)    14051 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/live_reader.py
--rw-rw-r--   0 root         (0) root         (0)    15660 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/local/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.331305 pypykatz-0.6.6/pypykatz/commons/readers/registry/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/registry/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.331305 pypykatz-0.6.6/pypykatz/commons/readers/registry/live/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/registry/live/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2103 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/registry/live/reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.331305 pypykatz-0.6.6/pypykatz/commons/readers/rekall/
--rw-rw-r--   0 root         (0) root         (0)      121 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/rekall/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7273 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/rekall/rekallreader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.331305 pypykatz-0.6.6/pypykatz/commons/readers/volatility3/
--rw-rw-r--   0 root         (0) root         (0)      494 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/volatility3/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7574 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/readers/volatility3/volreader.py
--rw-rw-r--   0 root         (0) root         (0)     6800 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/win_datatypes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.331305 pypykatz-0.6.6/pypykatz/commons/winapi/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7580 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.331305 pypykatz-0.6.6/pypykatz/commons/winapi/local/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3468 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/advapi32.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.347305 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)   114578 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/advapi32.py
--rw-rw-r--   0 root         (0) root         (0)    23608 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/defines.py
--rw-rw-r--   0 root         (0) root         (0)      590 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/fileinfo.py
--rw-rw-r--   0 root         (0) root         (0)    23491 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/kernel32.py
--rw-rw-r--   0 root         (0) root         (0)     3499 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/live_reader_ctypes.py
--rw-rw-r--   0 root         (0) root         (0)    11817 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/netapi32.py
--rw-rw-r--   0 root         (0) root         (0)     4186 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/netapi32_high.py
--rw-rw-r--   0 root         (0) root         (0)     6162 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/ntdll.py
--rw-rw-r--   0 root         (0) root         (0)     1459 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/privileges.py
--rw-rw-r--   0 root         (0) root         (0)     8117 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/privileges_types.py
--rw-rw-r--   0 root         (0) root         (0)    13706 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/psapi.py
--rw-rw-r--   0 root         (0) root         (0)    36775 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/version.py
--rw-rw-r--   0 root         (0) root         (0)     1824 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/winreg.py
--rw-rw-r--   0 root         (0) root         (0)      455 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/kernel32.py
--rw-rw-r--   0 root         (0) root         (0)      369 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/localwindowsapi.py
--rw-rw-r--   0 root         (0) root         (0)      306 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/ntdll.py
--rw-rw-r--   0 root         (0) root         (0)      185 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/psapi.py
--rw-rw-r--   0 root         (0) root         (0)     8719 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/local/sid.py
--rw-rw-r--   0 root         (0) root         (0)     4442 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/machine.py
--rw-rw-r--   0 root         (0) root         (0)     7715 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/commons/winapi/processmanipulator.py
--rw-rw-r--   0 root         (0) root         (0)     2216 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/debugfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.347305 pypykatz-0.6.6/pypykatz/dpapi/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/dpapi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    18077 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/dpapi/cmdhelper.py
--rw-rw-r--   0 root         (0) root         (0)     8056 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/dpapi/constants.py
--rw-rw-r--   0 root         (0) root         (0)    32019 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/dpapi/dpapi.py
--rw-rw-r--   0 root         (0) root         (0)     2820 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/dpapi/extras.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.347305 pypykatz-0.6.6/pypykatz/dpapi/functiondefs/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/dpapi/functiondefs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2046 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/dpapi/functiondefs/dpapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.355305 pypykatz-0.6.6/pypykatz/dpapi/structures/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/dpapi/structures/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6022 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/dpapi/structures/blob.py
--rw-rw-r--   0 root         (0) root         (0)     6418 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/dpapi/structures/credentialfile.py
--rw-rw-r--   0 root         (0) root         (0)     6949 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/dpapi/structures/masterkeyfile.py
--rw-rw-r--   0 root         (0) root         (0)      785 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/dpapi/structures/system.py
--rw-rw-r--   0 root         (0) root         (0)     9420 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/dpapi/structures/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.355305 pypykatz-0.6.6/pypykatz/example/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/example/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      701 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/example/phandle_dll.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.355305 pypykatz-0.6.6/pypykatz/kerberos/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/kerberos/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    18194 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/kerberos/cmdhelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.359305 pypykatz-0.6.6/pypykatz/kerberos/functiondefs/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/kerberos/functiondefs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5629 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/kerberos/functiondefs/advapi32.py
--rw-rw-r--   0 root         (0) root         (0)      965 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/kerberos/functiondefs/asn1structs.py
--rw-rw-r--   0 root         (0) root         (0)     1425 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/kerberos/functiondefs/kernel32.py
--rw-rw-r--   0 root         (0) root         (0)    48844 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/kerberos/functiondefs/netsecapi.py
--rw-rw-r--   0 root         (0) root         (0)     8670 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/kerberos/kerberos.py
--rw-rw-r--   0 root         (0) root         (0)    12969 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/kerberos/kerberoslive.py
--rw-rw-r--   0 root         (0) root         (0)     1723 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/kerberos/kirbiutils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.359305 pypykatz-0.6.6/pypykatz/ldap/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/ldap/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4458 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/ldap/cmdhelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.363305 pypykatz-0.6.6/pypykatz/lsadecryptor/
--rw-rw-r--   0 root         (0) root         (0)      143 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11057 2023-03-03 15:07:19.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/cmdhelper.py
--rw-rw-r--   0 root         (0) root         (0)      638 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/lsa_decryptor.py
--rw-rw-r--   0 root         (0) root         (0)    13543 2023-03-04 19:50:02.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/lsa_decryptor_nt5.py
--rw-rw-r--   0 root         (0) root         (0)     4182 2023-03-03 13:05:24.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/lsa_decryptor_nt6.py
--rw-rw-r--   0 root         (0) root         (0)     2949 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/lsa_template_nt5.py
--rw-rw-r--   0 root         (0) root         (0)    14946 2023-03-03 13:39:59.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/lsa_template_nt6.py
--rw-rw-r--   0 root         (0) root         (0)     1349 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/lsa_templates.py
--rw-rw-r--   0 root         (0) root         (0)     7024 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/package_commons.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.363305 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/
--rw-rw-r--   0 root         (0) root         (0)     1290 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.363305 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/cloudap/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/cloudap/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2842 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/cloudap/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)     4009 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/cloudap/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.363305 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/credman/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/credman/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9542 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/credman/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.375305 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/dpapi/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/dpapi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2307 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/dpapi/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)     3491 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/dpapi/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.375305 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/kerberos/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/kerberos/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10627 2023-03-03 23:32:10.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/kerberos/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)    44229 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/kerberos/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.375305 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/livessp/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/livessp/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2489 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/livessp/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)     2145 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/livessp/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.375305 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/msv/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/msv/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    16826 2023-03-03 21:49:19.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/msv/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)    26414 2023-03-03 21:35:02.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/msv/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.375305 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/ssp/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/ssp/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2531 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/ssp/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)     2387 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/ssp/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.375305 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/tspkg/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/tspkg/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3355 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/tspkg/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)     3700 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/tspkg/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.375305 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/wdigest/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/wdigest/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2966 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/wdigest/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)     4154 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/lsadecryptor/packages/wdigest/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.383305 pypykatz-0.6.6/pypykatz/parsers/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/parsers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3378 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/parsers/cmdhelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.383305 pypykatz-0.6.6/pypykatz/plugins/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/plugins/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3150 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/plugins/pypykatz_rekall.py
--rw-rw-r--   0 root         (0) root         (0)    13680 2023-03-03 15:05:29.000000 pypykatz-0.6.6/pypykatz/pypykatz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.383305 pypykatz-0.6.6/pypykatz/rdp/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/rdp/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2675 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/rdp/cmdhelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.383305 pypykatz-0.6.6/pypykatz/rdp/packages/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/rdp/packages/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.383305 pypykatz-0.6.6/pypykatz/rdp/packages/creds/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/rdp/packages/creds/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15541 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/rdp/packages/creds/decryptor.py
--rw-rw-r--   0 root         (0) root         (0)     3223 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/rdp/packages/creds/templates.py
--rw-rw-r--   0 root         (0) root         (0)     4905 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/rdp/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.391305 pypykatz-0.6.6/pypykatz/registry/
--rw-rw-r--   0 root         (0) root         (0)       54 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2803 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/aoffline_parser.py
--rw-rw-r--   0 root         (0) root         (0)     2605 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/cmdhelper.py
--rw-rw-r--   0 root         (0) root         (0)     3595 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/live_parser.py
--rw-rw-r--   0 root         (0) root         (0)     7104 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/offline_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.423306 pypykatz-0.6.6/pypykatz/registry/sam/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/sam/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5913 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/sam/asam.py
--rw-rw-r--   0 root         (0) root         (0)      562 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/sam/common.py
--rw-rw-r--   0 root         (0) root         (0)     5788 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/sam/sam.py
--rw-rw-r--   0 root         (0) root         (0)    13487 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/sam/structures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.435305 pypykatz-0.6.6/pypykatz/registry/security/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/security/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6891 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/security/acommon.py
--rw-rw-r--   0 root         (0) root         (0)     9293 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/security/asecurity.py
--rw-rw-r--   0 root         (0) root         (0)     6895 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/security/common.py
--rw-rw-r--   0 root         (0) root         (0)     9169 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/security/security.py
--rw-rw-r--   0 root         (0) root         (0)     5220 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/security/structures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.435305 pypykatz-0.6.6/pypykatz/registry/software/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/software/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1798 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/software/asoftware.py
--rw-rw-r--   0 root         (0) root         (0)     1726 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/software/software.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.435305 pypykatz-0.6.6/pypykatz/registry/system/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/system/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2739 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/system/asystem.py
--rw-rw-r--   0 root         (0) root         (0)     2645 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/registry/system/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.435305 pypykatz-0.6.6/pypykatz/remote/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/remote/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6590 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/remote/cmdhelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.439306 pypykatz-0.6.6/pypykatz/remote/live/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/remote/live/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.439306 pypykatz-0.6.6/pypykatz/remote/live/common/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/remote/live/common/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      318 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/remote/live/common/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.439306 pypykatz-0.6.6/pypykatz/remote/live/localgroup/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/remote/live/localgroup/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4608 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/remote/live/localgroup/enumerator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.443306 pypykatz-0.6.6/pypykatz/remote/live/session/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/remote/live/session/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4210 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/remote/live/session/enumerator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.443306 pypykatz-0.6.6/pypykatz/remote/live/share/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/remote/live/share/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4735 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/remote/live/share/enumerator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.447306 pypykatz-0.6.6/pypykatz/smb/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/smb/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    36903 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/smb/cmdhelper.py
--rw-rw-r--   0 root         (0) root         (0)      921 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/smb/dcsync.py
--rw-rw-r--   0 root         (0) root         (0)     7254 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/smb/lsassutils.py
--rw-rw-r--   0 root         (0) root         (0)     2172 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/smb/printer.py
--rw-rw-r--   0 root         (0) root         (0)     7846 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/smb/regutils.py
--rw-rw-r--   0 root         (0) root         (0)     2987 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/smb/shareenum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.447306 pypykatz-0.6.6/pypykatz/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.463306 pypykatz-0.6.6/pypykatz/utils/crypto/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/utils/crypto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2716 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/utils/crypto/cmdhelper.py
--rw-rw-r--   0 root         (0) root         (0)      630 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/utils/crypto/gppassword.py
--rw-rw-r--   0 root         (0) root         (0)    11726 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/utils/crypto/ofcdecrypt.py
--rw-rw-r--   0 root         (0) root         (0)     1876 2023-03-03 12:16:53.000000 pypykatz-0.6.6/pypykatz/utils/crypto/winhash.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.255305 pypykatz-0.6.6/pypykatz.egg-info/
--rw-r--r--   0 root         (0) root         (0)      392 2023-03-04 20:11:22.000000 pypykatz-0.6.6/pypykatz.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9400 2023-03-04 20:11:22.000000 pypykatz-0.6.6/pypykatz.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-04 20:11:22.000000 pypykatz-0.6.6/pypykatz.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-03-04 20:11:22.000000 pypykatz-0.6.6/pypykatz.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-03-04 20:11:22.000000 pypykatz-0.6.6/pypykatz.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-04 20:11:22.000000 pypykatz-0.6.6/pypykatz.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-04 20:11:22.000000 pypykatz-0.6.6/pypykatz.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-04 20:11:22.463306 pypykatz-0.6.6/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1577 2023-03-04 19:51:12.000000 pypykatz-0.6.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 20:11:22.463306 pypykatz-0.6.6/tests/
--rw-rw-r--   0 root         (0) root         (0)    10424 2023-03-03 23:41:25.000000 pypykatz-0.6.6/tests/test_async_lsassdecrypt.py
--rw-rw-r--   0 root         (0) root         (0)     9301 2023-03-03 19:42:49.000000 pypykatz-0.6.6/tests/test_lsassdecrypt.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.769717 pypykatz-0.6.8/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1077 2023-03-05 19:48:41.000000 pypykatz-0.6.8/LICENSE
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       26 2023-03-05 19:48:41.000000 pypykatz-0.6.8/MANIFEST.in
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      392 2023-05-30 16:14:33.765717 pypykatz-0.6.8/PKG-INFO
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8346 2023-03-05 19:48:41.000000 pypykatz-0.6.8/README.md
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       88 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pyproject.toml
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.701717 pypykatz-0.6.8/pypykatz/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4146 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/__amain__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       73 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4988 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/__main__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1250 2023-05-02 14:09:16.000000 pypykatz-0.6.8/pypykatz/_version.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.709717 pypykatz-0.6.8/pypykatz/alsadecryptor/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      143 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2013 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/asbmfile.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7601 2023-05-03 19:54:01.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/cmdhelper.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      642 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/lsa_decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    13761 2023-05-02 13:33:05.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/lsa_decryptor_nt5.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4047 2023-05-02 13:31:04.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/lsa_decryptor_nt6.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3400 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/lsa_template_nt5.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    17427 2023-05-02 13:30:23.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/lsa_template_nt6.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1351 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/lsa_templates.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7141 2023-05-02 13:32:21.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/package_commons.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.709717 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1305 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.709717 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/cloudap/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/cloudap/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3094 2023-05-03 19:53:13.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/cloudap/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6521 2023-05-02 14:00:39.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/cloudap/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.713717 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/credman/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/credman/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    15019 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/credman/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.713717 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/dpapi/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/dpapi/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2374 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/dpapi/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3912 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/dpapi/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.713717 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/kerberos/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/kerberos/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    10404 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/kerberos/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    68801 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/kerberos/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.717717 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/livessp/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/livessp/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2579 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/livessp/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3133 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/livessp/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.717717 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/msv/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/msv/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    16981 2023-05-02 14:06:26.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/msv/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    35725 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/msv/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.717717 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/ssp/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/ssp/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2673 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/ssp/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2937 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/ssp/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.721717 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/tspkg/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/tspkg/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3491 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/tspkg/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5017 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/tspkg/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.721717 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/wdigest/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/wdigest/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3096 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/wdigest/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4884 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/packages/wdigest/templates.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    25656 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/alsadecryptor/win_datatypes.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    11699 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/apypykatz.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    11849 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/argparsertest.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      395 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/argpretty.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.721717 pypykatz-0.6.8/pypykatz/commons/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    14494 2023-05-03 09:23:57.000000 pypykatz-0.6.8/pypykatz/commons/common.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3014 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/filetime.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8828 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/kerberosticket.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.721717 pypykatz-0.6.8/pypykatz/commons/readers/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.725717 pypykatz-0.6.8/pypykatz/commons/readers/local/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.729717 pypykatz-0.6.8/pypykatz/commons/readers/local/common/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/common/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)   113173 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/common/advapi32.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    23500 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/common/defines.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      590 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/common/fileinfo.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    22801 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/common/kernel32.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6625 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/common/live_reader_ctypes.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1459 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/common/privileges.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8117 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/common/privileges_types.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    13706 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/common/psapi.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    36775 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/common/version.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1824 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/common/winreg.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    14051 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/live_reader.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    15660 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/local/process.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.729717 pypykatz-0.6.8/pypykatz/commons/readers/registry/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/registry/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.729717 pypykatz-0.6.8/pypykatz/commons/readers/registry/live/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/registry/live/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2103 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/registry/live/reader.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.729717 pypykatz-0.6.8/pypykatz/commons/readers/rekall/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      121 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/rekall/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7273 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/rekall/rekallreader.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.733717 pypykatz-0.6.8/pypykatz/commons/readers/volatility3/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      494 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/volatility3/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7574 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/readers/volatility3/volreader.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6800 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/win_datatypes.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.733717 pypykatz-0.6.8/pypykatz/commons/winapi/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7580 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/constants.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.733717 pypykatz-0.6.8/pypykatz/commons/winapi/local/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3468 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/advapi32.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.741717 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)   114578 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/advapi32.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    23608 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/defines.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      590 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/fileinfo.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    23491 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/kernel32.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3499 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/live_reader_ctypes.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    11817 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/netapi32.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4186 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/netapi32_high.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6162 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/ntdll.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1459 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/privileges.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8117 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/privileges_types.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    13706 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/psapi.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    36775 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/version.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1824 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/winreg.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      455 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/kernel32.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      369 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/localwindowsapi.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      306 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/ntdll.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      185 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/psapi.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8719 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/local/sid.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4442 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/machine.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7715 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/commons/winapi/processmanipulator.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2216 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/debugfile.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.741717 pypykatz-0.6.8/pypykatz/dpapi/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/dpapi/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    18552 2023-05-02 12:41:42.000000 pypykatz-0.6.8/pypykatz/dpapi/cmdhelper.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8056 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/dpapi/constants.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    32577 2023-05-03 19:51:08.000000 pypykatz-0.6.8/pypykatz/dpapi/dpapi.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2820 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/dpapi/extras.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.741717 pypykatz-0.6.8/pypykatz/dpapi/functiondefs/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/dpapi/functiondefs/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2046 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/dpapi/functiondefs/dpapi.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.741717 pypykatz-0.6.8/pypykatz/dpapi/structures/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/dpapi/structures/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6022 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/dpapi/structures/blob.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6418 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/dpapi/structures/credentialfile.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6949 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/dpapi/structures/masterkeyfile.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      785 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/dpapi/structures/system.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     9420 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/dpapi/structures/vault.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.745717 pypykatz-0.6.8/pypykatz/example/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/example/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      701 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/example/phandle_dll.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.745717 pypykatz-0.6.8/pypykatz/kerberos/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/kerberos/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    18194 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/kerberos/cmdhelper.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.745717 pypykatz-0.6.8/pypykatz/kerberos/functiondefs/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/kerberos/functiondefs/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5629 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/kerberos/functiondefs/advapi32.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      965 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/kerberos/functiondefs/asn1structs.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1425 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/kerberos/functiondefs/kernel32.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    48844 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/kerberos/functiondefs/netsecapi.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8670 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/kerberos/kerberos.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    12969 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/kerberos/kerberoslive.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1723 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/kerberos/kirbiutils.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.745717 pypykatz-0.6.8/pypykatz/ldap/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/ldap/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4458 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/ldap/cmdhelper.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.749717 pypykatz-0.6.8/pypykatz/lsadecryptor/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      143 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    11456 2023-05-02 13:28:38.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/cmdhelper.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      638 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/lsa_decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    13563 2023-05-02 13:29:14.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/lsa_decryptor_nt5.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4238 2023-05-02 11:00:26.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/lsa_decryptor_nt6.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2949 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/lsa_template_nt5.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    15907 2023-05-02 12:43:38.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/lsa_template_nt6.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1349 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/lsa_templates.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7069 2023-05-02 11:00:51.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/package_commons.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.749717 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1290 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.749717 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/cloudap/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/cloudap/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3035 2023-05-02 19:36:56.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/cloudap/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4090 2023-05-03 19:49:31.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/cloudap/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.749717 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/credman/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/credman/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     9542 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/credman/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.749717 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/dpapi/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/dpapi/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2307 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/dpapi/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3491 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/dpapi/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.749717 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/kerberos/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/kerberos/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    10627 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/kerberos/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    44229 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/kerberos/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.753717 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/livessp/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/livessp/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2489 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/livessp/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2145 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/livessp/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.753717 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/msv/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/msv/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    17477 2023-05-02 14:06:53.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/msv/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    26414 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/msv/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.753717 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/ssp/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/ssp/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2531 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/ssp/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2387 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/ssp/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.753717 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/tspkg/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/tspkg/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3355 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/tspkg/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3700 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/tspkg/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.753717 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/wdigest/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/wdigest/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2966 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/wdigest/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4154 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/lsadecryptor/packages/wdigest/templates.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.753717 pypykatz-0.6.8/pypykatz/parsers/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/parsers/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3378 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/parsers/cmdhelper.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.757717 pypykatz-0.6.8/pypykatz/plugins/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/plugins/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3150 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/plugins/pypykatz_rekall.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    13680 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/pypykatz.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.757717 pypykatz-0.6.8/pypykatz/rdp/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/rdp/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2675 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/rdp/cmdhelper.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.757717 pypykatz-0.6.8/pypykatz/rdp/packages/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/rdp/packages/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.757717 pypykatz-0.6.8/pypykatz/rdp/packages/creds/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/rdp/packages/creds/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    15541 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/rdp/packages/creds/decryptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3223 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/rdp/packages/creds/templates.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4905 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/rdp/parser.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.761717 pypykatz-0.6.8/pypykatz/registry/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       54 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2803 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/aoffline_parser.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2605 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/cmdhelper.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3595 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/live_parser.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7104 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/offline_parser.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.761717 pypykatz-0.6.8/pypykatz/registry/sam/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/sam/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5913 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/sam/asam.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      562 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/sam/common.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5788 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/sam/sam.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    13487 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/sam/structures.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.761717 pypykatz-0.6.8/pypykatz/registry/security/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/security/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6891 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/security/acommon.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     9293 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/security/asecurity.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6895 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/security/common.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     9169 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/security/security.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5220 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/security/structures.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.761717 pypykatz-0.6.8/pypykatz/registry/software/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/software/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1798 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/software/asoftware.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1726 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/software/software.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.761717 pypykatz-0.6.8/pypykatz/registry/system/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/system/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2739 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/system/asystem.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2645 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/registry/system/system.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.765717 pypykatz-0.6.8/pypykatz/remote/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/remote/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6590 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/remote/cmdhelper.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.765717 pypykatz-0.6.8/pypykatz/remote/live/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/remote/live/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.765717 pypykatz-0.6.8/pypykatz/remote/live/common/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/remote/live/common/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      318 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/remote/live/common/common.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.765717 pypykatz-0.6.8/pypykatz/remote/live/localgroup/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/remote/live/localgroup/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4608 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/remote/live/localgroup/enumerator.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.765717 pypykatz-0.6.8/pypykatz/remote/live/session/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/remote/live/session/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4210 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/remote/live/session/enumerator.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.765717 pypykatz-0.6.8/pypykatz/remote/live/share/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/remote/live/share/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4735 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/remote/live/share/enumerator.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.765717 pypykatz-0.6.8/pypykatz/smb/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/smb/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    36903 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/smb/cmdhelper.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      921 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/smb/dcsync.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7254 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/smb/lsassutils.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2172 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/smb/printer.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7846 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/smb/regutils.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2987 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/smb/shareenum.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.765717 pypykatz-0.6.8/pypykatz/utils/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/utils/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.765717 pypykatz-0.6.8/pypykatz/utils/crypto/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/utils/crypto/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2716 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/utils/crypto/cmdhelper.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      630 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/utils/crypto/gppassword.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    11726 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/utils/crypto/ofcdecrypt.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1876 2023-03-05 19:48:41.000000 pypykatz-0.6.8/pypykatz/utils/crypto/winhash.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.705717 pypykatz-0.6.8/pypykatz.egg-info/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      392 2023-05-30 16:14:33.000000 pypykatz-0.6.8/pypykatz.egg-info/PKG-INFO
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     9400 2023-05-30 16:14:33.000000 pypykatz-0.6.8/pypykatz.egg-info/SOURCES.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-05-30 16:14:33.000000 pypykatz-0.6.8/pypykatz.egg-info/dependency_links.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       52 2023-05-30 16:14:33.000000 pypykatz-0.6.8/pypykatz.egg-info/entry_points.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      134 2023-05-30 16:14:33.000000 pypykatz-0.6.8/pypykatz.egg-info/requires.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        9 2023-05-30 16:14:33.000000 pypykatz-0.6.8/pypykatz.egg-info/top_level.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-05-30 16:14:33.000000 pypykatz-0.6.8/pypykatz.egg-info/zip-safe
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       38 2023-05-30 16:14:33.769717 pypykatz-0.6.8/setup.cfg
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1578 2023-05-30 16:05:22.000000 pypykatz-0.6.8/setup.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:14:33.765717 pypykatz-0.6.8/tests/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    10424 2023-03-05 19:48:41.000000 pypykatz-0.6.8/tests/test_async_lsassdecrypt.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     9301 2023-03-05 19:48:41.000000 pypykatz-0.6.8/tests/test_lsassdecrypt.py
```

### Comparing `pypykatz-0.6.6/LICENSE` & `pypykatz-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/README.md` & `pypykatz-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/__amain__.py` & `pypykatz-0.6.8/pypykatz/__amain__.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/__main__.py` & `pypykatz-0.6.8/pypykatz/__main__.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/_version.py` & `pypykatz-0.6.8/pypykatz/_version.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__ = "0.6.6"
+__version__ = "0.6.8"
 __banner__ = \
 """
 # pypyKatz %s 
 # Author: Tamas Jos @skelsec
 # License: MIT
 """ % __version__
```

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/asbmfile.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/asbmfile.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/cmdhelper.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/cmdhelper.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,33 +165,33 @@
 	async def run(self, args):
 		files_with_error = []
 		results = {}
 		###### Minidump
 		if args.cmd == 'minidump':
 			if args.directory:
 				dir_fullpath = os.path.abspath(args.memoryfile)
-				file_pattern = '*.dmp'
-				if args.recursive == True:
-					globdata = os.path.join(dir_fullpath, '**', file_pattern)
-				else:	
-					globdata = os.path.join(dir_fullpath, file_pattern)
+				for file_pattern in ['*.dmp', '*.DMP']:
+					if args.recursive == True:
+						globdata = os.path.join(dir_fullpath, '**', file_pattern)
+					else:
+						globdata = os.path.join(dir_fullpath, file_pattern)
 					
-				logger.info('Parsing folder %s' % dir_fullpath)
-				for filename in glob.glob(globdata, recursive=args.recursive):
-					logger.info('Parsing file %s' % filename)
-					try:
-						mimi = await apypykatz.parse_minidump_file(filename, packages = args.packages)
-						results[filename] = mimi
-					except Exception as e:
-						files_with_error.append(filename)
-						logger.exception('Error parsing file %s ' % filename)
-						if args.halt_on_error == True:
-							raise e
-						else:
-							pass
+					logger.info('Parsing folder %s' % dir_fullpath)
+					for filename in glob.glob(globdata, recursive=args.recursive):
+						logger.info('Parsing file %s' % filename)
+						try:
+							mimi = await apypykatz.parse_minidump_file(filename, packages = args.packages)
+							results[filename] = mimi
+						except Exception as e:
+							files_with_error.append(filename)
+							logger.exception('Error parsing file %s ' % filename)
+							if args.halt_on_error == True:
+								raise e
+							else:
+								pass
 					
 			else:
 				logger.info('Parsing file %s' % args.memoryfile)
 				try:
 					mimi = await apypykatz.parse_minidump_file(args.memoryfile, packages = args.packages)
 					results[args.memoryfile] = mimi
 				except Exception as e:
```

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/lsa_decryptor.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/lsa_decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/lsa_decryptor_nt5.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/lsa_decryptor_nt5.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 			self.logger.log('signature not found! %s' % self.decryptor_template.signature.hex())
 			raise Exception('LSA signature not found!')
 			
 		self.log('Found candidates on the following positions: %s' % ' '.join(hex(x) for x in fl))
 		self.log('Selecting first one @ 0x%08x' % fl[0])
 		return fl[0]
 
-	def decrypt(self, encrypted):
+	def decrypt(self, encrypted, segment_size=128):
 		# TODO: NT version specific, move from here in subclasses.
 		cleartext = b''
 		size = len(encrypted)
 		if size:
 			if (size % 8) != 0:
 				ctx = RC4(self.random_key)
 				cleartext = ctx.decrypt(encrypted)
```

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/lsa_decryptor_nt6.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/lsa_decryptor_nt6.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,23 +73,23 @@
 			self.log('BCRYPT_KEY_DATA\n%s' % hexdump(data, start = ptr_key))
 			kbk = await kbhk.ptr_key.read(self.reader, self.decryptor_template.key_struct)
 			self.log('HARD_KEY SIZE: 0x%x' % kbk.size)
 			if kbk.verify():
 				self.log('HARD_KEY data:\n%s' % hexdump(kbk.hardkey.data))
 				return kbk.hardkey.data
 
-	def decrypt(self, encrypted):
+	def decrypt(self, encrypted, segment_size=128):
 		# TODO: NT version specific, move from here in subclasses.
 		cleartext = b''
 		size = len(encrypted)
 		if size:
 			if size % 8:
 				if not self.aes_key or not self.iv:
 					return cleartext
-				cipher = AES(self.aes_key, MODE_CFB, self.iv)
+				cipher = AES(self.aes_key, MODE_CFB, self.iv, segment_size=segment_size)
 				cleartext = cipher.decrypt(encrypted)
 			else:
 				if not self.des_key or not self.iv:
 					return cleartext
 				cipher = TDES(self.des_key, MODE_CBC, self.iv[:8])
 				cleartext = cipher.decrypt(encrypted)
 		return cleartext
```

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/lsa_template_nt5.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/lsa_template_nt5.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/lsa_template_nt6.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/lsa_template_nt6.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 						template = templates['nt6']['x64']['7']
 				else:
 					template = templates['nt6']['x64']['4']
 			
 			elif sysinfo.buildnumber < WindowsBuild.WIN_10_1809.value:
 				template = templates['nt6']['x64']['5']
 				
-			elif WindowsBuild.WIN_10_1809.value >= sysinfo.buildnumber < WindowsMinBuild.WIN_11.value:
+			elif WindowsBuild.WIN_10_1809.value <= sysinfo.buildnumber < WindowsMinBuild.WIN_11.value:
 				template = templates['nt6']['x64']['6']
 			else:
 				template = templates['nt6']['x64']['8']
 			
 		else:
 			raise Exception('Missing LSA decrpytor template for Architecture: %s , Build number %s' % (sysinfo.architecture, sysinfo.buildnumber))
 		
@@ -404,22 +404,34 @@
 
 class LSA_x64_8(LsaTemplate_NT6):
 	def __init__(self):
 		LsaTemplate_NT6.__init__(self)
 		self.key_pattern = LSADecyptorKeyPattern()
 		self.key_pattern.signature = b'\x83\x64\x24\x30\x00\x48\x8d\x45\xe0\x44\x8b\x4d\xd8\x48\x8d\x15'
 		self.key_pattern.IV_length = 16
-		#self.key_pattern.offset_to_IV_ptr = 71
 		self.key_pattern.offset_to_IV_ptr = 58
 		self.key_pattern.offset_to_DES_key_ptr = -89
 		self.key_pattern.offset_to_AES_key_ptr = 16
 		
 		self.key_struct = KIWI_BCRYPT_KEY81
 		self.key_handle_struct = KIWI_BCRYPT_HANDLE_KEY
 
+class LSA_x64_9(LsaTemplate_NT6):
+	def __init__(self):
+		LsaTemplate_NT6.__init__(self)
+		self.key_pattern = LSADecyptorKeyPattern()
+		self.key_pattern.signature = b'\x83\x64\x24\x30\x00\x48\x8d\x45\xe0\x44\x8b\x4d\xd8\x48\x8d\x15'
+		self.key_pattern.IV_length = 16
+		self.key_pattern.offset_to_IV_ptr = 71
+		self.key_pattern.offset_to_DES_key_ptr = -89
+		self.key_pattern.offset_to_AES_key_ptr = 16
+		
+		self.key_struct = KIWI_BCRYPT_KEY81
+		self.key_handle_struct = KIWI_BCRYPT_HANDLE_KEY
+
 class LSA_x86_1(LsaTemplate_NT6):
 	def __init__(self):
 		LsaTemplate_NT6.__init__(self)
 		self.key_pattern = LSADecyptorKeyPattern()
 		self.key_pattern.signature = b'\x6a\x02\x6a\x10\x68'
 		self.key_pattern.IV_length = 16
 		self.key_pattern.offset_to_IV_ptr = 5
@@ -516,14 +528,15 @@
 			'2' : LSA_x64_2(),
 			'3' : LSA_x64_3(),
 			'4' : LSA_x64_4(),
 			'5' : LSA_x64_5(),
 			'6' : LSA_x64_6(),
 			'7' : LSA_x64_7(),
 			'8' : LSA_x64_8(),
+			'9' : LSA_x64_9(),
 		},
 		'x86': {
 			'1' : LSA_x86_1(),
 			'2' : LSA_x86_2(),
 			'3' : LSA_x86_3(),
 			'4' : LSA_x86_4(),
 			'5' : LSA_x86_5(),
```

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/lsa_templates.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/lsa_templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/package_commons.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/package_commons.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,26 +98,26 @@
 			await self.reader.move(ptr)
 			data = await self.reader.peek(datasize)
 			await self.reader.move(pos)
 			self.log('%s: %s\n%s' % (name, hex(ptr), hexdump(data, start = ptr)))
 		except Exception as e:
 			self.log('%s: Logging failed for position %s' % (name, hex(ptr)))
 		
-	def decrypt_password(self, enc_password, bytes_expected = False, trim_zeroes = True):
+	def decrypt_password(self, enc_password, bytes_expected = False, trim_zeroes = True, segment_size = 128):
 		"""
 		Common decryption method for LSA encrypted passwords. Result be string or hex encoded bytes (for machine accounts).
 		Also supports bad data, as orphaned credentials may contain actual password OR garbage
 		
 		enc_password: bytes The encrypted password bytes
 		bytes_expected: bool :indication that the result of decryption is bytes, no need for encoding
 		trim_zeroes: bool: if a text is expected then this variable tells wether we should trim the trailing zeroes after decryption
 		"""
 		
 		dec_password = None
-		temp = self.lsa_decryptor.decrypt(enc_password)
+		temp = self.lsa_decryptor.decrypt(enc_password, segment_size=segment_size)
 		if temp and len(temp) > 0:
 			if bytes_expected == False:
 				try: # normal password
 					dec_password = temp.decode('utf-16-le')
 				except: # machine password
 					try:
 						dec_password = temp.decode('utf-8')
```

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/__init__.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/cloudap/decryptor.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/cloudap/decryptor.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,24 +18,27 @@
 		t['credtype'] = self.credtype
 		t['cachedir'] = self.cachedir
 		t['PRT'] = self.PRT
 		t['key_guid'] = self.key_guid
 		t['dpapi_key'] = self.dpapi_key
 		t['dpapi_key_sha1'] = self.dpapi_key_sha1
 		return t
+
+	def get_masterkey_hex(self):
+		return self.dpapi_key.hex() if isinstance(self.dpapi_key, bytes) else self.dpapi_key
 		
 	def to_json(self):
 		return json.dumps(self.to_dict())
 		
 	def __str__(self):
 		t = '\t== Cloudap [%x]==\n' % self.luid
 		t += '\t\tcachedir %s\n' % self.cachedir
 		t += '\t\tPRT %s\n' % self.PRT
 		t += '\t\tkey_guid %s\n' % self.key_guid
-		t += '\t\tdpapi_key %s\n' % self.dpapi_key
+		t += '\t\tdpapi_key %s\n' % self.get_masterkey_hex()
 		t += '\t\tdpapi_key_sha1 %s\n' % self.dpapi_key_sha1
 		return t
 
 class CloudapDecryptor(PackageDecryptor):
 	def __init__(self, reader, decryptor_template, lsa_decryptor, sysinfo):
 		super().__init__('Cloudap', lsa_decryptor, sysinfo, reader)
 		self.decryptor_template = decryptor_template
@@ -54,39 +57,39 @@
 
 			if cloudap_entry.cacheEntry is None or cloudap_entry.cacheEntry.value == 0:
 				return
 			cache = await cloudap_entry.cacheEntry.read(self.reader)
 			cred.cachedir = cache.toname.decode('utf-16-le').replace('\x00','')
 			if cache.cbPRT != 0 and cache.PRT.value != 0:
 				ptr_enc = await cache.PRT.read_raw(self.reader, cache.cbPRT)
-				temp, raw_dec = self.decrypt_password(ptr_enc, bytes_expected=True)
+				temp, raw_dec = self.decrypt_password(ptr_enc, bytes_expected=True, segment_size=8)
 				try:
 					temp = temp.decode()
 				except:
 					pass
 				
-				cred.PRT = temp
+				cred.PRT = str(temp)
 				
 			if cache.toDetermine != 0:
 				unk = await cache.toDetermine.read(self.reader)
 				if unk is not None:
-					cred.key_guid = unk.guid.value
-					cred.dpapi_key, raw_dec = self.decrypt_password(unk.unk)
-					cred.dpapi_key_sha1 = hashlib.sha1(bytes.fromhex(cred.dpapi_key)).hexdigest()
+					cred.key_guid = unk.guid
+					cred.dpapi_key, raw_dec = self.decrypt_password(unk.unk, bytes_expected = True)
+					cred.dpapi_key_sha1 = hashlib.sha1(cred.dpapi_key).hexdigest()
 
 			if cred.PRT is None and cred.key_guid is None:
 				return
 			self.credentials.append(cred)
 		except Exception as e:
 			self.log('CloudAP entry parsing error! Reason %s' % e)
 			
 	
 	async def start(self):
 		try:
 			entry_ptr_value, entry_ptr_loc = await self.find_first_entry()
 		except Exception as e:
-			self.log('Failed to find structs! Reason: %s' % e)
+			self.log('Failed to find list entry! Reason: %s' % e)
 			return
 		
 		await self.reader.move(entry_ptr_loc)
-		entry_ptr = await self.decryptor_template.list_entry(self.reader)
+		entry_ptr = await self.decryptor_template.list_entry.load(self.reader)
 		await self.walk_list(entry_ptr, self.add_entry)
```

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/cloudap/templates.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/cloudap/templates.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 	@staticmethod
 	def get_template(sysinfo):
 		template = CloudapTemplate()
 		if sysinfo.buildnumber <= WindowsBuild.WIN_10_1903.value:
 			return None
 
 		if sysinfo.architecture == KatzSystemArchitecture.X64:
-			template.signature = b'\x44\x8b\x01\x44\x39\x42\x18\x75'
+			template.signature = b'\x44\x8b\x01\x44\x39\x42'
 			template.first_entry_offset = -9
 			template.list_entry = PKIWI_CLOUDAP_LOGON_LIST_ENTRY
+			if sysinfo.buildnumber > WindowsBuild.WIN_10_1903.value:
+				template.list_entry = PKIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2
 		
 		elif sysinfo.architecture == KatzSystemArchitecture.X86:
 			template.signature = b'\x8b\x31\x39\x72\x10\x75'
 			template.first_entry_offset = -8
 			template.list_entry = PKIWI_CLOUDAP_LOGON_LIST_ENTRY
 
 		else:
@@ -128,15 +130,15 @@
 		res.Sid = await PSID.loadvalue(reader)
 		res.unk10 = await DWORD.load(reader)
 		res.unk11 = await DWORD.load(reader)
 		res.unk12 = await DWORD.load(reader)
 		res.unk13 = await DWORD.load(reader)
 		res.toDetermine = await PKIWI_CLOUDAP_CACHE_UNK.load(reader)
 		res.unk14 = await PVOID.load(reader)
-		res.cbPRT = await DWORD.load(reader)
+		res.cbPRT = await DWORD.loadvalue(reader)
 		await reader.align()
 		res.PRT = await PVOID.load(reader) #PBYTE(reader)
 		return res
 
 class PKIWI_CLOUDAP_LOGON_LIST_ENTRY(POINTER):
 	def __init__(self):
 		super().__init__()
@@ -167,8 +169,49 @@
 		res.Blink = await PKIWI_CLOUDAP_LOGON_LIST_ENTRY.load(reader)
 		res.unk0 = await DWORD.load(reader)
 		res.unk1 = await DWORD.load(reader)
 		res.LocallyUniqueIdentifier = await LUID.loadvalue(reader)
 		res.unk2 = await DWORD64.load(reader)
 		res.unk3 = await DWORD64.load(reader)
 		res.cacheEntry = await PKIWI_CLOUDAP_CACHE_LIST_ENTRY.load(reader)
+		return res
+
+class PKIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2(POINTER):
+	def __init__(self):
+		super().__init__()
+	
+	@staticmethod
+	async def load(reader):
+		p = PKIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2()
+		p.location = reader.tell()
+		p.value = await reader.read_uint()
+		p.finaltype = KIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2
+		return p
+
+class KIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2:
+	def __init__(self):
+		self.Flink = None
+		self.Blink = None
+		self.unk0 = None
+		self.unk1 = None
+		self.unk2 = None
+		self.LocallyUniqueIdentifier = None
+		self.unk3 = None
+		self.unk4 = None
+		self.unk5 = None
+		self.cacheEntry = None
+	
+	@staticmethod
+	async def load(reader):
+		res = KIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2()
+		res.Flink = await PKIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2.load(reader)
+		res.Blink = await PKIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2.load(reader)
+		res.unk0 = await DWORD.load(reader)
+		res.unk1 = await DWORD.load(reader)
+		res.unk2 = await DWORD.load(reader)
+		res.LocallyUniqueIdentifier = await LUID.loadvalue(reader)
+		res.unk3 = await DWORD.load(reader)
+		await reader.align()
+		res.unk4 = await DWORD64.load(reader)
+		res.unk5 = await DWORD64.load(reader)
+		res.cacheEntry = await PKIWI_CLOUDAP_CACHE_LIST_ENTRY.load(reader)
 		return res
```

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/credman/templates.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/credman/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/dpapi/decryptor.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/dpapi/decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/dpapi/templates.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/dpapi/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/kerberos/decryptor.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/kerberos/decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/kerberos/templates.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/kerberos/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/livessp/decryptor.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/livessp/decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/livessp/templates.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/livessp/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/msv/decryptor.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/msv/decryptor.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 		t['wdigest_creds']  = []
 		t['ssp_creds']  = []
 		t['livessp_creds']  = []
 		t['dpapi_creds']  = []
 		t['kerberos_creds']  = []
 		t['credman_creds']  = []
 		t['tspkg_creds']  = []
+		t['cloudap_creds'] = []
 		for cred in self.msv_creds:
 			t['msv_creds'].append(cred.to_dict())
 		for cred in self.wdigest_creds:
 			t['wdigest_creds'].append(cred.to_dict())
 		for cred in self.ssp_creds:
 			t['ssp_creds'].append(cred.to_dict())
 		for cred in self.livessp_creds:
@@ -151,14 +152,16 @@
 			t['dpapi_creds'].append(cred.to_dict())
 		for cred in self.kerberos_creds:
 			t['kerberos_creds'].append(cred.to_dict())
 		for cred in self.credman_creds:
 			t['credman_creds'].append(cred.to_dict())
 		for cred in self.tspkg_creds:
 			t['tspkg_creds'].append(cred.to_dict())
+		for cred in self.cloudap_creds:
+			t['cloudap_creds'].append(cred.to_dict())
 		return t
 		
 	def to_json(self):
 		return json.dumps(self.to_dict(), cls=UniversalEncoder)
 	
 	def __str__(self):
 		t = '== LogonSession ==\n'
@@ -193,14 +196,17 @@
 				t+= str(cred)
 		if len(self.tspkg_creds) > 0:
 			for cred in self.tspkg_creds:
 				t+= str(cred)
 		if len(self.dpapi_creds) > 0:
 			for cred in self.dpapi_creds:
 				t+= str(cred)
+		if len(self.cloudap_creds) > 0:
+			for cred in self.cloudap_creds:
+				t+= str(cred)
 		return t
 
 	def to_row(self):
 		for cred in self.msv_creds:
 			t = cred.to_dict()
 			yield [self.luid, 'msv', self.session_id, self.sid, 'msv', '', self.domainname, self.username, 'NT', t['NThash'].hex() if t['NThash'] else '']
 			yield [self.luid, 'msv', self.session_id, self.sid, 'msv', '', self.domainname, self.username, 'LM', t['LMHash'].hex() if t['LMHash'] else '']
@@ -223,14 +229,20 @@
 			yield [self.luid, t['credtype'], self.session_id, self.sid, t['credtype'], '', self.domainname, self.username, 'plaintext', t['password']]
 		for cred in self.credman_creds:
 			t = cred.to_dict()
 			yield [self.luid, t['credtype'], self.session_id, self.sid, t['credtype'], '', self.domainname, self.username, 'plaintext', t['password']]
 		for cred in self.tspkg_creds:
 			t = cred.to_dict()
 			yield [self.luid, t['credtype'], self.session_id, self.sid, t['credtype'], '', self.domainname, self.username, 'plaintext', t['password']]
+		for cred in self.cloudap_creds:
+			t = cred.to_dict()
+			yield [self.luid, t['credtype'], self.session_id, self.sid, t['credtype'], '', self.domainname, self.username, 'masterkey', str(cred.get_masterkey_hex())]
+			yield [self.luid, t['credtype'], self.session_id, self.sid, t['credtype'], '', self.domainname, self.username, 'sha1', str(t['dpapi_key_sha1'])]
+			yield [self.luid, t['credtype'], self.session_id, self.sid, t['credtype'], '', self.domainname, self.username, 'PRT', str(t['PRT'])]
+
 
 	def to_grep_rows(self):
 		for cred in self.msv_creds:
 			t = cred.to_dict()
 			yield [
 				'msv', 
 				self.domainname, 
@@ -262,16 +274,15 @@
 		
 		for cred in self.dpapi_creds:
 			t = cred.to_dict()
 			yield [str(t['credtype']), '', '', '', '', '', str(t['masterkey']), str(t['sha1_masterkey']), str(t['key_guid']), '']
 		
 		for cred in self.cloudap_creds:
 			t = cred.to_dict()
-			#print(t)
-			yield [str(t['credtype']), '', '', '', '', '', str(t['dpapi_key']), str(t['dpapi_key_sha1']), str(t['key_guid']), base64.b64encode(str(t['PRT']).encode()).decode()]
+			yield [str(t['credtype']), '', '', '', '', '', str(cred.get_masterkey_hex()), str(t['dpapi_key_sha1']), str(t['key_guid']), str(t['PRT'])]
 
 
 
 		
 		
 class MsvDecryptor(PackageDecryptor):
 	def __init__(self, reader, decryptor_template, lsa_decryptor, credman_template, sysinfo):
```

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/msv/templates.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/msv/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/ssp/decryptor.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/ssp/decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/ssp/templates.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/ssp/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/tspkg/decryptor.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/tspkg/decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/tspkg/templates.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/tspkg/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/wdigest/decryptor.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/wdigest/decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/packages/wdigest/templates.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/packages/wdigest/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/alsadecryptor/win_datatypes.py` & `pypykatz-0.6.8/pypykatz/alsadecryptor/win_datatypes.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/apypykatz.py` & `pypykatz-0.6.8/pypykatz/apypykatz.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/argparsertest.py` & `pypykatz-0.6.8/pypykatz/argparsertest.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/common.py` & `pypykatz-0.6.8/pypykatz/commons/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import traceback
 import enum
 import json
 import datetime
+import base64
 
 from minidump.streams.SystemInfoStream import PROCESSOR_ARCHITECTURE
 
 def geterr(err:Exception):
 	t = str(err) + '\r\n'
 	for line in traceback.format_tb(err.__traceback__):
 		t += line
@@ -495,8 +496,16 @@
 		sysinfo = KatzSystemInfo()
 		sysinfo.architecture = rekallreader.processor_architecture		
 		sysinfo.operating_system = None
 		sysinfo.buildnumber = rekallreader.BuildNumber
 		sysinfo.msv_dll_timestamp = rekallreader.msv_dll_timestamp
 	
 		return sysinfo
-	
+
+
+def base64_decode_url(value: str, bytes_expected=False) -> str:
+	padding = 4 - (len(value) % 4)
+	value = value + ("=" * padding)
+	result = base64.urlsafe_b64decode(value)
+	if bytes_expected is True:
+		return result
+	return result.decode()
```

### Comparing `pypykatz-0.6.6/pypykatz/commons/filetime.py` & `pypykatz-0.6.8/pypykatz/commons/filetime.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/kerberosticket.py` & `pypykatz-0.6.8/pypykatz/commons/kerberosticket.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/local/common/advapi32.py` & `pypykatz-0.6.8/pypykatz/commons/readers/local/common/advapi32.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/local/common/defines.py` & `pypykatz-0.6.8/pypykatz/commons/readers/local/common/defines.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/local/common/fileinfo.py` & `pypykatz-0.6.8/pypykatz/commons/readers/local/common/fileinfo.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/local/common/kernel32.py` & `pypykatz-0.6.8/pypykatz/commons/readers/local/common/kernel32.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/local/common/live_reader_ctypes.py` & `pypykatz-0.6.8/pypykatz/commons/readers/local/common/live_reader_ctypes.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/local/common/privileges.py` & `pypykatz-0.6.8/pypykatz/commons/readers/local/common/privileges.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/local/common/privileges_types.py` & `pypykatz-0.6.8/pypykatz/commons/readers/local/common/privileges_types.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/local/common/psapi.py` & `pypykatz-0.6.8/pypykatz/commons/readers/local/common/psapi.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/local/common/version.py` & `pypykatz-0.6.8/pypykatz/commons/readers/local/common/version.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/local/common/winreg.py` & `pypykatz-0.6.8/pypykatz/commons/readers/local/common/winreg.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/local/live_reader.py` & `pypykatz-0.6.8/pypykatz/commons/readers/local/live_reader.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/local/process.py` & `pypykatz-0.6.8/pypykatz/commons/readers/local/process.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/registry/live/reader.py` & `pypykatz-0.6.8/pypykatz/commons/readers/registry/live/reader.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/rekall/rekallreader.py` & `pypykatz-0.6.8/pypykatz/commons/readers/rekall/rekallreader.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/readers/volatility3/volreader.py` & `pypykatz-0.6.8/pypykatz/commons/readers/volatility3/volreader.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/win_datatypes.py` & `pypykatz-0.6.8/pypykatz/commons/win_datatypes.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/constants.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/constants.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/advapi32.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/advapi32.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/advapi32.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/advapi32.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/defines.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/defines.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/fileinfo.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/fileinfo.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/kernel32.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/kernel32.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/live_reader_ctypes.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/live_reader_ctypes.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/netapi32.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/netapi32.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/netapi32_high.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/netapi32_high.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/ntdll.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/ntdll.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/privileges.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/privileges.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/privileges_types.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/privileges_types.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/psapi.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/psapi.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/version.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/version.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/function_defs/winreg.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/function_defs/winreg.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/local/sid.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/local/sid.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/machine.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/machine.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/commons/winapi/processmanipulator.py` & `pypykatz-0.6.8/pypykatz/commons/winapi/processmanipulator.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/debugfile.py` & `pypykatz-0.6.8/pypykatz/debugfile.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/dpapi/cmdhelper.py` & `pypykatz-0.6.8/pypykatz/dpapi/cmdhelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,18 @@
 		dpapi_wifi_group.add_argument('mkf', help= 'Keyfile generated by the masterkey -o command.')
 		dpapi_wifi_group.add_argument('wifixml', help='WIFI config XML file')
 
 		dpapi_describe_group = dpapi_subparsers.add_parser('describe', help='Print information on given structure')
 		dpapi_describe_group.add_argument('datatype', choices = ['blob', 'masterkey', 'pvk', 'vpol', 'credential'], help= 'Type of structure')
 		dpapi_describe_group.add_argument('data', help='filepath or hex-encoded data')
 
+		dpapi_cloudapkd_group = dpapi_subparsers.add_parser('cloudapkd', help='Decrypt KeyValue structure from CloudAPK')
+		dpapi_cloudapkd_group.add_argument('mkf', help= 'Keyfile generated by the masterkey -o command.')
+		dpapi_cloudapkd_group.add_argument('keyvalue', help='KeyValue string obtained from PRT')
+
 
 	def execute(self, args):
 		if len(self.keywords) > 0 and args.command in self.keywords:
 			self.run(args)
 		
 		if len(self.live_keywords) > 0 and args.command == 'live' and args.module in self.live_keywords:
 			self.run_live(args)
@@ -214,14 +218,18 @@
 			
 			if len(dpapi.masterkeys) == 0 and len(dpapi.backupkeys) == 0:
 				print('Failed to decrypt the masterkeyfile!')
 				return
 
 			dpapi.dump_masterkeys(args.out_file)
 
+		elif args.dapi_module == 'cloudapkd':
+			dpapi.load_masterkeys(args.mkf)
+			plain = dpapi.decrypt_cloudap_key(args.keyvalue)
+			print('Clear key: %s' % plain.hex())
 
 		elif args.dapi_module == 'credential':
 			dpapi.load_masterkeys(args.mkf)
 			cred_blob = dpapi.decrypt_credential_file(args.cred)
 			
 			print(cred_blob.to_text())
```

### Comparing `pypykatz-0.6.6/pypykatz/dpapi/constants.py` & `pypykatz-0.6.8/pypykatz/dpapi/constants.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/dpapi/dpapi.py` & `pypykatz-0.6.8/pypykatz/dpapi/dpapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from pypykatz.dpapi.structures.masterkeyfile import MasterKeyFile
 from pypykatz.dpapi.structures.credentialfile import CredentialFile, CREDENTIAL_BLOB
 from pypykatz.dpapi.structures.blob import DPAPI_BLOB
 from pypykatz.dpapi.structures.vault import VAULT_VCRD, VAULT_VPOL, VAULT_VPOL_KEYS
 from unicrypto.hashlib import md4 as MD4
 from unicrypto.symmetric import AES, MODE_GCM, MODE_CBC
 from winacl.dtyp.wcee.pvkfile import PVKFile
-from pypykatz.commons.common import UniversalEncoder
+from pypykatz.commons.common import UniversalEncoder, base64_decode_url
 
 
 from cryptography.hazmat.primitives.asymmetric.padding import PKCS1v15
 
 
 if platform.system().lower() == 'windows':
 	from pypykatz.commons.winapi.processmanipulator import ProcessManipulator
@@ -847,14 +847,29 @@
 			"HTTP only raw": False, #"false",
 			"SameSite raw": "lax", #"lax",
 			"This domain only": False, #"Valid for subdomains",
 			"This domain only raw": False, #"false",
 			"Store raw": "firefox-default", #"firefox-default",
 			"First Party Domain": "", #""
 		}
+	
+	def decrypt_cloudap_key(self, keyvalue_url_b64):
+		keyvalue = base64_decode_url(keyvalue_url_b64, bytes_expected=True)
+		keyvalue = keyvalue[8:] # skip the first 8 bytes
+		key_blob = DPAPI_BLOB.from_bytes(keyvalue)
+		return self.decrypt_blob(key_blob)
+	
+	def decrypt_cloudapkd_prt(self, PRT):
+		prt_json = json.loads(PRT)
+		keyvalue = prt_json.get('ProofOfPossesionKey',{}).get('KeyValue')
+		if keyvalue is None:
+			raise Exception('KeyValue not found in PRT')
+
+		keyvalue_dec = self.decrypt_cloudap_key(keyvalue)
+		return keyvalue_dec
 
 
 
 # arpparse helper
 def prepare_dpapi_live(methods = [], mkf = None, pkf = None):
 	dpapi = DPAPI()
```

### Comparing `pypykatz-0.6.6/pypykatz/dpapi/extras.py` & `pypykatz-0.6.8/pypykatz/dpapi/extras.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/dpapi/functiondefs/dpapi.py` & `pypykatz-0.6.8/pypykatz/dpapi/functiondefs/dpapi.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/dpapi/structures/blob.py` & `pypykatz-0.6.8/pypykatz/dpapi/structures/blob.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/dpapi/structures/credentialfile.py` & `pypykatz-0.6.8/pypykatz/dpapi/structures/credentialfile.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/dpapi/structures/masterkeyfile.py` & `pypykatz-0.6.8/pypykatz/dpapi/structures/masterkeyfile.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/dpapi/structures/system.py` & `pypykatz-0.6.8/pypykatz/dpapi/structures/system.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/dpapi/structures/vault.py` & `pypykatz-0.6.8/pypykatz/dpapi/structures/vault.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/example/phandle_dll.py` & `pypykatz-0.6.8/pypykatz/example/phandle_dll.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/kerberos/cmdhelper.py` & `pypykatz-0.6.8/pypykatz/kerberos/cmdhelper.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/kerberos/functiondefs/advapi32.py` & `pypykatz-0.6.8/pypykatz/kerberos/functiondefs/advapi32.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/kerberos/functiondefs/asn1structs.py` & `pypykatz-0.6.8/pypykatz/kerberos/functiondefs/asn1structs.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/kerberos/functiondefs/kernel32.py` & `pypykatz-0.6.8/pypykatz/kerberos/functiondefs/kernel32.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/kerberos/functiondefs/netsecapi.py` & `pypykatz-0.6.8/pypykatz/kerberos/functiondefs/netsecapi.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/kerberos/kerberos.py` & `pypykatz-0.6.8/pypykatz/kerberos/kerberos.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/kerberos/kerberoslive.py` & `pypykatz-0.6.8/pypykatz/kerberos/kerberoslive.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/kerberos/kirbiutils.py` & `pypykatz-0.6.8/pypykatz/kerberos/kirbiutils.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/ldap/cmdhelper.py` & `pypykatz-0.6.8/pypykatz/ldap/cmdhelper.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/cmdhelper.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/cmdhelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,21 @@
 				for luid in results[result].logon_sessions:
 					for row in results[result].logon_sessions[luid].to_grep_rows():
 						if hasattr(args, 'directory') and args.directory is not None:
 							row = [result] + row
 						print(':'.join(row))
 				for cred in results[result].orphaned_creds:
 					t = cred.to_dict()
-					if t['credtype'] != 'dpapi':
-						if t['password'] is not None:
+					if t['credtype'] == 'cloudap':
+						x = [str(t['credtype']), '', '', '', '', '', str(cred.get_masterkey_hex()), str(t['dpapi_key_sha1']), str(t['key_guid']), t['PRT']]
+						if hasattr(args, 'directory') and args.directory is not None:
+							x = [result] + x
+						print(':'.join(x))
+					elif t['credtype'] != 'dpapi':
+						if t.get('password', None) is not None and t['password'] is not None:
 							x =  [str(t['credtype']), str(t['domainname']), str(t['username']), '', '', '', '', '', str(t['password'])]
 							if hasattr(args, 'directory') and args.directory is not None:
 								x = [result] + x
 							print(':'.join(x))
 					else:
 						t = cred.to_dict()
 						x = [str(t['credtype']), '', '', '', '', '', str(t['masterkey']), str(t['sha1_masterkey']), str(t['key_guid']), '']
@@ -224,37 +229,38 @@
 				print('[%s] %s' % (filename, sysinfo))
 
 	
 		###### Minidump
 		elif args.cmd == 'minidump':
 			if args.directory:
 				dir_fullpath = os.path.abspath(args.memoryfile)
-				file_pattern = '*.dmp'
-				if args.recursive == True:
-					globdata = os.path.join(dir_fullpath, '**', file_pattern)
-				else:	
-					globdata = os.path.join(dir_fullpath, file_pattern)
-					
-				logger.info('Parsing folder %s' % dir_fullpath)
-				for filename in glob.glob(globdata, recursive=args.recursive):
-					logger.info('Parsing file %s' % filename)
-					try:
-						if args.kerberos_dir is not None and 'all' not in args.packages:
-							args.packages.append('ktickets')
-						mimi = pypykatz.parse_minidump_file(filename, packages=args.packages)
-						results[filename] = mimi
-						if args.halt_on_error == True and len(mimi.errors) > 0:
-							raise Exception('Error in modules!')
-					except Exception as e:
-						files_with_error.append(filename)
-						logger.exception('Error parsing file %s ' % filename)
-						if args.halt_on_error == True:
-							raise e
-						else:
-							pass
+				for file_pattern in ['*.dmp', '*.DMP']:
+					if args.recursive == True:
+						globdata = os.path.join(dir_fullpath, '**', file_pattern)
+					else:	
+						globdata = os.path.join(dir_fullpath, file_pattern)
+						
+					logger.info('Parsing folder %s' % dir_fullpath)
+					for filename in glob.glob(globdata, recursive=args.recursive):
+						logger.info('Parsing file %s' % filename)
+						try:
+							if args.kerberos_dir is not None and 'all' not in args.packages:
+								args.packages.append('ktickets')
+							mimi = pypykatz.parse_minidump_file(filename, packages=args.packages)
+							results[filename] = mimi
+							if args.halt_on_error == True and len(mimi.errors) > 0:
+								print(mimi.errors)
+								raise Exception('Error in modules!')
+						except Exception as e:
+							files_with_error.append(filename)
+							logger.exception('Error parsing file %s ' % filename)
+							if args.halt_on_error == True:
+								raise e
+							else:
+								pass
 					
 			else:
 				logger.info('Parsing file %s' % args.memoryfile)
 				try:
 					if args.kerberos_dir is not None and 'all' not in args.packages:
 						args.packages.append('ktickets')
 					mimi = pypykatz.parse_minidump_file(args.memoryfile, packages=args.packages)
```

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/lsa_decryptor.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/lsa_decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/lsa_decryptor_nt5.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/lsa_decryptor_nt5.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 			self.logger.log('signature not found! %s' % self.decryptor_template.signature.hex())
 			raise Exception('LSA signature not found!')
 			
 		self.log('Found candidates on the following positions: %s' % ' '.join(hex(x) for x in fl))
 		self.log('Selecting first one @ 0x%08x' % fl[0])
 		return fl[0]
 
-	def decrypt(self, encrypted):
+	def decrypt(self, encrypted, segment_size = 128):
 		# TODO: NT version specific, move from here in subclasses.
 		cleartext = b''
 		size = len(encrypted)
 		if size:
 			if (size % 8) != 0:
 				ctx = RC4(self.random_key)
 				cleartext = ctx.decrypt(encrypted)
```

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/lsa_decryptor_nt6.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/lsa_decryptor_nt6.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,27 +84,27 @@
 			self.log('BCRYPT_KEY_DATA\n%s' % hexdump(data, start = ptr_key))
 			kbk = kbhk.ptr_key.read(self.reader, self.decryptor_template.key_struct)
 			self.log('HARD_KEY SIZE: 0x%x' % kbk.size)
 			if kbk.verify():
 				self.log('HARD_KEY data:\n%s' % hexdump(kbk.hardkey.data))
 				return kbk.hardkey.data
 
-	def decrypt(self, encrypted):
+	def decrypt(self, encrypted, segment_size=128):
 		# TODO: NT version specific, move from here in subclasses.
 		cleartext = b''
 		size = len(encrypted)
 		if size:
 			if size % 8:
-				logger.debug('AES-CFB')
+				logger.debug('AES-CFB - %s' % size)
 				if not self.aes_key or not self.iv:
 					return cleartext
-				cipher = AES(self.aes_key, MODE_CFB, IV = self.iv, segment_size=128)
+				cipher = AES(self.aes_key, MODE_CFB, IV = self.iv, segment_size=segment_size)
 				cleartext = cipher.decrypt(encrypted)
 			else:
-				logger.debug('TDES')
+				logger.debug('TDES - size %s' % size)
 				if not self.des_key or not self.iv:
 					return cleartext
 				cipher = TDES(self.des_key, MODE_CBC, self.iv[:8])
 				cleartext = cipher.decrypt(encrypted)
 		return cleartext
 
 	def dump(self):
```

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/lsa_template_nt5.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/lsa_template_nt5.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/lsa_template_nt6.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/lsa_template_nt6.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #  Tamas Jos (@skelsec)
 #
 
 
 from minidump.win_datatypes import ULONG, PVOID, POINTER
 from pypykatz.commons.common import KatzSystemArchitecture, WindowsMinBuild, WindowsBuild
 from pypykatz.lsadecryptor.package_commons import PackageTemplate
+from pypykatz import logger
 
 class LsaTemplate_NT6(PackageTemplate):
 	def __init__(self):
 		super().__init__('LSA Decryptor')
 		self.key_pattern = None
 		self.key_handle_struct = None
 		self.key_struct = None
@@ -37,20 +38,22 @@
 				raise Exception('NT 5 is not yet supported!')
 			elif sysinfo.buildnumber <= WindowsMinBuild.WIN_2K3.value:
 				raise Exception('NT 5 is not yet supported!')
 			else:
 				keys = [x for x in templates['nt6']['x64']]
 				keys.sort(reverse = True)
 				for key in keys:
+					logger.debug('BF: using x64 - %s' % key)
 					yield templates['nt6']['x64'][key]
 		
 		
 	@staticmethod
 	def get_template(sysinfo):
 		template = LsaTemplate_NT6()
+		logger.debug('Buildnumber: %s' % sysinfo.buildnumber)
 		
 		if sysinfo.architecture == KatzSystemArchitecture.X86:
 			if sysinfo.buildnumber <= WindowsMinBuild.WIN_XP.value:
 				raise Exception("Maybe implemented later")
 			
 			elif sysinfo.buildnumber <= WindowsMinBuild.WIN_2K3.value:
 				template.nt_major = '5'
@@ -81,43 +84,50 @@
 				raise Exception("Maybe implemented later")
 			
 			elif sysinfo.buildnumber <= WindowsMinBuild.WIN_2K3.value:
 				raise Exception("Maybe implemented later")
 			
 			elif sysinfo.buildnumber < WindowsMinBuild.WIN_7.value:
 				#vista
+				logger.debug('using x64 - 1')
 				template = templates['nt6']['x64']['1']
 		
 			elif sysinfo.buildnumber < WindowsMinBuild.WIN_8.value:
-				#win 7
+				logger.debug('using x64 - 2')
 				template = templates['nt6']['x64']['2']
 			
 			elif sysinfo.buildnumber < WindowsMinBuild.WIN_10.value:
 				#win 8 and blue
 				if sysinfo.buildnumber < WindowsMinBuild.WIN_BLUE.value:
 					if sysinfo.msv_dll_timestamp < 0x60000000:
+						logger.debug('using x64 - 3')
 						template = templates['nt6']['x64']['3']
 					else:
+						logger.debug('using x64 - 7')
 						template = templates['nt6']['x64']['7']
 				else:
+					logger.debug('using x64 - 4')
 					template = templates['nt6']['x64']['4']
 					#win blue
 			
 			elif sysinfo.buildnumber < WindowsBuild.WIN_10_1809.value:
+				logger.debug('using x64 - 5')
 				template = templates['nt6']['x64']['5']
 				
-			elif WindowsBuild.WIN_10_1809.value >= sysinfo.buildnumber < WindowsMinBuild.WIN_11.value:
+			elif WindowsBuild.WIN_10_1809.value <= sysinfo.buildnumber < WindowsMinBuild.WIN_11.value:
+				logger.debug('using x64 - 6')
 				template = templates['nt6']['x64']['6']
 			else:
+				logger.debug('using x64 - 8')
 				template = templates['nt6']['x64']['8']
 			
 		else:
 			raise Exception('Missing LSA decrpytor template for Architecture: %s , Build number %s' % (sysinfo.architecture, sysinfo.buildnumber))
 		
-
+		
 		template.log_template('key_handle_struct', template.key_handle_struct)
 		template.log_template('key_struct', template.key_struct)
 		template.log_template('hard_key_struct', template.hard_key_struct)
 		
 		return template
 		
 		
@@ -316,22 +326,35 @@
 
 class LSA_x64_8(LsaTemplate_NT6):
 	def __init__(self):
 		LsaTemplate_NT6.__init__(self)
 		self.key_pattern = LSADecyptorKeyPattern()
 		self.key_pattern.signature = b'\x83\x64\x24\x30\x00\x48\x8d\x45\xe0\x44\x8b\x4d\xd8\x48\x8d\x15'
 		self.key_pattern.IV_length = 16
-		#self.key_pattern.offset_to_IV_ptr = 71
 		self.key_pattern.offset_to_IV_ptr = 58
 		self.key_pattern.offset_to_DES_key_ptr = -89
 		self.key_pattern.offset_to_AES_key_ptr = 16
 		
 		self.key_struct = KIWI_BCRYPT_KEY81
 		self.key_handle_struct = KIWI_BCRYPT_HANDLE_KEY
 
+class LSA_x64_9(LsaTemplate_NT6):
+	"""Same as LSA_x64_8 but with a different IV offset"""
+	def __init__(self):
+		LsaTemplate_NT6.__init__(self)
+		self.key_pattern = LSADecyptorKeyPattern()
+		self.key_pattern.signature = b'\x83\x64\x24\x30\x00\x48\x8d\x45\xe0\x44\x8b\x4d\xd8\x48\x8d\x15'
+		self.key_pattern.IV_length = 16
+		self.key_pattern.offset_to_IV_ptr = 71
+		self.key_pattern.offset_to_DES_key_ptr = -89
+		self.key_pattern.offset_to_AES_key_ptr = 16
+		
+		self.key_struct = KIWI_BCRYPT_KEY81
+		self.key_handle_struct = KIWI_BCRYPT_HANDLE_KEY
+
 class LSA_x86_1(LsaTemplate_NT6):
 	def __init__(self):
 		LsaTemplate_NT6.__init__(self)
 		self.key_pattern = LSADecyptorKeyPattern()
 		self.key_pattern.signature = b'\x6a\x02\x6a\x10\x68'
 		self.key_pattern.IV_length = 16
 		self.key_pattern.offset_to_IV_ptr = 5
@@ -429,14 +452,15 @@
 			'2' : LSA_x64_2(),
 			'3' : LSA_x64_3(),
 			'4' : LSA_x64_4(),
 			'5' : LSA_x64_5(),
 			'6' : LSA_x64_6(),
 			'7' : LSA_x64_7(),
 			'8' : LSA_x64_8(),
+			'9' : LSA_x64_9(), #same as 8 but fidderent IV offset
 		},
 		'x86': {
 			'1' : LSA_x86_1(),
 			'2' : LSA_x86_2(),
 			'3' : LSA_x86_3(),
 			'4' : LSA_x86_4(),
 			'5' : LSA_x86_5(),
```

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/lsa_templates.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/lsa_templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/package_commons.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/package_commons.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,26 +100,26 @@
 			self.reader.move(ptr)
 			data = self.reader.peek(datasize)
 			self.reader.move(pos)
 			self.log('%s: %s\n%s' % (name, hex(ptr), hexdump(data, start = ptr)))
 		except Exception as e:
 			self.log('%s: Logging failed for position %s' % (name, hex(ptr)))
 		
-	def decrypt_password(self, enc_password, bytes_expected = False, trim_zeroes = True):
+	def decrypt_password(self, enc_password, bytes_expected = False, trim_zeroes = True, segment_size=128):
 		"""
 		Common decryption method for LSA encrypted passwords. Result be string or hex encoded bytes (for machine accounts).
 		Also supports bad data, as orphaned credentials may contain actual password OR garbage
 		
 		enc_password: bytes The encrypted password bytes
 		bytes_expected: bool :indication that the result of decryption is bytes, no need for encoding
 		trim_zeroes: bool: if a text is expected then this variable tells wether we should trim the trailing zeroes after decryption
 		"""
 		
 		dec_password = None
-		temp = self.lsa_decryptor.decrypt(enc_password)
+		temp = self.lsa_decryptor.decrypt(enc_password, segment_size=segment_size)
 		if temp and len(temp) > 0:
 			if bytes_expected == False:
 				try: # normal password
 					dec_password = temp.decode('utf-16-le')
 				except: # machine password
 					try:
 						dec_password = temp.decode('utf-8')
```

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/__init__.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/cloudap/decryptor.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/cloudap/decryptor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import hashlib
 from pypykatz.lsadecryptor.package_commons import PackageDecryptor
+from pypykatz.dpapi.dpapi import DPAPI
 
 class CloudapCredential:
 	def __init__(self):
 		self.credtype = 'cloudap'
 		self.luid = None
 		self.sid = None
 		self.cachedir = None
@@ -21,21 +22,24 @@
 		t['key_guid'] = self.key_guid
 		t['dpapi_key'] = self.dpapi_key
 		t['dpapi_key_sha1'] = self.dpapi_key_sha1
 		return t
 		
 	def to_json(self):
 		return json.dumps(self.to_dict())
+	
+	def get_masterkey_hex(self):
+		return self.dpapi_key.hex() if isinstance(self.dpapi_key, bytes) else self.dpapi_key
 		
 	def __str__(self):
 		t = '\t== Cloudap [%x]==\n' % self.luid
 		t += '\t\tcachedir %s\n' % self.cachedir
 		t += '\t\tPRT %s\n' % self.PRT
 		t += '\t\tkey_guid %s\n' % self.key_guid
-		t += '\t\tdpapi_key %s\n' % self.dpapi_key
+		t += '\t\tdpapi_key %s\n' % self.get_masterkey_hex()
 		t += '\t\tdpapi_key_sha1 %s\n' % self.dpapi_key_sha1
 		return t
 
 class CloudapDecryptor(PackageDecryptor):
 	def __init__(self, reader, decryptor_template, lsa_decryptor, sysinfo):
 		super().__init__('Cloudap', lsa_decryptor, sysinfo, reader)
 		self.decryptor_template = decryptor_template
@@ -53,31 +57,32 @@
 			cred.luid = cloudap_entry.LocallyUniqueIdentifier
 
 			if cloudap_entry.cacheEntry is None or cloudap_entry.cacheEntry.value == 0:
 				return
 			cache = cloudap_entry.cacheEntry.read(self.reader)
 			cred.cachedir = cache.toname.decode('utf-16-le').replace('\x00','')
 			if cache.cbPRT != 0 and cache.PRT.value != 0:
-				temp, raw_dec = self.decrypt_password(cache.PRT.read_raw(self.reader, cache.cbPRT), bytes_expected=True)
+				temp, raw_dec = self.decrypt_password(cache.PRT.read_raw(self.reader, cache.cbPRT), bytes_expected=True, segment_size=8)
 				try:
 					temp = temp.decode()
 				except:
 					pass
 				
-				cred.PRT = temp
+				cred.PRT = str(temp)
 				
 			if cache.toDetermine != 0:
 				unk = cache.toDetermine.read(self.reader)
 				if unk is not None:
 					cred.key_guid = unk.guid.value
 					cred.dpapi_key, raw_dec = self.decrypt_password(unk.unk, bytes_expected = True)
 					cred.dpapi_key_sha1 = hashlib.sha1(cred.dpapi_key).hexdigest()
 
 			if cred.PRT is None and cred.key_guid is None:
 				return
+			
 			self.credentials.append(cred)
 		except Exception as e:
 			self.log('CloudAP entry parsing error! Reason %s' % e)
 			
 	
 	def start(self):
 		try:
```

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/cloudap/templates.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/cloudap/templates.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 		if sysinfo.buildnumber <= WindowsBuild.WIN_10_1903.value:
 			return None
 
 		if sysinfo.architecture == KatzSystemArchitecture.X64:
 			template.signature = b'\x44\x8b\x01\x44\x39\x42'
 			template.first_entry_offset = -9
 			template.list_entry = PKIWI_CLOUDAP_LOGON_LIST_ENTRY
+			if sysinfo.buildnumber > WindowsBuild.WIN_10_1903.value:
+				template.list_entry = PKIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2
+			
 		
 		elif sysinfo.architecture == KatzSystemArchitecture.X86:
 			template.signature = b'\x8b\x31\x39\x72\x10\x75'
 			template.first_entry_offset = -8
 			template.list_entry = PKIWI_CLOUDAP_LOGON_LIST_ENTRY
 
 		else:
@@ -91,29 +94,25 @@
 		self.unk0 = DWORD(reader)
 		self.unk1 = DWORD(reader)
 		self.LocallyUniqueIdentifier = LUID(reader).value
 		self.unk2 = DWORD64(reader)
 		self.unk3 = DWORD64(reader)
 		self.cacheEntry = PKIWI_CLOUDAP_CACHE_LIST_ENTRY(reader)
 
-
-#### THIS IS FOR TESTING!!!
-class PKIWI_CLOUDAP_LOGON_LIST_ENTRY_11(POINTER):
+class PKIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2(POINTER):
 	def __init__(self, reader):
-		super().__init__(reader, KIWI_CLOUDAP_LOGON_LIST_ENTRY_11)
+		super().__init__(reader, KIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2)
 
-class KIWI_CLOUDAP_LOGON_LIST_ENTRY_11:
+class KIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2:
 	def __init__(self, reader):
-		self.Flink = PKIWI_CLOUDAP_LOGON_LIST_ENTRY_11(reader)
-		self.Blink = PKIWI_CLOUDAP_LOGON_LIST_ENTRY_11(reader)
-		self.LocallyUniqueIdentifier = 1
-		reader.read(8*11)
-		#self.unk0 = DWORD(reader)
-		#self.unk1 = DWORD(reader)
-		#self.unk2 = DWORD(reader)
-		#reader.align()
-		#self.LocallyUniqueIdentifier = LUID(reader).value
-		#self.unk3 = DWORD64(reader)
-		#self.unk4 = DWORD64(reader)
-		#self.unk5 = DWORD64(reader)
-		#self.unk6 = DWORD64(reader)
-		self.cacheEntry = PKIWI_CLOUDAP_CACHE_LIST_ENTRY(reader)
+		self.Flink = PKIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2(reader)
+		self.Blink = PKIWI_CLOUDAP_LOGON_LIST_ENTRY_21H2(reader)
+		self.unk0 = DWORD(reader)
+		self.unk1 = DWORD(reader)
+		self.unk2 = DWORD(reader)
+		#reader.align() #there should be an aloignment here, but it's not???
+		self.LocallyUniqueIdentifier = LUID(reader).value
+		self.unk3 = DWORD(reader)
+		reader.align()
+		self.unk4 = DWORD64(reader)
+		self.unk5 = DWORD64(reader)
+		self.cacheEntry = PKIWI_CLOUDAP_CACHE_LIST_ENTRY(reader)
```

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/credman/templates.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/credman/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/dpapi/decryptor.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/dpapi/decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/dpapi/templates.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/dpapi/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/kerberos/decryptor.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/kerberos/decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/kerberos/templates.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/kerberos/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/livessp/decryptor.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/livessp/decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/livessp/templates.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/livessp/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/msv/decryptor.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/msv/decryptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 		t['wdigest_creds']  = []
 		t['ssp_creds']  = []
 		t['livessp_creds']  = []
 		t['dpapi_creds']  = []
 		t['kerberos_creds']  = []
 		t['credman_creds']  = []
 		t['tspkg_creds']  = []
+		t['cloudap_creds'] = []
 		for cred in self.msv_creds:
 			t['msv_creds'].append(cred.to_dict())
 		for cred in self.wdigest_creds:
 			t['wdigest_creds'].append(cred.to_dict())
 		for cred in self.ssp_creds:
 			t['ssp_creds'].append(cred.to_dict())
 		for cred in self.livessp_creds:
@@ -149,14 +150,16 @@
 			t['dpapi_creds'].append(cred.to_dict())
 		for cred in self.kerberos_creds:
 			t['kerberos_creds'].append(cred.to_dict())
 		for cred in self.credman_creds:
 			t['credman_creds'].append(cred.to_dict())
 		for cred in self.tspkg_creds:
 			t['tspkg_creds'].append(cred.to_dict())
+		for cred in self.cloudap_creds:
+			t['cloudap_creds'].append(cred.to_dict())
 		return t
 		
 	def to_json(self):
 		return json.dumps(self.to_dict(), cls=UniversalEncoder)
 	
 	def __str__(self):
 		t = '== LogonSession ==\n'
@@ -191,14 +194,17 @@
 				t+= str(cred)
 		if len(self.tspkg_creds) > 0:
 			for cred in self.tspkg_creds:
 				t+= str(cred)
 		if len(self.dpapi_creds) > 0:
 			for cred in self.dpapi_creds:
 				t+= str(cred)
+		if len(self.cloudap_creds) > 0:
+			for cred in self.cloudap_creds:
+				t+= str(cred)
 		return t
 
 	def to_row(self):
 		for cred in self.msv_creds:
 			t = cred.to_dict()
 			yield [self.luid, 'msv', self.session_id, self.sid, 'msv', '', self.domainname, self.username, 'NT', t['NThash'].hex() if t['NThash'] else '']
 			yield [self.luid, 'msv', self.session_id, self.sid, 'msv', '', self.domainname, self.username, 'LM', t['LMHash'].hex() if t['LMHash'] else '']
@@ -221,14 +227,19 @@
 			yield [self.luid, t['credtype'], self.session_id, self.sid, t['credtype'], '', self.domainname, self.username, 'plaintext', t['password']]
 		for cred in self.credman_creds:
 			t = cred.to_dict()
 			yield [self.luid, t['credtype'], self.session_id, self.sid, t['credtype'], '', self.domainname, self.username, 'plaintext', t['password']]
 		for cred in self.tspkg_creds:
 			t = cred.to_dict()
 			yield [self.luid, t['credtype'], self.session_id, self.sid, t['credtype'], '', self.domainname, self.username, 'plaintext', t['password']]
+		for cred in self.cloudap_creds:
+			t = cred.to_dict()
+			yield [self.luid, t['credtype'], self.session_id, self.sid, t['credtype'], '', self.domainname, self.username, 'masterkey', str(cred.get_masterkey_hex())]
+			yield [self.luid, t['credtype'], self.session_id, self.sid, t['credtype'], '', self.domainname, self.username, 'sha1', str(t['dpapi_key_sha1'])]
+			yield [self.luid, t['credtype'], self.session_id, self.sid, t['credtype'], '', self.domainname, self.username, 'PRT', str(t['PRT'])]
 
 	def to_grep_rows(self):
 		for cred in self.msv_creds:
 			t = cred.to_dict()
 			yield [
 				'msv', 
 				self.domainname, 
@@ -260,16 +271,15 @@
 		
 		for cred in self.dpapi_creds:
 			t = cred.to_dict()
 			yield [str(t['credtype']), '', '', '', '', '', str(t['masterkey']), str(t['sha1_masterkey']), str(t['key_guid']), '']
 		
 		for cred in self.cloudap_creds:
 			t = cred.to_dict()
-			#print(t)
-			yield [str(t['credtype']), '', '', '', '', '', str(t['dpapi_key']), str(t['dpapi_key_sha1']), str(t['key_guid']), base64.b64encode(str(t['PRT']).encode()).decode()]
+			yield [str(t['credtype']), '', '', '', '', '', str(cred.get_masterkey_hex()), str(t['dpapi_key_sha1']), str(t['key_guid']), str(t['PRT'])]
 
 
 
 		
 		
 class MsvDecryptor(PackageDecryptor):
 	def __init__(self, reader, decryptor_template, lsa_decryptor, credman_template, sysinfo):
```

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/msv/templates.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/msv/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/ssp/decryptor.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/ssp/decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/ssp/templates.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/ssp/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/tspkg/decryptor.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/tspkg/decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/tspkg/templates.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/tspkg/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/wdigest/decryptor.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/wdigest/decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/lsadecryptor/packages/wdigest/templates.py` & `pypykatz-0.6.8/pypykatz/lsadecryptor/packages/wdigest/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/parsers/cmdhelper.py` & `pypykatz-0.6.8/pypykatz/parsers/cmdhelper.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/plugins/pypykatz_rekall.py` & `pypykatz-0.6.8/pypykatz/plugins/pypykatz_rekall.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/pypykatz.py` & `pypykatz-0.6.8/pypykatz/pypykatz.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/rdp/cmdhelper.py` & `pypykatz-0.6.8/pypykatz/rdp/cmdhelper.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/rdp/packages/creds/decryptor.py` & `pypykatz-0.6.8/pypykatz/rdp/packages/creds/decryptor.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/rdp/packages/creds/templates.py` & `pypykatz-0.6.8/pypykatz/rdp/packages/creds/templates.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/rdp/parser.py` & `pypykatz-0.6.8/pypykatz/rdp/parser.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/aoffline_parser.py` & `pypykatz-0.6.8/pypykatz/registry/aoffline_parser.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/cmdhelper.py` & `pypykatz-0.6.8/pypykatz/registry/cmdhelper.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/live_parser.py` & `pypykatz-0.6.8/pypykatz/registry/live_parser.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/offline_parser.py` & `pypykatz-0.6.8/pypykatz/registry/offline_parser.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/sam/asam.py` & `pypykatz-0.6.8/pypykatz/registry/sam/asam.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/sam/common.py` & `pypykatz-0.6.8/pypykatz/registry/sam/common.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/sam/sam.py` & `pypykatz-0.6.8/pypykatz/registry/sam/sam.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/sam/structures.py` & `pypykatz-0.6.8/pypykatz/registry/sam/structures.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/security/acommon.py` & `pypykatz-0.6.8/pypykatz/registry/security/acommon.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/security/asecurity.py` & `pypykatz-0.6.8/pypykatz/registry/security/asecurity.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/security/common.py` & `pypykatz-0.6.8/pypykatz/registry/security/common.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/security/security.py` & `pypykatz-0.6.8/pypykatz/registry/security/security.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/security/structures.py` & `pypykatz-0.6.8/pypykatz/registry/security/structures.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/software/asoftware.py` & `pypykatz-0.6.8/pypykatz/registry/software/asoftware.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/software/software.py` & `pypykatz-0.6.8/pypykatz/registry/software/software.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/system/asystem.py` & `pypykatz-0.6.8/pypykatz/registry/system/asystem.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/registry/system/system.py` & `pypykatz-0.6.8/pypykatz/registry/system/system.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/remote/cmdhelper.py` & `pypykatz-0.6.8/pypykatz/remote/cmdhelper.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/remote/live/localgroup/enumerator.py` & `pypykatz-0.6.8/pypykatz/remote/live/localgroup/enumerator.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/remote/live/session/enumerator.py` & `pypykatz-0.6.8/pypykatz/remote/live/session/enumerator.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/remote/live/share/enumerator.py` & `pypykatz-0.6.8/pypykatz/remote/live/share/enumerator.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/smb/cmdhelper.py` & `pypykatz-0.6.8/pypykatz/smb/cmdhelper.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/smb/dcsync.py` & `pypykatz-0.6.8/pypykatz/smb/dcsync.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/smb/lsassutils.py` & `pypykatz-0.6.8/pypykatz/smb/lsassutils.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/smb/printer.py` & `pypykatz-0.6.8/pypykatz/smb/printer.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/smb/regutils.py` & `pypykatz-0.6.8/pypykatz/smb/regutils.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/smb/shareenum.py` & `pypykatz-0.6.8/pypykatz/smb/shareenum.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/utils/crypto/cmdhelper.py` & `pypykatz-0.6.8/pypykatz/utils/crypto/cmdhelper.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/utils/crypto/gppassword.py` & `pypykatz-0.6.8/pypykatz/utils/crypto/gppassword.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/utils/crypto/ofcdecrypt.py` & `pypykatz-0.6.8/pypykatz/utils/crypto/ofcdecrypt.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz/utils/crypto/winhash.py` & `pypykatz-0.6.8/pypykatz/utils/crypto/winhash.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/pypykatz.egg-info/SOURCES.txt` & `pypykatz-0.6.8/pypykatz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/setup.py` & `pypykatz-0.6.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,22 +47,22 @@
 	python_requires='>=3.6',
 	classifiers=[
 		"Programming Language :: Python :: 3.6",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
 	],
 	install_requires=[
-		'unicrypto>=0.0.10',
-		'minidump>=0.0.21',
-		'minikerberos>=0.4.0',
-		'aiowinreg>=0.0.7',
-		'msldap>=0.4.7',
-		'winacl>=0.1.6',
-		'aiosmb>=0.4.4',
-		'aesedb>=0.1.3',
+		'unicrypto==0.0.10',
+		'minidump==0.0.21',
+		'minikerberos==0.4.1',
+		'aiowinreg==0.0.10',
+		'msldap==0.5.5',
+		'winacl==0.1.7',
+		'aiosmb==0.4.6',
+		'aesedb==0.1.4',
 		'tqdm',
 	],
 	
 	# No more conveinent .exe entry point thanks to some idiot who 
 	# used the code without modification in a state-backed trojan.
 	# Thank you for runing it for everyone.
 	#
```

### Comparing `pypykatz-0.6.6/tests/test_async_lsassdecrypt.py` & `pypykatz-0.6.8/tests/test_async_lsassdecrypt.py`

 * *Files identical despite different names*

### Comparing `pypykatz-0.6.6/tests/test_lsassdecrypt.py` & `pypykatz-0.6.8/tests/test_lsassdecrypt.py`

 * *Files identical despite different names*

