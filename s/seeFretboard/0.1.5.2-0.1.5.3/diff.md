# Comparing `tmp/seeFretboard-0.1.5.2.tar.gz` & `tmp/seeFretboard-0.1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeFretboard-0.1.5.2.tar", last modified: Tue May 30 09:38:08 2023, max compression
+gzip compressed data, was "seeFretboard-0.1.5.3.tar", last modified: Tue May 30 16:01:04 2023, max compression
```

## Comparing `seeFretboard-0.1.5.2.tar` & `seeFretboard-0.1.5.3.tar`

### file list

```diff
@@ -1,880 +1,880 @@
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.194434 seeFretboard-0.1.5.2/
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.967843 seeFretboard-0.1.5.2/.venv/
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.967907 seeFretboard-0.1.5.2/.venv/lib/
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.967969 seeFretboard-0.1.5.2/.venv/lib/python3.11/
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.974670 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.979052 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/_distutils_hack/
--rw-r--r--   0 lindazhang   (501) staff       (20)     6128 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)       44 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/_distutils_hack/override.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.979968 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/
--rw-r--r--   0 lindazhang   (501) staff       (20)      355 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1198 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/__main__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1444 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.982010 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/
--rw-r--r--   0 lindazhang   (501) staff       (20)      573 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10192 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10734 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cache.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.984614 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/
--rw-r--r--   0 lindazhang   (501) staff       (20)      132 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6676 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7842 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    29250 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      774 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2472 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4338 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10817 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1968 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18172 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5118 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      116 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.988070 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/
--rw-r--r--   0 lindazhang   (501) staff       (20)     3882 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7582 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1685 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4129 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9815 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6591 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5289 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2951 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1703 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1132 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4762 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3188 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    32234 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12343 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5697 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6419 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3755 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7396 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13529 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.989060 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/distributions/
--rw-r--r--   0 lindazhang   (501) staff       (20)      858 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1221 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      729 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6494 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1164 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    24091 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.990282 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/index/
--rw-r--r--   0 lindazhang   (501) staff       (20)       30 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16504 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    37873 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6557 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.991336 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/locations/
--rw-r--r--   0 lindazhang   (501) staff       (20)    17794 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6319 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8149 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2556 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      340 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/main.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.992200 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/
--rw-r--r--   0 lindazhang   (501) staff       (20)     4280 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2595 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25277 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.993073 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/
--rw-r--r--   0 lindazhang   (501) staff       (20)      107 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1882 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8181 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7457 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9773 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.995283 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/
--rw-r--r--   0 lindazhang   (501) staff       (20)       63 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      990 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6442 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2520 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1030 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2617 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18602 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      738 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4644 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1907 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3858 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3600 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.996973 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/
--rw-r--r--   0 lindazhang   (501) staff       (20)       50 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16507 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2145 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6096 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7638 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18443 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4073 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1791 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.997813 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.999545 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4133 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1422 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1474 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2198 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1075 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1417 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3064 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5122 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9784 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.000504 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/
--rw-r--r--   0 lindazhang   (501) staff       (20)       51 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1354 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4105 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    27407 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25091 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6987 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.002202 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/req/
--rw-r--r--   0 lindazhang   (501) staff       (20)     2807 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16611 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17646 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    35763 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2858 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    24045 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.002663 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      583 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.003014 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    24129 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.004811 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5220 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18963 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    27878 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5705 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9914 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2526 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5455 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11533 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8167 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.011429 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1015 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1665 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1884 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5377 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      242 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5764 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3206 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1115 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2118 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1169 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3064 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5122 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      716 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3110 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4831 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      795 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11632 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22253 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1193 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2108 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5662 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9200 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7702 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8821 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1759 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3456 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4549 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.012800 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/vcs/
--rw-r--r--   0 lindazhang   (501) staff       (20)      596 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3519 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18116 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5238 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11729 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22811 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13079 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.013680 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/
--rw-r--r--   0 lindazhang   (501) staff       (20)     4966 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.015989 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
--rw-r--r--   0 lindazhang   (501) staff       (20)      465 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1379 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5033 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1535 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.016667 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/
--rw-r--r--   0 lindazhang   (501) staff       (20)      242 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5271 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1033 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      778 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16416 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3946 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4154 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7105 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      774 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.017246 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/
--rw-r--r--   0 lindazhang   (501) staff       (20)       94 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      255 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4279 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.030099 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/
--rw-r--r--   0 lindazhang   (501) staff       (20)     4797 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    31274 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1763 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10032 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3915 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5420 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.030557 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3242 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3732 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      542 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1860 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1683 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4006 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12176 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3934 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13566 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1753 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    36913 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1753 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    20735 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1759 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14537 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25796 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    42498 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1752 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    27055 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   104562 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    98484 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    98196 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   101363 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   128035 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   102774 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    95372 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5380 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6077 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3715 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2131 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30391 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.030992 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13560 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      402 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6400 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4137 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4007 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14848 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8505 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2812 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      244 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.032318 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/
--rw-r--r--   0 lindazhang   (501) staff       (20)      266 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2522 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11128 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3325 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.034089 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/
--rw-r--r--   0 lindazhang   (501) staff       (20)       75 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2839 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10678 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6741 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1866 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1079 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3709 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6181 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7134 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.037725 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/
--rw-r--r--   0 lindazhang   (501) staff       (20)      581 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    41259 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    51697 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    20834 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    51991 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14811 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5058 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    39801 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10820 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18102 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    66262 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    23513 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    43898 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.039178 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distro/
--rw-r--r--   0 lindazhang   (501) staff       (20)      981 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)       64 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    49330 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.043074 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/
--rw-r--r--   0 lindazhang   (501) staff       (20)      849 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3374 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      321 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12950 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    44375 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1881 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0 lindazhang   (501) staff       (20)       21 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   206539 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.044446 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/
--rw-r--r--   0 lindazhang   (501) staff       (20)     1132 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1081 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6080 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    34557 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.047310 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/
--rw-r--r--   0 lindazhang   (501) staff       (20)      661 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      497 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11488 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4378 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1431 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8487 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4676 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30110 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    15699 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4200 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14665 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.048468 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/
--rw-r--r--   0 lindazhang   (501) staff       (20)   108287 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      562 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.051809 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/
--rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1176 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4068 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4910 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2655 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6911 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      160 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6596 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.059198 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/
--rw-r--r--   0 lindazhang   (501) staff       (20)     2999 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      353 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    23685 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1697 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1938 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.059500 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/
--rw-r--r--   0 lindazhang   (501) staff       (20)    40386 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2917 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.064604 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/
--rw-r--r--   0 lindazhang   (501) staff       (20)     4810 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4104 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3314 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5086 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    35441 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    21938 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5871 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19351 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5073 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2212 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5014 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7335 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4674 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11753 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    32005 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.065538 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/
--rw-r--r--   0 lindazhang   (501) staff       (20)    11174 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    70232 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    53376 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      986 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2591 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3072 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3092 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4630 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6257 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.065912 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/
--rw-r--r--   0 lindazhang   (501) staff       (20)     3419 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6184 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    63187 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9110 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.069764 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/
--rw-r--r--   0 lindazhang   (501) staff       (20)     9171 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6426 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   213344 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.069939 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/
--rw-r--r--   0 lindazhang   (501) staff       (20)    23685 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9023 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    39129 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25341 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13402 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10787 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6805 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.070961 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/
--rw-r--r--   0 lindazhang   (501) staff       (20)      491 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      138 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11920 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.071733 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/
--rw-r--r--   0 lindazhang   (501) staff       (20)      546 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10927 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.077509 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/
--rw-r--r--   0 lindazhang   (501) staff       (20)     5178 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      435 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1397 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    21443 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6377 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10187 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      575 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1286 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18560 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3823 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3879 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      733 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    35288 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      695 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30180 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4235 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2912 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    33240 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.079176 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/
--rw-r--r--   0 lindazhang   (501) staff       (20)      537 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.079639 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      156 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5872 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1583 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17592 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4794 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.107970 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/
--rw-r--r--   0 lindazhang   (501) staff       (20)     6090 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8478 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10096 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   140235 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1064 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2114 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      265 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9695 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3225 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1236 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1643 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7063 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      423 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5472 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19919 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      351 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      417 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22820 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1926 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2783 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1840 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      890 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10368 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6819 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3264 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9842 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4503 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18015 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1054 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7131 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    97992 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1288 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5497 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6630 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7954 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      972 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2501 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      642 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1616 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2508 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9585 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5053 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3252 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14007 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14172 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3667 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11903 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8198 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5305 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4970 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      828 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3396 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10574 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    37414 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    59836 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8165 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11303 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1391 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      166 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4436 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4773 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2843 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1591 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    24224 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4374 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4425 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    26332 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1258 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    34995 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    39684 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3370 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    45686 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3627 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      102 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    26070 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9169 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    34549 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/six.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.110408 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/
--rw-r--r--   0 lindazhang   (501) staff       (20)    18364 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3314 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1944 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1496 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1376 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1908 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1383 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7550 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2790 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2145 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8011 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.111201 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/
--rw-r--r--   0 lindazhang   (501) staff       (20)      396 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22633 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2943 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      254 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    80114 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.113684 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/
--rw-r--r--   0 lindazhang   (501) staff       (20)     3333 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10811 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0 lindazhang   (501) staff       (20)       64 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    20070 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    39095 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.116042 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      957 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.116936 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17632 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13922 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11036 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4528 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17081 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    34448 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7097 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8217 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8579 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2440 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.117233 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.117612 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1417 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    34665 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19786 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5985 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30641 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.120009 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/
--rw-r--r--   0 lindazhang   (501) staff       (20)     1155 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4901 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1605 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      498 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3997 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3510 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22003 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17177 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5758 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6895 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10003 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14298 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5403 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.121272 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/
--rw-r--r--   0 lindazhang   (501) staff       (20)    10579 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8979 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1305 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6563 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4307 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.121470 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/
--rw-r--r--   0 lindazhang   (501) staff       (20)   108568 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.122497 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    24701 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.124491 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
--rw-r--r--   0 lindazhang   (501) staff       (20)      506 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4504 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2741 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2706 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      884 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3494 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3886 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3566 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2836 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.125034 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5420 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13515 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.125201 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/
--rw-r--r--   0 lindazhang   (501) staff       (20)    15526 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.126139 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
--rw-r--r--   0 lindazhang   (501) staff       (20)       83 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   132569 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18410 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.128474 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
--rw-r--r--   0 lindazhang   (501) staff       (20)      661 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      497 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11488 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4378 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1431 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8496 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4706 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30110 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    15699 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4200 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14665 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.131152 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/
--rw-r--r--   0 lindazhang   (501) staff       (20)     9159 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6426 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   213310 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.131359 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/
--rw-r--r--   0 lindazhang   (501) staff       (20)    23668 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9023 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    39129 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25341 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13402 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10787 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6805 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8425 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.131600 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/extern/
--rw-r--r--   0 lindazhang   (501) staff       (20)     2426 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.140102 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/
--rw-r--r--   0 lindazhang   (501) staff       (20)     8429 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      218 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_deprecation_warning.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.149736 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/
--rw-r--r--   0 lindazhang   (501) staff       (20)      537 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1330 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      411 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      239 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19672 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8603 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14789 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    47369 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17973 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.156631 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/
--rw-r--r--   0 lindazhang   (501) staff       (20)      430 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1614 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5441 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4701 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22051 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5617 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7728 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    31558 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16568 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5624 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4888 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2603 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13137 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30221 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2779 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2785 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1189 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8434 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1936 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      672 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11765 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19241 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7477 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4920 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9451 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12537 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      139 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3423 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8082 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    50186 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3589 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10270 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17910 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8226 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13713 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1972 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30235 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    23602 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      217 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      639 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3517 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18858 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12096 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    15641 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18128 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12952 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5248 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1972 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2392 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_imp.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1311 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_importlib.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      675 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_itertools.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      749 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_path.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      501 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_reqs.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.157859 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.160078 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
--rw-r--r--   0 lindazhang   (501) staff       (20)    30130 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1862 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      743 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1828 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2895 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2068 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1154 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2166 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.161768 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
--rw-r--r--   0 lindazhang   (501) staff       (20)      506 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4504 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2741 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2706 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      884 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3494 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3886 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3566 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2836 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.162246 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5420 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13512 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.162443 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/
--rw-r--r--   0 lindazhang   (501) staff       (20)    15517 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.163724 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
--rw-r--r--   0 lindazhang   (501) staff       (20)       82 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   117959 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16256 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    15130 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.166331 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/
--rw-r--r--   0 lindazhang   (501) staff       (20)      661 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      497 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11488 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4378 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1431 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8493 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4700 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30110 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    15699 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4200 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14665 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.168984 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/
--rw-r--r--   0 lindazhang   (501) staff       (20)     9159 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6426 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   213310 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.169155 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/
--rw-r--r--   0 lindazhang   (501) staff       (20)    23668 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9023 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    39129 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25341 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13402 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10787 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6805 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.169950 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/
--rw-r--r--   0 lindazhang   (501) staff       (20)      396 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22633 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2943 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      254 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    87149 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8425 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7346 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/archive_util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19539 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/build_meta.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.175943 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/
--rw-r--r--   0 lindazhang   (501) staff       (20)      396 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2381 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/alias.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16623 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1182 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6595 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/build.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4415 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    15821 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14115 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7012 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/develop.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4800 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    85662 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    31188 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    26795 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5163 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/install.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2226 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3875 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2612 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4946 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      468 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/register.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2128 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      658 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7071 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5086 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8102 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/test.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      462 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/upload.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7494 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.177582 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/
--rw-r--r--   0 lindazhang   (501) staff       (20)     1121 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13398 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.178953 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/
--rw-r--r--   0 lindazhang   (501) staff       (20)     1038 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11266 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1153 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1612 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   269900 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8736 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16319 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/expand.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19304 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25198 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      949 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/dep_util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5499 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/depends.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    20799 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/discovery.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    45578 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/dist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2464 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/errors.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5591 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/extension.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.179134 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/extern/
--rw-r--r--   0 lindazhang   (501) staff       (20)     2512 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4873 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/glob.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3824 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/installer.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      812 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/launch.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1210 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/logging.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4857 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/monkey.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    47724 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/msvc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3093 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/namespaces.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    40020 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/package_index.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      245 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/py34compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14348 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/sandbox.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      941 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      144 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/version.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8376 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      718 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/windows_support.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.184556 seeFretboard-0.1.5.2/Examples/
--rw-r--r--   0 lindazhang   (501) staff       (20)      939 2023-05-25 18:25:21.000000 seeFretboard-0.1.5.2/Examples/RunAllExamples.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      583 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/Examples/arpeggio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6161 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/Examples/cagedChord.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      581 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/Examples/createMidiAudio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      806 2023-05-25 18:29:01.000000 seeFretboard-0.1.5.2/Examples/createVideo.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      881 2023-05-25 18:29:06.000000 seeFretboard-0.1.5.2/Examples/createVideoWithAudio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1026 2023-05-25 18:29:10.000000 seeFretboard-0.1.5.2/Examples/createVideoWithMidiAudio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8789 2023-05-30 06:22:19.000000 seeFretboard-0.1.5.2/Examples/dropChord.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      416 2023-05-25 18:29:14.000000 seeFretboard-0.1.5.2/Examples/figureNextToEachOther.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      438 2023-05-25 18:29:21.000000 seeFretboard-0.1.5.2/Examples/generateScriptAndDiv.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      278 2023-05-25 18:29:25.000000 seeFretboard-0.1.5.2/Examples/generateStandalone.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      424 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/Examples/groundtruthVPredictionTest.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      240 2023-05-25 18:28:50.000000 seeFretboard-0.1.5.2/Examples/horizontalFretboard.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      281 2023-05-26 06:19:42.000000 seeFretboard-0.1.5.2/Examples/horizontalFretboardAddNotes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      492 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/Examples/interval.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      403 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/Examples/octave.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      687 2023-05-25 18:29:49.000000 seeFretboard-0.1.5.2/Examples/saveVideoWithAudio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      825 2023-05-26 06:19:42.000000 seeFretboard-0.1.5.2/Examples/scale.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      980 2023-05-25 18:30:02.000000 seeFretboard-0.1.5.2/Examples/testText.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      238 2023-05-25 18:30:06.000000 seeFretboard-0.1.5.2/Examples/verticalFretboard.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      282 2023-05-25 18:30:11.000000 seeFretboard-0.1.5.2/Examples/verticalFretboardAddNotes.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.184930 seeFretboard-0.1.5.2/Images/
--rw-r--r--   0 lindazhang   (501) staff       (20)   160597 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/Images/logo.png
--rw-r--r--   0 lindazhang   (501) staff       (20)     2408 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/LICENSE
--rw-r--r--   0 lindazhang   (501) staff       (20)       80 2023-05-30 08:16:27.000000 seeFretboard-0.1.5.2/MANIFEST.in
--rw-r--r--   0 lindazhang   (501) staff       (20)     2706 2023-05-30 09:38:08.194257 seeFretboard-0.1.5.2/PKG-INFO
--rw-r--r--   0 lindazhang   (501) staff       (20)     2359 2023-05-30 07:56:26.000000 seeFretboard-0.1.5.2/README.md
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.186305 seeFretboard-0.1.5.2/Tests/
--rw-r--r--   0 lindazhang   (501) staff       (20)     7138 2023-05-25 06:24:06.000000 seeFretboard-0.1.5.2/Tests/StylesTest.py
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:56:48.000000 seeFretboard-0.1.5.2/Tests/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.186421 seeFretboard-0.1.5.2/docs/
--rw-r--r--   0 lindazhang   (501) staff       (20)     1108 2023-05-30 06:42:14.000000 seeFretboard-0.1.5.2/docs/conf.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      289 2023-05-25 04:52:16.000000 seeFretboard-0.1.5.2/pyproject.toml
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.187556 seeFretboard-0.1.5.2/seeFretboard/
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.189959 seeFretboard-0.1.5.2/seeFretboard/Designs/
--rw-r--r--   0 lindazhang   (501) staff       (20)     7102 2023-05-30 02:47:47.000000 seeFretboard-0.1.5.2/seeFretboard/Designs/CirlceNote.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7552 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/seeFretboard/Designs/FretboardFigure.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    21591 2023-05-30 06:51:00.000000 seeFretboard-0.1.5.2/seeFretboard/Designs/FretboardStyle.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      139 2023-05-25 06:01:38.000000 seeFretboard-0.1.5.2/seeFretboard/Designs/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1238 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/seeFretboard/NotePosition.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:07.977019 seeFretboard-0.1.5.2/seeFretboard/Outputs/
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.190389 seeFretboard-0.1.5.2/seeFretboard/Outputs/Audios/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-30 08:34:27.000000 seeFretboard-0.1.5.2/seeFretboard/Outputs/Audios/placeHolder.txt
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.190509 seeFretboard-0.1.5.2/seeFretboard/Outputs/Embeds/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-30 08:34:30.000000 seeFretboard-0.1.5.2/seeFretboard/Outputs/Embeds/placeHolder.txt
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.190624 seeFretboard-0.1.5.2/seeFretboard/Outputs/Images/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-30 08:34:34.000000 seeFretboard-0.1.5.2/seeFretboard/Outputs/Images/placeHolder.txt
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.190738 seeFretboard-0.1.5.2/seeFretboard/Outputs/Videos/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-30 08:34:37.000000 seeFretboard-0.1.5.2/seeFretboard/Outputs/Videos/placeHolder.txt
--rw-r--r--   0 lindazhang   (501) staff       (20)     7537 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/seeFretboard/PitchCollection.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    53017 2023-05-30 08:47:08.000000 seeFretboard-0.1.5.2/seeFretboard/SeeFretboard.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.191837 seeFretboard-0.1.5.2/seeFretboard/Utilities/
--rw-r--r--   0 lindazhang   (501) staff       (20)    27150 2023-05-30 07:35:02.000000 seeFretboard-0.1.5.2/seeFretboard/Utilities/Constants.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12538 2023-05-30 06:38:05.000000 seeFretboard-0.1.5.2/seeFretboard/Utilities/Functions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2153 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/seeFretboard/Utilities/PathInfo.py
--rw-r--r--   0 lindazhang   (501) staff       (20)       73 2023-05-30 06:46:25.000000 seeFretboard-0.1.5.2/seeFretboard/Utilities/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.193903 seeFretboard-0.1.5.2/seeFretboard/Videos/
--rw-r--r--   0 lindazhang   (501) staff       (20)     2731 2023-05-24 04:39:52.000000 seeFretboard-0.1.5.2/seeFretboard/Videos/Audio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1767 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/seeFretboard/Videos/Frame.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2912 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/seeFretboard/Videos/Images.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12653 2023-05-30 07:16:36.000000 seeFretboard-0.1.5.2/seeFretboard/Videos/TabSequence.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11256 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/seeFretboard/Videos/Video.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7358 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/seeFretboard/Videos/VideoManager.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1885 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/seeFretboard/Videos/VideoNote.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      262 2023-05-25 06:14:15.000000 seeFretboard-0.1.5.2/seeFretboard/Videos/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      252 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.2/seeFretboard/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 09:38:08.188750 seeFretboard-0.1.5.2/seeFretboard.egg-info/
--rw-r--r--   0 lindazhang   (501) staff       (20)     2706 2023-05-30 09:38:07.000000 seeFretboard-0.1.5.2/seeFretboard.egg-info/PKG-INFO
--rw-r--r--   0 lindazhang   (501) staff       (20)    52116 2023-05-30 09:38:07.000000 seeFretboard-0.1.5.2/seeFretboard.egg-info/SOURCES.txt
--rw-r--r--   0 lindazhang   (501) staff       (20)        1 2023-05-30 09:38:07.000000 seeFretboard-0.1.5.2/seeFretboard.egg-info/dependency_links.txt
--rw-r--r--   0 lindazhang   (501) staff       (20)        9 2023-05-30 09:38:07.000000 seeFretboard-0.1.5.2/seeFretboard.egg-info/requires.txt
--rw-r--r--   0 lindazhang   (501) staff       (20)       13 2023-05-30 09:38:07.000000 seeFretboard-0.1.5.2/seeFretboard.egg-info/top_level.txt
--rw-r--r--   0 lindazhang   (501) staff       (20)       38 2023-05-30 09:38:08.194489 seeFretboard-0.1.5.2/setup.cfg
--rw-r--r--   0 lindazhang   (501) staff       (20)      971 2023-05-30 08:47:47.000000 seeFretboard-0.1.5.2/setup.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.994096 seeFretboard-0.1.5.3/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.763617 seeFretboard-0.1.5.3/.venv/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.763709 seeFretboard-0.1.5.3/.venv/lib/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.763801 seeFretboard-0.1.5.3/.venv/lib/python3.11/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.770348 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.774304 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/_distutils_hack/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6128 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)       44 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/_distutils_hack/override.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.775237 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      355 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1198 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/__main__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1444 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.777438 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      573 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10192 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10734 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cache.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.780020 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      132 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6676 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7842 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    29250 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      774 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2472 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4338 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10817 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1968 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18172 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5118 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      116 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.783429 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3882 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7582 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1685 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4129 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9815 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6591 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5289 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2951 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1703 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1132 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4762 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3188 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    32234 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12343 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5697 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6419 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3755 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7396 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13529 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.784437 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/distributions/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      858 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1221 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      729 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6494 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1164 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    24091 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.785294 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/index/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       30 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16504 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    37873 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6557 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.786486 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/locations/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17794 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6319 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8149 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2556 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      340 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/main.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.787432 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4280 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2595 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25277 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.788498 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      107 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1882 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8181 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7457 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9773 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.791169 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       63 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      990 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6442 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2520 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1030 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2617 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18602 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      738 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4644 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1907 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3858 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3600 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.793234 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       50 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16507 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2145 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6096 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7638 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18443 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4073 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1791 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.794066 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.795635 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4133 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1422 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1474 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2198 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1075 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1417 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3064 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5122 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9784 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.796652 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       51 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1354 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4105 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    27407 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25091 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6987 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.798418 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/req/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2807 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16611 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17646 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    35763 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2858 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    24045 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.798978 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      583 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.799345 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    24129 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.801912 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5220 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18963 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    27878 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5705 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9914 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2526 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5455 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11533 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8167 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.808048 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1015 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1665 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1884 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5377 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      242 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5764 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3206 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1115 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2118 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1169 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3064 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5122 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      716 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3110 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4831 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      795 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11632 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22253 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1193 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2108 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5662 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9200 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7702 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8821 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1759 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3456 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4549 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.809202 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/vcs/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      596 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3519 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18116 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5238 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11729 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22811 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13079 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.809960 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4966 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.812081 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      465 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1379 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5033 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1535 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.812635 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      242 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5271 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1033 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      778 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16416 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3946 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4154 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7105 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      774 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.813280 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       94 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      255 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4279 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.826893 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4797 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    31274 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1763 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10032 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3915 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5420 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.827327 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3242 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3732 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      542 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1860 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1683 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4006 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12176 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3934 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13566 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1753 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    36913 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1753 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    20735 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1759 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14537 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25796 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    42498 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1752 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    27055 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   104562 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    98484 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    98196 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   101363 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   128035 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   102774 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    95372 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5380 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6077 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3715 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2131 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30391 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.827822 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13560 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      402 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6400 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4137 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4007 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14848 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8505 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2812 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      244 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.829538 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      266 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2522 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11128 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3325 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.831091 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       75 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2839 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10678 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6741 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1866 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1079 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3709 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6181 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7134 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.834649 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      581 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    41259 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    51697 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    20834 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    51991 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14811 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5058 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    39801 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10820 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18102 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    66262 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    23513 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    43898 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.835973 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      981 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)       64 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    49330 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.838504 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      849 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3374 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      321 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12950 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    44375 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1881 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)       21 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   206539 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.839508 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1132 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1081 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6080 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    34557 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.842651 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      661 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      497 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11488 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4378 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1431 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8487 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4676 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30110 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15699 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4200 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14665 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.843520 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/
+-rw-r--r--   0 lindazhang   (501) staff       (20)   108287 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      562 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.845236 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1176 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4068 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4910 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2655 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6911 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      160 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6596 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.848672 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2999 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      353 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    23685 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1697 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1938 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.848885 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    40386 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2917 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.852277 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4810 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4104 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3314 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5086 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    35441 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    21938 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5871 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19351 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5073 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2212 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5014 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7335 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4674 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11753 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    32005 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.853301 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11174 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    70232 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    53376 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      986 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2591 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3072 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3092 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4630 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6257 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.853576 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3419 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6184 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    63187 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9110 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.856208 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9171 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6426 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   213344 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.856407 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    23685 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9023 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    39129 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25341 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13402 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10787 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6805 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.856969 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      491 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      138 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11920 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.857358 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      546 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10927 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.862005 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5178 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      435 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1397 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    21443 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6377 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10187 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      575 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1286 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18560 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3823 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3879 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      733 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    35288 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      695 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30180 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4235 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2912 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    33240 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.863454 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      537 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.863880 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      156 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5872 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1583 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17592 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4794 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.884954 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6090 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8478 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10096 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   140235 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1064 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2114 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      265 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9695 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3225 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1236 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1643 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7063 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      423 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5472 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19919 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      351 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      417 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22820 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1926 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2783 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1840 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      890 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10368 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6819 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3264 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9842 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4503 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18015 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1054 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7131 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    97992 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1288 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5497 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6630 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7954 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      972 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2501 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      642 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1616 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2508 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9585 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5053 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3252 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14007 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14172 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3667 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11903 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8198 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5305 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4970 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      828 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3396 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10574 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    37414 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    59836 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8165 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11303 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1391 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      166 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4436 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4773 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2843 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1591 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    24224 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4374 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4425 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    26332 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1258 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    34995 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    39684 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3370 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    45686 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3627 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      102 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    26070 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9169 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    34549 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/six.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.887012 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18364 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3314 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1944 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1496 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1376 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1908 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1383 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7550 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2790 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2145 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8011 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.887865 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      396 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22633 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2943 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      254 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    80114 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.890338 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3333 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10811 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)       64 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    20070 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    39095 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.892482 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      957 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.893530 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17632 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13922 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11036 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4528 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17081 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    34448 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7097 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8217 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8579 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2440 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.893850 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.894236 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1417 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    34665 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19786 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5985 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30641 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.898157 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1155 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4901 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1605 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      498 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3997 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3510 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22003 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17177 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5758 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6895 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10003 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14298 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5403 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.899798 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10579 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8979 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1305 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6563 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4307 2023-02-02 16:11:15.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.899989 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/
+-rw-r--r--   0 lindazhang   (501) staff       (20)   108568 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.901117 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    24701 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.904261 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      506 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4504 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2741 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2706 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      884 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3494 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3886 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3566 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2836 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.905063 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5420 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13515 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.905279 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15526 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.906688 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       83 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   132569 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18410 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.909656 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      661 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      497 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11488 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4378 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1431 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8496 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4706 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30110 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15699 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4200 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14665 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.912481 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9159 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6426 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   213310 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.912676 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    23668 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9023 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    39129 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25341 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13402 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10787 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6805 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8425 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.912926 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/extern/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2426 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.921363 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8429 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      218 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_deprecation_warning.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.933158 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      537 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1330 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      411 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      239 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19672 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8603 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14789 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    47369 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17973 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.947124 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      430 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1614 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5441 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4701 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22051 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5617 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7728 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    31558 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16568 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5624 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4888 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2603 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13137 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30221 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2779 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2785 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1189 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8434 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1936 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      672 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11765 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19241 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7477 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4920 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9451 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12537 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      139 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3423 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8082 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    50186 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3589 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10270 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17910 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8226 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13713 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1972 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30235 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    23602 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      217 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      639 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3517 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18858 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12096 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15641 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18128 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12952 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5248 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1972 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2392 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_imp.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1311 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_importlib.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      675 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_itertools.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      749 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_path.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      501 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_reqs.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.948254 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.951816 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30130 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1862 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      743 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1828 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2895 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2068 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1154 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2166 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.956322 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      506 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4504 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2741 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2706 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      884 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3494 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3886 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3566 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2836 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.957095 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5420 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13512 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.957343 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15517 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.959560 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       82 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   117959 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16256 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15130 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.962268 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      661 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      497 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11488 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4378 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1431 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8493 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4700 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30110 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15699 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4200 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14665 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.965428 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9159 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6426 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   213310 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.965624 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    23668 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9023 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    39129 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25341 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13402 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10787 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6805 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.966661 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      396 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22633 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2943 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      254 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    87149 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8425 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7346 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/archive_util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19539 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/build_meta.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.973552 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      396 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2381 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/alias.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16623 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1182 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6595 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/build.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4415 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15821 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14115 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7012 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/develop.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4800 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    85662 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    31188 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    26795 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5163 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/install.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2226 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3875 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2612 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4946 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      468 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/register.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2128 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      658 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7071 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5086 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8102 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/test.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      462 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/upload.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7494 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.975437 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1121 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13398 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.977409 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1038 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11266 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1153 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1612 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   269900 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8736 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16319 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/expand.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19304 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25198 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      949 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/dep_util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5499 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/depends.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    20799 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/discovery.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    45578 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/dist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2464 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/errors.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5591 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/extension.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.977638 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/extern/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2512 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4873 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/glob.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3824 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/installer.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      812 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/launch.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1210 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/logging.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4857 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/monkey.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    47724 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/msvc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3093 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/namespaces.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    40020 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/package_index.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      245 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/py34compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14348 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/sandbox.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      941 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      144 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/version.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8376 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      718 2023-02-02 16:11:14.000000 seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/windows_support.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.983306 seeFretboard-0.1.5.3/Examples/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      939 2023-05-25 18:25:21.000000 seeFretboard-0.1.5.3/Examples/RunAllExamples.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      583 2023-05-30 15:39:55.000000 seeFretboard-0.1.5.3/Examples/arpeggio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6161 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.3/Examples/cagedChord.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      581 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.3/Examples/createMidiAudio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      806 2023-05-25 18:29:01.000000 seeFretboard-0.1.5.3/Examples/createVideo.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      881 2023-05-30 15:54:45.000000 seeFretboard-0.1.5.3/Examples/createVideoWithAudio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1026 2023-05-25 18:29:10.000000 seeFretboard-0.1.5.3/Examples/createVideoWithMidiAudio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8789 2023-05-30 15:54:45.000000 seeFretboard-0.1.5.3/Examples/dropChord.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      416 2023-05-25 18:29:14.000000 seeFretboard-0.1.5.3/Examples/figureNextToEachOther.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      438 2023-05-25 18:29:21.000000 seeFretboard-0.1.5.3/Examples/generateScriptAndDiv.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      278 2023-05-25 18:29:25.000000 seeFretboard-0.1.5.3/Examples/generateStandalone.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      424 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.3/Examples/groundtruthVPredictionTest.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      255 2023-05-30 10:44:18.000000 seeFretboard-0.1.5.3/Examples/horizontalFretboard.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      297 2023-05-30 13:00:31.000000 seeFretboard-0.1.5.3/Examples/horizontalFretboardAddNotes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      492 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.3/Examples/interval.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      403 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.3/Examples/octave.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      687 2023-05-25 18:29:49.000000 seeFretboard-0.1.5.3/Examples/saveVideoWithAudio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      825 2023-05-26 06:19:42.000000 seeFretboard-0.1.5.3/Examples/scale.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      980 2023-05-25 18:30:02.000000 seeFretboard-0.1.5.3/Examples/testText.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      238 2023-05-25 18:30:06.000000 seeFretboard-0.1.5.3/Examples/verticalFretboard.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      282 2023-05-25 18:30:11.000000 seeFretboard-0.1.5.3/Examples/verticalFretboardAddNotes.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.983661 seeFretboard-0.1.5.3/Images/
+-rw-r--r--   0 lindazhang   (501) staff       (20)   160597 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.3/Images/logo.png
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2408 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.3/LICENSE
+-rw-r--r--   0 lindazhang   (501) staff       (20)       80 2023-05-30 08:16:27.000000 seeFretboard-0.1.5.3/MANIFEST.in
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2706 2023-05-30 16:01:04.993922 seeFretboard-0.1.5.3/PKG-INFO
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2359 2023-05-30 07:56:26.000000 seeFretboard-0.1.5.3/README.md
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.984953 seeFretboard-0.1.5.3/Tests/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7138 2023-05-25 06:24:06.000000 seeFretboard-0.1.5.3/Tests/StylesTest.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:56:48.000000 seeFretboard-0.1.5.3/Tests/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.985100 seeFretboard-0.1.5.3/docs/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1108 2023-05-30 06:42:14.000000 seeFretboard-0.1.5.3/docs/conf.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      289 2023-05-25 04:52:16.000000 seeFretboard-0.1.5.3/pyproject.toml
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.986559 seeFretboard-0.1.5.3/seeFretboard/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.988636 seeFretboard-0.1.5.3/seeFretboard/Designs/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7158 2023-05-30 15:59:23.000000 seeFretboard-0.1.5.3/seeFretboard/Designs/CirlceNote.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7593 2023-05-30 15:59:26.000000 seeFretboard-0.1.5.3/seeFretboard/Designs/FretboardFigure.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    21562 2023-05-30 15:54:45.000000 seeFretboard-0.1.5.3/seeFretboard/Designs/FretboardStyle.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      139 2023-05-25 06:01:38.000000 seeFretboard-0.1.5.3/seeFretboard/Designs/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1238 2023-05-30 15:54:45.000000 seeFretboard-0.1.5.3/seeFretboard/NotePosition.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.772518 seeFretboard-0.1.5.3/seeFretboard/Outputs/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.989012 seeFretboard-0.1.5.3/seeFretboard/Outputs/Audios/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-30 08:34:27.000000 seeFretboard-0.1.5.3/seeFretboard/Outputs/Audios/placeHolder.txt
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.989125 seeFretboard-0.1.5.3/seeFretboard/Outputs/Embeds/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-30 08:34:30.000000 seeFretboard-0.1.5.3/seeFretboard/Outputs/Embeds/placeHolder.txt
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.989237 seeFretboard-0.1.5.3/seeFretboard/Outputs/Images/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-30 08:34:34.000000 seeFretboard-0.1.5.3/seeFretboard/Outputs/Images/placeHolder.txt
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.989350 seeFretboard-0.1.5.3/seeFretboard/Outputs/Videos/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-30 08:34:37.000000 seeFretboard-0.1.5.3/seeFretboard/Outputs/Videos/placeHolder.txt
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8517 2023-05-30 15:42:57.000000 seeFretboard-0.1.5.3/seeFretboard/PitchCollection.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    57311 2023-05-30 15:49:30.000000 seeFretboard-0.1.5.3/seeFretboard/SeeFretboard.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.990281 seeFretboard-0.1.5.3/seeFretboard/Utilities/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    27150 2023-05-30 07:35:02.000000 seeFretboard-0.1.5.3/seeFretboard/Utilities/Constants.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13328 2023-05-30 15:57:34.000000 seeFretboard-0.1.5.3/seeFretboard/Utilities/Functions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2153 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.3/seeFretboard/Utilities/PathInfo.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)       73 2023-05-30 06:46:25.000000 seeFretboard-0.1.5.3/seeFretboard/Utilities/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.993521 seeFretboard-0.1.5.3/seeFretboard/Videos/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2731 2023-05-24 04:39:52.000000 seeFretboard-0.1.5.3/seeFretboard/Videos/Audio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1767 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.3/seeFretboard/Videos/Frame.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2912 2023-05-30 15:56:27.000000 seeFretboard-0.1.5.3/seeFretboard/Videos/Images.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12653 2023-05-30 15:54:45.000000 seeFretboard-0.1.5.3/seeFretboard/Videos/TabSequence.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11256 2023-05-30 15:54:45.000000 seeFretboard-0.1.5.3/seeFretboard/Videos/Video.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7358 2023-05-30 15:59:34.000000 seeFretboard-0.1.5.3/seeFretboard/Videos/VideoManager.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1885 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.3/seeFretboard/Videos/VideoNote.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      262 2023-05-25 06:14:15.000000 seeFretboard-0.1.5.3/seeFretboard/Videos/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      252 2023-05-30 00:48:35.000000 seeFretboard-0.1.5.3/seeFretboard/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-30 16:01:04.987502 seeFretboard-0.1.5.3/seeFretboard.egg-info/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2706 2023-05-30 16:01:04.000000 seeFretboard-0.1.5.3/seeFretboard.egg-info/PKG-INFO
+-rw-r--r--   0 lindazhang   (501) staff       (20)    52116 2023-05-30 16:01:04.000000 seeFretboard-0.1.5.3/seeFretboard.egg-info/SOURCES.txt
+-rw-r--r--   0 lindazhang   (501) staff       (20)        1 2023-05-30 16:01:04.000000 seeFretboard-0.1.5.3/seeFretboard.egg-info/dependency_links.txt
+-rw-r--r--   0 lindazhang   (501) staff       (20)        9 2023-05-30 16:01:04.000000 seeFretboard-0.1.5.3/seeFretboard.egg-info/requires.txt
+-rw-r--r--   0 lindazhang   (501) staff       (20)       13 2023-05-30 16:01:04.000000 seeFretboard-0.1.5.3/seeFretboard.egg-info/top_level.txt
+-rw-r--r--   0 lindazhang   (501) staff       (20)       38 2023-05-30 16:01:04.994150 seeFretboard-0.1.5.3/setup.cfg
+-rw-r--r--   0 lindazhang   (501) staff       (20)      971 2023-05-30 16:00:55.000000 seeFretboard-0.1.5.3/setup.py
```

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/__main__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cache.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/six.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_imp.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_importlib.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_itertools.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_path.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/archive_util.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/build_meta.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/alias.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/build.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/develop.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/install.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/test.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/expand.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/dep_util.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/depends.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/discovery.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/dist.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/errors.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/extension.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/glob.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/installer.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/launch.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/logging.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/monkey.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/msvc.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/namespaces.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/package_index.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/sandbox.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/wheel.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/.venv/lib/python3.11/site-packages/setuptools/windows_support.py` & `seeFretboard-0.1.5.3/.venv/lib/python3.11/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/Examples/RunAllExamples.py` & `seeFretboard-0.1.5.3/Examples/RunAllExamples.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/Examples/arpeggio.py` & `seeFretboard-0.1.5.3/Examples/arpeggio.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 
 from seeFretboard import SeeFretboard
 
-fretboard = SeeFretboard("h", 3, 12)
+fretboard = SeeFretboard("h", 1, 12)
 fretboard.drawHorizontalFretboard()
 
 fretboard.getPitchCollection().setPitchesType("pitchesWithOctave")
 #fretboard.getPitchCollection().setPitchesType("pitchesScaleDegrees")
 
 #fretboard.addArpeggio("f","major-13th")
 fretboard.addArpeggio("f","major")
```

### Comparing `seeFretboard-0.1.5.2/Examples/cagedChord.py` & `seeFretboard-0.1.5.3/Examples/cagedChord.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/Examples/createMidiAudio.py` & `seeFretboard-0.1.5.3/Examples/createMidiAudio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/Examples/createVideo.py` & `seeFretboard-0.1.5.3/Examples/createVideo.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/Examples/createVideoWithAudio.py` & `seeFretboard-0.1.5.3/Examples/createVideoWithAudio.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 fretboard = SeeFretboard("v", 1, 12)
 tabSeq = TabSequence(8)
 video = Video(0, 0, 0, 0)
 fretboard.drawVerticalFretboard()
 video.setVideoName("OpenStringG")
 
-'''
+"""
 Use guitar set track 0 to make frames
 Then frames to images
 then images to video with audio
-'''
+"""
 tabSeq.makingFrames()
 video.setAudioName("00_BN3-119-G_comp_hex_cln.wav")
 
 videoManager = VideoManager(fretboard,video,Images())
 #videoManager.saveAsVideoImagesNoSeconds()#generate images for audio
 videoManager.createVideoWithAudio()#createVideoWithMidiAudio
```

### Comparing `seeFretboard-0.1.5.2/Examples/createVideoWithMidiAudio.py` & `seeFretboard-0.1.5.3/Examples/createVideoWithMidiAudio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/Examples/dropChord.py` & `seeFretboard-0.1.5.3/Examples/dropChord.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from seeFretboard import SeeFretboard
 
 fretboard = SeeFretboard("h", 1, 12)
 fretboard.drawFretboard("v")#this function can change from h to v
 
 #fretboard.getPitchCollection().setPitchesType("pitchesScaleDegrees")
 
-'''
+"""
 Drop2 String6
-'''
+"""
 fretboard.addDropChord("c","maj7")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "maj7","Drop2", "2")
 # fretboard.setNoteType("prediction")
 # fretboard.addDropChord("c", "maj7","Drop2", "3")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "maj7","Drop2", "4")
@@ -47,17 +47,17 @@
 # fretboard.addDropChord("c","dim7")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "dim7","Drop2", "2")
 # fretboard.setNoteType("prediction")
 # fretboard.addDropChord("c", "dim7","Drop2", "3")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "dim7","Drop2", "4")
-'''
+"""
 Drop2 String5
-'''
+"""
 # fretboard.addDropChord("c","maj7","Drop2","1","5")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "maj7","Drop2", "2","5")
 # fretboard.setNoteType("prediction")
 # fretboard.addDropChord("c", "maj7","Drop2", "3","5")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "maj7","Drop2", "4","5")
@@ -91,17 +91,17 @@
 # fretboard.addDropChord("c", "dim7","Drop2", "2","5")
 # fretboard.setNoteType("prediction")
 # fretboard.addDropChord("c", "dim7","Drop2", "3","5")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "dim7","Drop2", "4","5")
 
 
-'''
+"""
 Drop2 String4
-'''
+"""
 # fretboard.addDropChord("c","maj7","Drop2","1","4")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "maj7","Drop2", "2","4")
 # fretboard.setNoteType("prediction")
 # fretboard.addDropChord("c", "maj7","Drop2", "3","4")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "maj7","Drop2", "4","4")
@@ -134,17 +134,17 @@
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "dim7","Drop2", "2","4")
 # fretboard.setNoteType("prediction")
 # fretboard.addDropChord("c", "dim7","Drop2", "3","4")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "dim7","Drop2", "4","4")
 
-'''
+"""
 Drop3 String6
-'''
+"""
 # fretboard.addDropChord("c","maj7","Drop3","1","6")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "maj7","Drop3", "2","6")
 # fretboard.setNoteType("prediction")
 # fretboard.addDropChord("c", "maj7","Drop3", "3","6")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "maj7","Drop3", "4","6")
@@ -176,17 +176,17 @@
 # fretboard.addDropChord("c","dim7","Drop3","1","6")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "dim7","Drop3", "2","6")
 # fretboard.setNoteType("prediction")
 # fretboard.addDropChord("c", "dim7","Drop3", "3","6")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "dim7","Drop3", "4","6")
-'''
+"""
 Drop3 String5
-'''
+"""
 # fretboard.addDropChord("c","maj7","Drop3","1","5")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "maj7","Drop3", "2","5")
 # fretboard.setNoteType("prediction")
 # fretboard.addDropChord("c", "maj7","Drop3", "3","5")
 # fretboard.setNoteType("groundTruth")
 # fretboard.addDropChord("c", "maj7","Drop3", "4","5")
```

### Comparing `seeFretboard-0.1.5.2/Examples/saveVideoWithAudio.py` & `seeFretboard-0.1.5.3/Examples/saveVideoWithAudio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/Examples/scale.py` & `seeFretboard-0.1.5.3/Examples/scale.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/Examples/testText.py` & `seeFretboard-0.1.5.3/Examples/testText.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/Images/logo.png` & `seeFretboard-0.1.5.3/Images/logo.png`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/LICENSE` & `seeFretboard-0.1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/PKG-INFO` & `seeFretboard-0.1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeFretboard
-Version: 0.1.5.2
+Version: 0.1.5.3
 Summary: For Release
 Home-page: https://github.com/LindaRZhang/seeFretboard
 Author: Linda Rong Zhang
 Author-email: ronglindaz@gmail.com
 License: GNU
 Project-URL: Bug Tracker, https://github.com/LindaRZhang/seeFretboard/issues
 Description-Content-Type: text/markdown
```

### Comparing `seeFretboard-0.1.5.2/README.md` & `seeFretboard-0.1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/Tests/StylesTest.py` & `seeFretboard-0.1.5.3/Tests/StylesTest.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/docs/conf.py` & `seeFretboard-0.1.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/seeFretboard/Designs/CirlceNote.py` & `seeFretboard-0.1.5.3/seeFretboard/Designs/CirlceNote.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 class CircleNote():
-    '''
+    """
     CircleNote is a class for displaying notes with customizable properties.
 
     Attributes:
-    - noteFaceColor (str): The color of the note face. Default is 'blue'.
-    - noteFill (bool): Indicates whether the note should be filled. Default is True.
-    - noteEdgeColor (str): The color of the note edge. Default is 'black'.
-    - noteEdgeWidth (int): The width of the note edge. Default is 2.
-    - noteRadius (float): The radius of the note. Default is 0.4.
-    - noteOpacity (float): The opacity of the note. Default is 1.
-    - noteTextColor (str): The color of the text inside note.
-    - noteTextFont (str): The font of the text inside note.
-    - intervals (list): List of intervals associated with the note.
-    - scaleDegrees (list): List of scale degrees associated with the note.
-    - name (str): The name of the note.
-    - nameWithOctave (str): The name of the note with octave information.
-    - fret (int): The fret position of the note.
-    - string (int): The string position of the note.
-    '''
+        - noteFaceColor (str): The color of the note face. Default is 'blue'.
+        - noteFill (bool): Indicates whether the note should be filled. Default is True.
+        - noteEdgeColor (str): The color of the note edge. Default is 'black'.
+        - noteEdgeWidth (int): The width of the note edge. Default is 2.
+        - noteRadius (float): The radius of the note. Default is 0.4.
+        - noteOpacity (float): The opacity of the note. Default is 1.
+        - noteTextColor (str): The color of the text inside note.
+        - noteTextFont (str): The font of the text inside note.
+        - intervals (list): List of intervals associated with the note.
+        - scaleDegrees (list): List of scale degrees associated with the note.
+        - name (str): The name of the note.
+        - nameWithOctave (str): The name of the note with octave information.
+        - fret (int): The fret position of the note.
+        - string (int): The string position of the note.
+    """
     def __init__(self, **kwargs):
-        '''
+        """
         Initializes a CircleNote object with the specified properties.
 
         Parameters:
         - **kwargs (dict): Additional keyword arguments for customizing the note properties.
-        '''
+        """
         #more for drawing part
         self.noteFaceColor = kwargs.get('noteFaceColor', 'blue')
         self.noteFill = kwargs.get('noteFill', True)
         self.noteEdgeColor = kwargs.get('noteEdgeColor', 'black')
         self.noteEdgeWidth = kwargs.get('noteEdgeWidth', 2)
         self.noteRadius = kwargs.get('noteRadius', 0.4)
         self.noteOpactiy = kwargs.get('noteOpactiy', 1)
@@ -43,192 +43,192 @@
         
         #current note string and fret
         self.fret = kwargs.get('fret', None)
         self.string = kwargs.get('string', None)
         
     
     def getNoteRadius(self):
-        '''
+        """
         Get the radius of the note.
 
         Returns:
         - noteRadius (float): The radius of the note.
-        '''
+        """
         return self.noteRadius
     
     def setNoteRadius(self,radius):
-        '''
+        """
         Set the radius of the note.
 
         Parameters:
         - radius (float): The radius of the note.
-        '''
+        """
         self.noteRadius = radius
         
     def getNoteFaceColor(self):
-        '''
+        """
         Get the color of the note face.
 
         Returns:
         - noteFaceColor (str): The color of the note face.
-        '''
+        """
         return self.noteFaceColor
     
     def setNoteFaceColor(self,color):
-        '''
+        """
         Set the color of the note face.
 
         Parameters:
         - color (str): The color of the note face.
-        '''
+        """
         self.noteFaceColor = color
         
     def getNoteEdgeColor(self):
-        '''
+        """
         Get the color of the note edge.
 
         Returns:
         - noteEdgeColor (str): The color of the note edge.
-        '''
+        """
         return self.noteEdgeColor
     
     def setNoteEdgeColor(self,color):
-        '''
+        """
         Set the color of the note edge.
 
         Parameters:
         - color (str): The color of the note edge.
-        '''
+        """
         self.noteEdgeColor = color
         
     def getNoteEdgeWidth(self):
-        '''
+        """
         Get the width of the note edge.
 
         Returns:
         - noteEdgeWidth (int): The width of the note edge.
-        '''
+        """
         return self.noteEdgeWidth
     
     def setNoteEdgeWidth(self,lw):
-        '''
+        """
         Set the width of the note edge.
 
         Parameters:
         - lw (int): The width of the note edge.
-        '''
+        """
         self.noteEdgeWidth = lw
         
     def getNoteFill(self):
-        '''
+        """
         Check if the note is filled.
 
         Returns:
         - noteFill (bool): True if the note is filled, False otherwise.
-        '''
+        """
         return self.noteFill
     
     def setNoteFill(self,noteFill):
-        '''
+        """
         Set whether the note should be filled.
 
         Parameters:
         - noteFill (bool): True to fill the note, False to leave it empty.
-        '''
+        """
         self.noteFill = noteFill
 
     def getNoteOpacity(self):
-        '''
+        """
         Get the opacity of the note.
 
         Returns:
         - noteOpacity (float): The opacity of the note.
-        '''
+        """
         return self.noteOpactiy
 
     def setNoteOpacity(self,noteOpacity):
-        '''
+        """
         Set the opacity of the note.
 
         Parameters:
         - noteOpacity (float): The opacity of the note.
-        '''
+        """
         self.noteOpacity = noteOpacity
     
     def getIntervals(self):
-        '''
+        """
         Get the intervals associated with the note.
 
         Returns:
         - intervals (list): List of intervals associated with the note.
-        '''
+        """
         return self.intervals
     
     def setIntervals(self, interval):
-        '''
+        """
         Set the intervals associated with the note.
 
         Parameters:
         - interval (list): List of intervals to associate with the note.
-        '''
+        """
 
         self.intervals = interval
     
     def getScaleDegrees(self):
-        '''
+        """
         Get the scale degrees associated with the note.
 
         Returns:
         - scaleDegrees (list): List of scale degrees associated with the note.
-        '''
+        """
         return self.scaleDegrees
     
     def setScaleDegrees(self, scaleDegree):
-        '''
+        """
         Set the scale degrees associated with the note.
 
         Parameters:
         - scaleDegree (list): List of scale degrees to associate with the note.
-        '''
+        """
         self.scaleDegrees = scaleDegree
     
     def getName(self):
-        '''
+        """
         Get the name of the note.
 
         Returns:
         - name (str): The name of the note.
-        '''
+        """
         return self.name
     
     def setName(self, name):
-        '''
+        """
         Set the name of the note.
 
         Parameters:
         - name (str): The name of the note.
-        '''
+        """
         self.name = name
     
     def getNameWithOctave(self):
-        '''
+        """
         Get the name of the note with octave information.
 
         Returns:
         - nameWithOctave (str): The name of the note with octave information.
-        '''
+        """
         return self.nameWithOctave
     
     def setNameWithOctave(self, nameWithOctave):
-        '''
+        """
         Set the name of the note with octave information.
 
         Parameters:
         - nameWithOctave (str): The name of the note with octave information.
-        '''
+        """
         self.nameWithOctave = nameWithOctave
 
     def getNoteTextColor(self):
         """Get the color of the note text."""
         return self.noteTextColor
 
     def setNoteTextColor(self, value):
```

### Comparing `seeFretboard-0.1.5.2/seeFretboard/Designs/FretboardFigure.py` & `seeFretboard-0.1.5.3/seeFretboard/Designs/FretboardFigure.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 from bokeh.plotting import figure
 from bokeh.models import Range1d
 import seeFretboard.Utilities.Constants as Constants
 
 class FretboardFigure():
-    '''
+    """
     The FretboardFigure class is responsible for creating a Bokeh figure object that represents a guitar fretboard. 
     It allows for customization of the figure's orientation, size, and range, as well as the addition of string and fret labels. 
     The class also includes methods for switching the orientation of the figure and getting/setting the x and y ranges.
     
     Attributes:
-    - fig (figure): The Bokeh figure object.
-    - figHorXRange (Range1d): The x-range for the horizontal orientation.
-    - figHorYRange (Range1d): The y-range for the horizontal orientation.
-    - figVerXRange (Range1d): The x-range for the vertical orientation.
-    - figVerYRange (Range1d): The y-range for the vertical orientation.
-    - orientation (str): The orientation of the fretboard figure ('h' for horizontal, 'v' for vertical).
-    - stringLabel (str): The string label layout.
-    - fretLabel (str): The fret label layout.
-    - width (int): The width of the figure.
-    - height (int): The height of the figure.
-    '''
+        - fig (figure): The Bokeh figure object.
+        - figHorXRange (Range1d): The x-range for the horizontal orientation.
+        - figHorYRange (Range1d): The y-range for the horizontal orientation.
+        - figVerXRange (Range1d): The x-range for the vertical orientation.
+        - figVerYRange (Range1d): The y-range for the vertical orientation.
+        - orientation (str): The orientation of the fretboard figure ('h' for horizontal, 'v' for vertical).
+        - stringLabel (str): The string label layout.
+        - fretLabel (str): The fret label layout.
+        - width (int): The width of the figure.
+        - height (int): The height of the figure.
+    """
     def __init__(self, note, theme, orientation="h", width = None, height=None):
-        '''
+        """
         Initializes a FretboardFigure object with the specified parameters.
 
         Parameters:
         - note (CircleNote): The CircleNote object.
         - theme (Theme): The Theme object.
         - orientation (str): The orientation of the fretboard figure ('h' for horizontal, 'v' for vertical). Default is 'h'.
         - width (int): The width of the figure. Default is None.
         - height (int): The height of the figure. Default is None.
-        '''
+        """
 
         self.fig = figure()
-        self.figHorXRange = Range1d(-8*note.getNoteRadius(),
+        self.figHorXRange = Range1d(-10*note.getNoteRadius(),
                                         (theme.fretboardRange.numOfFrets+1.3)*theme.fretboardDesign.distanceBetweenFrets)
         self.figHorYRange = Range1d(-3*note.getNoteRadius(),
                                         theme.fretboardDesign.distanceBetweenStrings*theme.tuning.numOfStrings)
         self.figVerXRange = Range1d(-3*note.getNoteRadius(),
                                         theme.fretboardDesign.distanceBetweenStrings*theme.tuning.numOfStrings)
         self.figVerYRange = Range1d(-8*note.getNoteRadius(),
                                         (theme.fretboardRange.numOfFrets+2)*theme.fretboardDesign.distanceBetweenFrets)
 
         self.orientation = orientation
         if (orientation == "h"):
             if(width == None or height == None):
-                self.fig.width = 800
+                self.fig.width = 900
                 self.fig.height = 400
             else:
                 self.fig.width = width
                 self.fig.height = height
             self.fig.x_range = self.figHorXRange
             self.fig.y_range = self.figHorYRange
         
         else:
             if(width == None or height == None):
                 self.fig.width = 400
-                self.fig.height = 800
+                self.fig.height = 900
             else:
                 self.fig.width = width
                 self.fig.height = height
 
             self.fig.x_range = self.figVerXRange
             self.fig.y_range = self.figVerYRange
 
@@ -78,31 +78,31 @@
         return self._stringLabel
 
     @stringLabel.setter
     def stringLabel(self, stringLabel):
         self._stringLabel = stringLabel
 
     def addStringLabelLayout(self):
-        '''
+        """
         Adds the string label layout to the figure.
-        '''
+        """
         self.fig.add_layout(self.stringLabel)
 
     @property
     def fretLabel(self):
         return self._fretLabel
 
     @fretLabel.setter
     def fretLabel(self, fretLabel):
         self._fretLabel = fretLabel
 
     def addFretLabelLayout(self):
-        '''
+        """
         Adds the fret label layout to the figure.
-        '''
+        """
         self.fig.add_layout(self.fretLabel)
 
     @property
     def fig(self):
         return self._fig
 
     @fig.setter
@@ -122,87 +122,87 @@
         return self.fig.height
 
     @height.setter
     def height(self, height):
         self.fig.height = height
 
     def getFigHorXRange(self):
-        '''
+        """
         Returns the x-range for the horizontal orientation.
 
         Returns:
         - Range1d: The x-range for the horizontal orientation.
-        '''
+        """
         return self.figHorXRange
 
     def setFigHorXRange(self, v1, v2):
-        '''
+        """
         Sets the x-range for the horizontal orientation.
 
         Parameters:
         - v1: The starting value of the x-range.
         - v2: The ending value of the x-range.
-        '''
+        """
         self.figHorXRange = Range1d(v1, v2)
 
     def getFigHorYRange(self):
-        '''
+        """
         Returns the y-range for the horizontal orientation.
 
         Returns:
         - Range1d: The y-range for the horizontal orientation.
-        '''
+        """
         return self.figHorYRange
 
     def setFigHorYRange(self, v1, v2):
-        '''
+        """
         Sets the y-range for the horizontal orientation.
 
         Parameters:
         - v1: The starting value of the y-range.
         - v2: The ending value of the y-range.
-        '''
+        """
         self.figHorYRange = Range1d(v1, v2)
 
     def getFigVerXRange(self):
-        '''
+        """
         Returns the x-range for the vertical orientation.
 
         Returns:
         - Range1d: The x-range for the vertical orientation.
-        '''
+        """
         return self.figVerXRange
 
     def setFigVerXRange(self, v1, v2):
-        '''
+        """
         Sets the x-range for the vertical orientation.
 
         Parameters:
         - v1: The starting value of the x-range.
         - v2: The ending value of the x-range.
-        '''
+        """
         self.figVerXRange = Range1d(v1, v2)
 
     def getFigVerYRange(self):
-        '''
+        """
         Returns the y-range for the vertical orientation.
 
         Returns:
         - Range1d: The y-range for the vertical orientation.
-        '''
+        """
         return self.figVerYRange
 
     def setFigVerYRange(self, v1, v2):
-        '''
+        """
         Sets the y-range for the vertical orientation.
 
         Parameters:
         - v1: The starting value of the y-range.
         - v2: The ending value of the y-range.
-        '''
+        """
         self.figVerYRange = Range1d(v1, v2)
 
     @property
     def fig_x_range(self):
         return self.fig.x_range
 
     @fig_x_range.setter
@@ -214,20 +214,20 @@
         return self.fig.y_range
 
     @fig_y_range.setter
     def fig_y_range(self, value):
         self.fig.y_range = value
 
     def switchOrientation(self, orientation):
-        '''
+        """
         Switches the orientation of the fretboard figure.
 
         Parameters:
         - orientation (str): The new orientation ('h' for horizontal, 'v' for vertical).
-        '''
+        """
         if self.orientation != orientation:
             newH = self.width
             newW = self.height
             self.width = newW
             self.height = newH
         if orientation in Constants.VERTICAL:
             self.fig_x_range = self.getFigVerXRange()
```

### Comparing `seeFretboard-0.1.5.2/seeFretboard/Designs/FretboardStyle.py` & `seeFretboard-0.1.5.3/seeFretboard/Designs/FretboardStyle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from seeFretboard.Utilities.Constants import STANDARD_TUNING, STANDARD_TUNING_MIDI
 from seeFretboard.Designs.CirlceNote import CircleNote
 
-'''
+"""
 These classes can be used to configure and customize the settings of a guitar fretboard for various purposes.
-'''
+"""
 
 class FretboardTheme:
     """Represents a theme for the fretboard visualization."""
 
     def __init__(self, theme=None, **kwargs):
         """
         Initializes a FretboardTheme object.
 
         Parameters:
             theme (str): The theme to apply ("blue, dark, wood, or green"). If None, a custom theme (light basically) is applied.
             **kwargs: Additional keyword arguments for custom theme settings.
         """
-        theme = theme.lower()
+
         self.customTheme(**kwargs)
         if(theme == "blue"):
             self.BlueTheme()
         elif(theme== "dark"):
             self.darkTheme()
         elif (theme == "wood"):
             self.woodTheme()
```

### Comparing `seeFretboard-0.1.5.2/seeFretboard/NotePosition.py` & `seeFretboard-0.1.5.3/seeFretboard/NotePosition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 class NotePositionsOnCurrentFretboard():
-    '''
+    """
     The NotePositionsOnCurrentFretboard class represents a position of a note on a guitar fretboard. 
     It has two main attributes: the string number and the fret number. 
     The class provides methods to get and set these attributes.
-    '''
+    """
     def __init__(self, string, fret):
         self.string = string
         self.fret = fret
     
     def getFret(self):
         """
         Returns the fret number of the note position.
```

### Comparing `seeFretboard-0.1.5.2/seeFretboard/PitchCollection.py` & `seeFretboard-0.1.5.3/seeFretboard/PitchCollection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 class PitchCollection():
-    def __init__(self, pitchesType = "pitchesNames"):
+    def __init__(self, pitchesType = ""):
         """
         A class representing a collection of pitches musically.
         
         Args:
             pitchesType (str): The type of pitches to store.
 
         Attributes:
             pitchesNames (list): A list of pitch names.
             pitchesWithOctave (list): A list of pitches with octave.
             pitchesScaleDegrees (list): A list of pitch scale degrees.
-            pitchesType (str): The type of pitches being stored.
+            pitchesEmpty (list): A list of pitches for displaying nothing
+            pitchesType (str): The type of pitches being stored: "pitchesNames",pitchesWithOctave", or "pitchesScaleDegrees":
             pitchesIndex (int): The current index for accessing pitches.
             frets (list): A list of fret values that correspond to the pitches.
             strings (list): A list of string values that correspond to the pitches.
             arrayTypeNow (list): The current array type based on pitchesType.
         """
         self.pitchesNames = [""]
         self.pitchesWithOctave = [""]
         self.pitchesScaleDegrees = [""]
+        self.pitchesEmpty = [""]
         self.pitchesType = pitchesType
         self.pitchesIndex = 0
 
         self.frets = []
         self.strings = []
         self.arrayTypeNow = []
     
@@ -77,14 +79,30 @@
         """Appends a value to the pitchesWithOctave list."""
         self.pitchesWithOctave.append(value)
 
     def setPitchWithOctave(self, value):
         """Sets the pitchesWithOctave list to the given value."""
         self.pitchesWithOctave = value
     
+    def getPitchesEmpty(self):
+        """Returns the pitchesEmpty list."""
+        return self.pitchesEmpty
+    
+    def setPitchesEmpty(self, value):
+        """Sets the pitchesEmpty list to the given value."""
+        self.pitchesEmpty = value
+
+    def appendPitchesEmpty(self, value):
+        """Appends a value to the pitchesEmpty list."""
+        self.pitchesEmpty.append(value)
+    
+    def emptyPitchesEmpty(self):
+        """Empties the pitchesEmpty list."""
+        self.pitchesEmpty = []
+
     def emptyPitchesWithOctaves(self):
         """Empties the pitchesWithOctave list."""
         self.pitcheshWithOctave = []
 
     def getPitchesScaleDegrees(self):
         """Returns the pitchesScaleDegrees list."""
         return self.pitchesScaleDegrees
@@ -112,20 +130,23 @@
     def getArrayTypeNow(self):
         """
         Returns the current arrayType based on the pitchesType.
 
         Returns:
             list: The current arrayTypeNow list based on the pitchesType.
         """
+        pitchValue = []
         if self.pitchesType == "pitchesNames":
             pitchValue = self.pitchesNames
         elif self.pitchesType == "pitchesWithOctave":
             pitchValue = self.pitchesWithOctave
         elif self.pitchesType == "pitchesScaleDegrees":
             pitchValue = self.pitchesScaleDegrees
+        else:
+            pitchValue = self.pitchesEmpty
         
         self.arrayTypeNow = pitchValue
         
         return self.arrayTypeNow
     
     def getArrayTypeNowAt(self, index):
         """
@@ -225,7 +246,15 @@
         
         Returns:
             tuple: A tuple containing the current fret, string, and pitch values.
 
         """
         return self.getFretsAt(self.pitchesIndex), self.getStringsAt(self.pitchesIndex), self.getArrayTypeNowAt(self.pitchesIndex)
 
+    def setAllEmpty(self):
+        self.pitchesNames = []
+        self.pitchesWithOctave = []
+        self.pitchesScaleDegrees = []
+        self.pitchesEmpty = []
+        self.frets = []
+        self.strings = []
+        self.arrayTypeNow = []
```

### Comparing `seeFretboard-0.1.5.2/seeFretboard/Utilities/Constants.py` & `seeFretboard-0.1.5.3/seeFretboard/Utilities/Constants.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/seeFretboard/Utilities/Functions.py` & `seeFretboard-0.1.5.3/seeFretboard/Utilities/Functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,40 +86,63 @@
     midiNotes = []
     for fret in frets:
         midi = fretToMidi(string,fret)
         midiNotes.append(midi)
 
     return midiNotes
 
-def fretToMidi(string, fret):
+def fretToMidi(stringMidi, fret):
     """Converts a fret number on a string to a MIDI note number.
     
     Args:
-        string (int): The string number, where 1 is the highest pitch string.
+        string (int): The string number, is the midi string corresponding to that string the fret is on.
         fret (int): The fret number on the string. 
         
     Returns:
         midi (int): The MIDI note number corresponding to the fret on the string.
     """
-    midi = int(string) + int(fret)
+    if(isinstance(fret, str) and fret.lower() == "x"):
+        midi = "x"
+    else:
+        midi = int(stringMidi) + int(fret)
     
     return midi
 
+def midisToNoteNameWithOctaves(midiNote):
+    """Converts a list of MIDI note number to a list of note name with octave.
+    
+    Args:
+        midiNote (list): The list of MIDI note number.
+        
+    Returns:
+        noteNameWithOctave (list): The list of note name and octave (e.g. "C4", "F#5") corresponding to the MIDI note number.
+    """
+    nameOctaves = []
+    for midiNote in midiNote:
+        octave = midiToNoteNameWithOctave(midiNote)
+        nameOctaves.append(octave)
+
+    return nameOctaves
+
 def midiToNoteNameWithOctave(midiNote):
     """Converts a MIDI note number to a note name with octave.
     
     Args:
         midiNote (int): The MIDI note number.
         
     Returns:
         noteNameWithOctave (str): The note name and octave (e.g. "C4", "F#5") corresponding to the MIDI note number.
     """
-    note = music21.note.Note()
-    note.pitch.midi = midiNote
-    return note.nameWithOctave
+    if(isinstance(midiNote, str) and midiNote.lower() == "x"):
+        nameWithOctave = "x"
+    else:
+        note = music21.note.Note()
+        note.pitch.midi = float(midiNote)
+        nameWithOctave = note.nameWithOctave
+    return nameWithOctave
 
 def calculateHalfSteps(startNote, endNote):
     """
     Calculates the number of half steps between two notes, considering enharmonic equivalents.
 
     Args:
         startNote (str): The starting note.
@@ -216,15 +239,15 @@
 
         processedShape["note"][type].append(newNote)
         processedShape["position"][type].append(str(pos))
 
     return processedShape
 
 def processDropShape(drop, rootNote, type, string, shapePos):
-    '''
+    """
     Processes a drop shape by calculating the corresponding notes, positions, and scale degrees.
 
     Args:
         drop (str): The drop shape name.
         rootNote (str): The root note of the shape.
         type (str): The type of the chord: maj7, dom7, min7, min7b5, dim7
         string (str): The string of the shape.
@@ -239,15 +262,15 @@
             "position": {
                 type: [list of positions]
             },
             "scaleDegree": {
                 type: [list of scale degrees]
             }
         }
-    '''
+    """
     shape = DROPShapes[drop]
 
     interval = calculateHalfSteps("c", rootNote)
 
     processedShape = {
         "note": {},
         "position": {},
@@ -267,56 +290,56 @@
 
         processedShape["note"][type].append(newNote)
         processedShape["position"][type].append(str(pos))
 
     return processedShape
 
 def checkChordType(type,seve=False):
-    '''
+    """
     Checks if the provided chord type is valid.
 
     Args:
         type (str): The chord type to check.
         seve (bool): If True, check for valid chord types for seventh chords.
 
     Raises:
         ValueError: If the provided chord type is not valid.
-    '''
+    """
     type = type.lower()
     if seve:
         if type not in ["dom7", "dim7", "maj7", "min7","min7b5"]:
             raise ValueError("Invalid chord type provided.")
     
     if type not in ["maj", "min", "dim", "aug", "dom7", "dim7", "maj7", "min7","min7b5"]:
         raise ValueError("Invalid chord type provided.")
 
 def ifInDict(value, dictionary):
-    '''
+    """
     Checks if a value is present in a dictionary.
 
     Args:
         value: The value to check.
         dictionary (dict): The dictionary to check.
 
     Raises:
         ValueError: If the value is not present in the dictionary.
-    '''
+    """
     if value.upper() not in dictionary.keys():
         raise ValueError("Invalid "+value+" in "+getDictionaryName(dictionary))
 
 def getDictionaryName(dictionary):
-    '''
+    """
     Returns the name of a dictionary.
 
     Args:
         dictionary (dict): The dictionary.
 
     Returns:
         name (str): The name of the dictionary.
-    '''
+    """
     for name, value in globals().items():
         if value is dictionary:
             return name
     return None
 
 class customShapes():
     """
```

### Comparing `seeFretboard-0.1.5.2/seeFretboard/Utilities/PathInfo.py` & `seeFretboard-0.1.5.3/seeFretboard/Utilities/PathInfo.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/seeFretboard/Videos/Audio.py` & `seeFretboard-0.1.5.3/seeFretboard/Videos/Audio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/seeFretboard/Videos/Frame.py` & `seeFretboard-0.1.5.3/seeFretboard/Videos/Frame.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/seeFretboard/Videos/Images.py` & `seeFretboard-0.1.5.3/seeFretboard/Videos/Images.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 from seeFretboard.Utilities.Constants import BASE_PATH
 
 class Images():
-    '''
+    """
     The Images class is designed to create and manage image files. 
     It allows the user to set the output path, name, and file type 
     of the image, and automatically generates a file name based on 
     these parameters. The class also includes getter and setter methods 
     for each attribute, allowing for easy modification of the image properties.
     
     Attributes:
         outputPathName (str): The output path name where the image will be saved.
         name (str): The name of the image.
         meta (str): The file extension or meta information of the image.
         fileName (str): The full file path and name of the image.
-    '''
+    """
     def __init__(self):
         """
         Initializes an Images object with default attribute values.
         """
         self.outputPathName = os.path.join(BASE_PATH, 'Outputs', 'Images')
         self.name = "default"
         self.meta = ".png"
```

### Comparing `seeFretboard-0.1.5.2/seeFretboard/Videos/TabSequence.py` & `seeFretboard-0.1.5.3/seeFretboard/Videos/TabSequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 from seeFretboard.Utilities.Constants import BASE_PATH,FRAMERATE
 # set for 6 string in standard tuning for now
 
 # tab consist of many frames or the frames in certain period
 
 
 class TabSequence(Frame):
-    '''
+    """
     The TabSequence class is responsible for generating sequences of frame from audio files. 
     It uses the GuitarSet dataset to extract note information from audio tracks and converts 
     this information into tablature frames. The class can generate frames in either fret or 
     MIDI format and can convert between the two. It also provides methods for adding tablature 
     frames and converting frames to notes with time information.
-    '''
+    """
     def __init__(self, trackNum=0, frameRate=FRAMERATE, filePath=os.path.join(BASE_PATH, 'GuitarSet')):
-        '''
+        """
         Parameters:
             trackNum (int): The index of the track to load from the dataset.
             frameRate (float, optional): The frame rate of the tab sequence. Default is FRAMERATE.
             filePath (str, optional): The file path to the GuitarSet dataset. Default is 'BASE_PATH/GuitarSet'.
-            '''
+            """
         super().__init__(frameRate)
 
         self.filePath = filePath
         self.guitarset = mirdata.initialize(
             'guitarset', data_home=self.filePath)
 
         self.guitarsetIds = self.guitarset.track_ids  # the list of guitar's track ids
```

### Comparing `seeFretboard-0.1.5.2/seeFretboard/Videos/Video.py` & `seeFretboard-0.1.5.3/seeFretboard/Videos/Video.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from .Frame import Frame
 from seeFretboard.Utilities.Constants import BASE_PATH, FRAMERATE
 
 class Video(Frame):
-    '''
+    """
     The Video class is designed to represent a video and inherits from the Frame class. 
     It stores information about the video such as the start and end times, current frame,
     frame step, video name, file extension, codec, and audio name. The main functionalities
     of the class are to add frames to the video, set and get the video properties, and save the video.
     
     Attributes:
         frames (dict): A dictionary of frames with their corresponding time frames.
@@ -23,15 +23,15 @@
         videoPathWithName (str): The path to the video file.
         audioPath (str): The path to the audio directory.
         audioName (str): The name of the audio file.
         audioPathWithName (str): The path to the audio file.
         videoWAudioPath (str): The path to the video with audio directory.
         videoWAudioName (str): The name of the video with audio.
         videoWAudioPathWithName (str): The path to the video with audio file.
-    '''
+    """
     def __init__(self, startTime, endTime, currentFrame, frameStep, frameRate=FRAMERATE, videoName="defaultVid", fileExtension=".mp4", codec="mp4v", videoWAudioName="defaultVideoWAudio"):
         super().__init__(frameRate)
 
         # format = {{frameNumber:chordString},{0:"5,0,5,5,0,0"},{1:"5,0,5,5,0,0"}}
         self.frames = {}
 
         # all these are digits or the keys
```

### Comparing `seeFretboard-0.1.5.2/seeFretboard/Videos/VideoManager.py` & `seeFretboard-0.1.5.3/seeFretboard/Videos/VideoManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,63 +5,63 @@
 import ffmpeg
 import cv2
 
 from bokeh.io import export_png, export_svg
 import glob
 
 class VideoManager():
-    '''
+    """
     The VideoManager class provides functionalities to manage video and image files. 
     It allows the user to save video frames as images, generate a video from saved images,
     create a video with audio, and delete all saved images. It also provides options to 
     display a progress bar while generating images and to set the output file format for 
     images.
 
     Attributes:
         fretboard (Fretboard): The Fretboard object.
         video (Video): The Video object.
         images (Images): The Images object.
         imageProgressBar (bool): Flag indicating whether to display a progress bar while generating images.
-    '''
+    """
     def __init__(self, fretboard, video, images, imageProgressBar=True):
         self.fretboard = fretboard
         self.video = video
         self.images = images
         self.imageProgressBar = imageProgressBar
 
     def saveAsVideoImages(self):
-        '''
+        """
         Saves video frames as images.
 
         This method iterates over the frames of the video and saves each frame as an image.
 
         Raises:
             FileNotFoundError: If the output directory specified in the Images object does not exist.
-        '''
+        """
         oriImgName = self.images.name
         print(oriImgName)
         for k, v in self.video.getFramesItems():
             self.fretboard.updateFretboard(v)
             self.images.name = str(k)+oriImgName
             self.saveImage()
             print("saving"+self.images.name)
         print("done")
 
     # 
     def saveAsVideoImagesNoSeconds(self):
-        '''
+        """
         Saves video frames as images when the number of seconds is not defined.
         For guitarset and other data where number of second is not defined
 
         This method saves video frames as images without considering the number of seconds.
         It uses a dictionary to track previously saved frames to avoid duplicate saving.
 
         Raises:
             FileNotFoundError: If the output directory specified in the Images object does not exist.
-        '''
+        """
         oriImgName = self.images.name
         images = {}
         print("IMAGES Generateing")
         for i in tqdm(range(len(self.video.getFrames())), disable=not(self.imageProgressBar)):
             frame = self.video.getFrames()[i]
             self.images.name = str(i)+oriImgName
 
@@ -74,23 +74,23 @@
                 self.saveImage()
                 image = Image.open(os.path.join(
                     self.images.outputPathName, self.images.name + self.images.meta))
                 images[frame] = image.copy()
         print("IMAGES Generate done")
 
     def saveAsVideo(self):
-        '''
+        """
         Generates a video from saved images.
 
         This method reads the saved images, orders them based on their filenames, and
         creates a video from the ordered frames.
 
         Raises:
             FileNotFoundError: If the output directory specified in the Images object does not exist.
-        '''
+        """
         images = os.listdir(self.images.outputPathName)
         images = sorted(images, key=lambda s: [
                         int(x) if x.isdigit() else x for x in re.split('(\d+)', s)])
 
         fourcc = cv2.VideoWriter_fourcc(*self.video.getCodec())
         frameSize = (self.fretboard.fretboardFig.fig.width, self.fretboard.fretboardFig.fig.height)
 
@@ -104,94 +104,94 @@
         cv2.destroyAllWindows()
         videoWriter.release()
 
         print("VIDEO " + self.video.getVideoName() +
               " saved at "+self.video.getVideoPathName())
 
     def createVideoWithAudio(self):
-        '''
+        """
         Creates a video with audio.
 
         This method combines the video file and audio file into a single video file with audio.
 
         Raises:
             FileNotFoundError: If the video or audio files specified in the Video object do not exist.
-        '''
+        """
         self.saveAsVideo()
 
         videoPath = ffmpeg.input(
             self.video.getVideoPathWithName()+self.video.getFileExtension())
         audioPath = ffmpeg.input(self.video.getAudioPathWithName())
 
 
         ffmpeg.concat(videoPath, audioPath, v=1, a=1).output(
             self.video.getVideoWAudioPathWithName()).run(overwrite_output=True)
         print("video save with audio done")
 
     def saveVideoWithAudio(self):
-        '''
+        """
         Saves a video with audio.
 
         This method combines the video file and audio file into a single video file with audio
         and saves it with a specified name.
 
         Raises:
             FileNotFoundError: If the video or audio files specified in the Video object do not exist.
-        '''
+        """
         videoPath = ffmpeg.input(
             self.video.getVideoPathWithName()+self.video.getFileExtension())
         audioPath = ffmpeg.input(self.video.getAudioPathWithName())
 
         ffmpeg.concat(videoPath, audioPath, v=1, a=1).output(
             self.video.getVideoName(
             )+".mp4").run(overwrite_output=True)
         print("video save with audio done")
     
     def saveImage(self):
-        '''
+        """
         Saves the fretboard visualization as an image.
 
         This method saves the current state of the fretboard visualization as an image file.
         The image format is determined by the file extension specified in the Images object.
         png and svg for now.
 
         Raises:
             FileNotFoundError: If the output directory specified in the Images object does not exist.
-        '''
+        """
         if (self.images.meta.lower() == ".png"):
             export_png(self.fretboard.getFretboardFig().fig, filename=self.images.fileName)
 
         elif (self.images.meta.lower() == ".svg"):
             export_svg(self.fretboard.getFretboardFig().fig, filename=self.images.fileName)
 
 
     def deleteAllImages(self):
-        '''
+        """
         Deletes all saved images.
 
         This method deletes all image files in the output directory specified in the Images object.
 
         Raises:
             FileNotFoundError: If the output directory specified in the Images object does not exist.
-        '''
+        """
         files = glob.glob(os.path.join(self.images.outputPathName, "*"))
         for f in files:
             os.remove(f)
         print("All Images Delete")
 
         
     @property
     def imageProgressBar(self):
-        '''
+        """
         bool: Flag indicating whether to display a progress bar while generating images.
-        '''
+        """
         return self._imageProgressBar
 
     @imageProgressBar.setter
     def imageProgressBar(self, imageProgressBar):
-        '''
+        """
         Setter for the imageProgressBar property.
 
         Args:
             imageProgressBar (bool): Flag indicating whether to display a progress bar while generating images.
-        '''
+        """
         self._imageProgressBar = imageProgressBar
```

### Comparing `seeFretboard-0.1.5.2/seeFretboard/Videos/VideoNote.py` & `seeFretboard-0.1.5.3/seeFretboard/Videos/VideoNote.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/seeFretboard.egg-info/PKG-INFO` & `seeFretboard-0.1.5.3/seeFretboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeFretboard
-Version: 0.1.5.2
+Version: 0.1.5.3
 Summary: For Release
 Home-page: https://github.com/LindaRZhang/seeFretboard
 Author: Linda Rong Zhang
 Author-email: ronglindaz@gmail.com
 License: GNU
 Project-URL: Bug Tracker, https://github.com/LindaRZhang/seeFretboard/issues
 Description-Content-Type: text/markdown
```

### Comparing `seeFretboard-0.1.5.2/seeFretboard.egg-info/SOURCES.txt` & `seeFretboard-0.1.5.3/seeFretboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.1.5.2/setup.py` & `seeFretboard-0.1.5.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='seeFretboard',
-    version='0.1.5.2',
+    version='0.1.5.3',
     author='Linda Rong Zhang',
     author_email='ronglindaz@gmail.com',
     description='For Release',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/LindaRZhang/seeFretboard',
     project_urls={
```

