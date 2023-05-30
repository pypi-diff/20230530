# Comparing `tmp/pop-create-idem-3.4.1.tar.gz` & `tmp/pop-create-idem-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-create-idem-3.4.1.tar", last modified: Tue May  9 14:57:04 2023, max compression
+gzip compressed data, was "pop-create-idem-3.5.0.tar", last modified: Tue May 30 15:37:55 2023, max compression
```

## Comparing `pop-create-idem-3.4.1.tar` & `pop-create-idem-3.5.0.tar`

### file list

```diff
@@ -1,132 +1,156 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.413895 pop-create-idem-3.4.1/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8796 2023-05-09 14:57:04.413895 pop-create-idem-3.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7947 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.408395 pop-create-idem-3.4.1/cloudspec/
--rw-r--r--   0 root         (0) root         (0)     8546 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/cloudspec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/cloudspec/conf.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/cloudspec/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.408395 pop-create-idem-3.4.1/pop_create_idem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.408395 pop-create-idem-3.4.1/pop_create_idem/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.409312 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/
--rw-r--r--   0 root         (0) root         (0)     3158 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/auto_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.409312 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/contracts/
--rw-r--r--   0 root         (0) root         (0)       78 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/docs.py
--rw-r--r--   0 root         (0) root         (0)     2780 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/exec_modules.py
--rw-r--r--   0 root         (0) root         (0)     3241 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/state_modules.py
--rw-r--r--   0 root         (0) root         (0)      270 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/templates.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/tests.py
--rw-r--r--   0 root         (0) root         (0)     3080 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/tool.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.409312 pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/
--rw-r--r--   0 root         (0) root         (0)     2154 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/function.py
--rw-r--r--   0 root         (0) root         (0)     5802 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/param.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.410228 pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/
--rw-r--r--   0 root         (0) root         (0)     3477 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/auto_state.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/exec.py
--rw-r--r--   0 root         (0) root         (0)      822 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/state.py
--rw-r--r--   0 root         (0) root         (0)      209 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/tool.py
--rw-r--r--   0 root         (0) root         (0)     2075 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.406561 pop-create-idem-3.4.1/pop_create_idem/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.410228 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.410228 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)     1764 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.410228 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)     2509 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
--rw-r--r--   0 root         (0) root         (0)      173 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.410228 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.404728 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.410228 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2633 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      626 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.404728 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      960 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.404728 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.404728 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      763 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      917 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)     3854 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1548 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412062 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/
--rw-r--r--   0 root         (0) root         (0)     3899 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412062 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/hooks/
--rw-r--r--   0 root         (0) root         (0)     1302 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     5076 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/init.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/params.py
--rw-r--r--   0 root         (0) root         (0)     6475 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/parse.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.406561 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412062 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1740 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/
--rw-r--r--   0 root         (0) root         (0)     1348 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
--rw-r--r--   0 root         (0) root         (0)      700 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
--rw-r--r--   0 root         (0) root         (0)     1885 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
--rw-r--r--   0 root         (0) root         (0)     1539 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
--rw-r--r--   0 root         (0) root         (0)     1408 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/
--rw-r--r--   0 root         (0) root         (0)     1903 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
--rw-r--r--   0 root         (0) root         (0)      941 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
--rw-r--r--   0 root         (0) root         (0)     4298 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/
--rw-r--r--   0 root         (0) root         (0)     1411 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.406561 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     2749 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/rest/
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/rest/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/swagger/
--rw-r--r--   0 root         (0) root         (0)      708 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/swagger/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.406561 pop-create-idem-3.4.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.413895 pop-create-idem-3.4.1/pop_create_idem/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.413895 pop-create-idem-3.4.1/pop_create_idem/tool/format/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/format/case.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/format/html.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/format/inflect.py
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/format/keyword.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/format/wrap.py
--rw-r--r--   0 root         (0) root         (0)      878 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/gradle.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/jinja.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-09 14:57:03.000000 pop-create-idem-3.4.1/pop_create_idem/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.408395 pop-create-idem-3.4.1/pop_create_idem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8796 2023-05-09 14:57:04.000000 pop-create-idem-3.4.1/pop_create_idem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5938 2023-05-09 14:57:04.000000 pop-create-idem-3.4.1/pop_create_idem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 14:57:04.000000 pop-create-idem-3.4.1/pop_create_idem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-09 14:57:04.000000 pop-create-idem-3.4.1/pop_create_idem.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-09 14:57:04.000000 pop-create-idem-3.4.1/pop_create_idem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-09 14:57:04.000000 pop-create-idem-3.4.1/pop_create_idem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-09 14:57:04.414812 pop-create-idem-3.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3004 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.261520 pop-create-idem-3.5.0/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-05-30 15:37:55.261520 pop-create-idem-3.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7947 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/cloudspec/
+-rw-r--r--   0 root         (0) root         (0)     8621 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/cloudspec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/cloudspec/conf.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/cloudspec/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/
+-rw-r--r--   0 root         (0) root         (0)     3158 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/auto_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/contracts/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/docs.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/exec_modules.py
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/state_modules.py
+-rw-r--r--   0 root         (0) root         (0)      270 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/templates.py
+-rw-r--r--   0 root         (0) root         (0)     5528 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/tests.py
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/tool.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/cloudspec/parse/
+-rw-r--r--   0 root         (0) root         (0)     2167 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/parse/function.py
+-rw-r--r--   0 root         (0) root         (0)     6216 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/parse/param.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/parse/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/cloudspec/template/
+-rw-r--r--   0 root         (0) root         (0)     3477 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/template/auto_state.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/template/exec.py
+-rw-r--r--   0 root         (0) root         (0)      943 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/template/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/template/state.py
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/template/test.py
+-rw-r--r--   0 root         (0) root         (0)      209 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/cloudspec/template/tool.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
+-rw-r--r--   0 root         (0) root         (0)      173 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/tests.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.249520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/
+-rw-r--r--   0 root         (0) root         (0)     4724 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     5629 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/init.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/params.py
+-rw-r--r--   0 root         (0) root         (0)     6475 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/parse.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
+-rw-r--r--   0 root         (0) root         (0)      700 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
+-rw-r--r--   0 root         (0) root         (0)      941 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
+-rw-r--r--   0 root         (0) root         (0)     4300 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2
+-rw-r--r--   0 root         (0) root         (0)      539 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2
+-rw-r--r--   0 root         (0) root         (0)      819 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/
+-rw-r--r--   0 root         (0) root         (0)      456 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/default.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.257520 pop-create-idem-3.5.0/pop_create_idem/pop_create/rest/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/rest/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.261520 pop-create-idem-3.5.0/pop_create_idem/pop_create/swagger/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/swagger/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.261520 pop-create-idem-3.5.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.261520 pop-create-idem-3.5.0/pop_create_idem/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.261520 pop-create-idem-3.5.0/pop_create_idem/tool/format/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/tool/format/case.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/tool/format/html.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/tool/format/inflect.py
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/tool/format/keyword.py
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/tool/format/wrap.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/tool/gradle.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/pop_create_idem/tool/jinja.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-30 15:37:54.000000 pop-create-idem-3.5.0/pop_create_idem/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:37:55.253520 pop-create-idem-3.5.0/pop_create_idem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-05-30 15:37:55.000000 pop-create-idem-3.5.0/pop_create_idem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7964 2023-05-30 15:37:55.000000 pop-create-idem-3.5.0/pop_create_idem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 15:37:55.000000 pop-create-idem-3.5.0/pop_create_idem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-30 15:37:55.000000 pop-create-idem-3.5.0/pop_create_idem.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-30 15:37:55.000000 pop-create-idem-3.5.0/pop_create_idem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-30 15:37:55.000000 pop-create-idem-3.5.0/pop_create_idem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-30 15:37:55.261520 pop-create-idem-3.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-05-30 15:37:41.000000 pop-create-idem-3.5.0/setup.py
```

### Comparing `pop-create-idem-3.4.1/LICENSE` & `pop-create-idem-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/PKG-INFO` & `pop-create-idem-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 3.4.1
+Version: 3.5.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-3.4.1/README.rst` & `pop-create-idem-3.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/cloudspec/__init__.py` & `pop-create-idem-3.5.0/cloudspec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         virtual_imports: List[str] = None,
         contracts: List[str] = None,
         func_alias: Dict[str, str] = None,
         virtualname: str = "",
         sub_virtual: bool = None,
         sub_alias: List[str] = None,
         functions: Dict[str, Dict[str, Dict[str, str]]] = None,
+        file_vars: Dict[str, Any] = None,
     ):
         """
         Args:
             doc: A docstring for this function
             imports: python imports that will for sure be available, program crashes if not available
             virtual_imports: python imports that prevent the module from loading, plugin does not load if not available
             contracts: A list of contracts to implement for this plugin
@@ -126,14 +127,15 @@
             virtual_imports=virtual_imports or [],
             contracts=contracts or [],
             func_alias=func_alias or {},
             virtualname=virtualname,
             sub_virtual=sub_virtual,
             sub_alias=sub_alias,
             functions=validated_functions,
+            file_vars=file_vars,
         )
 
 
 class CloudSpecFunction(NamespaceDict):
     """
     .. code-block:: json
```

### Comparing `pop-create-idem-3.4.1/cloudspec/conf.py` & `pop-create-idem-3.5.0/cloudspec/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/auto_state.py` & `pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/exec_modules.py` & `pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/exec_modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
         cli_ref = hub.cloudspec.parse.plugin.mod_ref(ctx, ref, plugin)
 
         plugin["func_alias"] = {"list_": "list"}
 
         to_write = hub.cloudspec.parse.plugin.header(plugin)
 
         for function_name, function_data in plugin.functions.items():
-
             if function_name in ["present", "absent", "describe"]:
                 # If plugin comes in with all methods, let's not create for state_modules functions
                 continue
 
             request_format_template_file = f"{template_dir}/{function_name}.jinja2"
             if os.path.isfile(request_format_template_file):
                 with open(f"{template_dir}/{function_name}.jinja2", "rb+") as f:
@@ -42,30 +41,35 @@
 
             template = hub.tool.jinja.template(
                 f"{hub.cloudspec.template.exec.FUNCTION}\n    {request_format}\n\n\n"
             )
 
             function_alias = plugin.func_alias.get(function_name, function_name)
 
-            to_write += template.render(
-                function=dict(
-                    name=function_name,
-                    hardcoded=function_data.hardcoded,
-                    doc=hub.cloudspec.parse.function.doc(function_data)
-                    + hub.cloudspec.parse.param.sphinx_docs(function_data.params)
-                    + hub.cloudspec.parse.function.return_type(function_data),
-                    ref=f"{ref}.{function_alias}",
-                    cli_ref=f"{cli_ref}.{function_alias}",
-                    header_params=hub.cloudspec.parse.param.headers(
-                        function_data.params
+            try:
+                to_write += template.render(
+                    function=dict(
+                        name=function_name,
+                        hardcoded=function_data.hardcoded,
+                        doc=hub.cloudspec.parse.function.doc(function_data)
+                        + hub.cloudspec.parse.param.sphinx_docs(function_data.params)
+                        + hub.cloudspec.parse.function.return_type(function_data),
+                        ref=f"{ref}.{function_alias}",
+                        cli_ref=f"{cli_ref}.{function_alias}",
+                        header_params=hub.cloudspec.parse.param.headers(
+                            function_data.params
+                        ),
+                        required_call_params=hub.cloudspec.parse.param.required_call_params(
+                            function_data.params
+                        ),
+                        return_type=function_data.return_type,
                     ),
-                    required_call_params=hub.cloudspec.parse.param.callers(
-                        function_data.params
+                    parameter=dict(
+                        mapping=hub.cloudspec.parse.param.mappings(function_data.params)
                     ),
-                    return_type=function_data.return_type,
-                ),
-                parameter=dict(
-                    mapping=hub.cloudspec.parse.param.mappings(function_data.params)
-                ),
-            )
+                )
+            except Exception as err:
+                hub.log.warning(
+                    f"Warning when generating function's action definitions for {function_name}: {err.__class__.__name__}: {err}"
+                )
 
         mod_file.write_text(to_write)
```

### Comparing `pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/state_modules.py` & `pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/state_modules.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,20 +64,25 @@
                 else:
                     request_format = cloud_spec.request_format.get(function_name)
 
                 template = hub.tool.jinja.template(
                     f"{TEMPLATE}\n    {request_format}\n\n\n"
                 )
 
-                to_write += template.render(
-                    service_name=cloud_spec.service_name,
-                    function=dict(
-                        ref=ref,
-                        state_ref=f"states.{state_ref}",
-                        **func_data[function_name]["function"],
-                    ),
-                    parameter=func_data[function_name]["parameter"],
-                    present_parameter=present_parameter,
-                    get_params=common_params,
-                )
+                try:
+                    to_write += template.render(
+                        service_name=cloud_spec.service_name,
+                        function=dict(
+                            ref=ref,
+                            state_ref=f"states.{state_ref}",
+                            **func_data[function_name]["function"],
+                        ),
+                        parameter=func_data[function_name]["parameter"],
+                        present_parameter=present_parameter,
+                        get_params=common_params,
+                    )
+                except Exception as err:
+                    hub.log.warning(
+                        f"Warning when generating function's action definitions for {function_name}: {err.__class__.__name__}: {err}"
+                    )
 
                 mod_file.write_text(to_write)
```

### Comparing `pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/tool.py` & `pop-create-idem-3.5.0/pop_create_idem/cloudspec/create/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,23 +60,28 @@
                     # cloudspec was provided with hardcoded request format
                     request_format = cloud_spec.request_format.get(func_name)
 
                 template = hub.tool.jinja.template(
                     f"{hub.cloudspec.template.tool.FUNCTION}\n    {request_format}\n\n"
                 )
 
-                to_write += template.render(
-                    function=dict(
-                        name=func_name,
-                        ref=ref,
-                        module_ref=f"tool.{module_ref}",
-                        **func_data,
-                        header_params=hub.cloudspec.parse.param.headers(
-                            func_data.params
+                try:
+                    to_write += template.render(
+                        function=dict(
+                            name=func_name,
+                            ref=ref,
+                            module_ref=f"tool.{module_ref}",
+                            **func_data,
+                            header_params=hub.cloudspec.parse.param.headers(
+                                func_data.params
+                            ),
                         ),
-                    ),
-                    parameter=dict(
-                        mapping=hub.cloudspec.parse.param.mappings(func_data.params)
-                    ),
-                )
+                        parameter=dict(
+                            mapping=hub.cloudspec.parse.param.mappings(func_data.params)
+                        ),
+                    )
+                except Exception as err:
+                    hub.log.warning(
+                        f"Warning when generating function's action definitions for {func_name}: {err.__class__.__name__}: {err}"
+                    )
 
         mod_file.write_text(to_write)
```

### Comparing `pop-create-idem-3.4.1/pop_create_idem/cloudspec/init.py` & `pop-create-idem-3.5.0/pop_create_idem/cloudspec/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/function.py` & `pop-create-idem-3.5.0/pop_create_idem/cloudspec/parse/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 function=dict(
                     name=function_name,
                     hardcoded=function_data.hardcoded,
                     doc=doc,
                     header_params=hub.cloudspec.parse.param.headers(
                         function_data.params
                     ),
-                    required_call_params=hub.cloudspec.parse.param.callers(
+                    required_call_params=hub.cloudspec.parse.param.required_call_params(
                         function_data.params
                     ),
                 ),
                 parameter=dict(
                     mapping=param_mapping,
                 ),
             )
```

### Comparing `pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/param.py` & `pop-create-idem-3.5.0/pop_create_idem/cloudspec/parse/param.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,29 +143,42 @@
         ret += f"), "
     else:
         ret += f", field(default={param_data.default})), "
 
     return ret
 
 
-def callers(hub, parameters: CloudSpecParam) -> str:
+def required_call_params(hub, parameters: CloudSpecParam) -> str:
     """
-    Get a mapping of the function args to the values that will be used in the final caller
+    Get a mapping of required function args to the values that will be used in the final caller
     """
     ret = []
 
     required_params = {
         name: data for name, data in parameters.items() if data["required"]
     }
     for param_data in required_params.values():
         ret.append(f"{param_data.snaked}={param_data.default or 'value'}")
 
     return ", ".join(ret)
 
 
+def all_call_params(hub, parameters: CloudSpecParam) -> str:
+    """
+    Get a mapping of all function args to the values that will be used in the final caller
+    """
+    ret = []
+
+    all_params = {name: data for name, data in parameters.items()}
+    for param_data in all_params.values():
+        ret.append(f"{param_data.snaked}={param_data.default or 'value'}")
+
+    return ", ".join(ret)
+
+
 def mappings(hub, parameters: CloudSpecParam) -> Dict[str, str]:
     ret = {}
     map_params = {
         name: data
         for name, data in parameters.items()
         if data["target_type"] == "mapping"
     }
```

### Comparing `pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/plugin.py` & `pop-create-idem-3.5.0/pop_create_idem/cloudspec/parse/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/auto_state.py` & `pop-create-idem-3.5.0/pop_create_idem/cloudspec/template/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/exec.py` & `pop-create-idem-3.5.0/pop_create_idem/cloudspec/template/exec.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/plugin.py` & `pop-create-idem-3.5.0/pop_create_idem/cloudspec/template/plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,8 +37,14 @@
 {%- if plugin.sub_alias -%}
 __sub_alias__ = {{plugin.sub_alias}}
 {%- endif %}
 
 {% if plugin.func_alias -%}
 __func_alias__ = {{plugin.func_alias}}
 {% endif %}
+
+{% if plugin.file_vars %}
+{% for var, val in plugin.file_vars.items() %}
+{{ var }} = {{ val }}
+{% endfor %}
+{% endif %}
 '''
```

### Comparing `pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/state.py` & `pop-create-idem-3.5.0/pop_create_idem/cloudspec/template/state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/conf.py` & `pop-create-idem-3.5.0/pop_create_idem/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,15 +34,21 @@
             root_directory,
             create_plugins=["auto_state", "tool", "state_modules", "tests", "docs"],
         )
     elif ctx.create_plugin == "templates":
         hub.cloudspec.init.run(
             ctx,
             root_directory,
-            create_plugins=["templates", "tests", "docs"],
+            create_plugins=["templates"],
+        )
+    elif ctx.create_plugin == "test_modules":
+        hub.cloudspec.init.run(
+            ctx,
+            root_directory,
+            create_plugins=["templates", "tests"],
         )
     else:
         raise ValueError(f"Invalid input '{ctx.create_plugin}' for --create-plugin.")
 
     # Sanitize based on other arguments
     if ctx.has_acct_plugin:
         hub.tool.path.rmtree(root_directory / ctx.clean_name / "acct")
```

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/init.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/function.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/function.py`

 * *Files 24% similar despite different names*

```diff
@@ -113,7 +113,31 @@
                             schema_ref, all_schemas
                         )
                     )
     except Exception as e:
         hub.log.debug(f"Failed to parse response mapping: {e.__class__.__name__}: {e}")
 
     return response_mappings
+
+
+def create_test_for_function(
+    hub, ctx, func_name: str, func_data: dict
+) -> Dict[str, Any]:
+    if func_name in ["get", "list", "create", "update", "delete"]:
+        test_module_type = "exec"
+    elif func_name in ["present", "absent", "describe"]:
+        test_module_type = "states"
+    else:
+        test_module_type = "tool"
+
+    return {
+        "doc": "",
+        "hardcoded": {
+            "resource_name": func_data.get("hardcoded", {}).get("resource_name"),
+            "service_name": ctx.service_name,
+            # This is critical to derive rendering location
+            "test_module_type": test_module_type,
+            # Add calling method's metadata such as name, call params etc.
+            "method_call_name": func_name,
+            "method_call_params": func_data.get("params"),
+        },
+    }
```

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/init.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/init.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,14 +67,17 @@
 
         # Get function plugins
         plugins = hub.pop_create.openapi3.parse.plugins(ctx, api)
 
         # Add any missing function which is required for idem resource modules
         plugins = hub.pop_create.openapi3.init.add_missing_known_functions(ctx, plugins)
 
+        # Add tests function
+        plugins = hub.pop_create.openapi3.init.add_tests_functions(ctx, plugins)
+
         cloud_spec = NamespaceDict(
             api_version=ctx.cloud_api_version,
             project_name=ctx.project_name,
             service_name=ctx.service_name,
             request_format={},
             plugins=plugins,
         )
@@ -135,7 +138,20 @@
                     )
                 elif func_name == "list":
                     plugins[ref]["functions"]["describe"] = (
                         plugins.get(ref).get("functions", {}).get(func_name)
                     )
 
     return plugins
+
+
+def add_tests_functions(hub, ctx, plugins):
+    for ref in list(plugins):
+        functions = plugins[ref].get("functions", {}).copy()
+        for func_name, func_data in functions.items():
+            plugins[ref]["functions"][
+                f"test_{func_name}"
+            ] = hub.pop_create.openapi3.function.create_test_for_function(
+                ctx=ctx, func_name=func_name, func_data=func_data
+            )
+
+    return plugins
```

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/params.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/params.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/parse.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/parse.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/schemas.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/schemas.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -15,31 +15,31 @@
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
         if ctx.test:
-            result["comment"] = f"Would delete {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}:{name}"
+            result["comment"] = f"Would delete {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}"
             return result
 
         delete_ret = await hub.exec.{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}.delete(
             ctx,
             name=name,
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
-            result["comment"].append(f"Deleted '{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}:{name}'")
+            result["comment"].append(f"Deleted {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}")
         else:
             # If there is any failure in create/update, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
-        result["comment"].append(f"'{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}:{name}' already absent")
+        result["comment"].append(f"{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name} already absent")
         return result
 
     result["old_state"] = before.ret
     return result
```

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -31,50 +31,50 @@
 
         if bool(changes.get("new")):
             if ctx.test:
                 result["new_state"] = hub.tool.{{ function.hardcoded.service_name }}.test_state_utils.generate_test_state(
                     enforced_state={},
                     desired_state=desired_state
                 )
-                result["comment"] = (f"Would update {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }} '{name}'",)
+                result["comment"] = (f"Would update {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}",)
                 return result
             else:
                 # Update the resource
                 update_ret = await hub.exec.{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}.update(
                     ctx,
                     name=name,
                     resource_id=resource_id,
                     **kwargs,
                     # TODO: Add other required parameters (including tags, if necessary): **{{ parameter.mapping.kwargs|default({}) }}
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
-                    result["comment"].append(f"Updated '{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}:{name}'")
+                    result["comment"].append(f"Updated '{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}'")
                 else:
                     result["comment"].append(update_ret["comment"])
     else:
         if ctx.test:
             result["new_state"] = hub.tool.{{ function.hardcoded.service_name }}.test_state_utils.generate_test_state(
                 enforced_state={},
                 desired_state=desired_state
             )
-            result["comment"] = (f"Would create {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }} {name}",)
+            result["comment"] = (f"Would create {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}",)
             return result
         else:
             create_ret = await hub.exec.{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}.create(
                 ctx,
                 name=name,
                 **kwargs
                 # TODO: Add other required parameters from: **{{ parameter.mapping.kwargs|default({})}}
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
-                result["comment"].append(f"Created '{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}:{name}'")
+                result["comment"].append(f"Created '{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}'")
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
                 result["new_state"] = dict(name=name, resource_id=resource_id)
             else:
                 result["comment"].append(create_ret["comment"])
 
     if not result["result"]:
```

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/pop_create/swagger/init.py` & `pop-create-idem-3.5.0/pop_create_idem/pop_create/swagger/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/tool/format/case.py` & `pop-create-idem-3.5.0/pop_create_idem/tool/format/case.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/tool/format/inflect.py` & `pop-create-idem-3.5.0/pop_create_idem/tool/format/inflect.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem/tool/gradle.py` & `pop-create-idem-3.5.0/pop_create_idem/tool/gradle.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.1/pop_create_idem.egg-info/PKG-INFO` & `pop-create-idem-3.5.0/pop_create_idem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 3.4.1
+Version: 3.5.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-3.4.1/pop_create_idem.egg-info/SOURCES.txt` & `pop-create-idem-3.5.0/pop_create_idem.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -26,21 +26,23 @@
 pop_create_idem/cloudspec/parse/function.py
 pop_create_idem/cloudspec/parse/param.py
 pop_create_idem/cloudspec/parse/plugin.py
 pop_create_idem/cloudspec/template/auto_state.py
 pop_create_idem/cloudspec/template/exec.py
 pop_create_idem/cloudspec/template/plugin.py
 pop_create_idem/cloudspec/template/state.py
+pop_create_idem/cloudspec/template/test.py
 pop_create_idem/cloudspec/template/tool.py
 pop_create_idem/pop_create/idem_cloud/init.py
 pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
 pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
+pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/tests.in
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
@@ -51,25 +53,38 @@
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
 pop_create_idem/pop_create/openapi3/function.py
 pop_create_idem/pop_create/openapi3/init.py
 pop_create_idem/pop_create/openapi3/params.py
 pop_create_idem/pop_create/openapi3/parse.py
 pop_create_idem/pop_create/openapi3/schemas.py
 pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/__init__.py
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/__init__.py
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/__init__.py
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/default.jinja2
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
 pop_create_idem/pop_create/rest/init.py
 pop_create_idem/pop_create/swagger/init.py
 pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
 pop_create_idem/tool/gradle.py
 pop_create_idem/tool/jinja.py
```

### Comparing `pop-create-idem-3.4.1/setup.py` & `pop-create-idem-3.5.0/setup.py`

 * *Files identical despite different names*

