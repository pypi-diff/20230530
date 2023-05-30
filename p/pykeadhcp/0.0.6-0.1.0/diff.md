# Comparing `tmp/pykeadhcp-0.0.6.tar.gz` & `tmp/pykeadhcp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeadhcp-0.0.6.tar", last modified: Fri May  5 21:10:21 2023, max compression
+gzip compressed data, was "pykeadhcp-0.1.0.tar", max compression
```

## Comparing `pykeadhcp-0.0.6.tar` & `pykeadhcp-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:10:21.774371 pykeadhcp-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-05-05 21:10:21.774371 pykeadhcp-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:10:21.774371 pykeadhcp-0.0.6/pykeadhcp/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:10:21.774371 pykeadhcp-0.0.6/pykeadhcp/daemons/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/daemons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/daemons/ctrlagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/daemons/ddns.py
--rw-r--r--   0 runner    (1001) docker     (123)    19979 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/daemons/dhcp4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/daemons/dhcp6.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/kea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:10:21.774371 pykeadhcp-0.0.6/pykeadhcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-05-05 21:10:21.000000 pykeadhcp-0.0.6/pykeadhcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-05 21:10:21.000000 pykeadhcp-0.0.6/pykeadhcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:10:21.000000 pykeadhcp-0.0.6/pykeadhcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 21:10:21.000000 pykeadhcp-0.0.6/pykeadhcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 21:10:21.000000 pykeadhcp-0.0.6/pykeadhcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:10:21.774371 pykeadhcp-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/setup.py
+-rw-r--r--   0        0        0    11356 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5301 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/README.md
+-rw-r--r--   0        0        0       30 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/__init__.py
+-rw-r--r--   0        0        0      174 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/daemons/__init__.py
+-rw-r--r--   0        0        0     4508 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/daemons/ctrlagent.py
+-rw-r--r--   0        0        0     4526 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/daemons/ddns.py
+-rw-r--r--   0        0        0    25048 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/daemons/dhcp4.py
+-rw-r--r--   0        0        0    21306 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/daemons/dhcp6.py
+-rw-r--r--   0        0        0     2718 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/exceptions.py
+-rw-r--r--   0        0        0     7453 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/kea.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/ctrlagent/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/dhcp4/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/dhcp4/lease.py
+-rw-r--r--   0        0        0      303 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/dhcp4/reservation.py
+-rw-r--r--   0        0        0      448 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/dhcp4/shared_network.py
+-rw-r--r--   0        0        0      472 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/dhcp4/subnet.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/dhcp6/__init__.py
+-rw-r--r--   0        0        0      341 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/dhcp6/lease.py
+-rw-r--r--   0        0        0      542 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/dhcp6/pd_pool.py
+-rw-r--r--   0        0        0      202 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/dhcp6/reservation.py
+-rw-r--r--   0        0        0      375 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/dhcp6/shared_network.py
+-rw-r--r--   0        0        0      491 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/dhcp6/subnet.py
+-rw-r--r--   0        0        0      495 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/enums.py
+-rw-r--r--   0        0        0      169 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/generic/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/generic/api_response.py
+-rw-r--r--   0        0        0      247 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/generic/base.py
+-rw-r--r--   0        0        0     1589 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/generic/dhcp_common.py
+-rw-r--r--   0        0        0      156 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/generic/hook.py
+-rw-r--r--   0        0        0      403 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/generic/lease.py
+-rw-r--r--   0        0        0      350 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/generic/option_data.py
+-rw-r--r--   0        0        0      412 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/generic/pool.py
+-rw-r--r--   0        0        0      488 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/generic/reservation.py
+-rw-r--r--   0        0        0      175 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/generic/shared_network.py
+-rw-r--r--   0        0        0      244 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/generic/sockets.py
+-rw-r--r--   0        0        0      472 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/generic/status.py
+-rw-r--r--   0        0        0      380 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pykeadhcp/models/generic/subnet.py
+-rw-r--r--   0        0        0      447 2023-05-30 08:59:01.536372 pykeadhcp-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5906 1970-01-01 00:00:00.000000 pykeadhcp-0.1.0/PKG-INFO
```

### Comparing `pykeadhcp-0.0.6/LICENSE` & `pykeadhcp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.0.6/pykeadhcp/daemons/ctrlagent.py` & `pykeadhcp-0.1.0/pykeadhcp/daemons/ctrlagent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,111 +1,126 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from pykeadhcp import Kea
 
+from pykeadhcp.models.generic import KeaResponse, StatusGet
+
 
 class CtrlAgent:
     def __init__(self, api: "Kea"):
         self.service = None  # Control Agent expects service: [] in payload
         self.api = api
 
-    def build_report(self) -> dict:
+        # Cache config and hooks
+        try:
+            self.cached_config = None
+            self.refresh_cached_config()
+            self.hook_libraries = self.api.get_active_hooks(
+                hooks=self.cached_config["Control-agent"]["hooks-libraries"]
+            )
+            self.api.hook_library[self.service] = self.hook_libraries
+        except:
+            pass
+
+    def refresh_cached_config(self):
+        """Sets the cached_config variable
+
+        This function should be called after any interaction with the API that potentially changes the configuration
+        eg. config-set, commands like config-test won't need a config refresh to keep the cached config up to date
+        """
+        config = self.config_get()
+        self.cached_config = config.arguments
+
+    def build_report(self) -> KeaResponse:
         """Returns list of compilation options that this particular binary was built with
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-build-report
         """
         return self.api.send_command(command="build-report", service=self.service)
 
-    def config_get(self) -> dict:
+    def config_get(self) -> KeaResponse:
         """Retrieves the current configuration used by the server
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-config-get
         """
         return self.api.send_command(command="config-get", service=self.service)
 
-    def config_reload(self) -> dict:
+    def config_reload(self) -> KeaResponse:
         """Reloads the last good configuration (configuration file on disk)
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-config-reload
         """
         return self.api.send_command(command="config-reload", service=self.service)
 
-    def config_set(self, config: dict) -> dict:
+    def config_set(self, config: dict) -> KeaResponse:
         """Replace the current server configuration with the provided configuration
 
         Args:
             config:     Configuration to set
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#config-set
         """
         return self.api.send_command_with_arguments(
             command="config-set", service=self.service, arguments=config
         )
 
-    def config_test(self, config: dict) -> dict:
+    def config_test(self, config: dict) -> KeaResponse:
         """Check whether the configuration supplied can be loaded by the dhcp4 daemon
 
         Args:
             config:     Configuration to test
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#config-test
         """
         return self.api.send_command_with_arguments(
             command="config-test", service=self.service, arguments=config
         )
 
-    def config_write(self, filename: str) -> dict:
+    def config_write(self, filename: str) -> KeaResponse:
         """Write the current configuration to a file on disk
 
         Args:
             filename:       Name of the configuration file
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#config-write
         """
         return self.api.send_command_with_arguments(
             command="config-write",
             service=self.service,
             arguments={"filename": filename},
         )
 
-    def list_commands(self) -> dict:
+    def list_commands(self) -> KeaResponse:
         """List all commands supported by the server/service
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-list-commands
         """
         return self.api.send_command_with_arguments(
             command="list-commands", service=self.service, arguments={}
         )
 
-    def shutdown(self) -> dict:
+    def shutdown(self) -> KeaResponse:
         """Instructs the server daemon to initiate its shutdown procedure
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-shutdown
         """
         return self.api.send_command_with_arguments(
             command="shutdown", service=self.service, arguments={"exit-value": 123}
         )
 
-    def status_get(self) -> dict:
+    def status_get(self) -> StatusGet:
         """Returns servers runtime information
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-status-get
         """
-        return self.api.send_command(command="status-get", service=self.service)
-
-    def version_get(self) -> dict:
-        """Returns extended information about the Kea Version that is running
-
-        Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-version-get
-        """
-        return self.api.send_command(command="version-get", service=self.service)
+        data = self.api.send_command(command="status-get", service=self.service)
+        return StatusGet.parse_obj(data.arguments)
```

### Comparing `pykeadhcp-0.0.6/pykeadhcp/daemons/ddns.py` & `pykeadhcp-0.1.0/pykeadhcp/daemons/ddns.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,129 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from pykeadhcp import Kea
 
+from pykeadhcp.models.generic import KeaResponse
+
 
 class Ddns:
     def __init__(self, api: "Kea"):
         self.service = "Ddns"
         self.api = api
 
-    def build_report(self) -> dict:
+        # Cache config and hooks
+        try:
+            self.cached_config = None
+            self.refresh_cached_config()
+            self.hook_libraries = self.api.get_active_hooks(
+                hooks=self.cached_config[self.service.capitalize()]["hooks-libraries"]
+            )
+            self.api.hook_library[self.service] = self.hook_libraries
+        except:
+            pass
+
+    def refresh_cached_config(self):
+        """Sets the cached_config variable
+
+        This function should be called after any interaction with the API that potentially changes the configuration
+        eg. config-set, commands like config-test won't need a config refresh to keep the cached config up to date
+        """
+        config = self.config_get()
+        self.cached_config = config.arguments
+
+    def build_report(self) -> KeaResponse:
         """Returns list of compilation options that this particular binary was built with
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-build-report
         """
         return self.api.send_command(command="build-report", service=self.service)
 
-    def config_get(self) -> dict:
+    def config_get(self) -> KeaResponse:
         """Retrieves the current configuration used by the server
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-config-get
         """
         return self.api.send_command(command="config-get", service=self.service)
 
-    def config_reload(self) -> dict:
+    def config_reload(self) -> KeaResponse:
         """Reloads the last good configuration (configuration file on disk)
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-config-reload
         """
         return self.api.send_command(command="config-reload", service=self.service)
 
-    def config_set(self, config: dict) -> dict:
+    def config_set(self, config: dict) -> KeaResponse:
         """Replace the current server configuration with the provided configuration
 
         Args:
             config:     Configuration to set
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#config-set
         """
         return self.api.send_command_with_arguments(
             command="config-set", service=self.service, arguments=config
         )
 
-    def config_test(self, config: dict) -> dict:
+    def config_test(self, config: dict) -> KeaResponse:
         """Check whether the configuration supplied can be loaded by the dhcp4 daemon
 
         Args:
             config:     Configuration to test
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#config-test
         """
         return self.api.send_command_with_arguments(
             command="config-test", service=self.service, arguments=config
         )
 
-    def config_write(self, filename: str) -> dict:
+    def config_write(self, filename: str) -> KeaResponse:
         """Write the current configuration to a file on disk
 
         Args:
             filename:       Name of the configuration file
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#config-write
         """
         return self.api.send_command_with_arguments(
             command="config-write",
             service=self.service,
             arguments={"filename": filename},
         )
 
-    def list_commands(self) -> dict:
+    def list_commands(self) -> KeaResponse:
         """List all commands supported by the server/service
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-list-commands
         """
         return self.api.send_command_with_arguments(
             command="list-commands", service=self.service, arguments={}
         )
 
-    def statistic_get(self, name: str) -> dict:
+    def statistic_get(self, name: str) -> KeaResponse:
         """Returns single statistic
 
         Args:
             name:       Name of the statistic to get
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-statistic-get
         """
         return self.api.send_command_with_arguments(
             command="statistic-get", service=self.service, arguments={"name": name}
         )
 
-    def statistic_get_all(self) -> dict:
+    def statistic_get_all(self) -> KeaResponse:
         """Returns all recorded statistics
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-statistic-get-all
         """
         return self.api.send_command_with_arguments(
             command="statistic-get-all", service=self.service, arguments={}
```

### Comparing `pykeadhcp-0.0.6/pykeadhcp/daemons/dhcp4.py` & `pykeadhcp-0.1.0/pykeadhcp/daemons/dhcp6.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,623 +1,628 @@
-from typing import TYPE_CHECKING, List, Dict
+from typing import TYPE_CHECKING, List
 
 if TYPE_CHECKING:
     from pykeadhcp import Kea
 
+from pykeadhcp.models.generic import KeaResponse, StatusGet
+from pykeadhcp.models.dhcp6.lease import Lease6, Lease6Page, Lease6TypeEnum
+from pykeadhcp.models.dhcp6.pd_pool import PDPool
+from pykeadhcp.models.dhcp6.reservation import Reservation6
+from pykeadhcp.models.dhcp6.shared_network import SharedNetwork6
+from pykeadhcp.models.dhcp6.subnet import Subnet6
+from pykeadhcp.exceptions import (
+    KeaSharedNetworkNotFoundException,
+    KeaSubnetNotFoundException,
+    KeaLeaseNotFoundException,
+)
 
-class Dhcp4:
+
+class Dhcp6:
     def __init__(self, api: "Kea"):
-        self.service = "dhcp4"
+        self.service = "dhcp6"
         self.api = api
 
-    def build_report(self) -> dict:
+        # Cache config and hooks
+        try:
+            self.cached_config = None
+            self.refresh_cached_config()
+            self.hook_libraries = self.api.get_active_hooks(
+                hooks=self.cached_config[self.service.capitalize()]["hooks-libraries"]
+            )
+            self.api.hook_library[self.service] = self.hook_libraries
+        except:
+            pass
+
+    def refresh_cached_config(self):
+        """Sets the cached_config variable
+
+        This function should be called after any interaction with the API that potentially changes the configuration
+        eg. subnet6-add, commands like lease6-add won't need a config refresh to keep the cached config up to date
+        """
+        config = self.config_get()
+        self.cached_config = config.arguments
+
+    def build_report(self) -> KeaResponse:
         """Returns list of compilation options that this particular binary was built with
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-build-report
         """
         return self.api.send_command(command="build-report", service=self.service)
 
-    def config_get(self) -> dict:
+    def config_get(self) -> KeaResponse:
         """Retrieves the current configuration used by the server
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-config-get
         """
         return self.api.send_command(command="config-get", service=self.service)
 
-    def config_reload(self) -> dict:
+    def config_reload(self) -> KeaResponse:
         """Reloads the last good configuration (configuration file on disk)
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-config-reload
         """
         return self.api.send_command(command="config-reload", service=self.service)
 
-    def config_set(self, config: dict) -> dict:
+    def config_set(self, config: dict) -> KeaResponse:
         """Replace the current server configuration with the provided configuration
 
         Args:
             config:     Configuration to set
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#config-set
         """
         return self.api.send_command_with_arguments(
             command="config-set", service=self.service, arguments=config
         )
 
-    def config_test(self, config: dict) -> dict:
+    def config_test(self, config: dict) -> KeaResponse:
         """Check whether the configuration supplied can be loaded by the dhcp4 daemon
 
         Args:
             config:     Configuration to test
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#config-test
         """
         return self.api.send_command_with_arguments(
             command="config-test", service=self.service, arguments=config
         )
 
-    def config_write(self, filename: str) -> dict:
+    def config_write(self, filename: str) -> KeaResponse:
         """Write the current configuration to a file on disk
 
         Args:
             filename:       Name of the configuration file
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#config-write
         """
         return self.api.send_command_with_arguments(
             command="config-write",
             service=self.service,
             arguments={"filename": filename},
         )
 
-    def dhcp_disable(self, max_period: int = 20) -> dict:
+    def dhcp_disable(self, max_period: int = 20) -> KeaResponse:
         """Globally disables DHCP service (dhcp4)
 
         Args:
             max_period:     Time until DHCP service is automatically renabled in seconds
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-dhcp-disable
         """
         return self.api.send_command_with_arguments(
             command="dhcp-disable",
             service=self.service,
             arguments={"max-period": max_period, "origin": "user"},
         )
 
-    def dhcp_enable(self) -> dict:
+    def dhcp_enable(self) -> KeaResponse:
         """Globally enables the DHCP service (dhcp4)
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/arm/ctrl-channel.html#the-dhcp-enable-command
         """
         return self.api.send_command_with_arguments(
             command="dhcp-enable", service=self.service, arguments={"origin": "user"}
         )
 
-    def ha_continue(self) -> dict:
-        pass
-
-    def ha_heartbeat(self) -> dict:
-        pass
-
-    def ha_maintenance_canel(self) -> dict:
-        pass
-
-    def ha_maintenance_notify(self) -> dict:
-        pass
-
-    def ha_maintenance_start(self) -> dict:
-        pass
-
-    def ha_reset(self) -> dict:
-        pass
-
-    def ha_scopes(self) -> dict:
-        pass
-
-    def ha_sync(self) -> dict:
-        pass
-
-    def ha_sync_complete_notify(self) -> dict:
-        pass
-
-    def lease4_add(
-        self,
-        *,
-        ip_address: str,
-        identifier_key: str = "hw-address",
-        identifier_value: str
-    ) -> dict:
-        """Administratively add a new IPv4 lease
+    def lease6_add(
+        self, *, ip_address: str, duid: str, iaid: int, **kwargs
+    ) -> KeaResponse:
+        """Administratively add a new IPv6 lease
 
         Args:
-            ip_address:         IPv4 Address of lease
-            identifier_key:     Supported identifier (hw-address, flex-id, etc...)
-            identifier_value:   Value of key (eg. flex-id data or hw-address MAC address)
+            ip_address:         IPv6 Address of lease
+            duid:               DHCP Unique Identifier
+            iaid:               Identity Assosication Identifer
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-add
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease6-add
         """
+        lease = Lease6(ip_address=ip_address, duid=duid, iaid=iaid, **kwargs)
+
         return self.api.send_command_with_arguments(
-            command="lease4-add",
+            command="lease6-add",
             service=self.service,
-            arguments={"ip-address": ip_address, identifier_key: identifier_value},
+            arguments=lease.dict(exclude_none=True, by_alias=True),
+            required_hook="lease_cmds",
         )
 
-    def lease4_del(self, ip_address: str) -> dict:
+    def lease6_del(self, ip_address: str) -> KeaResponse:
         """Deletes a lease from the lease database
 
         Args:
             ip_address:     IP address of lease to delete
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-del
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease6-del
         """
         return self.api.send_command_with_arguments(
-            command="lease4-del",
+            command="lease6-del",
             service=self.service,
             arguments={"ip-address": ip_address},
+            required_hook="lease_cmds",
         )
 
-    def lease4_get(self, ip_address: str) -> dict:
+    def lease6_get(self, ip_address: str, type: Lease6TypeEnum = None) -> Lease6:
         """Queries the lease database and retrieves existing lease
 
         Args:
             ip_address:     IP address of lease
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-get
         """
-        return self.api.send_command_with_arguments(
-            command="lease4-get",
+        payload = {"ip-address": ip_address}
+        if type:
+            payload.update["type"] = type
+
+        data = self.api.send_command_with_arguments(
+            command="lease6-get",
             service=self.service,
-            arguments={"ip-address": ip_address},
+            arguments=payload,
+            required_hook="lease_cmds",
         )
 
-    def lease4_get_all(self, subnets: List[int] = []) -> dict:
-        """Retrieves all IPv4 leases or all leases for the specified subnets
+        if data.result == 3:
+            raise KeaLeaseNotFoundException(ip_address)
+
+        return Lease6.parse_obj(data.arguments)
+
+    def lease6_get_all(self, subnets: List[int] = []) -> List[Lease6]:
+        """Retrieves all IPv6 leases or all leases for the specified subnets
 
         Args:
             subnets:        List of subnet IDs to fetch leases for
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-get-all
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease6-get-all
         """
-        return self.api.send_command_with_arguments(
-            command="lease4-get-all",
+        data = self.api.send_command_with_arguments(
+            command="lease6-get-all",
             service=self.service,
             arguments={"subnets": subnets},
+            required_hook="lease_cmds",
         )
 
-    def lease4_get_by_client_id(self, client_id: str) -> dict:
-        """Retrieves all IPv4 leases for the specified client id
+        if data.result == 3:
+            raise KeaLeaseNotFoundException(data.text)
+
+        leases = [Lease6.parse_obj(lease) for lease in data.arguments["leases"]]
+        return leases
+
+    def lease6_get_by_duid(self, duid: str) -> Lease6:
+        """Retrieves a lease for the specified duid
 
         Args:
-            client_id:      Client ID
+            duid:       DHCP Unique Identifier
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-get-by-client-id
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease6-get-by-duid
         """
-        return self.api.send_command_with_arguments(
-            command="lease4-get-by-client-id",
+        data = self.api.send_command_with_arguments(
+            command="lease6-get-by-duid",
             service=self.service,
-            arguments={"client-id": client_id},
+            arguments={"duid": duid},
+            required_hook="lease_cmds",
         )
 
-    def lease4_get_by_hostname(self, hostname: str) -> dict:
-        """Retrieves all IPv4 leases for the specified hostname
+        if data.result == 3:
+            raise KeaLeaseNotFoundException(
+                f"Unable to find a lease using duid '{duid}'"
+            )
+
+        lease = data.arguments["leases"][0]
+        return Lease6.parse_obj(lease)
+
+    def lease6_get_by_hostname(self, hostname: str) -> Lease6:
+        """Retrieves all IPv6 leases for the specified hostname
 
         Args:
             hostname:   Hostname
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-get-by-hostname
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease6-get-by-hostname
         """
-        return self.api.send_command_with_arguments(
-            command="lease4-get-by-hostname",
+        data = self.api.send_command_with_arguments(
+            command="lease6-get-by-hostname",
             service=self.service,
             arguments={"hostname": hostname},
+            required_hook="lease_cmds",
         )
 
-    def lease4_get_by_hw_address(self, hw_address: str) -> dict:
-        """Retrieves all IPv4 leases for the specified hardware address
-
-        Args:
-            hw_address:     Hardware Address
+        if data.result == 3:
+            raise KeaLeaseNotFoundException(
+                f"Unable to find lease using hostname '{hostname}'"
+            )
 
-        Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-get-by-hw-address
-        """
-        return self.api.send_command_with_arguments(
-            command="lease4-get-by-hw-address",
-            service=self.service,
-            arguments={"hw-address": hw_address},
-        )
+        lease = data.arguments["leases"][0]
+        return Lease6.parse_obj(lease)
 
-    def lease4_get_page(self, limit: int, search_from: str) -> dict:
-        """Retrieves all IPv4 leases by page
+    def lease6_get_page(self, limit: int, search_from: str) -> Lease6Page:
+        """Retrieves all IPv6 leases by page
 
         Args:
-            limit:          Set the limit of IPv4 leases to be returned
+            limit:          Set the limit of IPv6 leases to be returned
             search_from:    Start from either a specific IP address or 'start' for the first
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-get-page
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease6-get-page
         """
-        return self.api.send_command_with_arguments(
-            command="lease4-get-page",
+        data = self.api.send_command_with_arguments(
+            command="lease6-get-page",
             service=self.service,
             arguments={"from": search_from, "limit": limit},
+            required_hook="lease_cmds",
         )
 
-    def lease4_resend_ddns(self, ip_address: str) -> dict:
+        return Lease6Page.parse_obj(data.arguments)
+
+    def lease6_resend_ddns(self, ip_address: str) -> KeaResponse:
         """Sends an internal request to the ddns daemon to update DNS for an existing lease
 
         Args:
             ip_address:     Lease to update DDNS record
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-resend-ddns
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease6-resend-ddns
         """
         return self.api.send_command_with_arguments(
-            command="lease4-resend-ddns",
+            command="lease6-resend-ddns",
             service=self.service,
             arguments={"ip-address": ip_address},
+            required_hook="lease_cmds",
         )
 
-    def lease4_update(
-        self,
-        ip_address: str,
-        hostname: str = "",
-        hw_address: str = "",
-        subnet_id: int = None,
-        force_create: bool = None,
-    ) -> dict:
+    def lease6_update(
+        self, ip_address: str, duid: str, iaid: int, **kwargs
+    ) -> KeaResponse:
         """Updates an existing lease
 
         Args:
-            ip_address:     Lease IPv4 Address
-            hostname:       Hostname of lease
-            hw_address:     Ethernet MAC address
-            subnet_id:      ID of the subnet
-            force_create:   Creates the lease if it doesn't exist
+            ip_address:     Lease IPv6 Address
+            duid:           DHCP Unique Identifier
+            iaid:           IAID
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-update
         """
-        payload = {"ip-address": ip_address}
-        if hostname:
-            payload["hostname"] = hostname
-        if hw_address:
-            payload["hw-address"] = hw_address
-        if subnet_id:
-            payload["subnet-id"] = subnet_id
-        if force_create:
-            payload["force-create"] = force_create
-
-        return self.api.send_command_with_arguments(
-            command="lease4-update", service=self.service, arguments=payload
-        )
-
-    def lease4_wipe(self, subnet_id: int) -> dict:
-        """Removes all leases assosicated to the specified subnet id
-
-        Args:
-            subnet_id:      ID of the subnet
+        lease = Lease6(ip_address=ip_address, duid=duid, iaid=iaid, **kwargs)
 
-        Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-wipe
-        """
         return self.api.send_command_with_arguments(
-            command="lease4-wipe",
+            command="lease6-update",
             service=self.service,
-            arguments={"subnet-id": subnet_id},
-        )
-
-    def leases_reclaim(self) -> dict:
-        """Instructs the dhcp4 daemon to reclaim all expired leases
-
-        Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-leases-reclaim
-        """
-        return self.api.send_command_with_arguments(
-            command="leases-reclaim", service=self.service, arguments={"remove": True}
+            arguments=lease.dict(exclude_none=True, by_alias=True),
+            required_hook="lease_cmds",
         )
 
-    def libreload(self) -> dict:
-        """Unloads and then reloads all currently loaded hook libraries
-
-        Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#libreload
-        """
-        return self.api.send_command_with_arguments(
-            command="libreload", service=self.service, arguments={}
-        )
-
-    def list_commands(self) -> dict:
+    def list_commands(self) -> KeaResponse:
         """List all commands supported by the server/service
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-list-commands
         """
         return self.api.send_command_with_arguments(
             command="list-commands", service=self.service, arguments={}
         )
 
-    def network4_add(self, shared_networks: List[Dict]) -> dict:
-        """Adds a new shared network
+    def network6_add(self, shared_networks: List[SharedNetwork6]) -> KeaResponse:
+        """Adds new shared networks
 
         Args:
-            shared_networks:        List of shared networks to add
+            shared_networks:        List of Shared Networks to add
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-network4-add
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-network6-add
         """
         return self.api.send_command_with_arguments(
-            command="network4-add",
+            command="network6-add",
             service=self.service,
-            arguments={"shared-networks": shared_networks},
+            arguments={
+                "shared-networks": [
+                    network.dict(exclude_none=True) for network in shared_networks
+                ]
+            },
+            required_hook="subnet_cmds",
         )
 
-    def network4_del(self, name: str) -> dict:
+    def network6_del(self, name: str) -> KeaResponse:
         """Deletes an existing shared network
 
         Args:
             name:       Name of shared network
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#network4-del
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#network6-del
         """
         return self.api.send_command_with_arguments(
-            command="network4-del", service=self.service, arguments={"name": name}
+            command="network6-del",
+            service=self.service,
+            arguments={"name": name},
+            required_hook="subnet_cmds",
         )
 
-    def network4_get(self, name: str) -> dict:
+    def network6_get(self, name: str) -> SharedNetwork6:
         """Returns detailed information about a shared network, including subnets
 
         Args:
             name:       Name of shared network
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#network4-get
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#network6-get
         """
-        return self.api.send_command_with_arguments(
-            command="network4-get", service=self.service, arguments={"name": name}
+        data = self.api.send_command_with_arguments(
+            command="network6-get",
+            service=self.service,
+            arguments={"name": name},
+            required_hook="subnet_cmds",
         )
 
-    def network4_list(self) -> dict:
+        if data.result == 3:
+            raise KeaSharedNetworkNotFoundException(name)
+
+        if not data.arguments["shared-networks"]:
+            return None
+
+        shared_network = data.arguments["shared-networks"][0]
+        return SharedNetwork6.parse_obj(shared_network)
+
+    def network6_list(self) -> List[SharedNetwork6]:
         """Returns a full list of the current shared networks configured
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#network4-list
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#network6-list
         """
-        return self.api.send_command(command="network4-list", service=self.service)
+        data = self.api.send_command(
+            command="network6-list",
+            service=self.service,
+            required_hook="subnet_cmds",
+        )
+
+        networks = [
+            SharedNetwork6.parse_obj(network)
+            for network in data.arguments["shared-networks"]
+        ]
+        return networks
 
-    def network4_subnet_add(self, name: str, subnet_id: int) -> dict:
+    def network6_subnet_add(self, name: str, subnet_id: int) -> KeaResponse:
         """Add an existing subnet to an existing shared network
 
         Args:
             name:       Name of shared network
             subnet_id:  ID of the subnet
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#network4-subnet-add
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#network6-subnet-add
         """
         return self.api.send_command_with_arguments(
-            command="network4-subnet-add",
+            command="network6-subnet-add",
             service=self.service,
             arguments={"name": name, "id": subnet_id},
+            required_hook="subnet_cmds",
         )
 
-    def network4_subnet_del(self, name: str, subnet_id: int) -> dict:
+    def network6_subnet_del(self, name: str, subnet_id: int) -> KeaResponse:
         """Remove a subnet that is part of an existing shared network and demotes it to a plain standalone subnet
 
         Args:
             name:       Name of shared network
             subnet_id:  ID of the subnet
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#network4-subnet-del
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#network6-subnet-del
         """
         return self.api.send_command_with_arguments(
-            command="network4-subnet-del",
+            command="network6-subnet-del",
             service=self.service,
             arguments={"name": name, "id": subnet_id},
+            required_hook="subnet_cmds",
         )
 
-    def reservation_add(self) -> dict:
-        pass
-
-    def reservation_del(self) -> dict:
-        pass
-
-    def reservation_get(self) -> dict:
-        pass
-
-    def reservation_get_all(self) -> dict:
-        pass
-
-    def reservation_get_by_hostname(self) -> dict:
-        pass
-
-    def reservation_get_by_id(self) -> dict:
-        pass
-
-    def reservation_get_page(self) -> dict:
-        pass
-
-    def server_tag_get(self) -> dict:
-        pass
-
-    def shutdown(self) -> dict:
+    def shutdown(self) -> KeaResponse:
         """Instructs the server daemon to initiate its shutdown procedure
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-shutdown
         """
         return self.api.send_command_with_arguments(
             command="shutdown", service=self.service, arguments={"exit-value": 3}
         )
 
-    def stat_lease4_get(self) -> dict:
-        pass
-
-    def statistic_get(self, name: str) -> dict:
+    def statistic_get(self, name: str) -> KeaResponse:
         """Returns single statistic
 
         Args:
             name:       Name of the statistic to get
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-statistic-get
         """
         return self.api.send_command_with_arguments(
             command="statistic-get", service=self.service, arguments={"name": name}
         )
 
-    def statistic_get_all(self) -> dict:
+    def statistic_get_all(self) -> KeaResponse:
         """Returns all recorded statistics
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-statistic-get-all
         """
         return self.api.send_command_with_arguments(
             command="statistic-get-all", service=self.service, arguments={}
         )
 
-    def statistic_remove(self) -> dict:
-        pass
-
-    def statistic_remove_all(self) -> dict:
-        pass
-
-    def statistic_reset(self) -> dict:
-        pass
-
-    def statistic_reset_all(self) -> dict:
-        pass
-
-    def statistic_sample_age_set(self) -> dict:
-        pass
-
-    def statistic_sample_age_set_all(self) -> dict:
-        pass
-
-    def statistic_sample_count_set(self) -> dict:
-        pass
-
-    def statistic_sample_count_set_all(self) -> dict:
-        pass
-
-    def status_get(self) -> dict:
+    def status_get(self) -> StatusGet:
         """Returns servers runtime information
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-status-get
         """
-        return self.api.send_command(command="status-get", service=self.service)
+        data = self.api.send_command(command="status-get", service=self.service)
+        return StatusGet.parse_obj(data.arguments)
 
-    def subnet4_add(self, subnets: List[Dict]) -> dict:
+    def subnet6_add(self, subnets: List[Subnet6]) -> KeaResponse:
         """Creates and adds a new subnet
 
         Args:
             subnets:        List of subnets to add
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-subnet4-add
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet6-add
         """
         return self.api.send_command_with_arguments(
-            command="subnet4-add", service=self.service, arguments={"subnet4": subnets}
+            command="subnet6-add",
+            service=self.service,
+            arguments={
+                "subnet6": [subnet.dict(exclude_none=True) for subnet in subnets]
+            },
+            required_hook="subnet_cmds",
         )
 
-    def subnet4_del(self, subnet_id: int) -> dict:
+    def subnet6_del(self, subnet_id: int) -> KeaResponse:
         """Removes a subnet
 
         Args:
             subnet_id:      ID of the subnet
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet4-del
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet6-del
         """
-        return self.api.send_command_with_arguments(
-            command="subnet4-del", service=self.service, arguments={"id": subnet_id}
+        data = self.api.send_command_with_arguments(
+            command="subnet6-del",
+            service=self.service,
+            arguments={"id": subnet_id},
+            required_hook="subnet_cmds",
         )
 
-    def subnet4_delta_add(self, subnets: List[Dict]) -> dict:
+        if data.result == 3:
+            raise KeaSubnetNotFoundException(subnet_id)
+
+        return data
+
+    def subnet6_delta_add(self, subnets: List[Subnet6]) -> KeaResponse:
         """Updates (adds or overwrites) parts of a single subnet
 
         Args:
             subnets:        List of subnets to update/add
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet4-delta-add
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet6-delta-add
         """
         return self.api.send_command_with_arguments(
-            command="subnet4-delta-add",
+            command="subnet6-delta-add",
             service=self.service,
-            arguments={"subnet4": subnets},
+            arguments={
+                "subnet6": [subnet.dict(exclude_none=True) for subnet in subnets]
+            },
+            required_hook="subnet_cmds",
         )
 
-    def subnet4_delta_del(self, subnets: List[Dict]) -> dict:
+    def subnet6_delta_del(self, subnets: List[Subnet6]) -> KeaResponse:
         """Updates (removes) parts of a single subnet
 
         Args:
             subnets:        List of subnets to update/delete
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet4-delta-del
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet6-delta-del
         """
         return self.api.send_command_with_arguments(
-            command="subnet4-delta-del",
+            command="subnet6-delta-del",
             service=self.service,
-            arguments={"subnet4": subnets},
+            arguments={
+                "subnet6": [subnet.dict(exclude_none=True) for subnet in subnets]
+            },
+            required_hook="subnet_cmds",
         )
 
-    def subnet4_get(self, subnet_id: int) -> dict:
+    def subnet6_get(self, subnet_id: int) -> Subnet6:
         """Gets detailed information about the specified subnet
 
         Args:
             subnet_id:      ID of the subnet
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet4-get
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet6-get
         """
-        return self.api.send_command_with_arguments(
-            command="subnet4-get", service=self.service, arguments={"id": subnet_id}
+        data = self.api.send_command_with_arguments(
+            command="subnet6-get",
+            service=self.service,
+            arguments={"id": subnet_id},
+            required_hook="subnet_cmds",
         )
 
-    def subnet4_list(self) -> dict:
+        if data.result == 3:
+            raise KeaSubnetNotFoundException(subnet_id)
+
+        if not data.arguments["subnet6"]:
+            return None
+
+        subnet = data.arguments["subnet6"][0]
+        return Subnet6.parse_obj(subnet)
+
+    def subnet6_list(self) -> List[Subnet6]:
         """List all currently configured subnets
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet4-list
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet6-list
         """
-        return self.api.send_command(command="subnet4-list", service=self.service)
+        data = self.api.send_command(
+            command="subnet6-list",
+            service=self.service,
+            required_hook="subnet_cmds",
+        )
+
+        subnets = [Subnet6.parse_obj(subnet) for subnet in data.arguments["subnets"]]
+        return subnets
 
-    def subnet4_update(self, subnets: List[Dict]) -> dict:
+    def subnet6_update(self, subnets: List[Subnet6]) -> List[Subnet6]:
         """Updates (overwrites) a single subnet
 
         Args:
             subnets:        List of subnets to overwrite
 
         Kea API Reference:
-            https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet4-update
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet6-update
         """
         return self.api.send_command_with_arguments(
-            command="subnet4-update",
+            command="subnet6-update",
             service=self.service,
-            arguments={"subnet4": subnets},
+            arguments={
+                "subnet6": [subnet.dict(exclude_none=True) for subnet in subnets]
+            },
+            required_hook="subnet_cmds",
         )
 
-    def version_get(self) -> dict:
+    def version_get(self) -> KeaResponse:
         """Returns extended information about the Kea Version that is running
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-version-get
         """
         return self.api.send_command(command="version-get", service=self.service)
```

