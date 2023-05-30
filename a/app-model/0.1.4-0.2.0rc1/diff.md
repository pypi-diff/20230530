# Comparing `tmp/app_model-0.1.4.tar.gz` & `tmp/app_model-0.2.0rc1.tar.gz`

## Comparing `app_model-0.1.4.tar` & `app_model-0.2.0rc1.tar`

### file list

```diff
@@ -1,85 +1,86 @@
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 app_model-0.1.4/.github_changelog_generator
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 app_model-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 app_model-0.1.4/.readthedocs.yaml
--rw-r--r--   0        0        0    10999 2020-02-02 00:00:00.000000 app_model-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 app_model-0.1.4/codecov.yml
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 app_model-0.1.4/mkdocs.yml
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 app_model-0.1.4/setup.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 app_model-0.1.4/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 app_model-0.1.4/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 app_model-0.1.4/.github/dependabot.yml
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 app_model-0.1.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 app_model-0.1.4/.github/workflows/cron.yml
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 app_model-0.1.4/demo/keybinding_helper.py
--rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 app_model-0.1.4/demo/model_app.py
--rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 app_model-0.1.4/demo/qapplication.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 app_model-0.1.4/demo/multi_file/__init__.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 app_model-0.1.4/demo/multi_file/__main__.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 app_model-0.1.4/demo/multi_file/actions.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 app_model-0.1.4/demo/multi_file/app.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 app_model-0.1.4/demo/multi_file/constants.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 app_model-0.1.4/demo/multi_file/functions.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 app_model-0.1.4/docs/_macros.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 app_model-0.1.4/docs/application.md
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 app_model-0.1.4/docs/expressions.md
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 app_model-0.1.4/docs/index.md
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 app_model-0.1.4/docs/keybindings.md
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 app_model-0.1.4/docs/registries.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 app_model-0.1.4/docs/types.md
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/__init__.py
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/backends/__init__.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/backends/qt/__init__.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/backends/qt/_qaction.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/backends/qt/_qkeybindingedit.py
--rw-r--r--   0        0        0    16388 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/backends/qt/_qkeymap.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/backends/qt/_qmainwindow.py
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/backends/qt/_qmenu.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/backends/qt/_util.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/expressions/__init__.py
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/expressions/_context.py
--rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/expressions/_context_keys.py
--rw-r--r--   0        0        0    19026 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/expressions/_expressions.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/registries/__init__.py
--rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/registries/_commands_reg.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/registries/_keybindings_reg.py
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/registries/_menus_reg.py
--rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/registries/_register.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/types/__init__.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/types/_action.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/types/_base.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/types/_command_rule.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/types/_constants.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/types/_icon.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/types/_keybinding_rule.py
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/types/_menu_rule.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/types/_utils.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/types/_keys/__init__.py
--rw-r--r--   0        0        0    33529 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/types/_keys/_key_codes.py
--rw-r--r--   0        0        0     8891 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/types/_keys/_keybindings.py
--rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 app_model-0.1.4/src/app_model/types/_keys/_standard_bindings.py
--rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_actions.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_app.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_command_registry.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_key_codes.py
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_keybindings.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_registries.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_types.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/fixtures/fake_module.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_context/test_context.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_context/test_context_keys.py
--rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_context/test_expressions.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_qt/__init__.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_qt/test_demos.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_qt/test_qactions.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_qt/test_qkeybindingedit.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_qt/test_qkeymap.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_qt/test_qmainwindow.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 app_model-0.1.4/tests/test_qt/test_qmenu.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 app_model-0.1.4/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 app_model-0.1.4/LICENSE
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 app_model-0.1.4/README.md
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 app_model-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 app_model-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.github_changelog_generator
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.readthedocs.yaml
+-rw-r--r--   0        0        0    11612 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/codecov.yml
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/mkdocs.yml
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/setup.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.github/dependabot.yml
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.github/workflows/cron.yml
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/keybinding_helper.py
+-rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/model_app.py
+-rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/qapplication.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/multi_file/__init__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/multi_file/__main__.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/multi_file/actions.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/multi_file/app.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/multi_file/constants.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/multi_file/functions.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/_macros.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/application.md
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/expressions.md
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/index.md
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/keybindings.md
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/registries.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/types.md
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/__init__.py
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/_app.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/_pydantic_compat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/__init__.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/__init__.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/_qaction.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/_qkeybindingedit.py
+-rw-r--r--   0        0        0    16388 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/_qkeymap.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/_qmainwindow.py
+-rw-r--r--   0        0        0    12837 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/_qmenu.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/_util.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/expressions/__init__.py
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/expressions/_context.py
+-rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/expressions/_context_keys.py
+-rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/expressions/_expressions.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/registries/__init__.py
+-rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/registries/_commands_reg.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/registries/_keybindings_reg.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/registries/_menus_reg.py
+-rw-r--r--   0        0        0     8777 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/registries/_register.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/__init__.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_action.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_command_rule.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_constants.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_icon.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_keybinding_rule.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_menu_rule.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_utils.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_keys/__init__.py
+-rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_keys/_key_codes.py
+-rw-r--r--   0        0        0     9966 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_keys/_keybindings.py
+-rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_keys/_standard_bindings.py
+-rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_actions.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_app.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_command_registry.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_key_codes.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_keybindings.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_registries.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_types.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/fixtures/fake_module.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_context/test_context.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_context/test_context_keys.py
+-rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_context/test_expressions.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/__init__.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/test_demos.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/test_qactions.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/test_qkeybindingedit.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/test_qkeymap.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/test_qmainwindow.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/test_qmenu.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/LICENSE
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/README.md
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/PKG-INFO
```

### Comparing `app_model-0.1.4/.pre-commit-config.yaml` & `app_model-0.2.0rc1/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   autofix_commit_msg: "style: [pre-commit.ci] auto fixes [...]"
   autoupdate_commit_msg: "ci: [pre-commit.ci] autoupdate"
 
 default_install_hook_types: [pre-commit, commit-msg]
 
 repos:
   - repo: https://github.com/compilerla/conventional-pre-commit
-    rev: v2.1.1
+    rev: v2.2.0
     hooks:
       - id: conventional-pre-commit
         stages: [commit-msg]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
@@ -21,26 +21,26 @@
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.260
+    rev: v0.0.263
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.12.2
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.2.0
     hooks:
       - id: mypy
         files: "^src/"
         additional_dependencies:
           - pydantic
           - in-n-out
```

### Comparing `app_model-0.1.4/CHANGELOG.md` & `app_model-0.2.0rc1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 # Changelog
 
-## [0.1.4](https://github.com/pyapp-kit/app-model/tree/0.1.4) (2023-04-06)
+## [0.2.0](https://github.com/pyapp-kit/app-model/tree/0.2.0) (2023-05-30)
 
-[Full Changelog](https://github.com/pyapp-kit/app-model/compare/v0.1.3...0.1.4)
+[Full Changelog](https://github.com/pyapp-kit/app-model/compare/v0.1.4...0.2.0)
+
+**Merged pull requests:**
+
+- fix: fix menu titles in QtModelMenuBar [\#102](https://github.com/pyapp-kit/app-model/pull/102) ([tlambert03](https://github.com/tlambert03))
+- ci: \[pre-commit.ci\] autoupdate [\#99](https://github.com/pyapp-kit/app-model/pull/99) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- feat: support pydantic v2 [\#98](https://github.com/pyapp-kit/app-model/pull/98) ([tlambert03](https://github.com/tlambert03))
+
+## [v0.1.4](https://github.com/pyapp-kit/app-model/tree/v0.1.4) (2023-04-06)
+
+[Full Changelog](https://github.com/pyapp-kit/app-model/compare/v0.1.3...v0.1.4)
 
 **Merged pull requests:**
 
 - build: pin pydantic \< 2 [\#96](https://github.com/pyapp-kit/app-model/pull/96) ([tlambert03](https://github.com/tlambert03))
 
 ## [v0.1.3](https://github.com/pyapp-kit/app-model/tree/v0.1.3) (2023-04-06)
```

### Comparing `app_model-0.1.4/mkdocs.yml` & `app_model-0.2.0rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/setup.py` & `app_model-0.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/.github/workflows/ci.yml` & `app_model-0.2.0rc1/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -46,23 +46,52 @@
         run: |
           python -m pip install -U pip
           python -m pip install -e .[test]
 
       - name: Test
         run: pytest -s --color=yes
 
+  test-pydantic2:
+    name: pydantic2 (py${{ matrix.python-version }})
+    runs-on: ubuntu-latest
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ["3.8", "3.10", "3.11"]
+
+    steps:
+      - uses: actions/checkout@v3
+
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      - name: Install dependencies
+        run: |
+          python -m pip install -U pip
+          python -m pip install -e .[test]
+          pip install -U --pre pydantic
+
+      - name: Test
+        run: pytest --color=yes --cov=app_model --cov-report=xml
+
+      - name: Coverage
+        uses: codecov/codecov-action@v3
+
+
   test-qt:
     name: ${{ matrix.platform }} ${{ matrix.qt-backend }} (${{ matrix.python-version }})
     runs-on: ${{ matrix.platform }}
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.10"]
         platform: [macos-latest, ubuntu-latest, windows-latest]
-        qt-backend: [PyQt5, PyQt6, PySide2, PySide6]
+        qt-backend: [PyQt5, PyQt6, PySide2, "'PySide6<6.5.1'"]
         include:
           - python-version: "3.8"
             platform: "ubuntu-latest"
             qt-backend: "PyQt5==5.12"
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `app_model-0.1.4/.github/workflows/cron.yml` & `app_model-0.2.0rc1/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/demo/model_app.py` & `app_model-0.2.0rc1/demo/model_app.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/demo/qapplication.py` & `app_model-0.2.0rc1/demo/qapplication.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/demo/multi_file/actions.py` & `app_model-0.2.0rc1/demo/multi_file/actions.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/demo/multi_file/app.py` & `app_model-0.2.0rc1/demo/multi_file/app.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/docs/_macros.py` & `app_model-0.2.0rc1/docs/_macros.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/docs/index.md` & `app_model-0.2.0rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/docs/types.md` & `app_model-0.2.0rc1/docs/types.md`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/_app.py` & `app_model-0.2.0rc1/src/app_model/_app.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/backends/qt/__init__.py` & `app_model-0.2.0rc1/src/app_model/backends/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/backends/qt/_qaction.py` & `app_model-0.2.0rc1/src/app_model/backends/qt/_qaction.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/backends/qt/_qkeybindingedit.py` & `app_model-0.2.0rc1/src/app_model/backends/qt/_qkeybindingedit.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/backends/qt/_qkeymap.py` & `app_model-0.2.0rc1/src/app_model/backends/qt/_qkeymap.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/backends/qt/_qmainwindow.py` & `app_model-0.2.0rc1/src/app_model/backends/qt/_qmainwindow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Collection, List, Optional, Union
+from __future__ import annotations
+
+from typing import Collection, Mapping, Optional, Sequence, Union
 
 from qtpy.QtCore import Qt
 from qtpy.QtWidgets import QMainWindow, QWidget
 
 from app_model import Application
 
 from ._qmenu import QModelMenuBar, QModelToolBar
@@ -13,16 +15,24 @@
 
     def __init__(
         self, app: Union[str, Application], parent: Optional[QWidget] = None
     ) -> None:
         super().__init__(parent)
         self._app = Application.get_or_create(app) if isinstance(app, str) else app
 
-    def setModelMenuBar(self, menu_ids: List[str]) -> QModelMenuBar:
-        """Set the menu bar to a list of menu ids."""
+    def setModelMenuBar(
+        self, menu_ids: Mapping[str, str] | Sequence[str | tuple[str, str]]
+    ) -> QModelMenuBar:
+        """Set the menu bar to a list of menu ids.
+
+        Parameters
+        ----------
+        menu_ids : Mapping[str, str] | Sequence[str | tuple[str, str]]
+            A mapping of menu ids to menu titles or a sequence of menu ids.
+        """
         menu_bar = QModelMenuBar(menu_ids, self._app, self)
         self.setMenuBar(menu_bar)
         return menu_bar
 
     def addModelToolBar(
         self,
         menu_id: str,
```

### Comparing `app_model-0.1.4/src/app_model/backends/qt/_qmenu.py` & `app_model-0.2.0rc1/src/app_model/backends/qt/_qmenu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import (
     TYPE_CHECKING,
     Collection,
     Iterable,
-    List,
     Mapping,
     Optional,
+    Sequence,
     Set,
     Union,
     cast,
 )
 
 from qtpy.QtWidgets import QMenu, QMenuBar, QToolBar
 
@@ -255,26 +255,38 @@
 
     def _on_registry_changed(self, changed_ids: Set[str]) -> None:
         if self._menu_id in changed_ids:
             self.rebuild()
 
 
 class QModelMenuBar(QMenuBar):
-    """QMenuBar that is built from a list of model menu ids."""
+    """QMenuBar that is built from a list of model menu ids.
+
+    Parameters
+    ----------
+    menus : Mapping[str, str] | Sequence[str | tuple[str, str]]
+        A mapping of menu ids to menu titles or a sequence of menu ids.
+    app : Union[str, Application]
+        Application instance or name of application instance.
+    parent : Optional[QWidget]
+        Optional parent widget, by default None
+    """
 
     def __init__(
         self,
-        menus: List[str],
+        menus: Mapping[str, str] | Sequence[str | tuple[str, str]],
         app: Union[str, Application],
         parent: Optional[QWidget] = None,
     ) -> None:
         super().__init__(parent)
 
-        for menu_id in menus:
-            self.addMenu(QModelMenu(menu_id, app, "File", self))
+        menu_items = menus.items() if isinstance(menus, Mapping) else menus
+        for item in menu_items:
+            id_, title = item if isinstance(item, tuple) else (item, item.title())
+            self.addMenu(QModelMenu(id_, app, title, self))
 
     def update_from_context(
         self, ctx: Mapping[str, object], _recurse: bool = True
     ) -> None:
         """Update the enabled/visible state of each menu item with `ctx`.
 
         See `app_model.expressions` for details on expressions.
```

### Comparing `app_model-0.1.4/src/app_model/expressions/__init__.py` & `app_model-0.2.0rc1/src/app_model/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/expressions/_context.py` & `app_model-0.2.0rc1/src/app_model/expressions/_context.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/expressions/_context_keys.py` & `app_model-0.2.0rc1/src/app_model/expressions/_context_keys.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/expressions/_expressions.py` & `app_model-0.2.0rc1/src/app_model/expressions/_expressions.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,17 @@
     bound=Union[ast.cmpop, ast.operator, ast.boolop, ast.unaryop, ast.expr_context],
 )
 T = TypeVar("T")
 T2 = TypeVar("T2", bound=Union[ConstType, "Expr"])
 V = TypeVar("V", bound=ConstType)
 
 if TYPE_CHECKING:
+    from pydantic.annotated import GetCoreSchemaHandler
+    from pydantic_core import core_schema
+
     from ._context_keys import ContextKey
 
 
 def parse_expression(expr: Union[str, Expr]) -> Expr:
     """Parse string expression into an :class:`Expr` instance.
 
     Parameters
@@ -316,18 +319,26 @@
         rv = list(super().__reduce_ex__(protocol))
         rv[1] = tuple(getattr(self, f) for f in self._fields)
         return tuple(rv)
 
     @classmethod
     def __get_validators__(cls) -> Iterator[Callable[[Any], Expr]]:
         """Pydantic validators for this class."""
-        yield cls.validate
+        yield cls._validate
+
+    @classmethod
+    def __get_pydantic_core_schema__(
+        cls, source: type, handler: GetCoreSchemaHandler
+    ) -> core_schema.CoreSchema:
+        from pydantic_core import core_schema
+
+        return core_schema.no_info_plain_validator_function(cls._validate)
 
     @classmethod
-    def validate(cls, v: Any) -> Expr:
+    def _validate(cls, v: Any) -> Expr:
         """Validate v as an `Expr`. For use with Pydantic."""
         return v if isinstance(v, Expr) else parse_expression(v)
 
     def __hash__(self) -> int:
         _hash = hash(self.__class__)
         for f in self._fields:
             field = getattr(self, f)
```

### Comparing `app_model-0.1.4/src/app_model/registries/_commands_reg.py` & `app_model-0.2.0rc1/src/app_model/registries/_commands_reg.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/registries/_keybindings_reg.py` & `app_model-0.2.0rc1/src/app_model/registries/_keybindings_reg.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/registries/_menus_reg.py` & `app_model-0.2.0rc1/src/app_model/registries/_menus_reg.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         -------
         DisposeCallable
             A function that can be called to unregister the menu items.
         """
         changed_ids: Set[str] = set()
         disposers: List[Callable[[], None]] = []
         for menu_id, item in items:
-            item = MenuItem.validate(item)  # type: ignore
+            item = MenuItem._validate(item)  # type: ignore
             menu_dict = self._menu_items.setdefault(menu_id, {})
             menu_dict[item] = None
             changed_ids.add(menu_id)
 
             def _remove(dct: dict = menu_dict, _item: Any = item) -> None:
                 dct.pop(_item, None)
```

### Comparing `app_model-0.1.4/src/app_model/registries/_register.py` & `app_model-0.2.0rc1/src/app_model/registries/_register.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, TypeVar, overload
 
+from app_model._pydantic_compat import asdict
 from app_model.types import Action, MenuItem
 
 if TYPE_CHECKING:
     from typing import Any, Callable, List, Literal, Optional, Union
 
     from app_model import expressions
     from app_model._app import Application
@@ -219,15 +220,15 @@
         menu_item = MenuItem(command=action, when=action.enablement)
         disp = app.menus.append_menu_items([(app.menus.COMMAND_PALETTE_ID, menu_item)])
         disposers.append(disp)
 
     # keybinding
     for keyb in action.keybindings or ():
         if action.enablement is not None:
-            kwargs = keyb.dict()
+            kwargs = asdict(keyb)
             kwargs["when"] = (
                 action.enablement
                 if keyb.when is None
                 else action.enablement | keyb.when
             )
             _keyb = type(keyb)(**kwargs)
         else:
```

### Comparing `app_model-0.1.4/src/app_model/types/__init__.py` & `app_model-0.2.0rc1/src/app_model/types/__init__.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/types/_action.py` & `app_model-0.2.0rc1/src/app_model/types/_action.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Callable, Generic, List, Optional, TypeVar, Union
 
-from pydantic import Field, validator
+from pydantic import Field
+
+from app_model._pydantic_compat import validator
 
 from ._command_rule import CommandRule
 from ._keybinding_rule import KeyBindingRule
 from ._menu_rule import MenuRule
 from ._utils import _validate_python_name
 
 # maintain runtime compatibility with older typing_extensions
```

### Comparing `app_model-0.1.4/src/app_model/types/_command_rule.py` & `app_model-0.2.0rc1/src/app_model/types/_command_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,8 +71,8 @@
         None,
         description="(Optional) Condition under which the command should appear "
         "checked/toggled in any GUI representation (like a menu or button).",
     )
 
     def _as_command_rule(self) -> "CommandRule":
         """Simplify (subclasses) to a plain CommandRule."""
-        return CommandRule(**{f: getattr(self, f) for f in CommandRule.__fields__})
+        return CommandRule(**{f: getattr(self, f) for f in CommandRule.__annotations__})
```

### Comparing `app_model-0.1.4/src/app_model/types/_constants.py` & `app_model-0.2.0rc1/src/app_model/types/_constants.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/types/_icon.py` & `app_model-0.2.0rc1/src/app_model/types/_icon.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Any, Callable, Generator, Optional, TypedDict, Union
 
 from pydantic import Field
 
+from app_model._pydantic_compat import model_validator
+
 from ._base import _BaseModel
 
 
 class Icon(_BaseModel):
     """Icons used to represent commands, or submenus.
 
     May provide both a light and dark variant.  If only one is provided, it is used
@@ -21,26 +23,34 @@
         None,
         description="Icon path when a light theme is used. These may be superqt "
         "fonticon keys, such as `fa6s.arrow_down`",
     )
 
     @classmethod
     def __get_validators__(cls) -> Generator[Callable[..., Any], None, None]:
-        yield cls.validate
+        yield cls._validate
 
     @classmethod
-    def validate(cls, v: Any) -> "Icon":
+    def _validate(cls, v: Any) -> "Icon":
         """Validate icon."""
         # if a single string is passed, use it for both light and dark.
         if isinstance(v, Icon):
             return v
         if isinstance(v, str):
             v = {"dark": v, "light": v}
         return cls(**v)
 
+    # for v2
+    @model_validator(mode="wrap")
+    @classmethod
+    def _model_val(cls, v: Any, handler: Callable[[Any], "Icon"]) -> "Icon":
+        if isinstance(v, str):
+            v = {"dark": v, "light": v}
+        return handler(v)
+
 
 class IconDict(TypedDict):
     """Icon dictionary."""
 
     dark: Optional[str]
     light: Optional[str]
```

### Comparing `app_model-0.1.4/src/app_model/types/_keybinding_rule.py` & `app_model-0.2.0rc1/src/app_model/types/_keybinding_rule.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Any, Optional, TypedDict, Union
+from typing import Any, Callable, Optional, Type, TypedDict, TypeVar, Union
 
 from pydantic import Field
 
 from app_model import expressions
+from app_model._pydantic_compat import model_validator
 
 from ._base import _BaseModel
 from ._constants import OperatingSystem
 from ._keys import StandardKeyBinding
 
 KeyEncoding = Union[int, str]
+M = TypeVar("M")
 
 _OS = OperatingSystem.current()
 _WIN = _OS.is_windows
 _MAC = _OS.is_mac
 _LINUX = _OS.is_linux
 
 
@@ -61,14 +63,24 @@
     @classmethod
     def validate(cls, value: Any) -> "KeyBindingRule":
         """Validate keybinding rule."""
         if isinstance(value, StandardKeyBinding):
             return value.to_keybinding_rule()
         return super().validate(value)
 
+    # for v2
+    @model_validator(mode="wrap")
+    @classmethod
+    def _model_val(
+        cls: Type[M], v: Any, handler: Callable[[Any], M]
+    ) -> "KeyBindingRule":
+        if isinstance(v, StandardKeyBinding):
+            return v.to_keybinding_rule()
+        return handler(v)  # type: ignore
+
 
 class KeyBindingRuleDict(TypedDict, total=False):
     """Typed dict for KeyBindingRule kwargs."""
 
     primary: Optional[str]
     win: Optional[str]
     linux: Optional[str]
```

### Comparing `app_model-0.1.4/src/app_model/types/_menu_rule.py` & `app_model-0.2.0rc1/src/app_model/types/_menu_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,21 @@
-from typing import Any, Callable, Generator, Optional, Type, TypedDict, Union
+from typing import (
+    Any,
+    Callable,
+    Generator,
+    Optional,
+    Type,
+    TypedDict,
+    Union,
+)
 
-from pydantic import Field, validator
+from pydantic import Field
 
 from app_model import expressions
+from app_model._pydantic_compat import validator
 
 from ._base import _BaseModel
 from ._command_rule import CommandRule
 from ._icon import Icon
 
 
 class _MenuItemBase(_BaseModel):
@@ -28,29 +37,29 @@
         description="(Optional) Order of the item *within* its group. Note, order is "
         "not part of the plugin schema, plugins may provide it using the group key "
         "and the syntax 'group@order'.  If not provided, items are sorted by title.",
     )
 
     @classmethod
     def __get_validators__(cls) -> Generator[Callable[..., Any], None, None]:
-        yield cls.validate
+        yield cls._validate
 
     @classmethod
-    def validate(cls: Type["_MenuItemBase"], v: Any) -> "_MenuItemBase":
+    def _validate(cls: Type["_MenuItemBase"], v: Any) -> "_MenuItemBase":
         """Validate icon."""
         if isinstance(v, _MenuItemBase):
             return v
         if isinstance(v, dict):
             if "command" in v:
                 return MenuItem(**v)
             if "id" in v:
                 return MenuRule(**v)
             if "submenu" in v:
                 return SubmenuItem(**v)
-        raise TypeError(f"Invalid menu item: {v!r}", cls)  # pragma: no cover
+        raise ValueError(f"Invalid menu item: {v!r}", cls)  # pragma: no cover
 
 
 class MenuRule(_MenuItemBase):
     """A MenuRule defines a menu location and conditions for presentation.
 
     It does not define an actual command. That is done in either `MenuItem` or `Action`.
     """
```

### Comparing `app_model-0.1.4/src/app_model/types/_utils.py` & `app_model-0.2.0rc1/src/app_model/types/_utils.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/src/app_model/types/_keys/_key_codes.py` & `app_model-0.2.0rc1/src/app_model/types/_keys/_key_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from enum import IntEnum, IntFlag, auto
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Generator,
     NamedTuple,
     Set,
     Tuple,
     Type,
     Union,
     overload,
 )
 
+if TYPE_CHECKING:
+    from pydantic.annotated import GetCoreSchemaHandler
+    from pydantic_core import core_schema
+
 __all__ = ["KeyCode", "KeyMod", "ScanCode", "KeyChord"]
 
 # TODO:
 # https://stackoverflow.com/questions/3202629/where-can-i-find-a-list-of-mac-virtual-key-codes/16125341#16125341
 
 # flake8: noqa
 # fmt: off
@@ -164,14 +169,22 @@
         return _EVENTCODE_TO_KEYCODE.get(event_code, KeyCode.UNKNOWN)
 
     @classmethod
     def __get_validators__(cls) -> Generator[Callable[..., 'KeyCode'], None, None]:
         yield cls.validate
 
     @classmethod
+    def __get_pydantic_core_schema__(
+        cls, source: type, handler: 'GetCoreSchemaHandler'
+    ) -> 'core_schema.CoreSchema':
+        from pydantic_core import core_schema
+
+        return core_schema.no_info_plain_validator_function(cls.validate)
+
+    @classmethod
     def validate(cls, value: Any) -> 'KeyCode':
         if isinstance(value, KeyCode):
             return value
         if isinstance(value, int):
             return cls(value)
         if isinstance(value, str):
             return cls.from_string(value)
```

### Comparing `app_model-0.1.4/src/app_model/types/_keys/_keybindings.py` & `app_model-0.2.0rc1/src/app_model/types/_keys/_keybindings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import re
-from typing import Any, Callable, Dict, Generator, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Callable, Dict, Generator, List, Optional, Tuple
 
 from pydantic import BaseModel, Field
 
+from app_model._pydantic_compat import PYDANTIC2, model_validator
 from app_model.types._constants import OperatingSystem
 
 from ._key_codes import KeyChord, KeyCode, KeyMod
 
+if TYPE_CHECKING:
+    from pydantic.annotated import GetCoreSchemaHandler
+    from pydantic_core import core_schema
+
 _re_ctrl = re.compile(r"ctrl[\+|\-]")
 _re_shift = re.compile(r"shift[\+|\-]")
 _re_alt = re.compile(r"alt[\+|\-]")
 _re_meta = re.compile(r"meta[\+|\-]")
 _re_win = re.compile(r"win[\+|\-]")
 _re_cmd = re.compile(r"cmd[\+|\-]")
 
@@ -51,16 +56,17 @@
             out += str(self.key)
         return out
 
     def __eq__(self, other: Any) -> bool:
         # sourcery skip: remove-unnecessary-cast
         if not isinstance(other, SimpleKeyBinding):
             try:
-                other = SimpleKeyBinding.validate(other)
-            except TypeError:
+                if (other := SimpleKeyBinding._parse_input(other)) is None:
+                    return NotImplemented
+            except TypeError:  # pragma: no cover  # can happen with pydantic v2
                 return NotImplemented
         return bool(
             self.ctrl == other.ctrl
             and self.shift == other.shift
             and self.alt == other.alt
             and self.meta == other.meta
             and self.key == other.key
@@ -107,27 +113,41 @@
         if self.alt:
             mods |= KeyMod.Alt
         if self.meta:
             mods |= KeyMod.CtrlCmd if os.is_mac else KeyMod.WinCtrl
         return mods | (self.key or 0)
 
     @classmethod
-    def __get_validators__(cls) -> Generator[Callable[..., Any], None, None]:
-        yield cls.validate  # pragma: no cover
-
-    @classmethod
-    def validate(cls, v: Any) -> "SimpleKeyBinding":
-        """Validate a SimpleKeyBinding."""
+    def _parse_input(cls, v: Any) -> Optional["SimpleKeyBinding"]:
         if isinstance(v, SimpleKeyBinding):
             return v
         if isinstance(v, str):
             return cls.from_str(v)
         if isinstance(v, int):
             return cls.from_int(v)
-        return super().validate(v)
+        return None
+
+    @classmethod
+    def __get_validators__(cls) -> Generator[Callable[..., Any], None, None]:
+        yield cls._validate  # pragma: no cover
+
+    @classmethod
+    def _validate(cls, input: Any) -> "SimpleKeyBinding":
+        return cls._parse_input(input) or cls(**input)  # pragma: no cover
+
+    # for v2
+    @model_validator(mode="wrap")
+    @classmethod
+    def _model_val(
+        cls, input: Any, handler: Callable[[Any], "SimpleKeyBinding"]
+    ) -> "SimpleKeyBinding":
+        return cls._parse_input(input) or handler(input)
+
+
+MIN1 = {"min_length": 1} if PYDANTIC2 else {"min_items": 1}
 
 
 class KeyBinding:
     """KeyBinding.  May be a multi-part "Chord" (e.g. 'Ctrl+K Ctrl+C').
 
     This is the primary representation of a fully resolved keybinding. For consistency
     in the downstream API, it should  be preferred to :class:`SimplyKeyBinding`, even
@@ -136,15 +156,15 @@
     Chords (two separate keypress actions) are expressed as a string by separating
     the two keypress codes with a space. For example, 'Ctrl+K Ctrl+C'.
     """
 
     def __init__(self, *, parts: List[SimpleKeyBinding]):
         self.parts = parts
 
-    parts: List[SimpleKeyBinding] = Field(..., min_items=1)
+    parts: List[SimpleKeyBinding] = Field(..., **MIN1)  # type: ignore
 
     def __str__(self) -> str:
         return " ".join(str(part) for part in self.parts)
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, KeyBinding):
             try:
@@ -208,14 +228,24 @@
         return hash(tuple(self.parts))
 
     @classmethod
     def __get_validators__(cls) -> Generator[Callable[..., Any], None, None]:
         yield cls.validate  # pragma: no cover
 
     @classmethod
+    def __get_pydantic_core_schema__(
+        cls, source: type, handler: "GetCoreSchemaHandler"
+    ) -> "core_schema.CoreSchema":
+        from pydantic_core import core_schema
+
+        return core_schema.no_info_plain_validator_function(
+            cls.validate, serialization=core_schema.to_string_ser_schema()
+        )
+
+    @classmethod
     def validate(cls, v: Any) -> "KeyBinding":
         """Validate a SimpleKeyBinding."""
         if isinstance(v, KeyBinding):
             return v
         if isinstance(v, SimpleKeyBinding):
             return cls(parts=[v])
         if isinstance(v, int):
```

### Comparing `app_model-0.1.4/src/app_model/types/_keys/_standard_bindings.py` & `app_model-0.2.0rc1/src/app_model/types/_keys/_standard_bindings.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/tests/conftest.py` & `app_model-0.2.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/tests/test_actions.py` & `app_model-0.2.0rc1/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/tests/test_app.py` & `app_model-0.2.0rc1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/tests/test_command_registry.py` & `app_model-0.2.0rc1/tests/test_command_registry.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/tests/test_key_codes.py` & `app_model-0.2.0rc1/tests/test_key_codes.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/tests/test_keybindings.py` & `app_model-0.2.0rc1/tests/test_keybindings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 
 import pytest
 from pydantic import BaseModel
 
+from app_model._pydantic_compat import PYDANTIC2, asjson
 from app_model.types import (
     KeyBinding,
     KeyBindingRule,
     KeyCode,
     KeyMod,
     SimpleKeyBinding,
 )
@@ -21,24 +22,24 @@
     _mod = f"{mod}+" if mod else ""
     kb = SimpleKeyBinding.from_str(f"{_mod}{key}")
     assert str(kb).lower() == f"{_mod}{key}".lower()
     assert not kb.is_modifier_key()
 
     # we can compare it with another SimpleKeyBinding
     # using validate method just for test coverage... will pass to from_str
-    assert kb == SimpleKeyBinding.validate(f"{_mod}{key}")
+    assert kb == SimpleKeyBinding._parse_input(f"{_mod}{key}")
     # or with a string
     assert kb == f"{_mod}{key}"
     assert kb != ["A", "B"]  # check type error during comparison
 
     # round trip to int
     assert isinstance(kb.to_int(), KeyCombo)
     # using validate method just for test coverage... will pass to from_int
-    assert SimpleKeyBinding.validate(int(kb)) == kb
-    assert SimpleKeyBinding.validate(kb) == kb
+    assert SimpleKeyBinding._parse_input(int(kb)) == kb
+    assert SimpleKeyBinding._parse_input(kb) == kb
 
     # first part of a Keybinding is a simple keybinding
     as_full_kb = KeyBinding.validate(kb)
     assert as_full_kb.part0 == kb
     assert KeyBinding.validate(int(kb)).part0 == kb
 
     assert int(as_full_kb) == int(kb)
@@ -98,19 +99,22 @@
         kbs[new_a]
 
 
 def test_in_model():
     class M(BaseModel):
         key: KeyBinding
 
-        class Config:
-            json_encoders = {KeyBinding: str}
+        if not PYDANTIC2:
+
+            class Config:
+                json_encoders = {KeyBinding: str}
 
     m = M(key="Shift+A B")
-    assert m.json() == '{"key": "Shift+A B"}'
+    # pydantic v1 and v2 have slightly different json outputs
+    assert asjson(m).replace('": "', '":"') == '{"key":"Shift+A B"}'
 
 
 def test_standard_keybindings():
     class M(BaseModel):
         key: KeyBindingRule
 
     m = M(key=StandardKeyBinding.Copy)
```

### Comparing `app_model-0.1.4/tests/test_registries.py` & `app_model-0.2.0rc1/tests/test_registries.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/tests/test_types.py` & `app_model-0.2.0rc1/tests/test_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from pydantic import ValidationError
 
 from app_model.types import Action, Icon
 
 
 def test_icon_validate():
-    assert Icon.validate('"fa6s.arrow_down"') == Icon(
+    assert Icon._validate('"fa6s.arrow_down"') == Icon(
         dark='"fa6s.arrow_down"', light='"fa6s.arrow_down"'
     )
 
 
 def test_action_validation():
     with pytest.raises(ValidationError, match="'s!adf' is not a valid python_name"):
         Action(id="test", title="test", callback="s!adf")
```

### Comparing `app_model-0.1.4/tests/test_context/test_context.py` & `app_model-0.2.0rc1/tests/test_context/test_context.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/tests/test_context/test_context_keys.py` & `app_model-0.2.0rc1/tests/test_context/test_context_keys.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/tests/test_context/test_expressions.py` & `app_model-0.2.0rc1/tests/test_context/test_expressions.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/tests/test_qt/test_qactions.py` & `app_model-0.2.0rc1/tests/test_qt/test_qactions.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/tests/test_qt/test_qkeymap.py` & `app_model-0.2.0rc1/tests/test_qt/test_qkeymap.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/tests/test_qt/test_qmenu.py` & `app_model-0.2.0rc1/tests/test_qt/test_qmenu.py`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/.gitignore` & `app_model-0.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/LICENSE` & `app_model-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/README.md` & `app_model-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `app_model-0.1.4/pyproject.toml` & `app_model-0.2.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Topic :: Desktop Environment",
     "Topic :: Software Development",
     "Topic :: Software Development :: User Interfaces",
 ]
 dynamic = ["version"]
 dependencies = [
     "psygnal>=0.3.4",
-    "pydantic>=1.8,<2",
+    "pydantic>=1.8",
     "in-n-out>=0.1.5",
     "typing_extensions",
 ]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
```

### Comparing `app_model-0.1.4/PKG-INFO` & `app_model-0.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-model
-Version: 0.1.4
+Version: 0.2.0rc1
 Summary: Generic application schema implemented in python
 Project-URL: homepage, https://github.com/pyapp-kit/app-model
 Project-URL: repository, https://github.com/pyapp-kit/app-model
 Author: Talley Lambert
 Author-email: talley.lambert@gmail.com
 License: BSD 3-Clause License
 License-File: LICENSE
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Desktop Environment
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.8
 Requires-Dist: in-n-out>=0.1.5
 Requires-Dist: psygnal>=0.3.4
-Requires-Dist: pydantic<2,>=1.8
+Requires-Dist: pydantic>=1.8
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
```

