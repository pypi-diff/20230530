# Comparing `tmp/sumatra-client-1.2.0.tar.gz` & `tmp/sumatra-client-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumatra-client-1.2.0.tar", last modified: Fri Apr 21 20:39:45 2023, max compression
+gzip compressed data, was "sumatra-client-1.3.0rc1.tar", last modified: Tue May 30 20:07:54 2023, max compression
```

## Comparing `sumatra-client-1.2.0.tar` & `sumatra-client-1.3.0rc1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-04-21 20:39:45.732391 sumatra-client-1.2.0/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      167 2021-12-08 03:47:40.000000 sumatra-client-1.2.0/LICENSE
--rw-r--r--   0 kuhlmann   (501) staff       (20)      542 2023-04-21 20:39:45.732576 sumatra-client-1.2.0/PKG-INFO
--rw-r--r--   0 kuhlmann   (501) staff       (20)       93 2022-02-04 23:04:56.000000 sumatra-client-1.2.0/README.md
--rw-r--r--   0 kuhlmann   (501) staff       (20)       90 2021-12-03 22:49:56.000000 sumatra-client-1.2.0/pyproject.toml
--rw-r--r--   0 kuhlmann   (501) staff       (20)      767 2023-04-21 20:39:45.733482 sumatra-client-1.2.0/setup.cfg
--rw-r--r--   0 kuhlmann   (501) staff       (20)       85 2022-09-23 13:58:44.000000 sumatra-client-1.2.0/setup.py
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-04-21 20:39:45.728530 sumatra-client-1.2.0/sumatra_client/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      178 2023-04-05 19:51:09.000000 sumatra-client-1.2.0/sumatra_client/__init__.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     6859 2023-04-21 20:08:04.000000 sumatra-client-1.2.0/sumatra_client/auth.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)    21519 2023-04-21 20:08:04.000000 sumatra-client-1.2.0/sumatra_client/cli.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)    98466 2023-04-21 20:08:04.000000 sumatra-client-1.2.0/sumatra_client/client.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     8211 2023-04-05 19:51:09.000000 sumatra-client-1.2.0/sumatra_client/config.py
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-04-21 20:39:45.731471 sumatra-client-1.2.0/sumatra_client.egg-info/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      542 2023-04-21 20:39:45.000000 sumatra-client-1.2.0/sumatra_client.egg-info/PKG-INFO
--rw-r--r--   0 kuhlmann   (501) staff       (20)      461 2023-04-21 20:39:45.000000 sumatra-client-1.2.0/sumatra_client.egg-info/SOURCES.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2023-04-21 20:39:45.000000 sumatra-client-1.2.0/sumatra_client.egg-info/dependency_links.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)       52 2023-04-21 20:39:45.000000 sumatra-client-1.2.0/sumatra_client.egg-info/entry_points.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2021-12-03 22:57:42.000000 sumatra-client-1.2.0/sumatra_client.egg-info/not-zip-safe
--rw-r--r--   0 kuhlmann   (501) staff       (20)       97 2023-04-21 20:39:45.000000 sumatra-client-1.2.0/sumatra_client.egg-info/requires.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)       15 2023-04-21 20:39:45.000000 sumatra-client-1.2.0/sumatra_client.egg-info/top_level.txt
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-04-21 20:39:45.731951 sumatra-client-1.2.0/tests/
--rw-r--r--   0 kuhlmann   (501) staff       (20)     2309 2022-09-23 13:58:44.000000 sumatra-client-1.2.0/tests/test_config.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-05-30 20:07:54.628203 sumatra-client-1.3.0rc1/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      167 2021-12-08 03:47:40.000000 sumatra-client-1.3.0rc1/LICENSE
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      545 2023-05-30 20:07:54.628408 sumatra-client-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       93 2022-02-04 23:04:56.000000 sumatra-client-1.3.0rc1/README.md
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       90 2021-12-03 22:49:56.000000 sumatra-client-1.3.0rc1/pyproject.toml
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      827 2023-05-30 20:07:54.629378 sumatra-client-1.3.0rc1/setup.cfg
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       85 2022-09-23 13:58:44.000000 sumatra-client-1.3.0rc1/setup.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-05-30 20:07:54.623717 sumatra-client-1.3.0rc1/sumatra_client/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      373 2023-05-18 02:01:57.000000 sumatra-client-1.3.0rc1/sumatra_client/__init__.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     5568 2023-05-30 20:01:48.000000 sumatra-client-1.3.0rc1/sumatra_client/admin.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     9665 2023-05-30 20:01:48.000000 sumatra-client-1.3.0rc1/sumatra_client/auth.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)    23855 2023-05-18 02:01:57.000000 sumatra-client-1.3.0rc1/sumatra_client/cli.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)    99304 2023-05-19 19:17:38.000000 sumatra-client-1.3.0rc1/sumatra_client/client.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     8677 2023-05-30 20:01:48.000000 sumatra-client-1.3.0rc1/sumatra_client/config.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     4367 2023-05-18 18:11:52.000000 sumatra-client-1.3.0rc1/sumatra_client/workspace.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-05-30 20:07:54.627339 sumatra-client-1.3.0rc1/sumatra_client.egg-info/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      545 2023-05-30 20:07:54.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/PKG-INFO
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      513 2023-05-30 20:07:54.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/SOURCES.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2023-05-30 20:07:54.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/dependency_links.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       52 2023-05-30 20:07:54.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/entry_points.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2021-12-03 22:57:42.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/not-zip-safe
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       99 2023-05-30 20:07:54.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/requires.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       15 2023-05-30 20:07:54.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/top_level.txt
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-05-30 20:07:54.627780 sumatra-client-1.3.0rc1/tests/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     2309 2022-09-23 13:58:44.000000 sumatra-client-1.3.0rc1/tests/test_config.py
```

### Comparing `sumatra-client-1.2.0/PKG-INFO` & `sumatra-client-1.3.0rc1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumatra-client
-Version: 1.2.0
+Version: 1.3.0rc1
 Summary: Sumatra Python Client and CLI
 Home-page: https://sumatra.ai
 Author: Sumatra
 Author-email: support@sumatra.ai
 License: Sumatra Proprietary
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sumatra-client-1.2.0/setup.cfg` & `sumatra-client-1.3.0rc1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sumatra-client
-version = 1.2.0
+version = 1.3.0rc1
 author = Sumatra
 author_email = support@sumatra.ai
 url = https://sumatra.ai
 description = Sumatra Python Client and CLI
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Sumatra Proprietary
@@ -19,22 +19,25 @@
 zip_safe = False
 python_requires = >= 3.7
 packages = sumatra_client
 install_requires = 
 	awswrangler
 	boto3
 	colorama
-	pandas
+	pandas < 2
 	python_graphql_client
 	pendulum
 	requests
 	click
 	tqdm
 	sumatra-sdk
 
+[options.package_data]
+sumatra_client = certs/*.pem
+
 [options.entry_points]
 console_scripts = 
 	sumatra = sumatra_client.cli:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sumatra-client-1.2.0/sumatra_client/auth.py` & `sumatra-client-1.3.0rc1/sumatra_client/auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 import click
 import requests
 import json
 import time
+import threading
 from logging import getLogger
 
 from configparser import ConfigParser
 from requests.auth import AuthBase
-from urllib.parse import urlencode, urlparse, parse_qs
 from http.server import BaseHTTPRequestHandler, HTTPServer
+import ssl
 
 from sumatra_client.config import CONFIG
 
 logger = getLogger("sumatra.auth")
 
 AUTH_REDIRECT_PORTS = [20005, 20015, 20025]
 
@@ -41,15 +42,16 @@
         return not self == other
 
     def __call__(self, r):
         if not self._jwt_token:
             auth = CognitoAuth()
             self._jwt_token = auth.get_or_refresh_token()
         r.headers["Authorization"] = self._jwt_token
-        r.headers["x-sumatra-tenant"] = self._tenant
+        if "x-sumatra-tenant" not in r.headers:
+            r.headers["x-sumatra-tenant"] = self._tenant
         return r
 
 
 class SDKKeyAuth(AuthBase):
     """x-api-key: SDK_KEY"""
 
     def __init__(self):
@@ -66,38 +68,54 @@
         return r
 
 
 class CallbackServerHandler(BaseHTTPRequestHandler):
     def log_message(self, format, *args):
         logger.debug(format % args)
 
+    def do_OPTIONS(self):
+        self.send_response(204)
+        self.send_header("Access-Control-Allow-Origin", self.server._origin)
+        self.send_header("Access-Control-Allow-Methods", "POST")
+        self.send_header('Access-Control-Allow-Headers', 'Access-Control-Allow-Headers, Origin, Accept, X-Requested-With, Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers')
+        self.end_headers()
+
     def do_POST(self):
         l = int(self.headers.get("Content-Length", 0))
         response_json = json.loads(self.rfile.read(l))
         if "error" in response_json:
             raise RuntimeError(response_json.get("error"))
 
-        self.server.refresh_token = response_json.get("refreshToken")
-        self.server.id_token = response_json.get("idToken")
-        self.server.access_token = response_json.get("accessToken")
+        refresh_token = response_json.get("refreshToken")
+        id_token = response_json.get("idToken")
+        access_token = response_json.get("accessToken")
+        if not (refresh_token and id_token and access_token):
+            logger.debug(f"Invalid request body {json.dumps(response_json)}")
+            raise RuntimeError("Invalid request body from server during authentication")
+        self.server.refresh_token = refresh_token
+        self.server.id_token = id_token
+        self.server.access_token = access_token
         self.server.expires_at = response_json.get("expiration")
 
         self.send_response(200)
+        self.send_header("Access-Control-Allow-Origin", self.server._origin)
         self.end_headers()
         self.wfile.flush()
+        threading.Thread(target=self.server.shutdown, daemon=True).start()
 
 
 class CallbackServer(HTTPServer):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, origin=None, **kwargs):
         # Because HTTPServer is an old-style class, super() can't be used.
         HTTPServer.__init__(self, *args, **kwargs)
         self.refresh_token = None
         self.id_token = None
         self.access_token = None
         self.expires_at = None
+        self._origin = origin
 
 
 class CognitoAuth:
     def __init__(self):
         self._redirect_uri = None
         self._code_verifier = None
         self._response = {}
@@ -120,25 +138,25 @@
         fname = CONFIG.jwt_tokens_path
         logger.info(f"Loading tokens from {fname}")
         tokfile = ConfigParser()
         tokfile.read(fname)
         try:
             tokens = dict(tokfile[CONFIG.instance])
             tokens["expiration"] = int(tokens["expiration"])
-            assert "id" in tokens
+            assert tokens.get("id") and tokens.get("refresh")
             return tokens
         except Exception as e:
             logger
             raise TokenNotFoundException
 
     def _save_tokens(self, tokens: dict) -> None:
         fname = CONFIG.jwt_tokens_path
         logger.info(f"Saving tokens to {fname}")
         tokens = dict(tokens)
-        tokens["expiration"] = str(tokens["expiration"])
+        tokens = {k: str(v) for k, v in tokens.items()}
         tokfile = ConfigParser()
         tokfile.read(fname)
         tokfile[CONFIG.instance] = tokens
         os.makedirs(os.path.dirname(fname), exist_ok=True)
         with open(
             os.open(fname, os.O_CREAT | os.O_WRONLY | os.O_TRUNC, 0o600), "w"
         ) as f:
@@ -161,45 +179,87 @@
         self._save_tokens(new_tokens)
         return new_tokens
 
     # open browser and allow user to authenticate using selected cognito flow
     # and store returned auth code
     def _fetch_authorization_tokens(self):
         logger.info("Launching browser-based authentication.")
+        if CONFIG.server_version.startswith("v1.2"):
+            self._start_callback_listener_compat()
+        else:
+            self._start_callback_listener()
+
         auth_url = self._build_auth_url()
         try:
             click.launch(auth_url)
-            self._httpd.handle_request()
+            self._httpd.serve_forever(poll_interval=1)
+        except:
+            logger.exception("failed to handle request")
         finally:
             self._response = {
                 "refresh_token": self._httpd.refresh_token,
                 "id_token": self._httpd.id_token,
                 "access_token": self._httpd.access_token,
                 "expires_at": self._httpd.expires_at,
             }
             self._httpd.server_close()
+            if not (self._httpd.refresh_token and self._httpd.id_token and self._httpd.access_token):
+                raise RuntimeError("Callback server failed to receive access tokens")
 
     def _build_auth_url(self):
-        self._start_callback_listener()
-
         return f"{CONFIG.instance_url}/log-in-ext/{self._redirect_port}"
 
-    def _start_callback_listener(self):
+    def _start_callback_listener_compat(self):
+        logger.debug("Using 1.2.0 compatible request handler")
         for port in AUTH_REDIRECT_PORTS:
             try:
-                self._httpd = CallbackServer(("", int(port)), CallbackServerHandler)
+                self._httpd = CallbackServer(
+                    ("localhost", int(port)), CallbackServerHandler,
+                    origin=CONFIG.instance_url
+                )
                 self._redirect_uri = f"http://localhost:{port}"
                 self._redirect_port = port
                 break
             except OSError as e:
                 if e.errno == 48:
                     continue
                 else:
                     raise OSError(f"error during authentication: {e}")
         else:
+            raise
+
+    def _start_callback_listener(self):
+        for port in AUTH_REDIRECT_PORTS:
+            try:
+                context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+                certfile = os.path.join(
+                    os.path.dirname(__file__), os.pardir, "certs", "fullchain1.pem"
+                )
+                os.path.pardir
+                keyfile = os.path.join(
+                    os.path.dirname(__file__), os.pardir, "certs", "privkey1.pem"
+                )
+                context.load_cert_chain(certfile, keyfile)
+                self._httpd = CallbackServer(
+                    ("l0.lrd.sumatra.ai", int(port)), CallbackServerHandler,
+                    origin=CONFIG.instance_url
+                )
+                self._redirect_uri = f"http://l0.lrd.sumatra.ai:{port}"
+                self._redirect_port = port
+                self._httpd.socket = context.wrap_socket(
+                    self._httpd.socket,
+                    server_side=True,
+                )
+                break
+            except OSError as e:
+                if e.errno == 48:
+                    continue
+                else:
+                    raise OSError(f"error during authentication: {e}")
+        else:
             raise
 
     def _parse_token_response(self, response):
         now = int(time.time())
         expires_at = response.get("expires_at")
         expiration = now if not expires_at else int(expires_at)
```

### Comparing `sumatra-client-1.2.0/sumatra_client/cli.py` & `sumatra-client-1.3.0rc1/sumatra_client/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import argparse
 import logging
 import requests
 from colorama import Fore, Style
 from sumatra_client.config import CONFIG
 from sumatra_client.auth import CognitoAuth
 from sumatra_client.client import Client
+from sumatra_client.workspace import WorkspaceClient
+from sumatra_client.admin import AdminClient
 
 
 logger = logging.getLogger("sumatra.cli")
 
 
 def _tmp_branch_name() -> str:
     return "tmp_" + str(uuid.uuid4()).replace("-", "")
@@ -108,23 +110,21 @@
 
 
 def config(args) -> None:
     print(CONFIG.summary(args.unmask))
 
 
 def login(args) -> None:
-    instance = args.instance
     try:
-        curr_instance = CONFIG.instance
-    except:
-        curr_instance = "console.sumatra.ai"
-    prompt = f"Sumatra Instance URL [{curr_instance}]: "
-    instance = input(prompt).strip()
-    if not instance:
-        instance = curr_instance
+        instance = args.instance or CONFIG.instance
+    except RuntimeError:
+        instance = "console.sumatra.ai"
+    if not args.instance:
+        prompt = f"Sumatra Instance URL [{instance}]: "
+        instance = input(prompt).strip() or instance
     CONFIG.instance = instance
     try:
         CONFIG.update_from_stack()
     except requests.exceptions.ConnectionError:
         print(f"Unable to connect to {instance}. Please check the URL and try again.")
         sys.exit(1)
 
@@ -264,15 +264,18 @@
 
 def table_delete(args):
     Client().delete_table(args.table)
     print(f"Successfully deleted table '{args.table}'")
 
 
 def table_show(args):
-    print(Client().get_tables().loc[args.table])
+    try:
+        print(Client().get_tables().loc[args.table])
+    except KeyError:
+        raise KeyError(f"Table '{args.table}' not found.")
 
 
 def table_schema(args):
     print(Client().get_table_schema(args.table, args.version))
 
 
 def table_history(args):
@@ -289,15 +292,18 @@
 
 def model_delete(args):
     Client().delete_model(args.model)
     print(f"Successfully deleted model '{args.model}'")
 
 
 def model_show(args):
-    print(Client().get_models().loc[args.model])
+    try:
+        print(Client().get_models().loc[args.model])
+    except KeyError:
+        raise KeyError(f"Model '{args.model}' not found.")
 
 
 def model_history(args):
     print(Client().get_model_history(args.model))
 
 
 def model_schema(args):
@@ -306,84 +312,105 @@
 
 def model_put(args):
     print(
         Client().create_model_from_pmml(args.model, args.filename, comment=args.comment)
     )
 
 
-def version(args):
-    print(Client().version())
-
+def workspace_list(args):
+    workspaces = WorkspaceClient().get_workspaces().sort_index()
+    if args.show:
+        print(workspaces)
+    else:
+        print("\n".join(workspaces.index.to_list()))
 
-def tenant(args):
-    print(Client().tenant())
 
+def workspace_delete(args):
+    WorkspaceClient().delete_workspace(args.workspace)
+    print(f"Successfully deleted workspace '{args.workspace}'")
 
-def admin_list_tenants(args):
-    tenants = Client().list_tenants()
-    print("\n".join(tenants))
 
+def workspace_create(args):
+    WorkspaceClient().create_workspace(args.workspace, args.nickname)
+    print(f"Successfully created workspace '{args.workspace}'")
 
-def admin_current_tenant(args):
-    user = Client().get_user(args.user)
-    print(user["tenant"] + "\t" + user["role"])
 
+def workspace_show(args):
+    try:
+        print(WorkspaceClient().get_workspaces().loc[args.workspace])
+    except KeyError:
+        raise KeyError(f"Workspace '{args.workspace}' not found.")
 
-def admin_assign_tenant(args):
-    Client().set_tenant(args.user, args.tenant)
-    Client().set_role(args.user, args.role)
 
+def workspace_select(args):
+    CONFIG.workspace = args.workspace
+    CONFIG.save(update_default_instance=False)
     print(
-        f"Successfully assigned '{args.user}' to '{args.tenant}' with '{args.role}' role."
+        f"Current workspace in config set to '{args.workspace}' for {CONFIG.instance}\n"
     )
 
 
+def version(args):
+    print(Client().version())
+
+
+def tenant(args):
+    print(Client().tenant())
+
+
+def admin_list_tenants(args):
+    tenants = AdminClient().list_tenants()
+    print("\n".join(tenants))
+
+
 def admin_list_users(args):
-    users = Client().list_users()
+    users = AdminClient().list_users()
     print("\n".join(users))
 
 
-def admin_show_keys(args):
-    print(Client().get_keys())
+def admin_upgrade_tenant(args):
+    AdminClient().upgrade_tenant(args.tenant)
+    print(f"Successfully upgraded tenant '{args.tenant}'")
+
 
+def admin_downgrade_tenant(args):
+    AdminClient().downgrade_tenant(args.tenant)
+    print(f"Successfully downgraded tenant '{args.tenant}'")
 
-def admin_show_key_usage(args):
-    print(Client().get_key_usage())
+
+def admin_set_quota(args):
+    AdminClient().set_quota(args.tenant, args.monthly_events)
+    print(f"Successfully set quota for tenant '{args.tenant}' to {args.monthly_events}")
 
 
 ADMIN_COMMANDS = [
     {
         "name": "list-tenants",
         "help": "list all tenants",
         "handler": admin_list_tenants,
     },
     {
-        "name": "current-tenant",
-        "help": "show user's current tenant",
-        "handler": admin_current_tenant,
-    },
-    {
-        "name": "assign-tenant",
-        "help": "assign user to tenant",
-        "handler": admin_assign_tenant,
-    },
-    {
         "name": "list-users",
         "help": "list all users",
         "handler": admin_list_users,
     },
     {
-        "name": "show-keys",
-        "help": "show api and sdk keys",
-        "handler": admin_show_keys,
+        "name": "upgrade",
+        "help": "upgrade a tenant to premium tier",
+        "handler": admin_upgrade_tenant,
+    },
+    {
+        "name": "downgrade",
+        "help": "downgrade a tenant to free tier",
+        "handler": admin_downgrade_tenant,
     },
     {
-        "name": "show-key-usage",
-        "help": "show api and sdk key daily usage",
-        "handler": admin_show_key_usage,
+        "name": "set-quota",
+        "help": "set tenant monthly event quota",
+        "handler": admin_set_quota,
     },
 ]
 
 TIMELINE_COMMANDS = [
     {
         "name": "list",
         "help": "list all remote timelines",
@@ -509,14 +536,42 @@
     {
         "name": "put",
         "help": "upload a model object",
         "handler": model_put,
     },
 ]
 
+WORKSPACE_COMMANDS = [
+    {
+        "name": "list",
+        "help": "list all workspaces",
+        "handler": workspace_list,
+    },
+    {
+        "name": "delete",
+        "help": "delete workspace",
+        "handler": workspace_delete,
+    },
+    {
+        "name": "create",
+        "help": "create workspace",
+        "handler": workspace_create,
+    },
+    {
+        "name": "show",
+        "help": "display workspace metadata",
+        "handler": workspace_show,
+    },
+    {
+        "name": "select",
+        "help": "set current workspace in local config",
+        "handler": workspace_select,
+    },
+]
+
 COMMANDS = [
     {
         "name": "config",
         "help": "show configuration",
         "handler": config,
     },
     {
@@ -566,14 +621,19 @@
     },
     {
         "name": "timeline",
         "help": "run `sumatra timeline -h` for subcommands",
         "subcommands": TIMELINE_COMMANDS,
     },
     {
+        "name": "workspace",
+        "help": "run `sumatra workspace -h` for subcommands",
+        "subcommands": WORKSPACE_COMMANDS,
+    },
+    {
         "name": "admin",
         "help": "run `sumatra admin -h` for subcommands",
         "subcommands": ADMIN_COMMANDS,
     },
     {"name": "version", "help": "show remote sumatra version", "handler": version},
     {"name": "tenant", "help": "show tenant name", "handler": tenant},
 ]
@@ -695,21 +755,31 @@
                             "--show", action="store_true", help="display metadata"
                         )
                     if subcmd["name"] == "upload":
                         p.add_argument(
                             "file",
                             help="file with event data in JSON Lines format (may be gzipped)",
                         )
+                if cmd["name"] == "workspace":
+                    if subcmd["name"] in ["delete", "show", "select", "create"]:
+                        p.add_argument("workspace", help="workspace name")
+                    if subcmd["name"] == "list":
+                        p.add_argument(
+                            "--show", action="store_true", help="display metadata"
+                        )
+                    if subcmd["name"] == "create":
+                        p.add_argument(
+                            "--nickname", help="specify optional workspace nickname"
+                        )
                 if cmd["name"] == "admin":
-                    if subcmd["name"] in ["current-tenant", "assign-tenant"]:
-                        p.add_argument("user", help="cognito login name of user")
-                    if subcmd["name"] == "assign-tenant":
+                    if subcmd["name"] in ["upgrade", "downgrade", "set-quota"]:
                         p.add_argument("tenant", help="tenant name")
+                    if subcmd["name"] == "set-quota":
                         p.add_argument(
-                            "role", help="role name (reader, writer, publisher)"
+                            "monthly_events", help="monthly event quota", type=int
                         )
 
     args = parser.parse_args()
 
     log_level = logging.WARNING
     if args.verbose:
         log_level = logging.INFO
```

### Comparing `sumatra-client-1.2.0/sumatra_client/client.py` & `sumatra-client-1.3.0rc1/sumatra_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 import awswrangler as wr
 import boto3
 import gzip
 import pendulum
 import python_graphql_client
 import pandas as pd
 import requests
+import base64
 from time import sleep
 from datetime import datetime
-from typing import Any, Optional, Dict, List, Union
+from typing import Any, Optional, Dict, List, Union, Tuple
 from tqdm.auto import tqdm
 from requests.auth import AuthBase
 from sumatra_client.auth import SDKKeyAuth, CognitoJwtAuth
 from sumatra_client.config import CONFIG
-
+from sumatra_client.workspace import WorkspaceClient
 
 logger = logging.getLogger("sumatra.client")
 
 TENANT_PREFIX = "sumatra_"
 DEPS_FILE = "deps.scowl"
 TABLE_NAME_REGEXP = re.compile("^[a-z][a-zA-Z0-9_]*$")
 
@@ -107,95 +108,280 @@
     __Bots:__ Set the `SUMATRA_INSTANCE` and `SUMATRA_SDK_KEY` environment variables
     """
 
     def __init__(
         self,
         instance: Optional[str] = None,
         branch: Optional[str] = None,
-        workspace: str = "_default",
+        workspace: Optional[str] = None,
     ):
         """
         Create connection object.
 
         Arguments:
             instance: Sumatra instance url, e.g. `yourco.sumatra.ai`. If unspecified, the your config default will be used.
             branch: Set default branch. If unspecified, your config default will be used.
-            workspace: Sumatra workspace name to connect to. Required if not using an SDK key
+            workspace: Sumatra workspace name to connect to.
         """
         if instance:
             CONFIG.instance = instance
+        self._branch = branch or CONFIG.default_branch
+        self._workspace_arg = workspace or CONFIG.workspace
+        self._workspace = None
+        self._workspace_id = None
         if CONFIG.sdk_key:
+            logger.info("Connecting via SDK key")
             auth: AuthBase = SDKKeyAuth()
             endpoint = CONFIG.sdk_graphql_url
         else:
-            if not workspace:
-                raise ValueError("workspace argument required when not using an SDK key")
-            auth = CognitoJwtAuth(workspace)
+            auth = CognitoJwtAuth(self.workspace)
             endpoint = CONFIG.console_graphql_url
-
-        self._branch = branch or CONFIG.default_branch
-
         self._gql_client = python_graphql_client.GraphqlClient(
             auth=auth, endpoint=endpoint
         )
 
+    def _choose_workspace(self) -> Tuple[Optional[str], Optional[str]]:
+        if CONFIG.sdk_key:
+            sdk_key_workspace, tenant_id = self._get_workspace_from_sdk_key()
+            if self._workspace_arg and sdk_key_workspace != self._workspace_arg:
+                raise ValueError(
+                    f"SDK Key's workspace: '{sdk_key_workspace}' does not match "
+                    f"chosen workspace: '{self._workspace_arg}'."
+                )
+            return sdk_key_workspace, tenant_id
+        try:
+            workspaces = WorkspaceClient().get_workspaces()
+        except RuntimeError:  # TODO: this is a hack to support v1.2.X
+            tenant_id = WorkspaceClient()._old_tenant()
+            return tenant_id, tenant_id
+        if self._workspace_arg:
+            if self._workspace_arg not in workspaces.index:
+                raise ValueError(
+                    f"Workspace '{self._workspace_arg}' not found. "
+                    f"Choose one of: {workspaces.index.tolist()}."
+                )
+            ws = workspaces.loc[self._workspace_arg]
+            return ws.name, ws.tenant_id
+        if len(workspaces) == 1:
+            ws = workspaces.iloc[0]
+            return ws.name, ws.tenant_id
+        if len(workspaces) > 1:
+            raise RuntimeError(
+                "Unable to determine workspace. "
+                "Specify a workspace or run `sumatra workspace select`."
+            )
+        raise RuntimeError("No workspaces found. Run `sumatra workspace create` first.")
+
+    def _get_workspace_from_sdk_key(self):
+        logger.debug("Fetching workspace from SDK key")
+        query = """
+            query Workspace {
+                workspace {
+                    id
+                    slug
+                }
+            }
+        """
+
+        ret = self._gql_client.execute(query=query)
+
+        if "errors" in ret:
+            raise RuntimeError(ret["errors"][0]["message"])
+
+        d = ret["data"]["workspace"]
+        return d["slug"], d["id"]
+
     @property
     def instance(self) -> str:
         """
         Instance name from client config, e.g. `'yourco.sumatra.ai'`
         """
         return CONFIG.instance
 
     @property
+    def workspace(self) -> Optional[str]:
+        """
+        User's current workspace slug, e.g. `my-workspace`
+        """
+        if not self._workspace:
+            self._workspace, self._workspace_id = self._choose_workspace()
+        return self._workspace
+
+    def _tenant_id(self) -> Optional[str]:
+        if not self._workspace_id:
+            self._workspace, self._workspace_id = self._choose_workspace()
+        return self._workspace_id
+
+    def update_workspace(
+        self,
+        name: Optional[str] = None,
+        slug: Optional[str] = None,
+        icon: Optional[bytes] = None,
+    ) -> Dict:
+        """
+        Update workspace metadata.
+
+        Arguments:
+            name: A human readable name for the new workspace
+            slug: Desired slug of the new workspace. Must consist only of letters, numbers, '-', and '_'. If this slug is taken, a random one will be generated instead, which may be changed later.
+            icon: Binary encoding of a PNG image to use as the workspace icon. Max size 50kb
+
+        Returns:
+            A dict of the updated workspace metadata
+        """
+
+        query = """
+            mutation UpdateWorkspace($id: String!, $name: String, $slug: String, $icon: String) {
+                updateTenant(id: $id, name: $name, slug: $slug, icon: $icon) {
+                    id
+                    slug
+                    name
+                }
+            }
+        """
+
+        if icon:
+            icon = base64.b64encode(icon).decode()
+
+        ret = self._gql_client.execute(
+            query=query,
+            variables={
+                "id": self._tenant_id(),
+                "name": name,
+                "slug": slug,
+                "icon": icon,
+            },
+        )
+
+        if "errors" in ret:
+            raise RuntimeError(ret["errors"][0]["message"])
+
+        d = ret["data"]["updateTenant"]
+        return {
+            "id": d["id"],
+            "slug": d["slug"],
+            "name": d["name"],
+        }
+
+    @property
     def branch(self) -> str:
         """
         Default branch name
         """
         return self._branch
 
     @branch.setter
     def branch(self, branch: str) -> None:
         self._branch = branch
 
+    def user_email(self) -> str:
+        """
+        Return the email address of the connected user.
+
+        Returns:
+            Email address
+        """
+        logger.debug("Fetching user")
+        query = """
+        query CurrentUser {
+            currentUser {
+                email
+            }
+        }
+        """
+
+        ret = self._gql_client.execute(query=query)
+
+        if "errors" in ret:
+            raise RuntimeError(ret["errors"][0]["message"])
+
+        return ret["data"]["currentUser"]["email"]
+
     def tenant(self) -> str:
         """
         Return the assigned tenant name for the connected user.
+        (DEPRECATED) use .workspace instead
+
+        Returns:
+            Tenant name (slug)
+        """
+        if self.version().startswith("v1.2"):
+            return WorkspaceClient()._old_tenant()
+        logger.warn(
+            "tenant() is deprecated and will be removed in the next release. Use .workspace instead."
+        )
+        return self.workspace
+
+    def sdk_key(self) -> str:
+        """
+        Return the SDK key for the connected workspace
 
         Returns:
-            Tenant name
+            SDK key
         """
-        logger.debug("Fetching tenant")
+        logger.debug("Fetching tenant sdk key")
         query = """
-            query Tenant {
-                tenant {
-                    key
+            query SDKKey {
+                currentTenant {
+                    accessKeys(type: "sdk") {
+                        nodes {
+                            key
+                        }
+                    }
                 }
             }
         """
 
         ret = self._gql_client.execute(query=query)
 
         if "errors" in ret:
             raise RuntimeError(ret["errors"][0]["message"])
 
-        return ret["data"]["tenant"]["key"]
+        return ret["data"]["currentTenant"]["accessKeys"]["nodes"][0]["key"]
+
+    def api_key(self) -> str:
+        """
+        Return the API key for the connected workspace
+
+        Returns:
+            API key
+        """
+        logger.debug("Fetching tenant api key")
+        query = """
+            query APIKey {
+                currentTenant {
+                    accessKeys(type: "api") {
+                        nodes {
+                            key
+                        }
+                    }
+                }
+            }
+        """
+
+        ret = self._gql_client.execute(query=query)
+
+        if "errors" in ret:
+            raise RuntimeError(ret["errors"][0]["message"])
+
+        return ret["data"]["currentTenant"]["accessKeys"]["nodes"][0]["key"]
 
     def query_athena(self, sql: str) -> pd.DataFrame:
         """
         Execute a SQL query against the Athena backend and return the
         result as a dataframe.
 
         Arguments:
             sql: SQL query (e.g. "select * from event_log where event_type='login' limit 10")
 
         Returns:
             Result of query as a Pandas dataframe
         """
         session = self._get_session()
-        tenant = self.tenant()
+        tenant = self._tenant_id()
         return wr.athena.read_sql_query(
             boto3_session=session,
             sql=sql,
             database=TENANT_PREFIX + tenant,
             workgroup=TENANT_PREFIX + tenant,
         )
 
@@ -950,15 +1136,16 @@
         for f, t in schema[event_type].items():
             if t in type_map:
                 selectors.append(scalar_selector.format(f, f, type_map[t], f))
             # elif t == "time":
             #    selectors.append(time_selector.format(f, f, f))
             else:
                 selectors.append(selector.format(f, f))
-                json_fields.append(f)
+                if f in features:
+                    json_fields.append(f)
 
         where = f"where {where}" if where else ""
         inputs = ""
         if include_inputs:
             inputs = ', event as "_inputs"'
             json_fields.append("_inputs")
 
@@ -1511,14 +1698,15 @@
         features: List[str],
         start_ts: Union[pd.Timestamp, str],
         end_ts: Union[pd.Timestamp, str],
         extra_timelines: Optional[List[str]] = None,
         branch: Optional[str] = None,
     ) -> Materialization:
         """
+        (BETA)
         Recompute historical feature values from LIVE event log on given topology branch.
 
         This is the primary function of the SDK.
 
         Arguments:
             features: List of features to materialize, e.g. `['login.email', 'purchase.*']`
             start_ts: Earliest event timestamp to materialize (local client timezone).
@@ -1889,15 +2077,15 @@
             aws_access_key_id=creds["AccessKeyID"],
             aws_secret_access_key=creds["SecretAccessKey"],
             aws_session_token=creds["SessionToken"],
         )
 
     def get_deps(self, live: bool = False) -> str:
         """
-        Fetch latest dependencies from sever as Scowl source `require` statements.
+        Fetch latest dependencies from server as Scowl source `require` statements.
 
         Arguments:
             live: Return the LIVE versions of dependencies instead of latest.
 
         Returns:
             Scowl source code as string.
         """
@@ -2379,206 +2567,14 @@
             variables={
                 "name": model,
             },
         )
         if "errors" in ret:
             raise RuntimeError(ret["errors"][0]["message"])
 
-    def list_users(self) -> None:
-        """
-        List users.
-        """
-        query = """
-            query ListUsers {
-                users {
-                    nodes {
-                        username
-                    }
-                }
-            }
-        """
-
-        ret = self._gql_client.execute(query=query)
-
-        if "errors" in ret:
-            raise RuntimeError(ret["errors"][0]["message"])
-
-        return [user["username"] for user in ret["data"]["users"]["nodes"]]
-
-    def get_user(self, username: str) -> Dict[str, str]:
-        """
-        Get User.
-        """
-        query = """
-            query User($username: String!) {
-                user(username: $username) {
-                    username
-                    email
-                    role
-                    tenant
-                    admin
-                    status
-                }
-            }
-        """
-
-        ret = self._gql_client.execute(
-            query=query,
-            variables={
-                "username": username,
-            },
-        )
-
-        if "errors" in ret:
-            raise RuntimeError(ret["errors"][0]["message"])
-
-        return ret["data"]["user"]
-
-    def list_tenants(self) -> None:
-        """
-        List tenants.
-        """
-        query = """
-                query ListTenants {
-                    tenants {
-                        nodes {
-                            key
-                        }
-                    }
-                }
-            """
-
-        ret = self._gql_client.execute(query=query)
-
-        if "errors" in ret:
-            raise RuntimeError(ret["errors"][0]["message"])
-
-        return [tenant["key"] for tenant in ret["data"]["tenants"]["nodes"]]
-
-    def set_tenant(self, username: str, tenant: str):
-        """
-        Set tenant for user
-        """
-        query = """
-            mutation SetTenant($username: String!, $tenant: String!) {
-                 setUserTenant(username: $username, tenant: $tenant) {
-                    tenant
-                    username
-                  }
-            }
-        """
-
-        ret = self._gql_client.execute(
-            query=query,
-            variables={
-                "username": username,
-                "tenant": tenant,
-            },
-        )
-
-        if "errors" in ret:
-            raise RuntimeError(ret["errors"][0]["message"])
-
-    def set_role(self, username: str, role: str):
-        """
-        Set role for user
-        """
-        query = """
-            mutation SetRole($username: String!, $role: String!) {
-                 setUserRole(username: $username, role: $role) {
-                    role
-                    username
-                  }
-            }
-        """
-
-        ret = self._gql_client.execute(
-            query=query,
-            variables={
-                "username": username,
-                "role": role,
-            },
-        )
-
-        if "errors" in ret:
-            raise RuntimeError(ret["errors"][0]["message"])
-
-    def get_keys(self) -> pd.DataFrame:
-        """
-        Get API Keys for tenants
-        """
-        query = """
-            query ApiKeys {
-                tenants {
-                    nodes {
-                        key
-                        apiKey
-                        sdkKey
-                    }
-                }
-            }
-        """
-
-        ret = self._gql_client.execute(query=query)
-        if "errors" in ret:
-            raise RuntimeError(ret["errors"][0]["message"])
-
-        rows = []
-        for tenant in ret["data"]["tenants"]["nodes"]:
-            rows.append((tenant["key"], "api", tenant["apiKey"]))
-            rows.append((tenant["key"], "sdk", tenant["sdkKey"]))
-
-        return (
-            pd.DataFrame(rows, columns=("Tenant", "Type", "Key"))
-            .set_index(["Tenant", "Type"])
-            .sort_index()
-        )
-
-    def get_key_usage(self, start_date=None, end_date=None) -> pd.DataFrame:
-        """
-        Get API Key usage for tenants
-        """
-        query = """
-            query ApiKeyUsage($startDate: DateTime!, $endDate: DateTime!) {
-                apiKeyUsage(startDate: $startDate, endDate: $endDate) {
-                    tenant
-                    apiType
-                    dailyUsage
-                }
-            }
-        """
-
-        end_date = end_date or pendulum.today()
-        start_date = start_date or end_date.subtract(days=6)
-
-        ret = self._gql_client.execute(
-            query=query,
-            variables={
-                "startDate": start_date.to_iso8601_string(),
-                "endDate": end_date.to_iso8601_string(),
-            },
-        )
-
-        if "errors" in ret:
-            raise RuntimeError(ret["errors"][0]["message"])
-
-        days = [d.to_date_string() for d in end_date - start_date]
-        rows = []
-        for usage in ret["data"]["apiKeyUsage"]:
-            dailyUsage = usage["dailyUsage"]
-            if len(dailyUsage) == 0:
-                dailyUsage = [0 for _ in days]
-            rows.append([usage["tenant"], usage["apiType"]] + dailyUsage)
-
-        return (
-            pd.DataFrame(rows, columns=["Tenant", "Type"] + days)
-            .set_index(["Tenant", "Type"])
-            .sort_index()
-        )
-
 
 class ModelVersion:
     """
     A handle to a versioned model resource
     """
 
     def __init__(self, client: Client, name: str, version: str):
@@ -2835,15 +2831,15 @@
         if not self._tv:
             self._tv = self._get_table_version()
         return self._tv["key"]
 
 
 class Materialization:
     """
-    A handle to a server-side materialization job, which enriches a Timeline
+    A handle to a server-side materialization (replay) job, which enriches a Timeline
     (or set of Timelines) by running it (them) through a given Topology.
 
     Objects are not constructed directly. Materializations are returned by methods
     of the `Client` class.
     """
 
     def __init__(self, client, id):
@@ -2974,17 +2970,17 @@
         S3 bucket path where results are stored.
         """
         self.wait()
         return self._mtr["path"]
 
     def get_events(self, event_type: str, features: List[str] = []) -> pd.DataFrame:
         """
-        (DEPRECATED)
         Return enriched events of specified type. Waits if
         job is still processing.
+        (DEPRECATED) use get_features() instead.
 
         Arguments:
             event_type: Name of event type to fetch.
             features: Feature names to fetch. By default, fetch all.
 
         Returns:
             Enriched events
```

### Comparing `sumatra-client-1.2.0/sumatra_client/config.py` & `sumatra-client-1.3.0rc1/sumatra_client/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 import pendulum
 import getpass
 
 from logging import getLogger
 from pathlib import Path
 from posixpath import join as urljoin
 from configparser import ConfigParser
-from typing import Optional, Dict, Tuple
+from typing import Optional, Dict, Tuple, List
 
 logger = getLogger("sumatra.config")
 
 _CONFIG_PATH = os.path.expanduser(
     os.environ.get("SUMATRA_CONFIG_PATH", os.path.join(Path.home(), ".sumatra"))
 )
 _CONFIG_FILE = os.path.join(_CONFIG_PATH, "config")
 
 
 def _sanitize_instance(instance: str) -> Tuple[str, str]:
     if not instance:
-        raise Exception("Either provide 'instance' or run `sumatra login`")
+        raise RuntimeError("Either provide 'instance' or run `sumatra login`")
 
     for localhost in ("localhost:", "127.0.0.1:", "0.0.0.0:"):
         if instance.startswith(localhost):
             return "http", instance
         if instance.startswith(f"http://{localhost}"):
             return "http", instance[7:]
 
     if instance.startswith("http://"):
-        raise Exception("Sumatra Instance URL must start with https://")
+        raise ValueError("Sumatra Instance URL must start with https://")
 
     if instance.startswith("https://"):
         return "https", instance[8:]
 
     return "https", instance
 
 
@@ -94,14 +94,15 @@
             raise Exception("error fetching stack config from: " + stack_config_url)
 
     def summary(self, unmask=False):
         return f"""Config File: {_CONFIG_FILE}
 Tokens File: {self.jwt_tokens_path}
 
 instance:       {self.instance}
+workspace:      {self.workspace}
 default_branch: {self.default_branch}
 scowl_dir:      {self.scowl_dir}
 timezone:       {self.timezone}
 
 api_event_url:       {self.api_event_url}
 console_graphql_url: {self.console_graphql_url}
 sdk_graphql_url:     {self.sdk_graphql_url}
@@ -122,29 +123,30 @@
         self._set(
             "cognito_token_url",
             f"https://{user_pool_domain}.auth.us-east-1.amazoncognito.com/oauth2/token",
         )
         self._set("console_endpoint", stack["console_uri"])
         api_uri = stack["api_uri"]
         self._set("api_endpoint", api_uri)
+        self._set("server_version", stack.get("version", "v1.2.0"))
         sdk_uri = stack["sdk_uri"]
         sdk_vpce_ids = stack["sdk_vpc_endpoint_ids"]
         if sdk_vpce_ids:
             sdk_uri = sdk_uri.replace(".execute-api", f"-{sdk_vpce_ids[0]}.execute-api")
         self._set("sdk_endpoint", sdk_uri)
         self.save(update_default_instance=False)
 
     @property
     def instance(self) -> str:
         if not self._instance:
             self.instance = os.environ.get("SUMATRA_INSTANCE") or self._config[
                 "DEFAULT"
             ].get("instance")
         if not self._instance:
-            raise Exception("Either provide 'instance' or run `sumatra login`")
+            raise RuntimeError("Either provide 'instance' or run `sumatra login`")
         return self._instance
 
     @instance.setter
     def instance(self, instance: str) -> None:
         self._instance_protocol, self._instance = _sanitize_instance(instance)
 
     @property
@@ -174,22 +176,35 @@
 
     @default_branch.setter
     def default_branch(self, branch: str) -> None:
         self._set("default_branch", branch)
         self.save(update_default_instance=False)
 
     @property
+    def workspace(self) -> str:
+        return self._get("workspace")
+
+    @workspace.setter
+    def workspace(self, workspace: str) -> None:
+        self._set("workspace", workspace)
+        self.save(update_default_instance=False)
+
+    @property
     def timezone(self) -> Optional[str]:
         return self._get("timezone") or pendulum.now().timezone_name
 
     @property
     def scowl_dir(self) -> str:
         return self._get("scowl_dir") or "."
 
     @property
+    def server_version(self) -> str:
+        return self._get_or_stack("server_version")
+
+    @property
     def user_pool_id(self) -> str:
         return self._get_or_stack("user_pool_id")
 
     @property
     def user_pool_domain(self) -> str:
         return self._get_or_stack("user_pool_domain")
```

### Comparing `sumatra-client-1.2.0/sumatra_client.egg-info/PKG-INFO` & `sumatra-client-1.3.0rc1/sumatra_client.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumatra-client
-Version: 1.2.0
+Version: 1.3.0rc1
 Summary: Sumatra Python Client and CLI
 Home-page: https://sumatra.ai
 Author: Sumatra
 Author-email: support@sumatra.ai
 License: Sumatra Proprietary
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sumatra-client-1.2.0/tests/test_config.py` & `sumatra-client-1.3.0rc1/tests/test_config.py`

 * *Files identical despite different names*

