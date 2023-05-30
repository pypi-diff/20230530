# Comparing `tmp/zoom-python-client-0.0.5.tar.gz` & `tmp/zoom_python_client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoom-python-client-0.0.5.tar", last modified: Mon May 22 10:10:00 2023, max compression
+gzip compressed data, was "zoom_python_client-0.0.6.tar", max compression
```

## Comparing `zoom-python-client-0.0.5.tar` & `zoom_python_client-0.0.6.tar`

### file list

```diff
@@ -1,111 +1,24 @@
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.120776 zoom-python-client-0.0.5/
--rw-r--r--   0 rene       (501) staff       (20)       49 2022-09-06 12:27:11.000000 zoom-python-client-0.0.5/.coveragerc
--rw-r--r--   0 rene       (501) staff       (20)       65 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/.env.sample
--rw-r--r--   0 rene       (501) staff       (20)      137 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.flake8
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.008241 zoom-python-client-0.0.5/.github/
--rw-r--r--   0 rene       (501) staff       (20)     2918 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.github/CONTRIBUTING.md
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.013650 zoom-python-client-0.0.5/.github/workflows/
--rw-r--r--   0 rene       (501) staff       (20)     2325 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 rene       (501) staff       (20)      246 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.github/workflows/pre-commit.yaml
--rw-r--r--   0 rene       (501) staff       (20)      776 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.github/workflows/python-tests.yml
--rw-r--r--   0 rene       (501) staff       (20)     3086 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.gitignore
--rw-r--r--   0 rene       (501) staff       (20)      634 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 rene       (501) staff       (20)       14 2022-09-05 07:24:11.000000 zoom-python-client-0.0.5/.tool-versions
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.015264 zoom-python-client-0.0.5/.vscode/
--rw-r--r--   0 rene       (501) staff       (20)      475 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.vscode/settings.json
--rw-r--r--   0 rene       (501) staff       (20)    35149 2023-05-04 09:49:35.000000 zoom-python-client-0.0.5/LICENSE
--rw-r--r--   0 rene       (501) staff       (20)     3211 2023-05-22 10:10:00.120063 zoom-python-client-0.0.5/PKG-INFO
--rw-r--r--   0 rene       (501) staff       (20)     2632 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/README.md
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.021841 zoom-python-client-0.0.5/example/
--rw-r--r--   0 rene       (501) staff       (20)        0 2022-09-06 14:27:54.000000 zoom-python-client-0.0.5/example/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      355 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/example/get_meeting_livestream.py
--rw-r--r--   0 rene       (501) staff       (20)      317 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/example/get_user.py
--rw-r--r--   0 rene       (501) staff       (20)      630 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/example/get_user_meetings.py
--rw-r--r--   0 rene       (501) staff       (20)      938 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/example/set_meeting_livestream.py
--rw-r--r--   0 rene       (501) staff       (20)     1269 2023-05-22 10:08:43.000000 zoom-python-client-0.0.5/pyproject.toml
--rw-r--r--   0 rene       (501) staff       (20)      153 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/pytest.ini
--rw-r--r--   0 rene       (501) staff       (20)      145 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/requirements.dev.txt
--rw-r--r--   0 rene       (501) staff       (20)       63 2023-05-22 10:08:43.000000 zoom-python-client-0.0.5/requirements.txt
--rw-r--r--   0 rene       (501) staff       (20)       38 2023-05-22 10:10:00.121046 zoom-python-client-0.0.5/setup.cfg
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.023390 zoom-python-client-0.0.5/tests/
--rw-r--r--   0 rene       (501) staff       (20)        0 2022-09-05 07:32:56.000000 zoom-python-client-0.0.5/tests/__init__.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.024782 zoom-python-client-0.0.5/tests/utils/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/utils/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      176 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/utils/test_logger.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.031434 zoom-python-client-0.0.5/tests/zoom_python_client/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      405 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/base_test_case.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.033934 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/__init__.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.036425 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meeting_livestreams/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meeting_livestreams/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     3980 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meeting_livestreams/test_meeting_livestreams_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.039542 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meetings/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meetings/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1200 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meetings/test_meetings_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.046503 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/users/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/users/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1193 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/users/test_users_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.049817 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinar_livestreams/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinar_livestreams/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     3980 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinar_livestreams/test_webinar_livestreams_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.053669 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinars/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinars/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      748 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinars/test_webinars_component.py
--rw-r--r--   0 rene       (501) staff       (20)     1792 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/test_api_client.py
--rw-r--r--   0 rene       (501) staff       (20)     1757 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/test_zoom_api_client.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.056331 zoom-python-client-0.0.5/tests/zoom_python_client/utils/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/utils/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      185 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/utils/test_file_system.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.058652 zoom-python-client-0.0.5/tests/zoom_python_client/zoom_auth_api/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/zoom_auth_api/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1897 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/zoom_auth_api/test_zoom_auth_api_client.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:09:59.976798 zoom-python-client-0.0.5/venv/
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.080321 zoom-python-client-0.0.5/venv/bin/
--rwxr-xr-x   0 rene       (501) staff       (20)      649 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2html.py
--rwxr-xr-x   0 rene       (501) staff       (20)      771 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2html4.py
--rwxr-xr-x   0 rene       (501) staff       (20)     1106 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2html5.py
--rwxr-xr-x   0 rene       (501) staff       (20)      848 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2latex.py
--rwxr-xr-x   0 rene       (501) staff       (20)      671 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2man.py
--rwxr-xr-x   0 rene       (501) staff       (20)      837 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2odt.py
--rwxr-xr-x   0 rene       (501) staff       (20)     2193 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 rene       (501) staff       (20)      656 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 rene       (501) staff       (20)      692 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2s5.py
--rwxr-xr-x   0 rene       (501) staff       (20)      928 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2xetex.py
--rwxr-xr-x   0 rene       (501) staff       (20)      657 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2xml.py
--rwxr-xr-x   0 rene       (501) staff       (20)      725 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rstpep2html.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.086321 zoom-python-client-0.0.5/zoom_python_client/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     2401 2023-05-08 09:39:49.000000 zoom-python-client-0.0.5/zoom_python_client/api_client.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.092756 zoom-python-client-0.0.5/zoom_python_client/client_components/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/__init__.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.095579 zoom-python-client-0.0.5/zoom_python_client/client_components/meeting_livestreams/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/meeting_livestreams/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1722 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.100113 zoom-python-client-0.0.5/zoom_python_client/client_components/meetings/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/meetings/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      624 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/meetings/meetings_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.103139 zoom-python-client-0.0.5/zoom_python_client/client_components/users/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/users/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1286 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/users/users_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.105756 zoom-python-client-0.0.5/zoom_python_client/client_components/webinar_livestreams/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/webinar_livestreams/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1583 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.108782 zoom-python-client-0.0.5/zoom_python_client/client_components/webinars/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/webinars/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      401 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/webinars/webinars_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.115703 zoom-python-client-0.0.5/zoom_python_client/utils/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/utils/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      221 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/utils/file_system.py
--rw-r--r--   0 rene       (501) staff       (20)      731 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/zoom_python_client/utils/logger.py
--rw-r--r--   0 rene       (501) staff       (20)     5030 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/zoom_python_client/zoom_api_client.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.118693 zoom-python-client-0.0.5/zoom_python_client/zoom_auth_api/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/zoom_auth_api/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     2816 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py
--rw-r--r--   0 rene       (501) staff       (20)      817 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/zoom_client_interface.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.091885 zoom-python-client-0.0.5/zoom_python_client.egg-info/
--rw-r--r--   0 rene       (501) staff       (20)     3211 2023-05-22 10:09:59.000000 zoom-python-client-0.0.5/zoom_python_client.egg-info/PKG-INFO
--rw-r--r--   0 rene       (501) staff       (20)     3309 2023-05-22 10:09:59.000000 zoom-python-client-0.0.5/zoom_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 rene       (501) staff       (20)        1 2023-05-22 10:09:59.000000 zoom-python-client-0.0.5/zoom_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 rene       (501) staff       (20)      192 2023-05-22 10:09:59.000000 zoom-python-client-0.0.5/zoom_python_client.egg-info/requires.txt
--rw-r--r--   0 rene       (501) staff       (20)       29 2023-05-22 10:09:59.000000 zoom-python-client-0.0.5/zoom_python_client.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35149 2023-05-30 07:49:07.890357 zoom_python_client-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3306 2023-05-30 07:49:07.890357 zoom_python_client-0.0.6/README.md
+-rw-r--r--   0        0        0     1384 2023-05-30 07:49:07.890357 zoom_python_client-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 07:49:07.890357 zoom_python_client-0.0.6/zoom_python_client/__init__.py
+-rw-r--r--   0        0        0     2401 2023-05-30 07:49:07.890357 zoom_python_client-0.0.6/zoom_python_client/api_client.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:49:07.890357 zoom_python_client-0.0.6/zoom_python_client/client_components/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/meeting_livestreams/__init__.py
+-rw-r--r--   0        0        0     1722 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/meetings/__init__.py
+-rw-r--r--   0        0        0      624 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/meetings/meetings_component.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/users/__init__.py
+-rw-r--r--   0        0        0     1286 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/users/users_component.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/webinar_livestreams/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/webinars/__init__.py
+-rw-r--r--   0        0        0      401 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/webinars/webinars_component.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/utils/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/utils/file_system.py
+-rw-r--r--   0        0        0      731 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/utils/logger.py
+-rw-r--r--   0        0        0     5954 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/zoom_api_client.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/zoom_auth_api/__init__.py
+-rw-r--r--   0        0        0     4629 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py
+-rw-r--r--   0        0        0      817 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/zoom_client_interface.py
+-rw-r--r--   0        0        0     4338 1970-01-01 00:00:00.000000 zoom_python_client-0.0.6/PKG-INFO
```

### Comparing `zoom-python-client-0.0.5/LICENSE` & `zoom_python_client-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.5/PKG-INFO` & `zoom_python_client-0.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: zoom-python-client
-Version: 0.0.5
-Summary: Zoom API client for Python
-Author-email: Rene Fernandez <rene.fernandez@cern.ch>
-Project-URL: Homepage, https://github.com/cern-vc/zoom-python-client
-Project-URL: Bug Tracker, https://github.com/cern-vc/zoom-python-client/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Zoom Python client
 
 [![Python tests](https://github.com/cern-vc/zoom-python-client/actions/workflows/python-tests.yml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/python-tests.yml) [![pre-commit](https://github.com/cern-vc/zoom-python-client/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/pre-commit.yaml) [![CodeQL](https://github.com/cern-vc/zoom-python-client/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/codeql-analysis.yml) [![codecov](https://codecov.io/gh/cern-vc/zoom-python-client/branch/main/graph/badge.svg?token=04EY0K0P2S)](https://codecov.io/gh/cern-vc/zoom-python-client)
 
 > ⚠️ WIP: This project is a WIP and therefore may contain bugs. Use it at your own risk and keep this in mind if you decide to use it in production environments.
 
 Zoom API Python client with support for [Server to Server Oauth tokens](https://developers.zoom.us/docs/internal-apps/s2s-oauth/)
@@ -53,14 +38,30 @@
 
 zoom_client = ZoomApiClient(
         account_id="<YOUR ACCOUNT ID>",
         client_id="<YOUR CLIENT ID>",
         client_secret="<YOUR CLIENT SECRET>")
 ```
 
+### Use the file system to store the access token instead of environment
+
+There are some cases where you might want to store the access token in the file system in order to share its value with other elements of the application (Ex. different pods on a Kubernetes/Openshift application).
+
+You can define the path where the token will be stored, passing the `use_path` variable to the constructor:
+
+```python
+from src.zoom_python_client.zoom_api_client import ZoomApiClient
+
+zoom_client = ZoomApiClient(
+        account_id="<YOUR ACCOUNT ID>",
+        client_id="<YOUR CLIENT ID>",
+        client_secret="<YOUR CLIENT SECRET>",
+        use_path="/path/to/token/folder")
+```
+
 
 ## How to make API calls
 
 ```python
 MEETING_ID = "12345"
 USER_ID = "abcdfgh"
 
@@ -92,8 +93,8 @@
 2. update live stream
 3. update livestream status
 ### **webinars**:
 1. get webinar details
 ### **webinar live streams**:
 1. get webinar live stream
 2. update webinar live stream
-3. update webinar livestream status
+3. update webinar livestream status
```

### Comparing `zoom-python-client-0.0.5/zoom_python_client/api_client.py` & `zoom_python_client-0.0.6/zoom_python_client/api_client.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.5/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py` & `zoom_python_client-0.0.6/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.5/zoom_python_client/client_components/meetings/meetings_component.py` & `zoom_python_client-0.0.6/zoom_python_client/client_components/meetings/meetings_component.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.5/zoom_python_client/client_components/users/users_component.py` & `zoom_python_client-0.0.6/zoom_python_client/client_components/users/users_component.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.5/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py` & `zoom_python_client-0.0.6/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.5/zoom_python_client/utils/logger.py` & `zoom_python_client-0.0.6/zoom_python_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.5/zoom_python_client/zoom_api_client.py` & `zoom_python_client-0.0.6/zoom_python_client/zoom_api_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import os
-from typing import Any, Mapping, Union
+from typing import Any, Mapping, Optional, Union
 
 import requests
 from dotenv import load_dotenv
 
 from zoom_python_client.api_client import ApiClient
 from zoom_python_client.client_components.meeting_livestreams.meeting_livestreams_component import (
     MeetingLiveStreamsComponent,
@@ -37,31 +37,36 @@
     pass
 
 
 class ZoomApiClient(ZoomClientInterface):
     api_endpoint: str = "https://api.zoom.us/v2"
 
     @staticmethod
-    def init_from_env():
+    def init_from_env(use_path: Optional[str] = None):
         try:
             account_id = os.environ["ZOOM_ACCOUNT_ID"]
             client_id = os.environ["ZOOM_CLIENT_ID"]
             client_secret = os.environ["ZOOM_CLIENT_SECRET"]
-            zoom_client = ZoomApiClient(account_id, client_id, client_secret)
+            zoom_client = ZoomApiClient(
+                account_id, client_id, client_secret, use_path=use_path
+            )
             return zoom_client
         except KeyError as error:
             raise ZoomClientEnvError(
                 f"Required key not in environment: {error}"
             ) from error
 
     @staticmethod
-    def init_from_dotenv(custom_dotenv=".env"):
+    def init_from_dotenv(
+        custom_dotenv=".env",
+        use_path: Optional[str] = None,
+    ):
         project_dir = get_project_dir()
         load_dotenv(os.path.join(project_dir, custom_dotenv), verbose=True)
-        zoom_client = ZoomApiClient.init_from_env()
+        zoom_client = ZoomApiClient.init_from_env(use_path=use_path)
         return zoom_client
 
     def init_components(self):
         # Add all the new components here
         self.users = UsersComponent(self)
         self.meetings = MeetingsComponent(self)
         self.meeting_livestreams = MeetingLiveStreamsComponent(self)
@@ -70,37 +75,51 @@
 
     def __init__(
         self,
         account_id: str,
         client_id: str,
         client_secret: str,
         api_endpoint="https://api.zoom.us/v2",
+        use_path: Optional[str] = None,
     ):
         self.api_endpoint = api_endpoint
+        self.use_path = use_path
         self.api_client = ApiClient(self.api_endpoint)
         self.authentication_client = ZoomAuthApiClient(
-            account_id, client_id, client_secret
+            account_id, client_id, client_secret, use_path=use_path
         )
 
         # Initialize components
         self.init_components()
 
+    def load_access_token_and_expire_seconds(self):
+        if self.use_path:
+            logger.debug("Loading token from file")
+            # If the token is in a file, we need to get the token from the file
+            access_token = self.authentication_client.get_access_token_from_file()
+            expire_seconds = self.authentication_client.get_expire_seconds_from_file()
+        else:
+            logger.debug("Loading token from environment")
+            access_token = os.getenv("ZOOM_ACCESS_TOKEN", default=None)
+            expire_seconds = os.getenv("ZOOM_ACCESS_TOKEN_EXPIRE", default=None)
+        return access_token, expire_seconds
+
     def build_zoom_authorization_headers(self, force_token=False) -> dict:
-        access_token = os.getenv("ZOOM_ACCESS_TOKEN", default=None)
-        expire_seconds = os.getenv("ZOOM_ACCESS_TOKEN_EXPIRE", default=None)
+        access_token, expire_seconds = self.load_access_token_and_expire_seconds()
+        token_from = "file" if self.use_path else "environment"
         if (
             not access_token
             or not expire_seconds
-            or self.authentication_client.is_zoom_access_token_expired()
+            or self.authentication_client.is_zoom_access_token_expired(expire_seconds)
             or force_token
         ):
-            logger.debug("Token is not in the environment. Requesting new token.")
+            logger.debug(f"Token is not in the {token_from}. Requesting new token.")
             access_token = self.authentication_client.get_acceess_token()
         else:
-            logger.debug("The token is the environment. No need for a new token.")
+            logger.debug(f"The token is the {token_from}. No need for a new token.")
         zoom_headers = {"Authorization": "Bearer " + access_token}
         headers = self.api_client.build_headers(extra_headers=zoom_headers)
         return headers
 
     def build_query_string_from_dict(self, parameters: dict) -> str:
         query_string = "?"
         for key, value in parameters.items():
```

### Comparing `zoom-python-client-0.0.5/zoom_python_client/zoom_client_interface.py` & `zoom_python_client-0.0.6/zoom_python_client/zoom_client_interface.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.5/zoom_python_client.egg-info/PKG-INFO` & `zoom_python_client-0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 Metadata-Version: 2.1
 Name: zoom-python-client
-Version: 0.0.5
-Summary: Zoom API client for Python
-Author-email: Rene Fernandez <rene.fernandez@cern.ch>
-Project-URL: Homepage, https://github.com/cern-vc/zoom-python-client
-Project-URL: Bug Tracker, https://github.com/cern-vc/zoom-python-client/issues
-Classifier: Programming Language :: Python :: 3
+Version: 0.0.6
+Summary: Zoom API client for Python using server to server tokens
+Home-page: https://github.com/cern-vc/zoom-python-client
+License: GPL-3.0-only
+Keywords: zoom,api
+Author: Rene Fernandez Sanchez
+Author-email: rene.fernandez@cern.ch
+Maintainer: Rene Fernandez Sanchez
+Maintainer-email: rene.fernandez@cern.ch
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: python-dotenv (==0.21.0)
+Requires-Dist: requests (==2.23.0)
+Requires-Dist: typing-extensions (==4.3.0)
+Project-URL: Bug Tracker, https://github.com/cern-vc/zoom-python-client/issues
+Project-URL: Repository, https://github.com/cern-vc/zoom-python-client
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
 
 # Zoom Python client
 
 [![Python tests](https://github.com/cern-vc/zoom-python-client/actions/workflows/python-tests.yml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/python-tests.yml) [![pre-commit](https://github.com/cern-vc/zoom-python-client/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/pre-commit.yaml) [![CodeQL](https://github.com/cern-vc/zoom-python-client/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/codeql-analysis.yml) [![codecov](https://codecov.io/gh/cern-vc/zoom-python-client/branch/main/graph/badge.svg?token=04EY0K0P2S)](https://codecov.io/gh/cern-vc/zoom-python-client)
 
 > ⚠️ WIP: This project is a WIP and therefore may contain bugs. Use it at your own risk and keep this in mind if you decide to use it in production environments.
 
@@ -53,14 +63,30 @@
 
 zoom_client = ZoomApiClient(
         account_id="<YOUR ACCOUNT ID>",
         client_id="<YOUR CLIENT ID>",
         client_secret="<YOUR CLIENT SECRET>")
 ```
 
+### Use the file system to store the access token instead of environment
+
+There are some cases where you might want to store the access token in the file system in order to share its value with other elements of the application (Ex. different pods on a Kubernetes/Openshift application).
+
+You can define the path where the token will be stored, passing the `use_path` variable to the constructor:
+
+```python
+from src.zoom_python_client.zoom_api_client import ZoomApiClient
+
+zoom_client = ZoomApiClient(
+        account_id="<YOUR ACCOUNT ID>",
+        client_id="<YOUR CLIENT ID>",
+        client_secret="<YOUR CLIENT SECRET>",
+        use_path="/path/to/token/folder")
+```
+
 
 ## How to make API calls
 
 ```python
 MEETING_ID = "12345"
 USER_ID = "abcdfgh"
```

