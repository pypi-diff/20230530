# Comparing `tmp/fedrq-0.6.0.tar.gz` & `tmp/fedrq-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedrq-0.6.0.tar", last modified: Sat Apr  8 09:02:17 2023, max compression
+gzip compressed data, was "fedrq-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fedrq-0.6.0.tar` & `fedrq-0.7.0.tar`

### file list

```diff
@@ -1,112 +1,117 @@
--rw-r--r--   0        0        0      674 2023-02-19 18:37:34.746046 fedrq-0.6.0/.builds/epel9.yml
--rw-r--r--   0        0        0     2378 2023-03-20 03:33:03.369304 fedrq-0.6.0/.builds/main.yml
--rw-r--r--   0        0        0     1220 2023-02-19 18:37:34.746046 fedrq-0.6.0/.builds/mockbuild-36.yml
--rw-r--r--   0        0        0      751 2023-03-18 19:37:34.175930 fedrq-0.6.0/.builds/mockbuild.yml
--rw-r--r--   0        0        0      227 2023-02-19 18:37:34.746046 fedrq-0.6.0/.copr/Makefile
--rwxr-xr-x   0        0        0      512 2023-02-19 18:37:34.746046 fedrq-0.6.0/.copr/mk.sh
-lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.6.0/.data/share/licenses/fedrq/GPL-2.0-or-later.txt -> ../../../../LICENSES/GPL-2.0-or-later.txt
-lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.6.0/.data/share/licenses/fedrq/MIT.txt -> ../../../../LICENSES/MIT.txt
-lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.6.0/.data/share/licenses/fedrq/PSF-2.0.txt -> ../../../../LICENSES/PSF-2.0.txt
-lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.6.0/.data/share/licenses/fedrq/Unlicense.txt -> ../../../../LICENSES/Unlicense.txt
--rw-r--r--   0        0        0      260 2023-03-19 23:07:21.351951 fedrq-0.6.0/.gitignore
--rw-r--r--   0        0        0     2482 2023-03-19 02:41:47.073223 fedrq-0.6.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    17337 2022-12-13 02:49:11.735043 fedrq-0.6.0/LICENSES/GPL-2.0-or-later.txt
--rw-r--r--   0        0        0     1078 2022-12-13 02:49:11.735043 fedrq-0.6.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     2427 2023-02-19 18:37:34.747046 fedrq-0.6.0/LICENSES/PSF-2.0.txt
--rw-r--r--   0        0        0     1211 2023-02-19 18:37:34.747046 fedrq-0.6.0/LICENSES/Unlicense.txt
--rw-r--r--   0        0        0     9927 2023-04-08 08:59:20.590804 fedrq-0.6.0/NEWS.md
--rw-r--r--   0        0        0       89 2023-03-18 21:16:55.983019 fedrq-0.6.0/NEWS.md.license
--rw-r--r--   0        0        0    12144 2023-03-27 04:19:29.833647 fedrq-0.6.0/README.md
--rw-r--r--   0        0        0      210 2023-02-19 18:37:34.748046 fedrq-0.6.0/changelog
--rw-r--r--   0        0        0      129 2023-02-19 18:37:34.748046 fedrq-0.6.0/changelog.license
--rwxr-xr-x   0        0        0      906 2023-03-19 23:05:00.923501 fedrq-0.6.0/contrib/api_examples/a_noarch_bash.py
--rwxr-xr-x   0        0        0     2502 2023-03-19 23:05:00.924501 fedrq-0.6.0/contrib/api_examples/ftbfs_retirements.py
--rwxr-xr-x   0        0        0      709 2023-04-08 08:57:21.001532 fedrq-0.6.0/contrib/bump.sh
--rw-r--r--   0        0        0      630 2023-03-19 23:07:21.352951 fedrq-0.6.0/contrib/deploy-docsite/main.yaml
--rw-r--r--   0        0        0      183 2023-03-19 23:07:21.352951 fedrq-0.6.0/contrib/deploy-docsite/roles/configure/handlers/main.yaml
--rw-r--r--   0        0        0      885 2023-03-19 23:07:21.352951 fedrq-0.6.0/contrib/deploy-docsite/roles/configure/tasks/main.yml
--rw-r--r--   0        0        0      163 2023-03-19 23:07:21.352951 fedrq-0.6.0/contrib/deploy-docsite/roles/configure/templates/fedrq.caddyfile
--rw-r--r--   0        0        0      415 2023-03-19 23:07:21.352951 fedrq-0.6.0/contrib/deploy-docsite/roles/deploy/tasks/main.yaml
--rw-r--r--   0        0        0      156 2023-03-19 23:07:21.352951 fedrq-0.6.0/contrib/deploy-docsite/vars.yaml
--rwxr-xr-x   0        0        0      907 2023-03-27 04:19:29.833647 fedrq-0.6.0/contrib/fedoraify.py
--rwxr-xr-x   0        0        0      879 2023-03-18 19:37:34.175930 fedrq-0.6.0/contrib/publish.sh
--rw-r--r--   0        0        0     5378 2023-04-06 06:46:42.870073 fedrq-0.6.0/doc/API/Summary.md
--rw-r--r--   0        0        0      147 2023-03-19 23:07:21.353951 fedrq-0.6.0/doc/API/backends/base.md
--rw-r--r--   0        0        0      161 2023-03-19 23:07:21.353951 fedrq-0.6.0/doc/API/backends/dnf.md
--rw-r--r--   0        0        0      371 2023-03-19 23:07:21.353951 fedrq-0.6.0/doc/API/backends/libdnf5.md
--rw-r--r--   0        0        0      133 2023-03-19 23:07:21.353951 fedrq-0.6.0/doc/API/config.md
--rw-r--r--   0        0        0      145 2023-03-19 23:07:21.353951 fedrq-0.6.0/doc/API/release_repo.md
-lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.6.0/doc/News.md -> ../NEWS.md
--rw-r--r--   0        0        0     3178 2023-04-06 06:46:42.870073 fedrq-0.6.0/doc/dnf-repoquery-diff.md
--rw-r--r--   0        0        0    15252 2023-04-06 14:35:06.137989 fedrq-0.6.0/doc/fedrq.1.scd
--rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.6.0/doc/fedrq.1.scd.license
--rw-r--r--   0        0        0     4903 2023-04-06 14:11:08.209044 fedrq-0.6.0/doc/fedrq.5.scd
--rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.6.0/doc/fedrq.5.scd.license
-lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.6.0/doc/index.md -> ../README.md
--rw-r--r--   0        0        0      131 2023-03-19 23:07:21.353951 fedrq-0.6.0/fedrq.rpmlintrc
--rw-r--r--   0        0        0     3193 2023-04-08 08:59:20.574805 fedrq-0.6.0/fedrq.spec
--rw-r--r--   0        0        0     1960 2023-04-06 06:46:42.870073 fedrq-0.6.0/mkdocs.yml
--rw-r--r--   0        0        0     8102 2023-04-06 12:36:51.695430 fedrq-0.6.0/noxfile.py
--rw-r--r--   0        0        0     2596 2023-04-08 08:59:20.586804 fedrq-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      532 2023-03-18 19:37:34.178930 fedrq-0.6.0/ruff.toml
--rw-r--r--   0        0        0      281 2023-02-21 18:02:47.599086 fedrq-0.6.0/src/fedrq/__init__.py
--rw-r--r--   0        0        0      219 2023-02-19 18:37:34.750046 fedrq-0.6.0/src/fedrq/__main__.py
--rw-r--r--   0        0        0     1713 2023-02-21 18:02:47.600086 fedrq-0.6.0/src/fedrq/_compat.py
--rw-r--r--   0        0        0      173 2023-03-18 19:37:34.178930 fedrq-0.6.0/src/fedrq/_config.py
--rw-r--r--   0        0        0     1248 2023-03-18 19:37:34.179930 fedrq-0.6.0/src/fedrq/_utils.py
--rw-r--r--   0        0        0     2529 2023-02-21 18:02:47.601086 fedrq-0.6.0/src/fedrq/backends/__init__.py
--rw-r--r--   0        0        0    14355 2023-04-02 18:37:23.802073 fedrq-0.6.0/src/fedrq/backends/base.py
--rw-r--r--   0        0        0      630 2023-02-21 18:02:47.603086 fedrq-0.6.0/src/fedrq/backends/dnf/__init__.py
--rw-r--r--   0        0        0     6914 2023-03-20 03:32:46.002379 fedrq-0.6.0/src/fedrq/backends/dnf/backend.py
--rw-r--r--   0        0        0      741 2023-02-21 18:02:47.604086 fedrq-0.6.0/src/fedrq/backends/libdnf5/__init__.py
--rw-r--r--   0        0        0    27814 2023-03-20 17:10:06.077134 fedrq-0.6.0/src/fedrq/backends/libdnf5/backend.py
--rw-r--r--   0        0        0     1864 2023-04-06 12:36:51.697430 fedrq-0.6.0/src/fedrq/cli/__init__.py
--rw-r--r--   0        0        0    14644 2023-04-06 12:36:51.697430 fedrq-0.6.0/src/fedrq/cli/base.py
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.6.0/src/fedrq/cli/commands/__init__.py
--rw-r--r--   0        0        0     2854 2023-03-18 19:37:34.182930 fedrq-0.6.0/src/fedrq/cli/commands/pkgs.py
--rw-r--r--   0        0        0     2425 2023-03-17 02:28:51.186103 fedrq-0.6.0/src/fedrq/cli/commands/subpkgs.py
--rw-r--r--   0        0        0    10843 2023-03-18 19:37:34.182930 fedrq-0.6.0/src/fedrq/cli/commands/whatrequires.py
--rw-r--r--   0        0        0    13071 2023-04-06 12:36:51.698430 fedrq-0.6.0/src/fedrq/cli/formatters.py
--rw-r--r--   0        0        0    16106 2023-04-06 06:46:42.871073 fedrq-0.6.0/src/fedrq/config.py
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.6.0/src/fedrq/data/__init__.py
--rw-r--r--   0        0        0     6406 2023-04-06 13:40:31.480346 fedrq-0.6.0/src/fedrq/data/releases.toml
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.6.0/src/fedrq/data/repos/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-06 13:27:21.368508 fedrq-0.6.0/src/fedrq/data/repos/almalinux.repo
--rw-r--r--   0        0        0      639 2023-03-27 04:19:29.835647 fedrq-0.6.0/src/fedrq/data/repos/amazonlinux.repo
--rw-r--r--   0        0        0     1386 2023-04-06 12:36:51.699430 fedrq-0.6.0/src/fedrq/data/repos/centos-stream-compose.repo
--rw-r--r--   0        0        0     1850 2023-02-19 18:37:34.752046 fedrq-0.6.0/src/fedrq/data/repos/centos-stream.repo
--rw-r--r--   0        0        0     1494 2023-04-06 12:36:51.700430 fedrq-0.6.0/src/fedrq/data/repos/centos-stream8-compose.repo
--rw-r--r--   0        0        0     1599 2023-03-18 19:37:34.184930 fedrq-0.6.0/src/fedrq/data/repos/centos-stream8.repo
--rw-r--r--   0        0        0     2185 2023-03-18 19:37:34.184930 fedrq-0.6.0/src/fedrq/data/repos/epel.repo
--rw-r--r--   0        0        0     2402 2023-02-19 18:37:34.752046 fedrq-0.6.0/src/fedrq/data/repos/fedora-rawhide.repo
--rw-r--r--   0        0        0     1480 2023-02-19 18:37:34.752046 fedrq-0.6.0/src/fedrq/data/repos/fedora-updates-testing.repo
--rw-r--r--   0        0        0     1422 2023-02-19 18:37:34.752046 fedrq-0.6.0/src/fedrq/data/repos/fedora-updates.repo
--rw-r--r--   0        0        0     1375 2023-02-19 18:37:34.752046 fedrq-0.6.0/src/fedrq/data/repos/fedora.repo
--rw-r--r--   0        0        0      452 2023-02-19 18:37:34.752046 fedrq-0.6.0/src/fedrq/data/repos/rawhide-buildroot.repo
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.6.0/src/fedrq/py.typed
--rw-r--r--   0        0        0     8912 2023-04-03 17:52:29.583685 fedrq-0.6.0/src/fedrq/release_repo.py
--rw-r--r--   0        0        0      984 2023-02-21 18:02:47.612086 fedrq-0.6.0/src/fedrq/repoquery.py
--rwxr-xr-x   0        0        0      488 2023-02-19 18:37:34.753046 fedrq-0.6.0/srpm.sh
--rw-r--r--   0        0        0      154 2023-02-19 18:37:34.753046 fedrq-0.6.0/tests/.gitignore
--rw-r--r--   0        0        0     2912 2023-02-21 18:02:47.613086 fedrq-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0     1739 2023-02-21 18:02:47.614086 fedrq-0.6.0/tests/integration/test_backends.py
--rw-r--r--   0        0        0      636 2023-02-19 18:37:34.753046 fedrq-0.6.0/tests/integration/test_pkgs.py
--rw-r--r--   0        0        0     1219 2023-03-18 19:37:34.185930 fedrq-0.6.0/tests/integration/test_subpkgs.py
--rw-r--r--   0        0        0     1725 2023-02-19 18:37:34.753046 fedrq-0.6.0/tests/integration/test_whatrequires.py
--rw-r--r--   0        0        0     1334 2023-02-19 18:37:34.753046 fedrq-0.6.0/tests/integration/test_whatrequires_src.py
--rw-r--r--   0        0        0      332 2023-02-19 18:37:34.753046 fedrq-0.6.0/tests/test_data/_template.spec
--rwxr-xr-x   0        0        0     1449 2023-02-19 18:37:34.754046 fedrq-0.6.0/tests/test_data/build.sh
--rw-r--r--   0        0        0     1130 2023-02-19 18:37:34.754046 fedrq-0.6.0/tests/test_data/repos/repo1/specs/e1/packageb.spec
--rw-r--r--   0        0        0     1060 2023-02-19 18:37:34.754046 fedrq-0.6.0/tests/test_data/repos/repo1/specs/packagea.spec
--rw-r--r--   0        0        0     1156 2023-02-19 18:37:34.754046 fedrq-0.6.0/tests/test_data/repos/repo1/specs/packageb.spec
--rw-r--r--   0        0        0     2054 2023-03-18 19:37:34.185930 fedrq-0.6.0/tests/unit/test_checkconfig.py
--rw-r--r--   0        0        0     7127 2023-02-21 18:02:47.616086 fedrq-0.6.0/tests/unit/test_command.py
--rw-r--r--   0        0        0     7075 2023-02-21 18:02:47.617086 fedrq-0.6.0/tests/unit/test_formatters.py
--rw-r--r--   0        0        0      824 2023-03-18 19:37:34.185930 fedrq-0.6.0/tests/unit/test_pkgs.py
--rw-r--r--   0        0        0     1645 2023-03-18 19:37:34.185930 fedrq-0.6.0/tests/unit/test_release.py
--rw-r--r--   0        0        0      413 2023-02-21 18:02:47.618086 fedrq-0.6.0/tests/unit/test_repo.py
--rw-r--r--   0        0        0     1289 2023-03-20 17:10:06.077134 fedrq-0.6.0/tests/unit/test_repoquery.py
--rw-r--r--   0        0        0     2676 2023-02-19 18:37:34.755046 fedrq-0.6.0/tests/unit/test_subbpkgs.py
--rw-r--r--   0        0        0     4052 2023-03-17 01:22:48.917895 fedrq-0.6.0/tests/unit/test_whatrequires.py
--rw-r--r--   0        0        0      653 2023-02-19 18:37:34.755046 fedrq-0.6.0/tests/unit/test_whatrequires_src.py
--rw-r--r--   0        0        0    13999 1970-01-01 00:00:00.000000 fedrq-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      688 2023-05-28 23:13:09.924385 fedrq-0.7.0/.builds/epel9.yml
+-rw-r--r--   0        0        0     2406 2023-05-28 08:06:22.506837 fedrq-0.7.0/.builds/main.yml
+-rw-r--r--   0        0        0     1170 2023-05-28 23:13:09.924385 fedrq-0.7.0/.builds/mockbuild-36.yml
+-rw-r--r--   0        0        0      751 2023-03-18 19:37:34.175930 fedrq-0.7.0/.builds/mockbuild.yml
+-rw-r--r--   0        0        0      227 2023-02-19 18:37:34.746046 fedrq-0.7.0/.copr/Makefile
+-rwxr-xr-x   0        0        0      512 2023-02-19 18:37:34.746046 fedrq-0.7.0/.copr/mk.sh
+lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.7.0/.data/share/licenses/fedrq/GPL-2.0-or-later.txt -> ../../../../LICENSES/GPL-2.0-or-later.txt
+lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.7.0/.data/share/licenses/fedrq/MIT.txt -> ../../../../LICENSES/MIT.txt
+lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.7.0/.data/share/licenses/fedrq/PSF-2.0.txt -> ../../../../LICENSES/PSF-2.0.txt
+lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.7.0/.data/share/licenses/fedrq/Unlicense.txt -> ../../../../LICENSES/Unlicense.txt
+-rw-r--r--   0        0        0      268 2023-05-30 00:24:53.974774 fedrq-0.7.0/.gitignore
+-rw-r--r--   0        0        0     2482 2023-03-19 02:41:47.073223 fedrq-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    17337 2022-12-13 02:49:11.735043 fedrq-0.7.0/LICENSES/GPL-2.0-or-later.txt
+-rw-r--r--   0        0        0     1078 2022-12-13 02:49:11.735043 fedrq-0.7.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     2427 2023-02-19 18:37:34.747046 fedrq-0.7.0/LICENSES/PSF-2.0.txt
+-rw-r--r--   0        0        0     1211 2023-02-19 18:37:34.747046 fedrq-0.7.0/LICENSES/Unlicense.txt
+-rw-r--r--   0        0        0    12187 2023-05-30 00:25:30.044656 fedrq-0.7.0/NEWS.md
+-rw-r--r--   0        0        0       89 2023-03-18 21:16:55.983019 fedrq-0.7.0/NEWS.md.license
+-rw-r--r--   0        0        0    12144 2023-03-27 04:19:29.833647 fedrq-0.7.0/README.md
+-rwxr-xr-x   0        0        0      687 2023-04-09 15:43:04.496271 fedrq-0.7.0/contrib/add_frag.py
+-rwxr-xr-x   0        0        0      906 2023-03-19 23:05:00.923501 fedrq-0.7.0/contrib/api_examples/a_noarch_bash.py
+-rwxr-xr-x   0        0        0     2502 2023-03-19 23:05:00.924501 fedrq-0.7.0/contrib/api_examples/ftbfs_retirements.py
+-rw-r--r--   0        0        0      630 2023-03-19 23:07:21.352951 fedrq-0.7.0/contrib/deploy-docsite/main.yaml
+-rw-r--r--   0        0        0      183 2023-03-19 23:07:21.352951 fedrq-0.7.0/contrib/deploy-docsite/roles/configure/handlers/main.yaml
+-rw-r--r--   0        0        0      885 2023-03-19 23:07:21.352951 fedrq-0.7.0/contrib/deploy-docsite/roles/configure/tasks/main.yml
+-rw-r--r--   0        0        0      163 2023-03-19 23:07:21.352951 fedrq-0.7.0/contrib/deploy-docsite/roles/configure/templates/fedrq.caddyfile
+-rw-r--r--   0        0        0      415 2023-03-19 23:07:21.352951 fedrq-0.7.0/contrib/deploy-docsite/roles/deploy/tasks/main.yaml
+-rw-r--r--   0        0        0      156 2023-03-19 23:07:21.352951 fedrq-0.7.0/contrib/deploy-docsite/vars.yaml
+-rwxr-xr-x   0        0        0      914 2023-04-14 16:37:52.615305 fedrq-0.7.0/contrib/fedoraify.py
+-rw-r--r--   0        0        0     5728 2023-04-11 14:33:20.624926 fedrq-0.7.0/doc/API/Summary.md
+-rw-r--r--   0        0        0      147 2023-03-19 23:07:21.353951 fedrq-0.7.0/doc/API/backends/base.md
+-rw-r--r--   0        0        0      343 2023-04-11 19:16:07.821729 fedrq-0.7.0/doc/API/backends/dnf.md
+-rw-r--r--   0        0        0      532 2023-04-20 18:33:19.648796 fedrq-0.7.0/doc/API/backends/libdnf5.md
+-rw-r--r--   0        0        0      133 2023-03-19 23:07:21.353951 fedrq-0.7.0/doc/API/config.md
+-rw-r--r--   0        0        0      145 2023-03-19 23:07:21.353951 fedrq-0.7.0/doc/API/release_repo.md
+lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.7.0/doc/News.md -> ../NEWS.md
+-rw-r--r--   0        0        0     3322 2023-05-29 06:28:47.729780 fedrq-0.7.0/doc/dnf-repoquery-diff.md
+-rw-r--r--   0        0        0    16162 2023-05-29 23:47:52.009062 fedrq-0.7.0/doc/fedrq.1.scd
+-rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.7.0/doc/fedrq.1.scd.license
+-rw-r--r--   0        0        0     4958 2023-04-11 12:51:07.649356 fedrq-0.7.0/doc/fedrq.5.scd
+-rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.7.0/doc/fedrq.5.scd.license
+lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.7.0/doc/index.md -> ../README.md
+-rw-r--r--   0        0        0      131 2023-03-19 23:07:21.353951 fedrq-0.7.0/fedrq.rpmlintrc
+-rw-r--r--   0        0        0     3419 2023-05-30 00:25:29.984656 fedrq-0.7.0/fedrq.spec
+-rw-r--r--   0        0        0     2169 2023-04-11 19:22:07.524752 fedrq-0.7.0/mkdocs.yml
+-rw-r--r--   0        0        0    12445 2023-05-30 00:22:03.019335 fedrq-0.7.0/noxfile.py
+-rw-r--r--   0        0        0     2713 2023-05-30 00:25:22.777680 fedrq-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      532 2023-03-18 19:37:34.178930 fedrq-0.7.0/ruff.toml
+-rw-r--r--   0        0        0      281 2023-02-21 18:02:47.599086 fedrq-0.7.0/src/fedrq/__init__.py
+-rw-r--r--   0        0        0      219 2023-02-19 18:37:34.750046 fedrq-0.7.0/src/fedrq/__main__.py
+-rw-r--r--   0        0        0     1713 2023-02-21 18:02:47.600086 fedrq-0.7.0/src/fedrq/_compat.py
+-rw-r--r--   0        0        0      173 2023-03-18 19:37:34.178930 fedrq-0.7.0/src/fedrq/_config.py
+-rw-r--r--   0        0        0     1248 2023-03-18 19:37:34.179930 fedrq-0.7.0/src/fedrq/_utils.py
+-rw-r--r--   0        0        0     2529 2023-02-21 18:02:47.601086 fedrq-0.7.0/src/fedrq/backends/__init__.py
+-rw-r--r--   0        0        0    14439 2023-05-29 15:11:03.621468 fedrq-0.7.0/src/fedrq/backends/base.py
+-rw-r--r--   0        0        0      630 2023-02-21 18:02:47.603086 fedrq-0.7.0/src/fedrq/backends/dnf/__init__.py
+-rw-r--r--   0        0        0     6949 2023-05-29 06:34:45.893651 fedrq-0.7.0/src/fedrq/backends/dnf/backend.py
+-rw-r--r--   0        0        0      741 2023-02-21 18:02:47.604086 fedrq-0.7.0/src/fedrq/backends/libdnf5/__init__.py
+-rw-r--r--   0        0        0    28006 2023-05-29 23:47:52.135062 fedrq-0.7.0/src/fedrq/backends/libdnf5/backend.py
+-rw-r--r--   0        0        0     1955 2023-05-29 23:47:51.875063 fedrq-0.7.0/src/fedrq/cli/__init__.py
+-rw-r--r--   0        0        0    15680 2023-05-29 23:47:51.877063 fedrq-0.7.0/src/fedrq/cli/base.py
+-rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.7.0/src/fedrq/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2854 2023-03-18 19:37:34.182930 fedrq-0.7.0/src/fedrq/cli/commands/pkgs.py
+-rw-r--r--   0        0        0     1489 2023-05-29 23:47:51.877063 fedrq-0.7.0/src/fedrq/cli/commands/repolist.py
+-rw-r--r--   0        0        0     2425 2023-03-17 02:28:51.186103 fedrq-0.7.0/src/fedrq/cli/commands/subpkgs.py
+-rw-r--r--   0        0        0    10843 2023-03-18 19:37:34.182930 fedrq-0.7.0/src/fedrq/cli/commands/whatrequires.py
+-rw-r--r--   0        0        0    13071 2023-04-06 12:36:51.698430 fedrq-0.7.0/src/fedrq/cli/formatters.py
+-rw-r--r--   0        0        0    16722 2023-05-30 00:06:50.295329 fedrq-0.7.0/src/fedrq/config.py
+-rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.7.0/src/fedrq/data/__init__.py
+-rw-r--r--   0        0        0     7030 2023-05-29 23:47:52.009062 fedrq-0.7.0/src/fedrq/data/releases.toml
+-rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/data/repos/__init__.py
+-rw-r--r--   0        0        0     2053 2023-05-29 03:25:46.306279 fedrq-0.7.0/src/fedrq/data/repos/almalinux.repo
+-rw-r--r--   0        0        0      639 2023-03-27 04:19:29.835647 fedrq-0.7.0/src/fedrq/data/repos/amazonlinux.repo
+-rw-r--r--   0        0        0     1386 2023-05-29 03:25:46.306279 fedrq-0.7.0/src/fedrq/data/repos/centos-stream-compose.repo
+-rw-r--r--   0        0        0     1850 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/data/repos/centos-stream.repo
+-rw-r--r--   0        0        0     1494 2023-05-29 03:25:46.306279 fedrq-0.7.0/src/fedrq/data/repos/centos-stream8-compose.repo
+-rw-r--r--   0        0        0     1599 2023-03-18 19:37:34.184930 fedrq-0.7.0/src/fedrq/data/repos/centos-stream8.repo
+-rw-r--r--   0        0        0     1809 2023-05-29 03:58:29.496700 fedrq-0.7.0/src/fedrq/data/repos/eln.repo
+-rw-r--r--   0        0        0     2158 2023-05-29 03:25:46.306279 fedrq-0.7.0/src/fedrq/data/repos/epel.repo
+-rw-r--r--   0        0        0    14146 2023-05-29 03:25:46.419279 fedrq-0.7.0/src/fedrq/data/repos/fedora-eln.repo
+-rw-r--r--   0        0        0     2402 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/data/repos/fedora-rawhide.repo
+-rw-r--r--   0        0        0     1480 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/data/repos/fedora-updates-testing.repo
+-rw-r--r--   0        0        0     1422 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/data/repos/fedora-updates.repo
+-rw-r--r--   0        0        0     1375 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/data/repos/fedora.repo
+-rw-r--r--   0        0        0      425 2023-05-29 03:25:46.306279 fedrq-0.7.0/src/fedrq/data/repos/rawhide-buildroot.repo
+-rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/py.typed
+-rw-r--r--   0        0        0     8912 2023-05-28 01:30:25.101262 fedrq-0.7.0/src/fedrq/release_repo.py
+-rw-r--r--   0        0        0      984 2023-02-21 18:02:47.612086 fedrq-0.7.0/src/fedrq/repoquery.py
+-rwxr-xr-x   0        0        0      488 2023-02-19 18:37:34.753046 fedrq-0.7.0/srpm.sh
+-rw-r--r--   0        0        0      154 2023-02-19 18:37:34.753046 fedrq-0.7.0/tests/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-29 04:18:46.483879 fedrq-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     2912 2023-02-21 18:02:47.613086 fedrq-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:18:46.483879 fedrq-0.7.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1739 2023-02-21 18:02:47.614086 fedrq-0.7.0/tests/integration/test_backends.py
+-rw-r--r--   0        0        0      735 2023-05-28 08:06:22.609836 fedrq-0.7.0/tests/integration/test_pkgs.py
+-rw-r--r--   0        0        0     1219 2023-03-18 19:37:34.185930 fedrq-0.7.0/tests/integration/test_subpkgs.py
+-rw-r--r--   0        0        0     1725 2023-02-19 18:37:34.753046 fedrq-0.7.0/tests/integration/test_whatrequires.py
+-rw-r--r--   0        0        0     1334 2023-02-19 18:37:34.753046 fedrq-0.7.0/tests/integration/test_whatrequires_src.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:18:46.484879 fedrq-0.7.0/tests/test_data/__init__.py
+-rw-r--r--   0        0        0      332 2023-02-19 18:37:34.753046 fedrq-0.7.0/tests/test_data/_template.spec
+-rwxr-xr-x   0        0        0     1449 2023-02-19 18:37:34.754046 fedrq-0.7.0/tests/test_data/build.sh
+-rw-r--r--   0        0        0     1130 2023-02-19 18:37:34.754046 fedrq-0.7.0/tests/test_data/repos/repo1/specs/e1/packageb.spec
+-rw-r--r--   0        0        0     1060 2023-02-19 18:37:34.754046 fedrq-0.7.0/tests/test_data/repos/repo1/specs/packagea.spec
+-rw-r--r--   0        0        0     1156 2023-02-19 18:37:34.754046 fedrq-0.7.0/tests/test_data/repos/repo1/specs/packageb.spec
+-rw-r--r--   0        0        0        0 2023-05-29 04:18:46.484879 fedrq-0.7.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     2092 2023-05-29 15:11:03.621468 fedrq-0.7.0/tests/unit/test_checkconfig.py
+-rw-r--r--   0        0        0     7127 2023-05-28 01:58:42.063000 fedrq-0.7.0/tests/unit/test_command.py
+-rw-r--r--   0        0        0     7075 2023-02-21 18:02:47.617086 fedrq-0.7.0/tests/unit/test_formatters.py
+-rw-r--r--   0        0        0     2161 2023-05-29 23:47:52.009062 fedrq-0.7.0/tests/unit/test_pkgs.py
+-rw-r--r--   0        0        0     1645 2023-03-18 19:37:34.185930 fedrq-0.7.0/tests/unit/test_release.py
+-rw-r--r--   0        0        0      413 2023-02-21 18:02:47.618086 fedrq-0.7.0/tests/unit/test_repo.py
+-rw-r--r--   0        0        0      604 2023-05-29 23:47:51.877063 fedrq-0.7.0/tests/unit/test_repolist.py
+-rw-r--r--   0        0        0     1289 2023-03-20 17:10:06.077134 fedrq-0.7.0/tests/unit/test_repoquery.py
+-rw-r--r--   0        0        0     2676 2023-02-19 18:37:34.755046 fedrq-0.7.0/tests/unit/test_subbpkgs.py
+-rw-r--r--   0        0        0     4052 2023-03-17 01:22:48.917895 fedrq-0.7.0/tests/unit/test_whatrequires.py
+-rw-r--r--   0        0        0      653 2023-02-19 18:37:34.755046 fedrq-0.7.0/tests/unit/test_whatrequires_src.py
+-rw-r--r--   0        0        0    14085 1970-01-01 00:00:00.000000 fedrq-0.7.0/PKG-INFO
```

### Comparing `fedrq-0.6.0/.builds/epel9.yml` & `fedrq-0.7.0/.builds/epel9.yml`

 * *Files 3% similar despite different names*

```diff
@@ -15,10 +15,10 @@
       python3 -m venv venv
       ./venv/bin/pip install -U pip
       ./venv/bin/pip install nox
       EOF
       podman run -d -v $(pwd):/pwd:z -w /pwd --name c9ss --init centos:stream9 sleep infinity
       podman exec c9ss bash -xeu -o pipefail ./install.sh
   - pytest-py39: |
-      podman exec c9ss ./venv/bin/nox -e test -- -v
+      podman exec c9ss ./venv/bin/nox -e test -- -v --durations=7
   - typing-py39: |
       podman exec c9ss ./venv/bin/nox -e typing
```

### Comparing `fedrq-0.6.0/.builds/main.yml` & `fedrq-0.7.0/.builds/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -76,9 +76,9 @@
       tar czvf fedrq.tar.gz *.html
       hut pages publish fedrq.tar.gz -d gotmax23.srht.site -s "${site}"
   - lint: |
       cd fedrq
       $nox -e lint -- --check
   - pytest: |
       cd fedrq
-      FEDRQ_BACKEND=dnf $nox -e test -- -v
-      FEDRQ_BACKEND=libdnf5 $nox -e test -- -v
+      FEDRQ_BACKEND=dnf $nox -e test -- -v --durations=7
+      FEDRQ_BACKEND=libdnf5 $nox -e test -- -v --durations=7
```

### Comparing `fedrq-0.6.0/.builds/mockbuild-36.yml` & `fedrq-0.7.0/.builds/mockbuild-36.yml`

 * *Files 20% similar despite different names*

```diff
@@ -28,12 +28,11 @@
         --with libdnf5
       tar cvf results_fedrq.tar.gz results_fedrq
   - pytest-py310: |
       cd fedrq
       sudo dnf copr enable -y rpmsoftwaremanagement/dnf5-unstable
       sudo dnf install -y python3-libdnf5
       # Only run the integration tests. Units are run in the RPM build.
-      FEDRQ_BACKEND=dnf $nox -e test -- -v -k 'no_rpm_mock'
-      FEDRQ_BACKEND=libdnf5 $nox -e test -- -v -k 'no_rpm_mock'
+      FEDRQ_BACKEND=dnf $nox -e test -- -v -k 'no_rpm_mock' --durations=7
   - typing-py310: |
       cd fedrq
       $nox -e typing
```

### Comparing `fedrq-0.6.0/.builds/mockbuild.yml` & `fedrq-0.7.0/.builds/mockbuild.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/.copr/mk.sh` & `fedrq-0.7.0/.copr/mk.sh`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/CONTRIBUTING.md` & `fedrq-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/LICENSES/GPL-2.0-or-later.txt` & `fedrq-0.7.0/LICENSES/GPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/LICENSES/MIT.txt` & `fedrq-0.7.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/LICENSES/PSF-2.0.txt` & `fedrq-0.7.0/LICENSES/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/LICENSES/Unlicense.txt` & `fedrq-0.7.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/NEWS.md` & `fedrq-0.7.0/NEWS.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,90 @@
+NEWS
+=====
+
+## 0.7.0 - 2023-05-30 <a id='0.7.0'></a>
+
+### Highlighted examples
+
+fedrq now has a Fedora ELN release configuration builtin!
+
+You can preform simple queries
+
+```
+$ fedrq pkgs -b eln -F plainwithrepo ansible-core
+ansible-core-2.15.0-2.eln126.noarch eln-appstream
+ansible-core-2.15.0-2.eln126.src eln-appstream-source
+```
+
+or use more complex pipelines to determine how a package's build dependencies differ between ELN and Rawhide
+
+```
+$ comm -13 \
+    <(fedrq pkgs -b eln -s -F requires ansible-core | sort -u) \
+    <(fedrq pkgs -b rawhide -s -F requires ansible-core | sort -u)
+git-core
+glibc-all-langpacks
+python3dist(bcrypt)
+python3dist(passlib)
+python3dist(pexpect)
+python3dist(pytest)
+python3dist(pytest-forked)
+python3dist(pytest-mock)
+python3dist(pytest-xdist)
+python3dist(pywinrm)
+python3dist(pyyaml)
+python3-systemd
+/usr/bin/python
+```
+
+(This difference is expected, as tests are disabled when `%rhel` is defined.)
+
+fedrq also has a new `repolist` command to list enabled repos for a release.
+
+```
+$ fedrq repolist -b eln -r @no-crb
+eln-baseos
+eln-baseos-source
+eln-appstream
+eln-appstream-source
+```
+
+
+### Added
+
+- add `local` and `local:...` branches to allow querying the enabled system repos in
+- add `repolist` sucommand to display enabled repos
+  the same way that plain `dnf repoquery` does.
+- add Fedora ELN release configuration
+- add/document `@koji` and `@koji-src` generic repo classes
+
+---
+
+- add EPEL 9 packages to the upstream gotmax23/copr and gotmax23/copr-dev repositories
+- doc: add sig_policy.py to API examples
+- doc: add dnf and libdnf5 intersphinx
+
+### Changed
+
+- docs: show full function signatures w/ annotations
+- relicense CI files that are shared with tomcli to MIT
+- libdnf5 backend: use `libdnf5.conf.Vars.detect_release()` when available (libdnf5 >= 5.0.10)
+- backends: cache result of get_releasever()
+- config: check that release `matcher`s match the entire `--branch` not just
+  the beginning of it.
+
+### Fixed
+
+- doc: fix improper NEWS.md formatting
+- doc: correct `smartcache` description in fedrq(5).
+- libdnf5 backend: make the `BaseMaker.load_filelists()` method compatible with
+  libdnf5 >= 5.0.12.
+- packaging: remove remanent rpmautospec changelog file
+- packaging: remove unneeded fedora-repos-rawhide BR
+
 ## 0.6.0 - 2023-04-06 <a id="0.6.0"></a>
 
 ### Changed
 
 This release shouldn't introduce any backwards incompatibilities.
 
 ### Added
@@ -25,17 +108,14 @@
 - config: fix docstring typos and add links
 
 ### New contributors
 
 Thank you to Benson Muite (~bvkcm) for improving the README and correcting
 outdated information.
 
-NEWS
-=====
-
 ## 0.5.0 - 2023-03-18 <a id="0.5.0"></a>
 
 ### New dependencies
 - requests
 
 ### Highlighted examples
```

### Comparing `fedrq-0.6.0/README.md` & `fedrq-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/contrib/api_examples/a_noarch_bash.py` & `fedrq-0.7.0/contrib/api_examples/a_noarch_bash.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/contrib/api_examples/ftbfs_retirements.py` & `fedrq-0.7.0/contrib/api_examples/ftbfs_retirements.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/contrib/deploy-docsite/main.yaml` & `fedrq-0.7.0/contrib/deploy-docsite/main.yaml`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/contrib/deploy-docsite/roles/configure/tasks/main.yml` & `fedrq-0.7.0/contrib/deploy-docsite/roles/configure/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/contrib/fedoraify.py` & `fedrq-0.7.0/contrib/fedoraify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 # Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
 #
-# SPDX-License-Identifier: GPL-2.0-or-later
+# SPDX-License-Identifier: GPL-2.0-or-later OR MIT
 
 """
 Sync the upstream specfile with downstream.
 Include gpg signature and verify it.
 """
 
 import argparse
```

### Comparing `fedrq-0.6.0/doc/API/Summary.md` & `fedrq-0.7.0/doc/API/Summary.md`

 * *Files 3% similar despite different names*

```diff
@@ -125,11 +125,16 @@
 See [api-examples] for some simple example code.
 
 Real world examples:
 
 - [mkblocker.py] - given a list of source packages names, use jinja2 to
   template a specfile that Conflicts on every subpackage produced by the source
   packages. This was used as part of the [Mass_Retire_Golang_Leaves] Fedora Change.
+- [sig_policy.py] - enforces the FESCo [SIG Policy][sig-policy] by using fedrq
+  to find packages that meet certain criteria and adding the corresponding SIG
+  to the distgit repo's ACLs.
 
 [api-examples]: https://git.sr.ht/~gotmax23/fedrq/tree/main/item/contrib/api_examples
 [mkblocker.py]: https://git.sr.ht/~gotmax23/fedora-scripts/tree/main/item/go-sig/blocker/mkblocker.py
 [Mass_Retire_Golang_Leaves]: https://fedoraproject.org/wiki/Changes/Mass_Retire_Golang_Leaves#Implementation
+[sig_policy.py]: https://pagure.io/releng/blob/main/f/scripts/fesco/sig-policy/sig_policy.py
+[sig-policy]: https://docs.fedoraproject.org/en-US/fesco/SIG_policy/
```

### Comparing `fedrq-0.6.0/doc/dnf-repoquery-diff.md` & `fedrq-0.7.0/doc/dnf-repoquery-diff.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 Queries default to `rawhide` and enable the `rawhide` and `rawhide-source`
 repositories.
 This can be changed using the `-b` / `--branch` flags on the CLI or permanently
 with the `default_branch` option in the configuration.
 See the [BUILTIN RELEASES](../fedrq1/#builtin-releases) section of `man fedrq`
 for valid `--branch` options.
 Users can of course configure their own custom release profiles.
+You can use the pseudo `-b local` release which uses the default repositories
+with `enabled=1` in /etc/yum.repos.d and the system's releasever.
 
 ## Source repositories
 
 fedrq enables source repositories by default in its builtin release configs.
 While users are free to include whichever repositories they wish in their local
 configurations,
 commands such as `fedrq subpkgs` and `fedrq whatrequires-src` will not work
```

### Comparing `fedrq-0.6.0/doc/fedrq.1.scd` & `fedrq-0.7.0/doc/fedrq.1.scd`

 * *Files 5% similar despite different names*

```diff
@@ -205,14 +205,25 @@
 	with or without the *@*. See SPECIAL REPOS for which repo groups are
 	available for each release.
 *@repo:[key]* or *key* (fallback)
 	Accepts any repoid available in the system configuration or a .repo file
 	specific in the current ReleaseConfig's *defpaths*. If *key* is the name
 	of a release's repo group (see above), that will be enabled instead.
 
+The following generic repo class macros are available for Fedora releases:
+
+*@koji:[key]*
+	Load the repositories for a koji.fedoraproject.org tag. ++
+	Example: *@koji:f39-build-side-XXXX*
+*@koji-src:[key]*
+	Load the source repositories for a koji.fedoraproject.org tag.
+	It does not seem that Fedora Koji provides source repositories
+	for tags other than *rawhide* and *eln-build*.
+	For rawhide, see the preconfigured *@buildroot* repository group.
+
 
 
 # BUILTIN RELEASES
 
 [- Name
 :- Matcher (*--branch*)
 :- Release repo groups (*--repo*)
@@ -256,14 +267,30 @@
 :  @*base*, *@epel*, *@no-powertools*
 :  *@base* always includes powertools. *@epel* contains *@base* along with the EPEL
    repository. *@no-powertools* contains *@base* minus the powertools repository.
 |  Amazon Linux
 :  amazon2023
 :  *@base*
 : 
+|  Fedora ELN
+:  eln
+:  *@base*, *no-crb*
+: 
+|  Default local system repositories
+:  local
+:  N/A
+:  This uses the default repositories with *enabled=1* in /etc/yum.repos.d and
+   and the system's releasever.
+|  Default local system repositories with a different releasever
+:  local:[releasever]
+:  N/A
+:  This uses the default repositories with *enabled=1* in /etc/yum.repos.d and
+   and a custom releasever.
+
+; local should always be last in the above table
 
 ## SPECIAL REPOS
 
 
 *@base*
 	Release repositories enabled by default in the distribution++
 	(e.g. *fedora*, *fedora-source*, *updates*, *updates-source* for Fedora
```

### Comparing `fedrq-0.6.0/doc/fedrq.5.scd` & `fedrq-0.7.0/doc/fedrq.5.scd`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,18 @@
 
 # OPTIONS
 
 *default_branch* <str> (default: _rawhide_)
 	What branch to query by default when *-b*/*--branch* is not specified.
 *smartcache* <bool> (default: _true_)
 	Different releases have different _releasever_\s.
-	Switching the releasever clears the dnf cache.
+	Switching the releasever (i.e. passing a different value to *--branch*)
+	clears the dnf cache.
 	When *smartcache* is _true_\, fedrq sets *base.conf.cachedir* to
-	_/var/tmp/USER/BRANCH_ when changing the releasever.
+	_$XDG_CACHE_DIR/fedrq/BRANCH_ when changing the releasever.
 	The system cache is used if the requested branch's releasever is the
 	same as the system's releasever.
 *releases* <dict[str, ReleaseConfig]>
 	Keys are a friendly name for the distribution.
 	RELEASE specifies the format for the values.
 *filelists* <always|never|auto> (default: _auto_)
 	See *--filelists* in fedrq(1)
```

### Comparing `fedrq-0.6.0/fedrq.spec` & `fedrq-0.7.0/fedrq.spec`

 * *Files 15% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 # Copyright (C) 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: MIT
 # License text: https://spdx.org/licenses/MIT.html
 
 %bcond libdnf5 %[0%{?fedora} >= 38]
 
 Name:           fedrq
-Version:        0.6.0
+Version:        0.7.0
 Release:        1%{?dist}
 Summary:        A tool to query the Fedora and EPEL repositories
 
 # - code is GPL-2.0-or-later
 # - the data and config files in fedrq/data are UNLICENSEed
 # - Embeded repo defs are MIT.
 # - PSF-2.0 code copied from Cpython 3.11 for older Python versions
 License:        GPL-2.0-or-later AND Unlicense AND MIT AND PSF-2.0
 URL:            https://fedrq.gtmx.me
 %global furl    https://git.sr.ht/~gotmax23/fedrq
 Source0:        %{furl}/refs/download/v%{version}/fedrq-%{version}.tar.gz
 
 BuildArch:      noarch
 
+BuildRequires:  tomcli+tomlkit
 BuildRequires:  python3-devel
 # Test deps
 BuildRequires:  createrepo_c
-BuildRequires:  fedora-repos-rawhide
 BuildRequires:  distribution-gpg-keys
 BuildRequires:  python3-argcomplete
 BuildRequires:  python3-dnf
 %if %{with libdnf5}
 BuildRequires:  python3-libdnf5
 BuildRequires:  python3-rpm
 %endif
@@ -49,14 +49,17 @@
 %description
 fedrq is a tool to query the Fedora and EPEL repositories.
 
 
 %prep
 %autosetup -p1
 
+# See the comments in pyproject.toml
+tomcli-set pyproject.toml del tool.flit.external-data
+tomcli-set pyproject.toml list build-system.requires "flit_core >=3.2,<4"
 
 %generate_buildrequires
 %pyproject_buildrequires -x test
 
 
 %build
 %py3_shebang_fix contrib/api_examples/*.py
@@ -82,24 +85,27 @@
 %if %{with libdnf5}
 FEDRQ_BACKEND=libdnf5 %pytest -v -m "not no_rpm_mock"
 %endif
 
 
 %files -f %{pyproject_files}
 # Licenses are included in the wheel
-%license %{_licensedir}/fedrq/
+%license LICENSES/*.txt
 %doc README.md CONTRIBUTING.md NEWS.md contrib/api_examples
 %{_bindir}/fedrq*
 %{bash_completions_dir}/fedrq
 %{fish_completions_dir}/fedrq.fish
 %{_mandir}/man1/fedrq.1*
 %{_mandir}/man5/fedrq.5*
 
 
 %changelog
+* Tue May 30 2023 Maxwell G <maxwell@gtmx.me> - 0.7.0-1
+- Release 0.7.0.
+
 * Sat Apr 08 2023 Maxwell G <maxwell@gtmx.me> - 0.6.0-1
 - Release 0.6.0
 
 * Sat Mar 18 2023 Maxwell G <maxwell@gtmx.me> - 0.5.0-1
 - Release 0.5.0
 
 * Tue Mar 14 2023 Maxwell G <maxwell@gtmx.me> - 0.4.1-1
```

### Comparing `fedrq-0.6.0/mkdocs.yml` & `fedrq-0.7.0/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -45,18 +45,22 @@
       handlers:
         python:
           options:
             docstring_style: sphinx
             show_if_no_docstring: true
             merge_init_into_class: true
             filters: ["!^__?", "!LOG", "!logger"]
+            show_signature_annotations: true
+            separate_signature: true
           paths:
             - src/
           import:
             - https://docs.python.org/3/objects.inv
+            - https://dnf.readthedocs.io/en/latest/objects.inv
+            - https://dnf5.readthedocs.io/en/latest/objects.inv
   - exclude:
       glob:
         - "*.tar.gz"
         - "fedrq.1*"
         - "fedrq.5*"
 watch:
   - "README.md"
```

### Comparing `fedrq-0.6.0/noxfile.py` & `fedrq-0.7.0/noxfile.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # SPDX-FileCopyrightText: 2023 Maxwell G <gotmax@e.email>
 #
-# SPDX-License-Identifier: GPL-2.0-or-later
+# SPDX-License-Identifier: GPL-2.0-or-later OR MIT
 
 from __future__ import annotations
 
 import itertools
 import os
 import subprocess
+from collections.abc import Collection, Iterable
 from pathlib import Path
+from shutil import copy2, rmtree
 
 import nox
 import nox.command
 import nox.virtualenv
 
-nox.options.sessions = ("lint", "test", "libdnf5_test")
-
 IN_CI = "JOB_ID" in os.environ
 ALLOW_EDITABLE = os.environ.get("ALLOW_EDITABLE", str(not IN_CI)).lower() in (
     "1",
     "true",
 )
+LINT_SESSIONS = ("formatters", "codeql", "typing", "reuse")
+PROJECT = "fedrq"
+
+nox.options.sessions = (*LINT_SESSIONS, "test", "libdnf5_test")
 
 
 def install(session: nox.Session, *args, editable=False, **kwargs):
     if isinstance(session.virtualenv, nox.virtualenv.PassthroughEnv):
         session.warn(f"No venv. Skipping installation of {args}")
         return
     if editable and ALLOW_EDITABLE:
@@ -35,14 +39,18 @@
     kwargs.setdefault("text", True)
     kwargs.setdefault("stdout", subprocess.PIPE)
     kwargs.setdefault("check", True)
     proc = subprocess.run(args, **kwargs)
     return proc.stdout if return_stdout else proc
 
 
+def git(session: nox.Session, *args, **kwargs):
+    return session.run("git", *args, **kwargs, external=True)
+
+
 def _to_install_system(session, *packages: str):
     for package in packages:
         for whatprovides in [(), ("--whatprovides",), "yield"]:
             if whatprovides == "yield":
                 session.log(f"Installing RPM package {package!r}")
                 yield package
             if not subprocess.run(
@@ -95,23 +103,23 @@
     session.notify("test")
     session.notify("libdnf5_test")
 
 
 @nox.session(venv_params=["--system-site-packages"])
 def libdnf5_test(session: nox.Session):
     install_system(session, "python3-libdnf5")
-    test.func(session, "libdnf5")
+    test(session, "libdnf5")
 
 
 @nox.session(venv_backend="none")
 def lint(session: nox.Session):
     """
     Run format, codeql, typing, and reuse sessions
     """
-    for notify in ("formatters", "codeql", "typing", "reuse"):
+    for notify in LINT_SESSIONS:
         session.notify(notify)
 
 
 @nox.session()
 def codeql(session: nox.Session):
     install(
         session,
@@ -125,15 +133,15 @@
         *session.posargs,
         "src/fedrq/",
         "tests/",
         "noxfile.py",
     )
 
 
-@nox.session(venv_params=["--system-site-packages"])
+@nox.session
 def typing(session: nox.Session):
     install(session, ".[lint]", "-I", editable=True)
     session.run(
         "python", "-m", "mypy", "--enable-incomplete-feature=Unpack", "src/fedrq/"
     )
 
 
@@ -171,17 +179,17 @@
 
 @nox.session
 def reuse(session: nox.Session):
     install(session, "reuse")
     session.run("reuse", "lint")
 
 
-def install_fclogr(session: nox.Session):
+def install_fclogr(session: nox.Session, allow_local: bool = True):
     install_system(session, "rpm-build", "python3-rpm")
-    if Path("../fclogr").exists():
+    if allow_local and Path("../fclogr").exists():
         install(session, "-e", "../fclogr")
     else:
         install(session, "git+https://git.sr.ht/~gotmax23/fclogr#main")
 
 
 def _spec_changed(session: nox.Session) -> bool:
     if "fedrq.spec" not in run_silent("git", "diff", "--name-only", return_stdout=True):
@@ -205,30 +213,29 @@
         session.run("git", "restore", "fedrq.spec")
 
 
 @nox.session
 def srpm(session: nox.Session, posargs=None):
     posargs = posargs or session.posargs
     install_fclogr(session)
-    last_ref = run_silent("git", "describe", "--abbrev=0", "HEAD").stdout.strip()
-    session.run("fclogr", "--debug", "dev-srpm", "-r", last_ref, *posargs)
+    session.run("fclogr", "--debug", "dev-srpm", *posargs)
 
 
 @nox.session
 def mockbuild(session: nox.Session):
     install_system(session, "mock", "mock-core-configs")
     tmp = Path(session.create_tmp())
-    srpm.func(session, ("-o", tmp, "--keep"))
+    srpm(session, ("-o", tmp, "--keep"))
     spec_path = tmp / "fedrq.spec"
     margs = [
         "mock",
         "--spec",
-        spec_path,
+        str(spec_path),
         "--source",
-        tmp,
+        str(tmp),
         *session.posargs,
     ]
     if not session.interactive:
         margs.append("--verbose")
     if not {
         "--clean",
         "--no-clean",
@@ -237,23 +244,140 @@
         "-n",
         "-N",
     } & set(session.posargs):
         margs.insert(1, "-N")
     session.run(*margs, external=True)
 
 
-@nox.session(venv_backend="none")
+def ensure_clean(session: nox.Session):
+    if git(session, "status", "--porcelain", "--untracked-files", silent=True):
+        msg = "There are untracked and/or modified files."
+        session.error(msg)
+
+
+def _check_git_tag(session: nox.Session, version: str):
+    tag = "v" + version
+    tags = git(session, "tag", "--list", silent=True).splitlines()
+    if tag in tags:
+        session.error(f"{tag} is already tagged")
+
+
+@nox.session
 def bump(session: nox.Session):
-    session.run("bash", "-x", "contrib/bump.sh", *session.posargs)
+    version = session.posargs[0]
+    _check_git_tag(session, version)
+    ensure_clean(session)
+
+    install(session, "flit>=3.9", "tomcli[tomlkit]", "twine")
+    install_fclogr(session, False)
+
+    # Download generate_changelog
+    tmp = Path(session.create_tmp())
+    with session.chdir(tmp):
+        session.run_always(
+            "wget",
+            "https://git.sr.ht/~gotmax23/fedora-scripts/blob/main/generate_changelog.py",
+            external=True,
+        )
+
+    # Update version
+    session.run("tomcli-set", "pyproject.toml", "str", "project.version", version)
+
+    install(session, ".")
+
+    # Bump specfile
+    session.run(
+        "fclogr",
+        "bump",
+        "--new",
+        version,
+        "--comment",
+        f"Release {version}.",
+        f"{PROJECT}.spec",
+    )
+
+    # Bump changelog, commit, and tag
+    git(session, "add", f"{PROJECT}.spec", "pyproject.toml")
+    session.run(
+        "python", str(tmp / "generate_changelog.py"), f"--version={version}", "--tag"
+    )
+
+    if Path("dist").is_dir():
+        rmtree("dist")
+    session.run("flit", "build", "--use-vcs")
+    artifacts = _get_artifacts(("*.whl", "*.tar.gz"), expected_count=2)
+    session.run("twine", "check", "--strict", *artifacts)
+    _sign_artifacts(session)
+
+
+def _sign_artifacts(session: nox.Session) -> None:
+    uid = git(session, "config", "user.email", silent=True).strip()
+    artifacts = _get_artifacts(["tar.gz", "whl"], expected_count=2)
+    for path in artifacts:
+        if Path(path + ".asc").exists():
+            session.warn(f"{path}.asc already exists. Not signing it.")
+            continue
+        session.run(
+            "gpg", "--local-user", uid, "--armor", "--detach-sign", path, external=True
+        )
+
+
+def _get_artifacts(
+    exts: Collection[str] = ("whl", "tar.gz", "tar.gz.asc", "whl.asc"),
+    required=True,
+    extra_allowed=True,
+    expected_count: int | None = None,
+) -> Iterable[str]:
+    count = 0
+    all_files = set(Path("dist").iterdir())
+    for ext in exts:
+        found = tuple(Path("dist").glob(f"*.{ext}"))
+        if not found and required:
+            raise ValueError(f"No matches for {ext}")
+        count += len(found)
+        for file in found:
+            all_files.remove(file)
+        yield from map(str, found)
+    if all_files and not extra_allowed:
+        raise ValueError(f"Extra files found in dist: {all_files}")
+    if expected_count is not None and count != expected_count:
+        raise ValueError(f"Found {count} artifacts. Expected {expected_count}.")
 
 
 @nox.session
 def publish(session: nox.Session):
-    install(session, "copr", "dbus-python", "flit", "keyring", "twine")
-    session.run("bash", "-x", "contrib/publish.sh", *session.posargs)
+    # Setup
+    ensure_clean(session)
+    install(session, "twine", "tomcli[tomlkit]")
+    session.run(
+        "twine",
+        "upload",
+        "--non-interactive",
+        "--username",
+        "__token__",
+        *_get_artifacts(("*.whl", "*.tar.gz"), extra_allowed=False, expected_count=2),
+    )
+
+    # Copr build
+    copr_release(session)
+
+    # Push to git
+    if session.interactive and input("Push to Sourcehut (Y/n)").lower() != "n":
+        git(session, "push", "--follow-tags")
+        srht_artifacts(session)
+
+    # Post-release bump
+    version = session.run(  # type: ignore[union-attr]
+        "tomcli-get", "pyproject.toml", "project.version", silent=True
+    ).strip()
+    session.run(
+        "tomcli-set", "pyproject.toml", "str", "project.version", f"{version}.post0"
+    )
+    git(session, "add", "pyproject.toml")
+    git(session, "commit", "-S", "-m", "Post release version bump")
 
 
 @nox.session
 def docgen(session: nox.Session):
     """
     Generate extra content for the docsite
     """
@@ -276,11 +400,27 @@
             f"> doc/fedrq{i}.md",
             external=True,
         )
         # fmt: on
 
 
 @nox.session
+def copr_release(session: nox.Session):
+    install(session, "copr-cli", "requests-gssapi", "specfile")
+    tmp = Path(session.create_tmp())
+    dest = tmp / "tomcli.spec"
+    copy2("tomcli.spec", dest)
+    session.run("python", "contrib/fedoraify.py", str(dest))
+    session.run("copr-cli", "build", "--nowait", "gotmax23/tomcli", str(dest))
+
+
+@nox.session(python="none")
+def srht_artifacts(session: nox.Session):
+    artifacts = map(str, Path("dist").glob("*"))
+    session.run("hut", "git", "artifact", "upload", *artifacts, external=True)
+
+
+@nox.session
 def mkdocs(session: nox.Session):
     install(session, "-e", ".[doc]")
-    docgen.func(session)
+    docgen(session)
     session.run("mkdocs", *session.posargs)
```

### Comparing `fedrq-0.6.0/pyproject.toml` & `fedrq-0.7.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 requires = ["flit_core >=3.7,<4"]
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "fedrq"
 description = "fedrq is a tool to query the Fedora and EPEL repositories"
-version = "0.6.0"
+version = "0.7.0"
 authors = [{ name = "Maxwell G", email = "gotmax@e.email" }]
 readme = "README.md"
 license = { text = "GPL-2.0-or-later AND Unlicense AND MIT" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -54,28 +54,31 @@
 ]
 test = [
     "pytest",
     "pytest-mock",
     "tomli-w",
 ]
 doc = [
+    # mkdocstrings-python uses this to format function signatures
+    "black",
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings[python]>=0.18",
     "mkdocs-exclude",
 ]
 dev = [
     "fedrq[test]",
     "fedrq[lint]",
 ]
 
 [project.urls]
-Homepage = "https://sr.ht/~gotmax23/fedrq"
-Source = "https://git.sr.ht/~gotmax23/fedrq"
+Homepage = "https://fedrq.gtmx.me"
+Changelog = "https://fedrq.gtmx.me/Changelog"
 "Mailing List" = "https://lists.sr.ht/~gotmax23/fedrq"
+Source = "https://git.sr.ht/~gotmax23/fedrq"
 
 [project.scripts]
 fedrq = "fedrq.cli:main"
 
 [tool.flit.sdist]
 include = [
     "src/fedrq/data/",
```

### Comparing `fedrq-0.6.0/ruff.toml` & `fedrq-0.7.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/_compat.py` & `fedrq-0.7.0/src/fedrq/_compat.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/_utils.py` & `fedrq-0.7.0/src/fedrq/_utils.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/backends/__init__.py` & `fedrq-0.7.0/src/fedrq/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/backends/base.py` & `fedrq-0.7.0/src/fedrq/backends/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,15 +341,17 @@
     def load_release_repos(self, release: Release, set_releasever: bool = True) -> None:
         """
         Load the repositories from a fedrq.config.Release object
         """
         if set_releasever:
             self.set_var("releasever", release.version)
         if release.release_config.system_repos:
-            self.read_system_repos()
+            self.read_system_repos(
+                disable=not release.release_config.append_system_repos
+            )
         for path in release.release_config.full_def_paths:
             with importlib.resources.as_file(path) as fp:
                 LOG.debug("Reading %s", fp)
                 self._read_repofile_new(fp)
         release.repog.load(self, release.config, release)
 
     @abc.abstractmethod
```

### Comparing `fedrq-0.6.0/src/fedrq/backends/dnf/__init__.py` & `fedrq-0.7.0/src/fedrq/backends/dnf/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/backends/dnf/backend.py` & `fedrq-0.7.0/src/fedrq/backends/dnf/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from __future__ import annotations
 
 import logging
 import sys
 import typing as t
 from collections.abc import Collection
+from functools import cache
 
 from fedrq._utils import filter_latest
 from fedrq.backends import MissingBackendError
 from fedrq.backends.base import (
     BackendMod,
     BaseMakerBase,
     PackageCompat,
@@ -198,14 +199,15 @@
         return query
 
     @property
     def backend(self) -> BackendMod:
         return sys.modules[__name__]
 
 
+@cache
 def get_releasever():
     """
     Return the system releasever
     """
     return dnf.rpm.detect_releasever("/")
```

### Comparing `fedrq-0.6.0/src/fedrq/backends/libdnf5/__init__.py` & `fedrq-0.7.0/src/fedrq/backends/libdnf5/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/backends/libdnf5/backend.py` & `fedrq-0.7.0/src/fedrq/backends/libdnf5/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 [`fedrq.backends.base.BackendMod`][fedrq.backends.base.BackendMod] interface)
 that uses the libdnf5 Python bindings.
 """
 
 from __future__ import annotations
 
 import functools
+import inspect
 import logging
 import sys
 import typing as t
 from collections.abc import Collection, Iterable
 
 from fedrq._utils import filter_latest
 from fedrq.backends import MissingBackendError
@@ -355,15 +356,19 @@
         repoq = libdnf5.repo.RepoQuery(self.base)
         repoq.filter_id([name])
         return next(iter(repoq), None)
 
     def load_filelists(self) -> None:
         LOG.debug("Loading filelists")
         option = self._get_option(self.config, "optional_metadata_types")
-        option.add_item(libdnf5.conf.METADATA_TYPE_FILELISTS)
+        func = option.add_item
+        if "priority" in inspect.signature(func).parameters:
+            func(Priority_RUNTIME, libdnf5.conf.METADATA_TYPE_FILELISTS)
+        else:
+            func(libdnf5.conf.METADATA_TYPE_FILELISTS)
 
     def create_repo(self, repoid: str, **kwargs) -> None:
         """
         Add a Repo object to the repo sack and configure it.
         :param kwargs: key-values options that should be set on the Repo object
                        values (like $basearch) will be substituted automatically.
         """
@@ -798,27 +803,16 @@
         return r_query
 
     @property
     def backend(self) -> BackendMod:
         return sys.modules[__name__]
 
 
-def get_releasever() -> str:
-    """
-    Return the system releasever
-    """
-    # # Creating a second Base object just to retrieve this value is
-    # # prohibitively expensive.
-    # base = libdnf5.base.Base()
-    # base.load_config_from_file()
-    # base.setup()
-    # return base.get_vars().get_value("releasever")
-
-    # This is taken from dnf and slightly modified until
-    # https://github.com/rpm-software-management/dnf5/issues/281 is resolved.
+def _dnf_getreleasever() -> str:
+    # This is taken from dnf and slightly modified
     #
     # SPDX-License-Identifier: GPL-2.0-or-later
     # Copyright (C) 2012-2015  Red Hat, Inc.
     DISTROVERPKG = (
         "system-release(releasever)",
         "system-release",
         "distribution-release(releasever)",
@@ -860,14 +854,28 @@
                 releasever = releasever.decode("utf-8")
             return releasever
         return ""
     finally:
         ts.closeDB()
 
 
+@functools.cache
+def get_releasever() -> str:
+    """
+    Return the system releasever
+    """
+    # libdnf5 > 5.0.10
+    if hasattr(libdnf5.conf.Vars, "detect_release"):
+        base = libdnf5.base.Base()
+        return libdnf5.conf.Vars.detect_release(base.get_weak_ptr(), "/").get()
+    # Fall back to our copy of dnf4's code
+    else:
+        return _dnf_getreleasever()
+
+
 RepoError = RuntimeError
 
 __all__ = (
     "BACKEND",
     "BaseMaker",
     "Package",
     "PackageQuery",
```

### Comparing `fedrq-0.6.0/src/fedrq/cli/__init__.py` & `fedrq-0.7.0/src/fedrq/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 except ImportError:
     HAS_ARGCOMPLETE = False
 else:
     HAS_ARGCOMPLETE = True
 
 from fedrq.cli.base import CheckConfig, Command
 from fedrq.cli.commands.pkgs import Pkgs
+from fedrq.cli.commands.repolist import Repolist
 from fedrq.cli.commands.subpkgs import Subpkgs
 from fedrq.cli.commands.whatrequires import (
     WhatCommand,
     Whatenhances,
     Whatobsoletes,
     Whatrecommends,
     Whatrequires,
@@ -27,14 +28,15 @@
     Whatsuggests,
     Whatsupplements,
 )
 
 __all__ = (
     "Command",
     "Pkgs",
+    "Repolist",
     "Subpkgs",
     "WhatCommand",
     "Whatenhances",
     "Whatobsoletes",
     "Whatrecommends",
     "Whatrequires",
     "WhatrequiresSrc",
@@ -59,14 +61,15 @@
     return COMMANDS[args.action](args).run()
 
 
 COMMANDS: dict[str, type[Command]] = {
     "check-config": CheckConfig,
     "pkgs": Pkgs,
     "subpkgs": Subpkgs,
+    "repolist": Repolist,
     "whatenhances": Whatenhances,
     "whatobsoletes": Whatobsoletes,
     "whatrecommends": Whatrecommends,
     "whatrequires": Whatrequires,
     "wr": Whatrequires,
     "whatrequires-src": WhatrequiresSrc,
     "wrsrc": WhatrequiresSrc,
```

### Comparing `fedrq-0.6.0/src/fedrq/cli/base.py` & `fedrq-0.7.0/src/fedrq/cli/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import logging
 import re
 import sys
 from functools import wraps
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
+from fedrq.backends.base import BaseMakerBase
+
 try:
     import tomli_w
 except ImportError:
     HAS_TOMLI_W = False
 else:
     HAS_TOMLI_W = True
 
@@ -163,29 +165,58 @@
         avoid a performance penalty.
         """
         if logger.getEffectiveLevel() <= level:
             logger.debug("%s = %s", name, tuple(query))
         return query
 
     @classmethod
-    def parent_parser(cls) -> argparse.ArgumentParser:
+    def branch_repo_parser(cls) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser(add_help=False)
-        parser.add_argument(  # type: ignore[attr-defined]
-            "names", metavar="NAME", nargs="*", help="Mutually exclusive with --stdin"
-        ).completer = lambda **_: ()
-        parser.add_argument(
-            "-i", "--stdin", help="Read package names from stdin.", action="store_true"
-        )
         parser.add_argument(
             "-b",
             "--branch",
             help="Fedora or EPEL branch name "
             "(e.g. epel7, rawhide, epel9-next, f37) to query",
         )
         parser.add_argument("-r", "--repos", default="base")
+        parser.add_argument(
+            "-e",
+            "--enablerepo",
+            dest="enable_disable",
+            default=[],
+            action=_EnableDisableRepo,
+            metavar="REPO",
+            help="""
+            Enable certain repositories for the duration of this operation.
+            All repositories in the system configuration and any additional
+            defs in the selected branch are available.
+            """,
+        )
+        parser.add_argument(
+            "--disablerepo",
+            dest="enable_disable",
+            default=[],
+            action=_EnableDisableRepo,
+            metavar="REPO",
+            # PROVISIONAL
+            help=argparse.SUPPRESS,
+        )
+        return parser
+
+    @classmethod
+    def parent_parser(cls) -> argparse.ArgumentParser:
+        parser = argparse.ArgumentParser(
+            add_help=False, parents=[cls.branch_repo_parser()]
+        )
+        parser.add_argument(  # type: ignore[attr-defined]
+            "names", metavar="NAME", nargs="*", help="Mutually exclusive with --stdin"
+        ).completer = lambda **_: ()
+        parser.add_argument(
+            "-i", "--stdin", help="Read package names from stdin.", action="store_true"
+        )
         parser.add_argument("-l", "--latest", default=1, help="'all' or an intenger")
         parser.add_argument(  # type: ignore[attr-defined]
             "-F",
             "--formatter",
             default="plain",
         ).completer = cls.formatters._argcompleter
         cachedir_group = parser.add_mutually_exclusive_group()
@@ -219,36 +250,14 @@
             " which doesn't load filelists by default to save memory and bandwidth."
             " dnf4 always loads filelists.",
         )
         parser.add_argument("-B", "--backend", choices=tuple(BACKENDS))
         parser.add_argument(
             "--forcearch", help="Query a foreign architecture's repositories"
         )
-        parser.add_argument(
-            "-e",
-            "--enablerepo",
-            dest="enable_disable",
-            default=[],
-            action=_EnableDisableRepo,
-            metavar="REPO",
-            help="""
-            Enable certain repositories for the duration of this operation.
-            All repositories in the system configuration and any additional
-            defs in the selected branch are available.
-            """,
-        )
-        parser.add_argument(
-            "--disablerepo",
-            dest="enable_disable",
-            default=[],
-            action=_EnableDisableRepo,
-            metavar="REPO",
-            # PROVISIONAL
-            help=argparse.SUPPRESS,
-        )
         return parser
 
     @classmethod
     @abc.abstractmethod
     def make_parser(
         cls,
         parser_func: cabc.Callable = argparse.ArgumentParser,
@@ -328,14 +337,23 @@
     def v_release(self) -> str | None:
         try:
             self.release = self.config.get_release(self.args.branch, self.args.repos)
         except ConfigError as err:
             return str(err)
         return None
 
+    def _enable_disable_bm(self, bm: BaseMakerBase):
+        for func, repo in self.args.enable_disable:
+            if func == "enable":
+                self.release.get_repog(repo).load(bm, self.config, self.release)
+            elif func == "disable":
+                bm.disable_repo(repo, True)
+            else:
+                raise ValueError
+
     @v_fatal_error
     def v_rq(self) -> str | None:
         conf: dict[str, Any] = {}
         bvars: dict[str, Any] = {}
 
         # Set cachedir if it's explicitly passed
         if self.args.cachedir:
@@ -347,21 +365,15 @@
 
         if self.args.forcearch:
             conf["ignorearch"] = True
             bvars["arch"] = self.args.forcearch
         bm = self.backend.BaseMaker()
         try:
             self.release.make_base(self.config, conf, bvars, bm, False)
-            for func, repo in self.args.enable_disable:
-                if func == "enable":
-                    self.release.get_repog(repo).load(bm, self.config, self.release)
-                elif func == "disable":
-                    bm.disable_repo(repo, True)
-                else:
-                    raise ValueError
+            self._enable_disable_bm(bm)
         except ConfigError as exc:
             return str(exc)
         self.rq = self.backend.Repoquery(bm.fill_sack())
         return None
 
     @v_fatal_error
     def v_backend(self) -> str | None:
@@ -443,7 +455,36 @@
             sys.exit(f"default_branch '{self.config.default_branch}' is invalid")
         if not self.args.dump:
             print("No validation errors found!")
         else:
             flog.debug("Removing Nones from configuration dict")
             data_dict = self._strip_nones(json.loads(self.config.json()))
             tomli_w.dump(data_dict, sys.stdout.buffer)
+
+
+# class CommandBoilerplate(Command):
+#     """
+#     Help text
+#     """
+#     def __init__(self, args: argparse.Namespace) -> None:
+#         super().__init__(args)
+#         self.v_default()
+
+#     @classmethod
+#     def make_parser(
+#         cls,
+#         parser_func: cabc.Callable = argparse.ArgumentParser,
+#         *,
+#         add_help: bool = False,
+#         **kwargs,
+#     ) -> argparse.ArgumentParser:
+#         kwargs["description"] = cls.__doc__
+#         kwargs["parents"] = [cls.parent_parser()]
+#         if add_help:
+#             kwargs["help"] = cls.__doc__
+
+#         parser = parser_func(**kwargs)
+#         ...
+#         return parser
+
+#     def run(self) -> None:
+#         ...
```

### Comparing `fedrq-0.6.0/src/fedrq/cli/commands/pkgs.py` & `fedrq-0.7.0/src/fedrq/cli/commands/pkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/cli/commands/subpkgs.py` & `fedrq-0.7.0/src/fedrq/cli/commands/subpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/cli/commands/whatrequires.py` & `fedrq-0.7.0/src/fedrq/cli/commands/whatrequires.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/cli/formatters.py` & `fedrq-0.7.0/src/fedrq/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/config.py` & `fedrq-0.7.0/src/fedrq/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,22 +60,24 @@
     def __bool__(self) -> bool:
         return self == LoadFilelists.always
 
 
 class ReleaseConfig(BaseModel):
     name: str = Field(exclude=True)
     defs: dict[str, list[str]]
+    version: t.Optional[str] = None
     matcher: t.Pattern
     repo_dirs: list[Path] = Field(
         default_factory=lambda: [
             directory.joinpath("repos") for directory in CONFIG_DIRS
         ]
     )
     defpaths: set[str] = Field(default_factory=set)
     system_repos: bool = True
+    append_system_repos: bool = False
 
     koschei_collection: t.Optional[str] = None
     copr_chroot_fmt: t.Optional[str] = None
 
     full_def_paths: t.ClassVar[list[t.Union[Traversable, Path]]] = []
     repo_aliases: dict[str, str] = {}
     _repogs = PrivateAttr()
@@ -96,27 +98,33 @@
         flog.debug(f"Getting defpaths for {values['name']}: {value}")
         values["full_def_paths"] = cls._get_full_defpaths(
             values["name"], value.copy(), values["repo_dirs"]
         )
         return value
 
     @validator("matcher")
-    def v_matcher(cls, value: t.Pattern) -> t.Pattern:
-        if value.groups != 1:
+    def v_matcher(cls, value: t.Pattern, values: dict[str, t.Any]) -> t.Pattern:
+        if not values["version"] and value.groups != 1:
             raise ValueError("'matcher' must have exactly one capture group")
         return value
 
     @validator("repo_dirs", pre=True)
     def v_repo_dirs(cls, value: str | list[Path]) -> list[Path]:
         if not isinstance(value, str):
             return value
         return [Path(directory) for directory in value.split(":")]
 
+    @validator("append_system_repos", always=True)
+    def v_append_system_repos(cls, value: bool, values: dict[str, t.Any]) -> bool:
+        if value:
+            values["system_repos"] = True
+        return value
+
     def is_match(self, val: str) -> bool:
-        return bool(re.match(self.matcher, val))
+        return bool(re.fullmatch(self.matcher, val))
 
     def is_valid_repo(self, val: str) -> bool:
         try:
             self.repogs.get_repo(val)
         except ConfigError:
             return False
         else:
@@ -214,17 +222,25 @@
         self.repog: RepoG = self.get_repog(repo_name)
 
     def get_repog(self, key: str) -> RepoG:
         return self.release_config.repogs.get_repo(key)
 
     @property
     def version(self) -> str:
-        if match := re.match(self.release_config.matcher, self.branch):
-            return match.group(1)
-        raise ValueError(f"{self.branch} does not match {self.release_config.name}")
+        v: str | None = None
+        if self.release_config.version:
+            v = self.release_config.version
+        elif match := re.fullmatch(self.release_config.matcher, self.branch):
+            v = match.group(1)
+        if v is None:
+            raise ValueError(f"{self.branch} does not match {self.release_config.name}")
+        # Special case
+        if v == "$releasever":
+            v = self.config.backend_mod.get_releasever()
+        return v
 
     @property
     def copr_chroot_fmt(self) -> str | None:
         return self.release_config.copr_chroot_fmt
 
     @property
     def koschei_collection(self) -> str | None:
```

### Comparing `fedrq-0.6.0/src/fedrq/data/releases.toml` & `fedrq-0.7.0/src/fedrq/data/releases.toml`

 * *Files 13% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 defs.buildroot = ["fedrq-koji-rawhide", "fedrq-koji-rawhide-source"]
 # fedrq will search for the repository names in the following
 # paths if they're not available in your system configuration.
 defpaths = ["rawhide-buildroot.repo", "fedora-rawhide.repo"]
 system_repos = true
 # Example usage: `fedrq CMD -r @koji:f39-build-side-XXXX`
 repo_aliases.koji = "@baseurl:https://kojipkgs.fedoraproject.org/repos/{}/latest/$basearch"
+repo_aliases.koji-src = "@baseurl:https://kojipkgs.fedoraproject.org/repos/{}/latest/src"
 
 [releases.branched]
 # e.g. f36, f37
 matcher = "^f(\\d{2})$"
 koschei_collection = "Fedora {version}"
 copr_chroot_fmt = "fedora-{version}"
 
@@ -34,14 +35,15 @@
 defs.updates = ["@repo:updates", "updates-source"]
 defs.testing =  ["fedora", "fedora-source", "updates", "updates-source",
                  "updates-testing", "updates-testing-source"]
 defs.testing-only =  ["updates-testing", "updates-testing-source"]
 
 defpaths = ["fedora.repo", "fedora-updates.repo", "fedora-updates-testing.repo"]
 repo_aliases.koji = "@baseurl:https://kojipkgs.fedoraproject.org/repos/{}/latest/$basearch"
+repo_aliases.koji-src = "@baseurl:https://kojipkgs.fedoraproject.org/repos/{}/latest/src"
 
 [releases.epel]
 # e.g. epel8, epel9, epel10
 matcher = "^epel(\\d{1,2})$"
 koschei_collection = "EPEL {version}"
 copr_chroot_fmt = "epel-{version}"
 defpaths = ["epel.repo"]
@@ -213,7 +215,35 @@
 ]
 defs.no-powertools = [
     "almalinux-appstream",
     "almalinux-appstream-source",
     "almalinux-baseos",
     "almalinux-baseos-source",
 ]
+
+[releases.eln]
+matcher = "^(eln)$"
+defpaths = [
+    "fedora-eln.repo",
+]
+defs.no-crb = [
+    "eln-baseos",
+    "eln-baseos-source",
+    "eln-appstream",
+    "eln-appstream-source",
+]
+defs.base = [
+    "@no-crb",
+    "eln-crb",
+    "eln-crb-source",
+]
+
+[releases.local]
+matcher = "local"
+version = "$releasever"
+append_system_repos = true
+defs.base = []
+
+[releases.local-custom]
+matcher = "local:(.*)"
+append_system_repos = true
+defs.base = []
```

### Comparing `fedrq-0.6.0/src/fedrq/data/repos/almalinux.repo` & `fedrq-0.7.0/src/fedrq/data/repos/almalinux.repo`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# SPDX-FileCopyrightText: None
 # SPDX-License-Identifier: Unlicense
+# SPDX-FileCopyrightText: None
 
 [almalinux-baseos]
 name=AlmaLinux $releasever - BaseOS
 mirrorlist=https://mirrors.almalinux.org/mirrorlist/$releasever/baseos
 enabled=0
 gpgcheck=1
 gpgkey=file:///usr/share/distribution-gpg-keys/alma/RPM-GPG-KEY-AlmaLinux-$releasever
```

### Comparing `fedrq-0.6.0/src/fedrq/data/repos/amazonlinux.repo` & `fedrq-0.7.0/src/fedrq/data/repos/amazonlinux.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/data/repos/centos-stream-compose.repo` & `fedrq-0.7.0/src/fedrq/data/repos/centos-stream-compose.repo`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# SPDX-FileCopyrightText: None
 # SPDX-License-Identifier: Unlicense
+# SPDX-FileCopyrightText: None
 
 [centos-stream-compose-latest-appstream]
 name = centos-stream-compose-latest-appstream
 baseurl = https://composes.stream.centos.org/production/latest-CentOS-Stream/compose/AppStream/$basearch/os/
 enabled = 0
 gpgcheck = 0
```

### Comparing `fedrq-0.6.0/src/fedrq/data/repos/centos-stream.repo` & `fedrq-0.7.0/src/fedrq/data/repos/centos-stream.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/data/repos/centos-stream8-compose.repo` & `fedrq-0.7.0/src/fedrq/data/repos/centos-stream8-compose.repo`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# SPDX-FileCopyrightText: None
 # SPDX-License-Identifier: Unlicense
+# SPDX-FileCopyrightText: None
 
 [centos-stream8-compose-latest-appstream]
 name = centos-stream8-compose-latest-appstream
 baseurl = https://composes.stream.centos.org/stream-8/production/latest-CentOS-Stream/compose/AppStream/$basearch/os/
 enabled = 0
 gpgcheck = 0
```

### Comparing `fedrq-0.6.0/src/fedrq/data/repos/centos-stream8.repo` & `fedrq-0.7.0/src/fedrq/data/repos/centos-stream8.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/data/repos/epel.repo` & `fedrq-0.7.0/src/fedrq/data/repos/epel.repo`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: Unlicense
+# SPDX-FileCopyrightText: None
 
 [epel]
 name = "epel"
 metalink = "https://mirrors.fedoraproject.org/metalink?repo=epel-$releasever&arch=$basearch"
 gpgkey = "file:///usr/share/distribution-gpg-keys/epel/RPM-GPG-KEY-EPEL$releasever"
 gpgcheck = True
 enabled = False
```

### Comparing `fedrq-0.6.0/src/fedrq/data/repos/fedora-rawhide.repo` & `fedrq-0.7.0/src/fedrq/data/repos/fedora-rawhide.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/data/repos/fedora-updates-testing.repo` & `fedrq-0.7.0/src/fedrq/data/repos/fedora-updates-testing.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/data/repos/fedora-updates.repo` & `fedrq-0.7.0/src/fedrq/data/repos/fedora-updates.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/data/repos/fedora.repo` & `fedrq-0.7.0/src/fedrq/data/repos/fedora.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/release_repo.py` & `fedrq-0.7.0/src/fedrq/release_repo.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/src/fedrq/repoquery.py` & `fedrq-0.7.0/src/fedrq/repoquery.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/conftest.py` & `fedrq-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/integration/test_backends.py` & `fedrq-0.7.0/tests/integration/test_backends.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/integration/test_pkgs.py` & `fedrq-0.7.0/tests/integration/test_pkgs.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import pytest
 
 import fedrq.cli
 
 
+@pytest.mark.skip(
+    "This test loads rawhide metadata and is expensive. We already load f37."
+)
 @pytest.mark.no_rpm_mock
 def test_pkgs_basic_rawhide(capsys, target_cpu):
     fedrq.cli.main(["pkgs", "bash", "-Fna", "--sc"])
     stdout, stderr = capsys.readouterr()
     assert sorted(stdout.splitlines()) == sorted(["bash.src", f"bash.{target_cpu}"])
```

### Comparing `fedrq-0.6.0/tests/integration/test_subpkgs.py` & `fedrq-0.7.0/tests/integration/test_subpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/integration/test_whatrequires.py` & `fedrq-0.7.0/tests/integration/test_whatrequires.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/integration/test_whatrequires_src.py` & `fedrq-0.7.0/tests/integration/test_whatrequires_src.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/test_data/build.sh` & `fedrq-0.7.0/tests/test_data/build.sh`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/test_data/repos/repo1/specs/e1/packageb.spec` & `fedrq-0.7.0/tests/test_data/repos/repo1/specs/e1/packageb.spec`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/test_data/repos/repo1/specs/packagea.spec` & `fedrq-0.7.0/tests/test_data/repos/repo1/specs/packagea.spec`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/test_data/repos/repo1/specs/packageb.spec` & `fedrq-0.7.0/tests/test_data/repos/repo1/specs/packageb.spec`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/unit/test_checkconfig.py` & `fedrq-0.7.0/tests/unit/test_checkconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     assert "No validation errors found!" in out[0]
     assert not out[1]
 
 
 def test_checkconfig_dump(run_command2, patch_config_dirs):
     defs = {"base": ["testrepo1"]}
     expected = {
+        "append_system_repos": False,
         "matcher": "^(tester)$",
         "repo_aliases": {},
         "defpaths": ["testrepo1.repo"],
         "system_repos": False,
         "defs": defs,
         "repo_dirs": list(
             map(
```

### Comparing `fedrq-0.6.0/tests/unit/test_command.py` & `fedrq-0.7.0/tests/unit/test_command.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/unit/test_formatters.py` & `fedrq-0.7.0/tests/unit/test_formatters.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/unit/test_release.py` & `fedrq-0.7.0/tests/unit/test_release.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/unit/test_repoquery.py` & `fedrq-0.7.0/tests/unit/test_repoquery.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/unit/test_subbpkgs.py` & `fedrq-0.7.0/tests/unit/test_subbpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/unit/test_whatrequires.py` & `fedrq-0.7.0/tests/unit/test_whatrequires.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/tests/unit/test_whatrequires_src.py` & `fedrq-0.7.0/tests/unit/test_whatrequires_src.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.6.0/PKG-INFO` & `fedrq-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedrq
-Version: 0.6.0
+Version: 0.7.0
 Summary: fedrq is a tool to query the Fedora and EPEL repositories
 Author-email: Maxwell G <gotmax@e.email>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -16,14 +16,15 @@
 Classifier: Typing :: Typed
 Classifier: Environment :: Console
 Requires-Dist: pydantic ~= 1.0
 Requires-Dist: tomli; python_version<'3.11'
 Requires-Dist: requests
 Requires-Dist: fedrq[test] ; extra == "dev"
 Requires-Dist: fedrq[lint] ; extra == "dev"
+Requires-Dist: black ; extra == "doc"
 Requires-Dist: mkdocs ; extra == "doc"
 Requires-Dist: mkdocs-material ; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.18 ; extra == "doc"
 Requires-Dist: mkdocs-exclude ; extra == "doc"
 Requires-Dist: black ; extra == "lint"
 Requires-Dist: isort ; extra == "lint"
 Requires-Dist: mypy ; extra == "lint"
@@ -32,15 +33,16 @@
 Requires-Dist: tomli-w ; extra == "lint"
 Requires-Dist: types-requests ; extra == "lint"
 Requires-Dist: argcomplete ; extra == "lint"
 Requires-Dist: typing_extensions ; extra == "lint"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
 Requires-Dist: tomli-w ; extra == "test"
-Project-URL: Homepage, https://sr.ht/~gotmax23/fedrq
+Project-URL: Changelog, https://fedrq.gtmx.me/Changelog
+Project-URL: Homepage, https://fedrq.gtmx.me
 Project-URL: Mailing List, https://lists.sr.ht/~gotmax23/fedrq
 Project-URL: Source, https://git.sr.ht/~gotmax23/fedrq
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: lint
 Provides-Extra: test
```

