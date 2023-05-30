# Comparing `tmp/plumbum-1.8.1.tar.gz` & `tmp/plumbum-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Tue May 30 10:30:45 2023, max compression
```

## Comparing `plumbum-1.8.1.tar` & `plumbum-1.8.2.tar`

### file list

```diff
@@ -1,147 +1,148 @@
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 plumbum-1.8.1/.editorconfig
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 plumbum-1.8.1/.gitattributes
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 plumbum-1.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 plumbum-1.8.1/.readthedocs.yml
--rw-r--r--   0        0        0    21544 2020-02-02 00:00:00.000000 plumbum-1.8.1/CHANGELOG.rst
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 plumbum-1.8.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 plumbum-1.8.1/MANIFEST.in
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 plumbum-1.8.1/noxfile.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 plumbum-1.8.1/setup.cfg
--rwxr-xr-x   0        0        0     1066 2020-02-02 00:00:00.000000 plumbum-1.8.1/translations.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 plumbum-1.8.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 plumbum-1.8.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 plumbum-1.8.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 plumbum-1.8.1/conda.recipe/.gitignore
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 plumbum-1.8.1/conda.recipe/README.mkd
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 plumbum-1.8.1/conda.recipe/bld.bat
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 plumbum-1.8.1/conda.recipe/build.sh
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 plumbum-1.8.1/conda.recipe/meta.yaml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/.gitignore
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/Makefile
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_cheatsheet.rst
--rw-r--r--   0        0        0    22722 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_color_list.html
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_news.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/changelog.rst
--rw-r--r--   0        0        0    25760 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/cli.rst
--rw-r--r--   0        0        0    13654 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/colorlib.rst
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/colors.rst
--rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/conf.py
--rw-r--r--   0        0        0     7925 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/index.rst
--rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/local_commands.rst
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/local_machine.rst
--rw-r--r--   0        0        0     5130 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/make.bat
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/paths.rst
--rw-r--r--   0        0        0     9886 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/quickref.rst
--rw-r--r--   0        0        0    10216 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/remote.rst
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/typed_env.rst
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/utils.rst
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_static/fish-text-black.png
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_static/github-logo.png
--rw-r--r--   0        0        0     9085 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_static/logo.png
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_static/logo2.png
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_static/logo3.png
--rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_static/logo4.png
--rw-r--r--   0        0        0    74592 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_static/logo6.png
--rw-r--r--   0        0        0     9700 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_static/logo7.png
--rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_static/logo8.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_static/placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/_templates/placeholder
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/api/cli.rst
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/api/colors.rst
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/api/commands.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/api/fs.rst
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/api/machines.rst
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 plumbum-1.8.1/docs/api/path.rst
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 plumbum-1.8.1/examples/.gitignore
--rw-r--r--   0        0        0    16244 2020-02-02 00:00:00.000000 plumbum-1.8.1/examples/PHSP.png
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 plumbum-1.8.1/examples/SimpleColorCLI.py
--rwxr-xr-x   0        0        0      358 2020-02-02 00:00:00.000000 plumbum-1.8.1/examples/alignment.py
--rwxr-xr-x   0        0        0      704 2020-02-02 00:00:00.000000 plumbum-1.8.1/examples/color.py
--rwxr-xr-x   0        0        0     1086 2020-02-02 00:00:00.000000 plumbum-1.8.1/examples/filecopy.py
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 plumbum-1.8.1/examples/fullcolor.py
--rwxr-xr-x   0        0        0     3363 2020-02-02 00:00:00.000000 plumbum-1.8.1/examples/geet.py
--rwxr-xr-x   0        0        0      768 2020-02-02 00:00:00.000000 plumbum-1.8.1/examples/make_figures.py
--rwxr-xr-x   0        0        0     1585 2020-02-02 00:00:00.000000 plumbum-1.8.1/examples/simple_cli.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 plumbum-1.8.1/examples/testfigure.tex
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 plumbum-1.8.1/experiments/parallel.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 plumbum-1.8.1/experiments/test_parallel.py
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/__init__.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/_testtools.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cmd.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/colors.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/lib.py
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/typed_env.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/version.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/__init__.py
--rw-r--r--   0        0        0    38056 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/application.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/config.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/i18n.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/image.py
--rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/progress.py
--rw-r--r--   0        0        0    21071 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/switches.py
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/terminal.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/termsize.py
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/i18n/de.po
--rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/i18n/fr.po
--rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/i18n/nl.po
--rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/i18n/ru.po
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/i18n/de/LC_MESSAGES/plumbum.cli.mo
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/i18n/fr/LC_MESSAGES/plumbum.cli.mo
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/i18n/nl/LC_MESSAGES/plumbum.cli.mo
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/cli/i18n/ru/LC_MESSAGES/plumbum.cli.mo
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/colorlib/__init__.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/colorlib/__main__.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/colorlib/_ipython_ext.py
--rw-r--r--   0        0        0     6927 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/colorlib/factories.py
--rw-r--r--   0        0        0     8229 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/colorlib/names.py
--rw-r--r--   0        0        0    25049 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/colorlib/styles.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/commands/__init__.py
--rw-r--r--   0        0        0    19591 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/commands/base.py
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/commands/daemons.py
--rw-r--r--   0        0        0    17023 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/commands/modifiers.py
--rw-r--r--   0        0        0    13989 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/commands/processes.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/fs/__init__.py
--rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/fs/atomic.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/fs/mounts.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/machines/__init__.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/machines/_windows.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/machines/base.py
--rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/machines/env.py
--rw-r--r--   0        0        0    15783 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/machines/local.py
--rw-r--r--   0        0        0    17609 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/machines/paramiko_machine.py
--rw-r--r--   0        0        0    15952 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/machines/remote.py
--rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/machines/session.py
--rw-r--r--   0        0        0    15168 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/machines/ssh_machine.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/path/__init__.py
--rw-r--r--   0        0        0    16482 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/path/base.py
--rw-r--r--   0        0        0    10683 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/path/local.py
--rw-r--r--   0        0        0    11330 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/path/remote.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 plumbum-1.8.1/plumbum/path/utils.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/_test_paramiko.py
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/conftest.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/env.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/file with space.txt
--rwxr-xr-x   0        0        0      145 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/slow_process.bash
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_3_cli.py
--rw-r--r--   0        0        0    11574 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_cli.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_clicolor.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_color.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_config.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_env.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_factories.py
--rw-r--r--   0        0        0    35681 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_local.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_nohup.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_putty.py
--rw-r--r--   0        0        0    23851 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_remote.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_sudo.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_terminal.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_typed_env.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_utils.py
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_validate.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/test_visual_color.py
--rwxr-xr-x   0        0        0       10 2020-02-02 00:00:00.000000 plumbum-1.8.1/tests/not-in-path/dummy-executable
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 plumbum-1.8.1/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 plumbum-1.8.1/LICENSE
--rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 plumbum-1.8.1/README.rst
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 plumbum-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 plumbum-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0      118 2023-05-30 10:30:45.000000 plumbum-1.8.2/.editorconfig
+-rw-r--r--   0        0        0       35 2023-05-30 10:30:45.000000 plumbum-1.8.2/.gitattributes
+-rw-r--r--   0        0        0     1289 2023-05-30 10:30:45.000000 plumbum-1.8.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      384 2023-05-30 10:30:45.000000 plumbum-1.8.2/.readthedocs.yml
+-rw-r--r--   0        0        0    21952 2023-05-30 10:30:45.000000 plumbum-1.8.2/CHANGELOG.rst
+-rw-r--r--   0        0        0      835 2023-05-30 10:30:45.000000 plumbum-1.8.2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      216 2023-05-30 10:30:45.000000 plumbum-1.8.2/MANIFEST.in
+-rw-r--r--   0        0        0     1436 2023-05-30 10:30:45.000000 plumbum-1.8.2/noxfile.py
+-rw-r--r--   0        0        0      570 2023-05-30 10:30:45.000000 plumbum-1.8.2/setup.cfg
+-rwxr-xr-x   0        0        0     1066 2023-05-30 10:30:45.000000 plumbum-1.8.2/translations.py
+-rw-r--r--   0        0        0      162 2023-05-30 10:30:45.000000 plumbum-1.8.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-05-30 10:30:45.000000 plumbum-1.8.2/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      654 2023-05-30 10:30:45.000000 plumbum-1.8.2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2980 2023-05-30 10:30:45.000000 plumbum-1.8.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       67 2023-05-30 10:30:45.000000 plumbum-1.8.2/conda.recipe/.gitignore
+-rw-r--r--   0        0        0      819 2023-05-30 10:30:45.000000 plumbum-1.8.2/conda.recipe/README.mkd
+-rw-r--r--   0        0        0       51 2023-05-30 10:30:45.000000 plumbum-1.8.2/conda.recipe/bld.bat
+-rw-r--r--   0        0        0       38 2023-05-30 10:30:45.000000 plumbum-1.8.2/conda.recipe/build.sh
+-rw-r--r--   0        0        0      904 2023-05-30 10:30:45.000000 plumbum-1.8.2/conda.recipe/meta.yaml
+-rw-r--r--   0        0        0        8 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/.gitignore
+-rw-r--r--   0        0        0     5632 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/Makefile
+-rw-r--r--   0        0        0     5752 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_cheatsheet.rst
+-rw-r--r--   0        0        0    22722 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_color_list.html
+-rw-r--r--   0        0        0     2762 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_news.rst
+-rw-r--r--   0        0        0       53 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/changelog.rst
+-rw-r--r--   0        0        0    25762 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/cli.rst
+-rw-r--r--   0        0        0    13654 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/colorlib.rst
+-rw-r--r--   0        0        0    11770 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/colors.rst
+-rw-r--r--   0        0        0     8380 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/conf.py
+-rw-r--r--   0        0        0     8041 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/index.rst
+-rw-r--r--   0        0        0    13579 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/local_commands.rst
+-rw-r--r--   0        0        0     4161 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/local_machine.rst
+-rw-r--r--   0        0        0     5130 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/make.bat
+-rw-r--r--   0        0        0     4211 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/paths.rst
+-rw-r--r--   0        0        0     9886 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/quickref.rst
+-rw-r--r--   0        0        0    10216 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/remote.rst
+-rw-r--r--   0        0        0     2956 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/typed_env.rst
+-rw-r--r--   0        0        0     1728 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/utils.rst
+-rw-r--r--   0        0        0     2311 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/fish-text-black.png
+-rw-r--r--   0        0        0     2820 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/github-logo.png
+-rw-r--r--   0        0        0     9085 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo.png
+-rw-r--r--   0        0        0     3413 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo2.png
+-rw-r--r--   0        0        0     4527 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo3.png
+-rw-r--r--   0        0        0     4147 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo4.png
+-rw-r--r--   0        0        0    74592 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo6.png
+-rw-r--r--   0        0        0     9700 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo7.png
+-rw-r--r--   0        0        0     8599 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo8.png
+-rw-r--r--   0        0        0        0 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/placeholder
+-rw-r--r--   0        0        0        0 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_templates/placeholder
+-rw-r--r--   0        0        0      311 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/api/cli.rst
+-rw-r--r--   0        0        0      593 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/api/colors.rst
+-rw-r--r--   0        0        0      373 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/api/commands.rst
+-rw-r--r--   0        0        0      156 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/api/fs.rst
+-rw-r--r--   0        0        0      595 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/api/machines.rst
+-rw-r--r--   0        0        0      348 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/api/path.rst
+-rw-r--r--   0        0        0       75 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/.gitignore
+-rw-r--r--   0        0        0    16244 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/PHSP.png
+-rw-r--r--   0        0        0      504 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/SimpleColorCLI.py
+-rwxr-xr-x   0        0        0      358 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/alignment.py
+-rwxr-xr-x   0        0        0      704 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/color.py
+-rwxr-xr-x   0        0        0     1064 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/filecopy.py
+-rwxr-xr-x   0        0        0      270 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/fullcolor.py
+-rwxr-xr-x   0        0        0     3363 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/geet.py
+-rwxr-xr-x   0        0        0      768 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/make_figures.py
+-rwxr-xr-x   0        0        0     1585 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/simple_cli.py
+-rw-r--r--   0        0        0      330 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/testfigure.tex
+-rw-r--r--   0        0        0     5643 2023-05-30 10:30:45.000000 plumbum-1.8.2/experiments/parallel.py
+-rw-r--r--   0        0        0     1257 2023-05-30 10:30:45.000000 plumbum-1.8.2/experiments/test_parallel.py
+-rw-r--r--   0        0        0     3255 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/__init__.py
+-rw-r--r--   0        0        0      651 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/_testtools.py
+-rw-r--r--   0        0        0      292 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cmd.py
+-rw-r--r--   0        0        0      567 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colors.py
+-rw-r--r--   0        0        0     2036 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/lib.py
+-rw-r--r--   0        0        0     4935 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/typed_env.py
+-rw-r--r--   0        0        0      160 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/version.py
+-rw-r--r--   0        0        0      606 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/__init__.py
+-rw-r--r--   0        0        0    38071 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/application.py
+-rw-r--r--   0        0        0     3200 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/config.py
+-rw-r--r--   0        0        0     1647 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n.py
+-rw-r--r--   0        0        0     3346 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/image.py
+-rw-r--r--   0        0        0     8348 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/progress.py
+-rw-r--r--   0        0        0    21058 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/switches.py
+-rw-r--r--   0        0        0     7223 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/terminal.py
+-rw-r--r--   0        0        0     3109 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/termsize.py
+-rw-r--r--   0        0        0     6754 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/de.po
+-rw-r--r--   0        0        0     6734 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/fr.po
+-rw-r--r--   0        0        0     6727 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/nl.po
+-rw-r--r--   0        0        0     8070 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/ru.po
+-rw-r--r--   0        0        0     3553 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/de/LC_MESSAGES/plumbum.cli.mo
+-rw-r--r--   0        0        0     3514 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/fr/LC_MESSAGES/plumbum.cli.mo
+-rw-r--r--   0        0        0     3510 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/nl/LC_MESSAGES/plumbum.cli.mo
+-rw-r--r--   0        0        0     4836 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/ru/LC_MESSAGES/plumbum.cli.mo
+-rw-r--r--   0        0        0     1211 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colorlib/__init__.py
+-rw-r--r--   0        0        0      165 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colorlib/__main__.py
+-rw-r--r--   0        0        0      979 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colorlib/_ipython_ext.py
+-rw-r--r--   0        0        0     6927 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colorlib/factories.py
+-rw-r--r--   0        0        0     8260 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colorlib/names.py
+-rw-r--r--   0        0        0    25047 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colorlib/styles.py
+-rw-r--r--   0        0        0      773 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/commands/__init__.py
+-rw-r--r--   0        0        0    19546 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/commands/base.py
+-rw-r--r--   0        0        0     3543 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/commands/daemons.py
+-rw-r--r--   0        0        0    17042 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/commands/modifiers.py
+-rw-r--r--   0        0        0    13895 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/commands/processes.py
+-rw-r--r--   0        0        0       39 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/fs/__init__.py
+-rw-r--r--   0        0        0     9425 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/fs/atomic.py
+-rw-r--r--   0        0        0     1097 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/fs/mounts.py
+-rw-r--r--   0        0        0      356 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/_windows.py
+-rw-r--r--   0        0        0     3397 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/base.py
+-rw-r--r--   0        0        0     6327 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/env.py
+-rw-r--r--   0        0        0    15778 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/local.py
+-rw-r--r--   0        0        0    17619 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/paramiko_machine.py
+-rw-r--r--   0        0        0    15941 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/remote.py
+-rw-r--r--   0        0        0    11809 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/session.py
+-rw-r--r--   0        0        0    15149 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/ssh_machine.py
+-rw-r--r--   0        0        0      395 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/path/__init__.py
+-rw-r--r--   0        0        0    17362 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/path/base.py
+-rw-r--r--   0        0        0    10610 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/path/local.py
+-rw-r--r--   0        0        0    11309 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/path/remote.py
+-rw-r--r--   0        0        0     3532 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/path/utils.py
+-rw-r--r--   0        0        0      307 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/_test_paramiko.py
+-rw-r--r--   0        0        0     4145 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/conftest.py
+-rw-r--r--   0        0        0      368 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/env.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/file with space.txt
+-rwxr-xr-x   0        0        0      145 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/slow_process.bash
+-rw-r--r--   0        0        0      736 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_3_cli.py
+-rw-r--r--   0        0        0    11564 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_cli.py
+-rw-r--r--   0        0        0     2788 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_clicolor.py
+-rw-r--r--   0        0        0     2815 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_color.py
+-rw-r--r--   0        0        0     2013 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_config.py
+-rw-r--r--   0        0        0     2103 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_env.py
+-rw-r--r--   0        0        0     6354 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_factories.py
+-rw-r--r--   0        0        0    35677 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_local.py
+-rw-r--r--   0        0        0     2199 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_nohup.py
+-rw-r--r--   0        0        0     1938 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_putty.py
+-rw-r--r--   0        0        0    23757 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_remote.py
+-rw-r--r--   0        0        0      394 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_sudo.py
+-rw-r--r--   0        0        0     5266 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_terminal.py
+-rw-r--r--   0        0        0     1544 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_typed_env.py
+-rw-r--r--   0        0        0     1706 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_utils.py
+-rw-r--r--   0        0        0     2630 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_validate.py
+-rw-r--r--   0        0        0     2287 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_visual_color.py
+-rwxr-xr-x   0        0        0       10 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/not-in-path/dummy-executable
+-rw-r--r--   0        0        0     3191 2023-05-30 10:30:45.000000 plumbum-1.8.2/.gitignore
+-rw-r--r--   0        0        0     1080 2023-05-30 10:30:45.000000 plumbum-1.8.2/LICENSE
+-rw-r--r--   0        0        0     6920 2023-05-30 10:30:45.000000 plumbum-1.8.2/README.rst
+-rw-r--r--   0        0        0     5707 2023-05-30 10:30:45.000000 plumbum-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0    10132 2023-05-30 10:30:45.000000 plumbum-1.8.2/PKG-INFO
```

### Comparing `plumbum-1.8.1/.pre-commit-config.yaml` & `plumbum-1.8.2/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,56 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.3.0
+  rev: "v4.4.0"
   hooks:
   - id: check-added-large-files
   - id: check-case-conflict
   - id: check-merge-conflict
   - id: check-symlinks
   - id: check-yaml
     exclude: ^conda.recipe/meta.yaml$
   - id: debug-statements
   - id: end-of-file-fixer
   - id: mixed-line-ending
   - id: requirements-txt-fixer
   - id: trailing-whitespace
 
 - repo: https://github.com/psf/black
-  rev: "22.8.0"
+  rev: "23.3.0"
   hooks:
   - id: black
 
-- repo: https://github.com/PyCQA/isort
-  rev: "5.10.1"
+- repo: https://github.com/charliermarsh/ruff-pre-commit
+  rev: "v0.0.270"
   hooks:
-  - id: isort
-
-- repo: https://github.com/asottile/pyupgrade
-  rev: "v2.38.2"
-  hooks:
-  - id: pyupgrade
-    args: ["--py36-plus"]
-
-- repo: https://github.com/hadialqattan/pycln
-  rev: v2.1.1
-  hooks:
-  - id: pycln
-    args: [--all]
-    stages: [manual]
-
-- repo: https://github.com/pycqa/flake8
-  rev: "5.0.4"
-  hooks:
-  - id: flake8
-    exclude: docs/conf.py
-    additional_dependencies: [flake8-bugbear, flake8-print, flake8-2020]
+    - id: ruff
+      args: ["--fix", "--show-fixes"]
 
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: "v0.981"
+  rev: "v1.3.0"
   hooks:
   - id: mypy
     files: plumbum
     args: []
     additional_dependencies: [typed-ast, types-paramiko, types-setuptools]
 
+- repo: https://github.com/abravalheri/validate-pyproject
+  rev: "v0.13"
+  hooks:
+  - id: validate-pyproject
+
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.1
+  rev: "v2.2.4"
   hooks:
   - id: codespell
 
 - repo: https://github.com/pre-commit/pygrep-hooks
-  rev: "v1.9.0"
+  rev: "v1.10.0"
   hooks:
-  - id: python-check-blanket-noqa
-  - id: python-check-blanket-type-ignore
-  - id: python-no-log-warn
-  - id: python-use-type-annotations
   - id: rst-backticks
   - id: rst-directive-colons
   - id: rst-inline-touching-normal
```

### Comparing `plumbum-1.8.1/CHANGELOG.rst` & `plumbum-1.8.2/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+1.8.2
+-----
+
+* Fix author metadata on PyPI package and add static check (`#648 <https://github.com/tomerfiliba/plumbum/pull/648>`_)
+* Add testing for Python 3.12 beta 1 (`#650 <https://github.com/tomerfiliba/plumbum/pull/650>`_)
+* Use Ruff for linting (`#643 <https://github.com/tomerfiliba/plumbum/pull/643>`_)
+* Paths: Add type hinting for Path (`#646 <https://github.com/tomerfiliba/plumbum/pull/646>`_)
+
 1.8.1
 -----
 
 * Accept path-like objects (`#627 <https://github.com/tomerfiliba/plumbum/pull/627>`_)
 * Move the build backend to hatchling and hatch-vcs. Users should be unaffected. Third-party packaging may need to adapt to the new build system. (`#607 <https://github.com/tomerfiliba/plumbum/pull/607>`_)
 
 1.8.0
```

### Comparing `plumbum-1.8.1/CONTRIBUTING.rst` & `plumbum-1.8.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/noxfile.py` & `plumbum-1.8.2/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import nox
 
-ALL_PYTHONS = ["3.6", "3.7", "3.8", "3.9", "3.10", "3.11"]
+ALL_PYTHONS = ["3.6", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
 
 nox.options.sessions = ["lint", "tests"]
 
 
 @nox.session(reuse_venv=True)
 def lint(session):
     """
@@ -18,15 +18,15 @@
 
 @nox.session
 def pylint(session):
     """
     Run pylint.
     """
 
-    session.install(".", "paramiko", "ipython", "pylint~=2.15.7")
+    session.install(".", "paramiko", "ipython", "pylint~=2.17.4")
     session.run("pylint", "plumbum", *session.posargs)
 
 
 @nox.session(python=ALL_PYTHONS, reuse_venv=True)
 def tests(session):
     """
     Run the unit and regular tests.
```

### Comparing `plumbum-1.8.1/setup.cfg` & `plumbum-1.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/translations.py` & `plumbum-1.8.2/translations.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/.github/matchers/pylint.json` & `plumbum-1.8.2/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/.github/workflows/ci.yml` & `plumbum-1.8.2/.github/workflows/ci.yml`

 * *Files 24% similar despite different names*

```diff
@@ -6,17 +6,14 @@
     branches:
     - master
     - main
   pull_request:
     branches:
     - master
     - main
-  release:
-    types:
-    - published
 
 env:
   FORCE_COLOR: 3
 
 jobs:
 
   pre-commit:
@@ -36,18 +33,18 @@
         pipx run --python python nox -s pylint
 
   tests:
     name: Tests on 🐍 ${{ matrix.python-version }} ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.6", "3.8", "3.11"]
+        python-version: ["3.6", "3.8", "3.11", "3.12-dev"]
         os: [ubuntu-latest, windows-latest, macos-latest]
         include:
-        - python-version: 'pypy-3.7'
+        - python-version: 'pypy-3.8'
           os: ubuntu-latest
         - python-version: 'pypy-3.9'
           os: ubuntu-latest
         - python-version: '3.6'
           os: ubuntu-20.04
         exclude:
         - python-version: '3.6'
@@ -97,40 +94,14 @@
     - name: Upload coverage
       run: coveralls --service=github
       env:
         COVERALLS_PARALLEL: true
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         COVERALLS_FLAG_NAME: test-${{ matrix.os }}-${{ matrix.python-version }}
 
-
-  dist:
-    name: Dist
-    runs-on: ubuntu-22.04
-    steps:
-    - uses: actions/checkout@v3
-      with:
-        fetch-depth: 0
-    - uses: hynek/build-and-inspect-python-package@v1
-
-  deploy:
-    name: Deploy
-    runs-on: ubuntu-22.04
-    needs: [dist]
-    if: github.event_name == 'release' && github.event.action == 'published'
-
-    steps:
-    - uses: actions/download-artifact@v3
-      with:
-        name: Packages
-        path: dist
-
-    - uses: pypa/gh-action-pypi-publish@v1.6.4
-      with:
-        password: ${{ secrets.pypi_password }}
-
   coverage:
     needs: [tests]
     runs-on: ubuntu-22.04
     steps:
     - uses: actions/setup-python@v4
       with:
         python-version: "3.x"
```

### Comparing `plumbum-1.8.1/conda.recipe/README.mkd` & `plumbum-1.8.2/conda.recipe/README.mkd`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/conda.recipe/meta.yaml` & `plumbum-1.8.2/conda.recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/Makefile` & `plumbum-1.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/_cheatsheet.rst` & `plumbum-1.8.2/docs/_cheatsheet.rst`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     >>> local.cwd
     <Workdir /home/tomer/workspace/plumbum>
     >>> with local.cwd(local.cwd / "docs"):
     ...     chain()
     ...
     '15\n'
 
-A more explicit, and thread-safe way of running a command in a differet directory is using the ``.with_cwd()`` method:
+A more explicit, and thread-safe way of running a command in a different directory is using the ``.with_cwd()`` method::
 
 .. code-block:: python
 
     >>> ls_in_docs = local.cmd.ls.with_cwd("docs")
     >>> ls_in_docs()
     'api\nchangelog.rst\n_cheatsheet.rst\ncli.rst\ncolorlib.rst\n_color_list.html\ncolors.rst\nconf.py\nindex.rst\nlocal_commands.rst\nlocal_machine.rst\nmake.bat\nMakefile\n_news.rst\npaths.rst\nquickref.rst\nremote.rst\n_static\n_templates\ntyped_env.rst\nutils.rst\n'
 
@@ -111,17 +111,17 @@
 
 
 See :ref:`guide-local-commands-nesting`.
 
 Remote commands (over SSH)
 --------------------------
 
-Supports `openSSH <http://www.openssh.org/>`_-compatible clients,
-`PuTTY <http://www.chiark.greenend.org.uk/~sgtatham/putty/>`_ (on Windows)
-and `Paramiko <https://github.com/paramiko/paramiko/>`_ (a pure-Python implementation of SSH2)
+Supports `openSSH <https://www.openssh.com/>`_-compatible clients,
+`PuTTY <https://www.chiark.greenend.org.uk/~sgtatham/putty/>`_ (on Windows)
+and `Paramiko <https://github.com/paramiko/paramiko/>`_ (a pure-Python implementation of SSH2):
 
 .. code-block:: python
 
     >>> from plumbum import SshMachine
     >>> remote = SshMachine("somehost", user = "john", keyfile = "/path/to/idrsa")
     >>> r_ls = remote["ls"]
     >>> with remote.cwd("/lib"):
```

### Comparing `plumbum-1.8.1/docs/_color_list.html` & `plumbum-1.8.2/docs/_color_list.html`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/_news.rst` & `plumbum-1.8.2/docs/_news.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+* **2023.01.01**: Version 1.8.1 released with hatchling replacing setuptools for the build system, and support for Path objects in local.
+
 * **2022.10.05**: Version 1.8.0 released with ``NO_COLOR``/``FORCE_COLOR``, ``all_markers`` & future annotations for the CLI, some command enhancements, & Python 3.11 testing.
 
 * **2021.12.23**: Version 1.7.2 released with very minor fixes, final version to support Python 2.7 and 3.5.
 
 * **2021.11.23**: Version 1.7.1 released with a few features like reverse tunnels, color group titles, and a glob path fix. Better Python 3.10 support.
 
 * **2021.02.08**: Version 1.7.0 released with a few new features like ``.with_cwd``, some useful bugfixes, and lots of cleanup.
```

### Comparing `plumbum-1.8.1/docs/cli.rst` & `plumbum-1.8.2/docs/cli.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _guide-cli:
 
 Command-Line Interface (CLI)
 ============================
 
 The other side of *executing programs* with ease is **writing CLI programs** with ease.
 Python scripts normally use ``optparse`` or the more recent ``argparse``, and their
-`derivatives <http://packages.python.org/argh/index.html>`_; but all of these are somewhat
+`derivatives <https://pythonhosted.org/argh/index.html>`_; but all of these are somewhat
 limited in their expressive power, and are quite **unintuitive** (and even **unpythonic**).
 Plumbum's CLI toolkit offers a **programmatic approach** to building command-line applications;
 instead of creating a parser object and populating it with a series of "options", the CLI toolkit
 translates these primitives into Pythonic constructs and relies on introspection.
 
 From a bird's eye view, CLI applications are classes that extend :class:`plumbum.cli.Application`.
 They define a ``main()`` method and optionally expose methods and attributes as command-line
@@ -145,35 +145,35 @@
 
 When the program is run, the switch functions are invoked with their appropriate arguments;
 for instance, ``$ ./myapp.py --log-to-file=/tmp/log`` would translate to a call to
 ``app.log_to_file("/tmp/log")``. After all switches were processed, control passes to ``main``.
 
 .. note::
    Methods' docstrings and argument names will be used to render the help message, keeping your
-   code as `DRY <http://en.wikipedia.org/wiki/Don't_repeat_yourself>`_ as possible.
+   code as `DRY <https://en.wikipedia.org/wiki/Don't_repeat_yourself>`_ as possible.
 
    There's also :func:`autoswitch <plumbum.cli.autoswitch>`, which infers the name of the switch
-   from the function's name, e.g. ::
+   from the function's name, e.g.::
 
         @cli.autoswitch(str)
         def log_to_file(self, filename):
             pass
 
    Will bind the switch function to ``--log-to-file``.
 
 Arguments
 ^^^^^^^^^
 As demonstrated in the example above, switch functions may take no arguments (not counting
-``self``) or a single argument argument. If a switch function accepts an argument, it must
+``self``) or a single argument. If a switch function accepts an argument, it must
 specify the argument's *type*. If you require no special validation, simply pass ``str``;
 otherwise, you may pass any type (or any callable, in fact) that will take a string and convert
 it to a meaningful object. If conversion is not possible, the type (or callable) is expected to
 raise either ``TypeError`` or ``ValueError``.
 
-For instance ::
+For instance::
 
     class MyApp(cli.Application):
         _port = 8080
 
         @cli.switch(["-p"], int)
         def server_port(self, port):
             self._port = port
@@ -190,15 +190,15 @@
         ValueError("invalid literal for int() with base 10: 'foo'",)
 
 The toolkit includes two additional "types" (or rather, *validators*): ``Range`` and ``Set``.
 ``Range`` takes a minimal value and a maximal value and expects an integer in
 that range (inclusive). ``Set`` takes a set of allowed values, and expects the
 argument to match one of these values. You can set ``case_sensitive=False``, or
 add ``all_markers={"*", "all"}`` if you want to have a "trigger all markers"
-marker. Here's an example ::
+marker. Here's an example::
 
     class MyApp(cli.Application):
         _port = 8080
         _mode = "TCP"
 
         @cli.switch("-p", cli.Range(1024,65535))
         def server_port(self, port):
@@ -228,15 +228,15 @@
 
 
 Repeatable Switches
 ^^^^^^^^^^^^^^^^^^^
 Many times, you would like to allow a certain switch to be given multiple times. For instance,
 in ``gcc``, you may give several include directories using ``-I``. By default, switches may
 only be given once, unless you allow multiple occurrences by passing ``list = True`` to the
-``switch`` decorator ::
+``switch`` decorator::
 
     class MyApp(cli.Application):
         _dirs = []
 
         @cli.switch("-I", str, list = True)
         def include_dirs(self, dirs):
             self._dirs = dirs
@@ -256,15 +256,15 @@
 ^^^^^^^^^^^^^^^^^^
 If a certain switch is required, you can specify this by passing ``mandatory = True`` to the
 ``switch`` decorator. The user will not be able to run the program without specifying a value
 for this switch.
 
 Dependencies
 ^^^^^^^^^^^^
-Many time, the occurrence of a certain switch depends on the occurrence of another, e..g, it
+Many times, the occurrence of a certain switch depends on the occurrence of another, e.g., it
 may not be possible to give ``-x`` without also giving ``-y``. This constraint can be achieved
 by specifying the ``requires`` keyword argument to the ``switch`` decorator; it is a list
 of switch names that this switch depends on. If the required switches are missing, the user
 will not be able to run the program. ::
 
     class MyApp(cli.Application):
         @cli.switch("--log-to-file", str)
@@ -318,18 +318,17 @@
 the help message.
 
 Switch Attributes
 -----------------
 Many times it's desired to simply store a switch's argument in an attribute, or set a flag if
 a certain switch is given. For this purpose, the toolkit provides
 :class:`SwitchAttr <plumbum.cli.SwitchAttr>`, which is `data descriptor
-<http://docs.python.org/howto/descriptor.html>`_ that stores the argument in an instance attribute.
+<https://docs.python.org/howto/descriptor.html>`_ that stores the argument in an instance attribute.
 There are two additional "flavors" of ``SwitchAttr``: ``Flag`` (which toggles its default value
-if the switch is given) and ``CountOf`` (which counts the number of occurrences of the switch)
-::
+if the switch is given) and ``CountOf`` (which counts the number of occurrences of the switch)::
 
     class MyApp(cli.Application):
         log_file = cli.SwitchAttr("--log-file", str, default = None)
         enable_logging = cli.Flag("--no-log", default = True)
         verbosity_level = cli.CountOf("-v")
 
         def main(self):
@@ -368,15 +367,15 @@
 
 The ``main()`` method takes control once all the command-line switches have been processed.
 It may take any number of *positional argument*; for instance, in ``cp -r /foo /bar``,
 ``/foo`` and ``/bar`` are the *positional arguments*. The number of positional arguments
 that the program would accept depends on the signature of the method: if the method takes 5
 arguments, 2 of which have default values, then at least 3 positional arguments must be supplied
 by the user and at most 5. If the method also takes varargs (``*args``), the number of
-arguments that may be given is unbound ::
+arguments that may be given is unbound::
 
     class MyApp(cli.Application):
         def main(self, src, dst, mode = "normal"):
             print(src, dst, mode)
 
 ::
 
@@ -458,15 +457,15 @@
 
 Sub-commands
 ------------
 .. versionadded:: 1.1
 
 A common practice of CLI applications, as they span out and get larger, is to split their
 logic into multiple, pluggable *sub-applications* (or *sub-commands*). A classic example is version
-control systems, such as `git <http://git-scm.com/>`_, where ``git`` is the *root* command,
+control systems, such as `git <https://git-scm.com/>`_, where ``git`` is the *root* command,
 under which sub-commands such as ``commit`` or ``push`` are nested. Git even supports ``alias``-ing,
 which creates allows users to create custom sub-commands. Plumbum makes writing such applications
 really easy.
 
 Before we get to the code, it is important to stress out two things:
 
 * Under Plumbum, each sub-command is a full-fledged ``cli.Application`` on its own; if you wish,
@@ -481,15 +480,15 @@
   application is invoked. Take, for instance, ``git --foo=bar spam push origin --tags``: the root
   application, ``git``, is in charge of the switch ``--foo`` and the positional argument ``spam``,
   and the nested application ``push`` is in charge of the arguments that follow it. In theory,
   you can nest several sub-applications one into the other; in practice, only a single level
   is normally used.
 
 Here is an example of a mock version control system, called ``geet``. We're going to have a root
-application ``Geet``, which has two sub-commands - ``GeetCommit`` and ``GeetPush``: these are
+application ``Geet``, which has two sub-commands – ``GeetCommit`` and ``GeetPush``: these are
 attached to the root application using the ``subcommand`` decorator ::
 
     class Geet(cli.Application):
         """The l33t version control"""
         VERSION = "1.7.2"
 
         def main(self, *args):
@@ -613,13 +612,13 @@
 For the full list of helpers or more information, see the :ref:`api docs <api-cli>`.
 
 
 
 See Also
 --------
 * `filecopy.py <https://github.com/tomerfiliba/plumbum/blob/master/examples/filecopy.py>`_ example
-* `geet.py <https://github.com/tomerfiliba/plumbum/blob/master/examples/geet.py>`_ - a runnable
+* `geet.py <https://github.com/tomerfiliba/plumbum/blob/master/examples/geet.py>`_ – a runnable
   example of using sub-commands
-* `RPyC <http://rpyc.sf.net>`_ has changed it bash-based build script to Plumbum CLI.
+* `RPyC <https://rpyc.readthedocs.io/>`_ has changed its bash-based build script to Plumbum CLI.
   Notice `how short and readable <https://github.com/tomerfiliba/rpyc/blob/c457a28d689df7605838334a437c6b35f9a94618/build.py>`_
   it is.
 * A `blog post <http://tomerfiliba.com/blog/Plumbum/>`_ describing the philosophy of the CLI module
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `plumbum-1.8.1/docs/colorlib.rst` & `plumbum-1.8.2/docs/colorlib.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/colors.rst` & `plumbum-1.8.2/docs/colors.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/conf.py` & `plumbum-1.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/index.rst` & `plumbum-1.8.2/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     <ul>
     <li><a href="#requirements" title="Jump to download">Download</a></li>
     <li><a href="#user-guide" title="Jump to user guide">User Guide</a></li>
     <li><a href="#api-reference" title="Jump to API reference">API Reference</a></li>
     <li><a href="#about" title="Jump to user guide">About</a></li>
     </ul>
     <hr/>
-    <a href="http://tomerfiliba.com" target="_blank">
+    <a href="https://tomerfiliba.com" target="_blank">
     <img style="display: block; margin-left: auto; margin-right: auto" alt="Tomer Filiba"
     src="_static/fish-text-black.png" title="Tomer's Blog"/>
     <span style="color:transparent;position: absolute;font-size:5px;width: 0px;height: 0px;">Tomer Filiba</span></a>
     <br/>
-    <a href="http://github.com/tomerfiliba/plumbum" target="_blank">
+    <a href="https://github.com/tomerfiliba/plumbum" target="_blank">
     <img style="display: block; margin-left: auto; margin-right: auto; opacity: 0.7; width: 70px;"
     src="_static/github-logo.png" title="Github Repo"/></a>
     <br/>
     <a alt="Build Status" href="https://github.com/tomerfiliba/plumbum/actions" target="_blank">
     <img src="https://github.com/tomerfiliba/plumbum/workflows/CI/badge.svg"
     style="display: block; margin-left: auto; margin-right: auto;" title="Travis CI status"></a>
     </div>
@@ -30,15 +30,15 @@
 .. comment raw:: html
 
    <div style="width:795px; margin: 1em 0 2em 0; display: block; padding: 1em; border: 1px dotted #DDD;
     background-color: rgba(255, 255, 202, 0.69); border-radius: 5px;">
 
    <strong>Sticky</strong><br/>
 
-   <a class="reference external" href="https://pypi.python.org/pypi/rpyc">Version 3.2.3</a>
+   <a class="reference external" href="https://pypi.org/project/rpyc">Version 3.2.3</a>
    was released on December 2nd <br/>
 
    Please use the
    <a class="reference external" href="https://groups.google.com/forum/?fromgroups#!forum/rpyc">mailing list</a>
    to ask questions and use
    <a class="reference external" href="https://github.com/tomerfiliba/rpyc/issues">github issues</a>
    to report problems. <strong>Please do not email me directly</strong>.
@@ -71,30 +71,30 @@
 
 .. include:: _cheatsheet.rst
 
 Development and Installation
 ============================
 
 The library is developed on `GitHub <https://github.com/tomerfiliba/plumbum>`_, and will happily
-accept `patches <http://help.github.com/send-pull-requests/>`_ from users. Please use the GitHub's
+accept `patches <https://docs.github.com/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request>`_ from users. Please use the GitHub's
 built-in `issue tracker <https://github.com/tomerfiliba/plumbum/issues>`_ to report any problem
 you encounter or to request features. The library is released under the permissive `MIT license
 <https://github.com/tomerfiliba/plumbum/blob/master/LICENSE>`_.
 
 Requirements
 ------------
 
 Plumbum supports **Python 3.6-3.10** and **PyPy** and is continually tested on
 **Linux**, **Mac**, and **Windows** machines through `GitHub Actions
 <https://github.com/tomerfiliba/plumbum/actions>`_.  Any Unix-like machine
 should work fine out of the box, but on Windows, you'll probably want to
-install a decent `coreutils <http://en.wikipedia.org/wiki/Coreutils>`_
+install a decent `coreutils <https://en.wikipedia.org/wiki/GNU_Core_Utilities/>`_
 environment and add it to your ``PATH``, or use WSL(2). I can recommend `mingw
-<http://mingw.org/>`_ (which comes bundled with `Git for Windows
-<http://msysgit.github.com/>`_), but `cygwin <http://www.cygwin.com/>`_ should
+<https://mingw.osdn.io/>`_ (which comes bundled with `Git for Windows
+<https://gitforwindows.org/>`_), but `cygwin <http://www.cygwin.com/>`_ should
 work too. If you only wish to use Plumbum as a Popen-replacement to run Windows
 programs, then there's no need for the Unix tools.
 
 Note that for remote command execution, an **openSSH-compatible** client is
 required (also bundled with *Git for Windows*), and a ``bash``-compatible shell
 and a coreutils environment is also expected on the host machine.
 
@@ -102,15 +102,15 @@
 required for building SDists. These dependencies will be handled for you by PEP
 518 compatible builders, like `build <https://github.com/pypa/build>`_ and ``pip 10+``.
 
 Download
 --------
 
 You can **download** the library from the `Python Package Index
-<http://pypi.python.org/pypi/plumbum#downloads>`_ (in a variety of formats), or
+<https://pypi.org/pypi/plumbum/#files>`_ (in a variety of formats), or
 run ``pip install plumbum`` directly. If you use Anaconda, you can also get it
 from the ``conda-forge`` channel with ``conda install -c conda-forge plumbum``.
 
 User Guide
 ==========
 The user guide covers most of the features of Plumbum, with lots of code-snippets to get you
 swimming in no time. It introduces the concepts and "syntax" gradually, so it's recommended
@@ -157,20 +157,20 @@
 assuming nothing fancier than good-old SSH. On top of this, a file-system abstraction layer
 was devised, so that working with local and remote files would be seamless.
 
 I've toyed with this idea for some time now, but it wasn't until I had to write build scripts
 for a project I've been working on that I decided I've had it with shell scripts and it's time
 to make it happen. Plumbum was born from the scraps of the ``Path`` class, which I
 wrote for the aforementioned build system, and the ``SshContext`` and ``SshTunnel`` classes
-that I wrote for `RPyC <http://rpyc.sf.net>`_. When I combined the two with *shell combinators*
+that I wrote for `RPyC <https://rpyc.readthedocs.io/>`_. When I combined the two with *shell combinators*
 (because shell scripts do have an edge there) the magic happened and here we are.
 
 Credits
 =======
-The project has been inspired by **PBS** (now called `sh <http://amoffat.github.com/sh/>`_)
+The project has been inspired by **PBS** (now called `sh <http://amoffat.github.io/sh/>`_)
 of `Andrew Moffat <https://github.com/amoffat>`_,
 and has borrowed some of his ideas (namely treating programs like functions and the
 nice trick for importing commands). However, I felt there was too much magic going on in PBS,
 and that the syntax wasn't what I had in mind when I came to write shell-like programs.
 I contacted Andrew about these issues, but he wanted to keep PBS this way. Other than that,
 the two libraries go in different directions, where Plumbum attempts to provide a more
 wholesome approach.
```

#### html2text {}

```diff
@@ -25,65 +25,66 @@
 execution (over SSH), local and remote file-system :ref:`paths `, easy working-
 directory and environment :ref:`manipulation `, quick access to ANSI :ref:
 `colors `, and a programmatic :ref:`guide-cli` application toolkit. Now let's
 see some code! News ==== .. include:: _news.rst * :doc:`changelog` * :doc:
 `quickref` Cheat Sheet =========== .. include:: _cheatsheet.rst Development and
 Installation ============================ The library is developed on `GitHub
 github.com/tomerfiliba/plumbum>`_, and will happily accept `patches
-help.github.com/send-pull-requests/>`_ from users. Please use the GitHub's
-built-in `issue tracker
+docs.github.com/pull-requests/collaborating-with-pull-requests/proposing-
+changes-to-your-work-with-pull-requests/creating-a-pull-request>`_ from users.
+Please use the GitHub's built-in `issue tracker
 github.com/tomerfiliba/plumbum/issues>`_ to report any problem you encounter or
 to request features. The library is released under the permissive `MIT license
 github.com/tomerfiliba/plumbum/blob/master/LICENSE>`_. Requirements -----------
 - Plumbum supports **Python 3.6-3.10** and **PyPy** and is continually tested
 on **Linux**, **Mac**, and **Windows** machines through `GitHub Actions
 github.com/tomerfiliba/plumbum/actions>`_. Any Unix-like machine should work
 fine out of the box, but on Windows, you'll probably want to install a decent
 `coreutils
-en.wikipedia.org/wiki/Coreutils>`_ environment and add it to your ``PATH``, or
-use WSL(2). I can recommend `mingw
-mingw.org/>`_ (which comes bundled with `Git for Windows
-msysgit.github.com/>`_), but `cygwin
+en.wikipedia.org/wiki/GNU_Core_Utilities/>`_ environment and add it to your
+``PATH``, or use WSL(2). I can recommend `mingw
+mingw.osdn.io/>`_ (which comes bundled with `Git for Windows
+gitforwindows.org/>`_), but `cygwin
 www.cygwin.com/>`_ should work too. If you only wish to use Plumbum as a Popen-
 replacement to run Windows programs, then there's no need for the Unix tools.
 Note that for remote command execution, an **openSSH-compatible** client is
 required (also bundled with *Git for Windows*), and a ``bash``-compatible shell
 and a coreutils environment is also expected on the host machine. This project
 uses ``setuptools`` to build wheels; and ``setuptools_scm`` is required for
 building SDists. These dependencies will be handled for you by PEP 518
 compatible builders, like `build
 github.com/pypa/build>`_ and ``pip 10+``. Download -------- You can
 **download** the library from the `Python Package Index
-pypi.python.org/pypi/plumbum#downloads>`_ (in a variety of formats), or run
-``pip install plumbum`` directly. If you use Anaconda, you can also get it from
-the ``conda-forge`` channel with ``conda install -c conda-forge plumbum``. User
-Guide ========== The user guide covers most of the features of Plumbum, with
-lots of code-snippets to get you swimming in no time. It introduces the
-concepts and "syntax" gradually, so it's recommended you read it in order. A
-quick :ref:`reference guide is available `. .. toctree:: :maxdepth: 2
-local_commands paths local_machine remote utils cli typed_env colors changelog
-quickref API Reference ============= The API reference (generated from the
-*docstrings* within the library) covers all of the exposed APIs of the library.
-Note that some "advanced" features and some function parameters are missing
-from the guide, so you might want to consult with the API reference in these
-cases. .. toctree:: :maxdepth: 2 api/cli api/commands api/machines api/path
-api/fs api/colors colorlib .. note:: The ``local`` object is an instance of a
-``machine``. About ===== The original purpose of Plumbum was to enable local
-and remote program execution with ease, assuming nothing fancier than good-old
-SSH. On top of this, a file-system abstraction layer was devised, so that
-working with local and remote files would be seamless. I've toyed with this
-idea for some time now, but it wasn't until I had to write build scripts for a
-project I've been working on that I decided I've had it with shell scripts and
-it's time to make it happen. Plumbum was born from the scraps of the ``Path``
-class, which I wrote for the aforementioned build system, and the
-``SshContext`` and ``SshTunnel`` classes that I wrote for `RPyC
-rpyc.sf.net>`_. When I combined the two with *shell combinators* (because shell
-scripts do have an edge there) the magic happened and here we are. Credits
-======= The project has been inspired by **PBS** (now called `sh
-amoffat.github.com/sh/>`_) of `Andrew Moffat
+pypi.org/pypi/plumbum/#files>`_ (in a variety of formats), or run ``pip install
+plumbum`` directly. If you use Anaconda, you can also get it from the ``conda-
+forge`` channel with ``conda install -c conda-forge plumbum``. User Guide
+========== The user guide covers most of the features of Plumbum, with lots of
+code-snippets to get you swimming in no time. It introduces the concepts and
+"syntax" gradually, so it's recommended you read it in order. A quick :ref:
+`reference guide is available `. .. toctree:: :maxdepth: 2 local_commands paths
+local_machine remote utils cli typed_env colors changelog quickref API
+Reference ============= The API reference (generated from the *docstrings*
+within the library) covers all of the exposed APIs of the library. Note that
+some "advanced" features and some function parameters are missing from the
+guide, so you might want to consult with the API reference in these cases. ..
+toctree:: :maxdepth: 2 api/cli api/commands api/machines api/path api/fs api/
+colors colorlib .. note:: The ``local`` object is an instance of a ``machine``.
+About ===== The original purpose of Plumbum was to enable local and remote
+program execution with ease, assuming nothing fancier than good-old SSH. On top
+of this, a file-system abstraction layer was devised, so that working with
+local and remote files would be seamless. I've toyed with this idea for some
+time now, but it wasn't until I had to write build scripts for a project I've
+been working on that I decided I've had it with shell scripts and it's time to
+make it happen. Plumbum was born from the scraps of the ``Path`` class, which I
+wrote for the aforementioned build system, and the ``SshContext`` and
+``SshTunnel`` classes that I wrote for `RPyC
+rpyc.readthedocs.io/>`_. When I combined the two with *shell combinators*
+(because shell scripts do have an edge there) the magic happened and here we
+are. Credits ======= The project has been inspired by **PBS** (now called `sh
+amoffat.github.io/sh/>`_) of `Andrew Moffat
 github.com/amoffat>`_, and has borrowed some of his ideas (namely treating
 programs like functions and the nice trick for importing commands). However, I
 felt there was too much magic going on in PBS, and that the syntax wasn't what
 I had in mind when I came to write shell-like programs. I contacted Andrew
 about these issues, but he wanted to keep PBS this way. Other than that, the
 two libraries go in different directions, where Plumbum attempts to provide a
 more wholesome approach. Plumbum also pays tribute to `Rotem Yaari
```

### Comparing `plumbum-1.8.1/docs/local_commands.rst` & `plumbum-1.8.2/docs/local_commands.rst`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,23 @@
     >>> chain = ls["-l"] | grep[".py"]
     >>> print(chain)
     C:\Program Files\Git\bin\ls.exe -l | C:\Program Files\Git\bin\grep.exe .py
     >>>
     >>> chain()
     '-rw-r--r--    1 sebulba  Administ        0 Apr 27 11:54 setup.py\n'
 
+.. note::
+  Unlike common posix shells, plumbum only captures stderr of the last command in a pipeline.
+  If any of the other commands writes a large amount of text to the stderr, the whole pipeline
+  will stall (large amount equals to >64k on posix systems). This can happen with bioinformatics
+  tools that write progress information to stderr. To avoid this issue, you can discard stderr
+  of the first commands or redirect it to a file.
+
+  >>> chain = (bwa["mem", ...] >= "/dev/null") | samtools["view", ...]
+
 .. _guide-local-commands-redir:
 
 Input/Output Redirection
 ------------------------
 We can also use redirection into files (or any object that exposes a real ``fileno()``).
 If a string is given, it is assumed to be a file name, and a file with that name is opened
 for you. In this example, we're reading from ``stdin`` into ``grep world``, and redirecting
```

### Comparing `plumbum-1.8.1/docs/local_machine.rst` & `plumbum-1.8.2/docs/local_machine.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/make.bat` & `plumbum-1.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/paths.rst` & `plumbum-1.8.2/docs/paths.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/quickref.rst` & `plumbum-1.8.2/docs/quickref.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/remote.rst` & `plumbum-1.8.2/docs/remote.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/typed_env.rst` & `plumbum-1.8.2/docs/typed_env.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/utils.rst` & `plumbum-1.8.2/docs/utils.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/_static/fish-text-black.png` & `plumbum-1.8.2/docs/_static/fish-text-black.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/_static/github-logo.png` & `plumbum-1.8.2/docs/_static/github-logo.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/_static/logo.png` & `plumbum-1.8.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/_static/logo2.png` & `plumbum-1.8.2/docs/_static/logo2.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/_static/logo3.png` & `plumbum-1.8.2/docs/_static/logo3.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/_static/logo4.png` & `plumbum-1.8.2/docs/_static/logo4.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/_static/logo6.png` & `plumbum-1.8.2/docs/_static/logo6.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/_static/logo7.png` & `plumbum-1.8.2/docs/_static/logo7.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/_static/logo8.png` & `plumbum-1.8.2/docs/_static/logo8.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/api/colors.rst` & `plumbum-1.8.2/docs/api/colors.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/docs/api/machines.rst` & `plumbum-1.8.2/docs/api/machines.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/examples/PHSP.png` & `plumbum-1.8.2/examples/PHSP.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/examples/color.py` & `plumbum-1.8.2/examples/color.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/examples/filecopy.py` & `plumbum-1.8.2/examples/filecopy.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,15 @@
         logger.setLevel(logging.DEBUG)
 
     def main(self, src, dst):
         if local.path(dst).exists():
             if not self.overwrite:
                 logger.debug("Oh no! That's terrible")
                 raise ValueError("Destination already exists")
-            else:
-                delete(dst)
+            delete(dst)
 
         logger.debug("I'm going to copy %s to %s", src, dst)
         copy(src, dst)
         logger.debug("Great success")
 
 
 if __name__ == "__main__":
```

### Comparing `plumbum-1.8.1/examples/geet.py` & `plumbum-1.8.2/examples/geet.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/examples/make_figures.py` & `plumbum-1.8.2/examples/make_figures.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/examples/simple_cli.py` & `plumbum-1.8.2/examples/simple_cli.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/experiments/parallel.py` & `plumbum-1.8.2/experiments/parallel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from plumbum.commands.base import BaseCommand
 from plumbum.commands.processes import CommandNotFound, ProcessExecutionError, run_proc
 
 
 def make_concurrent(self, rhs):
     if not isinstance(rhs, BaseCommand):
         raise TypeError("rhs must be an instance of BaseCommand")
+
     if isinstance(self, ConcurrentCommand):
         if isinstance(rhs, ConcurrentCommand):
             self.commands.extend(rhs.commands)
         else:
             self.commands.append(rhs)
         return self
-    elif isinstance(rhs, ConcurrentCommand):
+
+    if isinstance(rhs, ConcurrentCommand):
         rhs.commands.insert(0, self)
         return rhs
-    else:
-        return ConcurrentCommand(self, rhs)
+
+    return ConcurrentCommand(self, rhs)
 
 
 BaseCommand.__and__ = make_concurrent
 
 
 class ConcurrentPopen:
     def __init__(self, procs):
@@ -65,29 +67,29 @@
         self.commands = list(commands)
 
     def formulate(self, level=0, args=()):
         form = ["("]
         for cmd in self.commands:
             form.extend(cmd.formulate(level, args))
             form.append("&")
-        return form + [")"]
+        return [*form, ")"]
 
     def popen(self, *args, **kwargs):
         return ConcurrentPopen([cmd[args].popen(**kwargs) for cmd in self.commands])
 
     def __getitem__(self, args):
         """Creates a bound-command with the given arguments"""
         if not isinstance(args, (tuple, list)):
             args = [
                 args,
             ]
         if not args:
             return self
-        else:
-            return ConcurrentCommand(*(cmd[args] for cmd in self.commands))
+
+        return ConcurrentCommand(*(cmd[args] for cmd in self.commands))
 
 
 class Cluster:
     def __init__(self, *machines):
         self.machines = list(machines)
 
     def __enter__(self):
@@ -160,15 +162,15 @@
     def __enter__(self):
         return self
 
     def __exit__(self, t, v, tb):
         self.close()
 
     def __del__(self):
-        try:
+        try:  # noqa: 167
             self.close()
         except Exception:
             pass
 
     def alive(self):
         """Returns ``True`` if the underlying shells are all alive, ``False`` otherwise"""
         return all(session.alive for session in self)
```

### Comparing `plumbum-1.8.1/experiments/test_parallel.py` & `plumbum-1.8.2/experiments/test_parallel.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/__init__.py` & `plumbum-1.8.2/plumbum/__init__.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/_testtools.py` & `plumbum-1.8.2/plumbum/_testtools.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/colors.py` & `plumbum-1.8.2/plumbum/colors.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/lib.py` & `plumbum-1.8.2/plumbum/lib.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/typed_env.py` & `plumbum-1.8.2/plumbum/typed_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,16 +138,15 @@
         raise EnvironmentVariableError(key_names[0])
 
     def __contains__(self, key):
         try:
             self._raw_get(key)
         except EnvironmentVariableError:
             return False
-        else:
-            return True
+        return True
 
     def __getattr__(self, name):
         # if we're here then there was no descriptor defined
         try:
             return self._raw_get(name)
         except EnvironmentVariableError:
             raise AttributeError(
```

### Comparing `plumbum-1.8.1/plumbum/cli/__init__.py` & `plumbum-1.8.2/plumbum/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/cli/application.py` & `plumbum-1.8.2/plumbum/cli/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
                 tailargs.extend(argv)
                 break
 
             if a in self._subcommands:
                 subcmd = self._subcommands[a].get()
                 self.nested_command = (
                     subcmd,
-                    [self.PROGNAME + " " + self._subcommands[a].name] + argv,
+                    [self.PROGNAME + " " + self._subcommands[a].name, *argv],
                 )
                 break
 
             if a.startswith("--") and len(a) >= 3:
                 # [--name], [--name=XXX], [--name, XXX], [--name, ==, XXX],
                 # [--name=, XXX], [--name, =XXX]
                 eqsign = a.find("=")
@@ -545,15 +545,15 @@
             for item in m.annotations:
                 annotation = (
                     sig.parameters[item].annotation
                     if item != "return"
                     else sig.return_annotation
                 )
                 if sys.version_info < (3, 10) and isinstance(annotation, str):
-                    annotation = eval(annotation)
+                    annotation = eval(annotation)  # noqa: PGH001
                 if item == m.varargs:
                     varargs = annotation
                 elif item != "return":
                     positional[args_names.index(item)] = annotation
 
             tailargs = self._positional_validate(
                 tailargs, positional, varargs, m.args[1:], m.varargs
@@ -566,15 +566,14 @@
         return ordered, tailargs
 
     def _positional_validate(self, args, validator_list, varargs, argnames, varargname):
         """Makes sure args follows the validation given input"""
         out_args = list(args)
 
         for i in range(min(len(args), len(validator_list))):
-
             if validator_list[i] is not None:
                 out_args[i] = self._handle_argument(
                     args[i], validator_list[i], argnames[i]
                 )
 
         if len(args) > len(validator_list):
             if varargs is not None:
```

### Comparing `plumbum-1.8.1/plumbum/cli/config.py` & `plumbum-1.8.2/plumbum/cli/config.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/cli/i18n.py` & `plumbum-1.8.2/plumbum/cli/i18n.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         def ngettext(self, str1, strN, n):  # pylint: disable=no-self-use
             if n == 1:
                 return str1.replace("{0}", str(n))
 
             return strN.replace("{0}", str(n))
 
     def get_translation_for(
-        package_name: str,  # pylint: disable=unused-argument
+        package_name: str,  # noqa: ARG001
     ) -> NullTranslation:
         return NullTranslation()
 
 else:
     import gettext
     import os
```

### Comparing `plumbum-1.8.1/plumbum/cli/image.py` & `plumbum-1.8.2/plumbum/cli/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from plumbum import colors
 
 from .. import cli
 from .termsize import get_terminal_size
 
 
 class Image:
-
     __slots__ = "size char_ratio".split()
 
     def __init__(self, size=None, char_ratio=2.45):
         self.size = size
         self.char_ratio = char_ratio
 
     def best_aspect(self, orig, term):
@@ -22,18 +21,17 @@
 
         if not self.char_ratio:  # Don't use if char ratio is 0
             return term
 
         orig_ratio = orig[0] / orig[1] / self.char_ratio
 
         if int(term[1] / orig_ratio) <= term[0]:
-            new_size = int(term[1] / orig_ratio), term[1]
-        else:
-            new_size = term[0], int(term[0] * orig_ratio)
-        return new_size
+            return int(term[1] / orig_ratio), term[1]
+
+        return term[0], int(term[0] * orig_ratio)
 
     def show(self, filename, double=False):
         """Display an image on the command line. Can select a size or show in double resolution."""
 
         import PIL.Image
 
         return (
@@ -96,15 +94,14 @@
 
     ratio = cli.SwitchAttr(
         ["--ratio"], float, default=2.45, help="Aspect ratio of the font"
     )
 
     @cli.positional(cli.ExistingFile)
     def main(self, filename):
-
         size = None
         if self.size:
             size = map(int, self.size.split("x"))
 
         Image(size, self.ratio).show(filename, self.double)
```

### Comparing `plumbum-1.8.1/plumbum/cli/progress.py` & `plumbum-1.8.2/plumbum/cli/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,14 @@
         sys.stdout.flush()
 
 
 class ProgressIPy(ProgressBase):  # pragma: no cover
     HTMLBOX = '<div class="widget-hbox widget-progress"><div class="widget-label" style="display:block;">{0}</div></div>'
 
     def __init__(self, *args, **kargs):
-
         # Ipython gives warnings when using widgets about the API potentially changing
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             try:
                 from ipywidgets import HTML, HBox, IntProgress
             except ImportError:  # Support IPython < 4.0
                 from IPython.html.widgets import HTML, HBox, IntProgress
@@ -238,15 +237,15 @@
     :param timer: Try to time the completion status of the iterator
     :param body: True if the slow portion occurs outside the iterator (in a loop, for example)
     """
 
     def __new__(cls, *args, **kargs):
         """Uses the generator trick that if a cls instance is returned, the __init__ method is not called."""
         try:  # pragma: no cover
-            __IPYTHON__  # pylint: disable=pointless-statement
+            __IPYTHON__  # noqa: B018
             try:
                 from traitlets import TraitError
             except ImportError:  # Support for IPython < 4.0
                 from IPython.utils.traitlets import TraitError
 
             try:
                 return ProgressIPy(*args, **kargs)
```

### Comparing `plumbum-1.8.1/plumbum/cli/switches.py` & `plumbum-1.8.2/plumbum/cli/switches.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,18 +157,15 @@
     names = [n.lstrip("-") for n in names]
     requires = [n.lstrip("-") for n in requires]
     excludes = [n.lstrip("-") for n in excludes]
 
     def deco(func):
         if argname is None:
             argspec = inspect.getfullargspec(func).args
-            if len(argspec) == 2:
-                argname2 = argspec[1]
-            else:
-                argname2 = _("VALUE")
+            argname2 = argspec[1] if len(argspec) == 2 else _("VALUE")
         else:
             argname2 = argname
         help2 = getdoc(func) if help is None else help
         if not help2:
             help2 = str(func)
         func._switch_info = SwitchInfo(
             names=names,
@@ -385,15 +382,16 @@
 class Validator(ABC):
     __slots__ = ()
 
     @abstractmethod
     def __call__(self, obj):
         "Must be implemented for a Validator to work"
 
-    def choices(self, partial=""):  # pylint: disable=no-self-use, unused-argument
+    # pylint: disable-next=no-self-use
+    def choices(self, partial=""):  # noqa: ARG002
         """Should return set of valid choices, can be given optional partial info"""
         return set()
 
     def __repr__(self):
         """If not overridden, will print the slots as args"""
 
         slots = {}
@@ -434,15 +432,15 @@
         obj = int(obj)
         if obj < self.start or obj > self.end:
             raise ValueError(
                 _("Not in range [{0:d}..{1:d}]").format(self.start, self.end)
             )
         return obj
 
-    def choices(self, partial=""):
+    def choices(self, partial=""):  # noqa: ARG002
         # TODO: Add partial handling
         return set(range(self.start, self.end + 1))
 
 
 class Set(Validator):
     """
     A switch-type validator that checks that the value is contained in a defined
@@ -491,15 +489,15 @@
 
         if not self.case_sensitive:
             value = value.lower()
 
         for opt in self.values:
             if isinstance(opt, str):
                 if not self.case_sensitive:
-                    opt = opt.lower()
+                    opt = opt.lower()  # noqa: PLW2901
                 if opt == value or value in self.all_markers:
                     yield opt  # always return original value
                 continue
             with contextlib.suppress(ValueError):
                 yield opt(value)
 
     def __call__(self, value: str, check_csv: bool = True) -> Union[str, List[str]]:
@@ -511,15 +509,15 @@
             return items
         return items[0]
 
     def choices(self, partial=""):
         choices = {opt if isinstance(opt, str) else f"({opt})" for opt in self.values}
         choices |= self.all_markers
         if partial:
-            choices = {opt for opt in choices if opt.lower().startswith(partial)}
+            return {opt for opt in choices if opt.lower().startswith(partial)}
         return choices
 
 
 CSV = Set(str, csv=True)
 
 
 class Predicate:
@@ -530,15 +528,16 @@
 
     def __str__(self):
         return self.func.__name__
 
     def __call__(self, val):
         return self.func(val)
 
-    def choices(self, partial=""):  # pylint: disable=no-self-use, unused-argument
+    # pylint: disable-next=no-self-use
+    def choices(self, partial=""):  # noqa: ARG002
         return set()
 
 
 @Predicate
 def ExistingDirectory(val):
     """A switch-type validator that ensures that the given argument is an existing directory"""
     p = local.path(val)
```

### Comparing `plumbum-1.8.1/plumbum/cli/terminal.py` & `plumbum-1.8.2/plumbum/cli/terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,31 +89,27 @@
         # this will display "blue", "yellow" and "green" but return a numerical value
     """
     if hasattr(options, "items"):
         options = options.items()
     sys.stdout.write(question.rstrip() + "\n")
     choices = {}
     defindex = None
-    for i, item in enumerate(options):
-        i += 1
+    for i, item in enumerate(options, 1):
         if isinstance(item, (tuple, list)) and len(item) == 2:
             text = item[0]
             val = item[1]
         else:
             text = item
             val = item
         choices[i] = val
         if default is not None and default == val:
             defindex = i
         sys.stdout.write(f"({i}) {text}\n")
     if default is not None:
-        if defindex is None:
-            msg = f"Choice [{default}]: "
-        else:
-            msg = f"Choice [{defindex}]: "
+        msg = f"Choice [{default}]: " if defindex is None else f"Choice [{defindex}]: "
     else:
         msg = "Choice: "
     while True:
         try:
             choice = readline(msg).strip()
         except EOFError:
             choice = ""
@@ -129,15 +125,15 @@
         return choices[choice]
 
 
 def prompt(
     question,
     type=str,  # pylint: disable=redefined-builtin
     default=NotImplemented,
-    validator=lambda val: True,
+    validator=lambda _: True,
 ):
     """
     Presents the user with a validated question, keeps asking if validation does not pass.
 
     :param question: The question to ask
     :param type: The type of the answer, defaults to str
     :param default: The default choice
```

### Comparing `plumbum-1.8.1/plumbum/cli/termsize.py` & `plumbum-1.8.2/plumbum/cli/termsize.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,22 +29,22 @@
     elif current_os in ("Linux", "Darwin", "FreeBSD", "SunOS") or current_os.startswith(
         "CYGWIN"
     ):
         size = _get_terminal_size_linux()
 
     else:  # pragma: no cover
         warnings.warn(
-            "Plumbum does not know the type of the current OS for term size, defaulting to UNIX"
+            "Plumbum does not know the type of the current OS for term size, defaulting to UNIX",
+            stacklevel=2,
         )
         size = _get_terminal_size_linux()
 
-    if (
-        size is None
-    ):  # we'll assume the standard 80x25 if for any reason we don't know the terminal size
-        size = default
+    # we'll assume the standard 80x25 if for any reason we don't know the terminal size
+    if size is None:
+        return default
     return size
 
 
 def _get_terminal_size_windows():  # pragma: no cover
     try:
         from ctypes import create_string_buffer, windll
```

### Comparing `plumbum-1.8.1/plumbum/cli/i18n/de.po` & `plumbum-1.8.2/plumbum/cli/i18n/de.po`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/cli/i18n/fr.po` & `plumbum-1.8.2/plumbum/cli/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/cli/i18n/nl.po` & `plumbum-1.8.2/plumbum/cli/i18n/nl.po`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/cli/i18n/ru.po` & `plumbum-1.8.2/plumbum/cli/i18n/ru.po`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/cli/i18n/de/LC_MESSAGES/plumbum.cli.mo` & `plumbum-1.8.2/plumbum/cli/i18n/de/LC_MESSAGES/plumbum.cli.mo`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/cli/i18n/fr/LC_MESSAGES/plumbum.cli.mo` & `plumbum-1.8.2/plumbum/cli/i18n/fr/LC_MESSAGES/plumbum.cli.mo`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/cli/i18n/nl/LC_MESSAGES/plumbum.cli.mo` & `plumbum-1.8.2/plumbum/cli/i18n/nl/LC_MESSAGES/plumbum.cli.mo`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/cli/i18n/ru/LC_MESSAGES/plumbum.cli.mo` & `plumbum-1.8.2/plumbum/cli/i18n/ru/LC_MESSAGES/plumbum.cli.mo`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/colorlib/__init__.py` & `plumbum-1.8.2/plumbum/colorlib/__init__.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/colorlib/_ipython_ext.py` & `plumbum-1.8.2/plumbum/colorlib/_ipython_ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from io import StringIO
 
 import IPython.display
 from IPython.core.magic import Magics, cell_magic, magics_class, needs_local_scope
 
-valid_choices = [x[8:] for x in dir(IPython.display) if "display_" == x[:8]]
+valid_choices = [x[8:] for x in dir(IPython.display) if x[:8] == "display_"]
 
 
 @magics_class
 class OutputMagics(Magics):  # pragma: no cover
     @needs_local_scope
     @cell_magic
     def to(self, line, cell, local_ns=None):
```

### Comparing `plumbum-1.8.1/plumbum/colorlib/factories.py` & `plumbum-1.8.2/plumbum/colorlib/factories.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/colorlib/names.py` & `plumbum-1.8.2/plumbum/colorlib/names.py`

 * *Files 3% similar despite different names*

```diff
@@ -314,33 +314,33 @@
 )
 color_html = _base_html + _normal_html + _grey_html
 
 color_codes_simple = list(range(8)) + list(range(60, 68))
 """Simple colors, remember that reset is #9, second half is non as common."""
 
 # Attributes
-attributes_ansi = dict(
-    bold=1,
-    dim=2,
-    italics=3,
-    underline=4,
-    reverse=7,
-    hidden=8,
-    strikeout=9,
-)
+attributes_ansi = {
+    "bold": 1,
+    "dim": 2,
+    "italics": 3,
+    "underline": 4,
+    "reverse": 7,
+    "hidden": 8,
+    "strikeout": 9,
+}
 
 # Stylesheet
-default_styles = dict(
-    warn="fg red",
-    title="fg cyan underline bold",
-    fatal="fg red bold",
-    highlight="bg yellow",
-    info="fg blue",
-    success="fg green",
-)
+default_styles = {
+    "warn": "fg red",
+    "title": "fg cyan underline bold",
+    "fatal": "fg red bold",
+    "highlight": "bg yellow",
+    "info": "fg blue",
+    "success": "fg green",
+}
 
 # Functions to be used for color name operations
 
 
 class FindNearest:
     """This is a class for finding the nearest color given rgb values.
     Different find methods are available."""
```

### Comparing `plumbum-1.8.1/plumbum/colorlib/styles.py` & `plumbum-1.8.2/plumbum/colorlib/styles.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,15 +342,15 @@
 
     attribute_names: Union[Dict[str, str], Dict[str, int]]
 
     _stdout: Optional[IO] = None
     end = "\n"
     """The endline character. Override if needed in subclasses."""
 
-    ANSI_REG = re.compile("\033" + r"\[([\d;]+)m")
+    ANSI_REG = re.compile("\033\\[([\\d;]+)m")
     """The regular expression that finds ansi codes in a string."""
 
     @property
     def stdout(self):
         """\
         This property will allow custom, class level control of stdout.
         It will use current sys.stdout if set to None (default).
@@ -381,16 +381,15 @@
         if len(invalid_attributes) > 0:
             raise AttributeNotFound(
                 "Attribute(s) not valid: " + ", ".join(invalid_attributes)
             )
 
     @classmethod
     def from_color(cls, color):
-        self = cls(fgcolor=color) if color.fg else cls(bgcolor=color)
-        return self
+        return cls(fgcolor=color) if color.fg else cls(bgcolor=color)
 
     def invert(self):
         """This resets current color(s) and flips the value of all
         attributes present"""
 
         other = self.__class__()
 
@@ -571,15 +570,14 @@
         if self.isreset:
             string = "reset"
         return f"<{name}: {string}>"
 
     def __eq__(self, other):
         """Equality is true only if reset, or if attributes, fg, and bg match."""
         if type(self) == type(other):
-
             if self.isreset:
                 return other.isreset
 
             return (
                 self.attributes == other.attributes
                 and self.fg == other.fg
                 and self.bg == other.bg
@@ -733,42 +731,41 @@
 
 
 class HTMLStyle(Style):
     """This was meant to be a demo of subclassing Style, but
     actually can be a handy way to quickly color html text."""
 
     __slots__ = ()
-    attribute_names = dict(
-        bold="b",
-        em="em",
-        italics="i",
-        li="li",
-        underline='span style="text-decoration: underline;"',
-        code="code",
-        ol="ol start=0",
-        strikeout="s",
-    )
+    attribute_names = {
+        "bold": "b",
+        "em": "em",
+        "italics": "i",
+        "li": "li",
+        "underline": 'span style="text-decoration: underline;"',
+        "code": "code",
+        "ol": "ol start=0",
+        "strikeout": "s",
+    }
     end = "<br/>\n"
 
     def __str__(self):
-
         if self.isreset:
             raise ResetNotSupported("HTML does not support global resets!")
 
         result = ""
 
         if self.bg and not self.bg.isreset:
             result += f'<span style="background-color: {self.bg.hex_code}">'
         if self.fg and not self.fg.isreset:
             result += f'<font color="{self.fg.hex_code}">'
         for attr in sorted(self.attributes):
             if self.attributes[attr]:
                 result += "<" + self.attribute_names[attr] + ">"
 
-        for attr in reversed(sorted(self.attributes)):
+        for attr in sorted(self.attributes, reverse=True):
             if not self.attributes[attr]:
                 result += "</" + self.attribute_names[attr].split(" ")[0] + ">"
         if self.fg and self.fg.isreset:
             result += "</font>"
         if self.bg and self.bg.isreset:
             result += "</span>"
```

### Comparing `plumbum-1.8.1/plumbum/commands/__init__.py` & `plumbum-1.8.2/plumbum/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/commands/base.py` & `plumbum-1.8.2/plumbum/commands/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,19 +373,19 @@
     def __repr__(self):
         return f"Pipeline({self.srccmd!r}, {self.dstcmd!r})"
 
     def _get_encoding(self):
         return self.srccmd._get_encoding() or self.dstcmd._get_encoding()
 
     def formulate(self, level=0, args=()):
-        return (
-            self.srccmd.formulate(level + 1)
-            + ["|"]
-            + self.dstcmd.formulate(level + 1, args)
-        )
+        return [
+            *self.srccmd.formulate(level + 1),
+            "|",
+            *self.dstcmd.formulate(level + 1, args),
+        ]
 
     @property
     def machine(self):
         return self.srccmd.machine
 
     def popen(self, args=(), **kwargs):
         src_kwargs = kwargs.copy()
@@ -418,20 +418,18 @@
 
         dstproc_verify = dstproc.verify
 
         def verify(proc, retcode, timeout, stdout, stderr):
             # TODO: right now it's impossible to specify different expected
             # return codes for different stages of the pipeline
             try:
-                or_retcode = [0] + list(retcode)
+                or_retcode = [0, *list(retcode)]
             except TypeError:
-                if retcode is None:
-                    or_retcode = None  # no-retcode-verification acts "greedily"
-                else:
-                    or_retcode = [0, retcode]
+                # no-retcode-verification acts "greedily"
+                or_retcode = None if retcode is None else [0, retcode]
             proc.srcproc.verify(or_retcode, timeout, stdout, stderr)
             dstproc_verify(retcode, timeout, stdout, stderr)
 
         dstproc.verify = MethodType(verify, dstproc)
 
         dstproc.stdin = srcproc.stdin
         return dstproc
@@ -450,15 +448,16 @@
     def _get_encoding(self):
         return self.cmd._get_encoding()
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.cmd!r}, {self.file!r})"
 
     def formulate(self, level=0, args=()):
-        return self.cmd.formulate(level + 1, args) + [
+        return [
+            *self.cmd.formulate(level + 1, args),
             self.SYM,
             shquote(getattr(self.file, "name", self.file)),
         ]
 
     @property
     def machine(self):
         return self.cmd.machine
```

### Comparing `plumbum-1.8.1/plumbum/commands/daemons.py` & `plumbum-1.8.2/plumbum/commands/daemons.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/commands/modifiers.py` & `plumbum-1.8.2/plumbum/commands/modifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,15 +325,15 @@
 
 class _NOHUP(ExecutionModifier):
     """
     An execution modifier that runs the given command in the background, disconnected
     from the current process, returning a
     standard popen object. It will keep running even if you close the current process.
     In order to slightly mimic shell syntax, it applies
-    when you right-and it with a command. If you wish to use a diffent working directory
+    when you right-and it with a command. If you wish to use a different working directory
     or different stdout, stderr, you can use named arguments. The default is ``NOHUP(
     cwd=local.cwd, stdout='nohup.out', stderr=None)``. If stderr is None, stderr will be
     sent to stdout. Use ``os.devnull`` for null output. Will respect redirected output.
     Example::
 
         sleep[5] & NOHUP                       # Outputs to nohup.out
         sleep[5] & NOHUP(stdout=os.devnull)    # No output
@@ -386,15 +386,15 @@
             line_timeout=self.line_timeout, mode=BY_TYPE, **self.kw
         ):
             if not lines:
                 continue
             level = self.levels[typ]
             for line in lines.splitlines():
                 if self.prefix:
-                    line = f"{self.prefix}: {line}"
+                    line = f"{self.prefix}: {line}"  # noqa: PLW2901
                 self.log(level, line)
         return popen.returncode
 
 
 class PipeToLoggerMixin:
     """
     This mixin allows piping plumbum commands' output into a logger.
```

### Comparing `plumbum-1.8.1/plumbum/commands/processes.py` & `plumbum-1.8.2/plumbum/commands/processes.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,33 +95,28 @@
     while True:
         try:
             yield queue.get_nowait()
         except QueueEmpty:
             break
 
 
-if IS_WIN32:
-    _iter_lines = _iter_lines_win32
-else:
-    _iter_lines = _iter_lines_posix
+_iter_lines = _iter_lines_win32 if IS_WIN32 else _iter_lines_posix
 
 
 # ===================================================================================================
 # Exceptions
 # ===================================================================================================
 class ProcessExecutionError(OSError):
     """Represents the failure of a process. When the exit code of a terminated process does not
     match the expected result, this exception is raised by :func:`run_proc
     <plumbum.commands.run_proc>`. It contains the process' return code, stdout, and stderr, as
     well as the command line used to create the process (``argv``)
     """
 
-    # pylint: disable-next=super-init-not-called
     def __init__(self, argv, retcode, stdout, stderr, message=None, *, host=None):
-
         # we can't use 'super' here since OSError only keeps the first 2 args,
         # which leads to failuring in loading this object from a pickle.dumps.
         # pylint: disable-next=non-parent-init-called
         Exception.__init__(self, argv, retcode, stdout, stderr)
 
         self.message = message
         self.host = host
@@ -252,15 +247,15 @@
 
 def _register_proc_timeout(proc, timeout):
     if timeout is not None:
         _timeout_queue.put((proc, time.time() + timeout))
 
 
 def _shutdown_bg_threads():
-    global _shutting_down  # pylint: disable=global-statement
+    global _shutting_down  # noqa: PLW0603
     _shutting_down = True
     # Make sure this still exists (don't throw error in atexit!)
     # TODO: not sure why this would be "falsey", though
     if _timeout_queue:  # type: ignore[truthy-bool]
         _timeout_queue.put((SystemExit, 0))
         # grace period
         bgthd.join(0.1)
@@ -366,15 +361,14 @@
     encoding = getattr(proc, "custom_encoding", None) or "utf-8"
     decode = lambda s: s.decode(encoding, errors="replace").rstrip()  # noqa: E731
 
     _register_proc_timeout(proc, timeout)
 
     buffers = [[], []]
     for t, line in _iter_lines(proc, decode, linesize, line_timeout):
-
         # verify that the proc hasn't timed out yet
         proc.verify(timeout=timeout, retcode=None, stdout=None, stderr=None)
 
         buffer = buffers[t]
         if buffer_size > 0:
             buffer.append(line)
             if buffer_size < math.inf:
```

### Comparing `plumbum-1.8.1/plumbum/fs/atomic.py` & `plumbum-1.8.2/plumbum/fs/atomic.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,23 +123,22 @@
         :param blocking: if ``True``, the call will block until we can grab the file system lock.
                          if ``False``, the call may fail immediately with the underlying exception
                          (``IOError`` or ``WindowsError``)
         """
         if self._owned_by == threading.get_ident():
             yield
             return
-        with self._thdlock:
-            with locked_file(self._fileobj.fileno(), blocking):
-                if not self.path.exists() and not self._ignore_deletion:
-                    raise ValueError("Atomic file removed from filesystem")
-                self._owned_by = threading.get_ident()
-                try:
-                    yield
-                finally:
-                    self._owned_by = None
+        with self._thdlock, locked_file(self._fileobj.fileno(), blocking):
+            if not self.path.exists() and not self._ignore_deletion:
+                raise ValueError("Atomic file removed from filesystem")
+            self._owned_by = threading.get_ident()
+            try:
+                yield
+            finally:
+                self._owned_by = None
 
     def delete(self):
         """
         Atomically delete the file (holds the lock while doing it)
         """
         with self.locked():
             self.path.delete()
@@ -229,18 +228,15 @@
 
     def next(self):
         """
         Read and increment the counter, returning its previous value
         """
         with self.atomicfile.locked():
             curr = self.atomicfile.read_atomic().decode("utf8")
-            if not curr:
-                curr = self.initial
-            else:
-                curr = int(curr)
+            curr = self.initial if not curr else int(curr)
             self.atomicfile.write_atomic(str(curr + 1).encode("utf8"))
             return curr
 
 
 class PidFileTaken(SystemExit):
     """
     This exception is raised when PidFile.acquire fails to lock the pid file. Note that it
@@ -297,17 +293,16 @@
                 pid = self.atomicfile.read_shared().strip().decode("utf8")
             except OSError:
                 pid = "Unknown"
             raise PidFileTaken(
                 f"PID file {self.atomicfile.path!r} taken by process {pid}",
                 pid,
             ) from None
-        else:
-            self.atomicfile.write_atomic(str(os.getpid()).encode("utf8"))
-            atexit.register(self.release)
+        self.atomicfile.write_atomic(str(os.getpid()).encode("utf8"))
+        atexit.register(self.release)
 
     def release(self):
         """
         Release the PID file (should only happen when the program terminates)
         """
         if self._ctx is None:
             return
```

### Comparing `plumbum-1.8.1/plumbum/fs/mounts.py` & `plumbum-1.8.2/plumbum/fs/mounts.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/plumbum/machines/_windows.py` & `plumbum-1.8.2/plumbum/machines/_windows.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,13 @@
             return None
         f.seek(LFANEW_OFFSET)
         lfanew = struct.unpack("L", f.read(4))[0]
         f.seek(lfanew)
         if f.read(4) != b"PE\x00\x00":
             return None
         f.seek(FILE_HEADER_SIZE + SUBSYSTEM_OFFSET, 1)
-        subsystem = struct.unpack("H", f.read(2))[0]
-        return subsystem
+        return struct.unpack("H", f.read(2))[0]
 
 
 # print(get_pe_subsystem("c:\\windows\\notepad.exe")) == 2
 # print(get_pe_subsystem("c:\\python32\\python.exe")) == 3
 # print(get_pe_subsystem("c:\\python32\\pythonw.exe")) == 2
```

### Comparing `plumbum-1.8.1/plumbum/machines/base.py` & `plumbum-1.8.2/plumbum/machines/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,16 +59,15 @@
         """Tests for the existence of the command, e.g., ``"ls" in plumbum.local``.
         ``cmd`` can be anything acceptable by ``__getitem__``.
         """
         try:
             self[cmd]
         except CommandNotFound:
             return False
-        else:
-            return True
+        return True
 
     @property
     def encoding(self):
         "This is a wrapper for custom_encoding"
         return self.custom_encoding
 
     @encoding.setter
```

### Comparing `plumbum-1.8.1/plumbum/machines/env.py` & `plumbum-1.8.2/plumbum/machines/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,9 +179,8 @@
             if name in self:
                 return self[name]
         try:
             # POSIX only
             import pwd
         except ImportError:
             return None
-        else:
-            return pwd.getpwuid(os.getuid())[0]  # @UndefinedVariable
+        return pwd.getpwuid(os.getuid())[0]  # @UndefinedVariable
```

### Comparing `plumbum-1.8.1/plumbum/machines/local.py` & `plumbum-1.8.2/plumbum/machines/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,17 +145,18 @@
     uname = platform.uname()[0]
     _program_cache: Dict[Tuple[str, str], LocalPath] = {}
 
     def __init__(self):
         self._as_user_stack = []
 
     if IS_WIN32:
-        _EXTENSIONS = [""] + env.get("PATHEXT", ":.exe:.bat").lower().split(
-            os.path.pathsep
-        )
+        _EXTENSIONS = [
+            "",
+            *env.get("PATHEXT", ":.exe:.bat").lower().split(os.path.pathsep),
+        ]
 
         @classmethod
         def _which(cls, progname):
             progname = progname.lower()
             for p in cls.env.path:
                 for ext in cls._EXTENSIONS:
                     fn = p / (progname + ext)
@@ -213,16 +214,15 @@
         return LocalPath(os.path.join(*parts2))
 
     def __contains__(self, cmd):
         try:
             self[cmd]
         except CommandNotFound:
             return False
-        else:
-            return True
+        return True
 
     def __getitem__(self, cmd):
         """Returns a `Command` object representing the given program. ``cmd`` can be a string or
         a :class:`LocalPath <plumbum.path.local.LocalPath>`; if it is a path, a command
         representing this path will be returned; otherwise, the program name will be looked up
         in the system's ``PATH`` (using ``which``). Usage::
 
@@ -422,20 +422,20 @@
                     ],
                     self.which("runas"),
                 )
             )
         else:
             if username is None:
                 self._as_user_stack.append(
-                    lambda argv: (["sudo"] + list(argv), self.which("sudo"))
+                    lambda argv: (["sudo", *list(argv)], self.which("sudo"))
                 )
             else:
                 self._as_user_stack.append(
                     lambda argv: (
-                        ["sudo", "-u", username] + list(argv),
+                        ["sudo", "-u", username, *list(argv)],
                         self.which("sudo"),
                     )
                 )
         try:
             yield
         finally:
             self._as_user_stack.pop(-1)
```

### Comparing `plumbum-1.8.1/plumbum/machines/paramiko_machine.py` & `plumbum-1.8.2/plumbum/machines/paramiko_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,16 @@
         self.returncode = None
         self.pid = None
         self.stdin_file = stdin_file
         self.stdout_file = stdout_file
         self.stderr_file = stderr_file
 
     def poll(self):
-        if self.returncode is None:
-            if self.channel.exit_status_ready():
-                return self.wait()
+        if self.returncode is None and self.channel.exit_status_ready():
+            return self.wait()
         return self.returncode
 
     def wait(self):
         if self.returncode is None:
             self.channel.recv_exit_status()
             self.returncode = self.channel.exit_status
             self.close()
@@ -282,15 +281,21 @@
         files directly, much like an interactive FTP/SFTP session
         """
         if not self._sftp:
             self._sftp = self._client.open_sftp()
         return self._sftp
 
     def session(
-        self, isatty=False, term="vt100", width=80, height=24, *, new_session=False
+        self,
+        isatty=False,
+        term="vt100",
+        width=80,
+        height=24,
+        *,
+        new_session=False,  # noqa: ARG002
     ):
         # new_session is ignored for ParamikoMachine
         trans = self._client.get_transport()
         trans.set_keepalive(self._keep_alive)
         chan = trans.open_session()
         if isatty:
             chan.get_pty(term, width, height)
@@ -304,15 +309,15 @@
 
     def popen(
         self,
         args,
         stdin=None,
         stdout=None,
         stderr=None,
-        new_session=False,  # pylint: disable=unused-argument
+        new_session=False,  # noqa: ARG002
         env=None,
         cwd=None,
     ):
         # new_session is ignored for ParamikoMachine
         argv = []
         envdelta = self.env.getdelta()
         if env:
@@ -475,19 +480,18 @@
 
 
 ###################################################################################################
 # Custom iter_lines for paramiko.Channel
 ###################################################################################################
 def _iter_lines(
     proc,
-    decode,  # pylint: disable=unused-argument
+    decode,  # noqa: ARG001
     linesize,
     line_timeout=None,
 ):
-
     from selectors import EVENT_READ, DefaultSelector
 
     # Python 3.4+ implementation
     def selector():
         sel = DefaultSelector()
         sel.register(proc.stdout.channel, EVENT_READ)
         while True:
```

### Comparing `plumbum-1.8.1/plumbum/machines/remote.py` & `plumbum-1.8.2/plumbum/machines/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,16 @@
         """A command that represents the default remote python interpreter"""
         if not self._python:
             self._python = self["python3"]
         return self._python
 
     def session(self, isatty=False, *, new_session=False):
         """Creates a new :class:`ShellSession <plumbum.session.ShellSession>` object; this invokes the user's
-        shell on the remote machine and executes commands on it over stdin/stdout/stderr"""
+        shell on the remote machine and executes commands on it over stdin/stdout/stderr
+        """
         raise NotImplementedError()
 
     def download(self, src, dst):
         """Downloads a remote file/directory (``src``) to a local destination (``dst``).
         ``src`` must be a string or a :class:`RemotePath <plumbum.path.remote.RemotePath>`
         pointing to this remote machine, and ``dst`` must be a string or a
         :class:`LocalPath <plumbum.machines.local.LocalPath>`"""
@@ -375,15 +376,15 @@
         else:
             stat_cmd = "stat -f '%HT,%Xp,%i,%d,%l,%u,%g,%z,%a,%m,%c' "
         rc, out, _ = self._session.run(stat_cmd + shquote(fn), retcode=None)
         if rc != 0:
             return None
         statres = out.strip().split(",")
         text_mode = statres.pop(0).lower()
-        res = StatRes((int(statres[0], 16),) + tuple(int(sr) for sr in statres[1:]))
+        res = StatRes((int(statres[0], 16), *tuple(int(sr) for sr in statres[1:])))
         res.text_mode = text_mode
         return res
 
     def _path_delete(self, fn):
         self._session.run(f"rm -rf {shquote(fn)}")
 
     def _path_move(self, src, dst):
@@ -391,15 +392,15 @@
 
     def _path_copy(self, src, dst):
         self._session.run(f"cp -r {shquote(src)} {shquote(dst)}")
 
     def _path_mkdir(
         self,
         fn,
-        mode=None,  # pylint: disable=unused-argument
+        mode=None,  # noqa: ARG002
         minus_p=True,
     ):
         p_str = "-p " if minus_p else ""
         cmd = f"mkdir {p_str}{shquote(fn)}"
         self._session.run(cmd)
 
     def _path_chmod(self, mode, fn):
@@ -420,15 +421,15 @@
             args.append(f":{group}")
         args.append(shquote(fn))
         self._session.run(" ".join(args))
 
     def _path_read(self, fn):
         data = self["cat"](fn)
         if self.custom_encoding and isinstance(data, str):
-            data = data.encode(self.custom_encoding)
+            return data.encode(self.custom_encoding)
         return data
 
     def _path_write(self, fn, data):
         if self.custom_encoding and isinstance(data, str):
             data = data.encode(self.custom_encoding)
         with NamedTemporaryFile() as f:
             f.write(data)
```

### Comparing `plumbum-1.8.1/plumbum/machines/session.py` & `plumbum-1.8.2/plumbum/machines/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def __init__(self, pipe, marker):
         self.pipe = pipe
         self.marker = marker
         self.marker = bytes(self.marker, "ascii")
 
     def close(self):
-        """'Closes' the marked pipe; following calls to ``readline`` will return """ ""
+        """'Closes' the marked pipe; following calls to ``readline`` will return "" """
         # consume everything
         while self.readline():
             pass
         self.pipe = None
 
     def readline(self):
         """Reads the next line from the pipe; returns "" when the special marker is reached.
@@ -61,15 +61,15 @@
         if self.pipe is None:
             return b""
         line = self.pipe.readline()
         if not line:
             raise EOFError()
         if line.strip() == self.marker:
             self.pipe = None
-            line = b""
+            return b""
         return line
 
 
 class SessionPopen(PopenAddons):
     """A shell-session-based ``Popen``-like object (has the following attributes: ``stdin``,
     ``stdout``, ``stderr``, ``returncode``)"""
 
@@ -273,18 +273,15 @@
         :returns: A :class:`SessionPopen <plumbum.session.SessionPopen>` instance
         """
         if self.proc is None:
             raise ShellSessionError("Shell session has already been closed")
         if self._current and not self._current._done:
             raise ShellSessionError("Each shell may start only one process at a time")
 
-        if isinstance(cmd, BaseCommand):
-            full_cmd = cmd.formulate(1)
-        else:
-            full_cmd = cmd
+        full_cmd = cmd.formulate(1) if isinstance(cmd, BaseCommand) else cmd
         marker = f"--.END{time.time() * random.random()}.--"
         if full_cmd.strip():
             full_cmd += " ; "
         else:
             full_cmd = "true ; "
         full_cmd += f"echo $? ; echo '{marker}'"
         if not self.isatty:
```

### Comparing `plumbum-1.8.1/plumbum/machines/ssh_machine.py` & `plumbum-1.8.2/plumbum/machines/ssh_machine.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,15 +123,14 @@
         ssh_opts=(),
         scp_opts=(),
         password=None,
         encoding="utf8",
         connect_timeout=10,
         new_session=False,
     ):
-
         if ssh_command is None:
             if password is not None:
                 ssh_command = local["sshpass"]["-p", password, "ssh"]
             else:
                 ssh_command = local["ssh"]
         if scp_command is None:
             if password is not None:
@@ -192,15 +191,19 @@
 
     def nohup(self, command):
         """
         Runs the given command using ``nohup`` and redirects std handles,
         allowing the command to run "detached" from its controlling TTY or parent.
         Does not return anything. Depreciated (use command.nohup or daemonic_popen).
         """
-        warnings.warn("Use .nohup on the command or use daemonic_popen)", FutureWarning)
+        warnings.warn(
+            "Use .nohup on the command or use daemonic_popen)",
+            FutureWarning,
+            stacklevel=2,
+        )
         self.daemonic_popen(command, cwd=".", stdout=None, stderr=None, append=False)
 
     def daemonic_popen(self, command, cwd=".", stdout=None, stderr=None, append=True):
         """
         Runs the given command using ``nohup`` and redirects std handles,
         allowing the command to run "detached" from its controlling TTY or parent.
         Does not return anything.
@@ -209,18 +212,15 @@
 
         """
         if stdout is None:
             stdout = "/dev/null"
         if stderr is None:
             stderr = "&1"
 
-        if str(cwd) == ".":
-            args = []
-        else:
-            args = ["cd", str(cwd), "&&"]
+        args = [] if str(cwd) == "." else ["cd", str(cwd), "&&"]
         args.append("nohup")
         args.extend(command.formulate())
         args.extend(
             [
                 (">>" if append else ">") + str(stdout),
                 "2" + (">>" if (append and stderr != "&1") else ">") + str(stderr),
                 "</dev/null",
@@ -251,15 +251,15 @@
 
     def tunnel(
         self,
         lport,
         dport,
         lhost="localhost",
         dhost="localhost",
-        connect_timeout=5,  # pylint: disable=unused-argument
+        connect_timeout=5,  # noqa: ARG002
         reverse=False,
     ):
         r"""Creates an SSH tunnel from the TCP port (``lport``) of the local machine
         (``lhost``, defaults to ``"localhost"``, but it can be any IP you can ``bind()``)
         to the remote TCP port (``dport``) of the destination machine (``dhost``, defaults
         to ``"localhost"``, which means *this remote machine*). This function also
         supports Unix sockets, in which case the local socket should be passed in as
@@ -328,19 +328,20 @@
                 proc, self.custom_encoding, connect_timeout=self.connect_timeout
             ),
             lport,
             dport,
             reverse,
         )
 
-    def _translate_drive_letter(self, path):  # pylint: disable=no-self-use
+    @staticmethod
+    def _translate_drive_letter(path):
         # replace c:\some\path with /c/some/path
         path = str(path)
         if ":" in path:
-            path = "/" + path.replace(":", "").replace("\\", "/")
+            return "/" + path.replace(":", "").replace("\\", "/")
         return path
 
     def download(self, src, dst):
         if isinstance(src, LocalPath):
             raise TypeError(f"src of download cannot be {src!r}")
         if isinstance(src, RemotePath) and src.remote != self:
             raise TypeError(f"src {src!r} points to a different remote machine")
@@ -392,15 +393,15 @@
             scp_command = local["pscp"]
         if not ssh_opts:
             ssh_opts = ["-ssh"]
         if user is None:
             user = local.env.user
         if port is not None:
             ssh_opts.extend(["-P", str(port)])
-            scp_opts = list(scp_opts) + ["-P", str(port)]
+            scp_opts = [*list(scp_opts), "-P", str(port)]
             port = None
         SshMachine.__init__(
             self,
             host,
             user,
             port,
             keyfile=keyfile,
```

### Comparing `plumbum-1.8.1/plumbum/path/base.py` & `plumbum-1.8.2/plumbum/path/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import io
 import itertools
 import operator
 import os
+import typing
 import warnings
 from abc import ABC, abstractmethod
 from functools import reduce
 
 FLAGS = {"f": os.F_OK, "w": os.W_OK, "r": os.R_OK, "x": os.X_OK}
 
 
@@ -16,26 +18,29 @@
 
     def __new__(cls, val, name=None):
         self = int.__new__(cls, val)
         self.name = name
         return self
 
 
+_PathImpl = typing.TypeVar("_PathImpl", bound="Path")
+
+
 class Path(str, ABC):
     """An abstraction over file system paths. This class is abstract, and the two implementations
     are :class:`LocalPath <plumbum.machines.local.LocalPath>` and
     :class:`RemotePath <plumbum.path.remote.RemotePath>`.
     """
 
     CASE_SENSITIVE = True
 
     def __repr__(self):
         return f"<{self.__class__.__name__} {self}>"
 
-    def __truediv__(self, other):
+    def __truediv__(self: _PathImpl, other: typing.Any) -> _PathImpl:
         """Joins two paths"""
         return self.join(other)
 
     def __getitem__(self, key):
         if type(key) == str or isinstance(key, Path):
             return self / key
         return str(self)[key]
@@ -44,15 +49,15 @@
         """Returns a (possibly empty) list of paths that matched the glob-pattern under this path"""
         return self.glob(expr)
 
     def __iter__(self):
         """Iterate over the files in this directory"""
         return iter(self.list())
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         if isinstance(other, Path):
             return self._get_info() == other._get_info()
         if isinstance(other, str):
             if self.CASE_SENSITIVE:
                 return str(self) == other
 
             return str(self).lower() == other.lower()
@@ -88,25 +93,25 @@
         """Paths should support checking to see if an file or folder is in them."""
         try:
             return (self / item.name).exists()
         except AttributeError:
             return (self / item).exists()
 
     @abstractmethod
-    def _form(self, *parts):
+    def _form(self: _PathImpl, *parts: typing.Any) -> _PathImpl:
         pass
 
     def up(self, count=1):
         """Go up in ``count`` directories (the default is 1)"""
         return self.join("../" * count)
 
     def walk(
         self,
-        filter=lambda p: True,  # pylint: disable=redefined-builtin
-        dir_filter=lambda p: True,
+        filter=lambda _: True,  # pylint: disable=redefined-builtin
+        dir_filter=lambda _: True,
     ):
         """traverse all (recursive) sub-elements under this directory, that match the given filter.
         By default, the filter accepts everything; you can provide a custom filter function that
         takes a path as an argument and returns a boolean
 
         :param filter: the filter (predicate function) for matching results. Only paths matching
                        this predicate are returned. Defaults to everything.
@@ -117,140 +122,144 @@
             if filter(p):
                 yield p
             if p.is_dir() and dir_filter(p):
                 yield from p.walk(filter, dir_filter)
 
     @property
     @abstractmethod
-    def name(self):
+    def name(self) -> str:
         """The basename component of this path"""
 
     @property
     def basename(self):
         """Included for compatibility with older Plumbum code"""
-        warnings.warn("Use .name instead", FutureWarning)
+        warnings.warn("Use .name instead", FutureWarning, stacklevel=2)
         return self.name
 
     @property
     @abstractmethod
-    def stem(self):
+    def stem(self) -> str:
         """The name without an extension, or the last component of the path"""
 
     @property
     @abstractmethod
-    def dirname(self):
+    def dirname(self: _PathImpl) -> _PathImpl:
         """The dirname component of this path"""
 
     @property
     @abstractmethod
-    def root(self):
+    def root(self) -> str:
         """The root of the file tree (`/` on Unix)"""
 
     @property
     @abstractmethod
-    def drive(self):
+    def drive(self) -> str:
         """The drive letter (on Windows)"""
 
     @property
     @abstractmethod
-    def suffix(self):
+    def suffix(self) -> str:
         """The suffix of this file"""
 
     @property
     @abstractmethod
-    def suffixes(self):
+    def suffixes(self) -> typing.List[str]:
         """This is a list of all suffixes"""
 
     @property
     @abstractmethod
-    def uid(self):
+    def uid(self) -> FSUser:
         """The user that owns this path. The returned value is a :class:`FSUser <plumbum.path.FSUser>`
         object which behaves like an ``int`` (as expected from ``uid``), but it also has a ``.name``
         attribute that holds the string-name of the user"""
 
     @property
     @abstractmethod
-    def gid(self):
+    def gid(self) -> FSUser:
         """The group that owns this path. The returned value is a :class:`FSUser <plumbum.path.FSUser>`
         object which behaves like an ``int`` (as expected from ``gid``), but it also has a ``.name``
         attribute that holds the string-name of the group"""
 
     @abstractmethod
-    def as_uri(self, scheme=None):
+    def as_uri(self, scheme: typing.Optional[str] = None) -> str:
         """Returns a universal resource identifier. Use ``scheme`` to force a scheme."""
 
     @abstractmethod
-    def _get_info(self):
+    def _get_info(self) -> typing.Any:
         pass
 
     @abstractmethod
-    def join(self, *parts):
+    def join(self: _PathImpl, *parts: typing.Any) -> _PathImpl:
         """Joins this path with any number of paths"""
 
     @abstractmethod
-    def list(self):
+    def list(self: _PathImpl) -> typing.List[_PathImpl]:
         """Returns the files in this directory"""
 
     @abstractmethod
-    def iterdir(self):
+    def iterdir(self: _PathImpl) -> typing.Iterable[_PathImpl]:
         """Returns an iterator over the directory. Might be slightly faster on Python 3.5 than .list()"""
 
     @abstractmethod
-    def is_dir(self):
+    def is_dir(self) -> bool:
         """Returns ``True`` if this path is a directory, ``False`` otherwise"""
 
     def isdir(self):
         """Included for compatibility with older Plumbum code"""
-        warnings.warn("Use .is_dir() instead", FutureWarning)
+        warnings.warn("Use .is_dir() instead", FutureWarning, stacklevel=2)
         return self.is_dir()
 
     @abstractmethod
-    def is_file(self):
+    def is_file(self) -> bool:
         """Returns ``True`` if this path is a regular file, ``False`` otherwise"""
 
-    def isfile(self):
+    def isfile(self) -> bool:
         """Included for compatibility with older Plumbum code"""
-        warnings.warn("Use .is_file() instead", FutureWarning)
+        warnings.warn("Use .is_file() instead", FutureWarning, stacklevel=2)
         return self.is_file()
 
     def islink(self):
         """Included for compatibility with older Plumbum code"""
-        warnings.warn("Use is_symlink instead", FutureWarning)
+        warnings.warn("Use is_symlink instead", FutureWarning, stacklevel=2)
         return self.is_symlink()
 
     @abstractmethod
-    def is_symlink(self):
+    def is_symlink(self) -> bool:
         """Returns ``True`` if this path is a symbolic link, ``False`` otherwise"""
 
     @abstractmethod
-    def exists(self):
+    def exists(self) -> bool:
         """Returns ``True`` if this path exists, ``False`` otherwise"""
 
     @abstractmethod
-    def stat(self):
+    def stat(self) -> os.stat_result:
         """Returns the os.stats for a file"""
 
     @abstractmethod
-    def with_name(self, name):
+    def with_name(self: _PathImpl, name: typing.Any) -> _PathImpl:
         """Returns a path with the name replaced"""
 
     @abstractmethod
-    def with_suffix(self, suffix, depth=1):
+    def with_suffix(
+        self: _PathImpl, suffix: str, depth: typing.Optional[int] = 1
+    ) -> _PathImpl:
         """Returns a path with the suffix replaced. Up to last ``depth`` suffixes will be
         replaced. None will replace all suffixes. If there are less than ``depth`` suffixes,
         this will replace all suffixes. ``.tar.gz`` is an example where ``depth=2`` or
         ``depth=None`` is useful"""
 
     def preferred_suffix(self, suffix):
         """Adds a suffix if one does not currently exist (otherwise, no change). Useful
         for loading files with a default suffix"""
         return self if len(self.suffixes) > 0 else self.with_suffix(suffix)
 
     @abstractmethod
-    def glob(self, pattern):
+    def glob(
+        self: _PathImpl, pattern: typing.Union[str, typing.Iterable[str]]
+    ) -> typing.List[_PathImpl]:
         """Returns a (possibly empty) list of paths that matched the glob-pattern under this path"""
 
     @abstractmethod
     def delete(self):
         """Deletes this path (recursively, if a directory)"""
 
     @abstractmethod
@@ -285,24 +294,26 @@
 
         Note that the defaults for ``parents`` and ``exist_ok`` are the opposite of what they are in
         Python's own ``pathlib`` - this is to maintain backwards-compatibility with Plumbum's behaviour
         from before they were implemented.
         """
 
     @abstractmethod
-    def open(self, mode="r", *, encoding=None):
+    def open(
+        self, mode: str = "r", *, encoding: typing.Optional[str] = None
+    ) -> io.IOBase:
         """opens this path as a file"""
 
     @abstractmethod
-    def read(self, encoding=None):
+    def read(self, encoding: typing.Optional[str] = None) -> str:
         """returns the contents of this file as a ``str``. By default the data is read
         as text, but you can specify the encoding, e.g., ``'latin1'`` or ``'utf8'``"""
 
     @abstractmethod
-    def write(self, data, encoding=None):
+    def write(self, data: typing.AnyStr, encoding: typing.Optional[str] = None) -> None:
         """writes the given data to this file. By default the data is written as-is
         (either text or binary), but you can specify the encoding, e.g., ``'latin1'``
         or ``'utf8'``"""
 
     @abstractmethod
     def touch(self):
         """Update the access time. Creates an empty file if none exists."""
@@ -327,20 +338,20 @@
 
     @staticmethod
     def _access_mode_to_flags(mode, flags=None):
         if flags is None:
             flags = FLAGS
 
         if isinstance(mode, str):
-            mode = reduce(operator.or_, [flags[m] for m in mode.lower()], 0)
+            return reduce(operator.or_, [flags[m] for m in mode.lower()], 0)
 
         return mode
 
     @abstractmethod
-    def access(self, mode=0):
+    def access(self, mode: typing.Union[int, str] = 0) -> bool:
         """Test file existence or permission bits
 
         :param mode: a bitwise-or of access bits, or a string-representation thereof:
                      ``'f'``, ``'x'``, ``'r'``, ``'w'`` for ``os.F_OK``, ``os.X_OK``,
                      ``os.R_OK``, ``os.W_OK``
         """
 
@@ -372,15 +383,15 @@
             parts.append(path.name)
             path = path.dirname
         return parts[::-1]
 
     @property
     def parts(self):
         """Splits the directory into parts, including the base directory, returns a tuple"""
-        return tuple([self.drive + self.root] + self.split())
+        return (self.drive + self.root, *self.split())
 
     def relative_to(self, source):
         """Computes the "relative path" require to get from ``source`` to ``self``. They satisfy the invariant
         ``source_path + (target_path - source_path) == target_path``. For example::
 
             /var/log/messages - /var/log/messages = []
             /var/log/messages - /var              = [log, messages]
@@ -409,15 +420,15 @@
             return fn(pattern)
 
         results = []
         for single_pattern in pattern:
             results.extend(fn(single_pattern))
         return sorted(list(set(results)))
 
-    def resolve(self, strict=False):  # pylint:disable=unused-argument
+    def resolve(self, strict=False):  # noqa: ARG002
         """Added to allow pathlib like syntax. Does nothing since
         Plumbum paths are always absolute. Does not (currently) resolve
         symlinks."""
         # TODO: Resolve symlinks here
         return self
 
     @property
```

### Comparing `plumbum-1.8.1/plumbum/path/local.py` & `plumbum-1.8.2/plumbum/path/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,18 +49,17 @@
             and not isinstance(parts[0], LocalWorkdir)
         ):
             return parts[0]
         if not parts:
             raise TypeError("At least one path part is required (none given)")
         if any(isinstance(path, RemotePath) for path in parts):
             raise TypeError(f"LocalPath cannot be constructed from {parts!r}")
-        self = super().__new__(
+        return super().__new__(
             cls, os.path.normpath(os.path.join(*(str(p) for p in parts)))
         )
-        return self
 
     @property
     def _path(self):
         return str(self)
 
     def _get_info(self):
         return self._path
@@ -212,25 +211,22 @@
 
     def read(self, encoding=None, mode="r"):
         if encoding and "b" not in mode:
             mode = mode + "b"
         with self.open(mode) as f:
             data = f.read()
             if encoding:
-                data = data.decode(encoding)
+                return data.decode(encoding)
             return data
 
     def write(self, data, encoding=None, mode=None):
         if encoding:
             data = data.encode(encoding)
         if mode is None:
-            if isinstance(data, str):
-                mode = "w"
-            else:
-                mode = "wb"
+            mode = "w" if isinstance(data, str) else "wb"
         with self.open(mode) as f:
             f.write(data)
 
     def touch(self):
         with open(str(self), "a", encoding="utf-8"):
             os.utime(str(self), None)
```

### Comparing `plumbum-1.8.1/plumbum/path/remote.py` & `plumbum-1.8.2/plumbum/path/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         # Simple skip if path is absolute
         if parts[0] and parts[0][0] not in ("/", "\\"):
             cwd = (
                 remote._cwd
                 if hasattr(remote, "_cwd")
                 else remote._session.run("pwd")[1].strip()
             )
-            parts = (cwd,) + parts
+            parts = (cwd, *parts)
 
         for p in parts:
             if windows:
                 plist = str(p).replace("\\", "/").split("/")
             else:
                 plist = str(p).split("/")
             if not plist[0]:
@@ -233,15 +233,15 @@
                     raise OSError(
                         errno.EEXIST, "File exists (on remote end)", str(self)
                     ) from None
 
     def read(self, encoding=None):
         data = self.remote._path_read(self)
         if encoding:
-            data = data.decode(encoding)
+            return data.decode(encoding)
         return data
 
     def write(self, data, encoding=None):
         if encoding:
             data = data.encode(encoding)
         self.remote._path_write(self, data)
 
@@ -319,16 +319,15 @@
         return ""
 
 
 class RemoteWorkdir(RemotePath):
     """Remote working directory manipulator"""
 
     def __new__(cls, remote):
-        self = super().__new__(cls, remote, remote._session.run("pwd")[1].strip())
-        return self
+        return super().__new__(cls, remote, remote._session.run("pwd")[1].strip())
 
     def __hash__(self):
         raise TypeError("unhashable type")
 
     def chdir(self, newdir):
         """Changes the current working directory to the given one"""
         self.remote._session.run(f"cd {shquote(newdir)}")
```

### Comparing `plumbum-1.8.1/plumbum/path/utils.py` & `plumbum-1.8.2/plumbum/path/utils.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/tests/conftest.py` & `plumbum-1.8.2/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         ot_run = list(itertools.chain.from_iterable(a.split(",") for a in ot_run))
     else:
         ot_run = config.inicfg.get("run_optional_tests", [])
         if ot_run:
             ot_run = list(re.split(r"[,\s]+", ot_run))
     ot_run = set(ot_run)
 
-    _logger.info("optional tests to run:", ot_run)
+    _logger.info("optional tests to run: %s", ot_run)
     if ot_run:
         unknown_tests = ot_run - ot_markers
         if unknown_tests:
             raise ValueError(
                 "Requested execution of undeclared optional tests: {}".format(
                     ", ".join(unknown_tests)
                 )
```

### Comparing `plumbum-1.8.1/tests/test_3_cli.py` & `plumbum-1.8.2/tests/test_3_cli.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/tests/test_cli.py` & `plumbum-1.8.2/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,15 @@
 @Geet.subcommand("commit")
 class GeetCommit(cli.Application):
     message = cli.Flag("-m", str)
 
     def main(self):
         if self.parent.debug:
             return "committing in debug"
-        else:
-            return "committing"
+        return "committing"
 
     def cleanup(self, retcode):
         self.parent.cleanups.append(2)
         print(f"geet commit cleaning up with rc = {retcode}")
 
 
 class Sample(cli.Application):
@@ -233,15 +232,14 @@
         assert rc == 2
 
         _, rc = SimpleApp.run(["foo", "--bacon=hello"], exit=False)
         assert rc == 2
 
     # Testing #371
     def test_extra_args(self, capsys):
-
         _, rc = PositionalApp.run(["positionalapp"], exit=False)
         assert rc != 0
         stdout, stderr = capsys.readouterr()
         assert "Expected at least" in stdout
 
         _, rc = PositionalApp.run(["positionalapp", "one"], exit=False)
         assert rc == 0
@@ -294,15 +292,15 @@
             pass
         else:
             # Paragraph indentation should be preserved
             assert "    ABC" in stdout
             assert "  DEF" in stdout
             assert "   - Item" in stdout
             # List items should not be combined into paragraphs
-            assert "  * Star 2"
+            assert "  * Star 2" in stdout
             # Lines of the same list item should be combined. (The right-hand expression of the 'or' operator
             # below is for when the terminal is too narrow, causing "GHI" to be wrapped to the next line.)
             assert "  GHI" not in stdout or "     GHI" in stdout
             # List item with invisible bullet should be indented without the bullet
             assert " XYZ" in stdout
 
     def test_default_main(self, capsys):
@@ -363,15 +361,14 @@
 
         assert rc == 0
         stdout, stderr = capsys.readouterr()
         assert "20" in stdout
         assert inst.eggs == "raw"
 
     def test_mandatory_env_var(self, capsys):
-
         _, rc = SimpleApp.run(["arg"], exit=False)
         assert rc == 2
         stdout, stderr = capsys.readouterr()
         assert "bacon is mandatory" in stdout
 
     def test_partial_switches(self, capsys):
         app = SimpleApp
```

### Comparing `plumbum-1.8.1/tests/test_clicolor.py` & `plumbum-1.8.2/tests/test_clicolor.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/tests/test_color.py` & `plumbum-1.8.2/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/tests/test_config.py` & `plumbum-1.8.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/tests/test_env.py` & `plumbum-1.8.2/tests/test_env.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+import contextlib
+
 from plumbum import local
 from plumbum._testtools import skip_on_windows
 
-try:
+with contextlib.suppress(ModuleNotFoundError):
     from plumbum.cmd import printenv
-except ImportError:
-    pass
 
 
 @skip_on_windows
 class TestEnv:
     def test_change_env(self):
         with local.env(silly=12):
-            assert 12 == local.env["silly"]
+            assert local.env["silly"] == 12
             actual = {x.split("=")[0] for x in printenv().splitlines() if "=" in x}
             localenv = {x[0] for x in local.env}
             print(actual, localenv)
             assert localenv == actual
             assert len(local.env) == len(actual)
 
     def test_dictlike(self):
@@ -39,15 +39,15 @@
         with local.env():
             local.env["simple_plum"] = "thing"
             assert "simple_plum" in local.env
             del local.env["simple_plum"]
             assert "simple_plum" not in local.env
             local.env["simple_plum"] = "thing"
             assert "simple_plum" in local.env
-            assert "thing" == local.env.pop("simple_plum")
+            assert local.env.pop("simple_plum") == "thing"
             assert "simple_plum" not in local.env
             local.env["simple_plum"] = "thing"
         assert "simple_plum" not in local.env
 
     @skip_on_windows
     def test_home(self):
         assert local.env.home == local.env["HOME"]
```

### Comparing `plumbum-1.8.1/tests/test_local.py` & `plumbum-1.8.2/tests/test_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,44 +30,42 @@
 
 # This is a string since we are testing local paths
 SDIR = os.path.dirname(os.path.abspath(__file__))
 
 
 class TestLocalPopen:
     def test_contextmanager(self):
-        if IS_WIN32:
-            command = ["dir"]
-        else:
-            command = ["ls"]
+        command = ["dir"] if IS_WIN32 else ["ls"]
         with PlumbumLocalPopen(command):
             pass
 
 
 class TestLocalPath:
     longpath = local.path("/some/long/path/to/file.txt")
 
     def test_name(self):
         name = self.longpath.name
         assert isinstance(name, str)
-        assert "file.txt" == str(name)
+        assert str(name) == "file.txt"
 
     def test_dirname(self):
         name = self.longpath.dirname
         assert isinstance(name, LocalPath)
-        assert "/some/long/path/to" == str(name).replace("\\", "/").lstrip("C:").lstrip(
-            "D:"
+        assert (
+            str(name).replace("\\", "/").lstrip("C:").lstrip("D:")
+            == "/some/long/path/to"
         )
 
     def test_uri(self):
         if IS_WIN32:
             pth = self.longpath.as_uri()
             assert pth.startswith("file:///")
             assert pth.endswith(":/some/long/path/to/file.txt")
         else:
-            assert "file:///some/long/path/to/file.txt" == self.longpath.as_uri()
+            assert self.longpath.as_uri() == "file:///some/long/path/to/file.txt"
 
     def test_pickle(self):
         path1 = local.path(".")
         path2 = local.path("~")
         assert pickle.loads(pickle.dumps(self.longpath)) == self.longpath
         assert pickle.loads(pickle.dumps(path1)) == path1
         assert pickle.loads(pickle.dumps(path2)) == path2
@@ -322,17 +320,15 @@
         assert "test_local.py" in local["ls"]().splitlines()
         assert "test_local.py" in ls().splitlines()
 
         with pytest.raises(CommandNotFound):
             local["non_exist1N9"]()
 
         with pytest.raises(ImportError):
-            from plumbum.cmd import non_exist1N9
-
-            assert non_exist1N9
+            from plumbum.cmd import non_exist1N9  # noqa: F401
 
     def test_pathlib(self):
         ls_path = Path(local.which("ls"))
         assert "test_local.py" in local[ls_path]().splitlines()
 
     def test_get(self):
         assert str(local["ls"]) == str(local.get("ls"))
@@ -343,25 +339,24 @@
         with pytest.raises(CommandNotFound):
             local.get("non_exist1N9", "non_exist1N8")
         with pytest.raises(CommandNotFound):
             local.get("non_exist1N9", "/tmp/non_exist1N8")
 
     def test_shadowed_by_dir(self):
         real_ls = local["ls"]
-        with local.tempdir() as tdir:
-            with local.cwd(tdir):
-                ls_dir = tdir / "ls"
-                ls_dir.mkdir()
-                fake_ls = local["ls"]
-                assert fake_ls.executable == real_ls.executable
-
-                local.env.path.insert(0, tdir)
-                fake_ls = local["ls"]
-                del local.env.path[0]
-                assert fake_ls.executable == real_ls.executable
+        with local.tempdir() as tdir, local.cwd(tdir):
+            ls_dir = tdir / "ls"
+            ls_dir.mkdir()
+            fake_ls = local["ls"]
+            assert fake_ls.executable == real_ls.executable
+
+            local.env.path.insert(0, tdir)
+            fake_ls = local["ls"]
+            del local.env.path[0]
+            assert fake_ls.executable == real_ls.executable
 
     def test_repr_command(self):
         assert "BG" in repr(BG)
         assert "FG" in repr(FG)
 
     @skip_on_windows
     def test_cwd(self):
@@ -526,15 +521,15 @@
     @skip_on_windows
     def test_pipe_stderr(self, capfd):
         from plumbum.cmd import cat, head
 
         cat["/dev/urndom"] & FG(1)
         assert "urndom" in capfd.readouterr()[1]
 
-        assert "" == capfd.readouterr()[1]
+        assert capfd.readouterr()[1] == ""
 
         (cat["/dev/urndom"] | head["-c", "10"]) & FG(retcode=1)
         assert "urndom" in capfd.readouterr()[1]
 
     @skip_on_windows
     def test_fair_error_attribution(self):
         # use LocalCommand directly for predictable argv
@@ -545,69 +540,69 @@
         assert e.value.argv == ["false"]
 
     @skip_on_windows
     def test_iter_lines_timeout(self):
         from plumbum.cmd import bash
 
         cmd = bash["-ce", "for ((i=0;1==1;i++)); do echo $i; sleep .3; done"]
-        with pytest.raises(ProcessTimedOut):
+        with pytest.raises(ProcessTimedOut):  # noqa: PT012
             for i, (out, err) in enumerate(cmd.popen().iter_lines(timeout=1)):
                 assert not err
                 assert out
                 print(i, "out:", out)
         assert i in (2, 3)  # Mac is a bit flakey
 
     @skip_on_windows
     def test_iter_lines_buffer_size(self):
         from plumbum.cmd import bash
 
         cmd = bash["-ce", "for ((i=0;i<100;i++)); do echo $i; done; false"]
-        with pytest.raises(ProcessExecutionError) as e:
+        with pytest.raises(ProcessExecutionError) as e:  # noqa: PT012
             for _ in cmd.popen().iter_lines(timeout=1, buffer_size=5):
                 pass
         assert e.value.stdout == "\n".join(map(str, range(95, 100))) + "\n"
 
     @skip_on_windows
     def test_iter_lines_timeout_by_type(self):
         from plumbum.cmd import bash
         from plumbum.commands.processes import BY_TYPE
 
         cmd = bash[
             "-ce", "for ((i=0;1==1;i++)); do echo $i; sleep .3; echo $i 1>&2; done"
         ]
         types = {1: "out:", 2: "err:"}
         counts = {1: 0, 2: 0}
-        with pytest.raises(ProcessTimedOut):
+        with pytest.raises(ProcessTimedOut):  # noqa: PT012
             # Order is important on mac
             for typ, line in cmd.popen().iter_lines(timeout=1, mode=BY_TYPE):
                 counts[typ] += 1
                 print(types[typ], line)
         assert counts[1] in (3, 4)  # Mac is a bit flakey
         assert counts[2] in (2, 3)  # Mac is a bit flakey
 
     @skip_on_windows
     def test_iter_lines_error(self):
         from plumbum.cmd import ls
 
-        with pytest.raises(ProcessExecutionError) as err:
+        with pytest.raises(ProcessExecutionError) as err:  # noqa: PT012
             for i, _lines in enumerate(ls["--bla"].popen()):  # noqa: B007
                 pass
             assert i == 1
         assert (
             "ls: unrecognized option" in err.value.stderr
             and "--bla" in err.value.stderr
         ) or "ls: illegal option -- -" in err.value.stderr
 
     @skip_on_windows
     def test_iter_lines_line_timeout(self):
         from plumbum.cmd import bash
 
         cmd = bash["-ce", "for ((i=0;1==1;i++)); do echo $i; sleep $i; done"]
 
-        with pytest.raises(ProcessLineTimedOut):
+        with pytest.raises(ProcessLineTimedOut):  # noqa: PT012
             # Order is important on mac
             for i, (out, err) in enumerate(cmd.popen().iter_lines(line_timeout=0.2)):
                 print(i, "out:", out)
                 print(i, "err:", err)
         assert i == 1
 
     @skip_on_windows
@@ -628,29 +623,29 @@
 
     @skip_on_windows
     def test_tee_modifier(self, capfd):
         from plumbum.cmd import echo
 
         result = echo["This is fun"] & TEE
         assert result[1] == "This is fun\n"
-        assert "This is fun\n" == capfd.readouterr()[0]
+        assert capfd.readouterr()[0] == "This is fun\n"
 
     @skip_on_windows
     def test_tee_race(self, capfd):
         from plumbum.cmd import seq
 
         EXPECT = "".join(f"{i}\n" for i in range(1, 5001))
         for _ in range(5):
             result = seq["1", "5000"] & TEE
             assert result[1] == EXPECT
-            assert EXPECT == capfd.readouterr()[0]
+            assert capfd.readouterr()[0] == EXPECT
 
     @skip_on_windows
     @pytest.mark.parametrize(
-        "modifier, expected",
+        ("modifier", "expected"),
         [
             (FG, None),
             (TF(FG=True), True),
             (RETCODE(FG=True), 0),
             (TEE, (0, "meow", "")),
         ],
     )
@@ -810,15 +805,15 @@
     def test_list_processes(self):
         assert list(local.list_processes())
 
     def test_pgrep(self):
         assert list(local.pgrep("[pP]ython"))
 
     def _generate_sigint(self):
-        with pytest.raises(KeyboardInterrupt):
+        with pytest.raises(KeyboardInterrupt):  # noqa: PT012
             if sys.platform == "win32":
                 from win32api import GenerateConsoleCtrlEvent
 
                 GenerateConsoleCtrlEvent(0, 0)  # send Ctrl+C to current TTY
             else:
                 os.kill(0, signal.SIGINT)
             time.sleep(1)
@@ -1020,15 +1015,15 @@
 
     @skip_on_windows
     def test_run_tee(self, capfd):
         from plumbum.cmd import echo
 
         result = echo["This is fun"].run_tee()
         assert result[1] == "This is fun\n"
-        assert "This is fun\n" == capfd.readouterr()[0]
+        assert capfd.readouterr()[0] == "This is fun\n"
 
     def test_run_tf(self):
         from plumbum.cmd import ls
 
         f = ls["-l"].run_tf()
         assert f is True
```

### Comparing `plumbum-1.8.1/tests/test_nohup.py` & `plumbum-1.8.2/tests/test_nohup.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/tests/test_putty.py` & `plumbum-1.8.2/tests/test_putty.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/tests/test_remote.py` & `plumbum-1.8.2/tests/test_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,30 +55,30 @@
 
 
 @skip_on_windows
 def test_connection():
     SshMachine(TEST_HOST)
 
 
-def test_incorrect_login(sshpass):
+def test_incorrect_login(sshpass):  # noqa: ARG001
     with pytest.raises(IncorrectLogin):
         SshMachine(
             TEST_HOST,
             password="swordfish",
             ssh_opts=[
                 "-o",
                 "PubkeyAuthentication=no",
                 "-o",
                 "PreferredAuthentications=password",
             ],
         )
 
 
 @pytest.mark.xfail(env.LINUX, reason="TODO: no idea why this fails on linux")
-def test_hostpubkey_unknown(sshpass):
+def test_hostpubkey_unknown(sshpass):  # noqa: ARG001
     with pytest.raises(HostPublicKeyUnknown):
         SshMachine(
             TEST_HOST,
             password="swordfish",
             ssh_opts=["-o", "UserKnownHostsFile=/dev/null", "-o", "UpdateHostKeys=no"],
         )
 
@@ -87,26 +87,26 @@
 class TestRemotePath:
     def _connect(self):
         return SshMachine(TEST_HOST)
 
     def test_name(self):
         name = RemotePath(self._connect(), "/some/long/path/to/file.txt").name
         assert isinstance(name, str)
-        assert "file.txt" == str(name)
+        assert str(name) == "file.txt"
 
     def test_dirname(self):
         name = RemotePath(self._connect(), "/some/long/path/to/file.txt").dirname
         assert isinstance(name, RemotePath)
-        assert "/some/long/path/to" == str(name)
+        assert str(name) == "/some/long/path/to"
 
     def test_uri(self):
         p1 = RemotePath(self._connect(), "/some/long/path/to/file.txt")
-        assert "ftp://" == p1.as_uri("ftp")[:6]
-        assert "ssh://" == p1.as_uri("ssh")[:6]
-        assert "/some/long/path/to/file.txt" == p1.as_uri()[-27:]
+        assert p1.as_uri("ftp")[:6] == "ftp://"
+        assert p1.as_uri("ssh")[:6] == "ssh://"
+        assert p1.as_uri()[-27:] == "/some/long/path/to/file.txt"
 
     def test_stem(self):
         p = RemotePath(self._connect(), "/some/long/path/to/file.txt")
         assert p.stem == "file"
         p = RemotePath(self._connect(), "/some/long/path/")
         assert p.stem == "path"
 
@@ -144,23 +144,22 @@
         )
         strassert(
             p2.with_name("something.tar"), RemotePath(self._connect(), "something.tar")
         )
 
     @skip_without_chown
     def test_chown(self):
-        with self._connect() as rem:
-            with rem.tempdir() as dir:
-                p = dir / "foo.txt"
-                p.write(b"hello")
-                # because we're connected to localhost, we expect UID and GID to be the same
-                assert p.uid == os.getuid()
-                assert p.gid == os.getgid()
-                p.chown(p.uid.name)
-                assert p.uid == os.getuid()
+        with self._connect() as rem, rem.tempdir() as dir:
+            p = dir / "foo.txt"
+            p.write(b"hello")
+            # because we're connected to localhost, we expect UID and GID to be the same
+            assert p.uid == os.getuid()
+            assert p.gid == os.getgid()
+            p.chown(p.uid.name)
+            assert p.uid == os.getuid()
 
     def test_parent(self):
         p1 = RemotePath(self._connect(), "/some/long/path/to/file.txt")
         p2 = p1.parent
         assert str(p2) == "/some/long/path/to"
 
     def test_mkdir(self):
@@ -178,15 +177,15 @@
                     (tmp / "a").mkdir(exist_ok=False, parents=True)
                 (tmp / "b" / "bb").mkdir(exist_ok=False, parents=True)
                 assert (tmp / "b" / "bb").exists()
                 assert (tmp / "b" / "bb").is_dir()
             assert not tmp.exists()
 
     @pytest.mark.xfail(
-        reason="mkdir's mode argument is not yet implemented " "for remote paths",
+        reason="mkdir's mode argument is not yet implemented for remote paths",
         strict=True,
     )
     def test_mkdir_mode(self):
         # (identical to test_local.TestLocalPath.test_mkdir_mode)
         with self._connect() as rem:
             with rem.tempdir() as tmp:
                 # just verify that mode argument works the same way it does for
@@ -225,15 +224,14 @@
 
             * copying a directory `a_dir` over an existing directory path with
               `override=True` succeeds
         """
 
         with self._connect() as rem:
             with rem.tempdir() as tmp:
-
                 # setup a file and make sure it exists...
                 (tmp / "file_a").touch()
                 assert (tmp / "file_a").exists()
                 assert (tmp / "file_a").is_file()
 
                 # setup a directory for copying into...
                 (tmp / "a_dir").mkdir(exist_ok=False, parents=False)
@@ -318,28 +316,30 @@
         with self._connect() as rem:
             with rem.cwd(os.path.dirname(os.path.abspath(__file__))):
                 rem["ls"]()
             with rem.cwd("/tmp"):
                 rem["pwd"]()
 
     def test_glob(self):
-        with self._connect() as rem:
-            with rem.cwd(os.path.dirname(os.path.abspath(__file__))):
-                filenames = [f.name for f in rem.cwd // ("*.py", "*.bash")]
-                assert "test_remote.py" in filenames
-                assert "slow_process.bash" in filenames
+        with self._connect() as rem, rem.cwd(
+            os.path.dirname(os.path.abspath(__file__))
+        ):
+            filenames = [f.name for f in rem.cwd // ("*.py", "*.bash")]
+            assert "test_remote.py" in filenames
+            assert "slow_process.bash" in filenames
 
     def test_glob_spaces(self):
-        with self._connect() as rem:
-            with rem.cwd(os.path.dirname(os.path.abspath(__file__))):
-                filenames = [f.name for f in rem.cwd // ("*space.txt")]
-                assert "file with space.txt" in filenames
+        with self._connect() as rem, rem.cwd(
+            os.path.dirname(os.path.abspath(__file__))
+        ):
+            filenames = [f.name for f in rem.cwd // ("*space.txt")]
+            assert "file with space.txt" in filenames
 
-                filenames = [f.name for f in rem.cwd // ("*with space.txt")]
-                assert "file with space.txt" in filenames
+            filenames = [f.name for f in rem.cwd // ("*with space.txt")]
+            assert "file with space.txt" in filenames
 
     def test_cmd(self):
         with self._connect() as rem:
             rem.cmd.ls("/tmp")
 
     @pytest.mark.usefixtures("testdir")
     def test_download_upload(self):
@@ -429,19 +429,19 @@
             except ProcessTimedOut:
                 assert i > 3
             else:
                 pytest.fail("Expected a timeout")
 
     def test_iter_lines_error(self):
         with self._connect() as rem:
-            with pytest.raises(ProcessExecutionError) as ex:
+            with pytest.raises(ProcessExecutionError) as ex:  # noqa: PT012
                 for i, _lines in enumerate(rem["ls"]["--bla"].popen()):  # noqa: B007
                     pass
                 assert i == 1
-            assert "/bin/ls: " in ex.value.stderr
+            assert "ls: " in ex.value.stderr
 
     def test_touch(self):
         with self._connect() as rem:
             rfile = rem.cwd / "sillyfile"
             assert not rfile.exists()
             rfile.touch()
             assert rfile.exists()
@@ -462,29 +462,25 @@
 @skip_on_windows
 class TestRemoteMachine(BaseRemoteMachineTest):
     def _connect(self):
         return SshMachine(TEST_HOST)
 
     @pytest.mark.parametrize("dynamic_lport", [False, True])
     def test_tunnel(self, dynamic_lport):
-
         for tunnel_prog in (self.TUNNEL_PROG_AF_INET, self.TUNNEL_PROG_AF_UNIX):
             with self._connect() as rem:
                 p = (rem.python["-u"] << tunnel_prog).popen()
                 port_or_socket = p.stdout.readline().decode("ascii").strip()
                 try:
                     port_or_socket = int(port_or_socket)
                     dhost = "localhost"
                 except ValueError:
                     dhost = None
 
-                if not dynamic_lport:
-                    lport = 12222
-                else:
-                    lport = 0
+                lport = 12222 if not dynamic_lport else 0
 
                 with rem.tunnel(lport, port_or_socket, dhost=dhost) as tun:
                     if not dynamic_lport:
                         assert tun.lport == lport
                     else:
                         assert_is_port(tun.lport)
                     assert tun.dport == port_or_socket
@@ -497,24 +493,22 @@
                     s.close()
 
                 print(p.communicate())
                 assert data == b"hello world"
 
     @pytest.mark.parametrize("dynamic_dport", [False, True])
     def test_reverse_tunnel(self, dynamic_dport):
-
         lport = 12223 + dynamic_dport
         with self._connect() as rem:
             queue = Queue()
             tunnel_server = Thread(target=serve_reverse_tunnel, args=(queue, lport))
             tunnel_server.start()
             message = str(time.time())
 
             if not dynamic_dport:
-
                 get_unbound_socket_remote = """import sys, socket
 s = socket.socket()
 s.bind(("", 0))
 s.listen(1)
 sys.stdout.write(str(s.getsockname()[1]))
 sys.stdout.flush()
 s.close()
```

### Comparing `plumbum-1.8.1/tests/test_terminal.py` & `plumbum-1.8.2/tests/test_terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         assert (
             capsys.readouterr()[0]
             == "What is your favorite color?\n(1) blue\n(2) yellow\n(3) green\nChoice [2]: Invalid choice, please try again\nChoice [2]: "
         )
 
     def test_choose_dict(self):
         with send_stdin("23\n1"):
-            value = choose("Pick", dict(one="a", two="b"))
+            value = choose("Pick", {"one": "a", "two": "b"})
             assert value in ("a", "b")
 
     def test_ordered_dict(self):
         dic = OrderedDict()
         dic["one"] = "a"
         dic["two"] = "b"
         with send_stdin("1"):
```

### Comparing `plumbum-1.8.1/tests/test_typed_env.py` & `plumbum-1.8.2/tests/test_typed_env.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def test_env(self):
         class E(TypedEnv):
             terminal = TypedEnv.Str("TERM")
             B = TypedEnv.Bool("BOOL", default=True)
             I = TypedEnv.Int("INT INTEGER".split())  # noqa: E741  # noqa: E741
             INTS = TypedEnv.CSV("CS_INTS", type=int)
 
-        raw_env = dict(TERM="xterm", CS_INTS="1,2,3,4")
+        raw_env = {"TERM": "xterm", "CS_INTS": "1,2,3,4"}
         e = E(raw_env)
 
         assert e.terminal == "xterm"
         e.terminal = "foo"
         assert e.terminal == "foo"
         assert raw_env["TERM"] == "foo"
         assert "terminal" not in raw_env
@@ -31,29 +31,29 @@
 
         e.B = True
         assert raw_env["BOOL"] == "yes"
 
         e.B = False
         assert raw_env["BOOL"] == "no"
 
-        assert e.INTS == [1, 2, 3, 4]
+        assert [1, 2, 3, 4] == e.INTS
         e.INTS = [1, 2]
-        assert e.INTS == [1, 2]
+        assert [1, 2] == e.INTS
         e.INTS = [1, 2, 3, 4]
 
         with pytest.raises(KeyError):
-            e.I
+            e.I  # noqa: B018
 
         raw_env["INTEGER"] = "4"
-        assert e.I == 4  # noqa: E741
+        assert e.I == 4
         assert e["I"] == 4
 
-        e.I = "5"  # noqa: E741
+        e.I = "5"
         assert raw_env["INT"] == "5"
-        assert e.I == 5  # noqa: E741
+        assert e.I == 5
         assert e["I"] == 5
 
         assert "{I} {B} {terminal}".format(**e) == "5 False foo"
-        assert dict(e) == dict(I=5, B=False, terminal="foo", INTS=[1, 2, 3, 4])
+        assert dict(e) == {"I": 5, "B": False, "terminal": "foo", "INTS": [1, 2, 3, 4]}
 
         r = TypedEnv(raw_env)
         assert "{INT} {BOOL} {TERM}".format(**r) == "5 no foo"
```

### Comparing `plumbum-1.8.1/tests/test_utils.py` & `plumbum-1.8.2/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from plumbum import SshMachine, local
 from plumbum._testtools import skip_on_windows
 from plumbum.path.utils import copy, delete, move
 
 
 @skip_on_windows
-@pytest.mark.ssh
+@pytest.mark.ssh()
 def test_copy_move_delete():
     from plumbum.cmd import touch
 
     with local.tempdir() as dir:
         (dir / "orog").mkdir()
         (dir / "orog" / "rec").mkdir()
         for i in range(20):
@@ -22,35 +22,33 @@
 
         s1 = sorted(f.name for f in (dir / "orig").walk())
 
         copy(dir / "orig", dir / "dup")
         s2 = sorted(f.name for f in (dir / "dup").walk())
         assert s1 == s2
 
-        with SshMachine("localhost") as rem:
-            with rem.tempdir() as dir2:
-                copy(dir / "orig", dir2)
-                s3 = sorted(f.name for f in (dir2 / "orig").walk())
-                assert s1 == s3
-
-                copy(dir2 / "orig", dir2 / "dup")
-                s4 = sorted(f.name for f in (dir2 / "dup").walk())
-                assert s1 == s4
-
-                copy(dir2 / "dup", dir / "dup2")
-                s5 = sorted(f.name for f in (dir / "dup2").walk())
-                assert s1 == s5
-
-                with SshMachine("localhost") as rem2:
-                    with rem2.tempdir() as dir3:
-                        copy(dir2 / "dup", dir3)
-                        s6 = sorted(f.name for f in (dir3 / "dup").walk())
-                        assert s1 == s6
+        with SshMachine("localhost") as rem, rem.tempdir() as dir2:
+            copy(dir / "orig", dir2)
+            s3 = sorted(f.name for f in (dir2 / "orig").walk())
+            assert s1 == s3
+
+            copy(dir2 / "orig", dir2 / "dup")
+            s4 = sorted(f.name for f in (dir2 / "dup").walk())
+            assert s1 == s4
+
+            copy(dir2 / "dup", dir / "dup2")
+            s5 = sorted(f.name for f in (dir / "dup2").walk())
+            assert s1 == s5
+
+            with SshMachine("localhost") as rem2, rem2.tempdir() as dir3:
+                copy(dir2 / "dup", dir3)
+                s6 = sorted(f.name for f in (dir3 / "dup").walk())
+                assert s1 == s6
 
-                        move(dir3 / "dup", dir / "superdup")
-                        assert not (dir3 / "dup").exists()
+                move(dir3 / "dup", dir / "superdup")
+                assert not (dir3 / "dup").exists()
 
-                        s7 = sorted(f.name for f in (dir / "superdup").walk())
-                        assert s1 == s7
+                s7 = sorted(f.name for f in (dir / "superdup").walk())
+                assert s1 == s7
 
-                        # test rm
-                        delete(dir)
+                # test rm
+                delete(dir)
```

### Comparing `plumbum-1.8.1/tests/test_validate.py` & `plumbum-1.8.2/tests/test_validate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 from plumbum import cli
 
 
 class TestValidator:
     def test_named(self):
         class Try:
             @cli.positional(x=abs, y=str)
-            def main(selfy, x, y):  # noqa: B902
+            def main(selfy, x, y):
                 pass
 
         assert Try.main.positional == [abs, str]
         assert Try.main.positional_varargs is None
 
     def test_position(self):
         class Try:
             @cli.positional(abs, str)
-            def main(selfy, x, y):  # noqa: B902
+            def main(selfy, x, y):
                 pass
 
         assert Try.main.positional == [abs, str]
         assert Try.main.positional_varargs is None
 
     def test_mix(self):
         class Try:
             @cli.positional(abs, str, d=bool)
-            def main(selfy, x, y, z, d):  # noqa: B902
+            def main(selfy, x, y, z, d):
                 pass
 
         assert Try.main.positional == [abs, str, None, bool]
         assert Try.main.positional_varargs is None
 
     def test_var(self):
         class Try:
             @cli.positional(abs, str, int)
-            def main(selfy, x, y, *g):  # noqa: B902
+            def main(selfy, x, y, *g):
                 pass
 
         assert Try.main.positional == [abs, str]
         assert Try.main.positional_varargs is int
 
     def test_defaults(self):
         class Try:
             @cli.positional(abs, str)
-            def main(selfy, x, y="hello"):  # noqa: B902
+            def main(selfy, x, y="hello"):
                 pass
 
         assert Try.main.positional == [abs, str]
 
 
 class TestProg:
     def test_prog(self, capsys):
         class MainValidator(cli.Application):
             @cli.positional(int, int, int)
             def main(self, myint, myint2, *mylist):
                 print(repr(myint), myint2, mylist)
 
         _, rc = MainValidator.run(["prog", "1", "2", "3", "4", "5"], exit=False)
         assert rc == 0
-        assert "1 2 (3, 4, 5)" == capsys.readouterr()[0].strip()
+        assert capsys.readouterr()[0].strip() == "1 2 (3, 4, 5)"
 
     def test_failure(self, capsys):
         class MainValidator(cli.Application):
             @cli.positional(int, int, int)
             def main(self, myint, myint2, *mylist):
                 print(myint, myint2, mylist)
 
@@ -76,12 +76,12 @@
         class MainValidator(cli.Application):
             @cli.positional(int, int)
             def main(self, myint, myint2=2):
                 print(repr(myint), repr(myint2))
 
         _, rc = MainValidator.run(["prog", "1"], exit=False)
         assert rc == 0
-        assert "1 2" == capsys.readouterr()[0].strip()
+        assert capsys.readouterr()[0].strip() == "1 2"
 
         _, rc = MainValidator.run(["prog", "1", "3"], exit=False)
         assert rc == 0
-        assert "1 3" == capsys.readouterr()[0].strip()
+        assert capsys.readouterr()[0].strip() == "1 3"
```

### Comparing `plumbum-1.8.1/tests/test_visual_color.py` & `plumbum-1.8.2/tests/test_visual_color.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/.gitignore` & `plumbum-1.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/LICENSE` & `plumbum-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/README.rst` & `plumbum-1.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.1/pyproject.toml` & `plumbum-1.8.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "hatchling.build"
 
 
 [project]
 name = "plumbum"
 description = "Plumbum: shell combinators library"
 readme = "README.rst"
-author = { name="Tomer Filiba", email="tomerfiliba@gmail.com" }
+authors = [{ name="Tomer Filiba", email="tomerfiliba@gmail.com" }]
 license = { file="LICENSE" }
 requires-python = ">=3.6"
 dynamic = ["version"]
 dependencies = [
     "pywin32; platform_system=='Windows' and platform_python_implementation!='PyPy'",
 ]
 classifiers = [
@@ -26,14 +26,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Build Tools",
     "Topic :: System :: Systems Administration",
 ]
 keywords = [
     "path",
     "local",
     "remote",
@@ -43,14 +44,22 @@
     "popen",
     "process",
     "execution",
     "color",
     "cli",
 ]
 
+[project.urls]
+Homepage = "https://github.com/tomerfiliba/plumbum"
+Documentation = "https://plumbum.readthedocs.io/"
+"Bug Tracker" = "https://github.com/tomerfiliba/plumbum/issues"
+Changelog = "https://plumbum.readthedocs.io/en/latest/changelog.html"
+Cheatsheet = "https://plumbum.readthedocs.io/en/latest/quickref.html"
+
+
 [project.optional-dependencies]
 dev = [
     "paramiko",
     "psutil",
     "pytest>=6.0",
     "pytest-cov",
     "pytest-mock",
@@ -106,18 +115,14 @@
 timeout = 300
 optional_tests = """
   ssh: requires self ssh access to run
   sudo: requires sudo access to run
 """
 
 
-[tool.isort]
-profile = "black"
-
-
 [tool.pylint]
 master.py-version = "3.6"
 master.jobs = "0"
 master.load-plugins = ["pylint.extensions.no_self_use"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.enable = [
@@ -152,8 +157,52 @@
   "too-many-public-methods",
   "too-many-return-statements",
   "too-many-statements",
   "unidiomatic-typecheck", # TODO: might be able to remove
   "unnecessary-lambda-assignment", # TODO: 4 instances
   "unused-import", # identical to flake8 but has typing false positives
   "eval-used",  # Needed for Python <3.10 annotations
-]
+  "unused-argument", # Covered by ruff
+  "global-statement", # Covered by ruff
+  "pointless-statement", # Covered by ruff
+]
+
+[tool.ruff]
+select = [
+  "E", "F", "W", # flake8
+  "B", "B904",   # flake8-bugbear
+  "I",           # isort
+  "ARG",         # flake8-unused-arguments
+  "C4",          # flake8-comprehensions
+  "ICN",         # flake8-import-conventions
+  "ISC",         # flake8-implicit-str-concat
+  "PGH",         # pygrep-hooks
+  "PIE",         # flake8-pie
+  "PL",          # pylint
+  "PT",          # flake8-pytest-style
+  "RET",         # flake8-return
+  "RUF",         # Ruff-specific
+  "SIM",         # flake8-simplify
+  "T20",         # flake8-print
+  "UP",          # pyupgrade
+  "YTT",         # flake8-2020
+
+]
+extend-ignore = [
+  "E501",
+  "PLR",
+  "PT004",
+  "PT011",  # TODO: add match parameter
+  "PLC1901", # Simplify == "", might be risky
+]
+target-version = "py37"
+exclude = ["docs/conf.py"]
+mccabe.max-complexity = 50
+flake8-unused-arguments.ignore-variadic-names = true
+
+[tool.ruff.per-file-ignores]
+"examples/*" = ["T20"]
+"experiments/*" = ["T20"]
+"tests/*" = ["T20"]
+"plumbum/cli/application.py" = ["T20"]
+"plumbum/commands/base.py" = ["SIM115"]
+"plumbum/commands/daemons.py" = ["SIM115"]
```

### Comparing `plumbum-1.8.1/PKG-INFO` & `plumbum-1.8.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Metadata-Version: 2.1
 Name: plumbum
-Version: 1.8.1
+Version: 1.8.2
 Summary: Plumbum: shell combinators library
+Project-URL: Homepage, https://github.com/tomerfiliba/plumbum
+Project-URL: Documentation, https://plumbum.readthedocs.io/
+Project-URL: Bug Tracker, https://github.com/tomerfiliba/plumbum/issues
+Project-URL: Changelog, https://plumbum.readthedocs.io/en/latest/changelog.html
+Project-URL: Cheatsheet, https://plumbum.readthedocs.io/en/latest/quickref.html
+Author-email: Tomer Filiba <tomerfiliba@gmail.com>
 License: Copyright (c) 2013 Tomer Filiba (tomerfiliba@gmail.com)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
@@ -31,14 +37,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=3.6
 Requires-Dist: pywin32; platform_system == 'Windows' and platform_python_implementation != 'PyPy'
 Provides-Extra: dev
 Requires-Dist: paramiko; extra == 'dev'
 Requires-Dist: psutil; extra == 'dev'
```

