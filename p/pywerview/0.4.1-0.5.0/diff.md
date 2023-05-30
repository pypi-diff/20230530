# Comparing `tmp/pywerview-0.4.1.tar.gz` & `tmp/pywerview-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywerview-0.4.1.tar", last modified: Thu Jan 26 15:10:44 2023, max compression
+gzip compressed data, was "pywerview-0.5.0.tar", last modified: Tue May 30 16:01:23 2023, max compression
```

## Comparing `pywerview-0.4.1.tar` & `pywerview-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 yme       (1000) yme       (1000)        0 2023-01-26 15:10:44.856761 pywerview-0.4.1/
--rw-r--r--   0 yme       (1000) yme       (1000)    35147 2020-04-21 15:38:28.000000 pywerview-0.4.1/LICENSE
--rw-r--r--   0 yme       (1000) yme       (1000)       26 2020-04-21 15:38:28.000000 pywerview-0.4.1/MANIFEST.in
--rw-rw-r--   0 yme       (1000) yme       (1000)    16136 2023-01-26 15:10:44.856761 pywerview-0.4.1/PKG-INFO
--rw-rw-r--   0 yme       (1000) yme       (1000)    15545 2023-01-26 14:59:18.000000 pywerview-0.4.1/README.md
-drwxrwxr-x   0 yme       (1000) yme       (1000)        0 2023-01-26 15:10:44.856761 pywerview-0.4.1/pywerview/
--rw-rw-r--   0 yme       (1000) yme       (1000)       50 2022-04-13 07:59:16.000000 pywerview-0.4.1/pywerview/__init__.py
-drwxrwxr-x   0 yme       (1000) yme       (1000)        0 2023-01-26 15:10:44.856761 pywerview-0.4.1/pywerview/cli/
--rw-r--r--   0 yme       (1000) yme       (1000)        0 2020-04-21 15:38:28.000000 pywerview-0.4.1/pywerview/cli/__init__.py
--rw-rw-r--   0 yme       (1000) yme       (1000)    24897 2023-01-26 14:59:18.000000 pywerview-0.4.1/pywerview/cli/helpers.py
--rw-rw-r--   0 yme       (1000) yme       (1000)    37937 2023-01-26 14:59:18.000000 pywerview-0.4.1/pywerview/cli/main.py
--rw-rw-r--   0 yme       (1000) yme       (1000)     6635 2023-01-26 14:59:18.000000 pywerview-0.4.1/pywerview/formatters.py
-drwxrwxr-x   0 yme       (1000) yme       (1000)        0 2023-01-26 15:10:44.856761 pywerview-0.4.1/pywerview/functions/
--rw-r--r--   0 yme       (1000) yme       (1000)        0 2020-04-21 15:38:28.000000 pywerview-0.4.1/pywerview/functions/__init__.py
--rw-rw-r--   0 yme       (1000) yme       (1000)    25619 2023-01-26 14:59:18.000000 pywerview-0.4.1/pywerview/functions/gpo.py
--rw-rw-r--   0 yme       (1000) yme       (1000)    14138 2023-01-26 14:59:18.000000 pywerview-0.4.1/pywerview/functions/hunting.py
--rw-rw-r--   0 yme       (1000) yme       (1000)     3304 2023-01-26 14:59:18.000000 pywerview-0.4.1/pywerview/functions/misc.py
--rw-rw-r--   0 yme       (1000) yme       (1000)    46312 2023-01-26 14:59:18.000000 pywerview-0.4.1/pywerview/functions/net.py
-drwxrwxr-x   0 yme       (1000) yme       (1000)        0 2023-01-26 15:10:44.856761 pywerview-0.4.1/pywerview/objects/
--rw-r--r--   0 yme       (1000) yme       (1000)        0 2020-04-21 15:38:28.000000 pywerview-0.4.1/pywerview/objects/__init__.py
--rw-rw-r--   0 yme       (1000) yme       (1000)     9520 2023-01-26 14:59:18.000000 pywerview-0.4.1/pywerview/objects/adobjects.py
--rw-rw-r--   0 yme       (1000) yme       (1000)     3087 2023-01-26 14:59:18.000000 pywerview-0.4.1/pywerview/objects/rpcobjects.py
--rw-rw-r--   0 yme       (1000) yme       (1000)    22053 2023-01-26 14:59:18.000000 pywerview-0.4.1/pywerview/requester.py
-drwxrwxr-x   0 yme       (1000) yme       (1000)        0 2023-01-26 15:10:44.856761 pywerview-0.4.1/pywerview/worker/
--rw-r--r--   0 yme       (1000) yme       (1000)        0 2020-04-21 15:38:28.000000 pywerview-0.4.1/pywerview/worker/__init__.py
--rw-rw-r--   0 yme       (1000) yme       (1000)     6947 2023-01-26 14:59:18.000000 pywerview-0.4.1/pywerview/worker/hunting.py
-drwxrwxr-x   0 yme       (1000) yme       (1000)        0 2023-01-26 15:10:44.856761 pywerview-0.4.1/pywerview.egg-info/
--rw-rw-r--   0 yme       (1000) yme       (1000)    16136 2023-01-26 15:10:44.000000 pywerview-0.4.1/pywerview.egg-info/PKG-INFO
--rw-rw-r--   0 yme       (1000) yme       (1000)      717 2023-01-26 15:10:44.000000 pywerview-0.4.1/pywerview.egg-info/SOURCES.txt
--rw-rw-r--   0 yme       (1000) yme       (1000)       78 2023-01-26 15:10:44.000000 pywerview-0.4.1/pywerview.egg-info/dependency_links.txt
--rw-rw-r--   0 yme       (1000) yme       (1000)       55 2023-01-26 15:10:44.000000 pywerview-0.4.1/pywerview.egg-info/entry_points.txt
--rw-rw-r--   0 yme       (1000) yme       (1000)        1 2021-02-11 10:59:55.000000 pywerview-0.4.1/pywerview.egg-info/not-zip-safe
--rw-rw-r--   0 yme       (1000) yme       (1000)       77 2023-01-26 15:10:44.000000 pywerview-0.4.1/pywerview.egg-info/requires.txt
--rw-rw-r--   0 yme       (1000) yme       (1000)       10 2023-01-26 15:10:44.000000 pywerview-0.4.1/pywerview.egg-info/top_level.txt
--rw-rw-r--   0 yme       (1000) yme       (1000)       79 2023-01-26 15:10:44.856761 pywerview-0.4.1/setup.cfg
--rw-rw-r--   0 yme       (1000) yme       (1000)     1245 2023-01-26 15:02:24.000000 pywerview-0.4.1/setup.py
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.565161 pywerview-0.5.0/
+-rw-rw-r--   0 szi       (1000) szi       (1000)    35147 2021-03-17 13:39:19.000000 pywerview-0.5.0/LICENSE
+-rw-rw-r--   0 szi       (1000) szi       (1000)       26 2021-03-17 13:39:19.000000 pywerview-0.5.0/MANIFEST.in
+-rw-rw-r--   0 szi       (1000) szi       (1000)    18122 2023-05-30 16:01:23.569161 pywerview-0.5.0/PKG-INFO
+-rw-rw-r--   0 szi       (1000) szi       (1000)    17551 2023-05-30 15:59:15.000000 pywerview-0.5.0/README.md
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.561161 pywerview-0.5.0/pywerview/
+-rw-rw-r--   0 szi       (1000) szi       (1000)       50 2022-04-13 08:50:48.000000 pywerview-0.5.0/pywerview/__init__.py
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.565161 pywerview-0.5.0/pywerview/cli/
+-rw-rw-r--   0 szi       (1000) szi       (1000)        0 2021-03-17 13:39:19.000000 pywerview-0.5.0/pywerview/cli/__init__.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)    26577 2023-05-24 15:55:25.000000 pywerview-0.5.0/pywerview/cli/helpers.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)    39496 2023-05-24 15:55:25.000000 pywerview-0.5.0/pywerview/cli/main.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)     7101 2023-05-24 15:55:25.000000 pywerview-0.5.0/pywerview/formatters.py
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.565161 pywerview-0.5.0/pywerview/functions/
+-rw-rw-r--   0 szi       (1000) szi       (1000)        0 2021-03-17 13:39:19.000000 pywerview-0.5.0/pywerview/functions/__init__.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)    25619 2023-01-26 10:46:48.000000 pywerview-0.5.0/pywerview/functions/gpo.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)    14138 2023-01-26 10:46:48.000000 pywerview-0.5.0/pywerview/functions/hunting.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)     3387 2023-05-24 15:55:25.000000 pywerview-0.5.0/pywerview/functions/misc.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)    46585 2023-05-30 15:59:39.000000 pywerview-0.5.0/pywerview/functions/net.py
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.565161 pywerview-0.5.0/pywerview/objects/
+-rw-rw-r--   0 szi       (1000) szi       (1000)        0 2021-03-17 13:39:19.000000 pywerview-0.5.0/pywerview/objects/__init__.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)     7519 2023-05-24 15:55:25.000000 pywerview-0.5.0/pywerview/objects/adobjects.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)     3087 2023-01-26 10:46:48.000000 pywerview-0.5.0/pywerview/objects/rpcobjects.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)    25526 2023-05-30 15:59:15.000000 pywerview-0.5.0/pywerview/requester.py
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.565161 pywerview-0.5.0/pywerview/worker/
+-rw-rw-r--   0 szi       (1000) szi       (1000)        0 2021-03-17 13:39:19.000000 pywerview-0.5.0/pywerview/worker/__init__.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)     6947 2023-01-26 10:46:48.000000 pywerview-0.5.0/pywerview/worker/hunting.py
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.565161 pywerview-0.5.0/pywerview.egg-info/
+-rw-rw-r--   0 szi       (1000) szi       (1000)    18122 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/PKG-INFO
+-rw-rw-r--   0 szi       (1000) szi       (1000)      717 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/SOURCES.txt
+-rw-rw-r--   0 szi       (1000) szi       (1000)       78 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/dependency_links.txt
+-rw-rw-r--   0 szi       (1000) szi       (1000)       54 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/entry_points.txt
+-rw-rw-r--   0 szi       (1000) szi       (1000)        1 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/not-zip-safe
+-rw-rw-r--   0 szi       (1000) szi       (1000)       77 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/requires.txt
+-rw-rw-r--   0 szi       (1000) szi       (1000)       10 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/top_level.txt
+-rw-rw-r--   0 szi       (1000) szi       (1000)       79 2023-05-30 16:01:23.569161 pywerview-0.5.0/setup.cfg
+-rw-rw-r--   0 szi       (1000) szi       (1000)     1245 2023-05-24 15:55:25.000000 pywerview-0.5.0/setup.py
```

### Comparing `pywerview-0.4.1/LICENSE` & `pywerview-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywerview-0.4.1/PKG-INFO` & `pywerview-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pywerview
-Version: 0.4.1
+Version: 0.5.0
 Summary: A Python port of PowerSploit's PowerView
 Home-page: https://github.com/the-useless-one/pywerview
 Author: Yannick Méheut
 Author-email: yannick@meheut.org
 License: GNU GPLv3
 Keywords: python powersploit pentesting recon active directory windows
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Security
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -100,47 +99,61 @@
 
     Subcommands:
       Available subcommands
 
       {get-adobject,get-adserviceaccount,get-objectacl,get-netuser,get-netgroup,get-netcomputer,get-netdomaincontroller,get-netfileserver,get-dfsshare,get-netou,get-netsite,get-netsubnet,get-netdomaintrust,get-netgpo,get-netpso,get-domainpolicy,get-gpttmpl,get-netgpogroup,find-gpocomputeradmin,find-gpolocation,get-netgroupmember,get-netsession,get-localdisks,get-netdomain,get-netshare,get-netloggedon,get-netlocalgroup,invoke-checklocaladminaccess,get-netprocess,get-userevent,invoke-userhunter,invoke-processhunter,invoke-eventhunter}
         get-adobject        Takes a domain SID, samAccountName or name, and return the associated object
         get-adserviceaccount
-                            Returns a list of all the gMSA of the specified domain (you need privileged account to retrieve passwords)
-        get-objectacl       Takes a domain SID, samAccountName or name, and return the ACL of the associated object
+                            Returns a list of all the gMSA of the specified domain. To retrieve passwords,
+                            you need a privileged account and a TLS connection to the LDAP server (use the
+                            --tls switch).
+        get-objectacl       Takes a domain SID, samAccountName or name, and return the ACL of the
+                            associated object
         get-netuser         Queries information about a domain user
-        get-netgroup        Get a list of all current domain groups, or a list of groups a domain user is member of
+        get-netgroup        Get a list of all current domain groups, or a list of groups a domain user is
+                            member of
         get-netcomputer     Queries informations about domain computers
         get-netdomaincontroller
                             Get a list of domain controllers for the given domain
-        get-netfileserver   Return a list of file servers, extracted from the domain users' homeDirectory, scriptPath, and profilePath fields
+        get-netfileserver   Return a list of file servers, extracted from the domain users' homeDirectory,
+                            scriptPath, and profilePath fields
         get-dfsshare        Return a list of all fault tolerant distributed file systems for a given domain
         get-netou           Get a list of all current OUs in the domain
         get-netsite         Get a list of all current sites in the domain
         get-netsubnet       Get a list of all current subnets in the domain
         get-netdomaintrust  Returns a list of all the trusts of the specified domain
         get-netgpo          Get a list of all current GPOs in the domain
         get-netpso          Get a list of all current PSOs in the domain
         get-domainpolicy    Returns the default domain or DC policy for the queried domain or DC
         get-gpttmpl         Helper to parse a GptTmpl.inf policy file path into a custom object
         get-netgpogroup     Parses all GPOs in the domain that set "Restricted Group" or "Groups.xml"
         find-gpocomputeradmin
-                            Takes a computer (or OU) and determine who has administrative access to it via GPO
-        find-gpolocation    Takes a username or a group name and determine the computers it has administrative access to via GPO
+                            Takes a computer (or OU) and determine who has administrative access to it via
+                            GPO
+        find-gpolocation    Takes a username or a group name and determine the computers it has
+                            administrative access to via GPO
         get-netgroupmember  Return a list of members of a domain group
-        get-netsession      Queries a host to return a list of active sessions on the host (you can use local credentials instead of domain credentials)
-        get-localdisks      Queries a host to return a list of active disks on the host (you can use local credentials instead of domain credentials)
+        get-netsession      Queries a host to return a list of active sessions on the host (you can use
+                            local credentials instead of domain credentials)
+        get-localdisks      Queries a host to return a list of active disks on the host (you can use local
+                            credentials instead of domain credentials)
         get-netdomain       Queries a host for available domains
-        get-netshare        Queries a host to return a list of available shares on the host (you can use local credentials instead of domain credentials)
-        get-netloggedon     This function will execute the NetWkstaUserEnum RPC call to query a given host for actively logged on users
-        get-netlocalgroup   Gets a list of members of a local group on a machine, or returns every local group. You can use local credentials instead of domain credentials, however, domain credentials are needed
-                            to resolve domain SIDs.
+        get-netshare        Queries a host to return a list of available shares on the host (you can use
+                            local credentials instead of domain credentials)
+        get-netloggedon     This function will execute the NetWkstaUserEnum RPC call to query a given host
+                            for actively logged on users
+        get-netlocalgroup   Gets a list of members of a local group on a machine, or returns every local
+                            group. You can use local credentials instead of domain credentials, however,
+                            domain credentials are needed to resolve domain SIDs.
         invoke-checklocaladminaccess
                             Checks if the given user has local admin access on the given host
-        get-netprocess      This function will execute the 'Select * from Win32_Process' WMI query to a given host for a list of executed process
-        get-userevent       This function will execute the 'SELECT * from Win32_NTLogEvent' WMI query to a given host for a list of executed process
+        get-netprocess      This function will execute the 'Select * from Win32_Process' WMI query to a
+                            given host for a list of executed process
+        get-userevent       This function will execute the 'SELECT * from Win32_NTLogEvent' WMI query to a
+                            given host for a list of executed process
         invoke-userhunter   Finds which machines domain users are logged into
         invoke-processhunter
                             Searches machines for processes with specific name, or ran by specific users
         invoke-eventhunter  Searches machines for events with specific name, or ran by specific users
 
 Take a look at the [wiki](https://github.com/the-useless-one/pywerview/wiki) to
 see a more detailed usage of every command.
@@ -150,15 +163,15 @@
 
 For example, my domain name is `uselessdomain.local`. The Win2K compatible name
 is `USELESSDOMAIN`. In every command,  I must use __`uselessdomain.local`__ as
 an argument, and __not__ `USELESSDOMAIN`.
 
 ## GLOBAL ARGUMENTS
 
-### LOGGING
+### Logging
 
 You can provide a logging level to `pywerview` modules by using `-l` or `--logging-level` options. Supported levels are:
 
 * `CRITICAL`: Only critical errors are displayed **(default)**
 * `WARNING` Warnings are displayed, along with citical errors
 * `DEBUG`: Debug level (caution: **very** verbose)
 * `ULTRA`: Extreme debugging level (caution: **very very** verbose)
@@ -233,18 +246,57 @@
 ```
 
 To recap:
 
 |           SPN in the ticket           | Can be used with LDAP functions | Can be used with SMB/RPC functions |
 | :-----------------------------------: | :-----------------------------: | :--------------------------------: |
 | `ldap/srv-ad.contoso.com@CONTOSO.COM` |              ✔️                  |                 ✔️                  |
-| `cifs/srv-ad.contoso.com@CONTOSO.COm` |              ✔️                  |                 ✔️                  |
+| `cifs/srv-ad.contoso.com@CONTOSO.COM` |              ✔️                  |                 ✔️                  |
 |       `ldap/srv-ad@CONTOSO.COM`       |              ❌                 |                 ✔️                  |
 
-### TLS CONNECTION
+*NOTE:* The same limitation exists for TGT in your cache credential file: `krbtgt/srv-ad.contoso.com@CONTOSO.COM` will work 
+but not `krbtgt/srv-ad@CONTOSO.COM`.
+
+### LDAP SChannel authentication
+
+SChannel authentication is supported for a subset of the submodules. Functions that support SChannel authentication are:
+
+* get-adobject
+* get-adserviceaccount
+* get-objectacl
+* get-netuser
+* get-netgroup
+* get-netcomputer
+* get-netdomaincontroller
+* get-netfileserver
+* get-netou
+* get-netsite
+* get-netsubnet
+* get-netdomaintrust
+* get-netpso
+* get-netgpo
+* get-netgroupmember
+
+To authenticate via SChannel:
+
+1. Retrieve the certificate and the key with your favorite tool ([ntlmrelayx.py](https://github.com/fortra/impacket), [certipy](https://github.com/ly4k/Certipy),...)
+2. `pywerview` needs a certificate file and a key file, so you need to extract them from the `.pfx`.
+3. Use `--cert` and  `--key` as in the following example:
+
+```console
+$ python3 pywerview.py get-netuser -w contoso.com --dc-ip 172.16.0.55 --cert stormtroopers.crt --key stormtroopers.key --username administrator --attributes distinguishedname useraccountcontrol --tls
+distinguishedname:  CN=Administrator,CN=Users,DC=contoso,DC=com
+useraccountcontrol: NORMAL_ACCOUNT
+
+```
+
+If you don't specify the `--tls` flag when using certificate authentication, `pywerview` will try to use StartTLS and an `EXTERNAL SASL` bind 
+as described in the [Microsoft documentation](https://learn.microsoft.com/en-us/openspecs/windows_protocols/ms-adts/8e73932f-70cf-46d6-88b1-8d9f86235e81)
+
+### TLS connection
 
 You can force a connection to the LDAPS port by using the `--tls` switch. It
 can be necessary with some functions, for example when retrieving gMSA
 passwords with `get-adserviceaccount`:
 
 ```console
 $ python3 pywerview.py get-adserviceaccount -t srv-ad.contoso.com -u 'SRV-MAIL$' --hashes $NT_HASH --resolve-sids
@@ -260,15 +312,15 @@
 samaccountname:          gMSA-01$
 msds-managedpassword:    69730ce3914ac6[redacted]
 msds-groupmsamembership: CN=SRV-MAIL,CN=Computers,DC=contoso,DC=com
 description:
 enabled:                 True
 ```
 
-### JSON OUTPUT
+### JSON output
 
 Pywerview can print results in json format by using the `--json` switch.
 
 ## TODO
 
 * Many, many more PowerView functionalities to implement. I'll now focus on
   forest functions, then inter-forest trust functions
@@ -309,9 +361,7 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
 Public License for more details.
 
 You should have received a copy of the GNU General Public License along
 with this program. If not, see
 [https://www.gnu.org/licenses/](https://www.gnu.org/licenses/).
 
-
-
```

### Comparing `pywerview-0.4.1/README.md` & `pywerview-0.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -83,47 +83,61 @@
 
     Subcommands:
       Available subcommands
 
       {get-adobject,get-adserviceaccount,get-objectacl,get-netuser,get-netgroup,get-netcomputer,get-netdomaincontroller,get-netfileserver,get-dfsshare,get-netou,get-netsite,get-netsubnet,get-netdomaintrust,get-netgpo,get-netpso,get-domainpolicy,get-gpttmpl,get-netgpogroup,find-gpocomputeradmin,find-gpolocation,get-netgroupmember,get-netsession,get-localdisks,get-netdomain,get-netshare,get-netloggedon,get-netlocalgroup,invoke-checklocaladminaccess,get-netprocess,get-userevent,invoke-userhunter,invoke-processhunter,invoke-eventhunter}
         get-adobject        Takes a domain SID, samAccountName or name, and return the associated object
         get-adserviceaccount
-                            Returns a list of all the gMSA of the specified domain (you need privileged account to retrieve passwords)
-        get-objectacl       Takes a domain SID, samAccountName or name, and return the ACL of the associated object
+                            Returns a list of all the gMSA of the specified domain. To retrieve passwords,
+                            you need a privileged account and a TLS connection to the LDAP server (use the
+                            --tls switch).
+        get-objectacl       Takes a domain SID, samAccountName or name, and return the ACL of the
+                            associated object
         get-netuser         Queries information about a domain user
-        get-netgroup        Get a list of all current domain groups, or a list of groups a domain user is member of
+        get-netgroup        Get a list of all current domain groups, or a list of groups a domain user is
+                            member of
         get-netcomputer     Queries informations about domain computers
         get-netdomaincontroller
                             Get a list of domain controllers for the given domain
-        get-netfileserver   Return a list of file servers, extracted from the domain users' homeDirectory, scriptPath, and profilePath fields
+        get-netfileserver   Return a list of file servers, extracted from the domain users' homeDirectory,
+                            scriptPath, and profilePath fields
         get-dfsshare        Return a list of all fault tolerant distributed file systems for a given domain
         get-netou           Get a list of all current OUs in the domain
         get-netsite         Get a list of all current sites in the domain
         get-netsubnet       Get a list of all current subnets in the domain
         get-netdomaintrust  Returns a list of all the trusts of the specified domain
         get-netgpo          Get a list of all current GPOs in the domain
         get-netpso          Get a list of all current PSOs in the domain
         get-domainpolicy    Returns the default domain or DC policy for the queried domain or DC
         get-gpttmpl         Helper to parse a GptTmpl.inf policy file path into a custom object
         get-netgpogroup     Parses all GPOs in the domain that set "Restricted Group" or "Groups.xml"
         find-gpocomputeradmin
-                            Takes a computer (or OU) and determine who has administrative access to it via GPO
-        find-gpolocation    Takes a username or a group name and determine the computers it has administrative access to via GPO
+                            Takes a computer (or OU) and determine who has administrative access to it via
+                            GPO
+        find-gpolocation    Takes a username or a group name and determine the computers it has
+                            administrative access to via GPO
         get-netgroupmember  Return a list of members of a domain group
-        get-netsession      Queries a host to return a list of active sessions on the host (you can use local credentials instead of domain credentials)
-        get-localdisks      Queries a host to return a list of active disks on the host (you can use local credentials instead of domain credentials)
+        get-netsession      Queries a host to return a list of active sessions on the host (you can use
+                            local credentials instead of domain credentials)
+        get-localdisks      Queries a host to return a list of active disks on the host (you can use local
+                            credentials instead of domain credentials)
         get-netdomain       Queries a host for available domains
-        get-netshare        Queries a host to return a list of available shares on the host (you can use local credentials instead of domain credentials)
-        get-netloggedon     This function will execute the NetWkstaUserEnum RPC call to query a given host for actively logged on users
-        get-netlocalgroup   Gets a list of members of a local group on a machine, or returns every local group. You can use local credentials instead of domain credentials, however, domain credentials are needed
-                            to resolve domain SIDs.
+        get-netshare        Queries a host to return a list of available shares on the host (you can use
+                            local credentials instead of domain credentials)
+        get-netloggedon     This function will execute the NetWkstaUserEnum RPC call to query a given host
+                            for actively logged on users
+        get-netlocalgroup   Gets a list of members of a local group on a machine, or returns every local
+                            group. You can use local credentials instead of domain credentials, however,
+                            domain credentials are needed to resolve domain SIDs.
         invoke-checklocaladminaccess
                             Checks if the given user has local admin access on the given host
-        get-netprocess      This function will execute the 'Select * from Win32_Process' WMI query to a given host for a list of executed process
-        get-userevent       This function will execute the 'SELECT * from Win32_NTLogEvent' WMI query to a given host for a list of executed process
+        get-netprocess      This function will execute the 'Select * from Win32_Process' WMI query to a
+                            given host for a list of executed process
+        get-userevent       This function will execute the 'SELECT * from Win32_NTLogEvent' WMI query to a
+                            given host for a list of executed process
         invoke-userhunter   Finds which machines domain users are logged into
         invoke-processhunter
                             Searches machines for processes with specific name, or ran by specific users
         invoke-eventhunter  Searches machines for events with specific name, or ran by specific users
 
 Take a look at the [wiki](https://github.com/the-useless-one/pywerview/wiki) to
 see a more detailed usage of every command.
@@ -133,15 +147,15 @@
 
 For example, my domain name is `uselessdomain.local`. The Win2K compatible name
 is `USELESSDOMAIN`. In every command,  I must use __`uselessdomain.local`__ as
 an argument, and __not__ `USELESSDOMAIN`.
 
 ## GLOBAL ARGUMENTS
 
-### LOGGING
+### Logging
 
 You can provide a logging level to `pywerview` modules by using `-l` or `--logging-level` options. Supported levels are:
 
 * `CRITICAL`: Only critical errors are displayed **(default)**
 * `WARNING` Warnings are displayed, along with citical errors
 * `DEBUG`: Debug level (caution: **very** verbose)
 * `ULTRA`: Extreme debugging level (caution: **very very** verbose)
@@ -216,18 +230,57 @@
 ```
 
 To recap:
 
 |           SPN in the ticket           | Can be used with LDAP functions | Can be used with SMB/RPC functions |
 | :-----------------------------------: | :-----------------------------: | :--------------------------------: |
 | `ldap/srv-ad.contoso.com@CONTOSO.COM` |              ✔️                  |                 ✔️                  |
-| `cifs/srv-ad.contoso.com@CONTOSO.COm` |              ✔️                  |                 ✔️                  |
+| `cifs/srv-ad.contoso.com@CONTOSO.COM` |              ✔️                  |                 ✔️                  |
 |       `ldap/srv-ad@CONTOSO.COM`       |              ❌                 |                 ✔️                  |
 
-### TLS CONNECTION
+*NOTE:* The same limitation exists for TGT in your cache credential file: `krbtgt/srv-ad.contoso.com@CONTOSO.COM` will work 
+but not `krbtgt/srv-ad@CONTOSO.COM`.
+
+### LDAP SChannel authentication
+
+SChannel authentication is supported for a subset of the submodules. Functions that support SChannel authentication are:
+
+* get-adobject
+* get-adserviceaccount
+* get-objectacl
+* get-netuser
+* get-netgroup
+* get-netcomputer
+* get-netdomaincontroller
+* get-netfileserver
+* get-netou
+* get-netsite
+* get-netsubnet
+* get-netdomaintrust
+* get-netpso
+* get-netgpo
+* get-netgroupmember
+
+To authenticate via SChannel:
+
+1. Retrieve the certificate and the key with your favorite tool ([ntlmrelayx.py](https://github.com/fortra/impacket), [certipy](https://github.com/ly4k/Certipy),...)
+2. `pywerview` needs a certificate file and a key file, so you need to extract them from the `.pfx`.
+3. Use `--cert` and  `--key` as in the following example:
+
+```console
+$ python3 pywerview.py get-netuser -w contoso.com --dc-ip 172.16.0.55 --cert stormtroopers.crt --key stormtroopers.key --username administrator --attributes distinguishedname useraccountcontrol --tls
+distinguishedname:  CN=Administrator,CN=Users,DC=contoso,DC=com
+useraccountcontrol: NORMAL_ACCOUNT
+
+```
+
+If you don't specify the `--tls` flag when using certificate authentication, `pywerview` will try to use StartTLS and an `EXTERNAL SASL` bind 
+as described in the [Microsoft documentation](https://learn.microsoft.com/en-us/openspecs/windows_protocols/ms-adts/8e73932f-70cf-46d6-88b1-8d9f86235e81)
+
+### TLS connection
 
 You can force a connection to the LDAPS port by using the `--tls` switch. It
 can be necessary with some functions, for example when retrieving gMSA
 passwords with `get-adserviceaccount`:
 
 ```console
 $ python3 pywerview.py get-adserviceaccount -t srv-ad.contoso.com -u 'SRV-MAIL$' --hashes $NT_HASH --resolve-sids
@@ -243,15 +296,15 @@
 samaccountname:          gMSA-01$
 msds-managedpassword:    69730ce3914ac6[redacted]
 msds-groupmsamembership: CN=SRV-MAIL,CN=Computers,DC=contoso,DC=com
 description:
 enabled:                 True
 ```
 
-### JSON OUTPUT
+### JSON output
 
 Pywerview can print results in json format by using the `--json` switch.
 
 ## TODO
 
 * Many, many more PowerView functionalities to implement. I'll now focus on
   forest functions, then inter-forest trust functions
```

### Comparing `pywerview-0.4.1/pywerview/cli/helpers.py` & `pywerview-0.5.0/pywerview/cli/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,154 +20,180 @@
 from pywerview.functions.net import NetRequester
 from pywerview.functions.gpo import GPORequester
 from pywerview.functions.misc import Misc
 from pywerview.functions.hunting import UserHunter, ProcessHunter, EventHunter
 
 def get_adobject(domain_controller, domain, user, password=str(),
                 lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
+                user_cert=str(), user_key=str(),
                 queried_domain=str(), queried_sid=str(), queried_name=str(),
                 queried_sam_account_name=str(), ads_path=str(), attributes=list(),
                 custom_filter=str()):
     requester = NetRequester(domain_controller, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls)
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
     return requester.get_adobject(queried_domain=queried_domain,
                     queried_sid=queried_sid, queried_name=queried_name,
                     queried_sam_account_name=queried_sam_account_name,
                     ads_path=ads_path, attributes=attributes, custom_filter=custom_filter)
 
 def get_adserviceaccount(domain_controller, domain, user, password=str(),
                 lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
+                user_cert=str(), user_key=str(),
                 queried_domain=str(), queried_sid=str(), queried_name=str(),
                 queried_sam_account_name=str(), ads_path=str(), resolve_sids=False):
     requester = NetRequester(domain_controller, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls)
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
     return requester.get_adserviceaccount(queried_domain=queried_domain,
                     queried_sid=queried_sid, queried_name=queried_name,
                     queried_sam_account_name=queried_sam_account_name,
                     ads_path=ads_path, resolve_sids=resolve_sids)
 
 def get_objectacl(domain_controller, domain, user, password=str(),
                 lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
                 queried_domain=str(), queried_sid=str(), queried_name=str(),
+                user_cert=str(), user_key=str(),
                 queried_sam_account_name=str(), ads_path=str(), sacl=False,
                 rights_filter=str(), resolve_sids=False, resolve_guids=False,
                 custom_filter=str()):
     requester = NetRequester(domain_controller, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls)
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
     return requester.get_objectacl(queried_domain=queried_domain,
                     queried_sid=queried_sid, queried_name=queried_name,
                     queried_sam_account_name=queried_sam_account_name,
                     ads_path=ads_path, sacl=sacl, rights_filter=rights_filter,
                     resolve_sids=resolve_sids, resolve_guids=resolve_guids,
                     custom_filter=custom_filter)
 
 def get_netuser(domain_controller, domain, user, password=str(), lmhash=str(),
-                nthash=str(), do_kerberos=False, do_tls=False, queried_username=str(),
+                nthash=str(), do_kerberos=False,  
+                user_cert=str(), user_key=str(), do_tls=False, queried_username=str(),
                 queried_domain=str(), ads_path=str(), admin_count=False, spn=False,
                 unconstrained=False, allow_delegation=False, preauth_notreq=False,
                 custom_filter=str(), attributes=[]):
     requester = NetRequester(domain_controller, domain, user, password,
-                             lmhash, nthash, do_kerberos, do_tls)
+                             lmhash, nthash, do_kerberos, do_tls,
+                             user_cert, user_key)
     return requester.get_netuser(queried_username=queried_username,
                                     queried_domain=queried_domain, ads_path=ads_path, admin_count=admin_count,
                                     spn=spn, unconstrained=unconstrained, allow_delegation=allow_delegation,
                                     preauth_notreq=preauth_notreq, custom_filter=custom_filter,
                                     attributes=attributes)
 
 def get_netgroup(domain_controller, domain, user, password=str(),
                 lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
+                user_cert=str(), user_key=str(),
                 queried_groupname='*', queried_sid=str(), queried_username=str(),
                 queried_domain=str(), ads_path=str(), admin_count=False,
                 full_data=False, custom_filter=str()):
     requester = NetRequester(domain_controller, domain, user, password,
-                                lmhash, nthash, do_kerberos, do_tls)
+                                lmhash, nthash, do_kerberos, do_tls,
+                                user_cert, user_key)
     return requester.get_netgroup(queried_groupname=queried_groupname,
                                     queried_sid=queried_sid, queried_username=queried_username,
                                     queried_domain=queried_domain, ads_path=ads_path, admin_count=admin_count,
                                     full_data=full_data, custom_filter=custom_filter)
 
 def get_netcomputer(domain_controller, domain, user, password=str(),
                     lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
+                    user_cert=str(), user_key=str(),
                     queried_computername=str(), queried_spn=str(), queried_os=str(),
                     queried_sp=str(), queried_domain=str(), ads_path=str(),
                     printers=False, unconstrained=False, laps_passwords=False, pre_created=False,
                     ping=False, full_data=False, custom_filter=str(), attributes=[]):
     requester = NetRequester(domain_controller, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls)
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
     return requester.get_netcomputer(queried_computername=queried_computername,
                                         queried_spn=queried_spn, queried_os=queried_os, queried_sp=queried_sp,
                                         queried_domain=queried_domain, ads_path=ads_path, printers=printers,
                                         unconstrained=unconstrained, laps_passwords=laps_passwords, 
                                         pre_created=pre_created, ping=ping, full_data=full_data, 
                                         custom_filter=custom_filter, attributes=attributes)
 
 def get_netdomaincontroller(domain_controller, domain, user, password=str(),
                                  lmhash=str(), nthash=str(), do_kerberos=False,
+                                 user_cert=str(), user_key=str(),
                                  do_tls=False, queried_domain=str()):
     requester = NetRequester(domain_controller, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls)
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
     return requester.get_netdomaincontroller(queried_domain=queried_domain)
 
 def get_netfileserver(domain_controller, domain, user, password=str(),
                                  lmhash=str(), nthash=str(), do_kerberos=False,
+                                 user_cert=str(), user_key=str(), 
                                  do_tls=False, queried_domain=str(), target_users=list()):
     requester = NetRequester(domain_controller, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls)
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
     return requester.get_netfileserver(queried_domain=queried_domain,
                                             target_users=target_users)
 
 def get_dfsshare(domain_controller, domain, user, password=str(),
                  lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
                  version=['v1', 'v2'], queried_domain=str(), ads_path=str()):
     requester = NetRequester(domain_controller, domain, user, password,
                                  lmhash, nthash, do_kerberos, do_tls)
     return requester.get_dfsshare(version=version, queried_domain=queried_domain, ads_path=ads_path)
 
 def get_netou(domain_controller, domain, user, password=str(), lmhash=str(),
               nthash=str(), do_kerberos=False, do_tls=False, queried_domain=str(),
-              queried_ouname='*', queried_guid=str(), ads_path=str(), full_data=False):
+              queried_ouname='*', queried_guid=str(), ads_path=str(), full_data=False,
+              user_cert=str(), user_key=str()):
     requester = NetRequester(domain_controller, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls)
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
     return requester.get_netou(queried_domain=queried_domain,
                                    queried_ouname=queried_ouname, queried_guid=queried_guid, ads_path=ads_path,
                                    full_data=full_data)
 
 def get_netsite(domain_controller, domain, user, password=str(), lmhash=str(),
                 nthash=str(), do_kerberos=False, do_tls=False, queried_domain=str(),
                 queried_sitename=str(), queried_guid=str(), ads_path=str(),
-                ads_prefix='CN=Sites,CN=Configuration', full_data=False):
+                ads_prefix='CN=Sites,CN=Configuration', full_data=False,
+                user_cert=str(), user_key=str()):
     requester = NetRequester(domain_controller, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls)
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
     return requester.get_netsite(queried_domain=queried_domain,
                                     queried_sitename=queried_sitename, queried_guid=queried_guid,
                                     ads_path=ads_path, ads_prefix=ads_prefix, full_data=full_data)
 
 def get_netsubnet(domain_controller, domain, user, password=str(),
                   lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
                   queried_domain=str(), queried_sitename=str(), ads_path=str(),
-                  ads_prefix='CN=Sites,CN=Configuration', full_data=False):
+                  ads_prefix='CN=Sites,CN=Configuration', full_data=False,
+                  user_cert=str(), user_key=str()):
     requester = NetRequester(domain_controller, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls)
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
     return requester.get_netsubnet(queried_domain=queried_domain,
                                        queried_sitename=queried_sitename, ads_path=ads_path, ads_prefix=ads_prefix,
                                        full_data=full_data)
 
 def get_netdomaintrust(domain_controller, domain, user, password=str(),
-                  lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False, queried_domain=str()):
+                  lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False, queried_domain=str(),
+                  user_cert=str(), user_key=str(), full_data=False):
     requester = NetRequester(domain_controller, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls)
-    return requester.get_netdomaintrust(queried_domain=queried_domain)
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
+    return requester.get_netdomaintrust(queried_domain=queried_domain, full_data=full_data)
 
 def get_netgroupmember(domain_controller, domain, user, password=str(),
                        lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
+                       user_cert=str(), user_key=str(),
                        queried_groupname=str(), queried_sid=str(), queried_domain=str(),
                        ads_path=str(), recurse=False, use_matching_rule=False,
                        full_data=False, custom_filter=str()):
     requester = NetRequester(domain_controller, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls)
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
     return requester.get_netgroupmember(queried_groupname=queried_groupname,
                                             queried_sid=queried_sid, queried_domain=queried_domain,
                                             ads_path=ads_path, recurse=recurse,
                                             use_matching_rule=use_matching_rule,
                                             full_data=full_data, custom_filter=custom_filter)
 
 def get_netsession(target_computername, domain, user, password=str(),
@@ -202,15 +228,16 @@
     return requester.get_netloggedon()
 
 def get_netlocalgroup(target_computername, domain_controller, domain, user,
                       password=str(), lmhash=str(), nthash=str(), do_kerberos=False,
                       do_tls=False, queried_groupname=str(), list_groups=False,
                       recurse=False):
     requester = NetRequester(target_computername, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls, domain_controller)
+                                 lmhash, nthash, do_kerberos, do_tls, 
+                                 domain_controller=domain_controller)
     return requester.get_netlocalgroup(queried_groupname=queried_groupname,
                                            list_groups=list_groups, recurse=recurse)
 
 def get_netprocess(target_computername, domain, user, password=str(),
                    lmhash=str(), nthash=str(), do_kerberos=False):
     requester = NetRequester(target_computername, domain, user, password,
                                  lmhash, nthash, do_kerberos)
@@ -222,28 +249,32 @@
     requester = NetRequester(target_computername, domain, user, password,
                                  lmhash, nthash, do_kerberos)
     return requester.get_userevent(event_type=event_type,
                                        date_start=date_start)
 
 def get_netgpo(domain_controller, domain, user, password=str(),
                lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
+               user_cert=str(), user_key=str(), 
                queried_gponame='*', queried_displayname=str(), queried_domain=str(),
                ads_path=str()):
     requester = GPORequester(domain_controller, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls)
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
     return requester.get_netgpo(queried_gponame=queried_gponame,
                                     queried_displayname=queried_displayname,
                                     queried_domain=queried_domain, ads_path=ads_path)
 
 def get_netpso(domain_controller, domain, user, password=str(),
                lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
+               user_cert=str(), user_key=str(), 
                queried_psoname='*', queried_displayname=str(), queried_domain=str(),
                ads_path=str()):
     requester = GPORequester(domain_controller, domain, user, password,
-                                 lmhash, nthash, do_kerberos, do_tls)
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
     return requester.get_netpso(queried_psoname=queried_psoname,
                                     queried_displayname=queried_displayname,
                                     queried_domain=queried_domain, ads_path=ads_path)
 
 def get_domainpolicy(domain_controller, domain, user, password=str(),
                      lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
                      source='domain', queried_domain=str(), resolve_sids=False):
```

### Comparing `pywerview-0.4.1/pywerview/cli/main.py` & `pywerview-0.5.0/pywerview/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
                  'ULTRA: Extreme debugging level (caution: very very verbose)')
     
     # json parser
     json_output_parser = argparse.ArgumentParser(add_help=False)
     json_output_parser.add_argument('--json', dest='json_output', action='store_true',
             help='Print results in JSON format')
 
-    # TODO: support keberos authentication
     # Credentials parser
     credentials_parser = argparse.ArgumentParser(add_help=False)
     credentials_parser.add_argument('-w', '--workgroup', dest='domain',
             default=str(), help='Name of the domain we authenticate with')
     credentials_parser.add_argument('-u', '--user',
             help='Username used to connect to the Domain Controller')
     credentials_parser.add_argument('-p', '--password',
@@ -60,14 +59,21 @@
             help='NTLM hashes, format is [LMHASH:]NTHASH')
     credentials_parser.add_argument('-k', action='store_true', dest='do_kerberos',
             help='Use Kerberos authentication. Grabs credentials from ccache file '
             '(KRB5CCNAME) based on target parameters. If valid credentials '
             'cannot be found, it will use the ones specified in the command '
             'line')
 
+    # Certificate authentication parser
+    certificate_parser = argparse.ArgumentParser(add_help=False)
+    certificate_parser.add_argument('--cert', dest='user_cert',
+            help='Certificatie associated to the user')
+    certificate_parser.add_argument('--key', dest='user_key',
+            help='Private key associated to the user')
+
     # AD parser, used for net* functions running against a domain controller
     ad_parser = argparse.ArgumentParser(add_help=False, parents=[credentials_parser])
     ad_parser.add_argument('-t', '--dc-ip', dest='domain_controller',
             required=True, help='IP address of the Domain Controller to target')
     ad_parser.add_argument('--tls', action='store_true', dest='do_tls',
             help='Force TLS connection to the Domain Controller')
 
@@ -102,34 +108,36 @@
             default=1, help='Number of threads to use (default: %(default)s)')
     hunter_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query for machines')
 
     # Parser for the get-adobject command
     get_adobject_parser = subparsers.add_parser('get-adobject', help='Takes a domain SID, '\
         'samAccountName or name, and return the associated object',
-        parents=[ad_parser, logging_parser, json_output_parser])
+        parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_adobject_parser.add_argument('--sid', dest='queried_sid',
             help='SID to query (wildcards accepted)')
     get_adobject_parser.add_argument('--sam-account-name', dest='queried_sam_account_name',
             help='samAccountName to query (wildcards accepted)')
     get_adobject_parser.add_argument('--name', dest='queried_name',
             help='Name to query (wildcards accepted)')
     get_adobject_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
     get_adobject_parser.add_argument('-a', '--ads-path',
             help='Additional ADS path')
+    get_adobject_parser.add_argument('--custom-filter', dest='custom_filter',
+            default=str(), help='Custom filter')
     get_adobject_parser.add_argument('--attributes', nargs='+', dest='attributes',
             default=[], help='Object attributes to return')
     get_adobject_parser.set_defaults(func=get_adobject)
 
     # Parser for the get-adserviceaccount command
     get_adserviceaccount_parser = subparsers.add_parser('get-adserviceaccount', help='Returns a list of all the '\
         'gMSA of the specified domain. To retrieve passwords, you need a privileged account and '\
         'a TLS connection to the LDAP server (use the --tls switch).',
-        parents=[ad_parser, logging_parser, json_output_parser])
+        parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_adserviceaccount_parser.add_argument('--sid', dest='queried_sid',
             help='SID to query (wildcards accepted)')
     get_adserviceaccount_parser.add_argument('--sam-account-name', dest='queried_sam_account_name',
             help='samAccountName to query (wildcards accepted)')
     get_adserviceaccount_parser.add_argument('--name', dest='queried_name',
             help='Name to query (wildcards accepted)')
     get_adserviceaccount_parser.add_argument('-d', '--domain', dest='queried_domain',
@@ -139,15 +147,15 @@
     get_adserviceaccount_parser.add_argument('--resolve-sids', dest='resolve_sids',
             action='store_true', help='Resolve SIDs when querying PrincipalsAllowedToRetrieveManagedPassword')
     get_adserviceaccount_parser.set_defaults(func=get_adserviceaccount)
     
     # Parser for the get-objectacl command
     get_objectacl_parser = subparsers.add_parser('get-objectacl', help='Takes a domain SID, '\
         'samAccountName or name, and return the ACL of the associated object',
-        parents=[ad_parser, logging_parser, json_output_parser])
+        parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_objectacl_parser.add_argument('--sid', dest='queried_sid',
             help='SID to query (wildcards accepted)')
     get_objectacl_parser.add_argument('--sam-account-name', dest='queried_sam_account_name',
             help='samAccountName to query (wildcards accepted)')
     get_objectacl_parser.add_argument('--name', dest='queried_name',
             help='Name to query (wildcards accepted)')
     get_objectacl_parser.add_argument('-d', '--domain', dest='queried_domain',
@@ -160,19 +168,21 @@
     get_objectacl_parser.add_argument('--rights-filter', dest='rights_filter',
             choices=['reset-password', 'write-members', 'allowed-to-authenticate', 'all'], help='A specific set of rights to return '\
                     '(reset-password, write-members, allowed-to-authenticate , all)')
     get_objectacl_parser.add_argument('--resolve-sids', dest='resolve_sids',
             action='store_true', help='Resolve SIDs when querying an ACL')
     get_objectacl_parser.add_argument('--resolve-guids', action='store_true',
             help='Resolve GUIDs to their display names')
+    get_objectacl_parser.add_argument('--custom-filter', dest='custom_filter',
+            default=str(), help='Custom filter')
     get_objectacl_parser.set_defaults(func=get_objectacl)
 
     # Parser for the get-netuser command
     get_netuser_parser = subparsers.add_parser('get-netuser', help='Queries information about '\
-        'a domain user', parents=[ad_parser, logging_parser, json_output_parser])
+        'a domain user', parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_netuser_parser.add_argument('--username', dest='queried_username',
             help='Username to query (wildcards accepted)')
     get_netuser_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
     get_netuser_parser.add_argument('-a', '--ads-path',
             help='Additional ADS path')
     get_netuser_parser.add_argument('--unconstrained', action='store_true',
@@ -190,34 +200,36 @@
     get_netuser_parser.add_argument('--attributes', nargs='+', dest='attributes',
             default=[], help='Object attributes to return')
     get_netuser_parser.set_defaults(func=get_netuser)
 
     # Parser for the get-netgroup command
     get_netgroup_parser = subparsers.add_parser('get-netgroup', help='Get a list of all current '\
         'domain groups, or a list of groups a domain user is member of',
-        parents=[ad_parser, logging_parser, json_output_parser])
+        parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_netgroup_parser.add_argument('--groupname', dest='queried_groupname',
             default='*', help='Group to query (wildcards accepted)')
     get_netgroup_parser.add_argument('--sid', dest='queried_sid',
             help='Group SID to query')
     get_netgroup_parser.add_argument('--username', dest='queried_username',
             help='Username to query: will list the groups this user is a member of (wildcards accepted)')
     get_netgroup_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
     get_netgroup_parser.add_argument('-a', '--ads-path', dest='ads_path',
             help='Additional ADS path')
     get_netgroup_parser.add_argument('--full-data', action='store_true',
             help='If set, returns full information on the groups, otherwise, just the samAccountName')
     get_netgroup_parser.add_argument('--admin-count', action='store_true',
             help='Query only users with adminCount=1')
+    get_netgroup_parser.add_argument('--custom-filter', dest='custom_filter',
+            default=str(), help='Custom filter')
     get_netgroup_parser.set_defaults(func=get_netgroup)
 
     # Parser for the get-netcomputer command
     get_netcomputer_parser = subparsers.add_parser('get-netcomputer', help='Queries informations about '\
-        'domain computers', parents=[ad_parser, logging_parser, json_output_parser])
+        'domain computers', parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_netcomputer_parser.add_argument('--computername', dest='queried_computername',
             default=str(), help='Computer name to query')
     get_netcomputer_parser.add_argument('-os', '--operating-system', dest='queried_os',
             help='Return computers with a specific operating system (wildcards accepted)')
     get_netcomputer_parser.add_argument('-sp', '--service-pack', dest='queried_sp',
             help='Return computers with a specific service pack (wildcards accepted)')
     get_netcomputer_parser.add_argument('-spn', '--service-principal-name', dest='queried_spn',
@@ -236,29 +248,32 @@
     get_netcomputer_parser.add_argument('--pre-created', action='store_true', dest='pre_created',
             help='Query only computers which are potentially vulnerable to "pre-created computer account" attack. '\
                  'Caution: This option is prone to false positives and negatives.')
     get_netcomputer_parser.add_argument('--ping', action='store_true',
             help='Ping computers (will only return up computers)')
     get_netcomputer_parser.add_argument('--full-data', action='store_true',
             help='If set, returns full information on the groups, otherwise, just the dnsHostName')
+    get_netcomputer_parser.add_argument('--custom-filter', dest='custom_filter',
+            default=str(), help='Custom filter')
     get_netcomputer_parser.add_argument('--attributes', nargs='+', dest='attributes',
             default=[], help='Object attributes to return')
     get_netcomputer_parser.set_defaults(func=get_netcomputer)
 
     # Parser for the get-netdomaincontroller command
     get_netdomaincontroller_parser = subparsers.add_parser('get-netdomaincontroller', help='Get a list of '\
-        'domain controllers for the given domain', parents=[ad_parser, logging_parser, json_output_parser])
+        'domain controllers for the given domain', parents=[ad_parser, logging_parser, 
+                                                             json_output_parser, certificate_parser])
     get_netdomaincontroller_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
     get_netdomaincontroller_parser.set_defaults(func=get_netdomaincontroller)
 
     # Parser for the get-netfileserver command
     get_netfileserver_parser = subparsers.add_parser('get-netfileserver', help='Return a list of '\
         'file servers, extracted from the domain users\' homeDirectory, scriptPath, and profilePath fields',
-        parents=[ad_parser, logging_parser, json_output_parser])
+        parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_netfileserver_parser.add_argument('--target-users', nargs='+',
             metavar='TARGET_USER', help='A list of users to target to find file servers (wildcards accepted)')
     get_netfileserver_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
     get_netfileserver_parser.set_defaults(func=get_netfileserver)
 
     # Parser for the get-dfsshare command
@@ -270,78 +285,80 @@
             default=['v1', 'v2'], help='The version of DFS to query for servers: v1, v2 or all (default: all)')
     get_dfsshare_parser.add_argument('-a', '--ads-path', dest='ads_path',
             help='Additional ADS path')
     get_dfsshare_parser.set_defaults(func=get_dfsshare)
 
     # Parser for the get-netou command
     get_netou_parser = subparsers.add_parser('get-netou', help='Get a list of all current '\
-        'OUs in the domain', parents=[ad_parser, logging_parser, json_output_parser])
+        'OUs in the domain', parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_netou_parser.add_argument('--ouname', dest='queried_ouname',
             default='*', help='OU name to query (wildcards accepted)')
     get_netou_parser.add_argument('--guid', dest='queried_guid',
             help='Only return OUs with the specified GUID in their gplink property.')
     get_netou_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
     get_netou_parser.add_argument('-a', '--ads-path',
             help='Additional ADS path')
     get_netou_parser.add_argument('--full-data', action='store_true',
             help='If set, returns full information on the OUs, otherwise, just the adspath')
     get_netou_parser.set_defaults(func=get_netou)
 
     # Parser for the get-netsite command
     get_netsite_parser = subparsers.add_parser('get-netsite', help='Get a list of all current '\
-        'sites in the domain', parents=[ad_parser, logging_parser, json_output_parser])
+        'sites in the domain', parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_netsite_parser.add_argument('--sitename', dest='queried_sitename',
             help='Site name to query (wildcards accepted)')
     get_netsite_parser.add_argument('--guid', dest='queried_guid',
             help='Only return sites with the specified GUID in their gplink property.')
     get_netsite_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
     get_netsite_parser.add_argument('-a', '--ads-path',
             help='Additional ADS path')
     get_netsite_parser.add_argument('--full-data', action='store_true',
             help='If set, returns full information on the sites, otherwise, just the name')
     get_netsite_parser.set_defaults(func=get_netsite)
 
     # Parser for the get-netsubnet command
     get_netsubnet_parser = subparsers.add_parser('get-netsubnet', help='Get a list of all current '\
-        'subnets in the domain', parents=[ad_parser, logging_parser, json_output_parser])
+        'subnets in the domain', parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_netsubnet_parser.add_argument('--sitename', dest='queried_sitename',
             help='Only return subnets for the specified site name (wildcards accepted)')
     get_netsubnet_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
     get_netsubnet_parser.add_argument('-a', '--ads-path',
             help='Additional ADS path')
     get_netsubnet_parser.add_argument('--full-data', action='store_true',
             help='If set, returns full information on the subnets, otherwise, just the name')
     get_netsubnet_parser.set_defaults(func=get_netsubnet)
 
     # Parser for the get-netdomaintrust command
     get_netdomaintrust_parser = subparsers.add_parser('get-netdomaintrust', help='Returns a list of all the '\
-        'trusts of the specified domain', parents=[ad_parser, logging_parser, json_output_parser])
+        'trusts of the specified domain', parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_netdomaintrust_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
+    get_netdomaintrust_parser.add_argument('--full-data', action='store_true',
+            help='If set, returns full information on the trusts, otherwise, just basic info')
     get_netdomaintrust_parser.set_defaults(func=get_netdomaintrust)
 
     # Parser for the get-netgpo command
     get_netgpo_parser = subparsers.add_parser('get-netgpo', help='Get a list of all current '\
-        'GPOs in the domain', parents=[ad_parser, logging_parser, json_output_parser])
+        'GPOs in the domain', parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_netgpo_parser.add_argument('--gponame', dest='queried_gponame',
             default='*', help='GPO name to query for (wildcards accepted)')
     get_netgpo_parser.add_argument('--displayname', dest='queried_displayname',
             help='Display name to query for (wildcards accepted)')
     get_netgpo_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
     get_netgpo_parser.add_argument('-a', '--ads-path',
             help='Additional ADS path')
     get_netgpo_parser.set_defaults(func=get_netgpo)
 
     # Parser for the get-netpso command
     get_netpso_parser = subparsers.add_parser('get-netpso', help='Get a list of all current '\
-        'PSOs in the domain', parents=[ad_parser, logging_parser, json_output_parser])
+        'PSOs in the domain', parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_netpso_parser.add_argument('--psoname', dest='queried_psoname',
             default='*', help='pso name to query for (wildcards accepted)')
     get_netpso_parser.add_argument('--displayname', dest='queried_displayname',
             help='Display name to query for (wildcards accepted)')
     get_netpso_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
     get_netpso_parser.add_argument('-a', '--ads-path',
@@ -405,17 +422,17 @@
     find_gpolocation_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
     find_gpolocation_parser.add_argument('--local-group', dest='queried_localgroup',
             default='S-1-5-32-544', help='The local group to check access against. It can be ' \
                     '\'Administrators\', \'RDP\', or a \'S-1-5-X\' SID type')
     find_gpolocation_parser.set_defaults(func=find_gpolocation)
 
-    # Parser for the get-netgroup command
+    # Parser for the get-netgroupmember command
     get_netgroupmember_parser = subparsers.add_parser('get-netgroupmember', help='Return a list of members of a domain group',
-        parents=[ad_parser, logging_parser, json_output_parser])
+        parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_netgroupmember_parser.add_argument('--groupname', dest='queried_groupname',
             help='Group to query, defaults to the \'Domain Admins\' group (wildcards accepted)')
     get_netgroupmember_parser.add_argument('--sid', dest='queried_sid',
             help='SID to query')
     get_netgroupmember_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
     get_netgroupmember_parser.add_argument('-a', '--ads-path', dest='ads_path',
@@ -423,14 +440,16 @@
     get_netgroupmember_parser.add_argument('-r', '--recurse', action='store_true',
             help='If the group member is a group, try to resolve its members as well')
     get_netgroupmember_parser.add_argument('--use-matching-rule', action='store_true',
             help='Use LDAP_MATCHING_RULE_IN_CHAIN in the LDAP search query when -Recurse is specified.\n' \
         'Much faster than manual recursion, but doesn\'t reveal cross-domain groups')
     get_netgroupmember_parser.add_argument('--full-data', action='store_true',
             help='If set, returns full information on the members')
+    get_netgroupmember_parser.add_argument('--custom-filter', dest='custom_filter',
+            default=str(), help='Custom filter')
     get_netgroupmember_parser.set_defaults(func=get_netgroupmember)
 
     # Parser for the get-netsession command
     get_netsession_parser = subparsers.add_parser('get-netsession', help='Queries a host to return a '\
         'list of active sessions on the host (you can use local credentials instead of domain credentials)',
         parents=[target_parser, logging_parser, json_output_parser])
     get_netsession_parser.set_defaults(func=get_netsession)
@@ -561,15 +580,16 @@
         except ValueError:
             args.lmhash, args.nthash = 'aad3b435b51404eeaad3b435b51404ee', args.hashes
         finally:
             args.password = str()
     else:
         args.lmhash = args.nthash = str()
 
-    if args.password is None and args.hashes is None and not args.do_kerberos:
+    if (args.password is None and args.hashes is None and not args.do_kerberos 
+            and not args.user_cert is None and args.user_key is None):
         from getpass import getpass
         args.password = getpass('Password:')
 
     parsed_args = dict()
     for k, v in vars(args).items():
         if k not in ('func', 'hashes', 'submodule', 'logging_level', 'json_output'):
             parsed_args[k] = v
```

### Comparing `pywerview-0.4.1/pywerview/formatters.py` & `pywerview-0.5.0/pywerview/formatters.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,22 +78,28 @@
                  0x100: 'extended_right', 0x10000: 'delete',
                  0x20000: 'read_control', 0x40000: 'write_dacl',
                  0x80000: 'write_owner'}
 
 __access_mask_generic = {0xf01ff: 'generic_all', 0x20094: 'generic_read',
                          0x20028: 'generic_write', 0x20004: 'generic_execute'}
 
-__trust_attrib = {0x1: 'non_transitive', 0x2: 'uplevel_only',
-                  0x4: 'filter_sids', 0x8: 'forest_transitive',
-                  0x10: 'cross_organization', 0x20: 'within_forest',
-                  0x40: 'treat_as_external',
-                  0x80: 'trust_uses_rc4_encryption',
-                  0x100: 'trust_uses_aes_keys',
-                  0X200: 'cross_organization_no_tgt_delegation',
-                  0x400: 'pim_trust'}
+# https://learn.microsoft.com/en-us/openspecs/windows_protocols/ms-adts/e9a2d23c-c31e-4a6f-88a0-6646fdb51a3c
+__trust_attrib = {0x1: 'TRUST_ATTRIBUTE_NON_TRANSITIVE', 
+                  0x2: 'TRUST_ATTRIBUTE_UPLEVEL_ONLY',
+                  0x4: 'TRUST_ATTRIBUTE_QUARANTINED_DOMAIN', 
+                  0x8: 'TRUST_ATTRIBUTE_FOREST_TRANSITIVE',
+                  0x10: 'TRUST_ATTRIBUTE_CROSS_ORGANIZATION', 
+                  0x20: 'TRUST_ATTRIBUTE_WITHIN_FOREST',
+                  0x40: 'TRUST_ATTRIBUTE_TREAT_AS_EXTERNAL',
+                  0x80: 'TRUST_ATTRIBUTE_USES_RC4_ENCRYPTION',
+                  # TODO: x100 seems not documented ?
+                  0x100: 'TRUST_USES_AES_KEYS',
+                  0X200: 'TRUST_ATTRIBUTE_CROSS_ORGANIZATION_NO_TGT_DELEGATION',
+                  0x400: 'TRUST_ATTRIBUTE_PIM_TRUST',
+                  0x800: 'TRUST_ATTRIBUTE_CROSS_ORGANIZATION_ENABLE_TGT_DELEGATION'}
 
 __trust_direction = {0: 'disabled', 1: 'inbound',
                      2: 'outbound', 3: 'bidirectional'}
 
 __trust_type = {1: 'windows_non_active_directory',
                 2: 'windows_active_directory', 3: 'mit'}
```

### Comparing `pywerview-0.4.1/pywerview/functions/gpo.py` & `pywerview-0.5.0/pywerview/functions/gpo.py`

 * *Files identical despite different names*

### Comparing `pywerview-0.4.1/pywerview/functions/hunting.py` & `pywerview-0.5.0/pywerview/functions/hunting.py`

 * *Files identical despite different names*

### Comparing `pywerview-0.4.1/pywerview/functions/misc.py` & `pywerview-0.5.0/pywerview/functions/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 
         return resp['pmsgOut']['V1']['pResult']['rItems'][0]['pName']
 
     def get_domainsid(self, queried_domain=str()):
 
         with pywerview.functions.net.NetRequester(self._domain_controller, self._domain, self._user,
                                                   self._password, self._lmhash, self._nthash,
-                                                  self._do_kerberos, self._do_tls) as r:
+                                                  self._do_kerberos, self._do_tls,
+                                                  self._user_cert, self._user_key) as r:
             domain_controllers = r.get_netdomaincontroller(queried_domain=queried_domain)
 
         if domain_controllers:
             primary_dc = domain_controllers[0]
             domain_sid = primary_dc.objectsid
 
             # we need to retrieve the domain sid from the controller sid
```

### Comparing `pywerview-0.4.1/pywerview/functions/net.py` & `pywerview-0.5.0/pywerview/functions/net.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,23 +66,22 @@
             if attr_value:
                 object_filter = '(&({}={}){})'.format(attr_desc, attr_value, filter_objectclass)
                 break
         else:
             object_filter = '(&(name=*){})'.format(filter_objectclass)
 
         adserviceaccounts = self._ldap_search(object_filter, adobj.GMSAAccount, attributes=attributes)
-        sid_resolver = NetRequester(self._domain_controller, self._domain, self._user, self._password, self._lmhash, self._nthash)
 
         # In this loop, we resolve SID (if true) and we populate 'enabled' attribute
         for i, adserviceaccount in enumerate(adserviceaccounts):
             if resolve_sids:
                 results = list()
                 for sid in getattr(adserviceaccount, 'msds-groupmsamembership'):
                     try:
-                        resolved_sid = sid_resolver.get_adobject(queried_sid=sid, queried_domain=self._queried_domain, 
+                        resolved_sid = self.get_adobject(queried_sid=sid, queried_domain=self._queried_domain, 
                                                                   attributes=['distinguishedname'])[0].distinguishedname
                     except IndexError:
                         self._logger.warning('We did not manage to resolve this SID ({}) against the DC'.format(sid))
                         resolved_sid = sid
                     results.append(resolved_sid)
                 adserviceaccounts[i].add_attributes({'msds-groupmsamembership': results})
             adserviceaccounts[i].add_attributes({'Enabled': 'ACCOUNTDISABLE' not in adserviceaccount.useraccountcontrol})
@@ -104,25 +103,25 @@
 
         guid_map = dict()
         # This works on a mono-domain forest, must be tested on a more complex one
         if resolve_guids:
             # Dirty fix to get base DN even if custom ADS path was given
             base_dn = ','.join(self._base_dn.split(',')[-2:])
             guid_map = {'{00000000-0000-0000-0000-000000000000}': 'All'}
-            with NetRequester(self._domain_controller, self._domain, self._user, self._password,
-                  self._lmhash, self._nthash, self._do_kerberos, self._do_tls) as net_requester:
-                for o in net_requester.get_adobject(ads_path='CN=Schema,CN=Configuration,{}'.format(base_dn),
-                        attributes=['name', 'schemaIDGUID'], custom_filter='(schemaIDGUID=*)'):
-                    guid_map['{{{}}}'.format(o.schemaidguid)] = o.name
-
-                for o in net_requester.get_adobject(ads_path='CN=Extended-Rights,CN=Configuration,{}'.format(base_dn),
-                        attributes=['name', 'rightsGuid'], custom_filter='(objectClass=controlAccessRight)'):
-                    guid_map['{{{}}}'.format(o.rightsguid.lower())] = o.name
+            for o in self.get_adobject(ads_path='CN=Schema,CN=Configuration,{}'.format(base_dn),
+                    attributes=['name', 'schemaIDGUID'], custom_filter='(schemaIDGUID=*)'):
+                        guid_map['{{{}}}'.format(o.schemaidguid)] = o.name
+
+            for o in self.get_adobject(ads_path='CN=Extended-Rights,CN=Configuration,{}'.format(base_dn),
+                    attributes=['name', 'rightsGuid'], custom_filter='(objectClass=controlAccessRight)'):
+                        guid_map['{{{}}}'.format(o.rightsguid.lower())] = o.name
+            self._base_dn = base_dn
 
         attributes = ['distinguishedname', 'objectsid', 'ntsecuritydescriptor']
+
         if sacl:
             controls = list()
             acl_type = 'Sacl'
         else:
             # The control is used to get access to ntSecurityDescriptor with an
             # unprivileged user, see https://stackoverflow.com/questions/40771503/selecting-the-ad-ntsecuritydescriptor-attribute-as-a-non-admin/40773088
             # /!\ May break pagination from what I've read (see Stack Overflow answer)
@@ -137,20 +136,15 @@
         rights_to_guid = {'reset-password': '{00299570-246d-11d0-a768-00aa006e0529}',
                 'write-members': '{bf9679c0-0de6-11d0-a285-00aa003049e2}',
                 'allowed-to-authenticate':'{68b1d179-0d15-4d4f-ab71-46152e79a7bc}',
                 'all': '{00000000-0000-0000-0000-000000000000}'}
         guid_filter = rights_to_guid.get(rights_filter, None)
 
         if resolve_sids:
-            sid_resolver = NetRequester(self._domain_controller, self._domain,
-                    self._user, self._password, self._lmhash, self._nthash,
-                    self._do_kerberos, self._do_tls)
             sid_mapping = adobj.ADObject._well_known_sids.copy()
-        else:
-            sid_resolver = None
 
         for security_descriptor in security_descriptors:
             sd = SR_SECURITY_DESCRIPTOR()
             try:
                 sd.fromString(security_descriptor.ntsecuritydescriptor)
             except TypeError:
                 continue
@@ -168,22 +162,22 @@
                 attributes['acetype'] = ace['TypeName']
                 attributes['binarysize'] = ace['AceSize']
                 attributes['aceflags'] = fmt.format_ace_flags(ace['AceFlags'])
                 attributes['accessmask'] = ace['Ace']['Mask']['Mask']
                 attributes['activedirectoryrights'] = fmt.format_ace_access_mask(ace['Ace']['Mask']['Mask'])
                 attributes['isinherited'] = bool(ace['AceFlags'] & 0x10)
                 attributes['securityidentifier'] = format_sid(ace['Ace']['Sid'].getData())
-                if sid_resolver:
+                if resolve_sids:
                     converted_sid = attributes['securityidentifier']
                     try:
                         resolved_sid = sid_mapping[converted_sid]
                     except KeyError:
                         try:
-                            resolved_sid = sid_resolver.get_adobject(queried_sid=converted_sid,
-                                    queried_domain=self._queried_domain, attributes=['distinguishedname'])[0]
+                            resolved_sid = self.get_adobject(queried_sid=converted_sid,
+                                    queried_domain=self._queried_domain, ads_path=self._base_dn, attributes=['distinguishedname'])[0]
                             resolved_sid = resolved_sid.distinguishedname
                         except IndexError:
                             self._logger.warning('We did not manage to resolve this SID ({}) against the DC'.format(converted_sid))
                             resolved_sid = attributes['securityidentifier']
                     finally:
                         sid_mapping[converted_sid] = resolved_sid
                         attributes['securityidentifier'] = resolved_sid
@@ -521,21 +515,31 @@
 
                 # `--groupname` option is missing, falling back to the "Domain Admins"
                 else:
                     self._logger.debug('No groupname provided, falling back to the "Domain Admins"'.format(queried_groupname))
                     if _sid:
                         queried_sid = _sid
                     else:
-                        with pywerview.functions.misc.Misc(self._domain_controller,
-                                                           self._domain, self._user,
-                                                           self._password, self._lmhash,
-                                                           self._nthash, self._do_kerberos,
-                                                           self._do_tls) as misc_requester:
-                            queried_sid = misc_requester.get_domainsid(queried_domain) + '-512'
+                        # Logic extract from pywerview.functions.Misc get_domainsid to save object creation
+                        # LDAP filter to extract DC
+                        domain_controller_filter = '(userAccountControl:1.2.840.113556.1.4.803:=8192)'
+                        domain_controllers = self.get_netcomputer(queried_domain=queried_domain, custom_filter=domain_controller_filter,
+                                                                attributes=['objectsid'])
+                        if domain_controllers:
+                            primary_dc = domain_controllers[0]
+                            domain_sid = primary_dc.objectsid
+
+                            # we need to retrieve the domain sid from the controller sid
+                            domain_sid = '-'.join(domain_sid.split('-')[:-1])
+                            queried_sid = domain_sid + '-512'
                             self._logger.debug('Found Domains Admins SID = {}'.format(queried_sid))
+                        else:
+                            self._logger.critical('We did not manage to retrieve domain controller, please specify a group name')
+                            return list()
+
                     groups = self.get_netgroup(queried_sid=queried_sid,
                                                queried_domain=self._queried_domain,
                                                full_data=True)
             except IndexError:
                 raise ValueError('The group {} was not found'.format(_groupname))
 
             final_members = list()
@@ -609,18 +613,26 @@
                 results.append(member)
                 if (recurse and (not use_matching_rule) and member.isgroup and member.membername):
                     groups_to_process.append((member.membername, str()))
 
         return results
 
     @LDAPRPCRequester._ldap_connection_init
-    def get_netdomaintrust(self, queried_domain):
+    def get_netdomaintrust(self, queried_domain, full_data=False):
+
+        if full_data:
+            attributes=list()
+        else:
+            attributes=['trustpartner', 'trustdirection',
+                        'whencreated', 'whenchanged',
+                        'trusttype', 'trustattributes']
+
         trust_search_filter = '(&(objectClass=trustedDomain))'
 
-        return self._ldap_search(trust_search_filter, adobj.Trust)
+        return self._ldap_search(trust_search_filter, adobj.Trust, attributes=attributes)
 
     @LDAPRPCRequester._rpc_connection_init(r'\srvsvc')
     def get_netsession(self):
 
         try:
             resp = srvs.hNetrSessionEnum(self._rpc_connection, '\x00', NULL, 10)
         except DCERPCException:
```

### Comparing `pywerview-0.4.1/pywerview/objects/rpcobjects.py` & `pywerview-0.5.0/pywerview/objects/rpcobjects.py`

 * *Files identical despite different names*

### Comparing `pywerview-0.4.1/pywerview/requester.py` & `pywerview-0.5.0/pywerview/requester.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import sys
 import logging
 import socket
 import ntpath
 import ldap3
 import os
 import tempfile
+import ssl
 
 from ldap3.protocol.formatters.formatters import *
 
 from impacket.smbconnection import SMBConnection
 from impacket.smbconnection import SessionError
 from impacket.krb5.ccache import CCache, Credential, CountedOctetString
 from impacket.krb5 import constants
@@ -36,23 +37,27 @@
 from impacket.dcerpc.v5.dtypes import NULL
 from impacket.dcerpc.v5.dcomrt import DCOMConnection
 from impacket.dcerpc.v5.rpcrt import DCERPCException
 
 import pywerview.formatters as fmt
 
 class LDAPRequester():
-    def __init__(self, domain_controller, domain=str(), user=(), password=str(),
-                 lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False):
+    def __init__(self, domain_controller, domain=str(), user=str(), password=str(),
+                 lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
+                 user_cert=str(), user_key=str()):
         self._domain_controller = domain_controller
         self._domain = domain
         self._user = user
         self._password = password
         self._lmhash = lmhash
         self._nthash = nthash
         self._do_kerberos = do_kerberos
+        self._do_certificate = user_cert and user_key
+        self._user_cert = user_cert
+        self._user_key = user_key
         self._do_tls = do_tls
         self._queried_domain = None
         self._ads_path = None
         self._ads_prefix = None
         self._ldap_connection = None
         self._base_dn = None
 
@@ -98,34 +103,49 @@
         new_creds['server'].fromPrincipal(Principal(principal, type=constants.PrincipalNameType.NT_PRINCIPAL.value))
 
         return new_creds
 
     def _create_ldap_connection(self, queried_domain=str(), ads_path=str(),
                                 ads_prefix=str()):
         if not self._domain:
-            if self._do_kerberos:
+            if self._do_certificate:
+                self._logger.critical('-w with the FQDN must be used when authenticating with certificates')
+                sys.exit(-1)
+            elif self._do_kerberos:
                 ccache = CCache.loadFile(os.getenv('KRB5CCNAME'))
                 self._domain = ccache.principal.realm['data'].decode('utf-8')
             else:
                 try:
                     self._domain = self._get_netfqdn()
                 except SessionError as e:
                     self._logger.critical(e)
                     sys.exit(-1)
 
         if not queried_domain:
-            if self._do_kerberos:
+            if self._do_certificate:
+                # TODO: CHECK!
+                # Change this message
+                self._logger.warning('Cross domain query with certificate is not yet supported, so domain=queried domain')
+                queried_domain = self._domain
+            elif self._do_kerberos:
                 ccache = CCache.loadFile(os.getenv('KRB5CCNAME'))
                 queried_domain = ccache.principal.realm['data'].decode('utf-8')
             else:
                 try:
                     queried_domain = self._get_netfqdn()
                 except SessionError as e:
                     self._logger.critical(e)
                     sys.exit(-1)
+        else:
+            if self._do_certificate:
+                # TODO: CHECK!
+                # Change this message
+                self._logger.warning('Cross domain query with certificate is not yet supported, so domain=queried domain')
+                queried_domain = self._domain
+
         self._queried_domain = queried_domain
 
         base_dn = str()
 
         if ads_prefix:
             self._ads_prefix = ads_prefix
             base_dn = '{},'.format(self._ads_prefix)
@@ -140,17 +160,19 @@
             base_dn += ','.join('dc={}'.format(x) for x in self._queried_domain.split('.'))
 
         # base_dn is no longer used within `_create_ldap_connection()`, but I don't want to break
         # the function call. So we store it in an attriute and use it in `_ldap_search()`
         self._base_dn = base_dn
 
         # Format the username and the domain
-        # ldap3 seems not compatible with USER@DOMAIN format
+        # ldap3 seems not compatible with USER@DOMAIN format with NTLM auth
         if self._do_kerberos:
             user = '{}@{}'.format(self._user, self._domain.upper())
+        elif self._do_certificate:
+            user = None
         else:
             user = '{}\\{}'.format(self._domain, self._user)
 
         # Call custom formatters for several AD attributes
         formatter = {'userAccountControl': fmt.format_useraccountcontrol,
                 'sAMAccountType': fmt.format_samaccounttype,
                 'trustType': fmt.format_trusttype,
@@ -214,14 +236,29 @@
                     # If we don't find any, we hope for the best (TGT in cache)
                     self._logger.debug('Alternative TGS not found, using KRB5CCNAME as is '
                             'while hoping it contains a TGT')
                     cred_store = dict()
             ldap_connection_kwargs['cred_store'] = cred_store
             self._logger.debug('LDAP binding parameters: server = {0} / user = {1} '
                    '/ Kerberos auth'.format(self._domain_controller, user))
+
+        elif self._do_certificate:
+            tls_mode = 'Implicit'
+            self._logger.debug('LDAPS authentication with certificate')
+            tls = ldap3.Tls(local_private_key_file=self._user_key, local_certificate_file=self._user_cert, validate=ssl.CERT_NONE)
+            ldap_server.tls = tls
+            # Explicit TLS, setting up StartTLS
+            if not self._do_tls:
+                tls_mode = 'Explicit'
+                self._logger.warning('Using certificate authentication but --tls not provided, setting up TLS with StartTLS')
+                ldap_connection_kwargs['authentication'] = ldap3.SASL
+                ldap_connection_kwargs['sasl_mechanism'] = ldap3.EXTERNAL
+            self._logger.debug('LDAP binding parameters: server = {0} / cert = {1} '
+                '/ key = {2} / {3} TLS / Certificate auth'.format(self._domain_controller, self._user_cert, self._user_key, tls_mode))
+
         else:
             self._logger.debug('LDAP authentication with NTLM')
             ldap_connection_kwargs['authentication'] = ldap3.NTLM
             if self._lmhash and self._nthash:
                 ldap_connection_kwargs['password'] = '{}:{}'.format(self._lmhash, self._nthash)
                 self._logger.debug('LDAP binding parameters: server = {0} / user = {1} '
                    '/ hash = {2}'.format(self._domain_controller, user, ldap_connection_kwargs['password']))
@@ -229,25 +266,42 @@
                 ldap_connection_kwargs['password'] = self._password
                 self._logger.debug('LDAP binding parameters: server = {0} / user = {1} '
                    '/ password = {2}'.format(self._domain_controller, user, ldap_connection_kwargs['password']))
 
         try:
             ldap_connection = ldap3.Connection(ldap_server, **ldap_connection_kwargs)
             try:
-                ldap_connection.bind()
+                if self._do_certificate:
+                    ldap_connection.open()
+                    if not self._do_tls:
+                        # raise_exceptions = True raises an exception (oh!) during StartTLS and
+                        # I don't know why, so we disable it for a moment
+                        ldap_connection.raise_exceptions = False
+                        self._logger.debug('Sending StartTLS command')
+                        if ldap_connection.start_tls():
+                            self._logger.debug('StartTLS succeeded')
+                            # Ok, back to normal
+                            ldap_connection.raise_exceptions = True
+                            ldap_connection.bind()
+                        else:
+                            self._logger.critical('StartTLS failed, exiting')
+                            sys.exit(-1)
+                else:
+                    ldap_connection.bind()
             except ldap3.core.exceptions.LDAPSocketOpenError as e:
                 self._logger.critical(e)
                 if self._do_tls:
                     self._logger.critical('TLS negociation failed, this error is mostly due to your host '
                                           'not supporting SHA1 as signing algorithm for certificates')
                 sys.exit(-1)
             except ldap3.core.exceptions.LDAPInvalidCredentialsResult:
                 # https://github.com/zyn3rgy/LdapRelayScan#ldaps-channel-binding-token-requirements
                 if 'AcceptSecurityContext error, data 80090346' in ldap_connection.result['message']:
-                    self._logger.critical('Server requires Channel Binding Token, try again without --tls flag')
+                    self._logger.critical('Server requires Channel Binding Token, try again without --tls flag '
+                                           'or use certificate authentication')
                     sys.exit(-1)
                 else:
                     self._logger.critical('Invalid Credentials')
                     sys.exit(-1)
 
         except ldap3.core.exceptions.LDAPStrongerAuthRequiredResult:
             # We need to try TLS
@@ -267,14 +321,22 @@
                 if 'AcceptSecurityContext error, data 80090346' in ldap_connection.result['message']:
                     self._logger.critical('Server requires Channel Binding Token and LDAP Signing, pywerview will not work')
                     sys.exit(-1)
                 else:
                     self._logger.critical('Invalid Credentials')
                     sys.exit(-1)
 
+        who_am_i = ldap_connection.extend.standard.who_am_i()
+
+        # Only failed here when using certificate authentication
+        if not who_am_i:
+            self._logger.critical('Certificate authentication failed')
+            sys.exit(-1)
+
+        self._logger.debug('Successfully connected to the LDAP as {}'.format(who_am_i))
         self._ldap_connection = ldap_connection
 
     def _ldap_search(self, search_filter, class_result, attributes=list(), controls=list()):
         results = list()
 
         # if no attribute name specified, we return all attributes
         if not attributes:
@@ -309,17 +371,17 @@
     def _ldap_connection_init(f):
         def wrapper(*args, **kwargs):
             instance = args[0]
             queried_domain = kwargs.get('queried_domain', None)
             ads_path = kwargs.get('ads_path', None)
             ads_prefix = kwargs.get('ads_prefix', None)
             if (not instance._ldap_connection) or \
-               (queried_domain != instance._queried_domain) or \
-               (ads_path != instance._ads_path) or \
-               (ads_prefix != instance._ads_prefix):
+               (queried_domain and queried_domain != instance._queried_domain) or \
+               (ads_path and ads_path != instance._ads_path) or \
+               (ads_prefix and ads_prefix != instance._ads_prefix):
                 if instance._ldap_connection:
                     instance._ldap_connection.unbind()
                 instance._create_ldap_connection(queried_domain=queried_domain,
                                                  ads_path=ads_path, ads_prefix=ads_prefix)
             return f(*args, **kwargs)
         return wrapper
 
@@ -446,36 +508,43 @@
         try:
             self._rpc_connection.disconnect()
         except AttributeError:
             pass
         self._rpc_connection = None
 
 class LDAPRPCRequester(LDAPRequester, RPCRequester):
-    def __init__(self, target_computer, domain=str(), user=(), password=str(),
+    def __init__(self, target_computer, domain=str(), user=str(), password=str(),
                  lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
-                 domain_controller=str()):
+                 user_cert=str(), user_key=str(), domain_controller=str()):
         # If no domain controller was given, we assume that the user wants to
         # target a domain controller to perform LDAP requests against
         if not domain_controller:
             domain_controller = target_computer
+
         LDAPRequester.__init__(self, domain_controller, domain, user, password,
-                               lmhash, nthash, do_kerberos, do_tls)
-        RPCRequester.__init__(self, target_computer, domain, user, password,
-                               lmhash, nthash, do_kerberos)
+                               lmhash, nthash, do_kerberos, do_tls,
+                               user_cert, user_key)
+
+        if user_cert is not None and user_key is not None:
+            RPCRequester.__init__(self, target_computer, domain, user, password,
+                                  lmhash, nthash, do_kerberos)
 
         logger = logging.getLogger('pywerview_main_logger.LDAPRPCRequester')
         self._logger = logger
 
     def __enter__(self):
         try:
             LDAPRequester.__enter__(self)
         except (socket.error, IndexError):
             pass
-        # This should work every time
-        RPCRequester.__enter__(self)
+
+        try:
+            RPCRequester.__enter__(self)
+        except (AttributeError):
+            pass
 
         return self
 
     def __exit__(self, type, value, traceback):
         LDAPRequester.__exit__(self, type, value, traceback)
         RPCRequester.__exit__(self, type, value, traceback)
```

### Comparing `pywerview-0.4.1/pywerview/worker/hunting.py` & `pywerview-0.5.0/pywerview/worker/hunting.py`

 * *Files identical despite different names*

### Comparing `pywerview-0.4.1/pywerview.egg-info/PKG-INFO` & `pywerview-0.5.0/pywerview.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pywerview
-Version: 0.4.1
+Version: 0.5.0
 Summary: A Python port of PowerSploit's PowerView
 Home-page: https://github.com/the-useless-one/pywerview
 Author: Yannick Méheut
 Author-email: yannick@meheut.org
 License: GNU GPLv3
 Keywords: python powersploit pentesting recon active directory windows
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Security
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -100,47 +99,61 @@
 
     Subcommands:
       Available subcommands
 
       {get-adobject,get-adserviceaccount,get-objectacl,get-netuser,get-netgroup,get-netcomputer,get-netdomaincontroller,get-netfileserver,get-dfsshare,get-netou,get-netsite,get-netsubnet,get-netdomaintrust,get-netgpo,get-netpso,get-domainpolicy,get-gpttmpl,get-netgpogroup,find-gpocomputeradmin,find-gpolocation,get-netgroupmember,get-netsession,get-localdisks,get-netdomain,get-netshare,get-netloggedon,get-netlocalgroup,invoke-checklocaladminaccess,get-netprocess,get-userevent,invoke-userhunter,invoke-processhunter,invoke-eventhunter}
         get-adobject        Takes a domain SID, samAccountName or name, and return the associated object
         get-adserviceaccount
-                            Returns a list of all the gMSA of the specified domain (you need privileged account to retrieve passwords)
-        get-objectacl       Takes a domain SID, samAccountName or name, and return the ACL of the associated object
+                            Returns a list of all the gMSA of the specified domain. To retrieve passwords,
+                            you need a privileged account and a TLS connection to the LDAP server (use the
+                            --tls switch).
+        get-objectacl       Takes a domain SID, samAccountName or name, and return the ACL of the
+                            associated object
         get-netuser         Queries information about a domain user
-        get-netgroup        Get a list of all current domain groups, or a list of groups a domain user is member of
+        get-netgroup        Get a list of all current domain groups, or a list of groups a domain user is
+                            member of
         get-netcomputer     Queries informations about domain computers
         get-netdomaincontroller
                             Get a list of domain controllers for the given domain
-        get-netfileserver   Return a list of file servers, extracted from the domain users' homeDirectory, scriptPath, and profilePath fields
+        get-netfileserver   Return a list of file servers, extracted from the domain users' homeDirectory,
+                            scriptPath, and profilePath fields
         get-dfsshare        Return a list of all fault tolerant distributed file systems for a given domain
         get-netou           Get a list of all current OUs in the domain
         get-netsite         Get a list of all current sites in the domain
         get-netsubnet       Get a list of all current subnets in the domain
         get-netdomaintrust  Returns a list of all the trusts of the specified domain
         get-netgpo          Get a list of all current GPOs in the domain
         get-netpso          Get a list of all current PSOs in the domain
         get-domainpolicy    Returns the default domain or DC policy for the queried domain or DC
         get-gpttmpl         Helper to parse a GptTmpl.inf policy file path into a custom object
         get-netgpogroup     Parses all GPOs in the domain that set "Restricted Group" or "Groups.xml"
         find-gpocomputeradmin
-                            Takes a computer (or OU) and determine who has administrative access to it via GPO
-        find-gpolocation    Takes a username or a group name and determine the computers it has administrative access to via GPO
+                            Takes a computer (or OU) and determine who has administrative access to it via
+                            GPO
+        find-gpolocation    Takes a username or a group name and determine the computers it has
+                            administrative access to via GPO
         get-netgroupmember  Return a list of members of a domain group
-        get-netsession      Queries a host to return a list of active sessions on the host (you can use local credentials instead of domain credentials)
-        get-localdisks      Queries a host to return a list of active disks on the host (you can use local credentials instead of domain credentials)
+        get-netsession      Queries a host to return a list of active sessions on the host (you can use
+                            local credentials instead of domain credentials)
+        get-localdisks      Queries a host to return a list of active disks on the host (you can use local
+                            credentials instead of domain credentials)
         get-netdomain       Queries a host for available domains
-        get-netshare        Queries a host to return a list of available shares on the host (you can use local credentials instead of domain credentials)
-        get-netloggedon     This function will execute the NetWkstaUserEnum RPC call to query a given host for actively logged on users
-        get-netlocalgroup   Gets a list of members of a local group on a machine, or returns every local group. You can use local credentials instead of domain credentials, however, domain credentials are needed
-                            to resolve domain SIDs.
+        get-netshare        Queries a host to return a list of available shares on the host (you can use
+                            local credentials instead of domain credentials)
+        get-netloggedon     This function will execute the NetWkstaUserEnum RPC call to query a given host
+                            for actively logged on users
+        get-netlocalgroup   Gets a list of members of a local group on a machine, or returns every local
+                            group. You can use local credentials instead of domain credentials, however,
+                            domain credentials are needed to resolve domain SIDs.
         invoke-checklocaladminaccess
                             Checks if the given user has local admin access on the given host
-        get-netprocess      This function will execute the 'Select * from Win32_Process' WMI query to a given host for a list of executed process
-        get-userevent       This function will execute the 'SELECT * from Win32_NTLogEvent' WMI query to a given host for a list of executed process
+        get-netprocess      This function will execute the 'Select * from Win32_Process' WMI query to a
+                            given host for a list of executed process
+        get-userevent       This function will execute the 'SELECT * from Win32_NTLogEvent' WMI query to a
+                            given host for a list of executed process
         invoke-userhunter   Finds which machines domain users are logged into
         invoke-processhunter
                             Searches machines for processes with specific name, or ran by specific users
         invoke-eventhunter  Searches machines for events with specific name, or ran by specific users
 
 Take a look at the [wiki](https://github.com/the-useless-one/pywerview/wiki) to
 see a more detailed usage of every command.
@@ -150,15 +163,15 @@
 
 For example, my domain name is `uselessdomain.local`. The Win2K compatible name
 is `USELESSDOMAIN`. In every command,  I must use __`uselessdomain.local`__ as
 an argument, and __not__ `USELESSDOMAIN`.
 
 ## GLOBAL ARGUMENTS
 
-### LOGGING
+### Logging
 
 You can provide a logging level to `pywerview` modules by using `-l` or `--logging-level` options. Supported levels are:
 
 * `CRITICAL`: Only critical errors are displayed **(default)**
 * `WARNING` Warnings are displayed, along with citical errors
 * `DEBUG`: Debug level (caution: **very** verbose)
 * `ULTRA`: Extreme debugging level (caution: **very very** verbose)
@@ -233,18 +246,57 @@
 ```
 
 To recap:
 
 |           SPN in the ticket           | Can be used with LDAP functions | Can be used with SMB/RPC functions |
 | :-----------------------------------: | :-----------------------------: | :--------------------------------: |
 | `ldap/srv-ad.contoso.com@CONTOSO.COM` |              ✔️                  |                 ✔️                  |
-| `cifs/srv-ad.contoso.com@CONTOSO.COm` |              ✔️                  |                 ✔️                  |
+| `cifs/srv-ad.contoso.com@CONTOSO.COM` |              ✔️                  |                 ✔️                  |
 |       `ldap/srv-ad@CONTOSO.COM`       |              ❌                 |                 ✔️                  |
 
-### TLS CONNECTION
+*NOTE:* The same limitation exists for TGT in your cache credential file: `krbtgt/srv-ad.contoso.com@CONTOSO.COM` will work 
+but not `krbtgt/srv-ad@CONTOSO.COM`.
+
+### LDAP SChannel authentication
+
+SChannel authentication is supported for a subset of the submodules. Functions that support SChannel authentication are:
+
+* get-adobject
+* get-adserviceaccount
+* get-objectacl
+* get-netuser
+* get-netgroup
+* get-netcomputer
+* get-netdomaincontroller
+* get-netfileserver
+* get-netou
+* get-netsite
+* get-netsubnet
+* get-netdomaintrust
+* get-netpso
+* get-netgpo
+* get-netgroupmember
+
+To authenticate via SChannel:
+
+1. Retrieve the certificate and the key with your favorite tool ([ntlmrelayx.py](https://github.com/fortra/impacket), [certipy](https://github.com/ly4k/Certipy),...)
+2. `pywerview` needs a certificate file and a key file, so you need to extract them from the `.pfx`.
+3. Use `--cert` and  `--key` as in the following example:
+
+```console
+$ python3 pywerview.py get-netuser -w contoso.com --dc-ip 172.16.0.55 --cert stormtroopers.crt --key stormtroopers.key --username administrator --attributes distinguishedname useraccountcontrol --tls
+distinguishedname:  CN=Administrator,CN=Users,DC=contoso,DC=com
+useraccountcontrol: NORMAL_ACCOUNT
+
+```
+
+If you don't specify the `--tls` flag when using certificate authentication, `pywerview` will try to use StartTLS and an `EXTERNAL SASL` bind 
+as described in the [Microsoft documentation](https://learn.microsoft.com/en-us/openspecs/windows_protocols/ms-adts/8e73932f-70cf-46d6-88b1-8d9f86235e81)
+
+### TLS connection
 
 You can force a connection to the LDAPS port by using the `--tls` switch. It
 can be necessary with some functions, for example when retrieving gMSA
 passwords with `get-adserviceaccount`:
 
 ```console
 $ python3 pywerview.py get-adserviceaccount -t srv-ad.contoso.com -u 'SRV-MAIL$' --hashes $NT_HASH --resolve-sids
@@ -260,15 +312,15 @@
 samaccountname:          gMSA-01$
 msds-managedpassword:    69730ce3914ac6[redacted]
 msds-groupmsamembership: CN=SRV-MAIL,CN=Computers,DC=contoso,DC=com
 description:
 enabled:                 True
 ```
 
-### JSON OUTPUT
+### JSON output
 
 Pywerview can print results in json format by using the `--json` switch.
 
 ## TODO
 
 * Many, many more PowerView functionalities to implement. I'll now focus on
   forest functions, then inter-forest trust functions
@@ -309,9 +361,7 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
 Public License for more details.
 
 You should have received a copy of the GNU General Public License along
 with this program. If not, see
 [https://www.gnu.org/licenses/](https://www.gnu.org/licenses/).
 
-
-
```

### Comparing `pywerview-0.4.1/pywerview.egg-info/SOURCES.txt` & `pywerview-0.5.0/pywerview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywerview-0.4.1/setup.py` & `pywerview-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools import setup, find_packages
 
 long_description = open('README.md').read()
 
 setup(name='pywerview',
-    version='0.4.1',
+    version='0.5.0',
     description='A Python port of PowerSploit\'s PowerView',
     long_description=long_description,
     long_description_content_type='text/markdown',
     dependency_links = ['https://github.com/SecureAuthCorp/impacket/tarball/master#egg=impacket-0.9.22'],
     classifiers=[
         'Environment :: Console',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
```

