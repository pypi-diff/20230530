# Comparing `tmp/multikeyjwt-1.0.0.tar.gz` & `tmp/multikeyjwt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multikeyjwt-1.0.0.tar", max compression
+gzip compressed data, was "multikeyjwt-1.1.0.tar", max compression
```

## Comparing `multikeyjwt-1.0.0.tar` & `multikeyjwt-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-05-29 13:16:14.231452 multikeyjwt-1.0.0/LICENSE
--rw-r--r--   0        0        0     3072 2023-05-29 20:28:56.570713 multikeyjwt-1.0.0/README.rst
--rw-r--r--   0        0        0     1966 2023-05-30 05:15:16.324207 multikeyjwt-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      273 2023-05-30 05:15:16.324572 multikeyjwt-1.0.0/src/multikeyjwt/__init__.py
--rw-r--r--   0        0        0     2482 2023-05-29 21:00:03.225700 multikeyjwt-1.0.0/src/multikeyjwt/config.py
--rw-r--r--   0        0        0      700 2023-05-29 13:17:05.492533 multikeyjwt-1.0.0/src/multikeyjwt/console.py
--rw-r--r--   0        0        0       25 2023-05-29 17:53:07.186037 multikeyjwt-1.0.0/src/multikeyjwt/jwt/__init__.py
--rw-r--r--   0        0        0      852 2023-05-29 20:27:36.579042 multikeyjwt-1.0.0/src/multikeyjwt/jwt/common.py
--rw-r--r--   0        0        0     2522 2023-05-30 06:11:54.955482 multikeyjwt-1.0.0/src/multikeyjwt/jwt/issuer.py
--rw-r--r--   0        0        0     2659 2023-05-29 20:28:56.589049 multikeyjwt-1.0.0/src/multikeyjwt/jwt/verifier.py
--rw-r--r--   0        0        0      114 2023-05-30 05:14:23.983577 multikeyjwt-1.0.0/src/multikeyjwt/middleware/__init__.py
--rw-r--r--   0        0        0     1809 2023-05-30 04:10:07.248745 multikeyjwt-1.0.0/src/multikeyjwt/middleware/jwtbearer.py
--rw-r--r--   0        0        0        0 2023-05-29 13:13:11.057378 multikeyjwt-1.0.0/src/multikeyjwt/py.typed
--rw-r--r--   0        0        0     4311 1970-01-01 00:00:00.000000 multikeyjwt-1.0.0/setup.py
--rw-r--r--   0        0        0     4042 1970-01-01 00:00:00.000000 multikeyjwt-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-29 13:16:14.231452 multikeyjwt-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3072 2023-05-29 20:28:56.570713 multikeyjwt-1.1.0/README.rst
+-rw-r--r--   0        0        0     1966 2023-05-30 17:05:33.004719 multikeyjwt-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      273 2023-05-30 17:05:33.005035 multikeyjwt-1.1.0/src/multikeyjwt/__init__.py
+-rw-r--r--   0        0        0     2482 2023-05-29 21:00:03.225700 multikeyjwt-1.1.0/src/multikeyjwt/config.py
+-rw-r--r--   0        0        0     3750 2023-05-30 17:05:33.005340 multikeyjwt-1.1.0/src/multikeyjwt/console.py
+-rw-r--r--   0        0        0       25 2023-05-29 17:53:07.186037 multikeyjwt-1.1.0/src/multikeyjwt/jwt/__init__.py
+-rw-r--r--   0        0        0      852 2023-05-29 20:27:36.579042 multikeyjwt-1.1.0/src/multikeyjwt/jwt/common.py
+-rw-r--r--   0        0        0     2522 2023-05-30 06:11:54.955482 multikeyjwt-1.1.0/src/multikeyjwt/jwt/issuer.py
+-rw-r--r--   0        0        0     2659 2023-05-29 20:28:56.589049 multikeyjwt-1.1.0/src/multikeyjwt/jwt/verifier.py
+-rw-r--r--   0        0        0      114 2023-05-30 05:14:23.983577 multikeyjwt-1.1.0/src/multikeyjwt/middleware/__init__.py
+-rw-r--r--   0        0        0     1809 2023-05-30 04:10:07.248745 multikeyjwt-1.1.0/src/multikeyjwt/middleware/jwtbearer.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:13:11.057378 multikeyjwt-1.1.0/src/multikeyjwt/py.typed
+-rw-r--r--   0        0        0     4311 1970-01-01 00:00:00.000000 multikeyjwt-1.1.0/setup.py
+-rw-r--r--   0        0        0     4042 1970-01-01 00:00:00.000000 multikeyjwt-1.1.0/PKG-INFO
```

### Comparing `multikeyjwt-1.0.0/LICENSE` & `multikeyjwt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multikeyjwt-1.0.0/README.rst` & `multikeyjwt-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `multikeyjwt-1.0.0/pyproject.toml` & `multikeyjwt-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multikeyjwt"
-version = "1.0.0"
+version = "1.1.0"
 description = "Verify JWTs with multiple public keys, FastAPI middleware for auth"
 authors = ["Eero af Heurlin <eero.afheurlin@iki.fi>"]
 homepage = "https://github.com/pvarki/python-multikeyjwt/"
 repository = "https://github.com/pvarki/python-multikeyjwt/"
 license = "MIT"
 readme = "README.rst"
```

### Comparing `multikeyjwt-1.0.0/src/multikeyjwt/config.py` & `multikeyjwt-1.1.0/src/multikeyjwt/config.py`

 * *Files identical despite different names*

### Comparing `multikeyjwt-1.0.0/src/multikeyjwt/jwt/common.py` & `multikeyjwt-1.1.0/src/multikeyjwt/jwt/common.py`

 * *Files identical despite different names*

### Comparing `multikeyjwt-1.0.0/src/multikeyjwt/jwt/issuer.py` & `multikeyjwt-1.1.0/src/multikeyjwt/jwt/issuer.py`

 * *Files identical despite different names*

### Comparing `multikeyjwt-1.0.0/src/multikeyjwt/jwt/verifier.py` & `multikeyjwt-1.1.0/src/multikeyjwt/jwt/verifier.py`

 * *Files identical despite different names*

### Comparing `multikeyjwt-1.0.0/src/multikeyjwt/middleware/jwtbearer.py` & `multikeyjwt-1.1.0/src/multikeyjwt/middleware/jwtbearer.py`

 * *Files identical despite different names*

### Comparing `multikeyjwt-1.0.0/setup.py` & `multikeyjwt-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 {'all': ['fastapi>0.89,<1.0'], 'fastapi': ['fastapi>0.89,<1.0']}
 
 entry_points = \
 {'console_scripts': ['multikeyjwt = multikeyjwt.console:multikeyjwt_cli']}
 
 setup_kwargs = {
     'name': 'multikeyjwt',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': 'Verify JWTs with multiple public keys, FastAPI middleware for auth',
     'long_description': '===========\nmultikeyjwt\n===========\n\nVerify JWTs with multiple public keys, FastAPI middleware for auth\n\nCreating signing keys\n---------------------\n\n.. code-block:: bash\n\n    echo "My very g00d Passphrase" >/tmp/jwtRS256_passphrase.txt\n    ./make_keypair.sh\n\n\nDocker\n------\n\nFor more controlled deployments and to get rid of "works on my computer" -syndrome, we always\nmake sure our software works under docker.\n\nIt\'s also a quick way to get started with a standard development environment.\n\nSSH agent forwarding\n^^^^^^^^^^^^^^^^^^^^\n\nWe need buildkit_::\n\n    export DOCKER_BUILDKIT=1\n\n.. _buildkit: https://docs.docker.com/develop/develop-images/build_enhancements/\n\nAnd also the exact way for forwarding agent to running instance is different on OSX::\n\n    export DOCKER_SSHAGENT="-v /run/host-services/ssh-auth.sock:/run/host-services/ssh-auth.sock -e SSH_AUTH_SOCK=/run/host-services/ssh-auth.sock"\n\nand Linux::\n\n    export DOCKER_SSHAGENT="-v $SSH_AUTH_SOCK:$SSH_AUTH_SOCK -e SSH_AUTH_SOCK"\n\nCreating a development container\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nBuild image, create container and start it::\n\n    docker build --ssh default --target devel_shell -t multikeyjwt:devel_shell .\n    docker create --name multikeyjwt_devel -v `pwd`":/app" -it `echo $DOCKER_SSHAGENT` multikeyjwt:devel_shell\n    docker start -i multikeyjwt_devel\n\npre-commit considerations\n^^^^^^^^^^^^^^^^^^^^^^^^^\n\nIf working in Docker instead of native env you need to run the pre-commit checks in docker too::\n\n    docker exec -i multikeyjwt_devel /bin/bash -c "pre-commit install"\n    docker exec -i multikeyjwt_devel /bin/bash -c "pre-commit run --all-files"\n\nYou need to have the container running, see above. Or alternatively use the docker run syntax but using\nthe running container is faster::\n\n    docker run --rm -it -v `pwd`":/app" multikeyjwt:devel_shell -c "pre-commit run --all-files"\n\nTest suite\n^^^^^^^^^^\n\nYou can use the devel shell to run py.test when doing development, for CI use\nthe "tox" target in the Dockerfile::\n\n    docker build --ssh default --target tox -t multikeyjwt:tox .\n    docker run --rm -it -v `pwd`":/app" `echo $DOCKER_SSHAGENT` multikeyjwt:tox\n\nProduction docker\n^^^^^^^^^^^^^^^^^\n\nThere\'s a "production" target as well for running the application, remember to change that\narchitecture tag to arm64 if building on ARM::\n\n    docker build --ssh default --target production -t multikeyjwt:latest .\n    docker run -it --name multikeyjwt multikeyjwt:amd64-latest\n\nDevelopment\n-----------\n\nTLDR:\n\n- Create and activate a Python 3.8 virtualenv (assuming virtualenvwrapper)::\n\n    mkvirtualenv -p `which python3.8` my_virtualenv\n\n- change to a branch::\n\n    git checkout -b my_branch\n\n- install Poetry: https://python-poetry.org/docs/#installation\n- Install project deps and pre-commit hooks::\n\n    poetry install\n    pre-commit install\n    pre-commit run --all-files\n\n- Ready to go.\n\nRemember to activate your virtualenv whenever working on the repo, this is needed\nbecause pylint and mypy pre-commit hooks use the "system" python for now (because reasons).\n',
     'author': 'Eero af Heurlin',
     'author_email': 'eero.afheurlin@iki.fi',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pvarki/python-multikeyjwt/',
```

### Comparing `multikeyjwt-1.0.0/PKG-INFO` & `multikeyjwt-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multikeyjwt
-Version: 1.0.0
+Version: 1.1.0
 Summary: Verify JWTs with multiple public keys, FastAPI middleware for auth
 Home-page: https://github.com/pvarki/python-multikeyjwt/
 License: MIT
 Author: Eero af Heurlin
 Author-email: eero.afheurlin@iki.fi
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

