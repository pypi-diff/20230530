# Comparing `tmp/asyncpeegee-0.1.0.tar.gz` & `tmp/asyncpeegee-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpeegee-0.1.0.tar", last modified: Tue May 30 02:09:18 2023, max compression
+gzip compressed data, was "asyncpeegee-0.1.1.tar", last modified: Tue May 30 02:33:56 2023, max compression
```

## Comparing `asyncpeegee-0.1.0.tar` & `asyncpeegee-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 violet     (501) staff       (20)        0 2023-05-30 02:09:18.242487 asyncpeegee-0.1.0/
--rw-r--r--   0 violet     (501) staff       (20)    35148 2023-05-30 01:36:12.000000 asyncpeegee-0.1.0/LICENSE
--rw-r--r--   0 violet     (501) staff       (20)      215 2023-05-30 02:09:18.242576 asyncpeegee-0.1.0/PKG-INFO
--rw-r--r--   0 violet     (501) staff       (20)      442 2023-05-30 02:06:12.000000 asyncpeegee-0.1.0/README.md
--rw-r--r--   0 violet     (501) staff       (20)      103 2023-05-30 02:09:18.242845 asyncpeegee-0.1.0/setup.cfg
--rw-r--r--   0 violet     (501) staff       (20)      394 2023-05-30 02:08:41.000000 asyncpeegee-0.1.0/setup.py
-drwxr-xr-x   0 violet     (501) staff       (20)        0 2023-05-30 02:09:18.238827 asyncpeegee-0.1.0/src/
-drwxr-xr-x   0 violet     (501) staff       (20)        0 2023-05-30 02:09:18.241121 asyncpeegee-0.1.0/src/asyncpeegee.egg-info/
--rw-r--r--   0 violet     (501) staff       (20)      215 2023-05-30 02:09:18.000000 asyncpeegee-0.1.0/src/asyncpeegee.egg-info/PKG-INFO
--rw-r--r--   0 violet     (501) staff       (20)      331 2023-05-30 02:09:18.000000 asyncpeegee-0.1.0/src/asyncpeegee.egg-info/SOURCES.txt
--rw-r--r--   0 violet     (501) staff       (20)        1 2023-05-30 02:09:18.000000 asyncpeegee-0.1.0/src/asyncpeegee.egg-info/dependency_links.txt
--rw-r--r--   0 violet     (501) staff       (20)       22 2023-05-30 02:09:18.000000 asyncpeegee-0.1.0/src/asyncpeegee.egg-info/requires.txt
--rw-r--r--   0 violet     (501) staff       (20)        7 2023-05-30 02:09:18.000000 asyncpeegee-0.1.0/src/asyncpeegee.egg-info/top_level.txt
-drwxr-xr-x   0 violet     (501) staff       (20)        0 2023-05-30 02:09:18.241594 asyncpeegee-0.1.0/src/peegee/
--rw-r--r--   0 violet     (501) staff       (20)     1061 2023-05-30 02:03:01.000000 asyncpeegee-0.1.0/src/peegee/__init__.py
--rw-r--r--   0 violet     (501) staff       (20)      833 2023-05-30 02:03:01.000000 asyncpeegee-0.1.0/src/peegee/apgtypes.py
-drwxr-xr-x   0 violet     (501) staff       (20)        0 2023-05-30 02:09:18.242218 asyncpeegee-0.1.0/src/peegee/pool/
--rw-r--r--   0 violet     (501) staff       (20)     1322 2023-05-30 02:03:01.000000 asyncpeegee-0.1.0/src/peegee/pool/__init__.py
--rw-r--r--   0 violet     (501) staff       (20)     1271 2023-05-30 02:03:01.000000 asyncpeegee-0.1.0/src/peegee/pool/context.py
+drwxr-xr-x   0 violet     (501) staff       (20)        0 2023-05-30 02:33:56.278115 asyncpeegee-0.1.1/
+-rw-r--r--   0 violet     (501) staff       (20)    35148 2023-05-30 01:36:12.000000 asyncpeegee-0.1.1/LICENSE
+-rw-r--r--   0 violet     (501) staff       (20)      215 2023-05-30 02:33:56.278190 asyncpeegee-0.1.1/PKG-INFO
+-rw-r--r--   0 violet     (501) staff       (20)      442 2023-05-30 02:11:17.000000 asyncpeegee-0.1.1/README.md
+-rw-r--r--   0 violet     (501) staff       (20)      103 2023-05-30 02:33:56.278753 asyncpeegee-0.1.1/setup.cfg
+-rw-r--r--   0 violet     (501) staff       (20)      453 2023-05-30 02:33:55.000000 asyncpeegee-0.1.1/setup.py
+drwxr-xr-x   0 violet     (501) staff       (20)        0 2023-05-30 02:33:56.273906 asyncpeegee-0.1.1/src/
+drwxr-xr-x   0 violet     (501) staff       (20)        0 2023-05-30 02:33:56.276854 asyncpeegee-0.1.1/src/asyncpeegee.egg-info/
+-rw-r--r--   0 violet     (501) staff       (20)      215 2023-05-30 02:33:56.000000 asyncpeegee-0.1.1/src/asyncpeegee.egg-info/PKG-INFO
+-rw-r--r--   0 violet     (501) staff       (20)      332 2023-05-30 02:33:56.000000 asyncpeegee-0.1.1/src/asyncpeegee.egg-info/SOURCES.txt
+-rw-r--r--   0 violet     (501) staff       (20)        1 2023-05-30 02:33:56.000000 asyncpeegee-0.1.1/src/asyncpeegee.egg-info/dependency_links.txt
+-rw-r--r--   0 violet     (501) staff       (20)       22 2023-05-30 02:33:56.000000 asyncpeegee-0.1.1/src/asyncpeegee.egg-info/requires.txt
+-rw-r--r--   0 violet     (501) staff       (20)        7 2023-05-30 02:33:56.000000 asyncpeegee-0.1.1/src/asyncpeegee.egg-info/top_level.txt
+drwxr-xr-x   0 violet     (501) staff       (20)        0 2023-05-30 02:33:56.277269 asyncpeegee-0.1.1/src/peegee/
+-rw-r--r--   0 violet     (501) staff       (20)      994 2023-05-30 02:33:21.000000 asyncpeegee-0.1.1/src/peegee/__init__.py
+-rw-r--r--   0 violet     (501) staff       (20)      343 2023-05-30 02:32:57.000000 asyncpeegee-0.1.1/src/peegee/__init__.pyi
+drwxr-xr-x   0 violet     (501) staff       (20)        0 2023-05-30 02:33:56.277860 asyncpeegee-0.1.1/src/peegee/pool/
+-rw-r--r--   0 violet     (501) staff       (20)     1309 2023-05-30 02:32:53.000000 asyncpeegee-0.1.1/src/peegee/pool/__init__.py
+-rw-r--r--   0 violet     (501) staff       (20)     1276 2023-05-30 02:32:09.000000 asyncpeegee-0.1.1/src/peegee/pool/context.py
```

### Comparing `asyncpeegee-0.1.0/LICENSE` & `asyncpeegee-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncpeegee-0.1.0/src/peegee/__init__.py` & `asyncpeegee-0.1.1/src/peegee/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,19 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from apgtypes import Connection
-from pool import create_pool, Pool, WrappedPool
+from pool import create_pool, WrappedPool
 from pool.context import PoolAcquireContext, WrappedPoolAcquireContext
 
 __all__ = [
-    "Connection",
-    "create_pool",
-    "Pool",
     "WrappedPool",
     "PoolAcquireContext",
-    "WrappedPoolAcquireContext"
+    "WrappedPoolAcquireContext",
+    "create_pool",
 ]
```

### Comparing `asyncpeegee-0.1.0/src/peegee/pool/__init__.py` & `asyncpeegee-0.1.1/src/peegee/pool/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+from peegee import Pool
+from pool.context import WrappedPoolAcquireContext
 from typing import Any
 import asyncpg
-from pool.context import WrappedPoolAcquireContext
-
-Pool = asyncpg.Pool[asyncpg.Record]
 
 class WrappedPool:
     pool: Pool
 
     def __init__(self, pool: Pool):
         self.pool = pool
```

### Comparing `asyncpeegee-0.1.0/src/peegee/pool/context.py` & `asyncpeegee-0.1.1/src/peegee/pool/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+from peegee import Connection
 from typing import Any
-import apgtypes
 import asyncpg.pool
 
 PoolAcquireContext = asyncpg.pool.PoolAcquireContext[asyncpg.Record]
 
 class WrappedPoolAcquireContext:
 	ctx: PoolAcquireContext
 	
 	def __init__(self, ctx: PoolAcquireContext):
 		self.ctx = ctx
 
-	async def __aenter__(self) -> apgtypes.Connection:
+	async def __aenter__(self) -> Connection:
 		return await self.ctx.__aenter__()  # type: ignore
 	
 	async def __aexit__(self, *exc: Any):
 		await self.ctx.__aexit__(self, *exc)
 
 	def __await__(self) -> Any:
 		return self.ctx.__await__()
```

