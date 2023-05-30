# Comparing `tmp/gh_release_install-0.8.0.tar.gz` & `tmp/gh_release_install-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gh_release_install-0.8.0.tar", max compression
+gzip compressed data, was "gh_release_install-0.9.0.tar", max compression
```

## Comparing `gh_release_install-0.8.0.tar` & `gh_release_install-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    35149 2022-09-17 14:20:46.467520 gh_release_install-0.8.0/LICENSE
--rw-r--r--   0        0        0     4213 2022-09-17 14:20:46.467520 gh_release_install-0.8.0/README.md
--rw-r--r--   0        0        0       71 2022-09-17 14:20:46.467520 gh_release_install-0.8.0/gh_release_install/__init__.py
--rw-r--r--   0        0        0     3456 2022-09-17 14:20:46.467520 gh_release_install-0.8.0/gh_release_install/cli.py
--rw-r--r--   0        0        0     6328 2022-09-17 14:20:46.467520 gh_release_install-0.8.0/gh_release_install/main.py
--rw-r--r--   0        0        0      864 2022-09-17 14:20:46.467520 gh_release_install-0.8.0/gh_release_install/unpack.py
--rw-r--r--   0        0        0     1380 2022-09-17 14:20:46.467520 gh_release_install-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5173 1970-01-01 00:00:00.000000 gh_release_install-0.8.0/setup.py
--rw-r--r--   0        0        0     5258 1970-01-01 00:00:00.000000 gh_release_install-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-01 21:02:41.322265 gh_release_install-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4718 2022-10-01 21:02:41.322265 gh_release_install-0.9.0/README.md
+-rw-r--r--   0        0        0       71 2022-10-01 21:02:41.322265 gh_release_install-0.9.0/gh_release_install/__init__.py
+-rw-r--r--   0        0        0     1784 2022-10-01 21:02:41.322265 gh_release_install-0.9.0/gh_release_install/checksum.py
+-rw-r--r--   0        0        0     3923 2022-10-01 21:02:41.322265 gh_release_install-0.9.0/gh_release_install/cli.py
+-rw-r--r--   0        0        0     7384 2022-10-01 21:02:41.322265 gh_release_install-0.9.0/gh_release_install/main.py
+-rw-r--r--   0        0        0      863 2022-10-01 21:02:41.322265 gh_release_install-0.9.0/gh_release_install/unpack.py
+-rw-r--r--   0        0        0     1390 2022-10-01 21:02:41.326265 gh_release_install-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5690 1970-01-01 00:00:00.000000 gh_release_install-0.9.0/setup.py
+-rw-r--r--   0        0        0     5763 1970-01-01 00:00:00.000000 gh_release_install-0.9.0/PKG-INFO
```

### Comparing `gh_release_install-0.8.0/LICENSE` & `gh_release_install-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gh_release_install-0.8.0/README.md` & `gh_release_install-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -56,15 +56,16 @@
 gh-release-install --help
 ```
 
 ## Usage
 
 ```sh
 usage: gh-release-install [-h] [--extract <filename>] [--version <version>]
-                          [--version-file <filename>] [-v] [-q]
+                          [--version-file <filename>]
+                          [--checksum <hash>:<digest|asset>] [-v] [-q]
                           REPOSITORY ASSET DESTINATION
 
 Install GitHub release file on your system.
 
 positional arguments:
   REPOSITORY            Github REPOSITORY org/repo to get the release from.
   ASSET                 Release ASSET filename. May contain variables such as
@@ -83,14 +84,20 @@
   --version <version>   Desired release version to install. When using 'latest'
                         the installer will guess the latest version from the
                         Github API. (default: latest)
   --version-file <filename>
                         Track the version installed on the system using a file.
                         May contain variables such as '{destination}'. (default:
                         None)
+  --checksum <hash>:<digest|asset>
+                        Asset checksum used to verify the downloaded ASSET.
+                        <hash> can be one of md5, sha1, sha224, sha256, sha384,
+                        sha512. <digest|asset> can either be the expected
+                        checksum, or the filename of an checksum file in the
+                        release assets. (default: None)
   -v, --verbose         Increase the verbosity. (default: 0)
   -q, --quiet           Disable logging. (default: None)
 
 template variables:
     {tag}               Release tag name.
     {version}           Release tag name without leading 'v'.
     {destination}       DESTINATION path, including the asset filename if path
@@ -102,9 +109,11 @@
         '/usr/local/bin/shfmt' \
         --version 'v3.3.1'
 
     gh-release-install 'prometheus/prometheus' \
         'prometheus-{version}.linux-amd64.tar.gz' \
         --extract 'prometheus-{version}.linux-amd64/prometheus' \
         '/usr/local/bin/prometheus' \
-        --version-file '{destination}.version'
+        --version-file '{destination}.version' \
+        --checksum 'sha256:sha256sums.txt'
+
 ```
```

### Comparing `gh_release_install-0.8.0/gh_release_install/cli.py` & `gh_release_install-0.9.0/gh_release_install/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from argparse import (
     ArgumentDefaultsHelpFormatter,
     ArgumentParser,
     RawDescriptionHelpFormatter,
 )
 
 from gh_release_install import GhReleaseInstall
+from gh_release_install.checksum import HASH_ALGORITHM
 
 logger = logging.getLogger(__name__)
 
 
 class ArgumentParserFormatter(
     RawDescriptionHelpFormatter,
     ArgumentDefaultsHelpFormatter,
@@ -58,14 +59,21 @@
 parser.add_argument(
     "--version-file",
     metavar="<filename>",
     help="""Track the version installed on the system using a file. May contain
             variables such as '{destination}'.""",
 )
 parser.add_argument(
+    "--checksum",
+    metavar="<hash>:<digest|asset>",
+    help=f"""Asset checksum used to verify the downloaded ASSET. <hash> can be one of
+             {', '.join(HASH_ALGORITHM)}. <digest|asset> can either be the expected
+             checksum, or the filename of an checksum file in the release assets.""",
+)
+parser.add_argument(
     "-v",
     "--verbose",
     dest="verbosity",
     action="count",
     default=0,
     help="Increase the verbosity.",
 )
@@ -90,15 +98,16 @@
         '/usr/local/bin/shfmt' \\
         --version 'v3.3.1'
 
     gh-release-install 'prometheus/prometheus' \\
         'prometheus-{version}.linux-amd64.tar.gz' \\
         --extract 'prometheus-{version}.linux-amd64/prometheus' \\
         '/usr/local/bin/prometheus' \\
-        --version-file '{destination}.version'
+        --version-file '{destination}.version' \\
+        --checksum 'sha256:sha256sums.txt'
 """
 
 
 def run():
     args = parser.parse_args()
 
     if args.verbosity is not None and args.verbosity >= 0:
@@ -111,14 +120,15 @@
     installer = GhReleaseInstall(
         repository=args.repository,
         asset=args.asset,
         destination=args.destination,
         extract=args.extract,
         version=args.version,
         version_file=args.version_file,
+        checksum=args.checksum,
     )
 
     try:
         installer.run()
     # pylint: disable=broad-except
     except Exception as exception:
         logger.exception(exception)
```

### Comparing `gh_release_install-0.8.0/gh_release_install/main.py` & `gh_release_install-0.9.0/gh_release_install/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,190 +5,223 @@
 from os import environ
 from pathlib import Path
 from shutil import move, unpack_archive
 from tempfile import TemporaryDirectory
 
 from requests import Session
 
+from .checksum import (
+    compute_file_checksum,
+    find_checksum_in_file,
+    is_hexdigest,
+    parse_checksum_option,
+)
 from .unpack import register_unpack_formats
 
-LATEST_VERSION = "latest"
+__all__ = ["GhReleaseInstall"]
+
+LATEST = "latest"
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
-def template_property(getter):
-    """
-    template_property store the content in shared dict '_tmpls'.
-    """
-
-    def setter(self, value):
-        # pylint: disable=protected-access
-        self._tmpls[getter.__name__] = value
+# pylint: disable=too-few-public-methods
+class Release:
+    def __init__(self, tag: str) -> None:
+        self.tag = tag
+
+    @property
+    def version(self) -> str:
+        return self.tag.strip("v")
 
-    return property(fget=getter, fset=setter)
 
+def get_latest_tag(session: Session, repository: str) -> str:
+    url = f"https://api.github.com/repos/{repository}/releases/latest"
+    with session.get(url) as res:
+        res.raise_for_status()
+        body = res.json()
 
-# pylint: disable=too-many-instance-attributes
-class GhReleaseInstall:
-    _local_tag: str | None = None
-    _local_version: str | None = None
-    _target_tag: str | None = None
-    _target_version: str | None = None
+    return body["tag_name"]
 
-    # Used for template properties
-    _tmpls: dict[str, str] = {}
 
+# pylint: disable=too-many-instance-attributes
+class GhReleaseInstall:
+    _target: Release | None = None
+    _local: Release | None = None
     _session: Session
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         repository: str,
         asset: str,
         destination: str | Path,
         extract: str | None = None,
-        version: str = LATEST_VERSION,
+        version: str = LATEST,
         version_file: str | None = None,
+        checksum: str | None = None,
     ):
-        self.repository = repository
-        self.asset = asset
-        self.destination = Path(destination)
-        self.extract = extract
-        self.version = version
-        self.version_file = version_file
+        self._repository = repository
+        self._asset = asset
+        self._destination = str(destination)
+        self._extract = extract
+        self._version = version
+        self._version_file = version_file
+
+        self.checksum_algorithm, self.checksum = None, None
+        if checksum is not None:
+            self.checksum_algorithm, self.checksum = parse_checksum_option(checksum)
 
         self._session = Session()
         if "GITHUB_TOKEN" in environ:
             logger.debug("Loading GITHUB_TOKEN from env")
             github_token = environ.get("GITHUB_TOKEN")
             self._session.headers.update({"Authorization": f"token {github_token}"})
 
         register_unpack_formats()
 
-    def _format_tmpl(self, tmpl: str | None, **kwargs: str) -> str | None:
-        if tmpl is None:
-            return None
-
-        if self._target_version is not None:
-            kwargs["version"] = self._target_version
-        if self._target_tag is not None:
-            kwargs["tag"] = self._target_tag
-
-        return str(tmpl).format(**kwargs)
-
-    @template_property
-    def asset(self) -> str | None:
-        return self._format_tmpl(self._tmpls["asset"])
+    def _resolve_path(self, path: str, **variables: str) -> str:
+        if self._target is not None:
+            variables["tag"] = self._target.tag
+            variables["version"] = self._target.version
+
+        return path.format(**variables)
+
+    @property
+    def asset(self) -> str:
+        return self._resolve_path(self._asset)
 
-    @template_property
+    @property
     def destination(self) -> Path:
-        destination = Path(self._format_tmpl(self._tmpls["destination"]))  # type: ignore
+        destination = Path(self._resolve_path(self._destination))
 
         if destination.is_dir():
             return destination / self.asset
 
         return destination
 
-    @template_property
+    @property
     def extract(self) -> str | None:
-        return self._format_tmpl(self._tmpls["extract"])
+        if self._extract is None:
+            return None
+        return self._resolve_path(self._extract)
 
-    @template_property
+    @property
     def version_file(self) -> Path | None:
-        version_file = self._format_tmpl(
-            self._tmpls["version_file"],
-            destination=self.destination,
+        if self._version_file is None:
+            return None
+
+        return Path(
+            self._resolve_path(
+                self._version_file,
+                destination=str(self.destination),
+            )
         )
-        return Path(version_file) if version_file is not None else None
+
+    def _github_asset_url(self, asset: str) -> str:
+        assert self._target is not None
+        return f"https://github.com/{self._repository}/releases/download/{self._target.tag}/{asset}"
 
     def _get_target_version(self):
         """
         If not provided, get latest tag/version from the Github repository.
         """
-        logger.debug(f"Requested '{self.version}' version")
-        if self.version == LATEST_VERSION:
-            url = f"https://api.github.com/repos/{self.repository}/releases/latest"
-
-            logger.debug(f"Calling '{url}'.")
-            res = self._session.get(url)
-            res.raise_for_status()
-            logger.debug(f"{res.request.method} {res.request.url} {res.status_code}")
-
-            body = res.json()
-
-            self._target_tag = body["tag_name"]
-            self._target_version = body["tag_name"].strip("v")
-            logger.info(f"Latest version is '{self._target_version}'")
+        if self._version == LATEST:
+            self._target = Release(get_latest_tag(self._session, self._repository))
         else:
-            self._target_tag = self.version
-            self._target_version = self.version.strip("v")
+            self._target = Release(self._version)
 
-        logger.debug(f"Target version resolved to '{self._target_version}'")
+        logger.debug(f"Target version is '{self._target.version}'")
 
     def _get_local_version(self):
         """
         Get local tag / version from possible version file.
         """
         if self.version_file is not None and self.version_file.exists():
-            local_version = self.version_file.read_text()
-            self._local_tag = local_version
-            self._local_version = local_version.strip("v")
-            logger.debug(f"Local version resolved to '{self._local_version}'")
+            self._local = Release(self.version_file.read_text(encoding="utf-8"))
+            logger.debug(f"Local version is '{self._local.version}'")
 
-    def _download_release_asset(self, tmp_dir: Path):
+    def _get_checksum_from_url(self, url: str) -> str | None:
         """
-        Download target version release file in a temporary file.
+        Download checksum file from the provided url and extract the checksum.
         """
-        url = (
-            "https://github.com"
-            f"/{self.repository}/releases/download/{self._target_tag}/{self.asset}"
-        )
+        with self._session.get(url) as res:
+            if res.status_code == 404:
+                return None
+            res.raise_for_status()
 
-        logger.debug(f"Calling '{url}'")
-        res = self._session.get(url, stream=True)
-        res.raise_for_status()
-        logger.debug(f"{res.request.method} {res.request.url} {res.status_code}")
+            return find_checksum_in_file(res.text, self.asset)
+
+    def _verify_checksum(self, asset_file: Path) -> bool:
+        """
+        Verify asset checksum, first check against a possible hand written digest,
+        then check against a digest from a asset checksum file.
+        """
+        assert self.checksum is not None
+        assert self.checksum_algorithm is not None
+
+        local_checksum = compute_file_checksum(self.checksum_algorithm, asset_file)
 
-        tmp_file = tmp_dir / self.asset
+        # We hope nobody will ever pass a asset filename that matches this check
+        if is_hexdigest(self.checksum_algorithm, self.checksum):
+            return local_checksum == self.checksum
 
-        logger.debug(f"Saving asset to '{tmp_file}'")
-        with tmp_file.open("wb") as tmp_fd:
-            for chunk in res.iter_content(chunk_size=256):
-                tmp_fd.write(chunk)
+        target_checksum_url = self._github_asset_url(self.checksum)
+        target_checksum = self._get_checksum_from_url(target_checksum_url)
+        return local_checksum == target_checksum
+
+    def _download_release_asset(self, tmp_dir: Path):
+        """
+        Download target version release file in a temporary file.
+        """
+        url = self._github_asset_url(self.asset)
+        with self._session.get(url, stream=True) as res:
+            res.raise_for_status()
+            tmp_file = tmp_dir / self.asset
+
+            logger.debug(f"Saving asset to '{tmp_file}'")
+            with tmp_file.open("wb") as tmp_fd:
+                for chunk in res.iter_content(chunk_size=2048):
+                    tmp_fd.write(chunk)
 
         return tmp_file
 
-    def _extract_release_asset(self, tmp_dir: Path, asset_file: Path):
+    def _extract_release_asset(self, tmp_dir: Path, asset_file: Path) -> Path:
         """
         Extract downloaded release archive.
         """
         unpack_archive(asset_file, tmp_dir)
+        assert self.extract is not None
         return tmp_dir / self.extract
 
     def run(self):
         self._get_target_version()
         self._get_local_version()
 
-        logger.debug(f"Target '{self._target_tag}' == Local '{self._local_tag}'")
-        if self._target_version == self._local_version:
-            logger.info("Target version is already installed")
-            sys.exit(0)
+        if self._local is not None:
+            if self._target.version == self._local.version:
+                logger.info("Target version is already installed")
+                sys.exit(0)
 
         with TemporaryDirectory(prefix="gh-release-installer") as tmp_dir:
             tmp_dir = Path(tmp_dir)
             asset_file = self._download_release_asset(tmp_dir)
-            logger.info(f"Downloaded asset to '{asset_file}'")
+
+            if self.checksum is not None:
+                if not self._verify_checksum(asset_file):
+                    logger.error("Checksum verification failed")
+                    sys.exit(1)
+                logger.info("Checksum verification succeeded")
 
             if self.extract is not None:
                 asset_file = self._extract_release_asset(tmp_dir, asset_file)
                 logger.info(f"Extracted archive to '{asset_file}'")
 
             move(asset_file, self.destination)
             self.destination.chmod(0o755)
             logger.info(f"Installed file to '{self.destination}'")
 
         # Save to local tag/version file
         if self.version_file is not None:
-            self.version_file.write_text(self._target_tag)
+            self.version_file.write_text(self._target.tag, encoding="utf-8")
             logger.info(f"Saved version file to '{self.version_file}'")
```

### Comparing `gh_release_install-0.8.0/gh_release_install/unpack.py` & `gh_release_install-0.9.0/gh_release_install/unpack.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,14 @@
     with filename.open("rb") as filename_fd:
         with extracted.open("wb") as extracted_fd:
             extracted_fd.write(bz2.decompress(filename_fd.read()))
 
 
 def register_unpack_formats():
     """Register custom unpack formats."""
-    logger.debug("Registering custom unpack formats.")
+    logger.debug("Registering custom unpack formats")
 
     formats = get_unpack_formats()
     if "bz2" not in map(lambda x: x[0], formats):
         register_unpack_format("bz2", [".bz2"], _unpack_bz2, description="bz2 files")
 
     logger.debug(f"Unpack formats available: {formats}")
```

### Comparing `gh_release_install-0.8.0/pyproject.toml` & `gh_release_install-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gh_release_install"
-version = "0.8.0"
+version = "0.9.0"
 description = "CLI helper to install Github releases on your system."
 readme = "README.md"
 authors = ["Joola <jooola@users.noreply.github.com>"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -26,15 +26,15 @@
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 isort = "^5.9.3"
 mypy = "^0.971"
 pylint = "^2.12.0"
 pytest = "^7.0.1"
-pytest-cov = "^3.0.0"
+pytest-cov = "^3.0.0 || ^4.0.0"
 pytest-xdist = "^2.5.0"
 requests-mock = "^1.9.3"
 types-requests = "^2.28.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gh_release_install-0.8.0/setup.py` & `gh_release_install-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['requests>=2.22.0,<2.29']
 
 entry_points = \
 {'console_scripts': ['gh-release-install = gh_release_install.cli:run']}
 
 setup_kwargs = {
     'name': 'gh-release-install',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'CLI helper to install Github releases on your system.',
-    'long_description': '# Github release installer\n\n[![CI](https://github.com/jooola/gh-release-install/actions/workflows/ci.yml/badge.svg)](https://github.com/jooola/gh-release-install/actions/workflows/ci.yml)\n[![PyPI Python Versions](https://img.shields.io/pypi/pyversions/gh-release-install.svg)](https://pypi.org/project/gh-release-install/)\n[![PyPI Package Version](https://img.shields.io/pypi/v/gh-release-install.svg)](https://pypi.org/project/gh-release-install/)\n\n`gh-release-install` is a CLI helper to install Github releases on your system.\nIt can be used for pretty much anything, to install a formatter in your CI, deploy\nsome binary using an orcherstration tool, or on your desktop.\n\nThis project was mainly created to...\n\n```sh\n# ...turn this mess:\nwget --quiet --output-document=- "https://github.com/koalaman/shellcheck/releases/download/v0.7.1/shellcheck-v0.7.1.linux.x86_64.tar.xz" \\\n    | tar --extract --xz --directory=/usr/local/bin --strip-components=1 --wildcards \'shellcheck*/shellcheck\' \\\n    && chmod +x /usr/local/bin/shellcheck\n\nwget --quiet --output-document=/usr/local/bin/shfmt "https://github.com/mvdan/sh/releases/download/v3.2.1/shfmt_v3.2.1_linux_amd64"\xa0\\\n    && chmod +x /usr/local/bin/shfmt\n\n# Into this:\npip3 install gh-release-install\n\ngh-release-install \\\n      "koalaman/shellcheck" \\\n      "shellcheck-{tag}.linux.x86_64.tar.xz" --extract "shellcheck-{tag}/shellcheck" \\\n      "/usr/bin/shellcheck"\n\ngh-release-install \\\n      "mvdan/sh" \\\n      "shfmt_{tag}_linux_amd64" \\\n      "/usr/bin/shfmt"\n```\n\nFeatures:\n\n- Download releases from Github.\n- Extract zip or tarball on the fly.\n- Pin to a desired version or get the `latest` version.\n- Keep track of the local tools version using a version file.\n\n## Installation\n\nInstall the package from pip:\n\n```sh\npip install gh-release-install\ngh-release-install --help\n```\n\nOr with with pipx:\n\n```sh\npipx install gh-release-install\ngh-release-install --help\n```\n\n## Usage\n\n```sh\nusage: gh-release-install [-h] [--extract <filename>] [--version <version>]\n                          [--version-file <filename>] [-v] [-q]\n                          REPOSITORY ASSET DESTINATION\n\nInstall GitHub release file on your system.\n\npositional arguments:\n  REPOSITORY            Github REPOSITORY org/repo to get the release from.\n  ASSET                 Release ASSET filename. May contain variables such as\n                        \'{version}\' or \'{tag}\'.\n  DESTINATION           Path to save the downloaded file. If DESTINATION is a\n                        directory, the asset name will be used as filename in\n                        that directory. May contain variables such as\n                        \'{version}\' or \'{tag}\'.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --extract <filename>  Extract the <filename> from the release asset archive\n                        and install the extracted file instead. May contain\n                        variables such as \'{version}\' or \'{tag}\'. (default:\n                        None)\n  --version <version>   Desired release version to install. When using \'latest\'\n                        the installer will guess the latest version from the\n                        Github API. (default: latest)\n  --version-file <filename>\n                        Track the version installed on the system using a file.\n                        May contain variables such as \'{destination}\'. (default:\n                        None)\n  -v, --verbose         Increase the verbosity. (default: 0)\n  -q, --quiet           Disable logging. (default: None)\n\ntemplate variables:\n    {tag}               Release tag name.\n    {version}           Release tag name without leading \'v\'.\n    {destination}       DESTINATION path, including the asset filename if path\n                        is a directory.\n\nexamples:\n    gh-release-install \'mvdan/sh\' \\\n        \'shfmt_{tag}_linux_amd64\' \\\n        \'/usr/local/bin/shfmt\' \\\n        --version \'v3.3.1\'\n\n    gh-release-install \'prometheus/prometheus\' \\\n        \'prometheus-{version}.linux-amd64.tar.gz\' \\\n        --extract \'prometheus-{version}.linux-amd64/prometheus\' \\\n        \'/usr/local/bin/prometheus\' \\\n        --version-file \'{destination}.version\'\n```\n',
+    'long_description': '# Github release installer\n\n[![CI](https://github.com/jooola/gh-release-install/actions/workflows/ci.yml/badge.svg)](https://github.com/jooola/gh-release-install/actions/workflows/ci.yml)\n[![PyPI Python Versions](https://img.shields.io/pypi/pyversions/gh-release-install.svg)](https://pypi.org/project/gh-release-install/)\n[![PyPI Package Version](https://img.shields.io/pypi/v/gh-release-install.svg)](https://pypi.org/project/gh-release-install/)\n\n`gh-release-install` is a CLI helper to install Github releases on your system.\nIt can be used for pretty much anything, to install a formatter in your CI, deploy\nsome binary using an orcherstration tool, or on your desktop.\n\nThis project was mainly created to...\n\n```sh\n# ...turn this mess:\nwget --quiet --output-document=- "https://github.com/koalaman/shellcheck/releases/download/v0.7.1/shellcheck-v0.7.1.linux.x86_64.tar.xz" \\\n    | tar --extract --xz --directory=/usr/local/bin --strip-components=1 --wildcards \'shellcheck*/shellcheck\' \\\n    && chmod +x /usr/local/bin/shellcheck\n\nwget --quiet --output-document=/usr/local/bin/shfmt "https://github.com/mvdan/sh/releases/download/v3.2.1/shfmt_v3.2.1_linux_amd64"\xa0\\\n    && chmod +x /usr/local/bin/shfmt\n\n# Into this:\npip3 install gh-release-install\n\ngh-release-install \\\n      "koalaman/shellcheck" \\\n      "shellcheck-{tag}.linux.x86_64.tar.xz" --extract "shellcheck-{tag}/shellcheck" \\\n      "/usr/bin/shellcheck"\n\ngh-release-install \\\n      "mvdan/sh" \\\n      "shfmt_{tag}_linux_amd64" \\\n      "/usr/bin/shfmt"\n```\n\nFeatures:\n\n- Download releases from Github.\n- Extract zip or tarball on the fly.\n- Pin to a desired version or get the `latest` version.\n- Keep track of the local tools version using a version file.\n\n## Installation\n\nInstall the package from pip:\n\n```sh\npip install gh-release-install\ngh-release-install --help\n```\n\nOr with with pipx:\n\n```sh\npipx install gh-release-install\ngh-release-install --help\n```\n\n## Usage\n\n```sh\nusage: gh-release-install [-h] [--extract <filename>] [--version <version>]\n                          [--version-file <filename>]\n                          [--checksum <hash>:<digest|asset>] [-v] [-q]\n                          REPOSITORY ASSET DESTINATION\n\nInstall GitHub release file on your system.\n\npositional arguments:\n  REPOSITORY            Github REPOSITORY org/repo to get the release from.\n  ASSET                 Release ASSET filename. May contain variables such as\n                        \'{version}\' or \'{tag}\'.\n  DESTINATION           Path to save the downloaded file. If DESTINATION is a\n                        directory, the asset name will be used as filename in\n                        that directory. May contain variables such as\n                        \'{version}\' or \'{tag}\'.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --extract <filename>  Extract the <filename> from the release asset archive\n                        and install the extracted file instead. May contain\n                        variables such as \'{version}\' or \'{tag}\'. (default:\n                        None)\n  --version <version>   Desired release version to install. When using \'latest\'\n                        the installer will guess the latest version from the\n                        Github API. (default: latest)\n  --version-file <filename>\n                        Track the version installed on the system using a file.\n                        May contain variables such as \'{destination}\'. (default:\n                        None)\n  --checksum <hash>:<digest|asset>\n                        Asset checksum used to verify the downloaded ASSET.\n                        <hash> can be one of md5, sha1, sha224, sha256, sha384,\n                        sha512. <digest|asset> can either be the expected\n                        checksum, or the filename of an checksum file in the\n                        release assets. (default: None)\n  -v, --verbose         Increase the verbosity. (default: 0)\n  -q, --quiet           Disable logging. (default: None)\n\ntemplate variables:\n    {tag}               Release tag name.\n    {version}           Release tag name without leading \'v\'.\n    {destination}       DESTINATION path, including the asset filename if path\n                        is a directory.\n\nexamples:\n    gh-release-install \'mvdan/sh\' \\\n        \'shfmt_{tag}_linux_amd64\' \\\n        \'/usr/local/bin/shfmt\' \\\n        --version \'v3.3.1\'\n\n    gh-release-install \'prometheus/prometheus\' \\\n        \'prometheus-{version}.linux-amd64.tar.gz\' \\\n        --extract \'prometheus-{version}.linux-amd64/prometheus\' \\\n        \'/usr/local/bin/prometheus\' \\\n        --version-file \'{destination}.version\' \\\n        --checksum \'sha256:sha256sums.txt\'\n\n```\n',
     'author': 'Joola',
     'author_email': 'jooola@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `gh_release_install-0.8.0/PKG-INFO` & `gh_release_install-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh-release-install
-Version: 0.8.0
+Version: 0.9.0
 Summary: CLI helper to install Github releases on your system.
 Author: Joola
 Author-email: jooola@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -81,15 +81,16 @@
 gh-release-install --help
 ```
 
 ## Usage
 
 ```sh
 usage: gh-release-install [-h] [--extract <filename>] [--version <version>]
-                          [--version-file <filename>] [-v] [-q]
+                          [--version-file <filename>]
+                          [--checksum <hash>:<digest|asset>] [-v] [-q]
                           REPOSITORY ASSET DESTINATION
 
 Install GitHub release file on your system.
 
 positional arguments:
   REPOSITORY            Github REPOSITORY org/repo to get the release from.
   ASSET                 Release ASSET filename. May contain variables such as
@@ -108,14 +109,20 @@
   --version <version>   Desired release version to install. When using 'latest'
                         the installer will guess the latest version from the
                         Github API. (default: latest)
   --version-file <filename>
                         Track the version installed on the system using a file.
                         May contain variables such as '{destination}'. (default:
                         None)
+  --checksum <hash>:<digest|asset>
+                        Asset checksum used to verify the downloaded ASSET.
+                        <hash> can be one of md5, sha1, sha224, sha256, sha384,
+                        sha512. <digest|asset> can either be the expected
+                        checksum, or the filename of an checksum file in the
+                        release assets. (default: None)
   -v, --verbose         Increase the verbosity. (default: 0)
   -q, --quiet           Disable logging. (default: None)
 
 template variables:
     {tag}               Release tag name.
     {version}           Release tag name without leading 'v'.
     {destination}       DESTINATION path, including the asset filename if path
@@ -127,10 +134,12 @@
         '/usr/local/bin/shfmt' \
         --version 'v3.3.1'
 
     gh-release-install 'prometheus/prometheus' \
         'prometheus-{version}.linux-amd64.tar.gz' \
         --extract 'prometheus-{version}.linux-amd64/prometheus' \
         '/usr/local/bin/prometheus' \
-        --version-file '{destination}.version'
+        --version-file '{destination}.version' \
+        --checksum 'sha256:sha256sums.txt'
+
 ```
```

