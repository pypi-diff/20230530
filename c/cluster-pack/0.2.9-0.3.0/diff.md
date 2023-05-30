# Comparing `tmp/cluster_pack-0.2.9-py3-none-any.whl.zip` & `tmp/cluster_pack-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 30463 bytes, number of entries: 18
--rw-r--r--  2.0 unx      300 b- defN 21-Oct-05 07:11 cluster_pack/__init__.py
--rw-r--r--  2.0 unx    18462 b- defN 21-Oct-05 07:11 cluster_pack/_version.py
--rw-r--r--  2.0 unx     4099 b- defN 21-Oct-05 07:11 cluster_pack/conda.py
--rw-r--r--  2.0 unx     8284 b- defN 21-Oct-05 07:11 cluster_pack/filesystem.py
--rw-r--r--  2.0 unx    12420 b- defN 21-Oct-05 07:11 cluster_pack/packaging.py
--rw-r--r--  2.0 unx      652 b- defN 21-Oct-05 07:11 cluster_pack/process.py
--rw-r--r--  2.0 unx    12175 b- defN 21-Oct-05 07:11 cluster_pack/uploader.py
--rw-r--r--  2.0 unx      123 b- defN 21-Oct-05 07:11 cluster_pack/skein/__init__.py
--rw-r--r--  2.0 unx      567 b- defN 21-Oct-05 07:11 cluster_pack/skein/_execute_fun.py
--rw-r--r--  2.0 unx     5560 b- defN 21-Oct-05 07:11 cluster_pack/skein/skein_config_builder.py
--rw-r--r--  2.0 unx    10587 b- defN 21-Oct-05 07:11 cluster_pack/skein/skein_launcher.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-05 07:11 cluster_pack/spark/__init__.py
--rw-r--r--  2.0 unx     2778 b- defN 21-Oct-05 07:11 cluster_pack/spark/spark_config_builder.py
--rw-r--r--  2.0 unx    11336 b- defN 21-Oct-05 07:11 cluster_pack-0.2.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     3623 b- defN 21-Oct-05 07:11 cluster_pack-0.2.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Oct-05 07:11 cluster_pack-0.2.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 21-Oct-05 07:11 cluster_pack-0.2.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1531 b- defN 21-Oct-05 07:11 cluster_pack-0.2.9.dist-info/RECORD
-18 files, 92602 bytes uncompressed, 27943 bytes compressed:  69.8%
+Zip file size: 32559 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx      334 b- defN 23-May-30 12:41 cluster_pack/__init__.py
+-rw-rw-r--  2.0 unx    18462 b- defN 23-May-30 12:41 cluster_pack/_version.py
+-rw-rw-r--  2.0 unx     5126 b- defN 23-May-30 12:41 cluster_pack/conda.py
+-rw-rw-r--  2.0 unx     8259 b- defN 23-May-30 12:41 cluster_pack/filesystem.py
+-rw-rw-r--  2.0 unx    17536 b- defN 23-May-30 12:41 cluster_pack/packaging.py
+-rw-rw-r--  2.0 unx      652 b- defN 23-May-30 12:41 cluster_pack/process.py
+-rw-rw-r--  2.0 unx    16176 b- defN 23-May-30 12:41 cluster_pack/uploader.py
+-rw-rw-r--  2.0 unx      123 b- defN 23-May-30 12:41 cluster_pack/skein/__init__.py
+-rw-rw-r--  2.0 unx      567 b- defN 23-May-30 12:41 cluster_pack/skein/_execute_fun.py
+-rw-rw-r--  2.0 unx     5523 b- defN 23-May-30 12:41 cluster_pack/skein/skein_config_builder.py
+-rw-rw-r--  2.0 unx    10587 b- defN 23-May-30 12:41 cluster_pack/skein/skein_launcher.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-30 12:41 cluster_pack/spark/__init__.py
+-rw-rw-r--  2.0 unx     3066 b- defN 23-May-30 12:41 cluster_pack/spark/spark_config_builder.py
+-rw-rw-r--  2.0 unx    11336 b- defN 23-May-30 12:41 cluster_pack-0.3.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3754 b- defN 23-May-30 12:41 cluster_pack-0.3.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-30 12:41 cluster_pack-0.3.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       13 b- defN 23-May-30 12:41 cluster_pack-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1531 b- defN 23-May-30 12:41 cluster_pack-0.3.0.dist-info/RECORD
+18 files, 103137 bytes uncompressed, 30039 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: cluster_pack/spark/__init__.py
 Comment: 
 
 Filename: cluster_pack/spark/spark_config_builder.py
 Comment: 
 
-Filename: cluster_pack-0.2.9.dist-info/LICENSE
+Filename: cluster_pack-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: cluster_pack-0.2.9.dist-info/METADATA
+Filename: cluster_pack-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: cluster_pack-0.2.9.dist-info/WHEEL
+Filename: cluster_pack-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: cluster_pack-0.2.9.dist-info/top_level.txt
+Filename: cluster_pack-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cluster_pack-0.2.9.dist-info/RECORD
+Filename: cluster_pack-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cluster_pack/__init__.py

```diff
@@ -8,9 +8,10 @@
     zip_path,
     get_editable_requirements,
     get_non_editable_requirements,
     get_default_fs,
     detect_packer_from_file,
     Packer,
     CONDA_PACKER,
-    PEX_PACKER
+    PEX_PACKER,
+    get_pyenv_usage_from_archive
 )
```

## cluster_pack/conda.py

```diff
@@ -1,19 +1,18 @@
 import hashlib
 import json
 import logging
 import os
-import subprocess
 try:
     import conda_pack
 except NotImplementedError:
     # conda is not supported on windows
     pass
 
-from typing import Dict, List, Collection
+from typing import List, Optional, Union
 
 from cluster_pack import process
 
 
 _logger = logging.getLogger(__name__)
 
 
@@ -71,41 +70,50 @@
     return [env for env in json.loads(stdout)['envs']]
 
 
 def pack_venv_in_conda(
         name: str,
         reqs: List[str],
         changed_reqs: bool = False,
-        output: str = None
+        output: str = None,
+        additional_repo: Optional[Union[List[str], str]] = None,
+        additional_indexes: Optional[List[str]] = None
 ) -> str:
     """
     Pack the current virtual environment
-
+    :param additional_repo: additional pypi repo(s) to download packages from
+    :param additional_indexes: additional indexes to download packages from
     :param reqs: directory to zip
     :param changed_reqs:
        we prefer zipping the current virtual env as much as possible,
        if it has been changed we need to create a new one with 'conda create -n env ..'
        and reinstall the dependencies inside
     :param output: a dedicated output path
     :return: destination of the archive
     """
     if not changed_reqs:
         return conda_pack.pack(name=name, output=output)
     else:
-        return create_and_pack_conda_env(reqs=reqs, output=output)
+        return create_and_pack_conda_env(
+            reqs=reqs, output=output, additional_repo=additional_repo,
+            additional_indexes=additional_indexes
+        )
 
 
 def create_and_pack_conda_env(
     spec_file: str = None,
     reqs: List[str] = None,
-    output: str = None
+    output: str = None,
+    additional_repo: Optional[Union[List[str], str]] = None,
+    additional_indexes: Optional[List[str]] = None
 ) -> str:
     """
     Create a new conda virtual environment and zip it
-
+    :param additional_repo: additional pypi repo(s) to download packages from
+    :param additional_indexes: additional indexes to download packages from
     :param spec_file: conda yaml spec file to use
     :param reqs: dependencies to install
     :param output: a dedicated output path
     :return: destination of the archive
     """
     project_env_name = get_conda_env_name(spec_file=spec_file, reqs=reqs)
 
@@ -115,10 +123,22 @@
     if reqs:
         env_python_bin = os.path.join(env_path, "bin", "python")
         if not os.path.exists(env_python_bin):
             raise RuntimeError(
                 "Failed to create Python binary at " + env_python_bin)
 
         _logger.info("Installing packages into " + env_path)
-        process.call([env_python_bin, "-m", "pip", "install"] + reqs)
+
+        cmd = [env_python_bin, "-m", "pip", "install"]
+        if additional_repo is not None:
+            additional_repo = additional_repo if isinstance(additional_repo, list) \
+                else [additional_repo]
+            for repo in additional_repo:
+                cmd.extend(['--extra-index-url', repo])
+
+        if additional_indexes:
+            for index in additional_indexes:
+                cmd.extend(["-f", index])
+
+        process.call(cmd + reqs)
 
     return conda_pack.pack(prefix=env_path, output=output, force=True)
```

## cluster_pack/filesystem.py

```diff
@@ -1,16 +1,16 @@
 import logging
 import os
 import pyarrow
 import shutil
 import types
 
 
-from typing import Dict, Tuple, Any, List, Iterator
-from pyarrow import filesystem, util
+from typing import Tuple, Any, List, Iterator
+from pyarrow import filesystem
 from urllib.parse import urlparse
 
 try:
     from s3fs import S3FileSystem
 
     # pyarrow calls mkdirs which is an alias to makedirs which is implemented as no-op
     # remove this once https://github.com/dask/s3fs/pull/331 is released
@@ -144,15 +144,15 @@
 
     def _genline(self) -> Iterator[bytes]:
         while True:
             out = self.readline()
             if out:
                 yield out
             else:
-                raise StopIteration
+                return
 
     def __iter__(self) -> Iterator[bytes]:
         return self._genline()
 
     def readlines(self, hint: int = None) -> List[bytes]:
         """Read and return a list of lines from the stream.
```

## cluster_pack/packaging.py

```diff
@@ -7,15 +7,15 @@
 import shutil
 import subprocess
 from subprocess import CalledProcessError
 import sys
 import tempfile
 from typing import (
     Tuple, Dict,
-    Collection, List, Any
+    Collection, List, Any, Optional, NamedTuple, Union
 )
 import uuid
 import zipfile
 import setuptools
 
 from cluster_pack import conda
 
@@ -26,14 +26,30 @@
 EDITABLE_PACKAGES_INDEX = 'editable_packages_index'
 
 _logger = logging.getLogger(__name__)
 
 JsonDictType = Dict[str, Any]
 
 
+class PexTooLargeError(RuntimeError):
+    pass
+
+
+class PythonEnvDescription(NamedTuple):
+    path_to_archive: str
+    interpreter_cmd: str
+    dest_path: str
+    must_unpack: bool
+
+
+UNPACKED_ENV_NAME = "pyenv"
+CONDA_CMD = f"{UNPACKED_ENV_NAME}/bin/python"
+LARGE_PEX_CMD = f"{UNPACKED_ENV_NAME}/__main__.py"
+
+
 def _get_tmp_dir() -> str:
     tmp_dir = f"/tmp/{uuid.uuid1()}"
     _logger.debug(f"local tmp_dir {tmp_dir}")
     os.makedirs(tmp_dir, exist_ok=True)
     return tmp_dir
 
 
@@ -80,41 +96,60 @@
         return [name + "==" + version
                 if version else name
                 for name, version in requirements.items()]
 
 
 def pack_spec_in_pex(spec_file: str,
                      output: str,
-                     pex_inherit_path: str = "prefer") -> str:
+                     pex_inherit_path: str = "fallback",
+                     allow_large_pex: bool = False,
+                     additional_repo: Optional[Union[List[str], str]] = None,
+                     additional_indexes: Optional[List[str]] = None) -> str:
     with open(spec_file, "r") as f:
         lines = [line for line in f.read().splitlines()
                  if line and not line.startswith("#")]
         _logger.debug(f"used requirements: {lines}")
-        return pack_in_pex(lines, output, pex_inherit_path=pex_inherit_path)
+        return pack_in_pex(lines, output, pex_inherit_path=pex_inherit_path,
+                           allow_large_pex=allow_large_pex,
+                           additional_repo=additional_repo,
+                           additional_indexes=additional_indexes)
 
 
 def pack_in_pex(requirements: List[str],
                 output: str,
                 ignored_packages: Collection[str] = [],
-                pex_inherit_path: str = "prefer",
-                editable_requirements:  Dict[str, str] = {}
+                pex_inherit_path: str = "fallback",
+                editable_requirements: Dict[str, str] = {},
+                allow_large_pex: bool = False,
+                additional_repo: Optional[Union[str, List[str]]] = None,
+                additional_indexes: Optional[List[str]] = None
                 ) -> str:
-    """
-    Pack current environment using a pex.
+    """Pack current environment using a pex.
 
+    :param additional_repo: an additional pypi repo if one was used env creation
     :param requirements: list of requirements (ex {'tensorflow': '1.15.0'})
     :param output: location of the pex
     :param ignored_packages: packages to be exluded from pex
     :param pex_inherit_path: see https://github.com/pantsbuild/pex/blob/master/pex/bin/pex.py#L264,
                              possible values ['false', 'fallback', 'prefer']
+    :param allow_large_pex: Creates a non-executable pex that will need to be unzipped to circumvent
+                            python's limitation with zips > 2Gb. The file will need to be unzipped
+                            and the entry point will be <output>/__main__.py
     :return: destination of the archive, name of the pex
     """
 
     with tempfile.TemporaryDirectory() as tempdir:
         cmd = ["pex", f"--inherit-path={pex_inherit_path}"]
+
+        if allow_large_pex:
+            cmd.extend(["--layout", "packed"])
+            tmp_ext = ".tmp"
+        else:
+            tmp_ext = ""
+
         if editable_requirements and len(editable_requirements) > 0:
             for current_package in editable_requirements.values():
                 _logger.debug("Add current path as source", current_package)
                 shutil.copytree(
                     current_package, os.path.join(tempdir, os.path.basename(current_package))
                 )
             cmd.append(f"--sources-directory={tempdir}")
@@ -124,62 +159,87 @@
             if pkg_name in ignored_packages:
                 _logger.debug(f"Ignore requirement {req}")
             else:
                 _logger.debug(f"Add requirement {req}")
                 cmd.append(req)
         if _is_criteo():
             cmd.append(f"--index-url={CRITEO_PYPI_URL}")
-        cmd.extend(["-o", output])
+
+        if additional_repo is not None:
+            additional_repo = additional_repo if isinstance(additional_repo, list) \
+                else [additional_repo]
+            for repo in additional_repo:
+                cmd.append(f"--index-url={repo}")
+
+        if additional_indexes:
+            for index in additional_indexes:
+                cmd.extend(["-f", index])
+
+        cmd.extend(["-o", output + tmp_ext])
 
         try:
             print(f"Running command: {' '.join(cmd)}")
-            subprocess.run(cmd, check=True)
-        except CalledProcessError:
+            call = subprocess.run(cmd, stderr=subprocess.PIPE, stdout=subprocess.PIPE)
+            call.check_returncode()
+
+            if not allow_large_pex and os.path.getsize(output + tmp_ext) > 2 * 1024 * 1024 * 1024:
+                raise PexTooLargeError("The generate pex is larger than 2Gb and won't be executable"
+                                       " by python; Please set the 'allow_large_pex' "
+                                       "flag in upload_env")
+
+        except CalledProcessError as err:
             _logger.exception('Cannot create pex')
+            _logger.exception(err.stderr.decode("ascii"))
             raise
 
-    return output
+        if allow_large_pex:
+            shutil.make_archive(output, 'zip', output + tmp_ext)
+
+    return output + '.zip' if allow_large_pex else output
 
 
 def _get_packages(editable: bool, executable: str = sys.executable) -> List[JsonDictType]:
     editable_mode = "-e" if editable else "--exclude-editable"
+    # We only keep the first line because pip warnings on subsequent lines can cause
+    # JSONDecodeError below
     results = subprocess.check_output(
         [f"{executable}", "-m", "pip", "list", "-l",
-         f"{editable_mode}", "--format", "json", "-v"]).decode()
+         f"{editable_mode}", "--format", "json", "-v"]).decode().split("\n")[0]
 
     _logger.debug(f"'pip list' with editable={editable} results:" + results)
 
-    parsed_results = json.loads(results)
-
-    # https://pip.pypa.io/en/stable/reference/pip_freeze/?highlight=freeze#cmdoption--all
-    # freeze hardcodes to ignore those packages: wheel, distribute, pip, setuptools
-    # To be iso with freeze we also remove those packages
-    return [element for element in parsed_results
-            if element["name"] not in
-            ["distribute", "wheel", "pip", "setuptools"]]
+    try:
+        return json.loads(results)
+    except json.JSONDecodeError as e:
+        _logger.error(f"Caught below exception while parsing output of pip list: {results}")
+        raise e
 
 
 class Packer(object):
     def env_name(self) -> str:
         raise NotImplementedError
 
     def extension(self) -> str:
         raise NotImplementedError
 
     def pack(self,
              output: str,
              reqs: List[str],
              additional_packages: Dict[str, str],
              ignored_packages: Collection[str],
-             editable_requirements: Dict[str, str]) -> str:
+             editable_requirements: Dict[str, str],
+             allow_large_pex: bool = False,
+             additional_repo: Optional[Union[str, List[str]]] = None,
+             additional_indexes: Optional[List[str]] = None) -> str:
         raise NotImplementedError
 
     def pack_from_spec(self,
                        spec_file: str,
-                       output: str) -> str:
+                       output: str,
+                       allow_large_pex: bool = False) -> str:
         raise NotImplementedError
 
 
 def get_env_name(env_var_name: str) -> str:
     """
     Return default virtual env
     """
@@ -198,52 +258,65 @@
         return 'tar.gz'
 
     def pack(self,
              output: str,
              reqs: List[str],
              additional_packages: Dict[str, str],
              ignored_packages: Collection[str],
-             editable_requirements:  Dict[str, str]) -> str:
+             editable_requirements: Dict[str, str],
+             allow_large_pex: bool = False,
+             additional_repo: Optional[Union[str, List[str]]] = None,
+             additional_indexes: Optional[List[str]] = None) -> str:
         return conda.pack_venv_in_conda(
-                  self.env_name(),
-                  reqs,
-                  len(additional_packages) > 0 or len(ignored_packages) > 0,
-                  output)
+            self.env_name(),
+            reqs,
+            len(additional_packages) > 0 or len(ignored_packages) > 0,
+            output,
+            additional_repo,
+            additional_indexes)
 
     def pack_from_spec(self,
                        spec_file: str,
-                       output: str) -> str:
+                       output: str,
+                       allow_large_pex: bool = False) -> str:
         return conda.create_and_pack_conda_env(
-                            spec_file=spec_file,
-                            reqs=None,
-                            output=output)
+            spec_file=spec_file,
+            reqs=None,
+            output=output)
 
 
 class PexPacker(Packer):
     def env_name(self) -> str:
         return get_env_name('VIRTUAL_ENV')
 
     def extension(self) -> str:
         return 'pex'
 
     def pack(self,
              output: str,
              reqs: List[str],
              additional_packages: Dict[str, str],
              ignored_packages: Collection[str],
-             editable_requirements:  Dict[str, str]) -> str:
+             editable_requirements: Dict[str, str],
+             allow_large_pex: bool = False,
+             additional_repo: Optional[Union[str, List[str]]] = None,
+             additional_indexes: Optional[List[str]] = None) -> str:
         return pack_in_pex(reqs,
                            output,
                            ignored_packages,
-                           editable_requirements=editable_requirements)
+                           editable_requirements=editable_requirements,
+                           allow_large_pex=allow_large_pex,
+                           additional_repo=additional_repo,
+                           additional_indexes=additional_indexes)
 
     def pack_from_spec(self,
                        spec_file: str,
-                       output: str) -> str:
-        return pack_spec_in_pex(spec_file=spec_file, output=output)
+                       output: str,
+                       allow_large_pex: bool = False) -> str:
+        return pack_spec_in_pex(spec_file=spec_file, output=output, allow_large_pex=allow_large_pex)
 
 
 CONDA_PACKER = CondaPacker()
 PEX_PACKER = PexPacker()
 
 
 def _get_editable_requirements(executable: str = sys.executable) -> List[str]:
@@ -260,16 +333,16 @@
 def get_non_editable_requirements(executable: str = sys.executable) -> Dict[str, str]:
     return {package["name"]: package["version"]
             for package in _get_packages(False, executable)}
 
 
 def detect_archive_names(
         packer: Packer,
-        package_path: str = None
-) -> Tuple[str, str, str]:
+        package_path: str = None,
+        allow_large_pex: bool = None) -> Tuple[str, str, str]:
     if _running_from_pex():
         pex_file = get_current_pex_filepath()
         env_name = os.path.splitext(os.path.basename(pex_file))[0]
     else:
         pex_file = ""
         env_name = packer.env_name()
 
@@ -277,14 +350,19 @@
         package_path = (f"{get_default_fs()}/user/{getpass.getuser()}"
                         f"/envs/{env_name}.{packer.extension()}")
     else:
         if "".join(os.path.splitext(package_path)[1]) != f".{packer.extension()}":
             raise ValueError(f"{package_path} has the wrong extension"
                              f", .{packer.extension()} is expected")
 
+    if (packer.extension() == PEX_PACKER.extension()
+            and allow_large_pex
+            and not package_path.endswith('.zip')):
+        package_path += '.zip'
+
     return package_path, env_name, pex_file
 
 
 def detect_packer_from_spec(spec_file: str) -> Packer:
     if os.path.basename(spec_file) == "requirements.txt":
         return PEX_PACKER
     elif spec_file.endswith(".yaml") or spec_file.endswith(".yml"):
@@ -298,34 +376,43 @@
     if _is_conda_env():
         return CONDA_PACKER
     else:
         return PEX_PACKER
 
 
 def detect_packer_from_file(zip_file: str) -> Packer:
-    if zip_file.endswith('.pex'):
+    if zip_file.endswith('.pex') or zip_file.endswith('.pex.zip'):
         return PEX_PACKER
     elif zip_file.endswith(".zip") or zip_file.endswith(".tar.gz"):
         return CONDA_PACKER
     else:
         raise ValueError(f"Archive format {zip_file} unsupported. "
                          "Must be .pex or conda .zip/.tar.gz")
 
 
 def get_current_pex_filepath() -> str:
     """
     If we run from a pex, returns the path
     """
-    import _pex
-    return os.path.abspath(os.path.dirname(os.path.dirname(os.path.dirname(_pex.__file__))))
+    # Env variable PEX has been introduced in pex==2.1.54 and is now the
+    # preferred way to detect whether we run from within a pex
+    if "PEX" in os.environ:
+        return os.environ["PEX"]
+
+    # We still temporarilly support the previous way
+    try:
+        import _pex
+        return os.path.abspath(os.path.dirname(os.path.dirname(os.path.dirname(_pex.__file__))))
+    except ModuleNotFoundError:
+        raise RuntimeError("Trying to get current pex file path while not running from PEX")
 
 
 def get_editable_requirements(
-    executable: str = sys.executable,
-    editable_packages_dir: str = os.getcwd()
+        executable: str = sys.executable,
+        editable_packages_dir: str = os.getcwd()
 ) -> Dict[str, str]:
     editable_requirements: Dict[str, str] = {}
     if _running_from_pex():
         try:
             package_names = open(
                 f"{editable_packages_dir}/{EDITABLE_PACKAGES_INDEX}"
             ).read().splitlines()
@@ -343,23 +430,56 @@
         editable_requirements = {os.path.basename(requirement_dir): requirement_dir
                                  for requirement_dir in _get_editable_requirements(executable)}
 
     _logger.info(f"found editable requirements {editable_requirements}")
     return editable_requirements
 
 
+def get_pyenv_usage_from_archive(path_to_archive: str) -> PythonEnvDescription:
+
+    archive_filename = os.path.basename(path_to_archive)
+
+    if archive_filename.endswith('.pex.zip'):
+        return PythonEnvDescription(
+            path_to_archive,
+            LARGE_PEX_CMD,
+            UNPACKED_ENV_NAME,
+            True)
+    elif archive_filename.endswith('.pex'):
+        return PythonEnvDescription(
+            path_to_archive,
+            f"./{archive_filename}",
+            archive_filename,
+            False)
+    elif archive_filename.endswith(".zip") or archive_filename.endswith(".tar.gz"):
+        return PythonEnvDescription(
+            path_to_archive,
+            CONDA_CMD,
+            UNPACKED_ENV_NAME,
+            True)
+    else:
+        raise ValueError(f"Archive format {archive_filename} unsupported. "
+                         "Must be .pex/pex.zip or conda .zip/.tar.gz")
+
+
 def get_default_fs() -> str:
     return subprocess.check_output("hdfs getconf -confKey fs.defaultFS".split()).strip().decode()
 
 
 def _is_conda_env() -> bool:
     return os.environ.get(CONDA_DEFAULT_ENV) is not None
 
 
 def _running_from_pex() -> bool:
+    # Env variable PEX has been introduced in pex==2.1.54 and is now the
+    # preferred way to detect whether we run from within a pex
+    if "PEX" in os.environ:
+        return True
+
+    # We still temporarilly support the previous way
     try:
         import _pex
         return True
     except ModuleNotFoundError:
         return False
```

## cluster_pack/uploader.py

```diff
@@ -1,30 +1,31 @@
 import getpass
 import hashlib
 import json
 import logging
 import os
-import pkg_resources
+import sys
 import pathlib
 import tempfile
 from typing import (
     Tuple,
     Dict,
     Collection,
     List,
-    Any
+    Any,
+    Optional,
+    Union
 )
 from urllib import parse, request
 
 from pex.pex_info import PexInfo
-from pkg_resources import Requirement
+from wheel_filename import parse_wheel_filename
 
 from cluster_pack import filesystem, packaging
 
-
 _logger = logging.getLogger(__name__)
 
 
 def _get_archive_metadata_path(package_path: str) -> str:
     url = parse.urlparse(package_path)
     return url._replace(path=str(pathlib.Path(url.path).with_suffix('.json'))).geturl()
 
@@ -55,23 +56,23 @@
             fd.write(json.dumps(current_packages_list, sort_keys=True, indent=4))
         if resolved_fs.exists(archive_meta_data):
             resolved_fs.rm(archive_meta_data)
         resolved_fs.put(tempfile_path, archive_meta_data)
 
 
 def upload_zip(
-    zip_file: str,
-    package_path: str = None,
-    force_upload: bool = False,
-    fs_args: Dict[str, Any] = {}
+        zip_file: str,
+        package_path: str = None,
+        force_upload: bool = False,
+        fs_args: Dict[str, Any] = {}
 ) -> str:
     packer = packaging.detect_packer_from_file(zip_file)
     package_path, _, _ = packaging.detect_archive_names(packer, package_path)
 
-    resolved_fs, path = filesystem.resolve_filesystem_and_path(package_path, **fs_args)
+    resolved_fs, _ = filesystem.resolve_filesystem_and_path(package_path, **fs_args)
 
     with tempfile.TemporaryDirectory() as tempdir:
         parsed_url = parse.urlparse(zip_file)
         if parsed_url.scheme == "http":
             tmp_zip_file = os.path.join(tempdir, os.path.basename(parsed_url.path))
             request.urlretrieve(zip_file, tmp_zip_file)
             zip_file = tmp_zip_file
@@ -84,73 +85,109 @@
 def upload_env(
         package_path: str = None,
         packer: packaging.Packer = None,
         additional_packages: Dict[str, str] = {},
         ignored_packages: Collection[str] = [],
         force_upload: bool = False,
         include_editable: bool = False,
-        fs_args: Dict[str, Any] = {}
+        fs_args: Dict[str, Any] = {},
+        allow_large_pex: bool = False,
+        additional_repo: Optional[Union[str, List[str]]] = None,
+        additional_indexes: Optional[List[str]] = None
 ) -> Tuple[str, str]:
+    """Upload current python env.
+
+    :param package_path: path where to upload current python env
+    :param packer: packer to use to package the current python env
+    :param additional_packages: additional packages, absent from current env,
+                            to add to the uploaded env
+    :param ignored_packages: specific arguments for special file systems (like S3)
+    :param force_upload: force the packaging and upload of current env
+    :param include_editable: whether to include or not packages installed in editable mode
+    :param fs_args: filesystem args
+    :param allow_large_pex: whether to allow or not building a large pex
+    :param additional_repo: additional repositories compliant with PEP 503 or local directories
+                            laid out in the same format.
+                            ex: https://download.pytorch.org/whl/cu113
+    :param additional_indexes: URLs or paths to an html files/indexes listing packages
+                            ex: https://dl.fbaipublicfiles.com/detectron2/wheels/cu102/
+                                torch1.10/index.html
+    :return: package_path
+    """
     if packer is None:
         packer = packaging.detect_packer_from_env()
-    package_path, env_name, pex_file = packaging.detect_archive_names(packer, package_path)
+    package_path, env_name, pex_file = \
+        packaging.detect_archive_names(packer, package_path, allow_large_pex)
 
-    resolved_fs, path = filesystem.resolve_filesystem_and_path(package_path, **fs_args)
+    resolved_fs, _ = filesystem.resolve_filesystem_and_path(package_path, **fs_args)
 
-    if not packaging._running_from_pex():
+    if pex_file == "":
         _upload_env_from_venv(
             package_path, packer,
             additional_packages, ignored_packages,
             resolved_fs,
             force_upload,
-            include_editable
+            include_editable,
+            allow_large_pex=allow_large_pex,
+            additional_repo=additional_repo,
+            additional_indexes=additional_indexes
         )
     else:
         _upload_zip(pex_file, package_path, resolved_fs, force_upload)
 
     return (package_path,
             env_name)
 
 
 def upload_spec(
-    spec_file: str,
-    package_path: str = None,
-    force_upload: bool = False,
-    fs_args: Dict[str, Any] = {}
-) -> str:
+        spec_file: str,
+        package_path: str = None,
+        force_upload: bool = False,
+        fs_args: Dict[str, Any] = {},
+        allow_large_pex: bool = False) -> str:
     """Upload an environment from a spec file
 
     :param spec_file: the spec file, must be requirements.txt or conda.yaml
     :param package_path: the path where to upload the package
     :param force_upload: whether the cache should be cleared
     :param fs_args: specific arguments for special file systems (like S3)
+    :param allow_large_pex: Creates a non-executable pex that will need to be unzipped to circumvent
+                            python's limitation with zips > 2Gb. The file will need to be unzipped
+                            and the entry point will be <output>/__main__.py
     :return: package_path
     """
     packer = packaging.detect_packer_from_spec(spec_file)
     if not package_path:
         package_path = (f"{packaging.get_default_fs()}/user/{getpass.getuser()}"
                         f"/envs/{_unique_filename(spec_file, packer)}")
     elif not package_path.endswith(packer.extension()):
         package_path = os.path.join(package_path, _unique_filename(spec_file, packer))
 
+    if (packer.extension() == packaging.PEX_PACKER.extension()
+            and allow_large_pex
+            and not package_path.endswith('.zip')):
+        package_path += '.zip'
+
     resolved_fs, path = filesystem.resolve_filesystem_and_path(package_path, **fs_args)
 
     hash = _get_hash(spec_file)
     _logger.info(f"Packaging from {spec_file} with hash={hash}")
     reqs = [hash]
 
-    if force_upload or not _is_archive_up_to_date(package_path, reqs, resolved_fs):
+    up_to_date = _is_archive_up_to_date(package_path, reqs, resolved_fs)
+    if force_upload or not up_to_date:
         _logger.info(
             f"Zipping and uploading your env to {package_path}"
         )
 
         with tempfile.TemporaryDirectory() as tempdir:
             archive_local = packer.pack_from_spec(
                 spec_file=spec_file,
-                output=f"{tempdir}/{packer.env_name()}.{packer.extension()}")
+                output=f"{tempdir}/{packer.env_name()}.{packer.extension()}",
+                allow_large_pex=allow_large_pex)
 
             dir = os.path.dirname(package_path)
             if not resolved_fs.exists(dir):
                 resolved_fs.mkdir(dir)
             resolved_fs.put(archive_local, package_path)
 
             _dump_archive_metadata(package_path, reqs, resolved_fs)
@@ -169,25 +206,25 @@
 
 def _get_hash(spec_file: str) -> str:
     with open(spec_file) as f:
         return hashlib.sha1(f.read().encode()).hexdigest()
 
 
 def _upload_zip(
-    zip_file: str, package_path: str,
-    resolved_fs: Any = None, force_upload: bool = False
+        zip_file: str, package_path: str,
+        resolved_fs: Any = None, force_upload: bool = False
 ) -> None:
     packer = packaging.detect_packer_from_file(zip_file)
     if packer == packaging.PEX_PACKER and resolved_fs.exists(package_path):
         with tempfile.TemporaryDirectory() as tempdir:
             local_copy_path = os.path.join(tempdir, os.path.basename(package_path))
             resolved_fs.get(package_path, local_copy_path)
             info_from_storage = PexInfo.from_pex(local_copy_path)
-            into_to_upload = PexInfo.from_pex(zip_file)
-            if not force_upload and info_from_storage.code_hash == into_to_upload.code_hash:
+            info_to_upload = PexInfo.from_pex(zip_file)
+            if not force_upload and info_from_storage.code_hash == info_to_upload.code_hash:
                 _logger.info(f"skip upload of current {zip_file}"
                              f" as it is already uploaded on {package_path}")
                 return
 
     _logger.info(f"upload current {zip_file} to {package_path}")
 
     dir = os.path.dirname(package_path)
@@ -197,17 +234,17 @@
     # Remove previous metadata
     archive_meta_data = _get_archive_metadata_path(package_path)
     if resolved_fs.exists(archive_meta_data):
         resolved_fs.rm(archive_meta_data)
 
 
 def _handle_packages(
-    current_packages: Dict[str, str],
-    additional_packages: Dict[str, str] = {},
-    ignored_packages: Collection[str] = []
+        current_packages: Dict[str, str],
+        additional_packages: Dict[str, str] = {},
+        ignored_packages: Collection[str] = []
 ) -> None:
     if len(additional_packages) > 0:
         additional_package_names = list(additional_packages.keys())
         current_packages_names = list(current_packages.keys())
 
         for name in current_packages_names:
             for additional_package_name in additional_package_names:
@@ -226,91 +263,136 @@
 def _upload_env_from_venv(
         package_path: str,
         packer: packaging.Packer = packaging.PEX_PACKER,
         additional_packages: Dict[str, str] = {},
         ignored_packages: Collection[str] = [],
         resolved_fs: Any = None,
         force_upload: bool = False,
-        include_editable: bool = False
+        include_editable: bool = False,
+        allow_large_pex: bool = False,
+        additional_repo: Optional[Union[str, List[str]]] = None,
+        additional_indexes: Optional[List[str]] = None
 ) -> None:
-    current_packages = packaging.get_non_editable_requirements()
+    executable = packaging.get_current_pex_filepath() \
+        if packaging._running_from_pex() else sys.executable
+    current_packages = packaging.get_non_editable_requirements(executable)
 
-    _handle_packages(
-        current_packages,
-        additional_packages,
-        ignored_packages
-    )
-
-    reqs = packaging.format_requirements(current_packages)
+    reqs = _build_reqs_from_venv(additional_packages, current_packages, ignored_packages)
 
     _logger.debug(f"Packaging current_packages={reqs}")
 
     if not force_upload and _is_archive_up_to_date(package_path, reqs, resolved_fs):
         _logger.info(f"{package_path} already exists")
         return
 
     with tempfile.TemporaryDirectory() as tempdir:
-        env_copied_from_fallback_location = False
-        local_package_path = f'{tempdir}/{packer.env_name()}.{packer.extension()}'
-        local_fs, local_package_path = filesystem.resolve_filesystem_and_path(local_package_path)
-
-        fallback_path = os.environ.get('C_PACK_ENV_FALLBACK_PATH')
-        if not force_upload and fallback_path and packer.extension() == 'pex':
-            _logger.info(f"Copying pre-built env from {fallback_path} to {local_package_path}")
-            if fallback_path.startswith("http://") or fallback_path.startswith("https://"):
-                request.urlretrieve(fallback_path, local_package_path)
-            else:
-                fallback_fs, fallback_path = filesystem.resolve_filesystem_and_path(fallback_path)
-                fallback_fs.get(fallback_path, local_package_path)
-
-            _logger.info(f'Checking requirements in {local_package_path}')
-
-            pex_info = PexInfo.from_pex(local_package_path)
-
-            req_from_pex = _sorted_requirements(_clean_pex_requirements(pex_info))
-            req_from_venv = _sorted_requirements(reqs)
-
-            if (req_from_pex == req_from_venv):
-                env_copied_from_fallback_location = True
-                _dump_archive_metadata(local_package_path, reqs, local_fs)
-                _logger.info('Env copied from fallback location')
-            else:
-                _logger.warning(f'Requirements not met for pre-built {local_package_path}')
-                _logger.info(f'Requirements from pex {req_from_pex}')
-                _logger.info(f'Requirements from venv {req_from_venv}')
-
-        if not env_copied_from_fallback_location:
-            if include_editable:
-                editable_requirements = packaging.get_editable_requirements()
-            else:
-                editable_requirements = {}
-
-            _logger.info(f"Generating and zipping your env to {local_package_path}")
-            local_package_path = packer.pack(
-                output=local_package_path,
-                reqs=reqs,
-                additional_packages=additional_packages,
-                ignored_packages=ignored_packages,
-                editable_requirements=editable_requirements
-            )
+        local_package_path = _pack_from_venv(executable, reqs, tempdir, packer, additional_packages,
+                                             ignored_packages, force_upload, include_editable,
+                                             allow_large_pex, additional_repo, additional_indexes)
 
         dir = os.path.dirname(package_path)
         if not resolved_fs.exists(dir):
             resolved_fs.mkdir(dir)
         _logger.info(f'Uploading env at {local_package_path} to {package_path}')
         resolved_fs.put(local_package_path, package_path)
 
         _dump_archive_metadata(package_path, reqs, resolved_fs)
 
 
-def _sorted_requirements(a: List[str]) -> List[str]:
+def _build_reqs_from_venv(
+        additional_packages: Dict[str, str],
+        current_packages: Dict[str, str],
+        ignored_packages: Collection[str]) -> List[str]:
+    _handle_packages(
+        current_packages,
+        additional_packages,
+        ignored_packages
+    )
+    return packaging.format_requirements(current_packages)
+
+
+def _pack_from_venv(executable: str,
+                    reqs: List[str],
+                    tempdir: str,
+                    packer: packaging.Packer = packaging.PEX_PACKER,
+                    additional_packages: Dict[str, str] = {},
+                    ignored_packages: Collection[str] = [],
+                    force_upload: bool = False,
+                    include_editable: bool = False,
+                    allow_large_pex: bool = False,
+                    additional_repo: Optional[Union[str, List[str]]] = None,
+                    additional_indexes: Optional[List[str]] = None) -> str:
+    env_copied_from_fallback_location = False
+    local_package_path = f'{tempdir}/{packer.env_name()}.{packer.extension()}'
+    local_fs, local_package_path = filesystem.resolve_filesystem_and_path(local_package_path)
+    fallback_path = os.environ.get('C_PACK_ENV_FALLBACK_PATH')
+    if not force_upload and fallback_path and packer.extension() == 'pex':
+        _logger.info(f"Copying pre-built env from {fallback_path} to {local_package_path}")
+        if fallback_path.startswith("http://") or fallback_path.startswith("https://"):
+            request.urlretrieve(fallback_path, local_package_path)
+        else:
+            fallback_fs, fallback_path = filesystem.resolve_filesystem_and_path(fallback_path)
+            fallback_fs.get(fallback_path, local_package_path)
+
+        _logger.info(f'Checking requirements in {local_package_path}')
+
+        pex_info = PexInfo.from_pex(local_package_path)
+
+        req_from_pex = _filter_out_requirements(
+            _sort_requirements(
+                _normalize_requirements(
+                    _format_pex_requirements(pex_info)
+                )
+            )
+        )
+        req_from_venv = _filter_out_requirements(
+            _sort_requirements(
+                _normalize_requirements(reqs)
+            )
+        )
+
+        if (req_from_pex == req_from_venv):
+            env_copied_from_fallback_location = True
+            _dump_archive_metadata(local_package_path, reqs, local_fs)
+            _logger.info('Env copied from fallback location')
+        else:
+            _logger.warning(f'Requirements not met for pre-built {local_package_path}')
+            _logger.info(f'Requirements from pex {req_from_pex}')
+            _logger.info(f'Requirements from venv {req_from_venv}')
+    if not env_copied_from_fallback_location:
+        if include_editable:
+            editable_requirements = packaging.get_editable_requirements(executable)
+        else:
+            editable_requirements = {}
+
+        _logger.info(f"Generating and zipping your env to {local_package_path}")
+        local_package_path = packer.pack(
+            output=local_package_path,
+            reqs=reqs,
+            additional_packages=additional_packages,
+            ignored_packages=ignored_packages,
+            editable_requirements=editable_requirements,
+            allow_large_pex=allow_large_pex,
+            additional_repo=additional_repo,
+            additional_indexes=additional_indexes
+        )
+    return local_package_path
+
+
+def _sort_requirements(a: List[str]) -> List[str]:
     return sorted([item.lower() for item in a])
 
 
-def _format_pex_requirement(req: Requirement) -> str:
-    return req.key + ",".join(["".join(spec) for spec in req.specs])
+def _format_pex_requirements(pex_info: PexInfo) -> List[str]:
+    reqs = [parse_wheel_filename(req) for req in pex_info.distributions.keys()]
+    return [f"{req.project}=={req.version}" for req in reqs]
+
+
+def _normalize_requirements(reqs: List[str]) -> List[str]:
+    return [req.replace('_', '-') for req in reqs]
+
 
+def _filter_out_requirements(reqs: List[str]) -> List[str]:
+    def _keep(req: str) -> bool:
+        return all([d not in req for d in ["wheel", "pip", "setuptools"]])
 
-def _clean_pex_requirements(pex_info: PexInfo) -> List[str]:
-    reqs = pkg_resources.parse_requirements(pex_info.requirements)
-    # pip and setup tools are natively embedded in pex, we ignore them here
-    return [_format_pex_requirement(req) for req in reqs if req.key not in ['pip', 'setuptools']]
+    return [req for req in reqs if _keep(req)]
```

## cluster_pack/skein/skein_config_builder.py

```diff
@@ -1,16 +1,14 @@
 import cloudpickle
 import os
-import skein
-import time
 import uuid
 
 from typing import NamedTuple, Callable, Dict, List, Optional, Any
 
-from cluster_pack import packaging, uploader, filesystem
+from cluster_pack import packaging, uploader
 
 
 class SkeinConfig(NamedTuple):
     script: str
     files: Dict[str, str]
     env: Dict[str, str]
```

## cluster_pack/spark/spark_config_builder.py

```diff
@@ -1,30 +1,34 @@
 
 import os
 import logging
-import pyspark
 from pyspark.sql import SparkSession
 
-from cluster_pack import packaging, uploader
+from cluster_pack import packaging, get_pyenv_usage_from_archive
 
 from typing import Dict, Optional, Any
 
 _logger = logging.getLogger(__name__)
 
 
 def add_packaged_environment(ssb: SparkSession.Builder, archive: str) -> None:
     archive = _make_path_hadoop_compatible(archive)
-    if archive.endswith('pex'):
-        _add_or_merge(ssb, "spark.yarn.dist.files", f"{archive}")
+
+    usage = get_pyenv_usage_from_archive(archive)
+    os.environ['PYSPARK_PYTHON'] = usage.interpreter_cmd
+
+    if usage.must_unpack:
+        _add_archive(ssb, f"{archive}#{usage.dest_path}")
+    else:
         ssb.config("spark.executorEnv.PEX_ROOT", "./.pex")
-        os.environ['PYSPARK_PYTHON'] = './' + archive.split('/')[-1]
-        os.environ['PYSPARK_DRIVER_PYTHON'] = archive.split('/')[-1]
+        _add_or_merge(ssb, "spark.yarn.dist.files", f"{archive}")
+
+    if _get_value(ssb, "spark.submit.deployMode") == "cluster":
+        os.environ['PYSPARK_DRIVER_PYTHON'] = usage.interpreter_cmd
     else:
-        _add_archive(ssb, f"{archive}#condaenv")
-        os.environ['PYSPARK_PYTHON'] = "./condaenv/bin/python"
         os.environ['PYSPARK_DRIVER_PYTHON'] = 'python'
 
     if not _get_value(ssb, "spark.master") == "yarn":
         _logger.info("Not running on yarn. Adding archive to spark.files")
         _add_or_merge(ssb, "spark.files", f"{archive}")
 
 
@@ -46,23 +50,26 @@
 
 
 def _add_archive(ssb: SparkSession.Builder, path: str) -> None:
     _add_or_merge(ssb, "spark.yarn.dist.archives", path)
 
 
 def _get_value(ssb: SparkSession.Builder, key: str) -> Optional[str]:
-    if key in ssb._options:
-        return ssb._options[key]
+    if key in ssb._options:  # type: ignore [attr-defined]
+        return ssb._options[key]  # type: ignore [attr-defined]
     return None
 
 
 def _add_or_merge(ssb: SparkSession.Builder, key: str, value: str) -> None:
-    if key in ssb._options:
-        old_value = ssb._options[key]
-        ssb.config(key, f"{old_value},{value}")
+    sep = ','
+    if key in ssb._options:  # type: ignore [attr-defined]
+        old_value = ssb._options[key]  # type: ignore [attr-defined]
+        old_value_set = set(old_value.split(sep))
+        old_value_set.add(value)
+        ssb.config(key, sep.join(old_value_set))
     else:
         ssb.config(key, value)
 
 
 # https://hadoop.apache.org/docs/current/hadoop-aws/tools/hadoop-aws/index.html#How_S3A_writes_data_to_S3
 # Hadoop uses s3a where aws seems to use S3 now
 # See https://github.com/dask/s3fs/pull/269 for s3fs
```

## Comparing `cluster_pack-0.2.9.dist-info/LICENSE` & `cluster_pack-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cluster_pack-0.2.9.dist-info/METADATA` & `cluster_pack-0.3.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster-pack
-Version: 0.2.9
+Version: 0.3.0
 Summary: A library on top of either pex or conda-packto make your Python code easily available on a cluster
 Home-page: https://github.com/criteo/cluster-pack
 Maintainer: Criteo
 Maintainer-email: github@criteo.com
 License: UNKNOWN
 Keywords: hadoop distributed cluster S3 HDFS
 Platform: UNKNOWN
@@ -13,24 +13,27 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: cloudpickle
-Requires-Dist: pex (==2.1.50)
+Requires-Dist: pex (==2.1.137)
 Requires-Dist: conda-pack
 Requires-Dist: pip (>=18.1)
 Requires-Dist: pyarrow
 Requires-Dist: fire
 Requires-Dist: types-setuptools
+Requires-Dist: wheel-filename
 
 # cluster-pack
 
 cluster-pack is a library on top of either [pex][pex] or [conda-pack][conda-pack] to make your Python code easily available on a cluster.
 
 Its goal is to make your prod/dev Python code & libraries easiliy available on any cluster. cluster-pack supports HDFS/S3 as a distributed storage.
```

