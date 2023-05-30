# Comparing `tmp/rciam-federation-registry-agent-3.0.1.tar.gz` & `tmp/rciam-federation-registry-agent-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rciam-federation-registry-agent-3.0.1.tar", last modified: Thu Dec 15 13:40:27 2022, max compression
+gzip compressed data, was "dist/rciam-federation-registry-agent-3.2.0.tar", last modified: Tue May 30 10:53:02 2023, max compression
```

## Comparing `rciam-federation-registry-agent-3.0.1.tar` & `rciam-federation-registry-agent-3.2.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-12-15 13:40:27.469269 rciam-federation-registry-agent-3.0.1/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-12-15 13:40:27.465269 rciam-federation-registry-agent-3.0.1/Keycloak/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10721 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/Keycloak/KeycloakClientApi.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/Keycloak/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11340 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/LICENSE
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-12-15 13:40:27.465269 rciam-federation-registry-agent-3.0.1/MitreidConnect/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7323 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/MitreidConnect/MitreidClientApi.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/MitreidConnect/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5867 2022-12-15 13:40:27.469269 rciam-federation-registry-agent-3.0.1/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5192 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/README.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-12-15 13:40:27.466269 rciam-federation-registry-agent-3.0.1/ServiceRegistryAms/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     2425 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/ServiceRegistryAms/PullPublish.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/ServiceRegistryAms/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-12-15 13:40:27.466269 rciam-federation-registry-agent-3.0.1/Utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/Utils/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1483 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/Utils/common.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1506 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/Utils/oauth.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-12-15 13:40:27.467270 rciam-federation-registry-agent-3.0.1/bin/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18637 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/bin/deployer_keycloak
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     6818 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/bin/deployer_mitreid
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     6459 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/bin/deployer_ssp
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-12-15 13:40:27.468269 rciam-federation-registry-agent-3.0.1/rciam_federation_registry_agent.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5867 2022-12-15 13:40:27.000000 rciam-federation-registry-agent-3.0.1/rciam_federation_registry_agent.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      759 2022-12-15 13:40:27.000000 rciam-federation-registry-agent-3.0.1/rciam_federation_registry_agent.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2022-12-15 13:40:27.000000 rciam-federation-registry-agent-3.0.1/rciam_federation_registry_agent.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2022-12-15 13:40:27.000000 rciam-federation-registry-agent-3.0.1/rciam_federation_registry_agent.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      142 2022-12-15 13:40:27.000000 rciam-federation-registry-agent-3.0.1/rciam_federation_registry_agent.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       55 2022-12-15 13:40:27.000000 rciam-federation-registry-agent-3.0.1/rciam_federation_registry_agent.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      154 2022-12-15 13:40:27.470270 rciam-federation-registry-agent-3.0.1/setup.cfg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1491 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/setup.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-12-15 13:40:27.469269 rciam-federation-registry-agent-3.0.1/tests/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/tests/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25367 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/tests/test_deployer_keycloak.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     4707 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/tests/test_deployer_mitreid.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     6565 2022-12-15 13:39:28.000000 rciam-federation-registry-agent-3.0.1/tests/test_deployer_ssp.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-30 10:53:02.470576 rciam-federation-registry-agent-3.2.0/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-30 10:53:02.465576 rciam-federation-registry-agent-3.2.0/Keycloak/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11427 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/Keycloak/KeycloakClientApi.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/Keycloak/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11340 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/LICENSE
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-30 10:53:02.465576 rciam-federation-registry-agent-3.2.0/MitreidConnect/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7366 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/MitreidConnect/MitreidClientApi.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/MitreidConnect/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5877 2023-05-30 10:53:02.470576 rciam-federation-registry-agent-3.2.0/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5202 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/README.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-30 10:53:02.466576 rciam-federation-registry-agent-3.2.0/ServiceRegistryAms/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     2400 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/ServiceRegistryAms/PullPublish.py
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/ServiceRegistryAms/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-30 10:53:02.466576 rciam-federation-registry-agent-3.2.0/Utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/Utils/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1493 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/Utils/common.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1531 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/Utils/oauth.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-30 10:53:02.467576 rciam-federation-registry-agent-3.2.0/bin/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18821 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/bin/deployer_keycloak
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     7011 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/bin/deployer_mitreid
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     6467 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/bin/deployer_ssp
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       30 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/pyproject.toml
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-30 10:53:02.469576 rciam-federation-registry-agent-3.2.0/rciam_federation_registry_agent.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5877 2023-05-30 10:53:02.000000 rciam-federation-registry-agent-3.2.0/rciam_federation_registry_agent.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      774 2023-05-30 10:53:02.000000 rciam-federation-registry-agent-3.2.0/rciam_federation_registry_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-30 10:53:02.000000 rciam-federation-registry-agent-3.2.0/rciam_federation_registry_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-30 10:53:02.000000 rciam-federation-registry-agent-3.2.0/rciam_federation_registry_agent.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      166 2023-05-30 10:53:02.000000 rciam-federation-registry-agent-3.2.0/rciam_federation_registry_agent.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       55 2023-05-30 10:53:02.000000 rciam-federation-registry-agent-3.2.0/rciam_federation_registry_agent.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      154 2023-05-30 10:53:02.471576 rciam-federation-registry-agent-3.2.0/setup.cfg
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1494 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/setup.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-30 10:53:02.470576 rciam-federation-registry-agent-3.2.0/tests/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/tests/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25028 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/tests/test_deployer_keycloak.py
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     6434 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/tests/test_deployer_mitreid.py
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     7253 2023-05-30 10:51:57.000000 rciam-federation-registry-agent-3.2.0/tests/test_deployer_ssp.py
```

### Comparing `rciam-federation-registry-agent-3.0.1/Keycloak/KeycloakClientApi.py` & `rciam-federation-registry-agent-3.2.0/Keycloak/KeycloakClientApi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import requests, json
 from urllib.parse import quote
 
+import requests
+
 """
 Manages all clients on Keycloak
 
 """
 
 
 class KeycloakClientApi:
@@ -31,15 +32,17 @@
         client_id (str): The client_id of the client
     
     Returns:
         response (JSON Object): A registered client in JSON format
     """
 
     def get_client_by_id(self, client_id):
-        url = self.auth_url + "/realms/" + self.realm + "/clients-registrations/default/" + quote(str(client_id), safe="")
+        url = (
+            self.auth_url + "/realms/" + self.realm + "/clients-registrations/default/" + quote(str(client_id), safe="")
+        )
         header = {"Authorization": "Bearer " + self.token}
 
         return self.http_request("GET", url, header)
 
     """
     Register new client
 
@@ -67,15 +70,17 @@
         client_object (str): A string with the client data in JSON format
     
     Returns:
         response (JSON Object): The registered client in JSON format
     """
 
     def update_client(self, client_id, client_object):
-        url = self.auth_url + "/realms/" + self.realm + "/clients-registrations/default/" + quote(str(client_id), safe="")
+        url = (
+            self.auth_url + "/realms/" + self.realm + "/clients-registrations/default/" + quote(str(client_id), safe="")
+        )
         header = {
             "Authorization": "Bearer " + self.token,
             "Content-Type": "application/json",
         }
 
         return self.http_request("PUT", url, header, client_object)
 
@@ -86,15 +91,17 @@
         client_id (str): The client_id of the client
     
     Returns:
         response (JSON Object): The registered client in JSON format
     """
 
     def delete_client(self, client_id):
-        url = self.auth_url + "/realms/" + self.realm + "/clients-registrations/default/" + quote(str(client_id), safe="")
+        url = (
+            self.auth_url + "/realms/" + self.realm + "/clients-registrations/default/" + quote(str(client_id), safe="")
+        )
         header = {"Authorization": "Bearer " + self.token}
 
         return self.http_request("DELETE", url, header)
 
     """
     Get OIDC client's "Permissions"
 
@@ -123,15 +130,15 @@
     """
 
     def update_client_authz_permissions(self, keycloak_id, action):
         url = self.auth_url + "/admin/realms/" + self.realm + "/clients/" + str(keycloak_id) + "/management/permissions"
         header = {"Authorization": "Bearer " + self.token}
         if action == "enable":
             enabled = True
-        elif action == "disable":
+        else:
             enabled = False
         client_object = {"enabled": enabled}
 
         return self.http_request("PUT", url, header, client_object)
 
     """
     Get realm default client scopes
@@ -290,23 +297,45 @@
     """
 
     def http_request(self, method, url, header, data=None):
         try:
             response = requests.request(method, url, headers=header, json=data)
             response.raise_for_status()
         except requests.exceptions.HTTPError as errh:
-            print("Http Error: %s with error: %s" % (url, repr(errh)))
-            return {"status": response.status_code, "error": repr(errh)}
+            print("HTTP Error: %s with error: HTTP %s and response: %s" % (url, response.status_code, response.json()))
+            return {
+                "status": response.status_code,
+                "error": repr(errh),
+                "response": response.json(),
+            }
         except requests.exceptions.ConnectionError as errc:
-            print("Error Connecting: %s with error: %s" % (url, repr(errc)))
-            return {"status": response.status_code, "error": repr(errc)}
+            print(
+                "Connection Error: %s with error: HTTP  %s and response: %s"
+                % (url, response.status_code, response.text)
+            )
+            return {
+                "status": response.status_code,
+                "error": repr(errc),
+                "response": response.json(),
+            }
         except requests.exceptions.Timeout as errt:
-            print("Timeout Error: %s with error: %s" % (url, repr(errt)))
-            return {"status": response.status_code, "error": repr(errt)}
+            print("Timeout Error: %s with error: HTTP %s and response: %s" % (url, response.status_code, response.text))
+            return {
+                "status": response.status_code,
+                "error": repr(errt),
+                "response": response.json(),
+            }
         except requests.exceptions.RequestException as err:
-            print("Failed to make request to %s with error: %s" % (url, err))
-            return {"status": response.status_code, "error": repr(err)}
+            print(
+                "Failed to make request to %s with error: HTTP  %s and response: %s"
+                % (url, response.status_code, response.text)
+            )
+            return {
+                "status": response.status_code,
+                "error": repr(err),
+                "response": response.json(),
+            }
 
         if method == "DELETE" or response.status_code == 204 or not response.text:
             return {"status": response.status_code, "response": "OK"}
         else:
             return {"status": response.status_code, "response": response.json()}
```

### Comparing `rciam-federation-registry-agent-3.0.1/LICENSE` & `rciam-federation-registry-agent-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rciam-federation-registry-agent-3.0.1/MitreidConnect/MitreidClientApi.py` & `rciam-federation-registry-agent-3.2.0/MitreidConnect/MitreidClientApi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import requests, json
+import requests
 
 """
 Manages all clients on MITREid Connect
 
 """
 
 
@@ -29,31 +29,30 @@
     """
 
     def getClients(self):
         url = self.issuer + "/api/clients"
         header = {"Authorization": "Bearer " + self.token}
 
         try:
-            response = requests.get(url, headers=header)
+            response = requests.get(url, headers=header, timeout=5)
             response.raise_for_status()
         except requests.exceptions.HTTPError as errh:
             print("Http Error: %s with error: %s" % (url, repr(errh)))
-            return {'status': response.status_code,'error': repr(errh) }
+            return {"status": response.status_code, "error": repr(errh)}
         except requests.exceptions.ConnectionError as errc:
             print("Error Connecting: %s with error: %s" % (url, repr(errc)))
-            return {'status': response.status_code,'error': repr(errc) }
+            return {"status": response.status_code, "error": repr(errc)}
         except requests.exceptions.Timeout as errt:
             print("Timeout Error: %s with error: %s" % (url, repr(errt)))
-            return {'status': response.status_code,'error': repr(errt) }
+            return {"status": response.status_code, "error": repr(errt)}
         except requests.exceptions.RequestException as err:
             print("Failed to make request to %s with error: %s" % (url, err))
-            return {'status': response.status_code,'error': repr(err) }
-
-        return {'status': response.status_code,'response': response.json()}
+            return {"status": response.status_code, "error": repr(err)}
 
+        return {"status": response.status_code, "response": response.json()}
 
     """
     Get a registered client by ID
 
     Parameters:
         id (str): The id of the client
     
@@ -62,31 +61,30 @@
     """
 
     def getClientById(self, id):
         url = self.issuer + "/api/clients/" + str(id)
         header = {"Authorization": "Bearer " + self.token}
 
         try:
-            response = requests.get(url, headers=header)
+            response = requests.get(url, headers=header, timeout=5)
             response.raise_for_status()
         except requests.exceptions.HTTPError as errh:
             print("Http Error: %s with error: %s" % (url, repr(errh)))
-            return {'status': response.status_code,'error': repr(errh) }
+            return {"status": response.status_code, "error": repr(errh)}
         except requests.exceptions.ConnectionError as errc:
             print("Error Connecting: %s with error: %s" % (url, repr(errc)))
-            return {'status': response.status_code,'error': repr(errc) }
+            return {"status": response.status_code, "error": repr(errc)}
         except requests.exceptions.Timeout as errt:
             print("Timeout Error: %s with error: %s" % (url, repr(errt)))
-            return {'status': response.status_code,'error': repr(errt) }
+            return {"status": response.status_code, "error": repr(errt)}
         except requests.exceptions.RequestException as err:
             print("Failed to make request to %s with error: %s" % (url, err))
-            return {'status': response.status_code,'error': repr(err) }
-
-        return {'status': response.status_code,'response': response.json()}
+            return {"status": response.status_code, "error": repr(err)}
 
+        return {"status": response.status_code, "response": response.json()}
 
     """
     Register new client
 
     Parameters:
         clientObject (str): A string with the client data in JSON format
     
@@ -98,31 +96,30 @@
         url = self.issuer + "/api/clients"
         header = {
             "Authorization": "Bearer " + self.token,
             "Content-Type": "application/json",
         }
 
         try:
-            response = requests.post(url, headers=header, json=clientObject)
+            response = requests.post(url, headers=header, json=clientObject, timeout=5)
             response.raise_for_status()
         except requests.exceptions.HTTPError as errh:
             print("Http Error: %s with error: %s" % (url, repr(errh)))
-            return {'status': response.status_code,'error': repr(errh) }
+            return {"status": response.status_code, "error": repr(errh)}
         except requests.exceptions.ConnectionError as errc:
             print("Error Connecting: %s with error: %s" % (url, repr(errc)))
-            return {'status': response.status_code,'error': repr(errc) }
+            return {"status": response.status_code, "error": repr(errc)}
         except requests.exceptions.Timeout as errt:
             print("Timeout Error: %s with error: %s" % (url, repr(errt)))
-            return {'status': response.status_code,'error': repr(errt) }
+            return {"status": response.status_code, "error": repr(errt)}
         except requests.exceptions.RequestException as err:
             print("Failed to make request to %s with error: %s" % (url, err))
-            return {'status': response.status_code,'error': repr(err) }
-
-        return {'status': response.status_code,'response': response.json()}
+            return {"status": response.status_code, "error": repr(err)}
 
+        return {"status": response.status_code, "response": response.json()}
 
     """
     Update an existing client by ID
 
     Parameters:
         id (str): The id of the client
         clientObject (str): A string with the client data in JSON format
@@ -135,31 +132,30 @@
         url = self.issuer + "/api/clients/" + str(id)
         header = {
             "Authorization": "Bearer " + self.token,
             "Content-Type": "application/json",
         }
 
         try:
-            response = requests.put(url, headers=header, json=clientObject)
+            response = requests.put(url, headers=header, json=clientObject, timeout=5)
             response.raise_for_status()
         except requests.exceptions.HTTPError as errh:
             print("Http Error: %s with error: %s" % (url, repr(errh)))
-            return {'status': response.status_code,'error': repr(errh) }
+            return {"status": response.status_code, "error": repr(errh)}
         except requests.exceptions.ConnectionError as errc:
             print("Error Connecting: %s with error: %s" % (url, repr(errc)))
-            return {'status': response.status_code,'error': repr(errc) }
+            return {"status": response.status_code, "error": repr(errc)}
         except requests.exceptions.Timeout as errt:
             print("Timeout Error: %s with error: %s" % (url, repr(errt)))
-            return {'status': response.status_code,'error': repr(errt) }
+            return {"status": response.status_code, "error": repr(errt)}
         except requests.exceptions.RequestException as err:
             print("Failed to make request to %s with error: %s" % (url, err))
-            return {'status': response.status_code,'error': repr(err) }
-
-        return {'status': response.status_code,'response': response.json()}
+            return {"status": response.status_code, "error": repr(err)}
 
+        return {"status": response.status_code, "response": response.json()}
 
     """
     Delete a registered client by ID
 
     Parameters:
         id (str): The id of the client
     
@@ -168,23 +164,23 @@
     """
 
     def deleteClientById(self, id):
         url = self.issuer + "/api/clients/" + str(id)
         header = {"Authorization": "Bearer " + self.token}
 
         try:
-            response = requests.delete(url, headers=header)       
+            response = requests.delete(url, headers=header, timeout=5)
             response.raise_for_status()
         except requests.exceptions.HTTPError as errh:
             print("Http Error: %s with error: %s" % (url, repr(errh)))
-            return {'status': response.status_code,'error': repr(errh) }
+            return {"status": response.status_code, "error": repr(errh)}
         except requests.exceptions.ConnectionError as errc:
             print("Error Connecting: %s with error: %s" % (url, repr(errc)))
-            return {'status': response.status_code,'error': repr(errc) }
+            return {"status": response.status_code, "error": repr(errc)}
         except requests.exceptions.Timeout as errt:
             print("Timeout Error: %s with error: %s" % (url, repr(errt)))
-            return {'status': response.status_code,'error': repr(errt) }
+            return {"status": response.status_code, "error": repr(errt)}
         except requests.exceptions.RequestException as err:
             print("Failed to make request to %s with error: %s" % (url, err))
-            return {'status': response.status_code,'error': repr(err) }
+            return {"status": response.status_code, "error": repr(err)}
 
-        return {'status': response.status_code,'response': 'OK'}
+        return {"status": response.status_code, "response": "OK"}
```

### Comparing `rciam-federation-registry-agent-3.0.1/PKG-INFO` & `rciam-federation-registry-agent-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rciam-federation-registry-agent
-Version: 3.0.1
+Version: 3.2.0
 Summary: A library that connects to ams using argo-ams-library and syncs with MITREid, SimpleSAMLphp and Keycloak
 Home-page: https://github.com/rciam/rciam-federation-registry-agent
 Author: grnet
 Author-email: faai@grnet.gr
 License: ASL 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: PHP
@@ -146,37 +146,37 @@
   ams.publish(args)
 ```
 
 ### Keycloak
 
 Use Keycloak as an API manager to communicate with Keycloak
 
-- First obtain an access token and create the Keycloak API Client (find clientCredentialsGrant under `Utils` directory)
+- First obtain an access token and create the Keycloak API Client (find client_credentials_grant under `Utils` directory)
 
 ```python
-  access_token = clientCredentialsGrant(issuer_url, client_id, client_secret)
+  access_token = client_credentials_grant(issuer_url, client_id, client_secret)
   keycloak_agent = KeycloakClientApi(issuer_url, access_token)
 ```
 
-- Use the following functions to create, delete and update a service on clientCredentialsGrant
+- Use the following functions to create, delete and update a service on client_credentials_grant
 
 ```python
   response = keycloak_agent.create_client(keycloak_msg)
   response = keycloak_agent.update_client(external_id, keycloak_msg)
   response = keycloak_agent.delete_client(external_id)
 ```
 
 ### MITREid Connect
 
 Use MITREid Connect as an API manager to communicate with MITREid
 
-- First obtain an access token and create the MITREid API Client (find refreshTokenGrant under `Utils` directory)
+- First obtain an access token and create the MITREid API Client (find refresh_token_grant under `Utils` directory)
 
 ```python
-  access_token = refreshTokenGrant(issuer_url, refresh_token, client_id, client_secret)
+  access_token = refresh_token_grant(issuer_url, refresh_token, client_id, client_secret)
   mitreid_agent = mitreidClientApi(issuer_url, access_token)
 ```
 
 - Use the following functions to create, delete and update a service on MITREid
 
 ```python
   response = mitreid_agent.createClient(mitreid_msg)
```

### Comparing `rciam-federation-registry-agent-3.0.1/README.md` & `rciam-federation-registry-agent-3.2.0/rciam_federation_registry_agent.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: rciam-federation-registry-agent
+Version: 3.2.0
+Summary: A library that connects to ams using argo-ams-library and syncs with MITREid, SimpleSAMLphp and Keycloak
+Home-page: https://github.com/rciam/rciam-federation-registry-agent
+Author: grnet
+Author-email: faai@grnet.gr
+License: ASL 2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: PHP
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # rciam-federation-registry-agent
 
 **RCIAM Federation Registry Agent** main objective is to sync data between RCIAM Federation Registry and
 different identity and access management solutions, such as Keycloak, SATOSA, SimpleSAMLphp and MITREid Connect.
 This python library includes a module named `ServiceRegistryAms/` to pull and publish messages from ARGO Messaging
 Service using the argo-ams-library, an API module named `MitreidConnect/` to communicate with the API of the MITREid, an
 API module named `Keycloak/` to communicate with the API of the Keycloak.
@@ -129,37 +146,37 @@
   ams.publish(args)
 ```
 
 ### Keycloak
 
 Use Keycloak as an API manager to communicate with Keycloak
 
-- First obtain an access token and create the Keycloak API Client (find clientCredentialsGrant under `Utils` directory)
+- First obtain an access token and create the Keycloak API Client (find client_credentials_grant under `Utils` directory)
 
 ```python
-  access_token = clientCredentialsGrant(issuer_url, client_id, client_secret)
+  access_token = client_credentials_grant(issuer_url, client_id, client_secret)
   keycloak_agent = KeycloakClientApi(issuer_url, access_token)
 ```
 
-- Use the following functions to create, delete and update a service on clientCredentialsGrant
+- Use the following functions to create, delete and update a service on client_credentials_grant
 
 ```python
   response = keycloak_agent.create_client(keycloak_msg)
   response = keycloak_agent.update_client(external_id, keycloak_msg)
   response = keycloak_agent.delete_client(external_id)
 ```
 
 ### MITREid Connect
 
 Use MITREid Connect as an API manager to communicate with MITREid
 
-- First obtain an access token and create the MITREid API Client (find refreshTokenGrant under `Utils` directory)
+- First obtain an access token and create the MITREid API Client (find refresh_token_grant under `Utils` directory)
 
 ```python
-  access_token = refreshTokenGrant(issuer_url, refresh_token, client_id, client_secret)
+  access_token = refresh_token_grant(issuer_url, refresh_token, client_id, client_secret)
   mitreid_agent = mitreidClientApi(issuer_url, access_token)
 ```
 
 - Use the following functions to create, delete and update a service on MITREid
 
 ```python
   response = mitreid_agent.createClient(mitreid_msg)
```

### Comparing `rciam-federation-registry-agent-3.0.1/ServiceRegistryAms/PullPublish.py` & `rciam-federation-registry-agent-3.2.0/ServiceRegistryAms/PullPublish.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import json
-from argparse import ArgumentParser
-from argo_ams_library import ArgoMessagingService,AmsMessage, AmsException
 
-class PullPublish():
-    def __init__(self,config):
-        self.pull_sub = config['pull_sub']
-        self.pub_topic = config['pub_topic']
-        self.pull_topic = config['pull_topic']
-        self.ams = ArgoMessagingService(endpoint=config['host'], token=config['token'], project=config['project'])
+from argo_ams_library import AmsException, AmsMessage, ArgoMessagingService
 
-    def pull(self,nummsgs):
+
+class PullPublish:
+    def __init__(self, config):
+        self.pull_sub = config["pull_sub"]
+        self.pub_topic = config["pub_topic"]
+        self.pull_topic = config["pull_topic"]
+        self.ams = ArgoMessagingService(endpoint=config["host"], token=config["token"], project=config["project"])
+
+    def pull(self, nummsgs):
         messages = []
         try:
             if not self.ams.has_sub(self.pull_sub):
-                self.ams.create_sub(self.pull_sub,self.pull_topic)
+                self.ams.create_sub(self.pull_sub, self.pull_topic)
         except AmsException as e:
             print(e)
             raise SystemExit(1)
 
         # try to pull number of messages from subscription. method will
         # return (ackIds, AmsMessage) tuples from which ackIds and messages
         # payload will be extracted.
         ackids = list()
         for id, msg in self.ams.pull_sub(self.pull_sub, nummsgs):
             data = msg.get_data()
-            msgid = msg.get_msgid()
-            attr = msg.get_attr()
+            # msgid = msg.get_msgid()
+            # attr = msg.get_attr()
             messages.append(json.loads(data.decode("utf-8")))
-            #print('msgid={0}, data={1}, attr={2}'.format(msgid, data, attr))
+            # print('msgid={0}, data={1}, attr={2}'.format(msgid, data, attr))
             ackids.append(id)
         return messages, ackids
 
-    def ack(self,ackids):
+    def ack(self, ackids):
         # pass list of extracted ackIds to AMS Service so that
         # it can move the offset for the next subscription pull
         # (basically acknowledging pulled messages)
         if ackids:
             self.ams.ack_sub(self.pull_sub, ackids)
 
-    def publish(self,messages):
+    def publish(self, messages):
         # messages = [{data:[{id:1},{state:'deployed'}],attributes=''}]
         try:
             if not self.ams.has_topic(self.pub_topic):
                 self.ams.create_topic(self.pub_topic)
         except AmsException as e:
             print(e)
             raise SystemExit(1)
@@ -50,15 +51,14 @@
         # publish one message to given topic. message is constructed with
         # help of AmsMessage which accepts data and attributes keys.
         # data is Base64 encoded, attributes is dictionary of arbitrary
         # key/value pairs
         msg = AmsMessage()
         msglist = []
         for message in messages:
-            msglist.append(msg(data=json.dumps(message['data']),attributes={}))
-
+            msglist.append(msg(data=json.dumps(message["data"]), attributes={}))
 
         try:
             ret = self.ams.publish(self.pub_topic, msglist)
             print(ret)
         except AmsException as e:
             print(e)
```

### Comparing `rciam-federation-registry-agent-3.0.1/Utils/common.py` & `rciam-federation-registry-agent-3.2.0/Utils/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import logging.config
 import logging
+import logging.config
 
 
 def get_log_conf(log_config_file=None):
     """
     Method that searches and gets the default location of configuration and logging configuration
     """
     if log_config_file is not None:
@@ -11,33 +11,33 @@
     else:
         logging.basicConfig(level=logging.INFO, format=logging.BASIC_FORMAT)
 
 
 # create_ams_response creates a json object with the result of the mitreId api call
 # that is readable from the rciam-federation-registry
 def create_ams_response(response, service_id, deployer_name, external_id, client_id):
-    msgNew = {}
-    msgNew["id"] = service_id
-    msgNew["status_code"] = response["status"]
+    new_msg = {}
+    new_msg["id"] = service_id
+    new_msg["status_code"] = response["status"]
     if len(deployer_name) > 0:
-        msgNew["deployer_name"] = deployer_name
+        new_msg["deployer_name"] = deployer_name
 
     if len(external_id) > 0:
-        msgNew["external_id"] = external_id
+        new_msg["external_id"] = external_id
 
     if len(client_id) > 0:
-        msgNew["client_id"] = client_id
+        new_msg["client_id"] = client_id
 
     if response["status"] != 200 and response["status"] != 201 and response["status"] != 204:
-        msgNew["error_description"] = response["error"]
-        msgNew["state"] = "error"
+        new_msg["error_description"] = response["error"]
+        new_msg["state"] = "error"
     else:
-        msgNew["state"] = "deployed"
+        new_msg["state"] = "deployed"
 
-    return msgNew
+    return new_msg
 
 
 """
 Method that creates the Keycloak issuer based on `auth_server` + `realm`
 
 Parameters:
     config (dict): Keycloak's config options
```

### Comparing `rciam-federation-registry-agent-3.0.1/Utils/oauth.py` & `rciam-federation-registry-agent-3.2.0/Utils/oauth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from requests_oauthlib import OAuth2Session
 from oauthlib.oauth2 import BackendApplicationClient
+from requests_oauthlib import OAuth2Session
 
 """Refreshing an OAuth 2 token using a refresh token.
 :param issuer: The token endpoint, must be HTTPS.
 :param refresh_token: The refresh_token to use.
 :param client_id: Client id obtained during registration
 :param client_secret: Client secret obtained during registration
 :return: An access token
 """
 
 
-def refreshTokenGrant(issuer, refreshToken, clientId, clientSecret):
-    tokenUrl = issuer + "/token"
+def refresh_token_grant(issuer, refresh_token, client_id, client_secret):
+    token_url = issuer + "/token"
 
-    extra = {"client_id": clientId, "client_secret": clientSecret}
+    extra = {"client_id": client_id, "client_secret": client_secret}
 
     try:
         print("Get access token from " + issuer)
         provider = OAuth2Session()
-        response = provider.refresh_token(tokenUrl, refreshToken, **extra)
+        response = provider.refresh_token(token_url, refresh_token, **extra)
     except:
         print("Failed to get access token")
         raise SystemExit(1)
     return response["access_token"]
 
 
-def clientCredentialsGrant(issuer, clientId, clientSecret):
-    tokenUrl = issuer + "/protocol/openid-connect/token"
+def client_credentials_grant(issuer, client_id, client_secret):
+    token_url = issuer + "/protocol/openid-connect/token"
 
     try:
-        print("[clientCredentialsGrant] Get access token from " + issuer)
-        client = BackendApplicationClient(client_id=clientId)
+        print("[client_credentials_grant] Get access token from " + issuer)
+        client = BackendApplicationClient(client_id=client_id)
         oauth = OAuth2Session(client=client)
-        response = oauth.fetch_token(token_url=tokenUrl, client_id=clientId, client_secret=clientSecret)
-        print("[clientCredentialsGrant] Access Token: " + response["access_token"])
+        response = oauth.fetch_token(token_url=token_url, client_id=client_id, client_secret=client_secret)
+        print("[client_credentials_grant] Access Token: " + response["access_token"])
     except:
-        print("[clientCredentialsGrant] Failed to get access token")
+        print("[client_credentials_grant] Failed to get access token")
         raise SystemExit(1)
     return response["access_token"]
```

### Comparing `rciam-federation-registry-agent-3.0.1/bin/deployer_keycloak` & `rciam-federation-registry-agent-3.2.0/bin/deployer_keycloak`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #!/usr/bin/env python3
 
-import json
-import time
 import argparse
+import json
 import logging
-from Utils.common import get_log_conf, create_ams_response, get_keycloak_issuer
-from ServiceRegistryAms.PullPublish import PullPublish
+import time
+
 from Keycloak.KeycloakClientApi import KeycloakClientApi
-from Utils.oauth import clientCredentialsGrant, refreshTokenGrant
+from ServiceRegistryAms.PullPublish import PullPublish
+from Utils.common import create_ams_response, get_keycloak_issuer, get_log_conf
+from Utils.oauth import client_credentials_grant, refresh_token_grant
 
 # Setup logger
 log = logging.getLogger(__name__)
 
 # Set default JSON Data
 jsonOidcTemplate = '{"attributes":{"client_credentials.use_refresh_token":"false","oauth2.device.authorization.grant.enabled":"false","oauth2.token.exchange.grant.enabled":false,"oidc.ciba.grant.enabled":"false","refresh.token.max.reuse":"0","revoke.refresh.token":"false","use.jwks.string":"false","use.jwks.url":"false","use.refresh.tokens":"false"},"directAccessGrantsEnabled":false,"implicitFlowEnabled":false,"publicClient":false,"serviceAccountsEnabled":false,"standardFlowEnabled":false,"webOrigins":["+"]}'
-jsonSamlTemplate = '{"attributes":{"saml.auto.updated":"true","saml.refresh.period":"3600","saml.skip.requested.attributes": "true"}}'
+jsonSamlTemplate = (
+    '{"attributes":{"saml.auto.updated":"true","saml.refresh.period":"3600","saml.skip.requested.attributes": "true"}}'
+)
 
 
 def map_token_endpoint_value(key):
     if key == "client_secret_post":
         return "client-secret"
     elif key == "client_secret_basic":
         return "client-secret"
@@ -74,46 +77,55 @@
             if "jwks" in msg:
                 new_msg["attributes"]["use.jwks.string"] = "true"
                 new_msg["attributes"]["jwks.string"] = json.dumps(msg.pop("jwks"))
             if "jwks_uri" in msg:
                 new_msg["attributes"]["use.jwks.url"] = True
                 new_msg["attributes"]["jwks.url"] = msg.pop("jwks_uri")
             if "refresh_token_validity_seconds" in msg:
-                new_msg["attributes"]["client.offline.session.idle.timeout"] = str(msg["refresh_token_validity_seconds"])
+                new_msg["attributes"]["client.offline.session.idle.timeout"] = str(
+                    msg["refresh_token_validity_seconds"]
+                )
                 if "reuse_refresh_token" in msg:
                     rotate_refresh_token = str(not msg.pop("reuse_refresh_token"))
                     new_msg["attributes"]["revoke.refresh.token"] = rotate_refresh_token.lower()
             if "code_challenge_method" in msg:
                 new_msg["attributes"]["pkce.code.challenge.method"] = msg.pop("code_challenge_method")
             if "access_token_validity_seconds" in msg:
                 if msg["access_token_validity_seconds"] < 60:
                     new_msg["attributes"]["access.token.lifespan"] = "60"
                 else:
                     new_msg["attributes"]["access.token.lifespan"] = str(msg.pop("access_token_validity_seconds"))
             if "id_token_timeout_seconds" in msg:
                 new_msg["attributes"]["id.token.lifespan"] = str(msg.pop("id_token_timeout_seconds"))
             if "device_code_validity_seconds" in msg:
                 new_msg["attributes"]["oauth2.device.code.lifespan"] = str(msg.pop("device_code_validity_seconds"))
-            if new_msg["standardFlowEnabled"] == True or new_msg["attributes"]["oauth2.device.authorization.grant.enabled"] == True:
+            if (
+                new_msg["standardFlowEnabled"] == True
+                or new_msg["attributes"]["oauth2.device.authorization.grant.enabled"] == True
+            ):
                 new_msg["consentRequired"] = True
         # Options for SAML clients
         elif msg["protocol"] == "saml":
             new_msg = json.loads(jsonSamlTemplate)
             new_msg["protocol"] = msg.pop("protocol")
             if "saml_consent" in keycloak_config:
                 new_msg["consentRequired"] = keycloak_config["saml_consent"]
             else:
                 new_msg["consentRequired"] = True
             if "metadata_url" in msg:
                 new_msg["attributes"]["saml.metadata.url"] = msg.pop("metadata_url")
             if "entity_id" in msg:
                 new_msg["clientId"] = msg.pop("entity_id")
             if "requested_attributes" in msg:
-                client_default_client_scopes, new_msg["protocolMappers"] = add_saml_scopes_and_mappers(msg["requested_attributes"])
-                new_msg["defaultClientScopes"] = list(sorted(set(client_default_client_scopes + realm_default_client_scopes)))
+                client_default_client_scopes, new_msg["protocolMappers"] = add_saml_scopes_and_mappers(
+                    msg["requested_attributes"]
+                )
+                new_msg["defaultClientScopes"] = list(
+                    sorted(set(client_default_client_scopes + realm_default_client_scopes))
+                )
     # Options for any type of client
     emails = []
     if "service_name" in msg:
         new_msg["name"] = msg.pop("service_name")
     if "logo_uri" in msg:
         new_msg["attributes"]["logoUri"] = msg.pop("logo_uri")
     if "website_url" in msg:
@@ -179,14 +191,15 @@
 # - the ams agent to handle the operation
 def publish_ams(pub_messages, ams_agent):
     if len(pub_messages) > 0:
         log.info("Publish messaged to ams")
         log.debug("Messages published to ams: " + str(pub_messages))
         ams_agent.publish(pub_messages)
 
+
 # Create the optional client scopes of the client
 def create_client_scopes(agent, client_uuid, client_config):
     realm_client_scopes = agent.sync_realm_client_scopes()
     new_optional_client_scopes = client_config["optionalClientScopes"]
 
     # Custom scopes that are not created in Keycloak
     create_client_scopes = list(set(new_optional_client_scopes) - set(realm_client_scopes.keys()))
@@ -202,14 +215,15 @@
 
     # Get updated client scopes
     realm_client_scopes = agent.sync_realm_client_scopes()
 
     for add_scope in create_client_scopes:
         agent.add_client_scope_by_id(client_uuid, realm_client_scopes[add_scope])
 
+
 # Update the client scopes of the client
 def update_client_scopes(agent, client_uuid, new_client_config, current_client_config):
     protocol = current_client_config["protocol"]
     if protocol == "saml":
         key = "defaultClientScopes"
     else:
         key = "optionalClientScopes"
@@ -238,30 +252,31 @@
 
     for remove_scope in remove_client_scopes:
         agent.remove_client_scope_by_id(client_uuid, realm_client_scopes[remove_scope], protocol)
 
     for add_scope in add_client_scopes:
         agent.add_client_scope_by_id(client_uuid, realm_client_scopes[add_scope], protocol)
 
+
 def add_saml_scopes_and_mappers(requested_attributes):
     scopes = []
     mappers = []
     for attribute in requested_attributes:
         scopes.append(attribute["friendly_name"])
         if attribute["type"] == "custom":
             mapper_object = {
                 "name": attribute["friendly_name"],
                 "protocol": "saml",
                 "protocolMapper": "saml-user-attribute-mapper",
                 "config": {
                     "attribute.nameformat": "URI Reference",
                     "user.attribute": attribute["friendly_name"],
                     "friendly.name": attribute["friendly_name"],
-                    "attribute.name": attribute["name"]
-                }
+                    "attribute.name": attribute["name"],
+                },
             }
             mappers.append(mapper_object)
     return scopes, mappers
 
 
 # Update the optional client scopes of the client
 def update_service_account(agent, client_uuid, current_client_config, keycloak_config):
@@ -360,22 +375,22 @@
     while True:
         log.info("Pull messages from ams")
         messages, ids = ams.pull(1)
         log.info("Received " + str(len(messages)) + " messages from ams")
         if len(messages) > 0:
             log.info("Get access token from " + config["keycloak"]["auth_server"])
             if "refresh_token" in config["keycloak"]:
-                access_token = refreshTokenGrant(
+                access_token = refresh_token_grant(
                     get_keycloak_issuer(config["keycloak"]),
                     config["keycloak"]["refresh_token"],
                     config["keycloak"]["client_id"],
                     config["keycloak"]["client_secret"],
                 )
             else:
-                access_token = clientCredentialsGrant(
+                access_token = client_credentials_grant(
                     get_keycloak_issuer(config["keycloak"]),
                     config["keycloak"]["client_id"],
                     config["keycloak"]["client_secret"],
                 )
             ams.ack(ids)
             responses = process_data(messages, access_token, config["keycloak"])
             publish_ams(responses, ams)
```

### Comparing `rciam-federation-registry-agent-3.0.1/bin/deployer_mitreid` & `rciam-federation-registry-agent-3.2.0/bin/deployer_mitreid`

 * *Files 25% similar despite different names*

```diff
@@ -1,163 +1,178 @@
 #!/usr/bin/env python3
 
-import json, time
 import argparse
+import json
 import logging
+import time
 from datetime import datetime
-from Utils.common import get_log_conf, create_ams_response
-from ServiceRegistryAms.PullPublish import PullPublish
+
 from MitreidConnect.MitreidClientApi import mitreidClientApi
-from Utils.oauth import refreshTokenGrant
+from ServiceRegistryAms.PullPublish import PullPublish
+from Utils.common import create_ams_response, get_log_conf
+from Utils.oauth import refresh_token_grant
 
 # Setup logger
 log = logging.getLogger(__name__)
 
+
 def map_token_endpoint_value(key):
-    if key == 'client_secret_post':
-        return 'SECRET_POST'
-    elif key == 'client_secret_basic':
-        return 'SECRET_BASIC'
-    elif key == 'client_secret_jwt':
-        return 'SECRET_JWT'
-    elif key == 'private_key_jwt':
-        return 'PRIVATE_KEY'
-    elif key == 'none':
-        return 'NONE'
+    if key == "client_secret_post":
+        return "SECRET_POST"
+    elif key == "client_secret_basic":
+        return "SECRET_BASIC"
+    elif key == "client_secret_jwt":
+        return "SECRET_JWT"
+    elif key == "private_key_jwt":
+        return "PRIVATE_KEY"
+    elif key == "none":
+        return "NONE"
+
 
 # format_mitreid_msg gets a message from ams rciam-federation in snake_case
 # and modifies it to camelCase format to be acceptable from mitreID API
 def format_mitreid_msg(msg, deployment_type):
     msgNew = {}
-    emails=[]
+    emails = []
     for key in msg.keys():
-        components = key.split('_')
-        new_key = components[0] + ''.join(x.title() for x in components[1:])
+        components = key.split("_")
+        new_key = components[0] + "".join(x.title() for x in components[1:])
         msgNew[new_key] = msg[key]
-    for contact in msg['contacts']:
-        if ( contact['type'] == 'technical' or contact['type'] == 'support' ):
-            emails.append(contact['email'])
-    msgNew['contacts'] = emails
-    if 'serviceName' in msgNew:
-        msgNew['clientName'] = msgNew.pop('serviceName')
-    if 'serviceDescription' in msgNew:
-        msgNew['clientDescription'] = msgNew.pop('serviceDescription')
-    if 'idTokenTimeoutSeconds' in msgNew:
-        msgNew['idTokenValiditySeconds'] = msgNew.pop('idTokenTimeoutSeconds')
-    if 'externalId' in msgNew:
-        msgNew.pop('externalId')
-    if 'createdAt' in msgNew:
-        if deployment_type == 'create':
-            msgNew.pop('createdAt')
-        elif deployment_type == 'edit':
+    for contact in msg["contacts"]:
+        if contact["type"] == "technical" or contact["type"] == "support":
+            emails.append(contact["email"])
+    msgNew["contacts"] = emails
+    if "serviceName" in msgNew:
+        msgNew["clientName"] = msgNew.pop("serviceName")
+    if "serviceDescription" in msgNew:
+        msgNew["clientDescription"] = msgNew.pop("serviceDescription")
+    if "idTokenTimeoutSeconds" in msgNew:
+        msgNew["idTokenValiditySeconds"] = msgNew.pop("idTokenTimeoutSeconds")
+    if "externalId" in msgNew:
+        msgNew.pop("externalId")
+    if "createdAt" in msgNew:
+        if deployment_type == "create":
+            msgNew.pop("createdAt")
+        elif deployment_type == "edit":
             try:
-                d = datetime.strptime(msgNew['createdAt'][:19],"%Y-%m-%dT%H:%M:%S")
-                msgNew['createdAt'] = d.strftime("%Y-%m-%dT%H:%M:%S+0000")
+                d = datetime.strptime(msgNew["createdAt"][:19], "%Y-%m-%dT%H:%M:%S")
+                msgNew["createdAt"] = d.strftime("%Y-%m-%dT%H:%M:%S+0000")
             except ValueError as err:
                 log.critical(err)
-    if 'tokenEndpointAuthMethod' in msgNew:
-        msgNew['tokenEndpointAuthMethod'] = map_token_endpoint_value(msgNew['tokenEndpointAuthMethod'])
-    if 'aupUri' in msgNew:
-        msgNew['tosUri'] = msgNew.pop('aupUri')
-    if 'websiteUrl' in msgNew:
-        msgNew['clientUri'] = msgNew.pop('websiteUrl')
+    if "tokenEndpointAuthMethod" in msgNew:
+        msgNew["tokenEndpointAuthMethod"] = map_token_endpoint_value(msgNew["tokenEndpointAuthMethod"])
+    if "aupUri" in msgNew:
+        msgNew["tosUri"] = msgNew.pop("aupUri")
+    if "websiteUrl" in msgNew:
+        msgNew["clientUri"] = msgNew.pop("websiteUrl")
     return msgNew
 
 
 # This function will gain an access token from the provided issuer and it will
 # make a POST request using mitreidClient to update or create the client
 #    Function update_data gets 3 arguments:
 #    - messages, the new incoming messages in json
 #    - issuer_url, the url of the issuer
 #    - access_token
 #    - deployer_name
 def update_data(messages, issuer_url, access_token, deployer_name):
-    pub_messages = [] # messages to be published
-    mitreid_agent = mitreidClientApi(issuer_url, access_token) # Create mitreid agent
+    pub_messages = []  # messages to be published
+    mitreid_agent = mitreidClientApi(issuer_url, access_token)  # Create mitreid agent
     for msg in messages:
-        log.debug('Message from ams: ' + str(msg))
-        service_id = msg.pop('id')    # Remove rciam service id to make request to mitreId
+        log.debug("Message from ams: " + str(msg))
+        service_id = msg.pop("id")  # Remove rciam service id to make request to mitreId
         external_id = ""
-        client_id = ''
+        client_id = ""
         try:
             response, external_id, client_id = call_mitreid(msg, mitreid_agent)
-            log.info('Message received from mitreId: ' + str(response))
+            log.info("Message received from mitreId: " + str(response))
             ams_message = create_ams_response(response, service_id, deployer_name, external_id, client_id)
         except:
-            log.critical('Exception catch, return error to ams')
-            ams_message = create_ams_response({'status': 0,'error': 'An error occurred while calling mitreId'}, service_id, deployer_name, external_id, client_id)
-        pub_messages.append({'attributes':{},'data':ams_message})
+            log.critical("Exception catch, return error to ams")
+            ams_message = create_ams_response(
+                {"status": 0, "error": "An error occurred while calling mitreId"},
+                service_id,
+                deployer_name,
+                external_id,
+                client_id,
+            )
+        pub_messages.append({"attributes": {}, "data": ams_message})
     return pub_messages
 
 
 # Publish message to ams upstream topic. Get as arguments
 # - the messages to be published
 # - the ams agent to handle the operation
 def publish_ams(pub_messages, ams_agent):
-    if len(pub_messages)>0:
-        log.info('Publish messaged to ams')
-        log.debug('Messages published to ams: ' + str(pub_messages))
+    if len(pub_messages) > 0:
+        log.info("Publish messaged to ams")
+        log.debug("Messages published to ams: " + str(pub_messages))
         ams_agent.publish(pub_messages)
 
 
 # Calls mitreid depending on the deployment type provided.
 # Operations handled:
 # - create
 # - delete
 # - edit
-def call_mitreid(registry_message,mitreid_agent):
-    deployment_type = registry_message.pop('deployment_type')
+def call_mitreid(registry_message, mitreid_agent):
+    deployment_type = registry_message.pop("deployment_type")
     mitreid_msg = format_mitreid_msg(registry_message, deployment_type)
-    log.debug('Formated message for mitreId: ' + str(mitreid_msg))
+    log.debug("Formatted message for mitreId: " + str(mitreid_msg))
     response = {}
     external_id = ""
-    client_id = ''
-    if deployment_type == 'create':
-        log.info('Create new client')
+    client_id = ""
+    if deployment_type == "create":
+        log.info("Create new client")
         response = mitreid_agent.createClient(mitreid_msg)
-        if (response['status']==200):
-            external_id = str(response['response']['id'])
-            client_id = response['response']['clientId']
-    elif deployment_type == 'delete':
-        external_id = str(registry_message['external_id'])
-        log.info('Delete client with id: ' + str(external_id))
-        response = mitreid_agent.deleteClientById(registry_message['external_id'])
-    elif deployment_type == 'edit':
-        external_id = str(registry_message['external_id'])
-        log.info('Update client with id: ' + str(external_id))
-        response = mitreid_agent.updateClientById(registry_message['external_id'], mitreid_msg)
-        if (response['status']==200):
-            client_id = response['response']['clientId']
+        if response["status"] == 200:
+            external_id = str(response["response"]["id"])
+            client_id = response["response"]["clientId"]
+    elif deployment_type == "delete":
+        external_id = str(registry_message["external_id"])
+        log.info("Delete client with id: " + str(external_id))
+        response = mitreid_agent.deleteClientById(registry_message["external_id"])
+    elif deployment_type == "edit":
+        external_id = str(registry_message["external_id"])
+        log.info("Update client with id: " + str(external_id))
+        response = mitreid_agent.updateClientById(registry_message["external_id"], mitreid_msg)
+        if response["status"] == 200:
+            client_id = response["response"]["clientId"]
     return response, external_id, client_id
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # Get config path from arguments
     parser = argparse.ArgumentParser()
-    parser.add_argument('-c', required=True, type=str, help="Configuration file location path")
+    parser.add_argument("-c", required=True, type=str, help="Configuration file location path")
     args = parser.parse_args()
     path = args.c
     with open(path) as json_data_file:
         config = json.load(json_data_file)
 
     # Get log_conf from project arguments else use the global setting
-    if 'log_conf' in config['mitreid']:
-        get_log_conf(config['mitreid']['log_conf'])
+    if "log_conf" in config["mitreid"]:
+        get_log_conf(config["mitreid"]["log_conf"])
     else:
-        get_log_conf(config['log_conf'])
+        get_log_conf(config["log_conf"])
+
+    log.info("Init ams agent")
+    ams = PullPublish(config["mitreid"]["ams"])
 
-    log.info('Init ams agent')
-    ams = PullPublish(config['mitreid']['ams'])
-    
     # Get messages
     while True:
-        log.info('Pull messages from ams')
+        log.info("Pull messages from ams")
         messages, ids = ams.pull(1)
-        log.info('Received ' + str(len(messages)) +' messages from ams')
+        log.info("Received " + str(len(messages)) + " messages from ams")
         if len(messages) > 0:
-            log.info('Get access token from ' + config['mitreid']['issuer'])
-            access_token = refreshTokenGrant(config['mitreid']['issuer'], config['mitreid']['refresh_token'], config['mitreid']['client_id'], config['mitreid']['client_secret'])
+            log.info("Get access token from " + config["mitreid"]["issuer"])
+            access_token = refresh_token_grant(
+                config["mitreid"]["issuer"],
+                config["mitreid"]["refresh_token"],
+                config["mitreid"]["client_id"],
+                config["mitreid"]["client_secret"],
+            )
             ams.ack(ids)
-            responses = update_data(messages, config['mitreid']['issuer'], access_token, "")
-            publish_ams(responses,ams)
-        time.sleep(config['mitreid']['ams']['poll_interval'])
-    log.info('Exit script')
+            responses = update_data(messages, config["mitreid"]["issuer"], access_token, "")
+            publish_ams(responses, ams)
+        time.sleep(config["mitreid"]["ams"]["poll_interval"])
+    log.info("Exit script")
```

### Comparing `rciam-federation-registry-agent-3.0.1/bin/deployer_ssp` & `rciam-federation-registry-agent-3.2.0/bin/deployer_ssp`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 #!/usr/bin/env python3
 
-import json, time
-import subprocess
 import argparse
-import requests
+import json
 import logging
-from Utils.common import get_log_conf, create_ams_response
+import subprocess
+import time
+
+import requests
+
 from ServiceRegistryAms.PullPublish import PullPublish
+from Utils.common import create_ams_response, get_log_conf
 
 log = logging.getLogger(__name__)
 
 """
 This function will return the altered current state and new additions to it
     Function update_data gets 2 arguments:
     - services, current state included in the php metadata file in json
```

### Comparing `rciam-federation-registry-agent-3.0.1/rciam_federation_registry_agent.egg-info/PKG-INFO` & `rciam-federation-registry-agent-3.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: rciam-federation-registry-agent
-Version: 3.0.1
-Summary: A library that connects to ams using argo-ams-library and syncs with MITREid, SimpleSAMLphp and Keycloak
-Home-page: https://github.com/rciam/rciam-federation-registry-agent
-Author: grnet
-Author-email: faai@grnet.gr
-License: ASL 2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: PHP
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # rciam-federation-registry-agent
 
 **RCIAM Federation Registry Agent** main objective is to sync data between RCIAM Federation Registry and
 different identity and access management solutions, such as Keycloak, SATOSA, SimpleSAMLphp and MITREid Connect.
 This python library includes a module named `ServiceRegistryAms/` to pull and publish messages from ARGO Messaging
 Service using the argo-ams-library, an API module named `MitreidConnect/` to communicate with the API of the MITREid, an
 API module named `Keycloak/` to communicate with the API of the Keycloak.
@@ -146,37 +129,37 @@
   ams.publish(args)
 ```
 
 ### Keycloak
 
 Use Keycloak as an API manager to communicate with Keycloak
 
-- First obtain an access token and create the Keycloak API Client (find clientCredentialsGrant under `Utils` directory)
+- First obtain an access token and create the Keycloak API Client (find client_credentials_grant under `Utils` directory)
 
 ```python
-  access_token = clientCredentialsGrant(issuer_url, client_id, client_secret)
+  access_token = client_credentials_grant(issuer_url, client_id, client_secret)
   keycloak_agent = KeycloakClientApi(issuer_url, access_token)
 ```
 
-- Use the following functions to create, delete and update a service on clientCredentialsGrant
+- Use the following functions to create, delete and update a service on client_credentials_grant
 
 ```python
   response = keycloak_agent.create_client(keycloak_msg)
   response = keycloak_agent.update_client(external_id, keycloak_msg)
   response = keycloak_agent.delete_client(external_id)
 ```
 
 ### MITREid Connect
 
 Use MITREid Connect as an API manager to communicate with MITREid
 
-- First obtain an access token and create the MITREid API Client (find refreshTokenGrant under `Utils` directory)
+- First obtain an access token and create the MITREid API Client (find refresh_token_grant under `Utils` directory)
 
 ```python
-  access_token = refreshTokenGrant(issuer_url, refresh_token, client_id, client_secret)
+  access_token = refresh_token_grant(issuer_url, refresh_token, client_id, client_secret)
   mitreid_agent = mitreidClientApi(issuer_url, access_token)
 ```
 
 - Use the following functions to create, delete and update a service on MITREid
 
 ```python
   response = mitreid_agent.createClient(mitreid_msg)
```

### Comparing `rciam-federation-registry-agent-3.0.1/rciam_federation_registry_agent.egg-info/SOURCES.txt` & `rciam-federation-registry-agent-3.2.0/rciam_federation_registry_agent.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 Keycloak/KeycloakClientApi.py
 Keycloak/__init__.py
 MitreidConnect/MitreidClientApi.py
 MitreidConnect/__init__.py
 ServiceRegistryAms/PullPublish.py
```

### Comparing `rciam-federation-registry-agent-3.0.1/tests/test_deployer_keycloak.py` & `rciam-federation-registry-agent-3.2.0/tests/test_deployer_keycloak.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
-import unittest
-import types
-import os
 import importlib.machinery
-from unittest.mock import MagicMock, Mock
+import os
+import types
+import unittest
+from unittest.mock import MagicMock
 
 
 def get_resource_path(relative_path):
     return os.path.join(os.path.dirname(__file__), relative_path)
 
 
 # load standalone script as module
@@ -17,15 +17,14 @@
 loader.exec_module(deployer_keycloak_oidc)
 
 deployer_keycloak_saml = types.ModuleType(loader.name)
 loader.exec_module(deployer_keycloak_saml)
 
 
 class TestDeployerKeycloak(unittest.TestCase):
-
     # Test the format is compatible with Keycloak
     def test_oidc_format_keycloak_msg(self):
         new_service = {
             "client_id": "testOidcId",
             "service_name": "testName",
             "service_description": "testDescription",
             "protocol": "oidc",
@@ -94,18 +93,14 @@
                     "revoke.refresh.token": "false",
                     "use.jwks.string": "false",
                     "use.jwks.url": "false",
                     "use.refresh.tokens": "false",
                 },
                 "consentRequired": False,
                 "optionalClientScopes": ["profile", "email"],
-                "implicitFlowEnabled": "false",
-                "publicClient": "false",
-                "serviceAccountsEnabled": "false",
-                "standardFlowEnabled": "false",
                 "clientId": "testOidcId",
                 "defaultClientScopes": ["example"],
                 "description": "testDescription",
                 "id": "a1a2a3a4-b5b6-c7c8-d9d0-testOidcId",
                 "protocol": "openid-connect",
                 "implicitFlowEnabled": False,
                 "name": "testName",
@@ -180,18 +175,14 @@
                     "oauth2.token.exchange.grant.enabled": False,
                     "oidc.ciba.grant.enabled": "false",
                     "use.jwks.string": "false",
                     "use.jwks.url": "false",
                     "use.refresh.tokens": "false",
                 },
                 "consentRequired": False,
-                "implicitFlowEnabled": "false",
-                "publicClient": "false",
-                "serviceAccountsEnabled": "false",
-                "standardFlowEnabled": "false",
                 "clientId": "testOidcId",
                 "description": "testDescription",
                 "id": "a1a2a3a4-b5b6-c7c8-d9d0-testOidcId",
                 "protocol": "openid-connect",
                 "implicitFlowEnabled": False,
                 "name": "testName",
                 "defaultClientScopes": ["example"],
@@ -415,15 +406,17 @@
                         "protocolMapper": "saml-user-attribute-mapper",
                         "consentRequired": False,
                     },
                 ],
             },
             "status": 201,
         }
-        realm_default_client_scopes = [{"id": "a1a2a3a4-b5b6-c7c8-d9d0-testScope4", "name": "example", "protocol": "saml"}]
+        realm_default_client_scopes = [
+            {"id": "a1a2a3a4-b5b6-c7c8-d9d0-testScope4", "name": "example", "protocol": "saml"}
+        ]
 
         mock = MagicMock()
         mock.create_client = MagicMock(return_value=out_service)
         mock.get_client_by_id = MagicMock(return_value=out_service)
         mock.get_realm_default_client_scopes = MagicMock(return_value=realm_default_client_scopes)
 
         func_result = deployer_keycloak_saml.deploy_to_keycloak(new_service, mock, "config")
@@ -539,15 +532,17 @@
                         "protocolMapper": "saml-user-attribute-mapper",
                         "consentRequired": False,
                     },
                 ],
             },
             "status": 201,
         }
-        realm_default_client_scopes = [{"id": "a1a2a3a4-b5b6-c7c8-d9d0-testScope8", "name": "example", "protocol": "saml"}]
+        realm_default_client_scopes = [
+            {"id": "a1a2a3a4-b5b6-c7c8-d9d0-testScope8", "name": "example", "protocol": "saml"}
+        ]
 
         mock = MagicMock()
         mock.update_client = MagicMock(return_value=out_service)
         mock.get_realm_default_client_scopes = MagicMock(return_value=realm_default_client_scopes)
 
         func_result = deployer_keycloak_saml.deploy_to_keycloak(new_service, mock, "config")
         self.assertEqual(
```

### Comparing `rciam-federation-registry-agent-3.0.1/tests/test_deployer_ssp.py` & `rciam-federation-registry-agent-3.2.0/tests/test_deployer_ssp.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,120 +1,175 @@
 #!/usr/bin/env python3
 
-import json
-import unittest
-import types
-import os
-import importlib.machinery
 import filecmp
-import requests
+import importlib.machinery
+import os
 import subprocess
+import types
+import unittest
 from unittest.mock import MagicMock, Mock
 
+import requests
+
+
 def get_resource_path(relative_path):
     return os.path.join(os.path.dirname(__file__), relative_path)
 
+
 # load standalone script as module
-loader = importlib.machinery.SourceFileLoader('deployer_ssp', get_resource_path('../bin/deployer_ssp'))
+loader = importlib.machinery.SourceFileLoader("deployer_ssp", get_resource_path("../bin/deployer_ssp"))
 deployer_ssp = types.ModuleType(loader.name)
 loader.exec_module(deployer_ssp)
 
-class TestDeployerSsp(unittest.TestCase):
 
+class TestDeployerSsp(unittest.TestCase):
     # Test that a creation adds a new enty in the data array
     def test_update_data_create(self):
         services = [{"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"}]
-        new_service = [{"id": "testId2", "entity_id": "testEntityId2", "deployment_type": "create", "metadata_url": "TestMetadataUrl2"}]
-        test_case_result = [{"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"}, \
-            {"registry_service_id": "testId2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrl2"}]
+        new_service = [
+            {
+                "id": "testId2",
+                "entity_id": "testEntityId2",
+                "deployment_type": "create",
+                "metadata_url": "TestMetadataUrl2",
+            }
+        ]
+        test_case_result = [
+            {"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"},
+            {"registry_service_id": "testId2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrl2"},
+        ]
 
         func_result = deployer_ssp.update_data(services, new_service)
         self.assertEqual(func_result, test_case_result)
 
     # Test that a creation of an existing enty do not alter the data array
     def test_update_data_double_create(self):
         services = [{"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"}]
-        new_service = [{"id": "testId2", "entity_id": "testEntityId2", "deployment_type": "create", "metadata_url": "TestMetadataUrl2"}]
-        test_case_result = [{"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"}, \
-            {"registry_service_id": "testId2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrl2"}]
+        new_service = [
+            {
+                "id": "testId2",
+                "entity_id": "testEntityId2",
+                "deployment_type": "create",
+                "metadata_url": "TestMetadataUrl2",
+            }
+        ]
+        test_case_result = [
+            {"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"},
+            {"registry_service_id": "testId2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrl2"},
+        ]
 
         func_result = deployer_ssp.update_data(services, new_service)
         func_result = deployer_ssp.update_data(func_result, new_service)
         self.assertEqual(func_result, test_case_result)
 
     # Test that an edit to an entry alters the data array
     def test_update_data_update(self):
-        services = [{"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"}, \
-            {"registry_service_id": "testId2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrl2"}]
-        update_service = [{"id": "testId2", "entity_id": "testEntityId2", "deployment_type": "edit", "metadata_url": "TestMetadataUrlEDIT"}]
-        test_case_result = [{"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"}, \
-            {"registry_service_id": "testId2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrlEDIT"}]
+        services = [
+            {"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"},
+            {"registry_service_id": "testId2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrl2"},
+        ]
+        update_service = [
+            {
+                "id": "testId2",
+                "entity_id": "testEntityId2",
+                "deployment_type": "edit",
+                "metadata_url": "TestMetadataUrlEDIT",
+            }
+        ]
+        test_case_result = [
+            {"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"},
+            {"registry_service_id": "testId2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrlEDIT"},
+        ]
 
         func_result = deployer_ssp.update_data(services, update_service)
         self.assertEqual(func_result, test_case_result)
 
     # Test that a deletion removes the entry from the data array
     def test_update_data_delete(self):
-        services = [{"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"}, \
-            {"registry_service_id": "testId2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrl2"}]
-        delete_service = [{"id": "testId2", "entity_id": "testEntityId2", "deployment_type": "delete", "metadata_url": "TestMetadataUrl2"}]
-        test_case_result = [{"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"}]
+        services = [
+            {"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"},
+            {"registry_service_id": "testId2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrl2"},
+        ]
+        delete_service = [
+            {
+                "id": "testId2",
+                "entity_id": "testEntityId2",
+                "deployment_type": "delete",
+                "metadata_url": "TestMetadataUrl2",
+            }
+        ]
+        test_case_result = [
+            {"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"}
+        ]
 
         func_result = deployer_ssp.update_data(services, delete_service)
         self.assertEqual(func_result, test_case_result)
 
     # Test that a deletion of a non existing entry does not alters the data array
     def test_update_data_double_delete(self):
-        services = [{"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"}, \
-            {"registry_service_id": "testId2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrl2"}]
-        delete_service = [{"id": "testId2", "entity_id": "testEntityId2", "deployment_type": "delete", "metadata_url": "TestMetadataUrl2"}]
-        test_case_result = [{"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"}]
+        services = [
+            {"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"},
+            {"registry_service_id": "testId2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrl2"},
+        ]
+        delete_service = [
+            {
+                "id": "testId2",
+                "entity_id": "testEntityId2",
+                "deployment_type": "delete",
+                "metadata_url": "TestMetadataUrl2",
+            }
+        ]
+        test_case_result = [
+            {"registry_service_id": "testId1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"}
+        ]
 
         func_result = deployer_ssp.update_data(services, delete_service)
         func_result = deployer_ssp.update_data(func_result, delete_service)
         self.assertEqual(func_result, test_case_result)
 
     # Verify the generated php config
     def test_generate_config(self):
-        services = [{"registry_service_id": "1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"}, \
-            {"registry_service_id": "2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrl2"}]
-        deployer_ssp.generate_config(services,'./test_file.php') 
-        self.assertTrue(filecmp.cmp('./test_file.php',get_resource_path('./files/ssp_config.php')), 'Files differ')
+        services = [
+            {"registry_service_id": "1", "whitelist": ["testEntityId1"], "src": "TestMetadataUrl1"},
+            {"registry_service_id": "2", "whitelist": ["testEntityId2"], "src": "TestMetadataUrl2"},
+        ]
+        deployer_ssp.generate_config(services, "./test_file.php")
+        self.assertTrue(filecmp.cmp("./test_file.php", get_resource_path("./files/ssp_config.php")), "Files differ")
 
     # Call ssp syncer with 200 http response
     def test_call_ssp_syncer_positive(self):
         mock = Mock()
         mock.status_code = 200
         mock.return_value.raise_for_status = None
-        mock.json = MagicMock(return_value='')
+        mock.json = MagicMock(return_value="")
         mock_req = requests
         mock_req.get = MagicMock(return_value=mock)
-        func_result = deployer_ssp.call_ssp_syncer('test_url', 'key', 60, 'hourly')
-        self.assertEqual(func_result['status'],200)
+        func_result = deployer_ssp.call_ssp_syncer("test_url", "key", 60, "hourly")
+        self.assertEqual(func_result["status"], 200)
 
     # Call ssp syncer with 400 http response
     def test_call_ssp_syncer_negative(self):
         mock = Mock()
         mock.status_code = 400
-        mock.return_value.raise_for_status = Exception('ERROR')
-        mock.json = MagicMock(return_value='ERROR')
+        mock.return_value.raise_for_status = Exception("ERROR")
+        mock.json = MagicMock(return_value="ERROR")
         mock_req = requests
         mock_req.get = MagicMock(return_value=mock)
-        func_result = deployer_ssp.call_ssp_syncer('test_url', 'key', 60, 'hourly')
-        self.assertEqual(func_result['status'],400)
+        func_result = deployer_ssp.call_ssp_syncer("test_url", "key", 60, "hourly")
+        self.assertEqual(func_result["status"], 400)
 
     # Test reading from php configuration file
     def test_get_services_from_conf(self):
         mock_sub = subprocess
         ret = subprocess.CompletedProcess
         ret.stdout = '[{"id":11}]'
         mock_sub.run = MagicMock(return_value=ret)
-        self.assertEqual(deployer_ssp.get_services_from_conf(''),[{"id":11}])
-    
+        self.assertEqual(deployer_ssp.get_services_from_conf(""), [{"id": 11}])
+
     # Test reading from php configuration file with return value that is not list
     def test_get_services_from_conf_fail(self):
         mock_sub = subprocess
         ret = subprocess.CompletedProcess
         ret.stdout = '{"id":11}'
         mock_sub.run = MagicMock(return_value=ret)
         with self.assertRaises(SystemExit):
-            deployer_ssp.get_services_from_conf('')
+            deployer_ssp.get_services_from_conf("")
```

