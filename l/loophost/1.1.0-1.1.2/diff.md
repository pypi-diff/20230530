# Comparing `tmp/loophost-1.1.0.tar.gz` & `tmp/loophost-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loophost-1.1.0.tar", max compression
+gzip compressed data, was "loophost-1.1.2.tar", max compression
```

## Comparing `loophost-1.1.0.tar` & `loophost-1.1.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0       68 2023-05-29 23:50:14.168206 loophost-1.1.0/README.md
--rw-r--r--   0        0        0        5 2023-05-29 23:50:14.168206 loophost-1.1.0/VERSION
--rw-r--r--   0        0        0      670 2023-05-29 23:50:14.168206 loophost-1.1.0/build.py
--rw-r--r--   0        0        0      925 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/__init__.py
--rw-r--r--   0        0        0     4401 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/flingroute.py
--rw-r--r--   0        0        0     3452 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/installer.py
--rw-r--r--   0        0        0     1353 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/launchd_plist.py
--rw-r--r--   0        0        0      787 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/plist/hub.plist.template
--rw-r--r--   0        0        0      771 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/plist/loophost.plist.template
--rw-r--r--   0        0        0     1150 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/plist/ssh.plist.template
--rw-r--r--   0        0        0      100 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/postinstall.py
--rw-r--r--   0        0        0    95159 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/static/fling-logo-dark.png
--rw-r--r--   0        0        0   265670 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/static/fling-logo-light.png
--rw-r--r--   0        0        0     6393 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/static/github-mark.png
--rw-r--r--   0        0        0     3834 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/static/logo-hc.txt
--rw-r--r--   0        0        0    34153 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/static/logo-square.png
--rw-r--r--   0        0        0      457 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/step_two.py
--rw-r--r--   0        0        0      828 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/templates/admin.html
--rw-r--r--   0        0        0     1657 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/templates/base.html
--rw-r--r--   0        0        0     2921 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/templates/local.html
--rw-r--r--   0        0        0     1478 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/templates/partials/apptable.html
--rw-r--r--   0        0        0      289 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/templates/partials/upgrade.html
--rw-r--r--   0        0        0     1730 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/templates/start/base.html
--rw-r--r--   0        0        0     1656 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/uninstall.py
--rw-r--r--   0        0        0      517 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/win/build.txt
--rw-r--r--   0        0        0     2431 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/win_hub.py
--rw-r--r--   0        0        0     2584 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/win_lp.py
--rw-r--r--   0        0        0     1181 2023-05-29 23:50:14.176206 loophost-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-29 23:50:14.176206 loophost-1.1.0/setup.py
--rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 loophost-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      692 2023-05-30 00:33:36.436715 loophost-1.1.2/build.py
+-rw-r--r--   0        0        0      964 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/__init__.py
+-rw-r--r--   0        0        0     4540 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/flingroute.py
+-rw-r--r--   0        0        0     3580 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/installer.py
+-rw-r--r--   0        0        0     1395 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/launchd_plist.py
+-rwxr-xr-x   0        0        0  8761344 2023-05-30 00:35:57.357405 loophost-1.1.2/loophost/loopproxy.exe
+-rw-r--r--   0        0        0      813 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/plist/hub.plist.template
+-rw-r--r--   0        0        0      796 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/plist/loophost.plist.template
+-rw-r--r--   0        0        0     1182 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/plist/ssh.plist.template
+-rw-r--r--   0        0        0      105 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/postinstall.py
+-rw-r--r--   0        0        0    95159 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/static/fling-logo-dark.png
+-rw-r--r--   0        0        0   265670 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/static/fling-logo-light.png
+-rw-r--r--   0        0        0     6393 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/static/github-mark.png
+-rw-r--r--   0        0        0     3854 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/static/logo-hc.txt
+-rw-r--r--   0        0        0    34153 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/static/logo-square.png
+-rw-r--r--   0        0        0      475 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/step_two.py
+-rw-r--r--   0        0        0      866 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/templates/admin.html
+-rw-r--r--   0        0        0     1718 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/templates/base.html
+-rw-r--r--   0        0        0     3007 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/templates/local.html
+-rw-r--r--   0        0        0     1517 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/templates/partials/apptable.html
+-rw-r--r--   0        0        0      293 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/templates/partials/upgrade.html
+-rw-r--r--   0        0        0     1770 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/templates/start/base.html
+-rw-r--r--   0        0        0     1712 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/uninstall.py
+-rw-r--r--   0        0        0      527 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/win/build.txt
+-rw-r--r--   0        0        0     2509 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/win_hub.py
+-rw-r--r--   0        0        0     2671 2023-05-30 00:33:36.436715 loophost-1.1.2/loophost/win_lp.py
+-rw-r--r--   0        0        0     1226 2023-05-30 00:33:36.436715 loophost-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-05-30 00:33:36.436715 loophost-1.1.2/README.md
+-rw-r--r--   0        0        0       43 2023-05-30 00:33:36.436715 loophost-1.1.2/setup.py
+-rw-r--r--   0        0        0        5 2023-05-30 00:33:36.436715 loophost-1.1.2/VERSION
+-rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 loophost-1.1.2/PKG-INFO
```

### Comparing `loophost-1.1.0/loophost/__init__.py` & `loophost-1.1.2/loophost/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-__version__ = "1.1.0"
-
-import os
-import pathlib
-import platform
-import sys
-
-
-LOOPHOST_DOMAIN = "loophost.dev"
-TUNNEL_DOMAIN = "fling.team"
-
-PYEX = sys.executable
-HUBDIR = os.path.dirname(os.path.realpath(__file__))
-
-
-def GET_LOOPHOST_DIR():
-    DIR = pathlib.Path("/Users", "Shared", ".loophost")
-    if platform.system().lower().startswith("win"):
-        DIR = pathlib.Path("\\Users", "Public", ".loophost")
-    os.makedirs(DIR, exist_ok=True)
-    os.chdir(DIR)
-    return os.path.abspath(os.path.curdir)
-
-
-_USERNAME = None
-
-
-def GET_FLINGUSER_NAME():
-    global _USERNAME
-    if _USERNAME is None:
-        flinguser_path = pathlib.Path(GET_LOOPHOST_DIR(), "flinguser.txt")
-        if os.path.exists(flinguser_path):
-            with open(flinguser_path, "r") as userfile:
-                _USERNAME = userfile.read()
-    return _USERNAME
-
-
-def DATA_FILE_PATH():
-    return pathlib.Path(GET_LOOPHOST_DIR(), "loophost.json")
+__version__ = "1.1.2"
+
+import os
+import pathlib
+import platform
+import sys
+
+
+LOOPHOST_DOMAIN = "loophost.dev"
+TUNNEL_DOMAIN = "fling.team"
+
+PYEX = sys.executable
+HUBDIR = os.path.dirname(os.path.realpath(__file__))
+
+
+def GET_LOOPHOST_DIR():
+    DIR = pathlib.Path("/Users", "Shared", ".loophost")
+    if platform.system().lower().startswith("win"):
+        DIR = pathlib.Path("\\Users", "Public", ".loophost")
+    os.makedirs(DIR, exist_ok=True)
+    os.chdir(DIR)
+    return os.path.abspath(os.path.curdir)
+
+
+_USERNAME = None
+
+
+def GET_FLINGUSER_NAME():
+    global _USERNAME
+    if _USERNAME is None:
+        flinguser_path = pathlib.Path(GET_LOOPHOST_DIR(), "flinguser.txt")
+        if os.path.exists(flinguser_path):
+            with open(flinguser_path, "r") as userfile:
+                _USERNAME = userfile.read()
+    return _USERNAME
+
+
+def DATA_FILE_PATH():
+    return pathlib.Path(GET_LOOPHOST_DIR(), "loophost.json")
```

### Comparing `loophost-1.1.0/loophost/flingroute.py` & `loophost-1.1.2/loophost/flingroute.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-"""Loophost administration web app.
-This runs as a launchd-dispatched python web app.
-It displays a web-based administration screen.
-Must be run with a CWD of the .loophost folder.
-"""
-
-import os
-import sys
-import json
-import pathlib
-from fling import start as startmod
-from fling.start import start
-from flask import Flask, request, render_template, redirect
-from flask_bootstrap import Bootstrap5
-from flask_caching import Cache
-from loophost.launchd_plist import register_tunnel, unregister_tunnel, generate_keys
-from loophost import HUBDIR, __version__, DATA_FILE_PATH
-from lastversion import has_update
-from fling_cli import get_fling_client
-from fling_client.api.loophost import expose_app_expose_app_put
-from flask_wtf.csrf import CSRFProtect
-
-
-config = json.loads(pathlib.Path.read_text(DATA_FILE_PATH()))
-
-admin = None
-if getattr(sys, 'frozen', False):
-    template_folder = os.path.join(sys._MEIPASS, 'templates')
-    static_folder = os.path.join(sys._MEIPASS, 'static')
-    admin = Flask(__name__, template_folder=template_folder, static_folder=static_folder)
-else:
-    admin = Flask(__name__)
-
-admin.config["SECRET_KEY"] = config.get('SECRET_KEY', 'foobar')
-csrf = CSRFProtect(admin)
-bootstrap = Bootstrap5(admin)
-cache = Cache(config={"CACHE_TYPE": "SimpleCache"})
-cache.init_app(admin)
-
-
-@cache.cached(timeout=3600)
-def latest_version():
-    return has_update(repo="loophost", at="pip", current_version=__version__)
-
-
-@admin.context_processor
-def inject_globals():
-    return dict(NEW_VERSION=latest_version())
-
-
-def setup_tunnel_keys(project):
-    if not os.path.exists("tunnelkey.pub"):
-        # TODO(JMC): Don't do this so often
-        fling_client = get_fling_client(require_auth=True)
-        pub, priv = generate_keys()
-        with open("tunnelkey.pub", "w+") as pubfile:
-            pubfile.write(pub)
-        with open("tunnelkey", "w+") as privfile:
-            privfile.write(priv)
-        os.chmod("tunnelkey", 0o600)
-        expose_app_expose_app_put.sync(
-            client=fling_client, app_name=project, ssh_public_key=pub
-        )
-
-
-def unbind(project):
-    del config["apps"][project]
-    with open(DATA_FILE_PATH(), "w+") as appjson:
-        appjson.write(json.dumps(config))
-    return
-
-
-def share(project):
-    target = pathlib.Path(
-        pathlib.Path.home(),
-        "Library",
-        "LaunchAgents",
-        f"dev.fling.hub.ssh.{project}.plist",
-    )
-
-    if project and project in config.get("share", {}):
-        del config["share"][project]
-        unregister_tunnel(target)
-    elif project:
-        setup_tunnel_keys(project)
-        if not config.get("share"):
-            config["share"] = {}
-        config["share"][project] = "public"
-        register_tunnel(
-            project, pathlib.Path(HUBDIR, "plist", "ssh.plist.template"), target
-        )
-    with open(DATA_FILE_PATH(), "w+") as appjson:
-        appjson.write(json.dumps(config))
-    return redirect(f"/config/{project}")
-
-
-@admin.route("/config/<project>", methods=["GET", "POST"])
-def config_page(project):
-    if project and project in config["apps"]:
-        print(f"Updating config for {project} with action {request.form.get('action')}")
-        if request.form.get("action") == "unbind":
-            unbind(project)
-            return redirect("/")
-        elif request.form.get("action") == "share":
-            share(project)
-    if request.form.get("application_port") and not request.form.get("action"):
-        config["apps"][project] = request.form.get("application_port")
-        with open(DATA_FILE_PATH(), "w+") as appjson:
-            appjson.write(json.dumps(config))
-
-    return render_template(
-        "local.html",
-        config=config,
-        apps=config["apps"],
-        share=config.get("share", {}),
-        project=project,
-    )
-
-
-@admin.route("/", defaults={"path": ""}, methods=["GET", "POST"])
-@admin.route("/<path:path>", methods=["GET", "POST"])
-def admin_page(path):
-    fqdn = request.host.split(".")
-    if len(fqdn) < 4:
-        return render_template(
-            "admin.html",
-            config=config,
-            apps=config["apps"],
-            share=config.get("share"),
-            fqdn=".".join(fqdn),
-        )
-    project = fqdn.pop(0)
-    return redirect(f"https://{config['fqdn']}/config/{project}")
-
-
-if __name__ == "__main__":
-    # admin.run(host=f"unix://{os.getcwd()}/loophost.soc")
-    admin.run(host=f"0.0.0.0", port=5816)
-
+"""Loophost administration web app.
+This runs as a launchd-dispatched python web app.
+It displays a web-based administration screen.
+Must be run with a CWD of the .loophost folder.
+"""
+
+import os
+import sys
+import json
+import pathlib
+from fling import start as startmod
+from fling.start import start
+from flask import Flask, request, render_template, redirect
+from flask_bootstrap import Bootstrap5
+from flask_caching import Cache
+from loophost.launchd_plist import register_tunnel, unregister_tunnel, generate_keys
+from loophost import HUBDIR, __version__, DATA_FILE_PATH
+from lastversion import has_update
+from fling_cli import get_fling_client
+from fling_client.api.loophost import expose_app_expose_app_put
+from flask_wtf.csrf import CSRFProtect
+
+
+config = json.loads(pathlib.Path.read_text(DATA_FILE_PATH()))
+
+admin = None
+if getattr(sys, 'frozen', False):
+    template_folder = os.path.join(sys._MEIPASS, 'templates')
+    static_folder = os.path.join(sys._MEIPASS, 'static')
+    admin = Flask(__name__, template_folder=template_folder, static_folder=static_folder)
+else:
+    admin = Flask(__name__)
+
+admin.config["SECRET_KEY"] = config.get('SECRET_KEY', 'foobar')
+csrf = CSRFProtect(admin)
+bootstrap = Bootstrap5(admin)
+cache = Cache(config={"CACHE_TYPE": "SimpleCache"})
+cache.init_app(admin)
+
+
+@cache.cached(timeout=3600)
+def latest_version():
+    return has_update(repo="loophost", at="pip", current_version=__version__)
+
+
+@admin.context_processor
+def inject_globals():
+    return dict(NEW_VERSION=latest_version())
+
+
+def setup_tunnel_keys(project):
+    if not os.path.exists("tunnelkey.pub"):
+        # TODO(JMC): Don't do this so often
+        fling_client = get_fling_client(require_auth=True)
+        pub, priv = generate_keys()
+        with open("tunnelkey.pub", "w+") as pubfile:
+            pubfile.write(pub)
+        with open("tunnelkey", "w+") as privfile:
+            privfile.write(priv)
+        os.chmod("tunnelkey", 0o600)
+        expose_app_expose_app_put.sync(
+            client=fling_client, app_name=project, ssh_public_key=pub
+        )
+
+
+def unbind(project):
+    del config["apps"][project]
+    with open(DATA_FILE_PATH(), "w+") as appjson:
+        appjson.write(json.dumps(config))
+    return
+
+
+def share(project):
+    target = pathlib.Path(
+        pathlib.Path.home(),
+        "Library",
+        "LaunchAgents",
+        f"dev.fling.hub.ssh.{project}.plist",
+    )
+
+    if project and project in config.get("share", {}):
+        del config["share"][project]
+        unregister_tunnel(target)
+    elif project:
+        setup_tunnel_keys(project)
+        if not config.get("share"):
+            config["share"] = {}
+        config["share"][project] = "public"
+        register_tunnel(
+            project, pathlib.Path(HUBDIR, "plist", "ssh.plist.template"), target
+        )
+    with open(DATA_FILE_PATH(), "w+") as appjson:
+        appjson.write(json.dumps(config))
+    return redirect(f"/config/{project}")
+
+
+@admin.route("/config/<project>", methods=["GET", "POST"])
+def config_page(project):
+    if project and project in config["apps"]:
+        print(f"Updating config for {project} with action {request.form.get('action')}")
+        if request.form.get("action") == "unbind":
+            unbind(project)
+            return redirect("/")
+        elif request.form.get("action") == "share":
+            share(project)
+    if request.form.get("application_port") and not request.form.get("action"):
+        config["apps"][project] = request.form.get("application_port")
+        with open(DATA_FILE_PATH(), "w+") as appjson:
+            appjson.write(json.dumps(config))
+
+    return render_template(
+        "local.html",
+        config=config,
+        apps=config["apps"],
+        share=config.get("share", {}),
+        project=project,
+    )
+
+
+@admin.route("/", defaults={"path": ""}, methods=["GET", "POST"])
+@admin.route("/<path:path>", methods=["GET", "POST"])
+def admin_page(path):
+    fqdn = request.host.split(".")
+    if len(fqdn) < 4:
+        return render_template(
+            "admin.html",
+            config=config,
+            apps=config["apps"],
+            share=config.get("share"),
+            fqdn=".".join(fqdn),
+        )
+    project = fqdn.pop(0)
+    return redirect(f"https://{config['fqdn']}/config/{project}")
+
+
+if __name__ == "__main__":
+    # admin.run(host=f"unix://{os.getcwd()}/loophost.soc")
+    admin.run(host=f"0.0.0.0", port=5816)
+
```

### Comparing `loophost-1.1.0/loophost/installer.py` & `loophost-1.1.2/loophost/installer.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-import getpass
-import json
-import os
-import platform
-import sys
-import pathlib
-import subprocess
-from subprocess import run
-import webbrowser
-from certbot.main import main as certmain
-from fling_cli.auth import gh_authenticate
-
-from loophost.launchd_plist import register_tunnel
-from loophost import (
-    LOOPHOST_DOMAIN,
-    TUNNEL_DOMAIN,
-    HUBDIR,
-    GET_LOOPHOST_DIR,
-    GET_FLINGUSER_NAME,
-    DATA_FILE_PATH,
-)
-
-
-def post_install_one():
-    print("Installing LoopHost...")
-    localuser_file = pathlib.Path(GET_LOOPHOST_DIR(), "localuser.txt")
-    with open(localuser_file, "w+") as userfile:
-        userfile.write(getpass.getuser())
-    authenticate_with_fling()
-    if not platform.system().lower().startswith('win'):
-        issue_certs()
-    create_update_loophost_json()
-    register_tunnel(
-        "flinghub",
-        pathlib.Path(HUBDIR, "plist", "loophost.plist.template"),
-        pathlib.Path(
-            pathlib.Path.home(), "Library/LaunchAgents/dev.fling.hub.local.plist"
-        ),
-    )
-
-    step_two_as_root()
-
-
-def post_install_two():
-    if platform.system().lower().startswith('win'):
-        issue_certs()
-    setup_launchd_scripts()
-
-
-def authenticate_with_fling():
-    if not GET_FLINGUSER_NAME():
-        gh_authenticate()
-    if not GET_FLINGUSER_NAME():
-        raise Exception("Github authentication failed, can't continue install.")
-
-
-
-def issue_certs():
-    USERNAME = GET_FLINGUSER_NAME()
-    print("Generating SSL certificates (this may take a minute)...")
-    cmd = [
-            "certonly",
-            "--config-dir", "./",
-            "--work-dir", "./",
-            "--logs-dir", "./",
-            "--non-interactive",
-            "--expand",
-            "--agree-tos",
-            f"-m webmaster@{LOOPHOST_DOMAIN}",
-            "--authenticator=fling_authenticator",
-            f'-d *.{USERNAME}.{LOOPHOST_DOMAIN}',
-            f'-d *.{USERNAME}.{TUNNEL_DOMAIN}',
-            f'-d {USERNAME}.{LOOPHOST_DOMAIN}',
-            "--fling_authenticator-propagation-seconds=15",
-        ]
-    
-    certmain(cmd)
-
-
-def create_update_loophost_json():
-    USERNAME = GET_FLINGUSER_NAME()
-    data = None
-    if os.path.exists(DATA_FILE_PATH()):
-        with open(DATA_FILE_PATH(), "r") as datafile:
-            data = json.loads(datafile.read())
-    else:
-        data = {"apps": {}, "share": {}}
-    data.update(
-        {
-            "fqdn": f"{USERNAME}.{LOOPHOST_DOMAIN}",
-            "tunnel": f"{USERNAME}.{TUNNEL_DOMAIN}",
-        }
-    )
-    with open(DATA_FILE_PATH(), "w") as datafile:
-        datafile.write(json.dumps(data))
-    return data
-
-
-def setup_launchd_scripts():
-    register_tunnel(
-        "flinghub",
-        pathlib.Path(HUBDIR, "plist", "hub.plist.template"),
-        "/Library/LaunchDaemons/dev.fling.hub.plist",
-    )
-    print("All done.")
-
-
-def step_two_as_root():
-    print(
-        """Switching to root/admin user to install web services on ports 443 and 80\n\r
-        (you will be prompted for your password)"""
-    )
-    cmd = "sudo python3 -m loophost.step_two"
-    if platform.system().lower().startswith('win'):
-        cmd = "python3 -m loophost.step_two"
-    run(
-        cmd,
-        shell=True,
-        # stdout=subprocess.PIPE,
-        # stderr=subprocess.PIPE,
-        # stdin=subprocess.PIPE,
-        cwd=GET_LOOPHOST_DIR(),
-        check=True
-    )
-    print("All finished.")
-    webbrowser.open(f"https://{GET_FLINGUSER_NAME()}.{LOOPHOST_DOMAIN}")
-    sys.exit()
-
+import getpass
+import json
+import os
+import platform
+import sys
+import pathlib
+import subprocess
+from subprocess import run
+import webbrowser
+from certbot.main import main as certmain
+from fling_cli.auth import gh_authenticate
+
+from loophost.launchd_plist import register_tunnel
+from loophost import (
+    LOOPHOST_DOMAIN,
+    TUNNEL_DOMAIN,
+    HUBDIR,
+    GET_LOOPHOST_DIR,
+    GET_FLINGUSER_NAME,
+    DATA_FILE_PATH,
+)
+
+
+def post_install_one():
+    print("Installing LoopHost...")
+    localuser_file = pathlib.Path(GET_LOOPHOST_DIR(), "localuser.txt")
+    with open(localuser_file, "w+") as userfile:
+        userfile.write(getpass.getuser())
+    authenticate_with_fling()
+    if not platform.system().lower().startswith('win'):
+        issue_certs()
+    create_update_loophost_json()
+    register_tunnel(
+        "flinghub",
+        pathlib.Path(HUBDIR, "plist", "loophost.plist.template"),
+        pathlib.Path(
+            pathlib.Path.home(), "Library/LaunchAgents/dev.fling.hub.local.plist"
+        ),
+    )
+
+    step_two_as_root()
+
+
+def post_install_two():
+    if platform.system().lower().startswith('win'):
+        issue_certs()
+    setup_launchd_scripts()
+
+
+def authenticate_with_fling():
+    if not GET_FLINGUSER_NAME():
+        gh_authenticate()
+    if not GET_FLINGUSER_NAME():
+        raise Exception("Github authentication failed, can't continue install.")
+
+
+
+def issue_certs():
+    USERNAME = GET_FLINGUSER_NAME()
+    print("Generating SSL certificates (this may take a minute)...")
+    cmd = [
+            "certonly",
+            "--config-dir", "./",
+            "--work-dir", "./",
+            "--logs-dir", "./",
+            "--non-interactive",
+            "--expand",
+            "--agree-tos",
+            f"-m webmaster@{LOOPHOST_DOMAIN}",
+            "--authenticator=fling_authenticator",
+            f'-d *.{USERNAME}.{LOOPHOST_DOMAIN}',
+            f'-d *.{USERNAME}.{TUNNEL_DOMAIN}',
+            f'-d {USERNAME}.{LOOPHOST_DOMAIN}',
+            "--fling_authenticator-propagation-seconds=15",
+        ]
+    
+    certmain(cmd)
+
+
+def create_update_loophost_json():
+    USERNAME = GET_FLINGUSER_NAME()
+    data = None
+    if os.path.exists(DATA_FILE_PATH()):
+        with open(DATA_FILE_PATH(), "r") as datafile:
+            data = json.loads(datafile.read())
+    else:
+        data = {"apps": {}, "share": {}}
+    data.update(
+        {
+            "fqdn": f"{USERNAME}.{LOOPHOST_DOMAIN}",
+            "tunnel": f"{USERNAME}.{TUNNEL_DOMAIN}",
+        }
+    )
+    with open(DATA_FILE_PATH(), "w") as datafile:
+        datafile.write(json.dumps(data))
+    return data
+
+
+def setup_launchd_scripts():
+    register_tunnel(
+        "flinghub",
+        pathlib.Path(HUBDIR, "plist", "hub.plist.template"),
+        "/Library/LaunchDaemons/dev.fling.hub.plist",
+    )
+    print("All done.")
+
+
+def step_two_as_root():
+    print(
+        """Switching to root/admin user to install web services on ports 443 and 80\n\r
+        (you will be prompted for your password)"""
+    )
+    cmd = "sudo python3 -m loophost.step_two"
+    if platform.system().lower().startswith('win'):
+        cmd = "python3 -m loophost.step_two"
+    run(
+        cmd,
+        shell=True,
+        # stdout=subprocess.PIPE,
+        # stderr=subprocess.PIPE,
+        # stdin=subprocess.PIPE,
+        cwd=GET_LOOPHOST_DIR(),
+        check=True
+    )
+    print("All finished.")
+    webbrowser.open(f"https://{GET_FLINGUSER_NAME()}.{LOOPHOST_DOMAIN}")
+    sys.exit()
+
```

### Comparing `loophost-1.1.0/loophost/launchd_plist.py` & `loophost-1.1.2/loophost/launchd_plist.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from io import StringIO
-import pathlib
-import shutil
-from loophost import LOOPHOST_DOMAIN, TUNNEL_DOMAIN, PYEX, HUBDIR, GET_FLINGUSER_NAME, GET_LOOPHOST_DIR
-from string import Template
-from subprocess import run
-import paramiko
-
-
-def generate_keys():
-    key = paramiko.RSAKey.generate(2048)
-    privateString = StringIO()
-    key.write_private_key(privateString)
-    return f"{key.get_name()} {key.get_base64()}", privateString.getvalue()
-
-
-def register_tunnel(project, template_path, target_path):
-    TARGET_DIR = GET_LOOPHOST_DIR()
-    shutil.copy2(template_path, TARGET_DIR)
-
-    d = {"CWD": TARGET_DIR,
-         "USERNAME": GET_FLINGUSER_NAME(),
-         "PYEX": PYEX,
-         "HUBDIR": HUBDIR,
-         "LOOPHOST_DOMAIN": LOOPHOST_DOMAIN,
-         "TUNNEL_DOMAIN": TUNNEL_DOMAIN,
-         "LOCAL_USER": pathlib.Path('localuser.txt').read_text().strip(),
-         "PROJECT": project}
-
-    with open(template_path, "r") as f:
-        src = Template(f.read())
-        result = src.substitute(d)
-        with open(target_path, "w+") as o:
-            o.write(result)
-
-    run(["launchctl", "unload", target_path], cwd=TARGET_DIR)
-    run(["launchctl", "load", target_path], cwd=TARGET_DIR)
-
-
-def unregister_tunnel(target_path):
-    run(["launchctl", "unload", target_path], cwd=GET_LOOPHOST_DIR())
-    shutil.rmtree(target_path, ignore_errors=True)
+from io import StringIO
+import pathlib
+import shutil
+from loophost import LOOPHOST_DOMAIN, TUNNEL_DOMAIN, PYEX, HUBDIR, GET_FLINGUSER_NAME, GET_LOOPHOST_DIR
+from string import Template
+from subprocess import run
+import paramiko
+
+
+def generate_keys():
+    key = paramiko.RSAKey.generate(2048)
+    privateString = StringIO()
+    key.write_private_key(privateString)
+    return f"{key.get_name()} {key.get_base64()}", privateString.getvalue()
+
+
+def register_tunnel(project, template_path, target_path):
+    TARGET_DIR = GET_LOOPHOST_DIR()
+    shutil.copy2(template_path, TARGET_DIR)
+
+    d = {"CWD": TARGET_DIR,
+         "USERNAME": GET_FLINGUSER_NAME(),
+         "PYEX": PYEX,
+         "HUBDIR": HUBDIR,
+         "LOOPHOST_DOMAIN": LOOPHOST_DOMAIN,
+         "TUNNEL_DOMAIN": TUNNEL_DOMAIN,
+         "LOCAL_USER": pathlib.Path('localuser.txt').read_text().strip(),
+         "PROJECT": project}
+
+    with open(template_path, "r") as f:
+        src = Template(f.read())
+        result = src.substitute(d)
+        with open(target_path, "w+") as o:
+            o.write(result)
+
+    run(["launchctl", "unload", target_path], cwd=TARGET_DIR)
+    run(["launchctl", "load", target_path], cwd=TARGET_DIR)
+
+
+def unregister_tunnel(target_path):
+    run(["launchctl", "unload", target_path], cwd=GET_LOOPHOST_DIR())
+    shutil.rmtree(target_path, ignore_errors=True)
```

### Comparing `loophost-1.1.0/loophost/plist/hub.plist.template` & `loophost-1.1.2/loophost/plist/loophost.plist.template`

 * *Files 22% similar despite different names*

#### Comparing `loophost-1.1.0/loophost/plist/hub.plist.template` & `loophost-1.1.2/loophost/plist/loophost.plist.template`

```diff
@@ -1,29 +1,28 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE plist
   PUBLIC '-//Apple//DTD PLIST 1.0//EN'
   'http://www.apple.com/DTDs/PropertyList-1.0.dtd'>
 <plist version="1.0">
   <dict>
     <key>Label</key>
-    <string>dev.fling.hub</string>
+    <string>dev.fling.hub.local</string>
     <key>ProgramArguments</key>
     <array>
-      <string>${HUBDIR}/bin/loopproxy</string>
-      <string>${CWD}</string>
+      <string>${PYEX}</string>
+      <string>-m</string>
+      <string>loophost.flingroute</string>
     </array>
     <key>RunAtLoad</key>
     <true/>
     <key>KeepAlive</key>
     <true/>
     <key>WorkingDirectory</key>
     <string>${CWD}</string>
     <key>StandardInPath</key>
-    <string>/tmp/flinghub.stdin</string>
+    <string>/tmp/flingroute.stdin</string>
     <key>StandardOutPath</key>
-    <string>/tmp/flinghub.stdout</string>
+    <string>/tmp/flingroute.stdout</string>
     <key>StandardErrorPath</key>
-    <string>/tmp/flinghub.stderr</string>
-    <key>UserName</key>
-    <string>root</string>
+    <string>/tmp/flingroute.stderr</string>
   </dict>
 </plist>
```

### Comparing `loophost-1.1.0/loophost/plist/ssh.plist.template` & `loophost-1.1.2/loophost/plist/ssh.plist.template`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0a3c 2144 4f43 5459 5045  F-8"?>.<!DOCTYPE
-00000030: 2070 6c69 7374 2050 5542 4c49 4320 222d   plist PUBLIC "-
-00000040: 2f2f 4170 706c 652f 2f44 5444 2050 4c49  //Apple//DTD PLI
-00000050: 5354 2031 2e30 2f2f 454e 2220 2268 7474  ST 1.0//EN" "htt
-00000060: 703a 2f2f 7777 772e 6170 706c 652e 636f  p://www.apple.co
-00000070: 6d2f 4454 4473 2f50 726f 7065 7274 794c  m/DTDs/PropertyL
-00000080: 6973 742d 312e 302e 6474 6422 3e0a 3c70  ist-1.0.dtd">.<p
-00000090: 6c69 7374 2076 6572 7369 6f6e 3d22 312e  list version="1.
-000000a0: 3022 3e0a 3c64 6963 743e 0a20 2020 203c  0">.<dict>.    <
-000000b0: 6b65 793e 4c61 6265 6c3c 2f6b 6579 3e0a  key>Label</key>.
-000000c0: 2020 2020 3c73 7472 696e 673e 6465 762e      <string>dev.
-000000d0: 666c 696e 672e 6875 622e 7373 682e 247b  fling.hub.ssh.${
-000000e0: 5052 4f4a 4543 547d 3c2f 7374 7269 6e67  PROJECT}</string
-000000f0: 3e0a 2020 2020 3c6b 6579 3e50 726f 6772  >.    <key>Progr
-00000100: 616d 4172 6775 6d65 6e74 733c 2f6b 6579  amArguments</key
-00000110: 3e0a 2020 2020 3c61 7272 6179 3e0a 2020  >.    <array>.  
-00000120: 2020 2020 2020 3c73 7472 696e 673e 7373        <string>ss
-00000130: 683c 2f73 7472 696e 673e 0a20 2020 2020  h</string>.     
-00000140: 2020 203c 7374 7269 6e67 3e2d 6f20 5365     <string>-o Se
-00000150: 7276 6572 416c 6976 6549 6e74 6572 7661  rverAliveInterva
-00000160: 6c3d 3630 3c2f 7374 7269 6e67 3e0a 2020  l=60</string>.  
-00000170: 2020 2020 2020 3c73 7472 696e 673e 2d6f        <string>-o
-00000180: 2045 7869 744f 6e46 6f72 7761 7264 4661   ExitOnForwardFa
-00000190: 696c 7572 653d 7965 733c 2f73 7472 696e  ilure=yes</strin
-000001a0: 673e 0a20 2020 2020 2020 203c 7374 7269  g>.        <stri
-000001b0: 6e67 3e2d 6f20 5573 6572 4b6e 6f77 6e48  ng>-o UserKnownH
-000001c0: 6f73 7473 4669 6c65 3d2f 6465 762f 6e75  ostsFile=/dev/nu
-000001d0: 6c6c 3c2f 7374 7269 6e67 3e0a 2020 2020  ll</string>.    
-000001e0: 2020 2020 3c73 7472 696e 673e 2d6f 2053      <string>-o S
-000001f0: 7472 6963 7448 6f73 744b 6579 4368 6563  trictHostKeyChec
-00000200: 6b69 6e67 3d6e 6f3c 2f73 7472 696e 673e  king=no</string>
-00000210: 0a20 2020 2020 2020 203c 7374 7269 6e67  .        <string
-00000220: 3e2d 693c 2f73 7472 696e 673e 0a20 2020  >-i</string>.   
-00000230: 2020 2020 203c 7374 7269 6e67 3e24 7b43       <string>${C
-00000240: 5744 7d2f 7475 6e6e 656c 6b65 793c 2f73  WD}/tunnelkey</s
-00000250: 7472 696e 673e 0a20 2020 2020 2020 203c  tring>.        <
-00000260: 7374 7269 6e67 3e2d 7020 3232 3232 3c2f  string>-p 2222</
-00000270: 7374 7269 6e67 3e0a 2020 2020 2020 2020  string>.        
-00000280: 3c73 7472 696e 673e 2d52 2024 7b50 524f  <string>-R ${PRO
-00000290: 4a45 4354 7d3a 3434 333a 6c6f 6361 6c68  JECT}:443:localh
-000002a0: 6f73 743a 3434 3333 3c2f 7374 7269 6e67  ost:4433</string
-000002b0: 3e0a 2020 2020 2020 2020 3c73 7472 696e  >.        <strin
-000002c0: 673e 247b 5553 4552 4e41 4d45 7d40 247b  g>${USERNAME}@${
-000002d0: 5455 4e4e 454c 5f44 4f4d 4149 4e7d 3c2f  TUNNEL_DOMAIN}</
-000002e0: 7374 7269 6e67 3e0a 2020 2020 3c2f 6172  string>.    </ar
-000002f0: 7261 793e 0a20 2020 203c 6b65 793e 576f  ray>.    <key>Wo
-00000300: 726b 696e 6744 6972 6563 746f 7279 3c2f  rkingDirectory</
-00000310: 6b65 793e 0a20 2020 203c 7374 7269 6e67  key>.    <string
-00000320: 3e24 7b43 5744 7d3c 2f73 7472 696e 673e  >${CWD}</string>
-00000330: 0a20 2020 203c 6b65 793e 5573 6572 4e61  .    <key>UserNa
-00000340: 6d65 3c2f 6b65 793e 0a20 2020 203c 7374  me</key>.    <st
-00000350: 7269 6e67 3e24 7b4c 4f43 414c 5f55 5345  ring>${LOCAL_USE
-00000360: 527d 3c2f 7374 7269 6e67 3e0a 2020 2020  R}</string>.    
-00000370: 3c6b 6579 3e52 756e 4174 4c6f 6164 3c2f  <key>RunAtLoad</
-00000380: 6b65 793e 0a20 2020 203c 7472 7565 2f3e  key>.    <true/>
-00000390: 0a20 2020 203c 6b65 793e 4b65 6570 416c  .    <key>KeepAl
-000003a0: 6976 653c 2f6b 6579 3e0a 2020 2020 3c74  ive</key>.    <t
-000003b0: 7275 652f 3e0a 2020 2020 3c6b 6579 3e53  rue/>.    <key>S
-000003c0: 7461 6e64 6172 644f 7574 5061 7468 3c2f  tandardOutPath</
-000003d0: 6b65 793e 0a20 2020 203c 7374 7269 6e67  key>.    <string
-000003e0: 3e2f 746d 702f 6c6f 6f70 686f 7374 2d74  >/tmp/loophost-t
-000003f0: 756e 6e65 6c2d 247b 5052 4f4a 4543 547d  unnel-${PROJECT}
-00000400: 2e73 7464 6f75 743c 2f73 7472 696e 673e  .stdout</string>
-00000410: 0a20 2020 203c 6b65 793e 5374 616e 6461  .    <key>Standa
-00000420: 7264 4572 726f 7250 6174 683c 2f6b 6579  rdErrorPath</key
-00000430: 3e0a 2020 2020 3c73 7472 696e 673e 2f74  >.    <string>/t
-00000440: 6d70 2f6c 6f6f 7068 6f73 742d 7475 6e6e  mp/loophost-tunn
-00000450: 656c 2d24 7b50 524f 4a45 4354 7d2e 7374  el-${PROJECT}.st
-00000460: 6465 7272 3c2f 7374 7269 6e67 3e0a 3c2f  derr</string>.</
-00000470: 6469 6374 3e0a 3c2f 706c 6973 743e       dict>.</plist>
+00000020: 462d 3822 3f3e 0d0a 3c21 444f 4354 5950  F-8"?>..<!DOCTYP
+00000030: 4520 706c 6973 7420 5055 424c 4943 2022  E plist PUBLIC "
+00000040: 2d2f 2f41 7070 6c65 2f2f 4454 4420 504c  -//Apple//DTD PL
+00000050: 4953 5420 312e 302f 2f45 4e22 2022 6874  IST 1.0//EN" "ht
+00000060: 7470 3a2f 2f77 7777 2e61 7070 6c65 2e63  tp://www.apple.c
+00000070: 6f6d 2f44 5444 732f 5072 6f70 6572 7479  om/DTDs/Property
+00000080: 4c69 7374 2d31 2e30 2e64 7464 223e 0d0a  List-1.0.dtd">..
+00000090: 3c70 6c69 7374 2076 6572 7369 6f6e 3d22  <plist version="
+000000a0: 312e 3022 3e0d 0a3c 6469 6374 3e0d 0a20  1.0">..<dict>.. 
+000000b0: 2020 203c 6b65 793e 4c61 6265 6c3c 2f6b     <key>Label</k
+000000c0: 6579 3e0d 0a20 2020 203c 7374 7269 6e67  ey>..    <string
+000000d0: 3e64 6576 2e66 6c69 6e67 2e68 7562 2e73  >dev.fling.hub.s
+000000e0: 7368 2e24 7b50 524f 4a45 4354 7d3c 2f73  sh.${PROJECT}</s
+000000f0: 7472 696e 673e 0d0a 2020 2020 3c6b 6579  tring>..    <key
+00000100: 3e50 726f 6772 616d 4172 6775 6d65 6e74  >ProgramArgument
+00000110: 733c 2f6b 6579 3e0d 0a20 2020 203c 6172  s</key>..    <ar
+00000120: 7261 793e 0d0a 2020 2020 2020 2020 3c73  ray>..        <s
+00000130: 7472 696e 673e 7373 683c 2f73 7472 696e  tring>ssh</strin
+00000140: 673e 0d0a 2020 2020 2020 2020 3c73 7472  g>..        <str
+00000150: 696e 673e 2d6f 2053 6572 7665 7241 6c69  ing>-o ServerAli
+00000160: 7665 496e 7465 7276 616c 3d36 303c 2f73  veInterval=60</s
+00000170: 7472 696e 673e 0d0a 2020 2020 2020 2020  tring>..        
+00000180: 3c73 7472 696e 673e 2d6f 2045 7869 744f  <string>-o ExitO
+00000190: 6e46 6f72 7761 7264 4661 696c 7572 653d  nForwardFailure=
+000001a0: 7965 733c 2f73 7472 696e 673e 0d0a 2020  yes</string>..  
+000001b0: 2020 2020 2020 3c73 7472 696e 673e 2d6f        <string>-o
+000001c0: 2055 7365 724b 6e6f 776e 486f 7374 7346   UserKnownHostsF
+000001d0: 696c 653d 2f64 6576 2f6e 756c 6c3c 2f73  ile=/dev/null</s
+000001e0: 7472 696e 673e 0d0a 2020 2020 2020 2020  tring>..        
+000001f0: 3c73 7472 696e 673e 2d6f 2053 7472 6963  <string>-o Stric
+00000200: 7448 6f73 744b 6579 4368 6563 6b69 6e67  tHostKeyChecking
+00000210: 3d6e 6f3c 2f73 7472 696e 673e 0d0a 2020  =no</string>..  
+00000220: 2020 2020 2020 3c73 7472 696e 673e 2d69        <string>-i
+00000230: 3c2f 7374 7269 6e67 3e0d 0a20 2020 2020  </string>..     
+00000240: 2020 203c 7374 7269 6e67 3e24 7b43 5744     <string>${CWD
+00000250: 7d2f 7475 6e6e 656c 6b65 793c 2f73 7472  }/tunnelkey</str
+00000260: 696e 673e 0d0a 2020 2020 2020 2020 3c73  ing>..        <s
+00000270: 7472 696e 673e 2d70 2032 3232 323c 2f73  tring>-p 2222</s
+00000280: 7472 696e 673e 0d0a 2020 2020 2020 2020  tring>..        
+00000290: 3c73 7472 696e 673e 2d52 2024 7b50 524f  <string>-R ${PRO
+000002a0: 4a45 4354 7d3a 3434 333a 6c6f 6361 6c68  JECT}:443:localh
+000002b0: 6f73 743a 3434 3333 3c2f 7374 7269 6e67  ost:4433</string
+000002c0: 3e0d 0a20 2020 2020 2020 203c 7374 7269  >..        <stri
+000002d0: 6e67 3e24 7b55 5345 524e 414d 457d 4024  ng>${USERNAME}@$
+000002e0: 7b54 554e 4e45 4c5f 444f 4d41 494e 7d3c  {TUNNEL_DOMAIN}<
+000002f0: 2f73 7472 696e 673e 0d0a 2020 2020 3c2f  /string>..    </
+00000300: 6172 7261 793e 0d0a 2020 2020 3c6b 6579  array>..    <key
+00000310: 3e57 6f72 6b69 6e67 4469 7265 6374 6f72  >WorkingDirector
+00000320: 793c 2f6b 6579 3e0d 0a20 2020 203c 7374  y</key>..    <st
+00000330: 7269 6e67 3e24 7b43 5744 7d3c 2f73 7472  ring>${CWD}</str
+00000340: 696e 673e 0d0a 2020 2020 3c6b 6579 3e55  ing>..    <key>U
+00000350: 7365 724e 616d 653c 2f6b 6579 3e0d 0a20  serName</key>.. 
+00000360: 2020 203c 7374 7269 6e67 3e24 7b4c 4f43     <string>${LOC
+00000370: 414c 5f55 5345 527d 3c2f 7374 7269 6e67  AL_USER}</string
+00000380: 3e0d 0a20 2020 203c 6b65 793e 5275 6e41  >..    <key>RunA
+00000390: 744c 6f61 643c 2f6b 6579 3e0d 0a20 2020  tLoad</key>..   
+000003a0: 203c 7472 7565 2f3e 0d0a 2020 2020 3c6b   <true/>..    <k
+000003b0: 6579 3e4b 6565 7041 6c69 7665 3c2f 6b65  ey>KeepAlive</ke
+000003c0: 793e 0d0a 2020 2020 3c74 7275 652f 3e0d  y>..    <true/>.
+000003d0: 0a20 2020 203c 6b65 793e 5374 616e 6461  .    <key>Standa
+000003e0: 7264 4f75 7450 6174 683c 2f6b 6579 3e0d  rdOutPath</key>.
+000003f0: 0a20 2020 203c 7374 7269 6e67 3e2f 746d  .    <string>/tm
+00000400: 702f 6c6f 6f70 686f 7374 2d74 756e 6e65  p/loophost-tunne
+00000410: 6c2d 247b 5052 4f4a 4543 547d 2e73 7464  l-${PROJECT}.std
+00000420: 6f75 743c 2f73 7472 696e 673e 0d0a 2020  out</string>..  
+00000430: 2020 3c6b 6579 3e53 7461 6e64 6172 6445    <key>StandardE
+00000440: 7272 6f72 5061 7468 3c2f 6b65 793e 0d0a  rrorPath</key>..
+00000450: 2020 2020 3c73 7472 696e 673e 2f74 6d70      <string>/tmp
+00000460: 2f6c 6f6f 7068 6f73 742d 7475 6e6e 656c  /loophost-tunnel
+00000470: 2d24 7b50 524f 4a45 4354 7d2e 7374 6465  -${PROJECT}.stde
+00000480: 7272 3c2f 7374 7269 6e67 3e0d 0a3c 2f64  rr</string>..</d
+00000490: 6963 743e 0d0a 3c2f 706c 6973 743e       ict>..</plist>
```

### Comparing `loophost-1.1.0/loophost/static/fling-logo-dark.png` & `loophost-1.1.2/loophost/static/fling-logo-dark.png`

 * *Files identical despite different names*

### Comparing `loophost-1.1.0/loophost/static/fling-logo-light.png` & `loophost-1.1.2/loophost/static/fling-logo-light.png`

 * *Files identical despite different names*

### Comparing `loophost-1.1.0/loophost/static/github-mark.png` & `loophost-1.1.2/loophost/static/github-mark.png`

 * *Files identical despite different names*

### Comparing `loophost-1.1.0/loophost/static/logo-hc.txt` & `loophost-1.1.2/loophost/static/logo-hc.txt`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
-                                                                                                                     
-                                               ,╓φφδ▒▒⌐             ,                                                   
-            ,╔φ▒▒╠▒╠▒▒φ≥╓,                   φ╠▒▒▒▒▒▒▒ε ]▒▒▒▒▒   ,╠▒▒▒╠─                                                
-        ,φ╠▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒╠φ╓              .╠▒▒▒▒▒╚╙╙╙⌐ ]▒▒▒▒▒   ╘▒▒▒▒▒∩                                                
-      .ê▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒╠╓            ╠▒▒▒▒╙       ]▒▒▒▒▒    ^╙╙╙`                                                 
-     ,╠▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒╦           ▒▒▒▒▒╓,,,,   ]▒▒▒▒▒    ╔╔╔╔╔         ,╔╔φφ╔≥╓,           ,╔╔φφφ╔╔╓ ,╓╔╔╔⌐    
-     ╠▒▒▒╠╙,  `╚▒▒▒▒▒╚└,  "╠▒▒▒▒░          ▒▒▒▒▒▒▒▒▒▒   ]▒▒▒▒▒   '▒▒▒▒▒      ╓▒▒▒▒▒▒▒▒▒▒▒▒φ,     «δ▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒ε    
-    ╔▒▒▒▒░╠▒▒ε  ╚▒▒▒╠╔▒▒╠   ╠▒▒▒╠          ▒▒▒▒▒▒▒▒▒▒   :▒▒▒▒▒   '▒▒▒▒▒     δ▒▒▒▒▒╚╙╙╙╚▒▒▒▒▒╔   φ▒▒▒▒▒╚╙╙╙╚╠▒▒▒▒▒╙"     
-    ╠▒▒▒▒╖╙╙╙  ,╠▒▒▒▒░╙╙╙  ;▒▒▒▒▒          ▒▒▒▒▒⌐       ]▒▒▒▒▒   '▒▒▒▒▒    ╔▒▒▒▒╚      "▒▒▒▒▒⌐ '▒▒▒▒▒⌐      ╚▒▒▒▒ε      
-    ╚▒▒▒▒▒╠φ╔φδ▒▒▒▒▒▒▒▒φ╔φ╠▒▒▒▒▒▒          ▒▒▒▒▒⌐       ]▒▒▒▒▒   '▒▒▒▒▒    ╠▒▒▒▒░       ╚▒▒▒▒Γ  ╠▒▒▒▒╦,, ,,╔▒▒▒▒▒⌐      
-     ╠▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒Γ          ▒▒▒▒▒⌐       ]▒▒▒▒▒   '▒▒▒▒▒    ▒▒▒▒▒░       ╚▒▒▒▒Γ  '╚▒▒▒▒▒▒▒▒▒▒▒▒▒╚└       
-     "╠▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒╙           ▒▒▒▒▒⌐       ]▒▒▒▒▒   '▒▒▒▒▒    ▒▒▒▒▒░       ╚▒▒▒▒Γ    ^╙╚╚▒▒▒▒▒▒╚╙`         
-       ╚▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒╚└            ▒▒▒▒▒⌐       ]▒▒▒▒▒   '▒▒▒▒▒    ▒▒▒▒▒░       ╚▒▒▒▒Γ        ╚▒▒▒▒             
-         └╙╚╠▒▒╚╚╠▒▒╚╚╠▒╠╚╚╙               ╚╚╚╚╚⌐       ^╚╚╚╚╚    ╚╚╚╚╚    ╚╚╚╚╚⌐       ╚╚╚╚╚┘     ²φ╠▒▒▒▒▒▒▒╔          
-            ╠▒▒¬ ╠▒▒ε ╠▒▒⌐                                                                        ╠▒▒▒▒╙╙╙╠▒▒▒▒~        
-            ╠▒╚  ╚▒╠  ╚▒╠⌐                                                                        ▒▒▒▒▒   ╓▒▒▒▒⌂        
-                                                                                                  └╠▒▒▒▒▒▒▒▒▒▒╙         
-                                                                                                    ^╙╙╚╚╚╚╙└           
-
+
+                                                                                                                     
+                                               ,╓φφδ▒▒⌐             ,                                                   
+            ,╔φ▒▒╠▒╠▒▒φ≥╓,                   φ╠▒▒▒▒▒▒▒ε ]▒▒▒▒▒   ,╠▒▒▒╠─                                                
+        ,φ╠▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒╠φ╓              .╠▒▒▒▒▒╚╙╙╙⌐ ]▒▒▒▒▒   ╘▒▒▒▒▒∩                                                
+      .ê▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒╠╓            ╠▒▒▒▒╙       ]▒▒▒▒▒    ^╙╙╙`                                                 
+     ,╠▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒╦           ▒▒▒▒▒╓,,,,   ]▒▒▒▒▒    ╔╔╔╔╔         ,╔╔φφ╔≥╓,           ,╔╔φφφ╔╔╓ ,╓╔╔╔⌐    
+     ╠▒▒▒╠╙,  `╚▒▒▒▒▒╚└,  "╠▒▒▒▒░          ▒▒▒▒▒▒▒▒▒▒   ]▒▒▒▒▒   '▒▒▒▒▒      ╓▒▒▒▒▒▒▒▒▒▒▒▒φ,     «δ▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒ε    
+    ╔▒▒▒▒░╠▒▒ε  ╚▒▒▒╠╔▒▒╠   ╠▒▒▒╠          ▒▒▒▒▒▒▒▒▒▒   :▒▒▒▒▒   '▒▒▒▒▒     δ▒▒▒▒▒╚╙╙╙╚▒▒▒▒▒╔   φ▒▒▒▒▒╚╙╙╙╚╠▒▒▒▒▒╙"     
+    ╠▒▒▒▒╖╙╙╙  ,╠▒▒▒▒░╙╙╙  ;▒▒▒▒▒          ▒▒▒▒▒⌐       ]▒▒▒▒▒   '▒▒▒▒▒    ╔▒▒▒▒╚      "▒▒▒▒▒⌐ '▒▒▒▒▒⌐      ╚▒▒▒▒ε      
+    ╚▒▒▒▒▒╠φ╔φδ▒▒▒▒▒▒▒▒φ╔φ╠▒▒▒▒▒▒          ▒▒▒▒▒⌐       ]▒▒▒▒▒   '▒▒▒▒▒    ╠▒▒▒▒░       ╚▒▒▒▒Γ  ╠▒▒▒▒╦,, ,,╔▒▒▒▒▒⌐      
+     ╠▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒Γ          ▒▒▒▒▒⌐       ]▒▒▒▒▒   '▒▒▒▒▒    ▒▒▒▒▒░       ╚▒▒▒▒Γ  '╚▒▒▒▒▒▒▒▒▒▒▒▒▒╚└       
+     "╠▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒╙           ▒▒▒▒▒⌐       ]▒▒▒▒▒   '▒▒▒▒▒    ▒▒▒▒▒░       ╚▒▒▒▒Γ    ^╙╚╚▒▒▒▒▒▒╚╙`         
+       ╚▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒╚└            ▒▒▒▒▒⌐       ]▒▒▒▒▒   '▒▒▒▒▒    ▒▒▒▒▒░       ╚▒▒▒▒Γ        ╚▒▒▒▒             
+         └╙╚╠▒▒╚╚╠▒▒╚╚╠▒╠╚╚╙               ╚╚╚╚╚⌐       ^╚╚╚╚╚    ╚╚╚╚╚    ╚╚╚╚╚⌐       ╚╚╚╚╚┘     ²φ╠▒▒▒▒▒▒▒╔          
+            ╠▒▒¬ ╠▒▒ε ╠▒▒⌐                                                                        ╠▒▒▒▒╙╙╙╠▒▒▒▒~        
+            ╠▒╚  ╚▒╠  ╚▒╠⌐                                                                        ▒▒▒▒▒   ╓▒▒▒▒⌂        
+                                                                                                  └╠▒▒▒▒▒▒▒▒▒▒╙         
+                                                                                                    ^╙╙╚╚╚╚╙└           
+
```

### Comparing `loophost-1.1.0/loophost/static/logo-square.png` & `loophost-1.1.2/loophost/static/logo-square.png`

 * *Files identical despite different names*

### Comparing `loophost-1.1.0/loophost/templates/local.html` & `loophost-1.1.2/loophost/templates/local.html`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-{% extends "base.html" %}
-{% block headline %}
-<h1>Configuration for "{{project}}"</h1>
-{% endblock%}
-
-{% block content %}
-{{ super() }}
-<main>
-
-  <div class="container px-5 mt-2 mb-5 font-monospace">
-
-    <form method="post" action="/config/{{project}}" id="config_form">
-      <script>
-        const action_submit = (action) => {
-          document.getElementById('form_action').value = action;
-          document.getElementById('config_form').submit();
-        }
-      </script>
-      <input type="hidden" name="action" id="form_action" />
-      <input type="hidden" name="csrf_token" value="{{ csrf_token() }}"/>
-
-{% if project in apps %}
-
-<h3>
-Loophost address: <a href="https://{{project}}.{{config['fqdn']}}">https://{{project}}.{{config['fqdn']}}</a></h3>
-<h3>
-Public address: 
-{% if project in share %} 
-        <a href="https://{{project}}.{{config["tunnel"]}}">https://{{project}}.{{config["tunnel"]}}</a> 
-{% else %} 
-        {% if config["tunnel"] %}
-                <a onclick="action_submit('share')" href="#">(disabled)</a>
-        
-        {% else %}
-                <a href="https://loophost.dev/upgrade.html">(disabled)</a>
-        {% endif %} 
-{% endif %}</h3>
-
-      {% else %}
-      <h3>Configure your new app:</h3>
-  {% endif %}
-<br/>
-
-<div class="row">
-  <div class="col col-7">
-          App Address: <input type="text" size="30" name="application_port" value="{{config['apps'].get(project, '')}}" />
-          <input type="submit" class="btn btn-primary" name="add_application" value="{% if project in apps %}Update{% else %}Add{% endif %} this app" />
-  </div>
-  <div class="col">
-          <p>Your application can run on a local network port, or a unix domain socket.</p>
-          <p>If it's running on a network port, make sure the address above starts with <b>the full http://localhost</b>, for example
-          http://localhost:8000.</p>
-          <p>If you're using a unix socket (which is much faster), use the full path to the socket (including a starting /). 
-          For example, /tmp/myapp.soc.</p><br/>
-  </div>     
-<div>
-
-{% if project in apps %} 
-<div class="row">
-  <div class="col col-lg-7">
-<a class="btn btn-primary" onclick="action_submit('share')" href="#">{% if project in share %}Disable public sharing{% else %}Enable public sharing{% endif %}</a>
-</div>
-  <div class="col">
-    <p>Public sharing will open up a remote tunnel that allows other people in the world to visit your application, at a dedicated address.</p>
-  </div>
-</div>
-
-<div class="row pb-3">
-  <div class="col col-lg-7">
-    <a class="btn btn-danger"  onclick="action_submit('unbind')" href="#">Unbind this project</a>
-  </div>
-  <div class="col">
-    <p>This will remove this app from loophost entirely, and disconnect any shared tunnels as well.</p>
-  </div>
-</div>
-
-<h4><a href="/">&lt;- Back to application list</a></h4>
-
-{% endif %}
-
-<br/>
-      
-    </form>
-    </div>
-  </main>
-{% endblock %}
+{% extends "base.html" %}
+{% block headline %}
+<h1>Configuration for "{{project}}"</h1>
+{% endblock%}
+
+{% block content %}
+{{ super() }}
+<main>
+
+  <div class="container px-5 mt-2 mb-5 font-monospace">
+
+    <form method="post" action="/config/{{project}}" id="config_form">
+      <script>
+        const action_submit = (action) => {
+          document.getElementById('form_action').value = action;
+          document.getElementById('config_form').submit();
+        }
+      </script>
+      <input type="hidden" name="action" id="form_action" />
+      <input type="hidden" name="csrf_token" value="{{ csrf_token() }}"/>
+
+{% if project in apps %}
+
+<h3>
+Loophost address: <a href="https://{{project}}.{{config['fqdn']}}">https://{{project}}.{{config['fqdn']}}</a></h3>
+<h3>
+Public address: 
+{% if project in share %} 
+        <a href="https://{{project}}.{{config["tunnel"]}}">https://{{project}}.{{config["tunnel"]}}</a> 
+{% else %} 
+        {% if config["tunnel"] %}
+                <a onclick="action_submit('share')" href="#">(disabled)</a>
+        
+        {% else %}
+                <a href="https://loophost.dev/upgrade.html">(disabled)</a>
+        {% endif %} 
+{% endif %}</h3>
+
+      {% else %}
+      <h3>Configure your new app:</h3>
+  {% endif %}
+<br/>
+
+<div class="row">
+  <div class="col col-7">
+          App Address: <input type="text" size="30" name="application_port" value="{{config['apps'].get(project, '')}}" />
+          <input type="submit" class="btn btn-primary" name="add_application" value="{% if project in apps %}Update{% else %}Add{% endif %} this app" />
+  </div>
+  <div class="col">
+          <p>Your application can run on a local network port, or a unix domain socket.</p>
+          <p>If it's running on a network port, make sure the address above starts with <b>the full http://localhost</b>, for example
+          http://localhost:8000.</p>
+          <p>If you're using a unix socket (which is much faster), use the full path to the socket (including a starting /). 
+          For example, /tmp/myapp.soc.</p><br/>
+  </div>     
+<div>
+
+{% if project in apps %} 
+<div class="row">
+  <div class="col col-lg-7">
+<a class="btn btn-primary" onclick="action_submit('share')" href="#">{% if project in share %}Disable public sharing{% else %}Enable public sharing{% endif %}</a>
+</div>
+  <div class="col">
+    <p>Public sharing will open up a remote tunnel that allows other people in the world to visit your application, at a dedicated address.</p>
+  </div>
+</div>
+
+<div class="row pb-3">
+  <div class="col col-lg-7">
+    <a class="btn btn-danger"  onclick="action_submit('unbind')" href="#">Unbind this project</a>
+  </div>
+  <div class="col">
+    <p>This will remove this app from loophost entirely, and disconnect any shared tunnels as well.</p>
+  </div>
+</div>
+
+<h4><a href="/">&lt;- Back to application list</a></h4>
+
+{% endif %}
+
+<br/>
+      
+    </form>
+    </div>
+  </main>
+{% endblock %}
```

### Comparing `loophost-1.1.0/loophost/templates/start/base.html` & `loophost-1.1.2/loophost/templates/start/base.html`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-<!DOCTYPE html>
-<!--[if lt IE 7]>      <html class="no-js lt-ie9 lt-ie8 lt-ie7"> <![endif]-->
-<!--[if IE 7]>         <html class="no-js lt-ie9 lt-ie8"> <![endif]-->
-<!--[if IE 8]>         <html class="no-js lt-ie9"> <![endif]-->
-<!--[if gt IE 8]>      <html class="no-js"> <!--<![endif]-->
-<html class="h-100">
-    <head>
-        {% block head %}
-        <!-- Required meta tags -->
-        <meta charset="utf-8">
-        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
-        <meta http-equiv="X-UA-Compatible" content="IE=edge">
-        <link rel="shortcut icon" href="{{ url_for('static', filename='favicon.ico') }}">
-        <title>{% block title %}Beautiful loading screen{% endblock %}</title>
-        <meta name="description" content="">
-        {% block styles %}
-        <link href="{{url_for('static', filename='start/styles.css')}}" rel="stylesheet">
-            <!-- Bootstrap CSS -->
-            {{ bootstrap.load_css() }}
-        {% endblock %}
-        {% endblock %}
-    </head>
-    {% block body %}
-    <body class="d-flex flex-column h-100">
-        <div id="maincontent">
-        <!--[if lt IE 7]>
-            <p class="browsehappy">You are using an <strong>outdated</strong> browser. Please <a href="#">upgrade your browser</a> to improve your experience.</p>
-        <![endif]-->
-            {% block content %}
-
-            {% endblock %}
-        </div>
-        {% block scripts %}
-            <!-- Optional JavaScript -->
-            {{ bootstrap.load_js() }}
-            <script defer data-domain="{{ domain_name|default('start.fling.wtf')}}" src="https://plausible.io/js/script.js"></script>
-            
-        {% endblock %}
-    </body>
-    {% endblock %}
+<!DOCTYPE html>
+<!--[if lt IE 7]>      <html class="no-js lt-ie9 lt-ie8 lt-ie7"> <![endif]-->
+<!--[if IE 7]>         <html class="no-js lt-ie9 lt-ie8"> <![endif]-->
+<!--[if IE 8]>         <html class="no-js lt-ie9"> <![endif]-->
+<!--[if gt IE 8]>      <html class="no-js"> <!--<![endif]-->
+<html class="h-100">
+    <head>
+        {% block head %}
+        <!-- Required meta tags -->
+        <meta charset="utf-8">
+        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
+        <meta http-equiv="X-UA-Compatible" content="IE=edge">
+        <link rel="shortcut icon" href="{{ url_for('static', filename='favicon.ico') }}">
+        <title>{% block title %}Beautiful loading screen{% endblock %}</title>
+        <meta name="description" content="">
+        {% block styles %}
+        <link href="{{url_for('static', filename='start/styles.css')}}" rel="stylesheet">
+            <!-- Bootstrap CSS -->
+            {{ bootstrap.load_css() }}
+        {% endblock %}
+        {% endblock %}
+    </head>
+    {% block body %}
+    <body class="d-flex flex-column h-100">
+        <div id="maincontent">
+        <!--[if lt IE 7]>
+            <p class="browsehappy">You are using an <strong>outdated</strong> browser. Please <a href="#">upgrade your browser</a> to improve your experience.</p>
+        <![endif]-->
+            {% block content %}
+
+            {% endblock %}
+        </div>
+        {% block scripts %}
+            <!-- Optional JavaScript -->
+            {{ bootstrap.load_js() }}
+            <script defer data-domain="{{ domain_name|default('start.fling.wtf')}}" src="https://plausible.io/js/script.js"></script>
+            
+        {% endblock %}
+    </body>
+    {% endblock %}
 </html>
```

### Comparing `loophost-1.1.0/loophost/uninstall.py` & `loophost-1.1.2/loophost/uninstall.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import os
-from pathlib import Path
-import shutil
-from subprocess import run
-import subprocess
-import sys
-from loophost import GET_LOOPHOST_DIR, GET_FLINGUSER_NAME
-
-
-def uninstall_one():
-    if not os.path.exists(Path("localuser.txt")):
-        print("Seems to have already been uninstalled")
-        exit(0)
-    LOCAL_USER = Path("localuser.txt").read_text().strip()
-    for service in Path("/Users", LOCAL_USER, "Library", "LaunchAgents").glob(
-        "dev.fling.hub*"
-    ):
-        run(["launchctl", "unload", service], cwd=GET_LOOPHOST_DIR())
-        os.unlink(service)
-    os.chdir(Path("/Users", LOCAL_USER))
-    restart_as_sudo()
-
-
-def uninstall_two():
-    for service in Path("/Library", "LaunchDaemons").glob("dev.fling.hub*"):
-        run(["launchctl", "unload", service], cwd=GET_LOOPHOST_DIR())
-        os.unlink(service)
-    # shutil.rmtree(TARGET_DIR)
-    # os.makedirs(TARGET_DIR, exist_ok=True)
-    # with open(Path(TARGET_DIR, "flinguser.txt"), "w+") as userfile:
-    #     userfile.write(GET_FLINGUSER_NAME())
-
-
-def restart_as_sudo():
-    print(
-        """Switching to root user to uninstall web services \n\n
-        (you will be prompted for your password)"""
-    )
-    run(
-        "sudo python3 -m loophost.uninstall",
-        shell=True,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        stdin=subprocess.PIPE
-    )
-    print("Uninstall finished.")
-    run("""/usr/bin/open "https://loophost.dev/exit_survey.html" """, shell=True)
-    sys.exit()
-
-
-if __name__ == "__main__":
-    # TODO: Make this impotent and reentrant safe
-    if os.geteuid() == 0:
-        uninstall_two()
-    else:
-        uninstall_one()
+import os
+from pathlib import Path
+import shutil
+from subprocess import run
+import subprocess
+import sys
+from loophost import GET_LOOPHOST_DIR, GET_FLINGUSER_NAME
+
+
+def uninstall_one():
+    if not os.path.exists(Path("localuser.txt")):
+        print("Seems to have already been uninstalled")
+        exit(0)
+    LOCAL_USER = Path("localuser.txt").read_text().strip()
+    for service in Path("/Users", LOCAL_USER, "Library", "LaunchAgents").glob(
+        "dev.fling.hub*"
+    ):
+        run(["launchctl", "unload", service], cwd=GET_LOOPHOST_DIR())
+        os.unlink(service)
+    os.chdir(Path("/Users", LOCAL_USER))
+    restart_as_sudo()
+
+
+def uninstall_two():
+    for service in Path("/Library", "LaunchDaemons").glob("dev.fling.hub*"):
+        run(["launchctl", "unload", service], cwd=GET_LOOPHOST_DIR())
+        os.unlink(service)
+    # shutil.rmtree(TARGET_DIR)
+    # os.makedirs(TARGET_DIR, exist_ok=True)
+    # with open(Path(TARGET_DIR, "flinguser.txt"), "w+") as userfile:
+    #     userfile.write(GET_FLINGUSER_NAME())
+
+
+def restart_as_sudo():
+    print(
+        """Switching to root user to uninstall web services \n\n
+        (you will be prompted for your password)"""
+    )
+    run(
+        "sudo python3 -m loophost.uninstall",
+        shell=True,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        stdin=subprocess.PIPE
+    )
+    print("Uninstall finished.")
+    run("""/usr/bin/open "https://loophost.dev/exit_survey.html" """, shell=True)
+    sys.exit()
+
+
+if __name__ == "__main__":
+    # TODO: Make this impotent and reentrant safe
+    if os.geteuid() == 0:
+        uninstall_two()
+    else:
+        uninstall_one()
```

### Comparing `loophost-1.1.0/loophost/win/build.txt` & `loophost-1.1.2/loophost/win/build.txt`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Notes for the windows build and installer
-
-cd C:\Users\joshuamckenty\.pyenv\pyenv-win\versions\3.10.5
-python Scripts/pywin32_postinstall.py -install
-
-cd C:\Users\joshuamckenty\projects\loophost\client
-pyinstaller --onefile --hidden-import win32timezone loophost\win_hub.py
-FOR /F %i IN ('python -c "import os; import win32service; print(os.path.dirname(win32service.__file__) + '\lib')"') DO set pywinpath=%i
-copy dist\win_hub.exe %pywinpath%\
-
+# Notes for the windows build and installer
+
+cd C:\Users\joshuamckenty\.pyenv\pyenv-win\versions\3.10.5
+python Scripts/pywin32_postinstall.py -install
+
+cd C:\Users\joshuamckenty\projects\loophost\client
+pyinstaller --onefile --hidden-import win32timezone loophost\win_hub.py
+FOR /F %i IN ('python -c "import os; import win32service; print(os.path.dirname(win32service.__file__) + '\lib')"') DO set pywinpath=%i
+copy dist\win_hub.exe %pywinpath%\
+
 // Get-Process -Id (Get-NetTCPConnection -LocalPort 443).OwningProcess
```

### Comparing `loophost-1.1.0/loophost/win_hub.py` & `loophost-1.1.2/loophost/win_lp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,87 @@
-import os
-import pathlib
-import sys
-import threading
-import win32serviceutil
-import win32service
-import win32event
-import servicemanager
-import socket
-import time
-import logging
-import concurrent.futures
-from loophost.flingroute import admin
-from loophost import GET_LOOPHOST_DIR
-
-os.chdir(GET_LOOPHOST_DIR())
-
-logging.basicConfig(
-    filename = 'c:\\Users\\Public\\.loophost\\loophost-hub.log',
-    level = logging.DEBUG, 
-    format = '[loophost-service] %(levelname)-7.7s %(message)s'
-)
-
-logging.debug("Loaded WinHub script")
-
-class workingthread(threading.Thread):
-    def __init__(self, quitEvent):
-        self.quitEvent = quitEvent
-        self.waitTime = 1
-        threading.Thread.__init__(self)
-
-    def run(self):
-        try:
-            # Running start_flask() function on different thread, so that it doesn't blocks the code
-            executor = concurrent.futures.ThreadPoolExecutor(max_workers=5)
-            executor.submit(self.start_flask)
-        except:
-            pass
-
-        # Following Lines are written so that, the program doesn't get quit
-        # Will Run a Endless While Loop till Stop signal is not received from Windows Service API
-        while not self.quitEvent.isSet():  # If stop signal is triggered, exit
-            time.sleep(1)
-
-    def start_flask(self):
-        logging.debug("Starting the web interface on port 5816")
-        admin.run(host="0.0.0.0", port=5816)
-
-
-
-class LoophostHubService (win32serviceutil.ServiceFramework):
-    _svc_name_ = "LoophostHub-Service"
-    _svc_display_name_ = "LoophostHub Service"
-    _svc_description_ = "Web interface for configuring loophost"
-    
-    def __init__(self,args):
-        logging.debug("Inside the Loophost HubService service")
-        socket.setdefaulttimeout(60)
-        win32serviceutil.ServiceFramework.__init__(self, args)
-        self.hWaitStop = threading.Event()
-        self.thread = workingthread(self.hWaitStop)
-
-    def SvcStop(self):
-        self.ReportServiceStatus(win32service.SERVICE_STOP_PENDING)
-        self.hWaitStop.set()
-
-    def SvcDoRun(self):
-        self.thread.start()
-        self.hWaitStop.wait()
-        self.thread.join()
-
-
-if __name__ == '__main__':
-    if len(sys.argv) < 2:
-        servicemanager.Initialize()
-        servicemanager.PrepareToHostSingle(LoophostHubService)
-        servicemanager.StartServiceCtrlDispatcher()
-    else:
-        win32serviceutil.HandleCommandLine(LoophostHubService)
+import os
+from subprocess import run
+import sys
+import threading
+import win32serviceutil
+import win32service
+# import win32event
+import servicemanager
+import socket
+import time
+import logging
+import concurrent.futures
+from loophost import GET_LOOPHOST_DIR, HUBDIR
+
+os.chdir(GET_LOOPHOST_DIR())
+
+
+logging.basicConfig(
+    filename="c:\\Users\\Public\\.loophost\\loophost-goproxy-service.log",
+    level=logging.DEBUG,
+    format="[loophost-service] %(levelname)-7.7s %(message)s",
+)
+
+
+class workingthread(threading.Thread):
+    def __init__(self, quitEvent):
+        self.quitEvent = quitEvent
+        self.waitTime = 1
+        threading.Thread.__init__(self)
+
+    def run(self):
+        try:
+            # Running start_flask() function on different thread, so that it doesn't blocks the code
+            executor = concurrent.futures.ThreadPoolExecutor(max_workers=5)
+            executor.submit(self.start_flask)
+        except Exception as e:
+            print(e)
+
+        # Following Lines are written so that, the program doesn't get quit
+        # Will Run a Endless While Loop till Stop signal is not received from Windows Service API
+        while not self.quitEvent.isSet():  # If stop signal is triggered, exit
+            time.sleep(1)
+
+    def start_flask(self):
+        cmd = "bin\\loopproxy.exe /Users/Public/.loophost"
+        run(
+            cmd,
+            shell=True,
+            # stdout=subprocess.PIPE,
+            # stderr=subprocess.PIPE,
+            # stdin=subprocess.PIPE,
+            cwd=HUBDIR,
+            check=True,
+        )
+
+
+class LoopProxyService(win32serviceutil.ServiceFramework):
+    _svc_name_ = "LoopProxy-Service"
+    _svc_display_name_ = "LoopProxy Service"
+    _svc_description_ = "This is my service"
+    # _exe_name_ = "loopproxy-service.exe"
+
+    def __init__(self, args):
+        socket.setdefaulttimeout(60)
+        win32serviceutil.ServiceFramework.__init__(self, args)
+        self.hWaitStop = threading.Event()
+        self.thread = workingthread(self.hWaitStop)
+
+    def SvcStop(self):
+        self.ReportServiceStatus(win32service.SERVICE_STOP_PENDING)
+        self.hWaitStop.set()
+
+    def SvcDoRun(self):
+        self.thread.start()
+        self.hWaitStop.wait()
+        self.thread.join()
+
+
+if __name__ == "__main__":
+    print(f"Got {len(sys.argv)} arguments")
+    if len(sys.argv) < 2:
+        print("")
+        servicemanager.Initialize()
+        servicemanager.PrepareToHostSingle(LoopProxyService)
+        servicemanager.StartServiceCtrlDispatcher()
+    else:
+        win32serviceutil.HandleCommandLine(LoopProxyService)
```

### Comparing `loophost-1.1.0/PKG-INFO` & `loophost-1.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loophost
-Version: 1.1.0
+Version: 1.1.2
 Summary: Loophost: for a better local dev
 License: Apache-2.0
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

