# Comparing `tmp/aiosmb-0.4.4.tar.gz` & `tmp/aiosmb-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosmb-0.4.4.tar", last modified: Tue Dec  6 20:21:23 2022, max compression
+gzip compressed data, was "aiosmb-0.4.6.tar", last modified: Tue May 30 16:04:29 2023, max compression
```

## Comparing `aiosmb-0.4.4.tar` & `aiosmb-0.4.6.tar`

### file list

```diff
@@ -1,267 +1,273 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.260637 aiosmb-0.4.4/
--rw-rw-r--   0 root         (0) root         (0)       26 2021-10-28 11:02:11.000000 aiosmb-0.4.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      373 2022-12-06 20:21:23.260637 aiosmb-0.4.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     6212 2022-03-29 22:04:29.000000 aiosmb-0.4.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.224637 aiosmb-0.4.4/aiosmb/
--rw-rw-r--   0 root         (0) root         (0)      269 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      128 2022-12-06 19:04:18.000000 aiosmb-0.4.4/aiosmb/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.228637 aiosmb-0.4.4/aiosmb/commons/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.228637 aiosmb-0.4.4/aiosmb/commons/connection/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/connection/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4080 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/commons/connection/factory.py
--rw-rw-r--   0 root         (0) root         (0)     1938 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/commons/connection/params.py
--rw-rw-r--   0 root         (0) root         (0)     6449 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/commons/connection/target.py
--rw-rw-r--   0 root         (0) root         (0)     2759 2022-12-03 18:37:37.000000 aiosmb-0.4.4/aiosmb/commons/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.228637 aiosmb-0.4.4/aiosmb/commons/interfaces/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.228637 aiosmb-0.4.4/aiosmb/commons/interfaces/blocking/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/interfaces/blocking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.228637 aiosmb-0.4.4/aiosmb/commons/interfaces/blocking/file/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/interfaces/blocking/file/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3154 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/interfaces/blocking/file/blockingfile.py
--rw-rw-r--   0 root         (0) root         (0)     2881 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/interfaces/blocking/file/file.py
--rw-rw-r--   0 root         (0) root         (0)     2366 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/interfaces/blocking/file/protocol.py
--rw-rw-r--   0 root         (0) root         (0)    14417 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/interfaces/directory.py
--rw-rw-r--   0 root         (0) root         (0)       77 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/interfaces/domain.py
--rw-rw-r--   0 root         (0) root         (0)    16222 2022-12-06 18:50:41.000000 aiosmb-0.4.4/aiosmb/commons/interfaces/file.py
--rw-rw-r--   0 root         (0) root         (0)      144 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/interfaces/localgroup.py
--rw-rw-r--   0 root         (0) root         (0)    31315 2022-12-04 19:58:36.000000 aiosmb-0.4.4/aiosmb/commons/interfaces/machine.py
--rw-rw-r--   0 root         (0) root         (0)      129 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/interfaces/session.py
--rw-rw-r--   0 root         (0) root         (0)     3210 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/interfaces/share.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.228637 aiosmb-0.4.4/aiosmb/commons/scanner/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/scanner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.228637 aiosmb-0.4.4/aiosmb/commons/scanner/common/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/scanner/common/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      340 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/scanner/common/comms.py
--rw-rw-r--   0 root         (0) root         (0)     4614 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/commons/scanner/scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.228637 aiosmb-0.4.4/aiosmb/commons/scanner/scanners/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/scanner/scanners/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.228637 aiosmb-0.4.4/aiosmb/commons/scanner/targetgen/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/scanner/targetgen/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      382 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/scanner/targetgen/filetarget.py
--rw-rw-r--   0 root         (0) root         (0)      482 2022-07-11 20:48:26.000000 aiosmb-0.4.4/aiosmb/commons/scanner/targetgen/listtarget.py
--rw-rw-r--   0 root         (0) root         (0)      155 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/smbcontainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.232637 aiosmb-0.4.4/aiosmb/commons/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1630 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/utils/apq.py
--rw-rw-r--   0 root         (0) root         (0)     3267 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/utils/decorators.py
--rw-rw-r--   0 root         (0) root         (0)      185 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/utils/extb.py
--rw-rw-r--   0 root         (0) root         (0)     1185 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/utils/glob2re.py
--rw-rw-r--   0 root         (0) root         (0)      953 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/utils/hexdump.py
--rw-rw-r--   0 root         (0) root         (0)      526 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/utils/ts2dt.py
--rw-rw-r--   0 root         (0) root         (0)      615 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/commons/utils/univeraljson.py
--rw-rw-r--   0 root         (0) root         (0)    54294 2022-12-06 18:48:57.000000 aiosmb-0.4.4/aiosmb/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.232637 aiosmb-0.4.4/aiosmb/dcerpc/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.236637 aiosmb-0.4.4/aiosmb/dcerpc/v5/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4775 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/bkrp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.236637 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.240637 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/connection/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/connection/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1117 2022-09-09 14:41:04.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/connection/authentication.py
--rw-rw-r--   0 root         (0) root         (0)     1492 2022-08-07 11:46:38.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/connection/connectionstring.py
--rw-rw-r--   0 root         (0) root         (0)     1108 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/connection/smbdcefactory.py
--rw-rw-r--   0 root         (0) root         (0)     5956 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/connection/target.py
--rw-rw-r--   0 root         (0) root         (0)     4956 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.240637 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/even6/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/even6/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    16568 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/even6/binxml.py
--rw-rw-r--   0 root         (0) root         (0)     1258 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/even6/resultset.py
--rw-rw-r--   0 root         (0) root         (0)     1891 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/secrets.py
--rw-rw-r--   0 root         (0) root         (0)      551 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/common/service.py
--rw-rw-r--   0 root         (0) root         (0)    25877 2022-10-05 20:41:05.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/connection.py
--rw-rw-r--   0 root         (0) root         (0)    39411 2022-03-15 07:57:51.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/drsuapi.py
--rw-rw-r--   0 root         (0) root         (0)    12950 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/dtypes.py
--rw-rw-r--   0 root         (0) root         (0)    27891 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/enum.py
--rw-rw-r--   0 root         (0) root         (0)    85380 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/epm.py
--rw-rw-r--   0 root         (0) root         (0)    11154 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/even.py
--rw-rw-r--   0 root         (0) root         (0)     8561 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/even6.py
--rw-rw-r--   0 root         (0) root         (0)   588944 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/hresult_errors.py
--rw-rw-r--   0 root         (0) root         (0)     4174 2022-01-10 19:05:50.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/icpr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.240637 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3367 2022-09-08 21:43:22.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/bkrp.py
--rw-rw-r--   0 root         (0) root         (0)    18418 2022-12-04 19:18:46.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/drsuapimgr.py
--rw-rw-r--   0 root         (0) root         (0)     9344 2022-09-12 21:52:19.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/endpointmgr.py
--rw-rw-r--   0 root         (0) root         (0)     4781 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/even6.py
--rw-rw-r--   0 root         (0) root         (0)     3904 2022-01-10 19:05:50.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/icprmgr.py
--rw-rw-r--   0 root         (0) root         (0)     8600 2022-09-13 10:33:50.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/lsatmgr.py
--rw-rw-r--   0 root         (0) root         (0)     6647 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/parmgr.py
--rw-rw-r--   0 root         (0) root         (0)    19794 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/remoteregistry.py
--rw-rw-r--   0 root         (0) root         (0)     7154 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/rprnmgr.py
--rw-rw-r--   0 root         (0) root         (0)    10536 2022-12-04 19:18:41.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/samrmgr.py
--rw-rw-r--   0 root         (0) root         (0)     9538 2022-12-04 19:18:32.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/servicemanager.py
--rw-rw-r--   0 root         (0) root         (0)     4362 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/srvsmgr.py
--rw-rw-r--   0 root         (0) root         (0)     8058 2021-11-01 23:36:41.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/tschmgr.py
--rw-rw-r--   0 root         (0) root         (0)     3335 2022-05-30 13:44:50.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/wkstmgr.py
--rw-rw-r--   0 root         (0) root         (0)    58858 2022-12-04 19:19:52.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/lsad.py
--rw-rw-r--   0 root         (0) root         (0)    15737 2022-12-04 19:19:41.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/lsat.py
--rw-rw-r--   0 root         (0) root         (0)    68997 2022-08-06 19:03:51.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/ndr.py
--rw-rw-r--   0 root         (0) root         (0)    84967 2022-03-13 13:30:41.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/nrpc.py
--rw-rw-r--   0 root         (0) root         (0)    19168 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/par.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.240637 aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.240637 aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3957 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/bind.py
--rw-rw-r--   0 root         (0) root         (0)     4619 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/bindack.py
--rw-rw-r--   0 root         (0) root         (0)     3058 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/bindnack.py
--rw-rw-r--   0 root         (0) root         (0)     1530 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/cancel.py
--rw-rw-r--   0 root         (0) root         (0)      596 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/commons.py
--rw-rw-r--   0 root         (0) root         (0)      554 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/constants.py
--rw-rw-r--   0 root         (0) root         (0)    29303 2022-12-04 18:59:16.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/rpcrt.py
--rw-rw-r--   0 root         (0) root         (0)    26617 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/rprn.py
--rw-rw-r--   0 root         (0) root         (0)    29227 2022-12-04 19:19:35.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/rrp.py
--rw-rw-r--   0 root         (0) root         (0)    86812 2022-12-04 19:19:30.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/samr.py
--rw-rw-r--   0 root         (0) root         (0)    41114 2022-12-04 19:32:19.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/scmr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.244637 aiosmb-0.4.4/aiosmb/dcerpc/v5/servers/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/servers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      400 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/servers/srvsvc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.244637 aiosmb-0.4.4/aiosmb/dcerpc/v5/servers/transport/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/servers/transport/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1150 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/servers/transport/smbtransport.py
--rw-rw-r--   0 root         (0) root         (0)    90286 2022-12-04 19:18:57.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/srvs.py
--rw-rw-r--   0 root         (0) root         (0)    22439 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/structure.py
--rw-rw-r--   0 root         (0) root         (0)   578104 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/system_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.244637 aiosmb-0.4.4/aiosmb/dcerpc/v5/transport/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/transport/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1963 2022-12-04 19:11:41.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/transport/smb.py
--rw-rw-r--   0 root         (0) root         (0)     2159 2022-12-04 19:10:59.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/transport/tcp.py
--rw-rw-r--   0 root         (0) root         (0)    21930 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/tsch.py
--rw-rw-r--   0 root         (0) root         (0)     2669 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/uuid.py
--rw-rw-r--   0 root         (0) root         (0)    35040 2022-12-04 19:18:53.000000 aiosmb-0.4.4/aiosmb/dcerpc/v5/wkst.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.244637 aiosmb-0.4.4/aiosmb/examples/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/examples/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3104 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/examples/epmtest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.244637 aiosmb-0.4.4/aiosmb/examples/scancommons/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/examples/scancommons/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      603 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/examples/scancommons/internal.py
--rw-rw-r--   0 root         (0) root         (0)      978 2021-10-29 20:22:08.000000 aiosmb-0.4.4/aiosmb/examples/scancommons/targetgens.py
--rw-rw-r--   0 root         (0) root         (0)      328 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/examples/scancommons/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.248637 aiosmb-0.4.4/aiosmb/examples/scanners/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/scanners/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3341 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/scanners/__main__.py
--rw-rw-r--   0 root         (0) root         (0)     2061 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/scanners/smbadmin.py
--rw-rw-r--   0 root         (0) root         (0)     3297 2022-11-28 23:10:31.000000 aiosmb-0.4.4/aiosmb/examples/scanners/smbfile.py
--rw-rw-r--   0 root         (0) root         (0)      943 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/scanners/smbfinger.py
--rw-rw-r--   0 root         (0) root         (0)     1040 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/scanners/smbiface.py
--rw-rw-r--   0 root         (0) root         (0)     1717 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/scanners/smbprintnightmare.py
--rw-rw-r--   0 root         (0) root         (0)     1324 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/scanners/smbproto.py
--rw-rw-r--   0 root         (0) root         (0)     1081 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/scanners/smbsession.py
--rw-rw-r--   0 root         (0) root         (0)     6766 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/smbcertreq.py
--rw-rw-r--   0 root         (0) root         (0)    36977 2022-12-04 15:41:51.000000 aiosmb-0.4.4/aiosmb/examples/smbclient.py
--rw-rw-r--   0 root         (0) root         (0)     1982 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/smbeventq.py
--rw-rw-r--   0 root         (0) root         (0)     4816 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/smbget.py
--rw-rw-r--   0 root         (0) root         (0)     1869 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/smbgetfile.py
--rw-rw-r--   0 root         (0) root         (0)     1879 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/examples/smbpathcompleter.py
--rw-rw-r--   0 root         (0) root         (0)     3682 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/smbreg.py
--rw-rw-r--   0 root         (0) root         (0)    15687 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/smbshareenum.py
--rw-rw-r--   0 root         (0) root         (0)      616 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/smbsharelist.py
--rw-rw-r--   0 root         (0) root         (0)     6334 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/examples/zl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.248637 aiosmb-0.4.4/aiosmb/external/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/external/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.248637 aiosmb-0.4.4/aiosmb/external/aiocmd/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/external/aiocmd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.248637 aiosmb-0.4.4/aiosmb/external/aiocmd/aiocmd/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/external/aiocmd/aiocmd/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6197 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/external/aiocmd/aiocmd/aiocmd.py
--rw-rw-r--   0 root         (0) root         (0)     3688 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/external/aiocmd/aiocmd/nested_completer.py
--rw-rw-r--   0 root         (0) root         (0)      718 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/external/aiocmd/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.248637 aiosmb-0.4.4/aiosmb/external/asciitree/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/external/asciitree/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.248637 aiosmb-0.4.4/aiosmb/external/asciitree/asciitree/
--rw-rw-r--   0 root         (0) root         (0)     2499 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/external/asciitree/asciitree/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2909 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/external/asciitree/asciitree/drawing.py
--rw-rw-r--   0 root         (0) root         (0)     1142 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/external/asciitree/asciitree/traversal.py
--rw-rw-r--   0 root         (0) root         (0)      136 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/external/asciitree/asciitree/util.py
--rw-rw-r--   0 root         (0) root         (0)      529 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/external/asciitree/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.248637 aiosmb-0.4.4/aiosmb/protocol/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1159 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.248637 aiosmb-0.4.4/aiosmb/protocol/compression/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/compression/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5422 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/compression/lznt1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.248637 aiosmb-0.4.4/aiosmb/protocol/crypto/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-13 13:16:07.000000 aiosmb-0.4.4/aiosmb/protocol/crypto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-20 12:59:03.000000 aiosmb-0.4.4/aiosmb/protocol/crypto/from_impacket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.248637 aiosmb-0.4.4/aiosmb/protocol/smb/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2331 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb/command_codes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.252637 aiosmb-0.4.4/aiosmb/protocol/smb/commands/
--rw-rw-r--   0 root         (0) root         (0)      278 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3565 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb/commands/negotiate.py
--rw-rw-r--   0 root         (0) root         (0)      835 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb/commons.py
--rw-rw-r--   0 root         (0) root         (0)     4600 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb/header.py
--rw-rw-r--   0 root         (0) root         (0)     1124 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.252637 aiosmb-0.4.4/aiosmb/protocol/smb2/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      593 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/command_codes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.252637 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/
--rw-rw-r--   0 root         (0) root         (0)     2483 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      858 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/cancel.py
--rw-rw-r--   0 root         (0) root         (0)     3805 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/close.py
--rw-rw-r--   0 root         (0) root         (0)    17789 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/create.py
--rw-rw-r--   0 root         (0) root         (0)     1680 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/echo.py
--rw-rw-r--   0 root         (0) root         (0)     1345 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/error.py
--rw-rw-r--   0 root         (0) root         (0)     2045 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/flush.py
--rw-rw-r--   0 root         (0) root         (0)    13635 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/ioctl.py
--rw-rw-r--   0 root         (0) root         (0)     1696 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/logoff.py
--rw-rw-r--   0 root         (0) root         (0)    23612 2022-03-20 10:20:56.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/negotiate.py
--rw-rw-r--   0 root         (0) root         (0)     4684 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/query_directory.py
--rw-rw-r--   0 root         (0) root         (0)     6149 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/query_info.py
--rw-rw-r--   0 root         (0) root         (0)     6696 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/read.py
--rw-rw-r--   0 root         (0) root         (0)     5325 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/sessionsetup.py
--rw-rw-r--   0 root         (0) root         (0)     7973 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/tree_connect.py
--rw-rw-r--   0 root         (0) root         (0)     1768 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/tree_disconnect.py
--rw-rw-r--   0 root         (0) root         (0)     5364 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/commands/write.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/header.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.256637 aiosmb-0.4.4/aiosmb/protocol/smb2/headers/
--rw-rw-r--   0 root         (0) root         (0)      382 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/headers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3599 2022-08-04 18:44:29.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/headers/asynch.py
--rw-rw-r--   0 root         (0) root         (0)     1102 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/headers/common.py
--rw-rw-r--   0 root         (0) root         (0)     1848 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/headers/compression.py
--rw-rw-r--   0 root         (0) root         (0)     3525 2022-12-06 10:52:10.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/headers/sync.py
--rw-rw-r--   0 root         (0) root         (0)     1421 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/headers/transform.py
--rw-rw-r--   0 root         (0) root         (0)     4687 2022-12-06 10:49:27.000000 aiosmb-0.4.4/aiosmb/protocol/smb2/message.py
--rw-rw-r--   0 root         (0) root         (0)    46916 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/serverconnection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.256637 aiosmb-0.4.4/aiosmb/transport/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/transport/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1523 2022-09-09 16:00:00.000000 aiosmb-0.4.4/aiosmb/transport/netbios.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.256637 aiosmb-0.4.4/aiosmb/wintypes/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6080 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/access_mask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.256637 aiosmb-0.4.4/aiosmb/wintypes/dtyp/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/dtyp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.256637 aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      347 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/access_mask.py
--rw-rw-r--   0 root         (0) root         (0)    18185 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/ace.py
--rw-rw-r--   0 root         (0) root         (0)      852 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/acl.py
--rw-rw-r--   0 root         (0) root         (0)     1233 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/guid.py
--rw-rw-r--   0 root         (0) root         (0)     6709 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/security_descriptor.py
--rw-rw-r--   0 root         (0) root         (0)     1081 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/security_information.py
--rw-rw-r--   0 root         (0) root         (0)     8490 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/sid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.256637 aiosmb-0.4.4/aiosmb/wintypes/dtyp/structures/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/dtyp/structures/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1158 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/dtyp/structures/filetime.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.256637 aiosmb-0.4.4/aiosmb/wintypes/fscc/
--rw-rw-r--   0 root         (0) root         (0)     3075 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/fscc/FileAttributes.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/fscc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.260637 aiosmb-0.4.4/aiosmb/wintypes/fscc/structures/
--rw-rw-r--   0 root         (0) root         (0)     2439 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/fscc/structures/FileFullDirectoryInformation.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/fscc/structures/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1898 2021-10-28 11:02:11.000000 aiosmb-0.4.4/aiosmb/wintypes/fscc/structures/fileinfoclass.py
--rw-rw-r--   0 root         (0) root         (0)    71052 2022-08-29 22:16:44.000000 aiosmb-0.4.4/aiosmb/wintypes/ntstatus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 20:21:23.228637 aiosmb-0.4.4/aiosmb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      373 2022-12-06 20:21:23.000000 aiosmb-0.4.4/aiosmb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7987 2022-12-06 20:21:23.000000 aiosmb-0.4.4/aiosmb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-06 20:21:23.000000 aiosmb-0.4.4/aiosmb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      257 2022-12-06 20:21:23.000000 aiosmb-0.4.4/aiosmb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-06 20:21:23.000000 aiosmb-0.4.4/aiosmb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      141 2022-12-06 20:21:23.000000 aiosmb-0.4.4/aiosmb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-12-06 20:21:23.000000 aiosmb-0.4.4/aiosmb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-06 20:21:23.260637 aiosmb-0.4.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1555 2022-11-26 21:08:30.000000 aiosmb-0.4.4/setup.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.151470 aiosmb-0.4.6/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       26 2023-03-05 19:48:31.000000 aiosmb-0.4.6/MANIFEST.in
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      373 2023-05-30 16:04:29.151470 aiosmb-0.4.6/PKG-INFO
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6212 2023-03-05 19:48:31.000000 aiosmb-0.4.6/README.md
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:28.939469 aiosmb-0.4.6/aiosmb/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      269 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      128 2023-04-15 10:44:41.000000 aiosmb-0.4.6/aiosmb/_version.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:28.963469 aiosmb-0.4.6/aiosmb/commons/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:28.967469 aiosmb-0.4.6/aiosmb/commons/connection/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/connection/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7019 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/connection/factory.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1938 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/connection/params.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6449 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/connection/target.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2759 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/exceptions.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:28.979469 aiosmb-0.4.6/aiosmb/commons/interfaces/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/interfaces/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:28.979469 aiosmb-0.4.6/aiosmb/commons/interfaces/blocking/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/interfaces/blocking/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:28.983469 aiosmb-0.4.6/aiosmb/commons/interfaces/blocking/file/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/interfaces/blocking/file/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3154 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/interfaces/blocking/file/blockingfile.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2881 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/interfaces/blocking/file/file.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2366 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/interfaces/blocking/file/protocol.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    20257 2023-04-07 18:20:43.000000 aiosmb-0.4.6/aiosmb/commons/interfaces/directory.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       77 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/interfaces/domain.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    20289 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/interfaces/file.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      144 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/interfaces/localgroup.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    33640 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/interfaces/machine.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      129 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/interfaces/session.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3210 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/interfaces/share.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:28.987469 aiosmb-0.4.6/aiosmb/commons/scanner/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/scanner/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:28.987469 aiosmb-0.4.6/aiosmb/commons/scanner/common/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/scanner/common/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      340 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/scanner/common/comms.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4614 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/scanner/scanner.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:28.987469 aiosmb-0.4.6/aiosmb/commons/scanner/scanners/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/scanner/scanners/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:28.995469 aiosmb-0.4.6/aiosmb/commons/scanner/targetgen/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/scanner/targetgen/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      382 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/scanner/targetgen/filetarget.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      482 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/scanner/targetgen/listtarget.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      155 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/smbcontainer.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:28.999469 aiosmb-0.4.6/aiosmb/commons/utils/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/utils/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1630 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/utils/apq.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3267 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/utils/decorators.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      185 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/utils/extb.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1185 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/utils/glob2re.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      953 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/utils/hexdump.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      526 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/utils/ts2dt.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      615 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/commons/utils/univeraljson.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    54328 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/connection.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:28.999469 aiosmb-0.4.6/aiosmb/dcerpc/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.031469 aiosmb-0.4.6/aiosmb/dcerpc/v5/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4775 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/bkrp.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.035469 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.051469 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/connection/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/connection/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1117 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/connection/authentication.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1492 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/connection/connectionstring.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1108 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/connection/smbdcefactory.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6812 2023-04-13 13:37:54.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/connection/target.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4686 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/domain.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.051469 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/even6/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/even6/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    16568 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/even6/binxml.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1258 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/even6/resultset.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1891 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/secrets.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      551 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/common/service.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    25877 2023-04-18 13:58:14.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/connection.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    39411 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/drsuapi.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    12950 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/dtypes.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    27891 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/enum.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    85380 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/epm.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    11154 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/even.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8561 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/even6.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7653 2023-04-18 21:01:00.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/gkdi.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)   588944 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/hresult_errors.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4174 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/icpr.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.051469 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3367 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/bkrp.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    18508 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/drsuapimgr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     9761 2023-04-13 13:37:38.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/endpointmgr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4781 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/even6.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6045 2023-04-19 09:39:57.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/gkdimgr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3904 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/icprmgr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8600 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/lsatmgr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6647 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/parmgr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    19794 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/remoteregistry.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7154 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/rprnmgr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    10536 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/samrmgr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     9538 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/servicemanager.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4362 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/srvsmgr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6927 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/tschmgr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3335 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/wkstmgr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    58858 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/lsad.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    15737 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/lsat.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    68997 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/ndr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    84967 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/nrpc.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    19168 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/par.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.051469 aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.063470 aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3957 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/bind.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4619 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/bindack.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3058 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/bindnack.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1530 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/cancel.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      596 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/commons.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      554 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/constants.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    29303 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/rpcrt.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    26617 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/rprn.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    29227 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/rrp.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    86812 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/samr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    41114 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/scmr.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.063470 aiosmb-0.4.6/aiosmb/dcerpc/v5/servers/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/servers/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      400 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/servers/srvsvc.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.063470 aiosmb-0.4.6/aiosmb/dcerpc/v5/servers/transport/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/servers/transport/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1150 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/servers/transport/smbtransport.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    90286 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/srvs.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    22439 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/structure.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)   578104 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/system_errors.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.079470 aiosmb-0.4.6/aiosmb/dcerpc/v5/transport/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/transport/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1963 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/transport/smb.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2159 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/transport/tcp.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    21930 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/tsch.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2669 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/uuid.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    35040 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/dcerpc/v5/wkst.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.103470 aiosmb-0.4.6/aiosmb/examples/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2994 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/epmtest.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.103470 aiosmb-0.4.6/aiosmb/examples/scancommons/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/scancommons/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      603 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/scancommons/internal.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      978 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/scancommons/targetgens.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      328 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/scancommons/utils.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.103470 aiosmb-0.4.6/aiosmb/examples/scanners/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/scanners/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3659 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/scanners/__main__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2061 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/scanners/smbadmin.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3297 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/scanners/smbfile.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      943 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/scanners/smbfinger.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1040 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/scanners/smbiface.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1717 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/scanners/smbprintnightmare.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1324 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/scanners/smbproto.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1081 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/scanners/smbsession.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6654 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/smbcertreq.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    37060 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/smbclient.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1982 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/smbeventq.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4816 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/smbget.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1869 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/smbgetfile.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1879 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/smbpathcompleter.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3682 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/smbreg.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    15687 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/smbshareenum.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      616 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/smbsharelist.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6334 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/examples/zl.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.103470 aiosmb-0.4.6/aiosmb/external/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/external/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.107470 aiosmb-0.4.6/aiosmb/external/aiocmd/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/external/aiocmd/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.107470 aiosmb-0.4.6/aiosmb/external/aiocmd/aiocmd/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/external/aiocmd/aiocmd/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6197 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/external/aiocmd/aiocmd/aiocmd.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3688 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/external/aiocmd/aiocmd/nested_completer.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      718 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/external/aiocmd/setup.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.107470 aiosmb-0.4.6/aiosmb/external/asciitree/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/external/asciitree/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.115470 aiosmb-0.4.6/aiosmb/external/asciitree/asciitree/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2499 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/external/asciitree/asciitree/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2909 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/external/asciitree/asciitree/drawing.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1142 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/external/asciitree/asciitree/traversal.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      136 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/external/asciitree/asciitree/util.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      529 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/external/asciitree/setup.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.115470 aiosmb-0.4.6/aiosmb/protocol/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1159 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/common.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.115470 aiosmb-0.4.6/aiosmb/protocol/compression/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/compression/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5422 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/compression/lznt1.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.115470 aiosmb-0.4.6/aiosmb/protocol/crypto/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/crypto/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/crypto/from_impacket.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.115470 aiosmb-0.4.6/aiosmb/protocol/smb/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2331 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb/command_codes.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.115470 aiosmb-0.4.6/aiosmb/protocol/smb/commands/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      278 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb/commands/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3565 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb/commands/negotiate.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      835 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb/commons.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4600 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb/header.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1124 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb/message.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.115470 aiosmb-0.4.6/aiosmb/protocol/smb2/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      593 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/command_codes.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.139470 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2483 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      858 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/cancel.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3805 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/close.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    17789 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/create.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1680 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/echo.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1345 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/error.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2045 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/flush.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    13635 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/ioctl.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1696 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/logoff.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    23612 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/negotiate.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4684 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/query_directory.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6149 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/query_info.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6696 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/read.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5325 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/sessionsetup.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7973 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/tree_connect.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1768 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/tree_disconnect.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5364 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/commands/write.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/header.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.139470 aiosmb-0.4.6/aiosmb/protocol/smb2/headers/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      382 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/headers/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3599 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/headers/asynch.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1102 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/headers/common.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1848 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/headers/compression.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3525 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/headers/sync.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1421 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/headers/transform.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4687 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/protocol/smb2/message.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.143470 aiosmb-0.4.6/aiosmb/relay/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-04-25 11:35:07.000000 aiosmb-0.4.6/aiosmb/relay/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3365 2023-04-25 21:01:30.000000 aiosmb-0.4.6/aiosmb/relay/server.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    10792 2023-04-25 20:41:18.000000 aiosmb-0.4.6/aiosmb/relay/serverconnection.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.143470 aiosmb-0.4.6/aiosmb/transport/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/transport/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1523 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/transport/netbios.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.143470 aiosmb-0.4.6/aiosmb/wintypes/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6080 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/access_mask.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.143470 aiosmb-0.4.6/aiosmb/wintypes/dtyp/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/dtyp/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.147470 aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      347 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/access_mask.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    18185 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/ace.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      852 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/acl.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1233 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/guid.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6709 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/security_descriptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1081 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/security_information.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8490 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/sid.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.151470 aiosmb-0.4.6/aiosmb/wintypes/dtyp/structures/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/dtyp/structures/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1158 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/dtyp/structures/filetime.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.151470 aiosmb-0.4.6/aiosmb/wintypes/fscc/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3075 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/fscc/FileAttributes.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/fscc/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:29.151470 aiosmb-0.4.6/aiosmb/wintypes/fscc/structures/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2439 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/fscc/structures/FileFullDirectoryInformation.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/fscc/structures/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1898 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/fscc/structures/fileinfoclass.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    71052 2023-03-05 19:48:31.000000 aiosmb-0.4.6/aiosmb/wintypes/ntstatus.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 16:04:28.955469 aiosmb-0.4.6/aiosmb.egg-info/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      373 2023-05-30 16:04:28.000000 aiosmb-0.4.6/aiosmb.egg-info/PKG-INFO
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8120 2023-05-30 16:04:28.000000 aiosmb-0.4.6/aiosmb.egg-info/SOURCES.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-05-30 16:04:28.000000 aiosmb-0.4.6/aiosmb.egg-info/dependency_links.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      257 2023-05-30 16:04:28.000000 aiosmb-0.4.6/aiosmb.egg-info/entry_points.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-05-30 16:04:28.000000 aiosmb-0.4.6/aiosmb.egg-info/not-zip-safe
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      123 2023-05-30 16:04:28.000000 aiosmb-0.4.6/aiosmb.egg-info/requires.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        7 2023-05-30 16:04:28.000000 aiosmb-0.4.6/aiosmb.egg-info/top_level.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       88 2023-03-05 19:48:31.000000 aiosmb-0.4.6/pyproject.toml
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       38 2023-05-30 16:04:29.151470 aiosmb-0.4.6/setup.cfg
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1550 2023-05-30 15:59:28.000000 aiosmb-0.4.6/setup.py
```

### Comparing `aiosmb-0.4.4/README.md` & `aiosmb-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/connection/params.py` & `aiosmb-0.4.6/aiosmb/commons/connection/params.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/connection/target.py` & `aiosmb-0.4.6/aiosmb/commons/connection/target.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/exceptions.py` & `aiosmb-0.4.6/aiosmb/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/interfaces/blocking/file/blockingfile.py` & `aiosmb-0.4.6/aiosmb/commons/interfaces/blocking/file/blockingfile.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/interfaces/blocking/file/file.py` & `aiosmb-0.4.6/aiosmb/commons/interfaces/blocking/file/file.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/interfaces/blocking/file/protocol.py` & `aiosmb-0.4.6/aiosmb/commons/interfaces/blocking/file/protocol.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/interfaces/file.py` & `aiosmb-0.4.6/aiosmb/commons/interfaces/file.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,86 +1,111 @@
-from pathlib import PureWindowsPath
+from pathlib import PureWindowsPath, PurePath, Path
 from aiosmb.wintypes.access_mask import FileAccessMask
 from aiosmb.protocol.smb2.commands import *
 from aiosmb.wintypes.fscc.structures.fileinfoclass import FileInfoClass
 from aiosmb.protocol.smb2.commands.query_info import SecurityInfo
+from aiosmb.wintypes.fscc.FileAttributes import FileAttributes
+
 import io
+import datetime
 import asyncio
-
+from contextlib import asynccontextmanager
+from aiosmb.connection import SMBConnection
 
 class SMBFile:
 	def __init__(self):
 		self.tree_id = None
 		self.parent_dir = None
-		self.fullpath = None
-		self.unc_path = None
-		self.share_path = None
-		self.name = None
-		self.size = None
-		self.creation_time = None
-		self.last_access_time = None
-		self.last_write_time = None
-		self.change_time = None
-		self.allocation_size = None
-		self.attributes = None
-		self.file_id = None
+		self.fullpath:str = None
+		self.unc_path:str = None
+		self.share_path:str = None
+		self.name:str = None
+		self.size:int = None
+		self.creation_time:datetime.datetime = None
+		self.last_access_time:datetime.datetime = None
+		self.last_write_time:datetime.datetime = None
+		self.change_time:datetime.datetime = None
+		self.allocation_size:datetime.datetime = None
+		self.attributes:FileAttributes = None
+		self.file_id:int = None
 		self.security_descriptor = None
 
 		#internal
 		self.__connection = None
 		self.__position = 0
 		self.is_pipe = False
 		self.maxreadsize = None
 		self.mode = ''
+	
+	async def __aenter__(self):
+		return self
+	
+	async def __aexit__(self, exc_type, exc_val, exc_tb):
+		await self.close()
 
 	@staticmethod
-	def from_uncpath(unc_path):
+	def prepare_mirror_path(basedir:str, unc_path:str, path_with_file = True):
+		unc_path = unc_path.lstrip('\\')
+		unc = PureWindowsPath('\\\\\\\\' + unc_path)
+		host = unc.parts[1].replace('.'	, '_')
+		share = unc.parts[2]
+		if share.find('$') != -1:
+			share = share[:-1] + '_'
+		if path_with_file is True:
+			dirs = [host, share] + list(unc.parts[3:-1])
+		else:
+			dirs = [host, share] + list(unc.parts[3:])
+		path_to_create = Path(basedir).joinpath(*dirs).resolve()
+		return path_to_create
+	
+	@staticmethod
+	def from_uncpath(unc_path:str):
 		"""
 		Creates SMBFile object from the UNC path supplied.
 		Example uncpath: \\\\127.0.0.1\\C$\\temp\\test.exe
 		"""
 		unc = PureWindowsPath(unc_path)
 		f = SMBFile()
 		f.share_path = unc.drive
 		f.name = unc.name
 		f.fullpath = '\\'.join(unc.parts[1:])
 		
 		return f
 
 	@staticmethod
-	def from_remotepath(connection, remotepath):
+	def from_remotepath(connection:SMBConnection, remotepath:str):
 		"""
 		Creates SMBFile object from the connection and the remote path supplied.
 		Example remotepath: \\C$\\temp\\test.exe
 		"""
 		temp = '\\\\%s\\%s'
 		if remotepath[0] == '\\':
 			temp = '\\\\%s%s'
 		unc = temp % (connection.target.get_hostname_or_ip(), remotepath)
 		return SMBFile.from_uncpath(unc)
 	
 	@staticmethod
-	def from_smbtarget(target):
+	def from_smbtarget(target:str):
 		"""
 		Creates SMBFile object from the SMBUrl object
 		"""
 		if target.path is None:
 			return None
 		
 		fpath = target.path.replace('/','\\')
 		temp = '\\\\%s%s'
 		unc = temp % (target.get_hostname_or_ip(), fpath)
 		return SMBFile.from_uncpath(unc)
 
 	@staticmethod
-	def from_pipename(connection, pipename):
+	def from_pipename(connection:SMBConnection, pipename:str):
 		return SMBFile.from_uncpath('\\\\%s\\IPC$\\%s' % (connection.target.get_hostname_or_ip(), pipename))
 
 	@staticmethod
-	async def delete_unc(connection, remotepath):
+	async def delete_unc(connection:SMBConnection, remotepath:str):
 		try:
 			remfile = SMBFile.from_uncpath(remotepath)
 			tree_entry, err = await connection.tree_connect(remfile.share_path)
 			if err is not None:
 				raise err
 			tree_id = tree_entry.tree_id
 
@@ -99,15 +124,15 @@
 			await connection.tree_disconnect(tree_id)
 			return True, None
 		
 		except Exception as e:
 			return False, e
 
 	@staticmethod
-	async def delete_rempath(connection, remotepath):
+	async def delete_rempath(connection:SMBConnection, remotepath:str):
 		try:
 			remfile = SMBFile.from_remotepath(connection, remotepath)
 			tree_entry, err = await connection.tree_connect(remfile.share_path)
 			if err is not None:
 				raise err
 			tree_id = tree_entry.tree_id
 
@@ -163,15 +188,15 @@
 
 			await self.__connection.tree_disconnect(tree_id)
 			return True, None
 		
 		except Exception as e:
 			return False, e
 
-	async def get_security_descriptor(self, connection):
+	async def get_security_descriptor(self, connection:SMBConnection):
 		"""Fetches the security descriptor of the file."""
 		if self.security_descriptor is None:
 			file_id = None
 			try:
 				tree_id = self.tree_id
 				if self.tree_id is None:
 					tree_entry, err = await connection.tree_connect(self.share_path)
@@ -205,15 +230,15 @@
 				if file_id is not None:
 					await connection.close(tree_id, file_id)
 				if tree_id is not None and self.tree_id is None:
 					await connection.tree_disconnect(tree_id)
 
 		return self.security_descriptor, None
 
-	async def __read(self, size, offset):
+	async def __read(self, size:int, offset:int):
 		"""
 		This is the main function for reading.
 		It does not do buffering, so if more data is returned it will just discard it
 		If less data is returned than requested it will do more reads until the requested size is reached.
 		Do not call this directly as it could go in an infinite loop 
 		"""
 		if self.is_pipe == True:
@@ -233,15 +258,15 @@
 			data, remaining, err = await self.__connection.read(self.tree_id, self.file_id, offset = offset, length = self.__connection.MaxReadSize)
 			if err is not None:
 				return None, err
 			buffer += data
 				
 			return buffer[:size], err
 
-	async def __write(self, data, position_in_file = 0):
+	async def __write(self, data:bytes, position_in_file:int = 0):
 		"""
 		Data must be bytes
 		"""
 		try:
 			remaining = len(data)
 			total_bytes_written = 0
 			offset = 0
@@ -254,15 +279,15 @@
 				remaining -= bytes_written
 				offset += bytes_written
 				
 			return total_bytes_written, None
 		except Exception as e:
 			return None, e
 
-	async def open(self, connection, mode = 'r'):
+	async def open(self, connection:SMBConnection, mode:str = 'r'):
 		try:
 			self.__connection = connection
 			self.maxreadsize = connection.MaxReadSize
 			self.mode = mode
 			if 'p' in self.mode:
 				self.is_pipe = True
 				self.size = 0
@@ -305,15 +330,42 @@
 			else:
 				raise Exception('ONLY read and write is supported at the moment!')
 			
 			return True, None
 		except Exception as e:
 			return False, e
 
-	async def open_pipe(self, connection, mode):
+	async def download(self, connection:SMBConnection ,local_path:str):
+		"""Downloads the file to the local path. File must not be open."""
+		try:
+			if self.is_pipe:
+				raise Exception('Cannot download a pipe!')
+			if self.__connection is not None:
+				raise Exception('Cannot download a file that is already open!')
+			
+			_, err = await self.open(connection, 'r')
+			if err is not None:
+				raise err
+			
+			lfpath = Path(local_path).joinpath(self.name)
+			with open(lfpath, 'wb') as f:
+				async for data, err in self.read_chunked():
+					if err is not None:
+						raise err
+					if not data:
+						break
+					f.write(data)
+			
+			return lfpath, None
+		except Exception as e:
+			return False, e
+		finally:
+			await self.close()
+		
+	async def open_pipe(self, connection:SMBConnection, mode:str):
 		try:
 			self.__connection = connection
 			self.is_pipe = True
 			self.size = 0
 			share_mode = 0
 			file_attrs = 0x80
 			create_options = 0
@@ -333,15 +385,15 @@
 				raise err
 
 			return True, None
 		except Exception as e:
 			return False, e
 		
 		
-	async def seek(self, offset, whence = 0):
+	async def seek(self, offset:int, whence:int = 0):
 		"""Sets the current position of the file buffer to the given offset."""
 		try:
 			if whence == 0:
 				if offset < 0:
 					raise Exception('Offset must be > 0 when whence is 0')
 				if offset > self.size:
 					raise Exception('Seeking outside of file size!')
@@ -359,49 +411,53 @@
 				else:
 					raise Exception('Seeking outside of file size!')
 			
 			return True, None
 		except Exception as e:
 			return None, e
 		
-	async def read(self, size = -1):
+	async def read(self, size:int = -1):
 		try:
 			if self.is_pipe is True:
 				data, err = await self.__read(size, 0)
 				return data, err
 			
 			if size > self.size:
-				raise Exception('Requested read size %s is larger than the file size %s' % (hex(size), hex(self.size)))
+				size = -1
+				#raise Exception('Requested read size %s is larger than the file size %s' % (hex(size), hex(self.size)))
 
 			if size == 0:
-				raise Exception('Cant read 0 bytes')
+				return b'', None
+				#raise Exception('Cant read 0 bytes')
 				
 			elif size == -1:
+				if self.__position == self.size:
+					return b'', None
 				data, err = await self.__read(self.size - self.__position, self.__position)
 				if err is not None:
 					raise err
 				self.__position += len(data)
 				
 				return data, err
 				
 			elif size > 0:
 				if self.__position == self.size:
-					return None
+					return b'', None
 				if size + self.__position > self.size:
 					size = self.size - self.__position
 				data, err = await self.__read(size, self.__position)
 				if err is not None:
 					raise err
 				self.__position += len(data)
 				return data, err
 
 		except Exception as e:
 			return None, e
 
-	async def read_chunked(self, size = -1, chunksize = -1):
+	async def read_chunked(self, size:int = -1, chunksize:int = -1):
 		"""
 		Much like read, but yields chuks of chunksize untill the full size is read
 		Use this when reading large files as a whole, as this method doesn't caches 
 		the whole data read in memory, only chunskize
 		chunksize -1 will use the maximum chunk allowed by the underlying connection layer, it is advised to not set manually!
 		"""
 		if self.is_pipe is True:
@@ -521,8 +577,90 @@
 	def __str__(self):
 		t = '===== FILE =====\r\n'
 		for k in self.__dict__:
 			if k.startswith('parent_'):
 				continue
 			t += '%s : %s\r\n' % (k, self.__dict__[k])
 		
-		return t
+		return t
+
+@asynccontextmanager
+async def smb_open(path:str, mode = 'r', connection = None) -> SMBFile:
+	"""
+	Opens a file on the remote server
+	path can be a smb:// url or a path like \\server\share\path\to\file
+	"""
+	try:
+		if path.lower().startswith('smb'):
+			from aiosmb.commons.connection.factory import SMBConnectionFactory
+			factory = SMBConnectionFactory.from_url(path)
+			if connection is None:
+				connection = factory.get_connection()
+				async with connection:
+					_, err = await connection.login()
+					if err is not None:
+						raise err
+					file = factory.get_file()
+					_, err = await file.open(connection, mode)
+					if err is not None:
+						raise err
+					yield file
+					return
+			else:
+				file = factory.get_file()
+				_, err = await file.open(connection, mode)
+				if err is not None:
+					raise err
+				yield file
+				return
+		else:
+			file = SMBFile.from_remotepath(connection, path)
+			_, err = await file.open(connection, mode)
+			if err is not None:
+				raise err
+			yield file
+			return
+	finally:
+		if file is not None:
+			await file.close()
+
+
+async def amain():
+	url = 'smb2+ntlm-password://TEST\\Administrator:Passw0rd!1@10.10.10.2/C$/temp/repodata.json'
+	async with smb_open(url, 'rb') as f:
+		data, err = await f.read(1024)
+		print(data)
+		print(len(data))
+	
+	from aiosmb.commons.connection.factory import SMBConnectionFactory
+	connection = SMBConnectionFactory.from_url(url).get_connection()
+	_, err = await connection.login()
+	if err is not None:
+		raise err
+		
+	async with smb_open('C$/temp/repodata.json', 'rb', connection=connection) as f:
+		while True:
+			data, err = await f.read(1024)
+			print(data)
+			print(len(data))
+			if data == b'':
+				break
+
+	async with smb_open('C$/temp/repodata1.json', 'wb', connection=connection) as f:
+		_, err = await f.write(b'HELLO')
+		if err is not None:
+			print(err)
+	
+	async with smb_open('C$/temp/repodata1.json', 'rb', connection=connection) as f:
+		data, err = await f.read(1024)
+		if err is not None:
+			print(err)
+			return
+		print(data)
+		print(len(data))
+	
+	print('DONE!')
+
+if __name__ == '__main__':
+	import asyncio
+	asyncio.run(amain())
+
```

### Comparing `aiosmb-0.4.4/aiosmb/commons/interfaces/machine.py` & `aiosmb-0.4.6/aiosmb/commons/interfaces/machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 
+import fnmatch
 import asyncio
 import ntpath
 import os
 
+
 from aiosmb import logger
 from aiosmb.commons.interfaces.share import SMBShare
 from aiosmb.commons.interfaces.session import SMBUserSession
 from aiosmb.commons.interfaces.file import SMBFile
 from aiosmb.commons.interfaces.directory import SMBDirectory
 from aiosmb.dcerpc.v5.interfaces.srvsmgr import SRVSRPC
 from aiosmb.dcerpc.v5.interfaces.samrmgr import SAMRRPC
@@ -23,15 +25,14 @@
 
 from aiosmb.dcerpc.v5 import tsch, scmr
 
 from aiosmb.commons.exceptions import SMBMachineException
 
 from aiosmb.commons.interfaces.blocking.file.file import SMBBlockingFileMgr
 from aiosmb.commons.interfaces.blocking.file.blockingfile import SMBBlockingFile
-from aiosmb.commons.utils.apq import AsyncProcessQueue
 from aiosmb.protocol.smb2.commands.ioctl import CtlCode, IOCTLREQFlags
 
 from aiosmb.dcerpc.v5.rprn import PRINTER_CHANGE_ADD_JOB
 
 class SMBMachine:
 	def __init__(self, connection, print_cb = None, force_rpc_auth = None):
 		self.connection = connection
@@ -78,22 +79,22 @@
 
 
 	def get_blocking_file(self):
 		"""
 		Please don't ever use this
 		Starts a file manager task and initializes the io queues
 		"""
-
-		in_q = AsyncProcessQueue()
-		out_q = AsyncProcessQueue()
-		fsm = SMBBlockingFileMgr(self.connection, in_q, out_q)
-		fsmt = asyncio.create_task(fsm.run())
-		self.blocking_mgr_tasks[fsmt] = 1
-		bfile = SMBBlockingFile(in_q, out_q)
-		return bfile
+		raise DeprecationWarning()
+		#in_q = AsyncProcessQueue()
+		#out_q = AsyncProcessQueue()
+		#fsm = SMBBlockingFileMgr(self.connection, in_q, out_q)
+		#fsmt = asyncio.create_task(fsm.run())
+		#self.blocking_mgr_tasks[fsmt] = 1
+		#bfile = SMBBlockingFile(in_q, out_q)
+		#return bfile
 
 	async def connect_rpc(self, service_name, reconnect = False):
 		try:
 			if service_name not in self.named_rpcs_proto:
 				raise Exception('Unknown service name : %s' % service_name)
 			
 			if service_name in self.open_rpcs and reconnect is False:
@@ -327,14 +328,39 @@
 			if err is not None:
 				continue
 				raise err
 
 			async for entry in shares[share_name].subdirs[''].list_r(self.connection, depth = depth, maxentries = maxentries, fetch_dir_sd = fetch_dir_sd, fetch_file_sd = fetch_file_sd, exclude_dir = exclude_dir):
 				yield entry
 				await asyncio.sleep(0)
+	
+	async def enum_files_with_filter(self, filter_cb):
+		shares = {}
+		async for share, err in self.list_shares():
+			if err is not None:
+				raise err
+			shares[share.name] = share
+			yield share, 'share', None
+
+		for share_name in shares:
+			res = await filter_cb('sharename', share_name)
+			if res is False:
+				continue
+
+			_, err = await shares[share_name].connect(self.connection)
+			if err is not None:
+				continue
+			
+			res = await filter_cb('share', shares[share_name])
+			if res is False:
+				continue
+
+			async for entry in shares[share_name].subdirs[''].list_r(self.connection, depth = 1000, maxentries = -1, filter_cb = filter_cb):
+				yield entry
+				await asyncio.sleep(0)
 
 	async def put_file(self, local_path, remote_path):
 		"""
 		remote_path must be a full UNC path with the file name included!
 
 		"""
 		try:
@@ -1013,13 +1039,79 @@
 			_, err = await self.connect_rpc('LSAD')
 			if err is not None:
 				raise err
 			return await self.named_rpcs['LSAD'].get_backupkeys()
 		except Exception as e:
 			return None, e
 	
-
-	#### TODO SECTION
-
-	async def list_mountpoints(self):
-		pass
-	
+#	"""
+#	fpath
+#	fname
+#	ext
+#	size
+#	creationtime
+#	content
+#	"""
+#	
+#	async def search(self, depth = 3, maxentries = None, exclude_share=['print$', 'PRINT$'], exclude_dir=[]):
+#		try:
+#			async for obj, otype, err in self.enum_all_recursively(self,  fetch_share_sd = False, fetch_dir_sd = False, fetch_file_sd = False):
+#				if otype != 'file':
+#					continue
+#
+#				share, 'share', None
+#
+#		except Exception as e:
+#			return None, e
+#	
+#
+#	#### TODO SECTION
+#
+#	async def list_mountpoints(self):
+#		pass
+#	
+#class FileFilter:
+#	def __init__(self):
+#		self.fname = None
+#		self.size = None
+#		self.creationtime = None
+#		self.content = None
+#		self.matchcase = False
+#	
+#	async def filter(self, fileobj:SMBFile, fcontent = None):
+#		try:
+#			fname_matches = True
+#			size_matches = True
+#			if self.fname is not None:
+#				fname_matches = False
+#				fname_matches = fnmatch.fnmatch(fileobj.fullpath, self.fname)
+#				if self.matchcase is False:
+#					fname_matches = fnmatch.fnmatchcase(fileobj.fullpath, self.fname)				
+#				
+#			if self.size is not None:
+#				size_matches = False
+#				if self.size.startswith('<=') is True:
+#					size = int(self.size[2:])
+#					if fileobj.size <= size:
+#						size_matches = True
+#				elif self.size.startswith('>=') is True:
+#					size = int(self.size[2:])
+#					if fileobj.size >= size:
+#						size_matches = True
+#				elif self.size.startswith('==') is True:
+#					size = int(self.size[2:])
+#					if fileobj.size == size:
+#						size_matches = True
+#				elif self.size[0] == '=' is True:
+#					size = int(self.size[1:])
+#					if fileobj.size == size:
+#						size_matches = True
+#			
+#			
+#				
+#			
+#
+#
+#
+#
+#		except Exception as e:
+#			return None, None, None, e
```

### Comparing `aiosmb-0.4.4/aiosmb/commons/interfaces/share.py` & `aiosmb-0.4.6/aiosmb/commons/interfaces/share.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/scanner/scanner.py` & `aiosmb-0.4.6/aiosmb/commons/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/utils/apq.py` & `aiosmb-0.4.6/aiosmb/commons/utils/apq.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/utils/decorators.py` & `aiosmb-0.4.6/aiosmb/commons/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/utils/glob2re.py` & `aiosmb-0.4.6/aiosmb/commons/utils/glob2re.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/utils/hexdump.py` & `aiosmb-0.4.6/aiosmb/commons/utils/hexdump.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/utils/ts2dt.py` & `aiosmb-0.4.6/aiosmb/commons/utils/ts2dt.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/commons/utils/univeraljson.py` & `aiosmb-0.4.6/aiosmb/commons/utils/univeraljson.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/connection.py` & `aiosmb-0.4.6/aiosmb/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from aiosmb.wintypes.fscc.structures.fileinfoclass import FileInfoClass
 from aiosmb.wintypes.fscc.structures.FileFullDirectoryInformation import FileFullDirectoryInformationList
 from aiosmb.wintypes.fscc.FileAttributes import FileAttributes
 
 from winacl.dtyp.security_descriptor import SECURITY_DESCRIPTOR
 from winacl.functions.constants import SE_OBJECT_TYPE
 
-#from aiosmb.commons.smbcontainer import *
 from aiosmb.commons.connection.target import *
 
 from unicrypto import hmac
 from unicrypto import hashlib
 from unicrypto.symmetric import AES, MODE_CCM, MODE_GCM
 from unicrypto.cmac import AES_CMAC
 from unicrypto.kdf import KDF_CounterMode
@@ -937,22 +936,25 @@
 			
 			await self.network_connection.write(msg.to_bytes())
 			return message_id, None
 		except Exception as e:
 			return None, e
 
 		
-	async def tree_connect(self, share_name):
+	async def tree_connect(self, share_name:str):
 		"""
 		share_name MUST be in "\\\\server\\share" format! Server can be NetBIOS name OR IP4 OR IP6 OR FQDN
 		"""
 		try:
 			if self.session_closed == True or self.status == SMBConnectionStatus.CLOSED:
 				raise SMBConnectionTerminated()
 			
+			if share_name is None:
+				raise Exception('Share name is None!')
+			
 			command = TREE_CONNECT_REQ()
 			command.Path = share_name
 			command.Flags = 0
 			
 			header = SMB2Header_SYNC()
 			header.Command  = SMB2Command.TREE_CONNECT
```

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/bkrp.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/bkrp.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/common/connection/authentication.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/common/connection/authentication.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/common/connection/connectionstring.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/common/connection/connectionstring.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/common/connection/smbdcefactory.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/common/connection/smbdcefactory.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/common/connection/target.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/common/connection/target.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 	def get_hostname_or_ip(self):
 		if self.smb_connection is not None:
 			return self.smb_connection.target.get_hostname_or_ip()
 		if self.hostname is None:
 			return self.ip
 		return self.hostname
 	
+	def get_ip_or_hostname(self):
+		if self.smb_connection is not None:
+			return self.smb_connection.target.get_ip_or_hostname()
+		if self.ip is None:
+			return self.hostname
+		return self.ip
+	
 	#def to_target_string(self) -> str:
 	#	if self.hostname is None:
 	#		raise Exception('Hostname is None!')
 	#	if self.domain is None:
 	#		raise Exception('Domain is None!')
 	#	return 'cifs/%s@%s' % (self.hostname, self.domain)
 
@@ -33,21 +40,21 @@
 		if self.smb_connection is not None:
 			return self.smb_connection.target.to_target_string()
 		return 'cifs/%s@%s' % (self.hostname, self.domain)
 
 	@staticmethod
 	def from_smbconnection(smb_connection, pipe = None):
 		if pipe is None:
-			target = DCERPCSMBTarget(None, smb_connection.target.get_hostname_or_ip(), smb_connection=smb_connection, timeout = smb_connection.target.timeout)
+			target = DCERPCSMBTarget(None, smb_connection.target.get_ip_or_hostname(), smb_connection=smb_connection, timeout = smb_connection.target.timeout, hostname=smb_connection.target.get_hostname_or_ip())
 		else:
-			target = DCERPCSMBTarget(None, smb_connection.target.get_hostname_or_ip(), pipe, smb_connection=smb_connection, timeout = smb_connection.target.timeout)
+			target = DCERPCSMBTarget(None, smb_connection.target.get_ip_or_hostname(), pipe, smb_connection=smb_connection, timeout = smb_connection.target.timeout, hostname=smb_connection.target.get_hostname_or_ip())
 		return target
 
 	@staticmethod
-	def from_connection_string(s, smb_connection = None, timeout = 1, proxies:List[UniProxyTarget] = None, dc_ip:str = None, domain:str = None):
+	def from_connection_string(s, smb_connection = None, timeout = 1, proxies:List[UniProxyTarget] = None, dc_ip:str = None, domain:str = None, hostname:str = None):
 		if isinstance(s, str):
 			connection_string = DCERPCStringBinding(s)
 		elif isinstance(s, DCERPCStringBinding):
 			connection_string = s
 		else:
 			raise Exception('Unknown string binding type %s' % type(s))
 		
@@ -58,25 +65,25 @@
 		ps = connection_string.get_protocol_sequence()
 		if ps == 'ncadg_ip_udp':
 			raise Exception('DCERPC UDP not implemented')
 			port = connection_string.get_endpoint()
 			target = DCERPCUDPTarget(connection_string, na, int(port), timeout = timeout)
 		elif ps == 'ncacn_ip_tcp':
 			port = connection_string.get_endpoint()
-			target = DCERPCTCPTarget(connection_string, na, port, timeout = timeout, dc_ip=dc_ip, domain = domain)
+			target = DCERPCTCPTarget(connection_string, na, port, timeout = timeout, dc_ip=dc_ip, domain = domain, hostname = hostname)
 		elif ps == 'ncacn_http':
 			raise Exception('DCERPC HTTP not implemented')
 			target = DCERPCHTTPTarget(connection_string, na, int(port), timeout = timeout)
 		elif ps == 'ncacn_np':
 			named_pipe = connection_string.get_endpoint()
 			if named_pipe:
 				named_pipe = named_pipe[len(r'\pipe'):]
-				target = DCERPCSMBTarget(connection_string, na, pipe=named_pipe, smb_connection=smb_connection, timeout = timeout)
+				target = DCERPCSMBTarget(connection_string, na, pipe=named_pipe, smb_connection=smb_connection, timeout = timeout, hostname = hostname)
 			else:
-				target = DCERPCSMBTarget(connection_string, na, smb_connection=smb_connection, timeout = timeout)
+				target = DCERPCSMBTarget(connection_string, na, smb_connection=smb_connection, timeout = timeout, hostname = hostname)
 		elif ps == 'ncalocal':
 			raise Exception('DCERPC LOCAL not implemented')
 			target = DCERPCLocalTarget(connection_string, na, int(port), timeout = timeout)
 		
 		else:
 			raise Exception('Unknown DCERPC protocol %s' % ps)
 
@@ -93,85 +100,94 @@
 	def __str__(self):
 		t = '==== DCERPCTarget ====\r\n'
 		for k in self.__dict__:
 			t += '%s: %s\r\n' % (k, self.__dict__[k])
 			
 		return t
 
+	def __hash__(self):
+		return hash(str(self.connection_string) + str(self.rpcprotocol) + str(self.pipe) +\
+			str(self.ip) + str(self.port) + str(self.protocol) + str(self.timeout) +\
+			str(self.hostname) + str(self.domain) + str(self.dc_ip))
+
+	def __eq__(self, other):
+		if not isinstance(other, DCERPCTarget):
+			return False
+		return self.__hash__() == other.__hash__()
 
 class DCERPCTCPTarget(DCERPCTarget):
-	def __init__(self, connection_string, ip, port, timeout = 1, proxies = None, dc_ip:str = None, domain:str = None):
+	def __init__(self, connection_string, ip, port, timeout = 1, proxies = None, dc_ip:str = None, domain:str = None, hostname = None):
 		DCERPCTarget.__init__(
 			self, 
 			connection_string, 
 			ip, 
 			int(port), 
 			UniProto.CLIENT_TCP, 
 			'ncacn_ip_tcp', 
 			proxies = proxies, 
 			timeout = timeout, 
-			hostname = None, 
+			hostname = hostname, 
 			domain = domain, 
 			dc_ip = dc_ip
 		)
 
 class DCERPCUDPTarget(DCERPCTarget):
-	def __init__(self, connection_string, ip, port, timeout = 1, proxies = None, dc_ip:str = None, domain:str = None):
+	def __init__(self, connection_string, ip, port, timeout = 1, proxies = None, dc_ip:str = None, domain:str = None, hostname = None):
 		DCERPCTarget.__init__(
 			self, 
 			connection_string, 
 			ip, 
 			int(port), 
 			UniProto.CLIENT_UDP, 
 			'ncadg_ip_udp', 
 			proxies = proxies, 
 			timeout = timeout, 
-			hostname = None, 
+			hostname = hostname, 
 			domain = domain, 
 			dc_ip = dc_ip
 		)
 
 class DCERPCSMBTarget(DCERPCTarget):
-	def __init__(self, connection_string, ip, pipe = None, smb_connection = None, timeout = 1):
+	def __init__(self, connection_string, ip, pipe = None, smb_connection = None, timeout = 1, hostname = None):
 		DCERPCTarget.__init__(
 			self, 
 			connection_string, 
 			ip, 
 			None, 
 			UniProto.CLIENT_TCP, 
 			'ncacn_np', 
 			proxies = smb_connection.target.proxies, 
 			timeout = timeout, 
-			hostname = None, 
+			hostname = hostname, 
 			domain = smb_connection.target.domain, 
 			dc_ip = smb_connection.target.dc_ip,
 			smb_connection = smb_connection,
 			pipe = pipe
 		)
 
 class DCERPCHTTPTarget(DCERPCTarget):
-	def __init__(self, connection_string, ip, port, timeout = 1, proxies = None, domain = None, dc_ip = None):
+	def __init__(self, connection_string, ip, port, timeout = 1, proxies = None, domain = None, dc_ip = None, hostname = None):
 		DCERPCTarget.__init__(
-			self, 
+			self,
 			connection_string,
 			ip,
 			port, 
 			UniProto.CLIENT_TCP,
 			'ncacn_http',
 			proxies = proxies, 
 			timeout = timeout, 
-			hostname = None, 
+			hostname = hostname, 
 			domain = domain, 
 			dc_ip = dc_ip
 		)
 		self.set_hostname_or_ip(ip)
 		self.port = int(port)
 
 class DCERPCLocalTarget(DCERPCTarget):
-	def __init__(self, connection_string, ip, port, timeout = 1):
+	def __init__(self, connection_string, ip, port, timeout = 1, hostname = None):
 		raise NotImplementedError()
 		DCERPCTarget.__init__(self, connection_string, DCERPCTargetType.LOCAL, timeout = timeout)
 		self.set_hostname_or_ip(ip)
 		self.port = int(port)
 		self.rpcprotocol = 'ncalocal'
```

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/common/domain.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/common/domain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import asyncio
 import logging
 import json
 
 import aiosmb
-from aiosmb.commons.connection.credential import SMBCredential
-from aiosmb.commons.connection.target import SMBTarget
-from aiosmb.commons.connection.authbuilder import AuthenticatorBuilder
-from aiosmb.connection import SMBConnection
-
-from aiosmb.dcerpc.v5.transport.smbtransport import SMBTransport
-from aiosmb.dcerpc.v5.interfaces.samrmgr import SMBSAMR
+from aiosmb.dcerpc.v5.interfaces.samrmgr import SAMRRPC
 from aiosmb.dcerpc.v5 import samr
 
 class SMBDomain:
 	def __init__(self, domain_name, samr = None, connection = None):
 		self.domain_name = domain_name
 		self.connection = connection
 		self.domain_access_level = None
@@ -29,15 +23,17 @@
 		
 	async def __aexit__(self, exc_type, exc, traceback):
 		pass
 	
 	async def open(self, access_level = samr.MAXIMUM_ALLOWED):
 		self.domain_access_level = access_level
 		if self.samr is None:
-			self.samr = SMBSAMR(self.connection)
+			self.samr, err = await SAMRRPC.from_smbconnection(self.connection)
+			if err is not None:
+				raise err
 			logging.debug('Connecting to SAMR')
 			try:
 				await self.samr.connect()
 			except Exception as e:
 				logging.exception('Failed to connect to SAMR')
 				raise e
 				
@@ -84,30 +80,31 @@
 	
 		
 	
 	
 	
 	
 async def domain_test(connection_string, domain_name, out_file = None, json_out = False):
-	target = SMBTarget.from_connection_string(connection_string)
-	credential = SMBCredential.from_connection_string(connection_string)
-	spneg = AuthenticatorBuilder.to_spnego_cred(credential, target)
+	from aiosmb.commons.connection.factory import SMBConnectionFactory
 	
-	async with SMBConnection(spneg, target) as connection: 
+	async with SMBConnectionFactory.from_url(connection_string).get_connection() as connection: 
 		await connection.login()
 		
 		async with SMBDomain(domain_name, connection=connection) as domain:
 			logging.debug('Connecting to SAMR')
 			try:
 				await domain.open(access_level = samr.DOMAIN_ALL_ACCESS)
 			except Exception as e:
 				logging.exception('Failed to create domain object')
 				
-			info = await domain.get_info()
-			
+			info, err = await domain.get_info()
+			if err is not None:
+				raise err
+			print(info)
+
 			async for user_name, user_sid in domain.list_users():
 				print(user_name, user_sid)
 				try:
 					user_handle = await domain.open_user(user_sid, access_level = samr.USER_ALL_ACCESS)
 					#x = await domain.get_security_info(user_handle)
 					user_info = await domain.get_user_info(user_handle)
```

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/common/even6/binxml.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/common/even6/binxml.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/common/even6/resultset.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/common/even6/resultset.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/common/secrets.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/common/secrets.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/common/service.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/common/service.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/connection.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/connection.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/drsuapi.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/drsuapi.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/dtypes.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/dtypes.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/enum.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/enum.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/epm.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/epm.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/even.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/even.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/even6.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/even6.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/hresult_errors.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/hresult_errors.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/icpr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/icpr.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/bkrp.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/bkrp.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/drsuapimgr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/drsuapimgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,28 +209,29 @@
 				'lmPwdHistory': '1.2.840.113556.1.4.160',
 				'supplementalCredentials': '1.2.840.113556.1.4.125',
 				'objectSid': '1.2.840.113556.1.4.146',
 				'pwdLastSet': '1.2.840.113556.1.4.96',
 				'userAccountControl':'1.2.840.113556.1.4.8'
 			}
 			formatOffered = drsuapi.DS_NT4_ACCOUNT_NAME_SANS_DOMAIN
-			
 			crackedName, err = await self.DRSCrackNames(
 					formatOffered,
 					drsuapi.DS_NAME_FORMAT.DS_UNIQUE_ID_NAME,
 					name=username
 				)
 			if err is not None:
 				raise err
 			
 			###### TODO: CHECKS HERE
 			
 			#guid = GUID.from_string(crackedName['pmsgOut']['V1']['pResult']['rItems'][0]['pName'][:-1][1:-1])
 			guid = crackedName['pmsgOut']['V1']['pResult']['rItems'][0]['pName'][:-1][1:-1]
-			
+			if len(guid) == 0:
+				raise Exception('User "%s" cannot be found in the domain!' % username)
+
 			userRecord, err = await self.DRSGetNCChanges(guid, ra)
 			if err is not None:
 				return None, err
 			
 			replyVersion = 'V%d' % userRecord['pdwOutVersion']
 			if userRecord['pmsgOut'][replyVersion]['cNumObjects'] == 0:
 				raise Exception('DRSGetNCChanges didn\'t return any object!')
```

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/endpointmgr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/endpointmgr.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,28 +43,31 @@
 		return EPM(connection, data_representation)
 
 	@staticmethod
 	def from_smbconnection(smb_connection, port:int = 135, protocol:str = 'ncacn_ip_tcp', data_representation = None):
 		"""
 		Sets up the EPM connection from an existing SMB connection
 		"""
-		dcerpc_target_str = r'%s:%s[%s]' % (protocol, smb_connection.target.get_hostname_or_ip(), port)
+		dcerpc_target_str = r'%s:%s[%s]' % (protocol, smb_connection.target.get_ip_or_hostname(), port)
 		target = DCERPCTarget.from_connection_string(dcerpc_target_str, proxies=smb_connection.target.proxies)
 		auth = DCERPCAuth.from_smb_gssapi(smb_connection.gssapi)
 		connection = DCERPC5Connection(auth, target)
 		connection.set_auth_type(RPC_C_AUTHN_LEVEL_NONE)
 		return EPM(connection, data_representation)
 
 	@staticmethod
-	def from_unitarget(target:UniTarget, protocol:str = 'ncacn_ip_tcp', port:int = 135, data_representation = None):
-		dcerpc_target_str = r'%s:%s[%s]' % (protocol, target.get_hostname_or_ip(), port)
+	def from_unitarget(target:UniTarget, protocol:str = 'ncacn_ip_tcp', port:int = 135, data_representation = None, credentials = None):
+		dcerpc_target_str = r'%s:%s[%s]' % (protocol, target.get_ip_or_hostname(), port)
 		target = DCERPCTarget.from_connection_string(dcerpc_target_str, proxies = target.proxies)
 		auth = None
+		if credentials is not None:
+			auth = DCERPCAuth.from_smb_gssapi(credentials)
 		connection = DCERPC5Connection(auth, target)
-		connection.set_auth_type(RPC_C_AUTHN_LEVEL_NONE)
+		if auth is None:
+			connection.set_auth_type(RPC_C_AUTHN_LEVEL_NONE)
 		return EPM(connection, data_representation)
 
 	@staticmethod
 	async def create_connection(target:UniTarget, credential:SPNEGOCredential, remoteIf):
 		epm = None
 		try:
 			epm = EPM.from_unitarget(target)
@@ -105,29 +108,44 @@
 		finally:
 			if epm is not None:
 				await epm.disconnect()
 
 	async def disconnect(self):
 		await self.dce.disconnect()
 
-	async def connect(self):
+	async def connect(self, autobind = True):
 		try:
 			_, err = await self.dce.connect()
 			if err is not None:
 				raise err
-			#print('EPM bind')
-			_, err = await self.dce.bind(MSRPC_UUID_PORTMAP)
+			
+			if not autobind:
+				return True, None
+			return await self.bind()
+		except Exception as e:
+			return False, e
+	
+	async def bind(self, uuid = MSRPC_UUID_PORTMAP):
+		try:
+			_, err = await self.dce.bind(uuid)
 			if err is not None:
 				raise err
-			#print('EPM done')
 			return True,None
 		except Exception as e:
-			#print('EPM err %s' % e)
 			return False, e
 
+	async def disconnect(self):
+		await self.dce.disconnect()
+	
+	async def request(self, request):
+		try:
+			return await self.dce.request(request)
+		except Exception as e:
+			return None, e
+
 	async def map(self, remoteIf):
 		try:
 			tower = EPMTower()
 			interface = EPMRPCInterface()
 
 			interface['InterfaceUUID'] = remoteIf[:16]
 			interface['MajorVersion'] = unpack('<H', remoteIf[16:][:2])[0]
```

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/even6.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/even6.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/icprmgr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/icprmgr.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/lsatmgr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/lsatmgr.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/parmgr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/parmgr.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/remoteregistry.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/remoteregistry.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/rprnmgr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/rprnmgr.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/samrmgr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/samrmgr.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/servicemanager.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/servicemanager.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/srvsmgr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/srvsmgr.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/tschmgr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/tschmgr.py`

 * *Files 20% similar despite different names*

```diff
@@ -260,46 +260,7 @@
 			 "&": "&amp;",
 			 '"': "&quot;",
 			 "'": "&apos;",
 			 ">": "&gt;",
 			 "<": "&lt;",
 			 }
 		return ''.join(replace_table.get(c, c) for c in data)
-
-async def amain():
-	try:
-		from aiosmb.commons.connection.credential import SMBCredential, SMBAuthProtocol, SMBCredentialsSecretType
-		from aiosmb.commons.connection.authbuilder import AuthenticatorBuilder
-		from aiosmb.dcerpc.v5.common.connection.authentication import DCERPCAuth
-
-		ip = '10.10.10.2'
-		target, err = await EPM.create_target(ip, TSCHRPC().service_uuid)
-		if err is not None:
-			raise err
-		
-		cred = SMBCredential(
-			username = 'Administrator', 
-			domain = 'TEST', 
-			secret = 'Passw0rd!1', 
-			secret_type = SMBCredentialsSecretType.PASSWORD, 
-			authentication_type = SMBAuthProtocol.NTLM, 
-			settings = None, 
-			target = None)
-
-		gssapi = AuthenticatorBuilder.to_spnego_cred(cred)
-		auth = DCERPCAuth.from_smb_gssapi(gssapi)
-		connection = DCERPC5Connection(auth, target)
-		service, err = await TSCHRPC.from_rpcconnection(connection, perform_dummy=True)
-		if err is not None:
-			raise err
-		
-		async for task, err in service.list_tasks():
-			if err is not None:
-				raise err
-			print(task)
-
-	except Exception as e:
-		traceback.print_exc()
-
-if __name__ == '__main__':
-	import asyncio
-	asyncio.run(amain())
```

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/interfaces/wkstmgr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/interfaces/wkstmgr.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/lsad.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/lsad.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/lsat.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/lsat.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/ndr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/ndr.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/nrpc.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/nrpc.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/par.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/par.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/bind.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/bind.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/bindack.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/bindack.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/bindnack.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/bindnack.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/cancel.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/cancel.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/commons.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/commons.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/protocol/conpdu/constants.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/protocol/conpdu/constants.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/rpcrt.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/rpcrt.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/rprn.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/rprn.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/rrp.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/rrp.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/samr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/samr.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/scmr.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/scmr.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/servers/transport/smbtransport.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/servers/transport/smbtransport.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/srvs.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/srvs.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/structure.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/structure.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/system_errors.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/system_errors.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/transport/smb.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/transport/smb.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/transport/tcp.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/transport/tcp.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/tsch.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/tsch.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/uuid.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/uuid.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/dcerpc/v5/wkst.py` & `aiosmb-0.4.6/aiosmb/dcerpc/v5/wkst.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/epmtest.py` & `aiosmb-0.4.6/aiosmb/examples/epmtest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import traceback
+from asyauth.common.constants import asyauthSecret
+from asyauth.common.credentials.spnego import SPNEGOCredential
+from asyauth.common.credentials.ntlm import NTLMCredential
 from aiosmb.dcerpc.v5.interfaces.endpointmgr import EPM
 from aiosmb.dcerpc.v5.epm import KNOWN_UUIDS, KNOWN_PROTOCOLS
 from aiosmb.dcerpc.v5.uuid import uuidtup_to_bin, generate, stringver_to_bin, bin_to_uuidtup, bin_to_string
-from aiosmb.commons.connection.credential import SMBCredential, SMBAuthProtocol, SMBCredentialsSecretType
-from aiosmb.commons.connection.authbuilder import AuthenticatorBuilder
 from aiosmb.dcerpc.v5.common.connection.authentication import DCERPCAuth
 from aiosmb.dcerpc.v5.connection import DCERPC5Connection
 from aiosmb.dcerpc.v5.dtypes import NULL
 from aiosmb.dcerpc.v5.rpcrt import RPC_C_AUTHN_LEVEL_NONE,\
 	RPC_C_AUTHN_LEVEL_CONNECT,\
 	RPC_C_AUTHN_LEVEL_CALL,\
 	RPC_C_AUTHN_LEVEL_PKT,\
@@ -55,25 +56,22 @@
 				raise err
 			
 			targets.append((uuidstr, service_uuid, target))
 		
 		for uuidstr, service_uuid, target in targets:
 			#print('UUID: %s' % uuidstr)
 			#print('Target: %s' % target)
-			cred = SMBCredential(
+			cred = NTLMCredential(
 				username = 'Administrator', 
 				domain = 'TEST', 
 				secret = 'Passw0rd!1', 
-				secret_type = SMBCredentialsSecretType.PASSWORD, 
-				authentication_type = SMBAuthProtocol.NTLM, 
-				settings = None, 
-				target = None
+				stype = asyauthSecret.PASSWORD, 
 			)
 
-			gssapi = AuthenticatorBuilder.to_spnego_cred(cred)
+			gssapi = SPNEGOCredential([cred]).build_context()
 			auth = DCERPCAuth.from_smb_gssapi(gssapi)
 			connection = DCERPC5Connection(auth, target)
 			connection.set_auth_level(RPC_C_AUTHN_LEVEL_CONNECT)
 			try:
 				_, err = await connection.connect()
 				if err is not None:
 					raise err
```

### Comparing `aiosmb-0.4.4/aiosmb/examples/scancommons/internal.py` & `aiosmb-0.4.6/aiosmb/examples/scancommons/internal.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/scancommons/targetgens.py` & `aiosmb-0.4.6/aiosmb/examples/scancommons/targetgens.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/scanners/__main__.py` & `aiosmb-0.4.6/aiosmb/examples/scanners/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 	parser = argparse.ArgumentParser(description='SMB Scanner', usage=usage)
 	parser.add_argument('-w', '--worker-count', type=int, default=100, help='Parallell count')
 	parser.add_argument('-t', '--timeout', type=int, default=10, help='Timeout for each connection')
 	parser.add_argument('--no-progress', action='store_false', help='Disable progress bar')
 	parser.add_argument('-o', '--out-file', help='Output file path.')
 	parser.add_argument('-s', '--scan', nargs='+', required=True, help='Scanner type')
 	parser.add_argument('-e', '--errors', action='store_true', help='Includes errors in output.')
+	parser.add_argument('-d', '--depth', type=int, default=6, help='Share enumeration depth.')
 	parser.add_argument('url', help = 'Connection string in URL format')
 	parser.add_argument('targets', nargs='*', help = 'Hostname or IP address or file with a list of targets')
 	args = parser.parse_args()
 
 	if len(args.targets) == 0:
 		print('No targets defined!')
 		return
@@ -54,20 +55,26 @@
 	connectionfactory = SMBConnectionFactory.from_url(args.url)
 	scantypes = []
 	for x in args.scan:
 		scantypes.append(x.lower())
 	executors = []
 	if 'all' in scantypes:
 		for k in smbscan_options:
+			if k == 'file':
+				executors.append(smbscan_options[k][0](connectionfactory, depth=args.depth))
+				continue
 			executors.append(smbscan_options[k][0](connectionfactory))
 	else:
 		for scantype in scantypes:
 			if scantype not in smbscan_options:
 				print('Unknown scan type: "%s"' % scantype)
 				return
+			if k == 'file':
+				executors.append(smbscan_options[k][0](connectionfactory, depth=args.depth))
+				continue
 			executors.append(smbscan_options[scantype][0](connectionfactory))
 			
 	timeout = args.timeout
 	if 'file' in scantypes:
 		timeout = None
 		
 	tgen = UniTargetGen.from_list(args.targets)
```

### Comparing `aiosmb-0.4.4/aiosmb/examples/scanners/smbadmin.py` & `aiosmb-0.4.6/aiosmb/examples/scanners/smbadmin.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/scanners/smbfile.py` & `aiosmb-0.4.6/aiosmb/examples/scanners/smbfile.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/scanners/smbfinger.py` & `aiosmb-0.4.6/aiosmb/examples/scanners/smbfinger.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/scanners/smbiface.py` & `aiosmb-0.4.6/aiosmb/examples/scanners/smbiface.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/scanners/smbprintnightmare.py` & `aiosmb-0.4.6/aiosmb/examples/scanners/smbprintnightmare.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/scanners/smbproto.py` & `aiosmb-0.4.6/aiosmb/examples/scanners/smbproto.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/scanners/smbsession.py` & `aiosmb-0.4.6/aiosmb/examples/scanners/smbsession.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/smbcertreq.py` & `aiosmb-0.4.6/aiosmb/examples/smbcertreq.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import os
 
 from aiosmb import logger
 from aiosmb._version import __banner__
 from aiosmb.commons.connection.factory import SMBConnectionFactory
 from aiosmb.dcerpc.v5.interfaces.icprmgr import ICPRRPC
 from aiosmb.dcerpc.v5.connection import DCERPC5Connection
-from aiosmb.commons.connection.authbuilder import AuthenticatorBuilder
 from aiosmb.dcerpc.v5.common.connection.authentication import DCERPCAuth
 from aiosmb.dcerpc.v5.interfaces.endpointmgr import EPM
 
 from msldap.ldap_objects.adcertificatetemplate import EKUS_NAMES
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.serialization import Encoding, pkcs7, pkcs12, BestAvailableEncryption, load_pem_private_key
@@ -36,15 +35,15 @@
 			pfx_password = 'admin'
 		
 		print('[+] Parsing connection parameters...')
 		su = SMBConnectionFactory.from_url(url)
 		ip = su.get_target().get_hostname_or_ip()
 
 		if cn is None:
-			cn = '%s@%s' % (su.username, su.domain)
+			cn = '%s@%s' % (su.credential.username, su.credential.domain)
 		
 		print('[*] Using CN: %s' % cn)
 		
 		print('[+] Generating RSA privat key...')
 		key = rsa.generate_private_key(0x10001, 2048)
 
 		print('[+] Building certificate request...')
@@ -86,16 +85,15 @@
 		
 		print('[+] Connecting to EPM...')
 		target, err = await EPM.create_target(ip, ICPRRPC().service_uuid, dc_ip = su.get_target().dc_ip, domain = su.get_target().domain)
 		if err is not None:
 			raise err
 		
 		print('[+] Connecting to ICRPR service...')
-		gssapi = AuthenticatorBuilder.to_spnego_cred(su.get_credential(), target)
-		auth = DCERPCAuth.from_smb_gssapi(gssapi)
+		auth = DCERPCAuth.from_smb_gssapi(su.get_credential())
 		connection = DCERPC5Connection(auth, target)
 		rpc, err = await ICPRRPC.from_rpcconnection(connection, perform_dummy=True)
 		if err is not None:
 			raise err
 		logger.debug('DCE Connected!')
 		
 		print('[+] Requesting certificate from the service...')
```

### Comparing `aiosmb-0.4.4/aiosmb/examples/smbclient.py` & `aiosmb-0.4.6/aiosmb/examples/smbclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -1291,14 +1291,17 @@
 
 async def amain(args):
 	client = SMBClient(args.smb_url, silent = args.silent)
 	if len(args.commands) == 0:
 		if args.no_interactive is True:
 			print('Not starting interactive!')
 			return
+		res = await client._run_single_command('login', [])
+		if res is False:
+			return
 		await client.run()
 	else:
 		for command in args.commands:
 			if command == 'i':
 				await client.run()
 				return
```

### Comparing `aiosmb-0.4.4/aiosmb/examples/smbeventq.py` & `aiosmb-0.4.6/aiosmb/examples/smbeventq.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/smbget.py` & `aiosmb-0.4.6/aiosmb/examples/smbget.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/smbgetfile.py` & `aiosmb-0.4.6/aiosmb/examples/smbgetfile.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/smbpathcompleter.py` & `aiosmb-0.4.6/aiosmb/examples/smbpathcompleter.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/smbreg.py` & `aiosmb-0.4.6/aiosmb/examples/smbreg.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/smbshareenum.py` & `aiosmb-0.4.6/aiosmb/examples/smbshareenum.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/smbsharelist.py` & `aiosmb-0.4.6/aiosmb/examples/smbsharelist.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/examples/zl.py` & `aiosmb-0.4.6/aiosmb/examples/zl.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/external/aiocmd/aiocmd/aiocmd.py` & `aiosmb-0.4.6/aiosmb/external/aiocmd/aiocmd/aiocmd.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/external/aiocmd/aiocmd/nested_completer.py` & `aiosmb-0.4.6/aiosmb/external/aiocmd/aiocmd/nested_completer.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/external/aiocmd/setup.py` & `aiosmb-0.4.6/aiosmb/external/aiocmd/setup.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/external/asciitree/asciitree/__init__.py` & `aiosmb-0.4.6/aiosmb/external/asciitree/asciitree/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/external/asciitree/asciitree/drawing.py` & `aiosmb-0.4.6/aiosmb/external/asciitree/asciitree/drawing.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/external/asciitree/asciitree/traversal.py` & `aiosmb-0.4.6/aiosmb/external/asciitree/asciitree/traversal.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/external/asciitree/setup.py` & `aiosmb-0.4.6/aiosmb/external/asciitree/setup.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/common.py` & `aiosmb-0.4.6/aiosmb/protocol/common.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/compression/lznt1.py` & `aiosmb-0.4.6/aiosmb/protocol/compression/lznt1.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb/command_codes.py` & `aiosmb-0.4.6/aiosmb/protocol/smb/command_codes.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb/commands/negotiate.py` & `aiosmb-0.4.6/aiosmb/protocol/smb/commands/negotiate.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb/commons.py` & `aiosmb-0.4.6/aiosmb/protocol/smb/commons.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb/header.py` & `aiosmb-0.4.6/aiosmb/protocol/smb/header.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb/message.py` & `aiosmb-0.4.6/aiosmb/protocol/smb/message.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/command_codes.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/command_codes.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/__init__.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/cancel.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/cancel.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/close.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/close.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/create.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/create.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/echo.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/echo.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/error.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/error.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/flush.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/flush.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/ioctl.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/ioctl.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/logoff.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/logoff.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/negotiate.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/negotiate.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/query_directory.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/query_directory.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/query_info.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/query_info.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/read.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/read.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/sessionsetup.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/sessionsetup.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/tree_connect.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/tree_connect.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/tree_disconnect.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/tree_disconnect.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/commands/write.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/commands/write.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/headers/asynch.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/headers/asynch.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/headers/common.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/headers/common.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/headers/compression.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/headers/compression.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/headers/sync.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/headers/sync.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/headers/transform.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/headers/transform.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/protocol/smb2/message.py` & `aiosmb-0.4.6/aiosmb/protocol/smb2/message.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/transport/netbios.py` & `aiosmb-0.4.6/aiosmb/transport/netbios.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/wintypes/access_mask.py` & `aiosmb-0.4.6/aiosmb/wintypes/access_mask.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/ace.py` & `aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/ace.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/acl.py` & `aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/acl.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/guid.py` & `aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/guid.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/security_descriptor.py` & `aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/security_descriptor.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/security_information.py` & `aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/security_information.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/wintypes/dtyp/constrcuted_security/sid.py` & `aiosmb-0.4.6/aiosmb/wintypes/dtyp/constrcuted_security/sid.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/wintypes/dtyp/structures/filetime.py` & `aiosmb-0.4.6/aiosmb/wintypes/dtyp/structures/filetime.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/wintypes/fscc/FileAttributes.py` & `aiosmb-0.4.6/aiosmb/wintypes/fscc/FileAttributes.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/wintypes/fscc/structures/FileFullDirectoryInformation.py` & `aiosmb-0.4.6/aiosmb/wintypes/fscc/structures/FileFullDirectoryInformation.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/wintypes/fscc/structures/fileinfoclass.py` & `aiosmb-0.4.6/aiosmb/wintypes/fscc/structures/fileinfoclass.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb/wintypes/ntstatus.py` & `aiosmb-0.4.6/aiosmb/wintypes/ntstatus.py`

 * *Files identical despite different names*

### Comparing `aiosmb-0.4.4/aiosmb.egg-info/SOURCES.txt` & `aiosmb-0.4.6/aiosmb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 aiosmb/__init__.py
 aiosmb/_version.py
 aiosmb/connection.py
-aiosmb/serverconnection.py
 aiosmb.egg-info/PKG-INFO
 aiosmb.egg-info/SOURCES.txt
 aiosmb.egg-info/dependency_links.txt
 aiosmb.egg-info/entry_points.txt
 aiosmb.egg-info/not-zip-safe
 aiosmb.egg-info/requires.txt
 aiosmb.egg-info/top_level.txt
@@ -54,14 +54,15 @@
 aiosmb/dcerpc/v5/connection.py
 aiosmb/dcerpc/v5/drsuapi.py
 aiosmb/dcerpc/v5/dtypes.py
 aiosmb/dcerpc/v5/enum.py
 aiosmb/dcerpc/v5/epm.py
 aiosmb/dcerpc/v5/even.py
 aiosmb/dcerpc/v5/even6.py
+aiosmb/dcerpc/v5/gkdi.py
 aiosmb/dcerpc/v5/hresult_errors.py
 aiosmb/dcerpc/v5/icpr.py
 aiosmb/dcerpc/v5/lsad.py
 aiosmb/dcerpc/v5/lsat.py
 aiosmb/dcerpc/v5/ndr.py
 aiosmb/dcerpc/v5/nrpc.py
 aiosmb/dcerpc/v5/par.py
@@ -89,14 +90,15 @@
 aiosmb/dcerpc/v5/common/even6/binxml.py
 aiosmb/dcerpc/v5/common/even6/resultset.py
 aiosmb/dcerpc/v5/interfaces/__init__.py
 aiosmb/dcerpc/v5/interfaces/bkrp.py
 aiosmb/dcerpc/v5/interfaces/drsuapimgr.py
 aiosmb/dcerpc/v5/interfaces/endpointmgr.py
 aiosmb/dcerpc/v5/interfaces/even6.py
+aiosmb/dcerpc/v5/interfaces/gkdimgr.py
 aiosmb/dcerpc/v5/interfaces/icprmgr.py
 aiosmb/dcerpc/v5/interfaces/lsatmgr.py
 aiosmb/dcerpc/v5/interfaces/parmgr.py
 aiosmb/dcerpc/v5/interfaces/remoteregistry.py
 aiosmb/dcerpc/v5/interfaces/rprnmgr.py
 aiosmb/dcerpc/v5/interfaces/samrmgr.py
 aiosmb/dcerpc/v5/interfaces/servicemanager.py
@@ -191,14 +193,17 @@
 aiosmb/protocol/smb2/commands/write.py
 aiosmb/protocol/smb2/headers/__init__.py
 aiosmb/protocol/smb2/headers/asynch.py
 aiosmb/protocol/smb2/headers/common.py
 aiosmb/protocol/smb2/headers/compression.py
 aiosmb/protocol/smb2/headers/sync.py
 aiosmb/protocol/smb2/headers/transform.py
+aiosmb/relay/__init__.py
+aiosmb/relay/server.py
+aiosmb/relay/serverconnection.py
 aiosmb/transport/__init__.py
 aiosmb/transport/netbios.py
 aiosmb/wintypes/__init__.py
 aiosmb/wintypes/access_mask.py
 aiosmb/wintypes/ntstatus.py
 aiosmb/wintypes/dtyp/__init__.py
 aiosmb/wintypes/dtyp/constrcuted_security/__init__.py
```

### Comparing `aiosmb-0.4.4/setup.py` & `aiosmb-0.4.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	version=verstr,
 
 	# Application author details:
 	author="Tamas Jos",
 	author_email="info@skelsecprojects.com",
 
 	# Packages
-	packages=find_packages(),
+	packages=find_packages(exclude=["tests*"]),
 
 	# Include additional files into the package
 	include_package_data=True,
 
 
 	# Details
 	url="https://github.com/skelsec/aiosmb",
@@ -35,20 +35,19 @@
 	#
 	# license="LICENSE.txt",
 	description="Asynchronous SMB protocol implementation",
 
 	# long_description=open("README.txt").read(),
 	python_requires='>=3.7',
 	install_requires=[
-		'unicrypto>=0.0.9',
-		'asyauth>=0.0.8',
-		'asysocks>=0.2.2',
-		'minikerberos>=0.3.5',
+		'unicrypto==0.0.10',
+		'asyauth==0.0.14',
+		'asysocks==0.2.7',
 		'prompt-toolkit>=3.0.2',
-		'winacl>=0.1.5',
+		'winacl==0.1.7',
 		'six',
 		'tqdm',
 		'colorama',
 		'asn1crypto',
 		'wcwidth',
 	],
```

