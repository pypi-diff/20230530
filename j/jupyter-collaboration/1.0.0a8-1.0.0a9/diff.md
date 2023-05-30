# Comparing `tmp/jupyter_collaboration-1.0.0a8.tar.gz` & `tmp/jupyter_collaboration-1.0.0a9.tar.gz`

## Comparing `jupyter_collaboration-1.0.0a8.tar` & `jupyter_collaboration-1.0.0a9.tar`

### file list

```diff
@@ -1,103 +1,108 @@
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.eslintrc.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.flake8
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.gitconfig
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.npmignore
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.prettierrc
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.readthedocs.yaml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.stylelintrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.yarnrc.yml
--rw-r--r--   0        0        0    38959 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/CHANGELOG.md
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/CONTRIBUTING.md
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/RELEASE.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/codecov.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/install.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/lerna.json
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/package.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/setup.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/tsconfig.json
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/tsconfig.test.json
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/typedoc.json
--rw-r--r--   0        0        0   488941 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/yarn.lock
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/Makefile
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/make.bat
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/conf.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/configuration.md
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/index.md
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/_static/jupyter_logo.svg
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/_static/logo-icon.png
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/developer/architecture.md
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/developer/contributing.rst
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/developer/javascript_api.rst
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/developer/python_api.rst
--rw-r--r--   0        0        0    61242 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/images/rtc_shared_cursors.png
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter-config/jupyter_collaboration.json
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/_version.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/app.py
--rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/handlers.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/loaders.py
--rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/rooms.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/stores.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/utils.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/package.json
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/user-menu-bar.json
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/413.cf154c48ecaa08648e56.js
--rw-r--r--   0        0        0    11162 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/493.0975334cbddac1bcf819.js
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/497.ab1a0ee570b8e4f31289.js
--rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/8.6b2a09634af3599cbddb.js
--rw-r--r--   0        0        0     8177 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/839.2efa17f8ec8b5c6c87a6.js
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/9.f46ff2dd7fa86c1246e8.js
--rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/933.f161fc3dcf0d2c141b27.js
--rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/remoteEntry.c7ae49e75d2022d8409a.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/style.js
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/scripts/bump_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/tests/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/tests/conftest.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/tests/test_ydoc.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/README.md
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/babel.config.js
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/tsconfig.json
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/collaboratorspanel.tsx
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/components.tsx
--rw-r--r--   0        0        0    11792 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/cursors.ts
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/index.ts
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/menu.ts
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/tokens.ts
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/userinfopanel.tsx
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/utils.ts
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/style/base.css
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/style/index.js
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/style/menu.css
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/style/sidepanel.css
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/README.md
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/tsconfig.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/schema/user-menu-bar.json
--rw-r--r--   0        0        0     5870 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/src/collaboration.ts
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/src/filebrowser.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/src/index.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/style/index.css
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/style/index.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/babel.config.js
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/jest.config.js
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/tsconfig.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/tsconfig.test.json
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/src/index.ts
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/src/requests.ts
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/src/tokens.ts
--rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/src/ydrive.ts
--rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/src/yprovider.ts
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/test/yprovider.spec.ts
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/LICENSE
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/README.md
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/pyproject.toml
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/PKG-INFO
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.eslintrc.js
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.flake8
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.gitconfig
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.licenserc.yaml
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.npmignore
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.prettierrc
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.readthedocs.yaml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.stylelintrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.yarnrc.yml
+-rw-r--r--   0        0        0    42584 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/CHANGELOG.md
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/CONTRIBUTING.md
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/RELEASE.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/codecov.yml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/install.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/lerna.json
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/package.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/setup.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/tsconfig.json
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/tsconfig.test.json
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/typedoc.json
+-rw-r--r--   0        0        0   488215 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/yarn.lock
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/Makefile
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/make.bat
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/conf.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/configuration.md
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/index.md
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/_static/jupyter_logo.svg
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/_static/logo-icon.png
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/developer/architecture.md
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/developer/contributing.rst
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/developer/javascript_api.rst
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/developer/python_api.rst
+-rw-r--r--   0        0        0    61242 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/images/rtc_shared_cursors.png
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter-config/jupyter_collaboration.json
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/_version.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/app.py
+-rw-r--r--   0        0        0    12505 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/handlers.py
+-rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/loaders.py
+-rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/rooms.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/stores.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/utils.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/websocketserver.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/events/session.yaml
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/package.json
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/shared-link.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/user-menu-bar.json
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/413.cf154c48ecaa08648e56.js
+-rw-r--r--   0        0        0    11162 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/493.efdf15c07c2318ee4cd7.js
+-rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/760.c3c71c52d5e0ace455c5.js
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/8.883cdb5327aeb22e2587.js
+-rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/839.14d748171b9c87a422f9.js
+-rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/87.c69c6c0210f40538f288.js
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/933.737bcc7ac7d9a6826f35.js
+-rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/remoteEntry.f78dd7195bd101ba931a.js
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/style.js
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/scripts/bump_version.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/tests/__init__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/tests/conftest.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/tests/test_loaders.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/README.md
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/tsconfig.json
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/collaboratorspanel.tsx
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/components.tsx
+-rw-r--r--   0        0        0    11792 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/cursors.ts
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/index.ts
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/menu.ts
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/sharedlink.ts
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/tokens.ts
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/userinfopanel.tsx
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/style/base.css
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/style/index.js
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/style/menu.css
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/style/sidepanel.css
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/README.md
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/tsconfig.json
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/schema/shared-link.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/schema/user-menu-bar.json
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/collaboration.ts
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/filebrowser.ts
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/index.ts
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/sharedlink.ts
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/style/index.css
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/style/index.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/babel.config.js
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/jest.config.js
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/package.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/tsconfig.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/tsconfig.test.json
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/src/index.ts
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/src/requests.ts
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/src/tokens.ts
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/src/ydrive.ts
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/src/yprovider.ts
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/src/__tests__/yprovider.spec.ts
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/LICENSE
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/README.md
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/pyproject.toml
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/PKG-INFO
```

### Comparing `jupyter_collaboration-1.0.0a8/.eslintrc.js` & `jupyter_collaboration-1.0.0a9/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/.pre-commit-config.yaml` & `jupyter_collaboration-1.0.0a9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/CHANGELOG.md` & `jupyter_collaboration-1.0.0a9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,48 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.0.0alpha9
+
+([Full Changelog](https://github.com/jupyterlab/jupyter_collaboration/compare/@jupyter/collaboration-extension@1.0.0-alpha.8...fbae4ff5054bf98507ac87429e0322c22be6b830))
+
+### Enhancements made
+
+- Add share link feature [#150](https://github.com/jupyterlab/jupyter_collaboration/pull/150) ([@fcollonval](https://github.com/fcollonval))
+- Improve code architecture [#146](https://github.com/jupyterlab/jupyter_collaboration/pull/146) ([@fcollonval](https://github.com/fcollonval))
+- Add logger for file editor [#145](https://github.com/jupyterlab/jupyter_collaboration/pull/145) ([@fcollonval](https://github.com/fcollonval))
+- Emit events for collaborative sessions [#139](https://github.com/jupyterlab/jupyter_collaboration/pull/139) ([@hbcarlos](https://github.com/hbcarlos))
+
+### Bugs fixed
+
+- Support file types [#154](https://github.com/jupyterlab/jupyter_collaboration/pull/154) ([@hbcarlos](https://github.com/hbcarlos))
+- Fix injecting user menu bar in top bar. [#149](https://github.com/jupyterlab/jupyter_collaboration/pull/149) ([@fcollonval](https://github.com/fcollonval))
+- Wait for the document to be synced [#148](https://github.com/jupyterlab/jupyter_collaboration/pull/148) ([@fcollonval](https://github.com/fcollonval))
+- Fix asyncio.Task type for python\<=3.8 [#143](https://github.com/jupyterlab/jupyter_collaboration/pull/143) ([@davidbrochart](https://github.com/davidbrochart))
+
+### Maintenance and upkeep improvements
+
+- Fix binder env [#152](https://github.com/jupyterlab/jupyter_collaboration/pull/152) ([@fcollonval](https://github.com/fcollonval))
+- Add license to files automatically [#147](https://github.com/jupyterlab/jupyter_collaboration/pull/147) ([@fcollonval](https://github.com/fcollonval))
+- Add JavaScript and lab extension test in CI [#144](https://github.com/jupyterlab/jupyter_collaboration/pull/144) ([@fcollonval](https://github.com/fcollonval))
+- Fix asyncio.Task type for python\<=3.8 [#143](https://github.com/jupyterlab/jupyter_collaboration/pull/143) ([@davidbrochart](https://github.com/davidbrochart))
+- Update lab [#141](https://github.com/jupyterlab/jupyter_collaboration/pull/141) ([@hbcarlos](https://github.com/hbcarlos))
+- Fix typo and punctuation [#140](https://github.com/jupyterlab/jupyter_collaboration/pull/140) ([@krassowski](https://github.com/krassowski))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab/jupyter_collaboration/graphs/contributors?from=2023-04-24&to=2023-05-30&type=c))
+
+[@codecov-commenter](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Acodecov-commenter+updated%3A2023-04-24..2023-05-30&type=Issues) | [@davidbrochart](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Adavidbrochart+updated%3A2023-04-24..2023-05-30&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Afcollonval+updated%3A2023-04-24..2023-05-30&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Agithub-actions+updated%3A2023-04-24..2023-05-30&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Ahbcarlos+updated%3A2023-04-24..2023-05-30&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Akrassowski+updated%3A2023-04-24..2023-05-30&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Awelcome+updated%3A2023-04-24..2023-05-30&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.0.0alpha8
 
 ([Full Changelog](https://github.com/jupyterlab/jupyter_collaboration/compare/@jupyter/collaboration-extension@1.0.0-alpha.7...2e5a6cc66961a5552e8a89c0850c7483c1e1acb2))
 
 ### Enhancements made
 
 - Follow up #133 [#136](https://github.com/jupyterlab/jupyter_collaboration/pull/136) ([@hbcarlos](https://github.com/hbcarlos))
@@ -27,16 +62,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlab/jupyter_collaboration/graphs/contributors?from=2023-03-29&to=2023-04-24&type=c))
 
 [@codecov-commenter](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Acodecov-commenter+updated%3A2023-03-29..2023-04-24&type=Issues) | [@davidbrochart](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Adavidbrochart+updated%3A2023-03-29..2023-04-24&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Afcollonval+updated%3A2023-03-29..2023-04-24&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Agithub-actions+updated%3A2023-03-29..2023-04-24&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Ahbcarlos+updated%3A2023-03-29..2023-04-24&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.0.0alpha7
 
 ([Full Changelog](https://github.com/jupyterlab/jupyter_collaboration/compare/@jupyter/collaboration-extension@1.0.0-alpha.6...9d8475f5cc333e22b50160ec32e508a4e8c75c06))
 
 ### Enhancements made
 
 - Allow other extensions to register shared models [#133](https://github.com/jupyterlab/jupyter_collaboration/pull/133) ([@hbcarlos](https://github.com/hbcarlos))
```

### Comparing `jupyter_collaboration-1.0.0a8/package.json` & `jupyter_collaboration-1.0.0a9/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9631696428571429%*

 * *Differences: {"'devDependencies'": "{'typescript': '~5.0.4'}", "'version'": "'1.0.0-alpha.9'"}*

```diff
@@ -19,15 +19,15 @@
         "prettier": "^2.8.4",
         "rimraf": "^4.1.2",
         "stylelint": "^15.2.0",
         "stylelint-config-recommended": "^10.0.0",
         "stylelint-config-standard": "^30.0.1",
         "stylelint-prettier": "^3.0.0",
         "typedoc": "~0.23.28",
-        "typescript": "~5.0.2"
+        "typescript": "~5.0.4"
     },
     "homepage": "https://github.com/jupyterlab/jupyter_collaboration",
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
@@ -59,14 +59,14 @@
         "stylelint:check": "stylelint --cache \"packages/**/style/**/*.css\"",
         "test": "lerna run test",
         "test:cov": "lerna run test:cov",
         "test:debug": "lerna run test:debug",
         "test:debug:watch": "lerna run test:debug:watch",
         "watch": "lerna run watch"
     },
-    "version": "1.0.0-alpha.8",
+    "version": "1.0.0-alpha.9",
     "workspaces": {
         "packages": [
             "packages/*"
         ]
     }
 }
```

### Comparing `jupyter_collaboration-1.0.0a8/typedoc.json` & `jupyter_collaboration-1.0.0a9/typedoc.json`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/yarn.lock` & `jupyter_collaboration-1.0.0a9/yarn.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1255,19 +1255,19 @@
   version: 0.8.0
   resolution: "@babel/regjsgen@npm:0.8.0"
   checksum: 89c338fee774770e5a487382170711014d49a68eb281e74f2b5eac88f38300a4ad545516a7786a8dd5702e9cf009c94c2f582d200f077ac5decd74c56b973730
   languageName: node
   linkType: hard
 
 "@babel/runtime@npm:^7.8.4":
-  version: 7.21.0
-  resolution: "@babel/runtime@npm:7.21.0"
+  version: 7.21.5
+  resolution: "@babel/runtime@npm:7.21.5"
   dependencies:
     regenerator-runtime: ^0.13.11
-  checksum: 7b33e25bfa9e0e1b9e8828bb61b2d32bdd46b41b07ba7cb43319ad08efc6fda8eb89445193e67d6541814627df0ca59122c0ea795e412b99c5183a0540d338ab
+  checksum: 358f2779d3187f5c67ad302e8f8d435412925d0b991d133c7d4a7b1ddd5a3fda1b6f34537cb64628dfd96a27ae46df105bed3895b8d754b88cacdded8d1129dd
   languageName: node
   linkType: hard
 
 "@babel/template@npm:^7.18.10, @babel/template@npm:^7.20.7, @babel/template@npm:^7.3.3":
   version: 7.20.7
   resolution: "@babel/template@npm:7.20.7"
   dependencies:
@@ -1310,66 +1310,67 @@
 "@bcoe/v8-coverage@npm:^0.2.3":
   version: 0.2.3
   resolution: "@bcoe/v8-coverage@npm:0.2.3"
   checksum: 850f9305536d0f2bd13e9e0881cb5f02e4f93fad1189f7b2d4bebf694e3206924eadee1068130d43c11b750efcc9405f88a8e42ef098b6d75239c0f047de1a27
   languageName: node
   linkType: hard
 
-"@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.4.0":
-  version: 6.4.2
-  resolution: "@codemirror/autocomplete@npm:6.4.2"
+"@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.5.1":
+  version: 6.6.1
+  resolution: "@codemirror/autocomplete@npm:6.6.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.6.0
     "@lezer/common": ^1.0.0
   peerDependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
-  checksum: c6cc4edb1c412153e6f6f27926674d7f1d386d1f30d6d4f60c5b52bfa0105870b0c70449b69891937bcf082340d8b0fa6d1f9f28f5eb60adc2974ed4c73aadc1
+  checksum: 5ce596f806626534d567d87ab22bbe3c69bb8540ab72f1702372ae533cb75ff1123f223df9953efb9ef8885ed15e938ac79ac94e5de21fe380bd08b87569ce7c
   languageName: node
   linkType: hard
 
-"@codemirror/commands@npm:^6.1.0":
-  version: 6.2.2
-  resolution: "@codemirror/commands@npm:6.2.2"
+"@codemirror/commands@npm:^6.2.3":
+  version: 6.2.4
+  resolution: "@codemirror/commands@npm:6.2.4"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
-  checksum: d3aa1ca8cbd7b9434eedba6b6d783411670796bf6ab61990afc4fd0c04645189fe4dd55bb95e23b943e9089f9739bc7e92aa4b2ac3eac09cfa2b91a45f608d3e
+  checksum: 468895fa19ff0554181b698c81f850820de5c0289cab92c44392fb127286f09ca72b921d6ea4353b70b616a4fd0c3667d86b6f917202a3ad2e196eb7b581f7b6
   languageName: node
   linkType: hard
 
-"@codemirror/lang-cpp@npm:^6.0.0":
+"@codemirror/lang-cpp@npm:^6.0.2":
   version: 6.0.2
   resolution: "@codemirror/lang-cpp@npm:6.0.2"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/cpp": ^1.0.0
   checksum: bb9eba482cca80037ce30c7b193cf45eff19ccbb773764fddf2071756468ecc25aa53c777c943635054f89095b0247b9b50c339e107e41e68d34d12a7295f9a9
   languageName: node
   linkType: hard
 
-"@codemirror/lang-css@npm:^6.0.0":
-  version: 6.1.1
-  resolution: "@codemirror/lang-css@npm:6.1.1"
+"@codemirror/lang-css@npm:^6.0.0, @codemirror/lang-css@npm:^6.1.1":
+  version: 6.2.0
+  resolution: "@codemirror/lang-css@npm:6.2.0"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
+    "@lezer/common": ^1.0.2
     "@lezer/css": ^1.0.0
-  checksum: 9b0bf7c7544fb604b67325689d783981e4099560f577bc1f10c52cb18e9d275ebdbdbd3f335a1dbb9c4910c36320f74ca015fc92ef99f930ecb9d481a2bf3511
+  checksum: d824f169083613b63f04992c24d3fecd45c718cd3deb9da3f332dd3a889a762d05ea812e31ddf7ee4b661722f8c8b49676515cb98609067c53e25ac8b469a5e4
   languageName: node
   linkType: hard
 
-"@codemirror/lang-html@npm:^6.0.0, @codemirror/lang-html@npm:^6.4.0":
+"@codemirror/lang-html@npm:^6.0.0, @codemirror/lang-html@npm:^6.4.3":
   version: 6.4.3
   resolution: "@codemirror/lang-html@npm:6.4.3"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/lang-css": ^6.0.0
     "@codemirror/lang-javascript": ^6.0.0
     "@codemirror/language": ^6.4.0
@@ -1378,122 +1379,122 @@
     "@lezer/common": ^1.0.0
     "@lezer/css": ^1.1.0
     "@lezer/html": ^1.3.0
   checksum: 6177d19147580964ecd6910ae951201929a96e63f4f0e624c3138e2805fa87ec6d6d952a3a888c5a52af78b6dd6d04d7d8c76c6a9cd65b1921dc467b5dbaea72
   languageName: node
   linkType: hard
 
-"@codemirror/lang-java@npm:^6.0.0":
+"@codemirror/lang-java@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-java@npm:6.0.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/java": ^1.0.0
   checksum: 4679104683cbffcd224ac04c7e5d144b787494697b26470b07017259035b7bb3fa62609d9a61bfbc566f1756d9f972f9f26d96a3c1362dd48881c1172f9a914d
   languageName: node
   linkType: hard
 
-"@codemirror/lang-javascript@npm:^6.0.0, @codemirror/lang-javascript@npm:^6.1.0":
-  version: 6.1.4
-  resolution: "@codemirror/lang-javascript@npm:6.1.4"
+"@codemirror/lang-javascript@npm:^6.0.0, @codemirror/lang-javascript@npm:^6.1.7":
+  version: 6.1.7
+  resolution: "@codemirror/lang-javascript@npm:6.1.7"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.6.0
     "@codemirror/lint": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
     "@lezer/javascript": ^1.0.0
-  checksum: d550db179c522cd7c39d26815ee47ac4751656c856d42eeb3743e67482d4377692c4fcd3413b0e97c2c7070b6b10aaa582909c6234f42b04145d56efc49c8a6b
+  checksum: 15ce6695e7276102dbc874d178cbc4434d126b7a3e08f89aa9338c7dce5d2d6bdd5f1c6d114a744a8fa26dfc62b0dc639fe6e5c7b306bd14ed37272e75739736
   languageName: node
   linkType: hard
 
-"@codemirror/lang-json@npm:^6.0.0":
+"@codemirror/lang-json@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-json@npm:6.0.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/json": ^1.0.0
   checksum: e9e87d50ff7b81bd56a6ab50740b1dd54e9a93f1be585e1d59d0642e2148842ea1528ac7b7221eb4ddc7fe84bbc28065144cc3ab86f6e06c6aeb2d4b4e62acf1
   languageName: node
   linkType: hard
 
-"@codemirror/lang-markdown@npm:^6.0.0":
-  version: 6.1.0
-  resolution: "@codemirror/lang-markdown@npm:6.1.0"
+"@codemirror/lang-markdown@npm:^6.1.1":
+  version: 6.1.1
+  resolution: "@codemirror/lang-markdown@npm:6.1.1"
   dependencies:
     "@codemirror/lang-html": ^6.0.0
     "@codemirror/language": ^6.3.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
     "@lezer/markdown": ^1.0.0
-  checksum: faee880c5e695391fc5b92788d1500bed3f0cc3766c987077cdc1643cf38b97eb1774a29491a7a75064089478b895e7c8fe5a4f08ac93c9614ccbbe188f10b47
+  checksum: db891dad10a8ea8db17d0a9222774389794cb0957b784e3f154bf27ab4a9be89a28ad4c2f6abf7d829115c3ce46694a2816b61723a5d5776c1d75d566ce016c8
   languageName: node
   linkType: hard
 
-"@codemirror/lang-php@npm:^6.0.0":
+"@codemirror/lang-php@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-php@npm:6.0.1"
   dependencies:
     "@codemirror/lang-html": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.0.0
     "@lezer/php": ^1.0.0
   checksum: c003a29a426486453fdfddbf7302982fa2aa7f059bf6f1ce4cbf08341b0162eee5e2f50e0d71c418dcd358491631780156d846fe352754d042576172c5d86721
   languageName: node
   linkType: hard
 
-"@codemirror/lang-python@npm:^6.1.0":
+"@codemirror/lang-python@npm:^6.1.2":
   version: 6.1.2
   resolution: "@codemirror/lang-python@npm:6.1.2"
   dependencies:
     "@codemirror/autocomplete": ^6.3.2
     "@codemirror/language": ^6.0.0
     "@lezer/python": ^1.0.0
   checksum: e822a1236fb3c2773e1889d4a24f8f2f7fb45ab8cf6e0521d311508a3eda19c4dcf4e2f943766b93545e673f3f0336725418e0bb48b3d9fb6a942339d164cfa5
   languageName: node
   linkType: hard
 
-"@codemirror/lang-rust@npm:^6.0.0":
+"@codemirror/lang-rust@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-rust@npm:6.0.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/rust": ^1.0.0
   checksum: 8a439944cb22159b0b3465ca4fa4294c69843219d5d30e278ae6df8e48f30a7a9256129723c025ec9b5e694d31a3560fb004300b125ffcd81c22d13825845170
   languageName: node
   linkType: hard
 
-"@codemirror/lang-sql@npm:^6.3.0":
-  version: 6.4.0
-  resolution: "@codemirror/lang-sql@npm:6.4.0"
+"@codemirror/lang-sql@npm:^6.4.1":
+  version: 6.4.1
+  resolution: "@codemirror/lang-sql@npm:6.4.1"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 5981b08ff103ae4c36209617543be2ba811ffd26aa68632252ae8526e6c1b7436ff240221348247d3fd5eebb892a4040e7b0b6accbbc5c7968634fd2a9ba0559
+  checksum: d1823e760b88bb15399684b1136b3c7167f104854645b971aa80d7e261e4ad204a5258f1ccd9bbb37a90b20821d2b8fcfac9092198e599b21e7a0cb1e50dc0ee
   languageName: node
   linkType: hard
 
-"@codemirror/lang-wast@npm:^6.0.0":
+"@codemirror/lang-wast@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-wast@npm:6.0.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: 600d98d3ea6a4e99292244ed707e39a2abd9f3abf62cfeff5c819a0cc0c7e86b8c5b91e91c1b7ea21233d9ea09c41abe61d8a40b2547bb5db74239c6df857934
   languageName: node
   linkType: hard
 
-"@codemirror/lang-xml@npm:^6.0.0":
+"@codemirror/lang-xml@npm:^6.0.2":
   version: 6.0.2
   resolution: "@codemirror/lang-xml@npm:6.0.2"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.4.0
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.0.0
@@ -1512,60 +1513,60 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
     style-mod: ^4.0.0
   checksum: bb9411620e2f231653a3f0c4429e0d19a3843bff5dbc117df4649d7bf783ec4ad809c0add8bc0887a4ec3f48b4f8f941621168e47d76101d5383f0d670af1722
   languageName: node
   linkType: hard
 
-"@codemirror/legacy-modes@npm:^6.3.0":
+"@codemirror/legacy-modes@npm:^6.3.2":
   version: 6.3.2
   resolution: "@codemirror/legacy-modes@npm:6.3.2"
   dependencies:
     "@codemirror/language": ^6.0.0
   checksum: fa5f5477fb9e19267251e2ecd3de8c1a4c2512813555bb60111dce3951f2c3f6080a2985a573b7542534ba1d2c34115f7e39ee23fdf8f6f81db6f8ce447c1efc
   languageName: node
   linkType: hard
 
 "@codemirror/lint@npm:^6.0.0":
-  version: 6.2.0
-  resolution: "@codemirror/lint@npm:6.2.0"
+  version: 6.2.1
+  resolution: "@codemirror/lint@npm:6.2.1"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
-  checksum: b97e55a07bca9f7e357e495853ba189ae0ff7dfe7e7ae445d7a0d6c6926ec792c7f5c6b6c13a1f137fd9fedf44a6624e9d500f76d0d46a3c3e9d19c2cda9d28a
+  checksum: 0e383c6b8b0fc463f90f8ebdc71628ba39cffbe4f3667a8382b8eedb61aff9eafe947cb3db947701c8f306acdc9576a2da889d0161ccdd14c9245705cfbd4571
   languageName: node
   linkType: hard
 
-"@codemirror/search@npm:^6.2.0":
-  version: 6.3.0
-  resolution: "@codemirror/search@npm:6.3.0"
+"@codemirror/search@npm:^6.3.0":
+  version: 6.4.0
+  resolution: "@codemirror/search@npm:6.4.0"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
-  checksum: b757eebbb541c9d74fe36ccfdd03bc3e4e7aebb08b491e207d5898f24aaa612558c393ba49de5bf375972f5774de817fcfbad1ac551dda1a34badb41cf130d36
+  checksum: 441e04fc896ac984f224e3adb20bc8a6c63d929778335c70d2cb1e3843674c7998db93e2ab1cd05e8276cb3819766cd23951eec748fdf8e66e3611bd9a55aab5
   languageName: node
   linkType: hard
 
 "@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.1.4, @codemirror/state@npm:^6.2.0":
   version: 6.2.0
   resolution: "@codemirror/state@npm:6.2.0"
   checksum: fdc99c773dc09c700dd02bf918f06132aa8d3069c262cc4eb6ca5c810ce24ae2d7e90719ae7630a8158fd263018de6d40bd78f312e6bfba754e737b64e6c6b3d
   languageName: node
   linkType: hard
 
-"@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.2.2, @codemirror/view@npm:^6.6.0, @codemirror/view@npm:^6.7.0":
-  version: 6.9.3
-  resolution: "@codemirror/view@npm:6.9.3"
+"@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.2.2, @codemirror/view@npm:^6.6.0, @codemirror/view@npm:^6.7.0, @codemirror/view@npm:^6.9.6":
+  version: 6.11.1
+  resolution: "@codemirror/view@npm:6.11.1"
   dependencies:
     "@codemirror/state": ^6.1.4
     style-mod: ^4.0.0
     w3c-keyname: ^2.2.4
-  checksum: 718ecbb021ca75eb89003f73c846a07d36a708dcfec8345f0f0dbcfc0d0df5ea6f114918694b2730a6d49e5e50502bcce79ce7ff94ce55748e068e5a35073755
+  checksum: a7e6ebb1f31b3d998018adcd031edb19dcf4018b6524ad82ca4fe1cc65e902626307c1f7c2875fcd4c72c16fa04886c2309c50ef5c9ebfbce3285c514ed53acb
   languageName: node
   linkType: hard
 
 "@csstools/css-parser-algorithms@npm:^2.0.1":
   version: 2.1.0
   resolution: "@csstools/css-parser-algorithms@npm:2.1.0"
   peerDependencies:
@@ -2014,75 +2015,80 @@
   languageName: node
   linkType: hard
 
 "@jupyter/collaboration-extension@workspace:packages/collaboration-extension":
   version: 0.0.0-use.local
   resolution: "@jupyter/collaboration-extension@workspace:packages/collaboration-extension"
   dependencies:
-    "@jupyter/collaboration": ^1.0.0-alpha.8
-    "@jupyter/docprovider": ^1.0.0-alpha.8
-    "@jupyterlab/application": ^4.0.0-beta.0
-    "@jupyterlab/apputils": ^4.0.0-beta.0
-    "@jupyterlab/builder": ^4.0.0-beta.0
-    "@jupyterlab/codemirror": ^4.0.0-beta.0
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/filebrowser": ^4.0.0-beta.0
-    "@jupyterlab/services": ^7.0.0-beta.0
-    "@jupyterlab/settingregistry": ^4.0.0-beta.0
-    "@jupyterlab/statedb": ^4.0.0-beta.0
-    "@jupyterlab/translation": ^4.0.0-beta.0
-    "@jupyterlab/ui-components": ^4.0.0-beta.0
-    "@lumino/commands": ^2.0.0
-    "@lumino/widgets": ^2.0.0
-    "@types/react": ^18.0.27
+    "@jupyter/collaboration": ^1.0.0-alpha.9
+    "@jupyter/docprovider": ^1.0.0-alpha.9
+    "@jupyterlab/application": ^4.0.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/builder": ^4.0.0
+    "@jupyterlab/codemirror": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/filebrowser": ^4.0.0
+    "@jupyterlab/fileeditor": ^4.0.0
+    "@jupyterlab/logconsole": ^4.0.0
+    "@jupyterlab/notebook": ^4.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/settingregistry": ^4.0.0
+    "@jupyterlab/statedb": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
+    "@lumino/commands": ^2.1.0
+    "@lumino/widgets": ^2.1.0
+    "@types/react": ~18.0.26
     npm-run-all: ^4.1.5
     rimraf: ^4.1.2
-    typescript: ~5.0.2
+    typescript: ~5.0.4
     y-protocols: ^1.0.5
     y-websocket: ^1.3.15
     yjs: ^13.5.40
   languageName: unknown
   linkType: soft
 
-"@jupyter/collaboration@^1.0.0-alpha.8, @jupyter/collaboration@workspace:packages/collaboration":
+"@jupyter/collaboration@^1.0.0-alpha.9, @jupyter/collaboration@workspace:packages/collaboration":
   version: 0.0.0-use.local
   resolution: "@jupyter/collaboration@workspace:packages/collaboration"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.7.0
-    "@jupyterlab/apputils": ^4.0.0-beta.0
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/services": ^7.0.0-beta.0
-    "@jupyterlab/ui-components": ^4.0.0-beta.0
-    "@lumino/coreutils": ^2.0.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/ui-components": ^4.0.0
+    "@lumino/coreutils": ^2.1.0
     "@lumino/virtualdom": ^2.0.0
-    "@lumino/widgets": ^2.0.0
+    "@lumino/widgets": ^2.1.0
     "@types/react": ^18.0.27
     react: ^18.2.0
     rimraf: ^4.1.2
-    typescript: ~5.0.2
+    typescript: ~5.0.4
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   languageName: unknown
   linkType: soft
 
-"@jupyter/docprovider@^1.0.0-alpha.8, @jupyter/docprovider@workspace:packages/docprovider":
+"@jupyter/docprovider@^1.0.0-alpha.9, @jupyter/docprovider@workspace:packages/docprovider":
   version: 0.0.0-use.local
   resolution: "@jupyter/docprovider@workspace:packages/docprovider"
   dependencies:
-    "@jupyter/ydoc": ^1.0.0
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/services": ^7.0.0-beta.0
-    "@jupyterlab/testing": ^4.0.0-beta.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
-    "@lumino/signaling": ^2.0.0
+    "@jupyter/ydoc": ^1.0.2
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/testing": ^4.0.0
+    "@lumino/coreutils": ^2.1.0
+    "@lumino/disposable": ^2.1.0
+    "@lumino/signaling": ^2.1.0
     "@types/jest": ^29.2.0
+    jest: ^29.5.0
     rimraf: ^4.1.2
-    typescript: ~5.0.2
+    typescript: ~5.0.4
     y-protocols: ^1.0.5
     y-websocket: ^1.3.15
     yjs: ^13.5.40
   languageName: unknown
   linkType: soft
 
 "@jupyter/real-time-collaboration@workspace:.":
@@ -2100,119 +2106,119 @@
     prettier: ^2.8.4
     rimraf: ^4.1.2
     stylelint: ^15.2.0
     stylelint-config-recommended: ^10.0.0
     stylelint-config-standard: ^30.0.1
     stylelint-prettier: ^3.0.0
     typedoc: ~0.23.28
-    typescript: ~5.0.2
+    typescript: ~5.0.4
   languageName: unknown
   linkType: soft
 
-"@jupyter/ydoc@npm:^0.3.4":
-  version: 0.3.4
-  resolution: "@jupyter/ydoc@npm:0.3.4"
-  dependencies:
-    "@jupyterlab/nbformat": ^3.0.0 || ^4.0.0-alpha.15
-    "@lumino/coreutils": ^1.11.0 || ^2.0.0-alpha.6
-    "@lumino/disposable": ^1.10.0 || ^2.0.0-alpha.6
-    "@lumino/signaling": ^1.10.0 || ^2.0.0-alpha.6
-    y-protocols: ^1.0.5
-    yjs: ^13.5.40
-  checksum: edd14a01be6ceac437d3ebfb5f7a2d2c8eac60fec91e48d8d2ef2bef9f1423b4350c57dba25b3b043759ffb61b601a3815c1ea56532d1d707e3fbeb5df86b7e6
-  languageName: node
-  linkType: hard
-
-"@jupyter/ydoc@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "@jupyter/ydoc@npm:1.0.0"
+"@jupyter/ydoc@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "@jupyter/ydoc@npm:1.0.2"
   dependencies:
     "@jupyterlab/nbformat": ^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0
     "@lumino/coreutils": ^1.11.0 || ^2.0.0
     "@lumino/disposable": ^1.10.0 || ^2.0.0
     "@lumino/signaling": ^1.10.0 || ^2.0.0
     y-protocols: ^1.0.5
     yjs: ^13.5.40
-  checksum: 482f97b7e1e71736a3598dec41659696453821f056ecfaa8e67215b3766b7770cb6d718982069124698e1a824cb9aee20835a248d1d393d2229e7920a2b69f5c
+  checksum: 739f9630940466b3cfcd7b742dd06479f81772ca13f863d057af0bbb5e318829506969066ab72977e7c721644982b5c8f88cf44e1ae81955ed1c27e87632d1f2
   languageName: node
   linkType: hard
 
-"@jupyterlab/application@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/application@npm:4.0.0-beta.0"
+"@jupyterlab/application@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/application@npm:4.0.0"
   dependencies:
     "@fortawesome/fontawesome-free": ^5.12.0
-    "@jupyterlab/apputils": ^4.0.0-beta.0
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/docregistry": ^4.0.0-beta.0
-    "@jupyterlab/rendermime": ^4.0.0-beta.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-beta.0
-    "@jupyterlab/services": ^7.0.0-beta.0
-    "@jupyterlab/statedb": ^4.0.0-beta.0
-    "@jupyterlab/translation": ^4.0.0-beta.0
-    "@jupyterlab/ui-components": ^4.0.0-beta.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/statedb": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
-    "@lumino/application": ^2.0.0
-    "@lumino/commands": ^2.0.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
+    "@lumino/application": ^2.1.1
+    "@lumino/commands": ^2.1.1
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
-    "@lumino/polling": ^2.0.0
+    "@lumino/polling": ^2.1.1
     "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.0.0
-    "@lumino/widgets": ^2.0.0
-  checksum: 0143ff36f29150ee0e43521b5bc0b83b578ea1addf40143b992276433cc7625f1bd303fce29ecf3cfebc35c70ac7f2170e97d459096ba721532bd066dd8bee21
+    "@lumino/signaling": ^2.1.1
+    "@lumino/widgets": ^2.1.1
+  checksum: 82750647de5997d6945627f517d82ffad3e7c272bce0c195819cc138b59546fbe43ee6c0ef4baf88de303964288ed1ac36234a99bedfb319eaf456b1321b199c
   languageName: node
   linkType: hard
 
-"@jupyterlab/apputils@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/apputils@npm:4.0.0-beta.0"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/observables": ^5.0.0-beta.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-beta.0
-    "@jupyterlab/services": ^7.0.0-beta.0
-    "@jupyterlab/settingregistry": ^4.0.0-beta.0
-    "@jupyterlab/statedb": ^4.0.0-beta.0
-    "@jupyterlab/statusbar": ^4.0.0-beta.0
-    "@jupyterlab/translation": ^4.0.0-beta.0
-    "@jupyterlab/ui-components": ^4.0.0-beta.0
+"@jupyterlab/apputils@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/apputils@npm:4.0.0"
+  dependencies:
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/settingregistry": ^4.0.0
+    "@jupyterlab/statedb": ^4.0.0
+    "@jupyterlab/statusbar": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
-    "@lumino/commands": ^2.0.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
+    "@lumino/commands": ^2.1.1
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/messaging": ^2.0.0
-    "@lumino/signaling": ^2.0.0
+    "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
-    "@lumino/widgets": ^2.0.0
+    "@lumino/widgets": ^2.1.1
     "@types/react": ^18.0.26
     react: ^18.2.0
     sanitize-html: ~2.7.3
-  checksum: 863bb1b19b4d79873ae679ce46e30cb355f8abb7592a1e4bc6889e1516a5b4aaa4918583bf3874fde7cfca2f7f432e77576c950951165bb4bb85e3efd797db1b
+  checksum: 360bf34e9810a7014c6637a6ac5c23a2ee73da8339675235cee3866beb3a477dc3b4d993c0a79da5ebe472f5c28fa131d507d62e20b3a93853f05e62b126add9
+  languageName: node
+  linkType: hard
+
+"@jupyterlab/attachments@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/attachments@npm:4.0.0"
+  dependencies:
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@lumino/disposable": ^2.1.1
+    "@lumino/signaling": ^2.1.1
+  checksum: 71c8e488a0d31e00e1345336edece04faa0d2b6fbf5de284fad05bb2a8f732c57e9b2ffe10999dd416a1d00cdce4bc425f9f88dd91684cb8b55eea52a1d5ed98
   languageName: node
   linkType: hard
 
-"@jupyterlab/builder@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/builder@npm:4.0.0-beta.0"
+"@jupyterlab/builder@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/builder@npm:4.0.0"
   dependencies:
     "@lumino/algorithm": ^2.0.0
-    "@lumino/application": ^2.0.0
-    "@lumino/commands": ^2.0.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
+    "@lumino/application": ^2.1.1
+    "@lumino/commands": ^2.1.1
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
-    "@lumino/dragdrop": ^2.0.0
+    "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.0.0
+    "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
-    "@lumino/widgets": ^2.0.0
+    "@lumino/widgets": ^2.1.1
     ajv: ^8.12.0
     commander: ^9.4.1
     css-loader: ^6.7.1
     duplicate-package-checker-webpack-plugin: ^3.0.0
     fs-extra: ^10.1.0
     glob: ~7.1.6
     license-webpack-plugin: ^2.3.14
@@ -2226,378 +2232,554 @@
     terser-webpack-plugin: ^5.3.7
     webpack: ^5.76.1
     webpack-cli: ^5.0.1
     webpack-merge: ^5.8.0
     worker-loader: ^3.0.2
   bin:
     build-labextension: lib/build-labextension.js
-  checksum: 9245f364d2bb20a4804b63b01cef890a113833057abfa1f978a636fb33dcbe93782a78c1245fa516cf2dde071b937cfd1dabfe6959e84e5b781a9de9a1237300
+  checksum: c359031858376e37b2fe46bc7897fe0568b0cf90bcaaee6bded2e22f207c61a32d4b00b6954de00082e551dd07b6259997c00feeb25e7d44acf9ac97934fdd45
   languageName: node
   linkType: hard
 
-"@jupyterlab/codeeditor@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/codeeditor@npm:4.0.0-beta.0"
+"@jupyterlab/cells@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/cells@npm:4.0.0"
   dependencies:
     "@codemirror/state": ^6.2.0
-    "@jupyter/ydoc": ^0.3.4
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/nbformat": ^4.0.0-beta.0
-    "@jupyterlab/observables": ^5.0.0-beta.0
-    "@jupyterlab/statusbar": ^4.0.0-beta.0
-    "@jupyterlab/translation": ^4.0.0-beta.0
-    "@jupyterlab/ui-components": ^4.0.0-beta.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
-    "@lumino/dragdrop": ^2.0.0
+    "@codemirror/view": ^6.9.6
+    "@jupyter/ydoc": ^1.0.2
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/attachments": ^4.0.0
+    "@jupyterlab/codeeditor": ^4.0.0
+    "@jupyterlab/codemirror": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/documentsearch": ^4.0.0
+    "@jupyterlab/filebrowser": ^4.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/outputarea": ^4.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/toc": ^6.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
+    "@lumino/algorithm": ^2.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/domutils": ^2.0.0
+    "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
-    "@lumino/signaling": ^2.0.0
-    "@lumino/widgets": ^2.0.0
+    "@lumino/polling": ^2.1.1
+    "@lumino/signaling": ^2.1.1
+    "@lumino/virtualdom": ^2.0.0
+    "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: c9988e6a92be593859f7f476ff57a226c9ff4064cfdefa9b620eb365cf949c50eafcc23f9191d83c30e230cdbe50430fe55be603697f2bb19eb98753a08e26fc
+  checksum: 2474642428f344a316b0296640f9adb07e805d3c8896d1a601a2a5131fc4f4a8a4a627583f3dff904f7c318d6c0f236bc0d9cd200545f395796fcfe4244ecbcb
   languageName: node
   linkType: hard
 
-"@jupyterlab/codemirror@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/codemirror@npm:4.0.0-beta.0"
+"@jupyterlab/codeeditor@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/codeeditor@npm:4.0.0"
   dependencies:
-    "@codemirror/autocomplete": ^6.4.0
-    "@codemirror/commands": ^6.1.0
-    "@codemirror/lang-cpp": ^6.0.0
-    "@codemirror/lang-css": ^6.0.0
-    "@codemirror/lang-html": ^6.4.0
-    "@codemirror/lang-java": ^6.0.0
-    "@codemirror/lang-javascript": ^6.1.0
-    "@codemirror/lang-json": ^6.0.0
-    "@codemirror/lang-markdown": ^6.0.0
-    "@codemirror/lang-php": ^6.0.0
-    "@codemirror/lang-python": ^6.1.0
-    "@codemirror/lang-rust": ^6.0.0
-    "@codemirror/lang-sql": ^6.3.0
-    "@codemirror/lang-wast": ^6.0.0
-    "@codemirror/lang-xml": ^6.0.0
-    "@codemirror/language": ^6.4.0
-    "@codemirror/legacy-modes": ^6.3.0
-    "@codemirror/search": ^6.2.0
     "@codemirror/state": ^6.2.0
-    "@codemirror/view": ^6.7.0
-    "@jupyter/ydoc": ^0.3.4
-    "@jupyterlab/codeeditor": ^4.0.0-beta.0
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/documentsearch": ^4.0.0-beta.0
-    "@jupyterlab/nbformat": ^4.0.0-beta.0
-    "@jupyterlab/translation": ^4.0.0-beta.0
-    "@lezer/common": ^1.0.0
-    "@lezer/generator": ^1.0.0
-    "@lezer/highlight": ^1.0.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
-    "@lumino/signaling": ^2.0.0
+    "@jupyter/ydoc": ^1.0.2
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/statusbar": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/dragdrop": ^2.1.1
+    "@lumino/messaging": ^2.0.0
+    "@lumino/signaling": ^2.1.1
+    "@lumino/widgets": ^2.1.1
+    react: ^18.2.0
+  checksum: 8287d77738a41814eb83621691adbcee119e6a7b3d4741250e53fc11b8664ce1f6ae5a79150222b235d45ec7b22db980d773d77a517d6b5c6a241b8a27817b7a
+  languageName: node
+  linkType: hard
+
+"@jupyterlab/codemirror@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/codemirror@npm:4.0.0"
+  dependencies:
+    "@codemirror/autocomplete": ^6.5.1
+    "@codemirror/commands": ^6.2.3
+    "@codemirror/lang-cpp": ^6.0.2
+    "@codemirror/lang-css": ^6.1.1
+    "@codemirror/lang-html": ^6.4.3
+    "@codemirror/lang-java": ^6.0.1
+    "@codemirror/lang-javascript": ^6.1.7
+    "@codemirror/lang-json": ^6.0.1
+    "@codemirror/lang-markdown": ^6.1.1
+    "@codemirror/lang-php": ^6.0.1
+    "@codemirror/lang-python": ^6.1.2
+    "@codemirror/lang-rust": ^6.0.1
+    "@codemirror/lang-sql": ^6.4.1
+    "@codemirror/lang-wast": ^6.0.1
+    "@codemirror/lang-xml": ^6.0.2
+    "@codemirror/language": ^6.6.0
+    "@codemirror/legacy-modes": ^6.3.2
+    "@codemirror/search": ^6.3.0
+    "@codemirror/state": ^6.2.0
+    "@codemirror/view": ^6.9.6
+    "@jupyter/ydoc": ^1.0.2
+    "@jupyterlab/codeeditor": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/documentsearch": ^4.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@lezer/common": ^1.0.2
+    "@lezer/generator": ^1.2.2
+    "@lezer/highlight": ^1.1.4
+    "@lezer/markdown": ^1.0.2
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/signaling": ^2.1.1
     yjs: ^13.5.40
-  checksum: 30b50b2ca608cf500c58bea301b9e6dcbffd81e649cb26d85c6a016a8cb0262e22b3e8dec13bc38e0f2c191992871e673c0f6ed3451ae07ad48dd8431cc56d39
+  checksum: 3252c57f1d35924d6d6ad2a48690fa8bbe4e1a22455f9e1514b4405d16ff379532477aed331cd28908e8d0ef572ee76937ee5f382c95dc62e5dd97fa911603d5
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:^6.0.0-beta.0":
-  version: 6.0.0-beta.0
-  resolution: "@jupyterlab/coreutils@npm:6.0.0-beta.0"
+"@jupyterlab/coreutils@npm:^6.0.0":
+  version: 6.0.0
+  resolution: "@jupyterlab/coreutils@npm:6.0.0"
   dependencies:
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
-    "@lumino/signaling": ^2.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/signaling": ^2.1.1
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
-  checksum: d5321b8b6b4feb248bb6beb039d0589c98501221beb93a9c97a0b7405bd19ef14c80c3afbaa27dbf72b195cd2a3b75e7306c52a43da78f2d133324d2f787573b
+  checksum: c46bb60af792186b4d9d60378fdb2f03473055736e438e05971bcbf1d5edb62c7722f1465e5ef2fd2dc9c4b5b6043301012478b218cf6c475a99914b26a1fd14
   languageName: node
   linkType: hard
 
-"@jupyterlab/docmanager@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/docmanager@npm:4.0.0-beta.0"
+"@jupyterlab/docmanager@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/docmanager@npm:4.0.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-beta.0
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/docregistry": ^4.0.0-beta.0
-    "@jupyterlab/services": ^7.0.0-beta.0
-    "@jupyterlab/statusbar": ^4.0.0-beta.0
-    "@jupyterlab/translation": ^4.0.0-beta.0
-    "@jupyterlab/ui-components": ^4.0.0-beta.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/statusbar": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.0.0
-    "@lumino/widgets": ^2.0.0
+    "@lumino/signaling": ^2.1.1
+    "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: 5cf19942f67d40e9108af6b653a8f7e94d17828e816e56fca14eb96287bfa4bd9b38bcb1674f2718a6b9283c2d8c9ef065004c324cea304342f91f57aaa8d042
+  checksum: d9495bea5f5e5de2d133be0ea097b9d2634575d1054dafb198d49398bfed6b9ff52d5d2ce0848ae11462fa5070f6651eccda3242f867661758f135b0703839f9
   languageName: node
   linkType: hard
 
-"@jupyterlab/docregistry@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/docregistry@npm:4.0.0-beta.0"
-  dependencies:
-    "@jupyter/ydoc": ^0.3.4
-    "@jupyterlab/apputils": ^4.0.0-beta.0
-    "@jupyterlab/codeeditor": ^4.0.0-beta.0
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/observables": ^5.0.0-beta.0
-    "@jupyterlab/rendermime": ^4.0.0-beta.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-beta.0
-    "@jupyterlab/services": ^7.0.0-beta.0
-    "@jupyterlab/translation": ^4.0.0-beta.0
-    "@jupyterlab/ui-components": ^4.0.0-beta.0
+"@jupyterlab/docregistry@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/docregistry@npm:4.0.0"
+  dependencies:
+    "@jupyter/ydoc": ^1.0.2
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/codeeditor": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.0.0
-    "@lumino/widgets": ^2.0.0
-  checksum: 413062f626169534bd66485162946faa34825d97d8b02950bc8429f043a3c10e2bd93cec95b9e7362f33efb56a54f0dffd2de7f78a607e41d0555c0be0440334
+    "@lumino/signaling": ^2.1.1
+    "@lumino/widgets": ^2.1.1
+  checksum: 8927ea10312238333d1036ea6f4047d86779120cdf6c8391f91e5d859e85d504c2345f629a2a8cf50cdc394739828cc4868a46ebefe1c20932a2f496463ca250
   languageName: node
   linkType: hard
 
-"@jupyterlab/documentsearch@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/documentsearch@npm:4.0.0-beta.0"
+"@jupyterlab/documentsearch@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/documentsearch@npm:4.0.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-beta.0
-    "@jupyterlab/translation": ^4.0.0-beta.0
-    "@jupyterlab/ui-components": ^4.0.0-beta.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
-    "@lumino/polling": ^2.0.0
-    "@lumino/signaling": ^2.0.0
-    "@lumino/widgets": ^2.0.0
+    "@lumino/polling": ^2.1.1
+    "@lumino/signaling": ^2.1.1
+    "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: e29a6f02e6d67a57fdd2beeda3657f537729e4c7d88c463fa6f9c23996d6309d924b62d2fb4f776bac84d17434cfafc80cd25a775f91ccf4827cf8260bac392e
+  checksum: 686befb5ae48a485530f298f7d067b5c77d17524fff779f8c468857c44baab75f1ed3c504546f6440cf0cfc8420e617abcbaa120208d2166cfb124a6455e5472
   languageName: node
   linkType: hard
 
-"@jupyterlab/filebrowser@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/filebrowser@npm:4.0.0-beta.0"
-  dependencies:
-    "@jupyterlab/apputils": ^4.0.0-beta.0
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/docmanager": ^4.0.0-beta.0
-    "@jupyterlab/docregistry": ^4.0.0-beta.0
-    "@jupyterlab/services": ^7.0.0-beta.0
-    "@jupyterlab/statedb": ^4.0.0-beta.0
-    "@jupyterlab/statusbar": ^4.0.0-beta.0
-    "@jupyterlab/translation": ^4.0.0-beta.0
-    "@jupyterlab/ui-components": ^4.0.0-beta.0
+"@jupyterlab/filebrowser@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/filebrowser@npm:4.0.0"
+  dependencies:
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docmanager": ^4.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/statedb": ^4.0.0
+    "@jupyterlab/statusbar": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
-    "@lumino/dragdrop": ^2.0.0
+    "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
-    "@lumino/polling": ^2.0.0
-    "@lumino/signaling": ^2.0.0
+    "@lumino/polling": ^2.1.1
+    "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
-    "@lumino/widgets": ^2.0.0
+    "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: ff4c5ac57f7e8eb08d2a820a63222248c369ea06e63b9423eb299a3aad07d147ae153569eee73771a21f662b13f10b44d832b6bee29a8968bc50d7668b9233f8
+  checksum: 58e61e9b0e6d373fa5cd93398dfee146c635d5f5008d00e640c4f0687ed8ed7135779806e159703a88ecd55f45b1725214c657a466e63577b70b0380c5852df5
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.15, @jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0":
-  version: 3.6.2
-  resolution: "@jupyterlab/nbformat@npm:3.6.2"
+"@jupyterlab/fileeditor@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/fileeditor@npm:4.0.0"
   dependencies:
-    "@lumino/coreutils": ^1.11.0
-  checksum: 9da3c71ca8a8c72d77a941fd527ce1e83f9f0978c3f35106f70f40bab929d261d8a91464303da38cca52450a5cbea0375049b2883795cec457f2673138d3e953
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/codeeditor": ^4.0.0
+    "@jupyterlab/codemirror": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/documentsearch": ^4.0.0
+    "@jupyterlab/lsp": ^4.0.0
+    "@jupyterlab/statusbar": ^4.0.0
+    "@jupyterlab/toc": ^6.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
+    "@lumino/commands": ^2.1.1
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/messaging": ^2.0.0
+    "@lumino/widgets": ^2.1.1
+    react: ^18.2.0
+    regexp-match-indices: ^1.0.2
+  checksum: f981f4b3b2cca2e81bf8beab7ef23361d3073bdba811ba22b3d50adc092bca34aa4c5f81c37c52ae91e9e57d35ae953bc856bc084dfe2db418d746ccaa8869b5
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/nbformat@npm:4.0.0-beta.0"
+"@jupyterlab/logconsole@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/logconsole@npm:4.0.0"
   dependencies:
-    "@lumino/coreutils": ^2.0.0
-  checksum: 7d6a56d665af349f7e60e0464ce2e4ebc03b25090561aececd23b3e8fe0042af458abb6234523f9a45080f78ac21c5c5bc306a54f74f4b4545e56faf251a9331
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/outputarea": ^4.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/messaging": ^2.0.0
+    "@lumino/signaling": ^2.1.1
+    "@lumino/widgets": ^2.1.1
+  checksum: d1c60c7871b2f1a8f405f6bbcdab3ade621262d2d5804a83269afc2dc11d249a5dcc7578702b0c45805c8ab657a6970add685fe5a2f1fc90e46b18aa34378bba
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:^5.0.0-beta.0":
-  version: 5.0.0-beta.0
-  resolution: "@jupyterlab/observables@npm:5.0.0-beta.0"
+"@jupyterlab/lsp@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/lsp@npm:4.0.0"
   dependencies:
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/codeeditor": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/signaling": ^2.1.1
+    lodash.mergewith: ^4.6.1
+    vscode-jsonrpc: ^6.0.0
+    vscode-languageserver-protocol: ^3.17.0
+    vscode-ws-jsonrpc: ~1.0.2
+  checksum: 7657fe88fc155e7a988558b9b8d34a36d6bb5fee0571a0953ac77add170f82b2f7ad1d76c1f90185087daebb4d40c5ff9e7f44478abbcb485736f7806d3d7fb8
+  languageName: node
+  linkType: hard
+
+"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/nbformat@npm:4.0.0"
+  dependencies:
+    "@lumino/coreutils": ^2.1.1
+  checksum: 152da6b9622c7683543ad2bd9525857a8a39b4b8a5474998e921232f108c366dd8625daeb14e2cc2aa8aac124b9a5d16f285310cd241c9769d51af80730dbd59
+  languageName: node
+  linkType: hard
+
+"@jupyterlab/notebook@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/notebook@npm:4.0.0"
+  dependencies:
+    "@jupyter/ydoc": ^1.0.2
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/cells": ^4.0.0
+    "@jupyterlab/codeeditor": ^4.0.0
+    "@jupyterlab/codemirror": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/documentsearch": ^4.0.0
+    "@jupyterlab/lsp": ^4.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/settingregistry": ^4.0.0
+    "@jupyterlab/statusbar": ^4.0.0
+    "@jupyterlab/toc": ^6.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/domutils": ^2.0.0
+    "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
-    "@lumino/signaling": ^2.0.0
-  checksum: 1f75edbba3aa29018e5f60fb05f489eb994e9578e57ffafcfaaf6be17cc45b4bde39d40b6e946d6ec9067134e79197bf990c70c4e2eefa075cb65a0553fa9af5
+    "@lumino/properties": ^2.0.0
+    "@lumino/signaling": ^2.1.1
+    "@lumino/virtualdom": ^2.0.0
+    "@lumino/widgets": ^2.1.1
+    react: ^18.2.0
+  checksum: 29ba29519fba567d0d686426b750d58bfddf6235cb3ad812ef671750637dbfcdafb5348feda44168d83f65936e5478562cffdc7ceeabac221fcdfab38f11bc31
+  languageName: node
+  linkType: hard
+
+"@jupyterlab/observables@npm:^5.0.0":
+  version: 5.0.0
+  resolution: "@jupyterlab/observables@npm:5.0.0"
+  dependencies:
+    "@lumino/algorithm": ^2.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/messaging": ^2.0.0
+    "@lumino/signaling": ^2.1.1
+  checksum: 1554f473e0ab0eef288ea86945c03a07d79f478bfdf55651036161a58cd1d9a0695e202ced0ebe3a6863f73ba12ccd85b86f7a4c2e6f9fe41ccddb0c4fbbc33e
+  languageName: node
+  linkType: hard
+
+"@jupyterlab/outputarea@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/outputarea@npm:4.0.0"
+  dependencies:
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@lumino/algorithm": ^2.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/messaging": ^2.0.0
+    "@lumino/properties": ^2.0.0
+    "@lumino/signaling": ^2.1.1
+    "@lumino/widgets": ^2.1.1
+  checksum: d2c22e1fe1ebe4407e7a5d383addda64561b5a3afda277a0c4750be48bf30fbb90ee6a3401ac0a9410a7e3c969792d34bc2dcc880806fa3b290ecace01710e80
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime-interfaces@npm:^3.8.0-beta.0":
-  version: 3.8.0-beta.0
-  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.0-beta.0"
+"@jupyterlab/rendermime-interfaces@npm:^3.8.0":
+  version: 3.8.0
+  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.0"
   dependencies:
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/widgets": ^2.0.0
-  checksum: c4416c9dab2bccc0fe4e941ef6d58ef8c110178357f2c01960481a6326534d49552bb3cd765ea7b146282103de47f344143aa06aa08db39e2cde835c0f9e76e9
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/widgets": ^2.1.1
+  checksum: 5e70a58a4d8aa7380a041d267972851b9b3fa5e4d68d254ede51c9e5bea4a76b38d47bc5c512e2fd84cd297f5bcaf9cbc9f73ba0824b5b910b10043309a820c7
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/rendermime@npm:4.0.0-beta.0"
+"@jupyterlab/rendermime@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/rendermime@npm:4.0.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-beta.0
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/nbformat": ^4.0.0-beta.0
-    "@jupyterlab/observables": ^5.0.0-beta.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-beta.0
-    "@jupyterlab/services": ^7.0.0-beta.0
-    "@jupyterlab/translation": ^4.0.0-beta.0
-    "@lumino/coreutils": ^2.0.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@lumino/coreutils": ^2.1.1
     "@lumino/messaging": ^2.0.0
-    "@lumino/signaling": ^2.0.0
-    "@lumino/widgets": ^2.0.0
+    "@lumino/signaling": ^2.1.1
+    "@lumino/widgets": ^2.1.1
     lodash.escape: ^4.0.1
-  checksum: 387100358027e289a39219e7e6992369e86ff16e18794696516eef3181a7de115a49a4bd0579808b309202a0e3e0c4e4378a059e3dc2f0aa9ef73a00cf8d8c00
+  checksum: fb6373517bf2fa2557b38ccf53ba95b45c9327f86f14726dedd433f0b3466f439ab98cb2c8ae10aded9f269bf7c11225765e286aeca56f3755bada8f5d5e102a
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^7.0.0-beta.0":
-  version: 7.0.0-beta.0
-  resolution: "@jupyterlab/services@npm:7.0.0-beta.0"
-  dependencies:
-    "@jupyter/ydoc": ^0.3.4
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/nbformat": ^4.0.0-beta.0
-    "@jupyterlab/settingregistry": ^4.0.0-beta.0
-    "@jupyterlab/statedb": ^4.0.0-beta.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
-    "@lumino/polling": ^2.0.0
+"@jupyterlab/services@npm:^7.0.0":
+  version: 7.0.0
+  resolution: "@jupyterlab/services@npm:7.0.0"
+  dependencies:
+    "@jupyter/ydoc": ^1.0.2
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/settingregistry": ^4.0.0
+    "@jupyterlab/statedb": ^4.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/polling": ^2.1.1
     "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.0.0
+    "@lumino/signaling": ^2.1.1
     ws: ^8.11.0
-  checksum: 4c931e73afd252e61f223d97de8589b37f6fa2d898920e6fef30dc217140a9ac18d7ead71ce2f3d1085b991a319d42f9fa7b3587029dd64a4e2883b15d5fcd5d
+  checksum: 96e986e8007247aa5258586263e31e48dfa6e7e7bb2a9d61f699e41b291f50c8653a9c42ae340a428c9af58946c47f7021ccb6b79b74b750cf1547b8d6c81b03
   languageName: node
   linkType: hard
 
-"@jupyterlab/settingregistry@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/settingregistry@npm:4.0.0-beta.0"
+"@jupyterlab/settingregistry@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/settingregistry@npm:4.0.0"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.0-beta.0
-    "@jupyterlab/statedb": ^4.0.0-beta.0
-    "@lumino/commands": ^2.0.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
-    "@lumino/signaling": ^2.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/statedb": ^4.0.0
+    "@lumino/commands": ^2.1.1
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/signaling": ^2.1.1
     "@rjsf/utils": ^5.1.0
     ajv: ^8.12.0
     json5: ^2.2.3
-  checksum: 34bf60052ccbfc51a7cbed3fea7e2f737a88e597aab588dd8e772f4414e13c578f6ec7e939184043e00a61cab17147bf63a8afba5fbf5b51f3de7e34c47ec605
+  peerDependencies:
+    react: ">=16"
+  checksum: f52cd36c28336ad554a4eb43f6cef7f82cb7a9161897e8b633da8c0b4519d0ed7e3e34846fec132714867b0190a9c19754e88edef31ffdf6dc2d1afe49b50041
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/statedb@npm:4.0.0-beta.0"
+"@jupyterlab/statedb@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/statedb@npm:4.0.0"
   dependencies:
-    "@lumino/commands": ^2.0.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
+    "@lumino/commands": ^2.1.1
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
     "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.0.0
-  checksum: cad61119c2c519ce4407109bb199b12190f212eefc571cc0f4f234e0a2aae789b5f198272bb3e9d58c15c2aac3b186ed03f104ee4d2bdf57473f3a1788dc3176
+    "@lumino/signaling": ^2.1.1
+  checksum: e90c943b4486df3a1bd53c64c0860e40706a26f4307628f2c71168090f47f85bab2fd68529366aa74211501a6875bd6d7098e1cd976f2e7d2d197a687b6b3bd3
   languageName: node
   linkType: hard
 
-"@jupyterlab/statusbar@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/statusbar@npm:4.0.0-beta.0"
+"@jupyterlab/statusbar@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/statusbar@npm:4.0.0"
   dependencies:
-    "@jupyterlab/ui-components": ^4.0.0-beta.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
-    "@lumino/signaling": ^2.0.0
-    "@lumino/widgets": ^2.0.0
+    "@lumino/signaling": ^2.1.1
+    "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: b6a1cff897b3981dc4565a28d1b9a763293bed3ed0f4a2ad3bee66a1113e7def5e831bb34080a6a22acc04d038583aeb3dbcceef87c72b0eb6c5e876642c85c3
+  checksum: 861444ba5ca001f9174b58d5a2c46e4d7947856b1c5302d3ec70e6c72d1608c77b65c792904e07fd8612f11d51ac9f30aa2ad3cbd256e701d6c12138e3f9b89f
   languageName: node
   linkType: hard
 
-"@jupyterlab/testing@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/testing@npm:4.0.0-beta.0"
+"@jupyterlab/testing@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/testing@npm:4.0.0"
   dependencies:
     "@babel/core": ^7.10.2
     "@babel/preset-env": ^7.10.2
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/signaling": ^2.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/signaling": ^2.1.1
     child_process: ~1.0.2
     deepmerge: ^4.2.2
     fs-extra: ^10.1.0
     identity-obj-proxy: ^3.0.0
     jest: ^29.2.0
     jest-environment-jsdom: ^29.3.0
     jest-junit: ^15.0.0
     node-fetch: ^2.6.0
     simulate-event: ~1.4.0
-    ts-jest: ^29.0.0
-  checksum: 4a78e480b0a55468875e91177facf3e14701c74e05eb7ce0b906fde64dd8bfd967dc7bfa62a3b6e65a0e209b7c30c06dc52fd17d9aa4f634ebacb37e28eaeb33
+    ts-jest: ^29.1.0
+  peerDependencies:
+    typescript: ">=4.3"
+  checksum: cb9a38b2eb6f714981193d937e48a006419963734f880b1392ddcc3705fef0d5ce93bfd2cfd740bac202aecc579fa73f3b7bcb4f6e02224e047e4be64d339fbd
   languageName: node
   linkType: hard
 
-"@jupyterlab/translation@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/translation@npm:4.0.0-beta.0"
+"@jupyterlab/toc@npm:^6.0.0":
+  version: 6.0.0
+  resolution: "@jupyterlab/toc@npm:6.0.0"
   dependencies:
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-beta.0
-    "@jupyterlab/services": ^7.0.0-beta.0
-    "@jupyterlab/statedb": ^4.0.0-beta.0
-    "@lumino/coreutils": ^2.0.0
-  checksum: 901bf5452b7b00bccab38f7cfd5b40cc37e833c83cf21f9d8b3b6b6422deb7394a2cee0d5df695b3c30f22d7e43e656c03aa19fcc0558abd8ae0e797f4a5105c
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/messaging": ^2.0.0
+    "@lumino/signaling": ^2.1.1
+    "@lumino/widgets": ^2.1.1
+    react: ^18.2.0
+  checksum: 7fd8cbbeaaad272355296d8ddab01c54233373d2c0457d93beae1efa2e491845980746b75f46f78f49370668a323f42ef923b76c55bf9a520548845f7c5e2d57
   languageName: node
   linkType: hard
 
-"@jupyterlab/ui-components@npm:^4.0.0-beta.0":
-  version: 4.0.0-beta.0
-  resolution: "@jupyterlab/ui-components@npm:4.0.0-beta.0"
+"@jupyterlab/translation@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/translation@npm:4.0.0"
   dependencies:
-    "@jupyterlab/coreutils": ^6.0.0-beta.0
-    "@jupyterlab/observables": ^5.0.0-beta.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-beta.0
-    "@jupyterlab/translation": ^4.0.0-beta.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/statedb": ^4.0.0
+    "@lumino/coreutils": ^2.1.1
+  checksum: f3124bff6e3eb9c1adbe91f60dd823a3b4a4b8b453fbf024a605f5be44463fa7eb15e176238255a775c96b50e4cc551bde757a03531e56a76db25a30feed469f
+  languageName: node
+  linkType: hard
+
+"@jupyterlab/ui-components@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/ui-components@npm:4.0.0"
+  dependencies:
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/translation": ^4.0.0
     "@lumino/algorithm": ^2.0.0
-    "@lumino/commands": ^2.0.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
+    "@lumino/commands": ^2.1.1
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
-    "@lumino/polling": ^2.0.0
+    "@lumino/polling": ^2.1.1
     "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.0.0
+    "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
-    "@lumino/widgets": ^2.0.0
+    "@lumino/widgets": ^2.1.1
     "@rjsf/core": ^5.1.0
     "@rjsf/utils": ^5.1.0
     react: ^18.2.0
     react-dom: ^18.2.0
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
-  checksum: f4de4594a4c7301dc1fa055119284a119fbf0d16e6fb5f4e371f855f02a5b47ea148cec0bee4e5217a1c09bda4ad07542554bd6fcaa073e68d6d9409ceb346ad
+  checksum: 781a5b48acc16a098f9f88ec4cc840912100da96f9d1f64c93cd5fdb9afddd33bbeb891d0a6383ee8f12f001056d9c0beabded2a99a05d374dcf7d952e784e40
   languageName: node
   linkType: hard
 
 "@lerna/child-process@npm:6.6.1":
   version: 6.6.1
   resolution: "@lerna/child-process@npm:6.6.1"
   dependencies:
@@ -2722,27 +2904,27 @@
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: a7e4893aacaa7f26d5679c77a640f401b37d14155cb54863aa91b59dfd220b280360a341c0fedafc65d31101de13a5ae33cf3876c352f2da528344dafdc9b3d7
   languageName: node
   linkType: hard
 
-"@lezer/generator@npm:^1.0.0":
-  version: 1.2.2
-  resolution: "@lezer/generator@npm:1.2.2"
+"@lezer/generator@npm:^1.2.2":
+  version: 1.2.3
+  resolution: "@lezer/generator@npm:1.2.3"
   dependencies:
     "@lezer/common": ^1.0.2
     "@lezer/lr": ^1.3.0
   bin:
     lezer-generator: dist/lezer-generator.cjs
-  checksum: 62f93704d7b0b53bbd842c65552b9089f354edbf5f50f05d65a214a5dba05c0a63c898ca448a93ecc803d5b8b05d5eb593a5e5509c478c8dfa3b49ff28dcafb3
+  checksum: 300edf525f15ff27b84c366f1e9e66d741222f4b206cf015851679d7d153f5653b205ed9c3241f8df225eb97cefc99207343e148fe26bf2c4f636a00839976a8
   languageName: node
   linkType: hard
 
-"@lezer/highlight@npm:^1.0.0, @lezer/highlight@npm:^1.1.3":
+"@lezer/highlight@npm:^1.0.0, @lezer/highlight@npm:^1.1.3, @lezer/highlight@npm:^1.1.4":
   version: 1.1.4
   resolution: "@lezer/highlight@npm:1.1.4"
   dependencies:
     "@lezer/common": ^1.0.0
   checksum: 30e848c02839bfcd9472fcd6e74d71cba12379cef38f27d0c6cab0e6831f92150cfc629d267a40cc31f84cf46ac0a935400163fdf931b2672c516bec29417485
   languageName: node
   linkType: hard
@@ -2765,43 +2947,43 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: 2fffea6627d130413ffad4e61040267974cca3167d98881b9e5b5e2455530de74a82c234d93603e92a4972fad314671453c49c0a76b0f4547c4617d671fd7b99
   languageName: node
   linkType: hard
 
 "@lezer/javascript@npm:^1.0.0":
-  version: 1.4.2
-  resolution: "@lezer/javascript@npm:1.4.2"
+  version: 1.4.3
+  resolution: "@lezer/javascript@npm:1.4.3"
   dependencies:
     "@lezer/highlight": ^1.1.3
     "@lezer/lr": ^1.3.0
-  checksum: 542261c297709babfe450de1233c13fe2f5b111678d280cb0f8304f12bcdae294cb43c0ac64bbd647e5039de3286f6f0715d120fb132bd5af778363d1f612a1f
+  checksum: 520dc2d84c84841ef554993c1c0dfe503487aa9be398ebcf617b51d06f99121841d4ca1cf25f3f53d00efa820ea778cc2271da425a606ac66e9f09a4c8cc6677
   languageName: node
   linkType: hard
 
 "@lezer/json@npm:^1.0.0":
   version: 1.0.0
   resolution: "@lezer/json@npm:1.0.0"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: c1ca0cdf681415b58a383a669944bed66da3aa830870d32d1e471d545cff0fe43d9ac8a0d2a318a96daa99cd5a645b1d58ba8fbdd2e8d7ca4d33a62c7582cbab
   languageName: node
   linkType: hard
 
 "@lezer/lr@npm:^1.0.0, @lezer/lr@npm:^1.1.0, @lezer/lr@npm:^1.3.0":
-  version: 1.3.3
-  resolution: "@lezer/lr@npm:1.3.3"
+  version: 1.3.4
+  resolution: "@lezer/lr@npm:1.3.4"
   dependencies:
     "@lezer/common": ^1.0.0
-  checksum: 1804074c794005a31c54d80ab72127f19ae5be29bb627c52bc001a57b1af97a9e62732ff13e3aeb7bc53b330202b6bd3747272c64d87f257dbba533e75a183a3
+  checksum: 58bc25a9ba891dc6ca713fc8768706935e65d6e54d79a8ddb40c742cc799e87eddf4f49a6d6566a649c4726a9ab79a4200d36c9351608285a9bee6cdf3b33341
   languageName: node
   linkType: hard
 
-"@lezer/markdown@npm:^1.0.0":
+"@lezer/markdown@npm:^1.0.0, @lezer/markdown@npm:^1.0.2":
   version: 1.0.2
   resolution: "@lezer/markdown@npm:1.0.2"
   dependencies:
     "@lezer/common": ^1.0.0
     "@lezer/highlight": ^1.0.0
   checksum: c4bbfcd8a5a9d924a7cf2b5e5e99c78e7705473cc59804070278b5cfcf478af9dd567025d0926cbf03e3ea6abb8f173425220d3107c05a2d7e0ca3fe3d5c92ef
   languageName: node
@@ -2814,20 +2996,20 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.1.0
   checksum: a847c255c030b4d38913ddf1d5bd7324d83be7ef8d1d244542870be03b9bf7dc71283afeb2415c40dfd188cb99f0cc44bad760b5f3b7c35c3b8e5e00253848fc
   languageName: node
   linkType: hard
 
 "@lezer/python@npm:^1.0.0":
-  version: 1.1.4
-  resolution: "@lezer/python@npm:1.1.4"
+  version: 1.1.5
+  resolution: "@lezer/python@npm:1.1.5"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: d525e15c75493d4a47eccb72cbdaf942fbc35e8eb2b2a998f12ec869b56a6a5be0a1065ec250ab228b2fdcf8d4b02115b06b0edcbfe72558f2ad8ad161f4d241
+  checksum: 0327b90d18135bcc6e0b13369074f6e4cbc3204f6b91e0ffac674a2f8e4d32a0ecb7450fa0974c066018f09ec4be2c6568a0fac219336696188363a8cf1c92a3
   languageName: node
   linkType: hard
 
 "@lezer/rust@npm:^1.0.0":
   version: 1.0.0
   resolution: "@lezer/rust@npm:1.0.0"
   dependencies:
@@ -2850,88 +3032,79 @@
 "@lumino/algorithm@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/algorithm@npm:2.0.0"
   checksum: 663edf536e94397b449c6a2643a735e602fbb396dec86b56ad1193a768dce27c6e7da5ad0384aa90086ea44cbb64dde3f9d565e9fd81858f1eb0c6b4253f3b94
   languageName: node
   linkType: hard
 
-"@lumino/application@npm:^2.0.0":
-  version: 2.0.1
-  resolution: "@lumino/application@npm:2.0.1"
+"@lumino/application@npm:^2.1.1":
+  version: 2.1.1
+  resolution: "@lumino/application@npm:2.1.1"
   dependencies:
-    "@lumino/commands": ^2.0.1
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/widgets": ^2.0.1
-  checksum: c389b6e35b614c14551963f864a50383ca3a51192adbbef8c208d9ed7d8cd526d5c498743f5e6ca0b7de362027b68324e1cde0c735b314326d21ced15edf8e7b
+    "@lumino/commands": ^2.1.1
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/widgets": ^2.1.1
+  checksum: 442a047e43a85b48189d15a5a322f39cac01b9bee7b252aa76579c53e503f2cf2100f2e3aff61cd1d92fef07f04c0a3a6680c475890e0923456e296ceb79a692
   languageName: node
   linkType: hard
 
 "@lumino/collections@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/collections@npm:2.0.0"
   dependencies:
     "@lumino/algorithm": ^2.0.0
   checksum: 4a7fc3571e92a1368a1ef01300ad7b6e0d4ff13cb78b89533d5962eea66d4a7550e15d8b80fa3ab1816b1a89382f35015f9dddf72ab04654c17e5b516b845d8f
   languageName: node
   linkType: hard
 
-"@lumino/commands@npm:^2.0.0, @lumino/commands@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@lumino/commands@npm:2.0.1"
+"@lumino/commands@npm:^2.1.0, @lumino/commands@npm:^2.1.1":
+  version: 2.1.1
+  resolution: "@lumino/commands@npm:2.1.1"
   dependencies:
     "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/keyboard": ^2.0.0
-    "@lumino/signaling": ^2.0.0
+    "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
-  checksum: cefc9bb4b7b61054f199b5bf35501765688eb2922af2610087f43e4bb5f6663ee8579fcf02e12d6083697456423ada67cae5b2d020daa0856c646d050b30d420
-  languageName: node
-  linkType: hard
-
-"@lumino/coreutils@npm:^1.11.0":
-  version: 1.12.1
-  resolution: "@lumino/coreutils@npm:1.12.1"
-  peerDependencies:
-    crypto: 1.0.1
-  checksum: 55f1b87997f8dd0af28ff23c2d4b3aa252e515b9d3bc91b350a5c6c8526ceae61b14b55dc0d8d01691c69d42974b3d559f2b49bc7ced0f474b8f5dc52b3e83ed
+  checksum: a076244e9c4f7a3c6dab02642fdd38dbbaab6e5754acaeeb84a5195dc5c2fc19343ba754c3a0f89c9b60f16c61cb793301cdb6e8d69bdc30e18ed7e32f40d524
   languageName: node
   linkType: hard
 
-"@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^1.11.0 || ^2.0.0-alpha.6, @lumino/coreutils@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/coreutils@npm:2.0.0"
-  checksum: 341b5f569b2804e9651ecec6a441a0a0a9153656cc9dc0480eff8bb1d667df92ee4d64421fbb1469f0f503cd2ce3428c61dd3e5d2eb163e2e21748c318fd7b9e
+"@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^2.1.0, @lumino/coreutils@npm:^2.1.1":
+  version: 2.1.1
+  resolution: "@lumino/coreutils@npm:2.1.1"
+  checksum: dfdeb2b0282caae17b6c3edfebadf4ce7c75fc879fa60cacfef9b154412f4b35e4ffd95b1833b99d8dacb99aaaa04513570129ae2024c3f33e2677a01f0576ce
   languageName: node
   linkType: hard
 
-"@lumino/disposable@npm:^1.10.0 || ^2.0.0, @lumino/disposable@npm:^1.10.0 || ^2.0.0-alpha.6, @lumino/disposable@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/disposable@npm:2.0.0"
+"@lumino/disposable@npm:^1.10.0 || ^2.0.0, @lumino/disposable@npm:^2.1.0, @lumino/disposable@npm:^2.1.1":
+  version: 2.1.1
+  resolution: "@lumino/disposable@npm:2.1.1"
   dependencies:
-    "@lumino/signaling": ^2.0.0
-  checksum: d12ad6e3c72fdb869566374a89250678951a4138ed0e80478976a035ca5c48e0de06300fb6ad5cb9d3fc9694058e3b3367653dc63829ee3e67503a03e2252ccc
+    "@lumino/signaling": ^2.1.1
+  checksum: ed6cdfe13f3346178a087690d4e7baeccaed7e73ca23cb239765202409f5c01b4729a4058b4717f963462ee9ef2e5cb14ad1974e3163741267290edc3715c85c
   languageName: node
   linkType: hard
 
 "@lumino/domutils@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/domutils@npm:2.0.0"
   checksum: 4a146bfc1006d5fd00ccecc61d9803965d269c15c48c892fd87216336ce967f0db91f31203c5616c83d260224cddf25af4abb6704a6770757d19e44068f690bf
   languageName: node
   linkType: hard
 
-"@lumino/dragdrop@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/dragdrop@npm:2.0.0"
+"@lumino/dragdrop@npm:^2.1.1":
+  version: 2.1.1
+  resolution: "@lumino/dragdrop@npm:2.1.1"
   dependencies:
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
-  checksum: 37d605582a51877febc74a05ecf563bb3aeded1c570139a4fd86c046c8f050b605ce48da2e17a6998790e8dcd0a38fbb7cbe281ffd5efb8697ad3699c2ad9442
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+  checksum: 68c896afc44476b11a501e5b30ec55db06c2648a45f078713a111b2bf3b2e9171a7c5478ff6bdeb771a7c1e397fe3bba7bc5eadb4fe3e1294851d677f811b5b8
   languageName: node
   linkType: hard
 
 "@lumino/keyboard@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/keyboard@npm:2.0.0"
   checksum: 3852ba51f437b1c1d7e552a0f844592a05e04dd5012070dc6e4384c58965d1ebf536c6875c1b7bae03cde3c715ddc36cd290992fcefc1a8c39094194f4689fdd
@@ -2944,67 +3117,67 @@
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/collections": ^2.0.0
   checksum: 1e82dcf9b110834d4342dc63dfeac0ee780880fb99051bd82d00a1f83afd91b276c1cea5af85a414d92c527adc365d54f20ec780123b562f89c5a2cd3e96bf81
   languageName: node
   linkType: hard
 
-"@lumino/polling@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/polling@npm:2.0.0"
+"@lumino/polling@npm:^2.1.1":
+  version: 2.1.1
+  resolution: "@lumino/polling@npm:2.1.1"
   dependencies:
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
-    "@lumino/signaling": ^2.0.0
-  checksum: f62916ad474f1be50124a9adf2c717c588fbf486c318465b10c6517e0245ad76276c3b82a5e0353f73ac92c55bc0966fd85a58c1381827ba68bf8b791705b7ee
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/signaling": ^2.1.1
+  checksum: 69177b26d5fc541e72533cbe7d7f7999eea541d392f1082d20dbd9e1797e7d46fba47bae9c65c06f9ccb2780cbae636e9354d9bf4423b5e1020754d4b07d4f6b
   languageName: node
   linkType: hard
 
 "@lumino/properties@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/properties@npm:2.0.0"
   checksum: 81187a11a779eed4e20ff0035e77dee99bd271b0cf649096c4e8809dd6bdd06955b1a974bc1a115e536f8d2840b30183bb78a362b2c6991824477df6d17e6c59
   languageName: node
   linkType: hard
 
-"@lumino/signaling@npm:^1.10.0 || ^2.0.0, @lumino/signaling@npm:^1.10.0 || ^2.0.0-alpha.6, @lumino/signaling@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/signaling@npm:2.0.0"
+"@lumino/signaling@npm:^1.10.0 || ^2.0.0, @lumino/signaling@npm:^2.1.0, @lumino/signaling@npm:^2.1.1":
+  version: 2.1.1
+  resolution: "@lumino/signaling@npm:2.1.1"
   dependencies:
     "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.0.0
-  checksum: fb46a1b33c4a0cec723e8c6f1a9b6e89544ee1a3b94731437639c0e9a1a29c07ff225179081846ee16c5001bf11bcaace646d1307bbb76ea6ae04006f442cd28
+    "@lumino/coreutils": ^2.1.1
+  checksum: 283ad4239b8577f68aca3d0b2606f73cc1c775f84cab25cf49aa6cd195f0d87949ef43fdff03b38b5a49ebbf2468581c6786d5f8b6159a04b2051260be5eab86
   languageName: node
   linkType: hard
 
 "@lumino/virtualdom@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/virtualdom@npm:2.0.0"
   dependencies:
     "@lumino/algorithm": ^2.0.0
   checksum: 6fc1d88e7d4a656be7664ccfc5745eb1d4e3d2034db0b11ad6abefcc642f22d265003eef0e1d02bca2e42b6da127123118c631369006f78e88a08885a6f36c25
   languageName: node
   linkType: hard
 
-"@lumino/widgets@npm:^2.0.0, @lumino/widgets@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@lumino/widgets@npm:2.0.1"
+"@lumino/widgets@npm:^2.1.0, @lumino/widgets@npm:^2.1.1":
+  version: 2.1.1
+  resolution: "@lumino/widgets@npm:2.1.1"
   dependencies:
     "@lumino/algorithm": ^2.0.0
-    "@lumino/commands": ^2.0.1
-    "@lumino/coreutils": ^2.0.0
-    "@lumino/disposable": ^2.0.0
+    "@lumino/commands": ^2.1.1
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
-    "@lumino/dragdrop": ^2.0.0
+    "@lumino/dragdrop": ^2.1.1
     "@lumino/keyboard": ^2.0.0
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.0.0
+    "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
-  checksum: 5cb54991f269a3ac3517aea20d960cf9340739067a8c11ce3c601d725fe1db841a576a84e316b73f2b35c243f0fa6da98f4cdfe397ce49e05ae886ca38a037e0
+  checksum: e2ad4a97d6ec43e5e1863c2a521b6b8cb7a708a470c1e78b0f34ff4ad8b9fca191597586c3033233a29ff0fa14b62aeef5ea2fe66af3058d39e711c6af129cf4
   languageName: node
   linkType: hard
 
 "@nodelib/fs.scandir@npm:2.1.5":
   version: 2.1.5
   resolution: "@nodelib/fs.scandir@npm:2.1.5"
   dependencies:
@@ -3237,40 +3410,27 @@
   resolution: "@npmcli/query@npm:3.0.0"
   dependencies:
     postcss-selector-parser: ^6.0.10
   checksum: 90fca7edd5f3e59e875dd8729e6c3aa174292e5b66caa0d7db85841cc5eeb414c7eb7d7637d30f638605d05e1238e718d09b8c1a251f43cfc21d9ac6835c7b39
   languageName: node
   linkType: hard
 
-"@npmcli/run-script@npm:4.1.7":
+"@npmcli/run-script@npm:4.1.7, @npmcli/run-script@npm:^4.1.0":
   version: 4.1.7
   resolution: "@npmcli/run-script@npm:4.1.7"
   dependencies:
     "@npmcli/node-gyp": ^2.0.0
     "@npmcli/promise-spawn": ^3.0.0
     node-gyp: ^9.0.0
     read-package-json-fast: ^2.0.3
     which: ^2.0.2
   checksum: 87c32b12fed981fe8a48de985dd1ae0350bcda2830ca4a35efe4b2b96932905cccd04e6e2de5bfea8ed4e2bf3b6f8315630ff9a09c72f80ff3c49f19a9fc80ff
   languageName: node
   linkType: hard
 
-"@npmcli/run-script@npm:^4.1.0":
-  version: 4.2.1
-  resolution: "@npmcli/run-script@npm:4.2.1"
-  dependencies:
-    "@npmcli/node-gyp": ^2.0.0
-    "@npmcli/promise-spawn": ^3.0.0
-    node-gyp: ^9.0.0
-    read-package-json-fast: ^2.0.3
-    which: ^2.0.2
-  checksum: 7b8d6676353f157e68b26baf848e01e5d887bcf90ce81a52f23fc9a5d93e6ffb60057532d664cfd7aeeb76d464d0c8b0d314ee6cccb56943acb3b6c570b756c8
-  languageName: node
-  linkType: hard
-
 "@npmcli/run-script@npm:^6.0.0":
   version: 6.0.0
   resolution: "@npmcli/run-script@npm:6.0.0"
   dependencies:
     "@npmcli/node-gyp": ^3.0.0
     "@npmcli/promise-spawn": ^6.0.0
     node-gyp: ^9.0.0
@@ -3568,41 +3728,41 @@
   peerDependencies:
     typescript: ^3 || ^4
   checksum: 64eb6d90aafa889f62fe73d128b7be2b3295dffde4d5dff63bad75d512b6bc1d8419d8fc784a1a60b45aba4cda2eaf6e233bf59797a1d91b26fac27d99dae047
   languageName: node
   linkType: hard
 
 "@rjsf/core@npm:^5.1.0":
-  version: 5.4.0
-  resolution: "@rjsf/core@npm:5.4.0"
+  version: 5.6.2
+  resolution: "@rjsf/core@npm:5.6.2"
   dependencies:
-    lodash: ^4.17.15
-    lodash-es: ^4.17.15
+    lodash: ^4.17.21
+    lodash-es: ^4.17.21
     markdown-to-jsx: ^7.2.0
-    nanoid: ^3.3.4
-    prop-types: ^15.7.2
+    nanoid: ^3.3.6
+    prop-types: ^15.8.1
   peerDependencies:
-    "@rjsf/utils": ^5.0.0
+    "@rjsf/utils": 5.6.x
     react: ^16.14.0 || >=17
-  checksum: 3d0a2bd0814c8aae3ffb524a0d53ba9141475bcf63975b9a5409602ab9d3ce60f0bdc49c86cff7e30b0d1468562e74a8d5ec2a61b9e5329cf9ef57dcdf227167
+  checksum: 8cc9c1a439fcb232be66464aa1bc370b49dc0f872ae09cca296adf07ea993cb8dbec366c26414ff2ea92490f89fafd39ca5fb2369b424ff0035cbf045de44927
   languageName: node
   linkType: hard
 
 "@rjsf/utils@npm:^5.1.0":
-  version: 5.4.0
-  resolution: "@rjsf/utils@npm:5.4.0"
+  version: 5.6.2
+  resolution: "@rjsf/utils@npm:5.6.2"
   dependencies:
     json-schema-merge-allof: ^0.8.1
     jsonpointer: ^5.0.1
-    lodash: ^4.17.15
-    lodash-es: ^4.17.15
+    lodash: ^4.17.21
+    lodash-es: ^4.17.21
     react-is: ^18.2.0
   peerDependencies:
     react: ^16.14.0 || >=17
-  checksum: 096283446b100dec731d06abc0a758588138321c930194cc6bb5c4d2def7be28e058eba3ab2741b30421d1c095c3f700a349d3f6d69d2c0b903f2695b855afe6
+  checksum: f6ab90d2cf383f8f7d14ba70f51b2e0171997aeee1f822115734ec39d0f208477374046e4cc2b4cbabe544f8bb6a6250f0bd5fb9e9470aae876a0896eabfa23e
   languageName: node
   linkType: hard
 
 "@sigstore/protobuf-specs@npm:^0.1.0":
   version: 0.1.0
   resolution: "@sigstore/protobuf-specs@npm:0.1.0"
   checksum: 9959bc5176906609dda6ad2a1f5226fac1e49fcb4d29f38969d2a2e3a05cba8e2479721ba78c46a507513abacb63f25a991e5e8856c300204cded455f34ba8c5
@@ -3707,25 +3867,18 @@
   dependencies:
     "@types/estree": "*"
     "@types/json-schema": "*"
   checksum: 06d3b3fba12004294591b5c7a52e3cec439472195da54e096076b1f2ddfbb8a445973b9681046dd530a6ac31eca502f635abc1e3ce37d03513089358e6f822ee
   languageName: node
   linkType: hard
 
-"@types/estree@npm:*":
-  version: 1.0.0
-  resolution: "@types/estree@npm:1.0.0"
-  checksum: 910d97fb7092c6738d30a7430ae4786a38542023c6302b95d46f49420b797f21619cdde11fa92b338366268795884111c2eb10356e4bd2c8ad5b92941e9e6443
-  languageName: node
-  linkType: hard
-
-"@types/estree@npm:^0.0.51":
-  version: 0.0.51
-  resolution: "@types/estree@npm:0.0.51"
-  checksum: e56a3bcf759fd9185e992e7fdb3c6a5f81e8ff120e871641607581fb3728d16c811702a7d40fa5f869b7f7b4437ab6a87eb8d98ffafeee51e85bbe955932a189
+"@types/estree@npm:*, @types/estree@npm:^1.0.0":
+  version: 1.0.1
+  resolution: "@types/estree@npm:1.0.1"
+  checksum: e9aa175eacb797216fafce4d41e8202c7a75555bc55232dee0f9903d7171f8f19f0ae7d5191bb1a88cb90e65468be508c0df850a9fb81b4433b293a5a749899d
   languageName: node
   linkType: hard
 
 "@types/graceful-fs@npm:^4.1.3":
   version: 4.1.6
   resolution: "@types/graceful-fs@npm:4.1.6"
   dependencies:
@@ -3833,21 +3986,32 @@
   version: 15.7.5
   resolution: "@types/prop-types@npm:15.7.5"
   checksum: 5b43b8b15415e1f298243165f1d44390403bb2bd42e662bca3b5b5633fdd39c938e91b7fce3a9483699db0f7a715d08cef220c121f723a634972fdf596aec980
   languageName: node
   linkType: hard
 
 "@types/react@npm:^18.0.26, @types/react@npm:^18.0.27":
-  version: 18.0.31
-  resolution: "@types/react@npm:18.0.31"
+  version: 18.2.6
+  resolution: "@types/react@npm:18.2.6"
   dependencies:
     "@types/prop-types": "*"
     "@types/scheduler": "*"
     csstype: ^3.0.2
-  checksum: 6befbd5587e266905b50fd6bbd7c1cacd557bddf99e6a9862ca2f1d06df3dca71b9d485a37d010479730f021aab93b852d417c714de5efc2f41be0ff4c09b4db
+  checksum: dea9d232d8df7ac357367a69dcb557711ab3d5501807ffa77cebeee73d49ee94d095f298e36853c63ed47cce097eee4c7eae2aaa8c02fac3f0171ec1b523a819
+  languageName: node
+  linkType: hard
+
+"@types/react@npm:~18.0.26":
+  version: 18.0.38
+  resolution: "@types/react@npm:18.0.38"
+  dependencies:
+    "@types/prop-types": "*"
+    "@types/scheduler": "*"
+    csstype: ^3.0.2
+  checksum: 34481c79f4f7ea2aefbaa45281319dc183200230d932d968463eba1643bd3635073d0a17c5c613150a69e36ca18b811ecffafea6384fa3dff3b5203866339d69
   languageName: node
   linkType: hard
 
 "@types/scheduler@npm:*":
   version: 0.16.3
   resolution: "@types/scheduler@npm:0.16.3"
   checksum: 2b0aec39c24268e3ce938c5db2f2e77f5c3dd280e05c262d9c2fe7d890929e4632a6b8e94334017b66b45e4f92a5aa42ba3356640c2a1175fa37bef2f5200767
@@ -3956,24 +4120,14 @@
   dependencies:
     "@typescript-eslint/types": 5.55.0
     "@typescript-eslint/visitor-keys": 5.55.0
   checksum: f253db88f69a29e4abe2f567d0a611cc3e7fb1a911a2cc54a2f6baf16e3de4d1883b3f8e45ee61b3db9fa5543dda0fd7b608de9d28ba6173ab49bfd17ff90cad
   languageName: node
   linkType: hard
 
-"@typescript-eslint/scope-manager@npm:5.57.0":
-  version: 5.57.0
-  resolution: "@typescript-eslint/scope-manager@npm:5.57.0"
-  dependencies:
-    "@typescript-eslint/types": 5.57.0
-    "@typescript-eslint/visitor-keys": 5.57.0
-  checksum: 4a851f23da2adbf6341b04c1e3f19fcb66415683f26805d3123725d18845bd4a150bd182de0a91279d5682f2568bb5dd831d4ad0bdb70f49d9ca7381cec4dd17
-  languageName: node
-  linkType: hard
-
 "@typescript-eslint/type-utils@npm:5.55.0":
   version: 5.55.0
   resolution: "@typescript-eslint/type-utils@npm:5.55.0"
   dependencies:
     "@typescript-eslint/typescript-estree": 5.55.0
     "@typescript-eslint/utils": 5.55.0
     debug: ^4.3.4
@@ -3990,21 +4144,14 @@
 "@typescript-eslint/types@npm:5.55.0":
   version: 5.55.0
   resolution: "@typescript-eslint/types@npm:5.55.0"
   checksum: 7d851f09a2106514d3a9c7164d34758f30abfe554e3c7a02be75cdc7e16644e23ca32840a8f39a0321bc509927fb4d98ce91b22b21e8544ac56cef33b815a864
   languageName: node
   linkType: hard
 
-"@typescript-eslint/types@npm:5.57.0":
-  version: 5.57.0
-  resolution: "@typescript-eslint/types@npm:5.57.0"
-  checksum: 79a100fb650965f63c01c20e6abd79ca0d2043c3a329b9fef89917d6b9ba3c0f946dca3f14f2975ee6349daadd6ce0e98fde3aafe4b710e5a27abe1adc590c85
-  languageName: node
-  linkType: hard
-
 "@typescript-eslint/typescript-estree@npm:5.55.0":
   version: 5.55.0
   resolution: "@typescript-eslint/typescript-estree@npm:5.55.0"
   dependencies:
     "@typescript-eslint/types": 5.55.0
     "@typescript-eslint/visitor-keys": 5.55.0
     debug: ^4.3.4
@@ -4015,33 +4162,15 @@
   peerDependenciesMeta:
     typescript:
       optional: true
   checksum: d24a11aee3d01067018d99804f420aecb8af88e43bf170d5d14f6480bd378c0a81ce49a37f5d6c36e5f0f319e3fa8b099720f295f2767338be1a4f7e9a5323e1
   languageName: node
   linkType: hard
 
-"@typescript-eslint/typescript-estree@npm:5.57.0":
-  version: 5.57.0
-  resolution: "@typescript-eslint/typescript-estree@npm:5.57.0"
-  dependencies:
-    "@typescript-eslint/types": 5.57.0
-    "@typescript-eslint/visitor-keys": 5.57.0
-    debug: ^4.3.4
-    globby: ^11.1.0
-    is-glob: ^4.0.3
-    semver: ^7.3.7
-    tsutils: ^3.21.0
-  peerDependenciesMeta:
-    typescript:
-      optional: true
-  checksum: 648b88f88ea6cc293ec67b4c0f4f3c2bf733be7e0f2eee08aadbaec6939fd724a6c287decc336abbf67b9e366cc2c48f2e0e48d8302b533e783f798332a06e83
-  languageName: node
-  linkType: hard
-
-"@typescript-eslint/utils@npm:5.55.0":
+"@typescript-eslint/utils@npm:5.55.0, @typescript-eslint/utils@npm:^5.10.0":
   version: 5.55.0
   resolution: "@typescript-eslint/utils@npm:5.55.0"
   dependencies:
     "@eslint-community/eslint-utils": ^4.2.0
     "@types/json-schema": ^7.0.9
     "@types/semver": ^7.3.12
     "@typescript-eslint/scope-manager": 5.55.0
@@ -4051,233 +4180,205 @@
     semver: ^7.3.7
   peerDependencies:
     eslint: ^6.0.0 || ^7.0.0 || ^8.0.0
   checksum: 368cfc3fb9d6af6901e739e2e41c3f7f1c1244576607445f4f59d95eccb237f73e1a75e7f0816ec9a32a0f1ec6bb4a3602a99e17e70fe184e62f7c69dcbe4b8d
   languageName: node
   linkType: hard
 
-"@typescript-eslint/utils@npm:^5.10.0":
-  version: 5.57.0
-  resolution: "@typescript-eslint/utils@npm:5.57.0"
-  dependencies:
-    "@eslint-community/eslint-utils": ^4.2.0
-    "@types/json-schema": ^7.0.9
-    "@types/semver": ^7.3.12
-    "@typescript-eslint/scope-manager": 5.57.0
-    "@typescript-eslint/types": 5.57.0
-    "@typescript-eslint/typescript-estree": 5.57.0
-    eslint-scope: ^5.1.1
-    semver: ^7.3.7
-  peerDependencies:
-    eslint: ^6.0.0 || ^7.0.0 || ^8.0.0
-  checksum: 461258e1194d24c5e642c65ba1afd612712fa8e617ac85cfbbe3dde2557fe4abadedbce19a6954ae0cccbfb92b8a09f38d65a3eedca0394861a5d1c4c893c5ed
-  languageName: node
-  linkType: hard
-
 "@typescript-eslint/visitor-keys@npm:5.55.0":
   version: 5.55.0
   resolution: "@typescript-eslint/visitor-keys@npm:5.55.0"
   dependencies:
     "@typescript-eslint/types": 5.55.0
     eslint-visitor-keys: ^3.3.0
   checksum: 0b24c72dff99dd2cf41c19d20067f8ab20a38aa2e82c79c5530bec7cf651031e95c80702fc21c813c9b94e5f3d4cd210f13967b2966ef38abe548cb5f05848a3
   languageName: node
   linkType: hard
 
-"@typescript-eslint/visitor-keys@npm:5.57.0":
-  version: 5.57.0
-  resolution: "@typescript-eslint/visitor-keys@npm:5.57.0"
-  dependencies:
-    "@typescript-eslint/types": 5.57.0
-    eslint-visitor-keys: ^3.3.0
-  checksum: 77d53f74648e48bf1c6313cd60568c2b1539157ac13945f26204a54beb156666c24f3d033dd0db8ed5d1d4595ee63c072732b17132e4488b46763bf8fdcefa49
-  languageName: node
-  linkType: hard
-
-"@webassemblyjs/ast@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/ast@npm:1.11.1"
+"@webassemblyjs/ast@npm:1.11.6, @webassemblyjs/ast@npm:^1.11.5":
+  version: 1.11.6
+  resolution: "@webassemblyjs/ast@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/helper-numbers": 1.11.1
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.1
-  checksum: 1eee1534adebeece635362f8e834ae03e389281972611408d64be7895fc49f48f98fddbbb5339bf8a72cb101bcb066e8bca3ca1bf1ef47dadf89def0395a8d87
+    "@webassemblyjs/helper-numbers": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+  checksum: 38ef1b526ca47c210f30975b06df2faf1a8170b1636ce239fc5738fc231ce28389dd61ecedd1bacfc03cbe95b16d1af848c805652080cb60982836eb4ed2c6cf
   languageName: node
   linkType: hard
 
-"@webassemblyjs/floating-point-hex-parser@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/floating-point-hex-parser@npm:1.11.1"
-  checksum: b8efc6fa08e4787b7f8e682182d84dfdf8da9d9c77cae5d293818bc4a55c1f419a87fa265ab85252b3e6c1fd323d799efea68d825d341a7c365c64bc14750e97
+"@webassemblyjs/floating-point-hex-parser@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/floating-point-hex-parser@npm:1.11.6"
+  checksum: 29b08758841fd8b299c7152eda36b9eb4921e9c584eb4594437b5cd90ed6b920523606eae7316175f89c20628da14326801090167cc7fbffc77af448ac84b7e2
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-api-error@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/helper-api-error@npm:1.11.1"
-  checksum: 0792813f0ed4a0e5ee0750e8b5d0c631f08e927f4bdfdd9fe9105dc410c786850b8c61bff7f9f515fdfb149903bec3c976a1310573a4c6866a94d49bc7271959
+"@webassemblyjs/helper-api-error@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-api-error@npm:1.11.6"
+  checksum: e8563df85161096343008f9161adb138a6e8f3c2cc338d6a36011aa55eabb32f2fd138ffe63bc278d009ada001cc41d263dadd1c0be01be6c2ed99076103689f
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-buffer@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/helper-buffer@npm:1.11.1"
-  checksum: a337ee44b45590c3a30db5a8b7b68a717526cf967ada9f10253995294dbd70a58b2da2165222e0b9830cd4fc6e4c833bf441a721128d1fe2e9a7ab26b36003ce
+"@webassemblyjs/helper-buffer@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-buffer@npm:1.11.6"
+  checksum: b14d0573bf680d22b2522e8a341ec451fddd645d1f9c6bd9012ccb7e587a2973b86ab7b89fe91e1c79939ba96095f503af04369a3b356c8023c13a5893221644
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-numbers@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/helper-numbers@npm:1.11.1"
+"@webassemblyjs/helper-numbers@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-numbers@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/floating-point-hex-parser": 1.11.1
-    "@webassemblyjs/helper-api-error": 1.11.1
+    "@webassemblyjs/floating-point-hex-parser": 1.11.6
+    "@webassemblyjs/helper-api-error": 1.11.6
     "@xtuc/long": 4.2.2
-  checksum: 44d2905dac2f14d1e9b5765cf1063a0fa3d57295c6d8930f6c59a36462afecc6e763e8a110b97b342a0f13376166c5d41aa928e6ced92e2f06b071fd0db59d3a
+  checksum: f4b562fa219f84368528339e0f8d273ad44e047a07641ffcaaec6f93e5b76fd86490a009aa91a294584e1436d74b0a01fa9fde45e333a4c657b58168b04da424
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-wasm-bytecode@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/helper-wasm-bytecode@npm:1.11.1"
-  checksum: eac400113127832c88f5826bcc3ad1c0db9b3dbd4c51a723cfdb16af6bfcbceb608170fdaac0ab7731a7e18b291be7af68a47fcdb41cfe0260c10857e7413d97
+"@webassemblyjs/helper-wasm-bytecode@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-wasm-bytecode@npm:1.11.6"
+  checksum: 3535ef4f1fba38de3475e383b3980f4bbf3de72bbb631c2b6584c7df45be4eccd62c6ff48b5edd3f1bcff275cfd605a37679ec199fc91fd0a7705d7f1e3972dc
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-wasm-section@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/helper-wasm-section@npm:1.11.1"
+"@webassemblyjs/helper-wasm-section@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-wasm-section@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.1
-    "@webassemblyjs/helper-buffer": 1.11.1
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.1
-    "@webassemblyjs/wasm-gen": 1.11.1
-  checksum: 617696cfe8ecaf0532763162aaf748eb69096fb27950219bb87686c6b2e66e11cd0614d95d319d0ab1904bc14ebe4e29068b12c3e7c5e020281379741fe4bedf
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+    "@webassemblyjs/wasm-gen": 1.11.6
+  checksum: b2cf751bf4552b5b9999d27bbb7692d0aca75260140195cb58ea6374d7b9c2dc69b61e10b211a0e773f66209c3ddd612137ed66097e3684d7816f854997682e9
   languageName: node
   linkType: hard
 
-"@webassemblyjs/ieee754@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/ieee754@npm:1.11.1"
+"@webassemblyjs/ieee754@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/ieee754@npm:1.11.6"
   dependencies:
     "@xtuc/ieee754": ^1.2.0
-  checksum: 23a0ac02a50f244471631802798a816524df17e56b1ef929f0c73e3cde70eaf105a24130105c60aff9d64a24ce3b640dad443d6f86e5967f922943a7115022ec
+  checksum: 13574b8e41f6ca39b700e292d7edf102577db5650fe8add7066a320aa4b7a7c09a5056feccac7a74eb68c10dea9546d4461412af351f13f6b24b5f32379b49de
   languageName: node
   linkType: hard
 
-"@webassemblyjs/leb128@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/leb128@npm:1.11.1"
+"@webassemblyjs/leb128@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/leb128@npm:1.11.6"
   dependencies:
     "@xtuc/long": 4.2.2
-  checksum: 33ccc4ade2f24de07bf31690844d0b1ad224304ee2062b0e464a610b0209c79e0b3009ac190efe0e6bd568b0d1578d7c3047fc1f9d0197c92fc061f56224ff4a
+  checksum: 7ea942dc9777d4b18a5ebfa3a937b30ae9e1d2ce1fee637583ed7f376334dd1d4274f813d2e250056cca803e0952def4b954913f1a3c9068bcd4ab4ee5143bf0
   languageName: node
   linkType: hard
 
-"@webassemblyjs/utf8@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/utf8@npm:1.11.1"
-  checksum: 972c5cfc769d7af79313a6bfb96517253a270a4bf0c33ba486aa43cac43917184fb35e51dfc9e6b5601548cd5931479a42e42c89a13bb591ffabebf30c8a6a0b
+"@webassemblyjs/utf8@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/utf8@npm:1.11.6"
+  checksum: 807fe5b5ce10c390cfdd93e0fb92abda8aebabb5199980681e7c3743ee3306a75729bcd1e56a3903980e96c885ee53ef901fcbaac8efdfa480f9c0dae1d08713
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-edit@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/wasm-edit@npm:1.11.1"
+"@webassemblyjs/wasm-edit@npm:^1.11.5":
+  version: 1.11.6
+  resolution: "@webassemblyjs/wasm-edit@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.1
-    "@webassemblyjs/helper-buffer": 1.11.1
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.1
-    "@webassemblyjs/helper-wasm-section": 1.11.1
-    "@webassemblyjs/wasm-gen": 1.11.1
-    "@webassemblyjs/wasm-opt": 1.11.1
-    "@webassemblyjs/wasm-parser": 1.11.1
-    "@webassemblyjs/wast-printer": 1.11.1
-  checksum: 6d7d9efaec1227e7ef7585a5d7ff0be5f329f7c1c6b6c0e906b18ed2e9a28792a5635e450aca2d136770d0207225f204eff70a4b8fd879d3ac79e1dcc26dbeb9
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+    "@webassemblyjs/helper-wasm-section": 1.11.6
+    "@webassemblyjs/wasm-gen": 1.11.6
+    "@webassemblyjs/wasm-opt": 1.11.6
+    "@webassemblyjs/wasm-parser": 1.11.6
+    "@webassemblyjs/wast-printer": 1.11.6
+  checksum: 29ce75870496d6fad864d815ebb072395a8a3a04dc9c3f4e1ffdc63fc5fa58b1f34304a1117296d8240054cfdbc38aca88e71fb51483cf29ffab0a61ef27b481
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-gen@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/wasm-gen@npm:1.11.1"
+"@webassemblyjs/wasm-gen@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/wasm-gen@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.1
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.1
-    "@webassemblyjs/ieee754": 1.11.1
-    "@webassemblyjs/leb128": 1.11.1
-    "@webassemblyjs/utf8": 1.11.1
-  checksum: 1f6921e640293bf99fb16b21e09acb59b340a79f986c8f979853a0ae9f0b58557534b81e02ea2b4ef11e929d946708533fd0693c7f3712924128fdafd6465f5b
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+    "@webassemblyjs/ieee754": 1.11.6
+    "@webassemblyjs/leb128": 1.11.6
+    "@webassemblyjs/utf8": 1.11.6
+  checksum: a645a2eecbea24833c3260a249704a7f554ef4a94c6000984728e94bb2bc9140a68dfd6fd21d5e0bbb09f6dfc98e083a45760a83ae0417b41a0196ff6d45a23a
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-opt@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/wasm-opt@npm:1.11.1"
+"@webassemblyjs/wasm-opt@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/wasm-opt@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.1
-    "@webassemblyjs/helper-buffer": 1.11.1
-    "@webassemblyjs/wasm-gen": 1.11.1
-    "@webassemblyjs/wasm-parser": 1.11.1
-  checksum: 21586883a20009e2b20feb67bdc451bbc6942252e038aae4c3a08e6f67b6bae0f5f88f20bfc7bd0452db5000bacaf5ab42b98cf9aa034a6c70e9fc616142e1db
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/wasm-gen": 1.11.6
+    "@webassemblyjs/wasm-parser": 1.11.6
+  checksum: b4557f195487f8e97336ddf79f7bef40d788239169aac707f6eaa2fa5fe243557c2d74e550a8e57f2788e70c7ae4e7d32f7be16101afe183d597b747a3bdd528
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-parser@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/wasm-parser@npm:1.11.1"
+"@webassemblyjs/wasm-parser@npm:1.11.6, @webassemblyjs/wasm-parser@npm:^1.11.5":
+  version: 1.11.6
+  resolution: "@webassemblyjs/wasm-parser@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.1
-    "@webassemblyjs/helper-api-error": 1.11.1
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.1
-    "@webassemblyjs/ieee754": 1.11.1
-    "@webassemblyjs/leb128": 1.11.1
-    "@webassemblyjs/utf8": 1.11.1
-  checksum: 1521644065c360e7b27fad9f4bb2df1802d134dd62937fa1f601a1975cde56bc31a57b6e26408b9ee0228626ff3ba1131ae6f74ffb7d718415b6528c5a6dbfc2
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-api-error": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+    "@webassemblyjs/ieee754": 1.11.6
+    "@webassemblyjs/leb128": 1.11.6
+    "@webassemblyjs/utf8": 1.11.6
+  checksum: 8200a8d77c15621724a23fdabe58d5571415cda98a7058f542e670ea965dd75499f5e34a48675184947c66f3df23adf55df060312e6d72d57908e3f049620d8a
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wast-printer@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/wast-printer@npm:1.11.1"
+"@webassemblyjs/wast-printer@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/wast-printer@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.1
+    "@webassemblyjs/ast": 1.11.6
     "@xtuc/long": 4.2.2
-  checksum: f15ae4c2441b979a3b4fce78f3d83472fb22350c6dc3fd34bfe7c3da108e0b2360718734d961bba20e7716cb8578e964b870da55b035e209e50ec9db0378a3f7
+  checksum: d2fa6a4c427325ec81463e9c809aa6572af6d47f619f3091bf4c4a6fc34f1da3df7caddaac50b8e7a457f8784c62cd58c6311b6cb69b0162ccd8d4c072f79cf8
   languageName: node
   linkType: hard
 
-"@webpack-cli/configtest@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@webpack-cli/configtest@npm:2.0.1"
+"@webpack-cli/configtest@npm:^2.1.0":
+  version: 2.1.0
+  resolution: "@webpack-cli/configtest@npm:2.1.0"
   peerDependencies:
     webpack: 5.x.x
     webpack-cli: 5.x.x
-  checksum: 15d0ca835f2e16ec99e9f295f07b676435b9e706d7700df0ad088692fea065e34772fc44b96a4f6a86178b9ca8cf1ff941fbce15269587cf0925d70b18928cea
+  checksum: b875fccd8be9a936924e24986725823347703e3eb72ea884e74669ca20f007704e859855a6a05940d5d3805ce2fc08b183a0f1658d5395b5454b3f5f88293081
   languageName: node
   linkType: hard
 
 "@webpack-cli/info@npm:^2.0.1":
   version: 2.0.1
   resolution: "@webpack-cli/info@npm:2.0.1"
   peerDependencies:
     webpack: 5.x.x
     webpack-cli: 5.x.x
   checksum: b8fba49fee10d297c2affb0b064c9a81e9038d75517c6728fb85f9fb254cae634e5d33e696dac5171e6944ae329d85fddac72f781c7d833f7e9dfe43151ce60d
   languageName: node
   linkType: hard
 
-"@webpack-cli/serve@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@webpack-cli/serve@npm:2.0.1"
+"@webpack-cli/serve@npm:^2.0.4":
+  version: 2.0.4
+  resolution: "@webpack-cli/serve@npm:2.0.4"
   peerDependencies:
     webpack: 5.x.x
     webpack-cli: 5.x.x
   peerDependenciesMeta:
     webpack-dev-server:
       optional: true
-  checksum: 75c55f8398dd60e4821f81bec6e96287cebb3ab1837ef016779bc2f0c76a1d29c45b99e53daa99ba1fa156b5e2b61c19abf58098de20c2b58391b1f496ecc145
+  checksum: 561ea2e6eb551415f0b1675393a8480e1201293fe37eae334cbb1fdc466986668cca76ca1ca327ada9b498eae27cbecef0793e3bb5677288f1a5216cad414efe
   languageName: node
   linkType: hard
 
 "@xtuc/ieee754@npm:^1.2.0":
   version: 1.2.0
   resolution: "@xtuc/ieee754@npm:1.2.0"
   checksum: ac56d4ca6e17790f1b1677f978c0c6808b1900a5b138885d3da21732f62e30e8f0d9120fcf8f6edfff5100ca902b46f8dd7c1e3f903728634523981e80e2885a
@@ -4357,28 +4458,15 @@
   resolution: "abort-controller@npm:3.0.0"
   dependencies:
     event-target-shim: ^5.0.0
   checksum: 170bdba9b47b7e65906a28c8ce4f38a7a369d78e2271706f020849c1bfe0ee2067d4261df8bbb66eb84f79208fd5b710df759d64191db58cfba7ce8ef9c54b75
   languageName: node
   linkType: hard
 
-"abstract-leveldown@npm:^6.2.1":
-  version: 6.3.0
-  resolution: "abstract-leveldown@npm:6.3.0"
-  dependencies:
-    buffer: ^5.5.0
-    immediate: ^3.2.3
-    level-concat-iterator: ~2.0.0
-    level-supports: ~1.0.0
-    xtend: ~4.0.0
-  checksum: 121a8509d8c6a540e656c2a69e5b8d853d4df71072011afefc868b98076991bb00120550e90643de9dc18889c675f62413409eeb4c8c204663124c7d215e4ec3
-  languageName: node
-  linkType: hard
-
-"abstract-leveldown@npm:~6.2.1, abstract-leveldown@npm:~6.2.3":
+"abstract-leveldown@npm:^6.2.1, abstract-leveldown@npm:~6.2.1, abstract-leveldown@npm:~6.2.3":
   version: 6.2.3
   resolution: "abstract-leveldown@npm:6.2.3"
   dependencies:
     buffer: ^5.5.0
     immediate: ^3.2.3
     level-concat-iterator: ~2.0.0
     level-supports: ~1.0.0
@@ -4487,15 +4575,15 @@
   resolution: "ajv-keywords@npm:3.5.2"
   peerDependencies:
     ajv: ^6.9.1
   checksum: 7dc5e5931677a680589050f79dcbe1fefbb8fea38a955af03724229139175b433c63c68f7ae5f86cf8f65d55eb7c25f75a046723e2e58296707617ca690feae9
   languageName: node
   linkType: hard
 
-"ajv-keywords@npm:^5.0.0":
+"ajv-keywords@npm:^5.1.0":
   version: 5.1.0
   resolution: "ajv-keywords@npm:5.1.0"
   dependencies:
     fast-deep-equal: ^3.1.3
   peerDependencies:
     ajv: ^8.8.2
   checksum: c35193940b853119242c6757787f09ecf89a2c19bcd36d03ed1a615e710d19d450cb448bfda407b939aba54b002368c8bff30529cc50a0536a8e10bcce300421
@@ -4510,15 +4598,15 @@
     fast-json-stable-stringify: ^2.0.0
     json-schema-traverse: ^0.4.1
     uri-js: ^4.2.2
   checksum: 874972efe5c4202ab0a68379481fbd3d1b5d0a7bd6d3cc21d40d3536ebff3352a2a1fabb632d4fd2cc7fe4cbdcd5ed6782084c9bbf7f32a1536d18f9da5007d4
   languageName: node
   linkType: hard
 
-"ajv@npm:^8.0.0, ajv@npm:^8.0.1, ajv@npm:^8.12.0, ajv@npm:^8.8.0":
+"ajv@npm:^8.0.0, ajv@npm:^8.0.1, ajv@npm:^8.12.0, ajv@npm:^8.9.0":
   version: 8.12.0
   resolution: "ajv@npm:8.12.0"
   dependencies:
     fast-deep-equal: ^3.1.1
     json-schema-traverse: ^1.0.0
     require-from-string: ^2.0.2
     uri-js: ^4.2.2
@@ -5245,28 +5333,21 @@
   resolution: "cli-cursor@npm:3.1.0"
   dependencies:
     restore-cursor: ^3.1.0
   checksum: 2692784c6cd2fd85cfdbd11f53aea73a463a6d64a77c3e098b2b4697a20443f430c220629e1ca3b195ea5ac4a97a74c2ee411f3807abf6df2b66211fec0c0a29
   languageName: node
   linkType: hard
 
-"cli-spinners@npm:2.6.1":
+"cli-spinners@npm:2.6.1, cli-spinners@npm:^2.5.0":
   version: 2.6.1
   resolution: "cli-spinners@npm:2.6.1"
   checksum: 423409baaa7a58e5104b46ca1745fbfc5888bbd0b0c5a626e052ae1387060839c8efd512fb127e25769b3dc9562db1dc1b5add6e0b93b7ef64f477feb6416a45
   languageName: node
   linkType: hard
 
-"cli-spinners@npm:^2.5.0":
-  version: 2.7.0
-  resolution: "cli-spinners@npm:2.7.0"
-  checksum: a9afaf73f58d1f951fb23742f503631b3cf513f43f4c7acb1b640100eb76bfa16efbcd1994d149ffc6603a6d75dd3d4a516a76f125f90dce437de9b16fd0ee6f
-  languageName: node
-  linkType: hard
-
 "cli-width@npm:^3.0.0":
   version: 3.0.0
   resolution: "cli-width@npm:3.0.0"
   checksum: 4c94af3769367a70e11ed69aa6095f1c600c0ff510f3921ab4045af961820d57c0233acfa8b6396037391f31b4c397e1f614d234294f979ff61430a6c166c3f6
   languageName: node
   linkType: hard
 
@@ -5410,14 +5491,21 @@
   resolution: "combined-stream@npm:1.0.8"
   dependencies:
     delayed-stream: ~1.0.0
   checksum: 49fa4aeb4916567e33ea81d088f6584749fc90c7abec76fd516bf1c5aa5c79f3584b5ba3de6b86d26ddd64bae5329c4c7479343250cfe71c75bb366eae53bb7c
   languageName: node
   linkType: hard
 
+"commander@npm:^10.0.1":
+  version: 10.0.1
+  resolution: "commander@npm:10.0.1"
+  checksum: 436901d64a818295803c1996cd856621a74f30b9f9e28a588e726b2b1670665bccd7c1a77007ebf328729f0139838a88a19265858a0fa7a8728c4656796db948
+  languageName: node
+  linkType: hard
+
 "commander@npm:^2.20.0":
   version: 2.20.3
   resolution: "commander@npm:2.20.3"
   checksum: ab8c07884e42c3a8dbc5dd9592c606176c7eb5c1ca5ff274bcf907039b2c41de3626f684ea75ccf4d361ba004bbaff1f577d5384c155f3871e456bdf27becf9e
   languageName: node
   linkType: hard
 
@@ -5762,28 +5850,21 @@
   resolution: "cssstyle@npm:2.3.0"
   dependencies:
     cssom: ~0.3.6
   checksum: 5f05e6fd2e3df0b44695c2f08b9ef38b011862b274e320665176467c0725e44a53e341bc4959a41176e83b66064ab786262e7380fd1cabeae6efee0d255bb4e3
   languageName: node
   linkType: hard
 
-"csstype@npm:3.0.10":
+"csstype@npm:3.0.10, csstype@npm:^3.0.2":
   version: 3.0.10
   resolution: "csstype@npm:3.0.10"
   checksum: 20a8fa324f2b33ddf94aa7507d1b6ab3daa6f3cc308888dc50126585d7952f2471de69b2dbe0635d1fdc31223fef8e070842691877e725caf456e2378685a631
   languageName: node
   linkType: hard
 
-"csstype@npm:^3.0.2":
-  version: 3.1.1
-  resolution: "csstype@npm:3.1.1"
-  checksum: 1f7b4f5fdd955b7444b18ebdddf3f5c699159f13e9cf8ac9027ae4a60ae226aef9bbb14a6e12ca7dba3358b007cee6354b116e720262867c398de6c955ea451d
-  languageName: node
-  linkType: hard
-
 "dargs@npm:^7.0.0":
   version: 7.0.0
   resolution: "dargs@npm:7.0.0"
   checksum: b8f1e3cba59c42e1f13a114ad4848c3fc1cf7470f633ee9e9f1043762429bc97d91ae31b826fb135eefde203a3fdb20deb0c0a0222ac29d937b8046085d668d1
   languageName: node
   linkType: hard
 
@@ -5895,15 +5976,15 @@
 "define-lazy-prop@npm:^2.0.0":
   version: 2.0.0
   resolution: "define-lazy-prop@npm:2.0.0"
   checksum: 0115fdb065e0490918ba271d7339c42453d209d4cb619dfe635870d906731eff3e1ade8028bb461ea27ce8264ec5e22c6980612d332895977e89c1bbc80fcee2
   languageName: node
   linkType: hard
 
-"define-properties@npm:^1.1.3, define-properties@npm:^1.1.4":
+"define-properties@npm:^1.1.3, define-properties@npm:^1.1.4, define-properties@npm:^1.2.0":
   version: 1.2.0
   resolution: "define-properties@npm:1.2.0"
   dependencies:
     has-property-descriptors: ^1.0.0
     object-keys: ^1.1.1
   checksum: e60aee6a19b102df4e2b1f301816804e81ab48bb91f00d0d935f269bf4b3f79c88b39e4f89eaa132890d23267335fd1140dfcd8d5ccd61031a0a2c41a54e33a6
   languageName: node
@@ -6157,21 +6238,21 @@
   resolution: "end-of-stream@npm:1.4.4"
   dependencies:
     once: ^1.4.0
   checksum: 530a5a5a1e517e962854a31693dbb5c0b2fc40b46dad2a56a2deec656ca040631124f4795823acc68238147805f8b021abbe221f4afed5ef3c8e8efc2024908b
   languageName: node
   linkType: hard
 
-"enhanced-resolve@npm:^5.10.0":
-  version: 5.12.0
-  resolution: "enhanced-resolve@npm:5.12.0"
+"enhanced-resolve@npm:^5.14.0":
+  version: 5.14.0
+  resolution: "enhanced-resolve@npm:5.14.0"
   dependencies:
     graceful-fs: ^4.2.4
     tapable: ^2.2.0
-  checksum: bf3f787facaf4ce3439bef59d148646344e372bef5557f0d37ea8aa02c51f50a925cd1f07b8d338f18992c29f544ec235a8c64bcdb56030196c48832a5494174
+  checksum: fff1aaebbf376371e5df4502e111967f6247c37611ad3550e4e7fca657f6dcb29ef7ffe88bf14e5010b78997f1ddd984a8db97af87ee0a5477771398fd326f5b
   languageName: node
   linkType: hard
 
 "enquirer@npm:~2.3.6":
   version: 2.3.6
   resolution: "enquirer@npm:2.3.6"
   dependencies:
@@ -6275,18 +6356,18 @@
     typed-array-length: ^1.0.4
     unbox-primitive: ^1.0.2
     which-typed-array: ^1.1.9
   checksum: 037f55ee5e1cdf2e5edbab5524095a4f97144d95b94ea29e3611b77d852fd8c8a40e7ae7101fa6a759a9b9b1405f188c3c70928f2d3cd88d543a07fc0d5ad41a
   languageName: node
   linkType: hard
 
-"es-module-lexer@npm:^0.9.0":
-  version: 0.9.3
-  resolution: "es-module-lexer@npm:0.9.3"
-  checksum: 84bbab23c396281db2c906c766af58b1ae2a1a2599844a504df10b9e8dc77ec800b3211fdaa133ff700f5703d791198807bba25d9667392d27a5e9feda344da8
+"es-module-lexer@npm:^1.2.1":
+  version: 1.2.1
+  resolution: "es-module-lexer@npm:1.2.1"
+  checksum: c4145b853e1491eaa5d591e4580926d242978c38071ad3d09165c3b6d50314cc0ae3bf6e1dec81a9e53768b9299df2063d2e4a67d7742a5029ddeae6c4fc26f0
   languageName: node
   linkType: hard
 
 "es-set-tostringtag@npm:^2.0.1":
   version: 2.0.1
   resolution: "es-set-tostringtag@npm:2.0.1"
   dependencies:
@@ -6586,15 +6667,15 @@
 "events@npm:^3.2.0, events@npm:^3.3.0":
   version: 3.3.0
   resolution: "events@npm:3.3.0"
   checksum: f6f487ad2198aa41d878fa31452f1a3c00958f46e9019286ff4787c84aac329332ab45c9cdc8c445928fc6d7ded294b9e005a7fce9426488518017831b272780
   languageName: node
   linkType: hard
 
-"execa@npm:5.0.0":
+"execa@npm:5.0.0, execa@npm:^5.0.0":
   version: 5.0.0
   resolution: "execa@npm:5.0.0"
   dependencies:
     cross-spawn: ^7.0.3
     get-stream: ^6.0.0
     human-signals: ^2.1.0
     is-stream: ^2.0.0
@@ -6603,31 +6684,14 @@
     onetime: ^5.1.2
     signal-exit: ^3.0.3
     strip-final-newline: ^2.0.0
   checksum: a044367ebdcc68ca019810cb134510fc77bbc55c799122258ee0e00e289c132941ab48c2a331a036699c42bc8d479d451ae67c105fce5ce5cc813e7dd92d642b
   languageName: node
   linkType: hard
 
-"execa@npm:^5.0.0":
-  version: 5.1.1
-  resolution: "execa@npm:5.1.1"
-  dependencies:
-    cross-spawn: ^7.0.3
-    get-stream: ^6.0.0
-    human-signals: ^2.1.0
-    is-stream: ^2.0.0
-    merge-stream: ^2.0.0
-    npm-run-path: ^4.0.1
-    onetime: ^5.1.2
-    signal-exit: ^3.0.3
-    strip-final-newline: ^2.0.0
-  checksum: fba9022c8c8c15ed862847e94c252b3d946036d7547af310e344a527e59021fd8b6bb0723883ea87044dc4f0201f949046993124a42ccb0855cae5bf8c786343
-  languageName: node
-  linkType: hard
-
 "exit@npm:^0.1.2":
   version: 0.1.2
   resolution: "exit@npm:0.1.2"
   checksum: abc407f07a875c3961e4781dfcb743b58d6c93de9ab263f4f8c9d23bb6da5f9b7764fc773f86b43dd88030444d5ab8abcb611cb680fba8ca075362b77114bba3
   languageName: node
   linkType: hard
 
@@ -6976,15 +7040,15 @@
     define-properties: ^1.1.3
     es-abstract: ^1.19.0
     functions-have-names: ^1.2.2
   checksum: acd21d733a9b649c2c442f067567743214af5fa248dbeee69d8278ce7df3329ea5abac572be9f7470b4ec1cd4d8f1040e3c5caccf98ebf2bf861a0deab735c27
   languageName: node
   linkType: hard
 
-"functions-have-names@npm:^1.2.2":
+"functions-have-names@npm:^1.2.2, functions-have-names@npm:^1.2.3":
   version: 1.2.3
   resolution: "functions-have-names@npm:1.2.3"
   checksum: c3f1f5ba20f4e962efb71344ce0a40722163e85bee2101ce25f88214e78182d2d2476aa85ef37950c579eb6cf6ee811c17b3101bb84004bb75655f3e33f3fdb5
   languageName: node
   linkType: hard
 
 "gauge@npm:^4.0.3":
@@ -7068,28 +7132,21 @@
 "get-port@npm:5.1.1":
   version: 5.1.1
   resolution: "get-port@npm:5.1.1"
   checksum: 0162663ffe5c09e748cd79d97b74cd70e5a5c84b760a475ce5767b357fb2a57cb821cee412d646aa8a156ed39b78aab88974eddaa9e5ee926173c036c0713787
   languageName: node
   linkType: hard
 
-"get-stream@npm:6.0.0":
+"get-stream@npm:6.0.0, get-stream@npm:^6.0.0":
   version: 6.0.0
   resolution: "get-stream@npm:6.0.0"
   checksum: 587e6a93127f9991b494a566f4971cf7a2645dfa78034818143480a80587027bdd8826cdcf80d0eff4a4a19de0d231d157280f24789fc9cc31492e1dcc1290cf
   languageName: node
   linkType: hard
 
-"get-stream@npm:^6.0.0":
-  version: 6.0.1
-  resolution: "get-stream@npm:6.0.1"
-  checksum: e04ecece32c92eebf5b8c940f51468cd53554dcbb0ea725b2748be583c9523d00128137966afce410b9b051eb2ef16d657cd2b120ca8edafcf5a65e81af63cad
-  languageName: node
-  linkType: hard
-
 "get-symbol-description@npm:^1.0.0":
   version: 1.0.0
   resolution: "get-symbol-description@npm:1.0.0"
   dependencies:
     call-bind: ^1.0.2
     get-intrinsic: ^1.1.1
   checksum: 9ceff8fe968f9270a37a1f73bf3f1f7bda69ca80f4f80850670e0e7b9444ff99323f7ac52f96567f8b5f5fbe7ac717a0d81d3407c7313e82810c6199446a5247
@@ -7196,25 +7253,25 @@
     minimatch: ^3.0.4
     once: ^1.3.0
     path-is-absolute: ^1.0.0
   checksum: f52480fc82b1e66e52990f0f2e7306447d12294c83fbbee0395e761ad1178172012a7cc0673dbf4810baac400fc09bf34484c08b5778c216403fd823db281716
   languageName: node
   linkType: hard
 
-"glob@npm:^7.1.3, glob@npm:^7.1.4":
-  version: 7.2.3
-  resolution: "glob@npm:7.2.3"
+"glob@npm:^7.1.3, glob@npm:^7.1.4, glob@npm:~7.1.6":
+  version: 7.1.7
+  resolution: "glob@npm:7.1.7"
   dependencies:
     fs.realpath: ^1.0.0
     inflight: ^1.0.4
     inherits: 2
-    minimatch: ^3.1.1
+    minimatch: ^3.0.4
     once: ^1.3.0
     path-is-absolute: ^1.0.0
-  checksum: 29452e97b38fa704dabb1d1045350fb2467cf0277e155aa9ff7077e90ad81d1ea9d53d3ee63bd37c05b09a065e90f16aec4a65f5b8de401d1dac40bc5605d133
+  checksum: b61f48973bbdcf5159997b0874a2165db572b368b931135832599875919c237fc05c12984e38fe828e69aa8a921eb0e8a4997266211c517c9cfaae8a93988bb8
   languageName: node
   linkType: hard
 
 "glob@npm:^8.0.1":
   version: 8.1.0
   resolution: "glob@npm:8.1.0"
   dependencies:
@@ -7235,28 +7292,14 @@
     minimatch: ^7.4.1
     minipass: ^4.2.4
     path-scurry: ^1.6.1
   checksum: f3d188e9f70e24fa729a63ca197bcdb36d838677abec1fb9bbfe4b7620063bf90dc0f8d195203d632abfdfa049fad0edf22f93c60076de67cef20c23bcbfaee8
   languageName: node
   linkType: hard
 
-"glob@npm:~7.1.6":
-  version: 7.1.7
-  resolution: "glob@npm:7.1.7"
-  dependencies:
-    fs.realpath: ^1.0.0
-    inflight: ^1.0.4
-    inherits: 2
-    minimatch: ^3.0.4
-    once: ^1.3.0
-    path-is-absolute: ^1.0.0
-  checksum: b61f48973bbdcf5159997b0874a2165db572b368b931135832599875919c237fc05c12984e38fe828e69aa8a921eb0e8a4997266211c517c9cfaae8a93988bb8
-  languageName: node
-  linkType: hard
-
 "global-modules@npm:^2.0.0":
   version: 2.0.0
   resolution: "global-modules@npm:2.0.0"
   dependencies:
     global-prefix: ^3.0.0
   checksum: d6197f25856c878c2fb5f038899f2dca7cbb2f7b7cf8999660c0104972d5cfa5c68b5a0a77fa8206bb536c3903a4615665acb9709b4d80846e1bb47eaef65430
   languageName: node
@@ -7324,28 +7367,21 @@
   resolution: "gopd@npm:1.0.1"
   dependencies:
     get-intrinsic: ^1.1.3
   checksum: a5ccfb8806e0917a94e0b3de2af2ea4979c1da920bc381667c260e00e7cafdbe844e2cb9c5bcfef4e5412e8bf73bab837285bc35c7ba73aaaf0134d4583393a6
   languageName: node
   linkType: hard
 
-"graceful-fs@npm:4.2.10":
+"graceful-fs@npm:4.2.10, graceful-fs@npm:^4.1.11, graceful-fs@npm:^4.1.15, graceful-fs@npm:^4.1.2, graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.4, graceful-fs@npm:^4.2.6, graceful-fs@npm:^4.2.9":
   version: 4.2.10
   resolution: "graceful-fs@npm:4.2.10"
   checksum: 3f109d70ae123951905d85032ebeae3c2a5a7a997430df00ea30df0e3a6c60cf6689b109654d6fdacd28810a053348c4d14642da1d075049e6be1ba5216218da
   languageName: node
   linkType: hard
 
-"graceful-fs@npm:^4.1.11, graceful-fs@npm:^4.1.15, graceful-fs@npm:^4.1.2, graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.4, graceful-fs@npm:^4.2.6, graceful-fs@npm:^4.2.9":
-  version: 4.2.11
-  resolution: "graceful-fs@npm:4.2.11"
-  checksum: ac85f94da92d8eb6b7f5a8b20ce65e43d66761c55ce85ac96df6865308390da45a8d3f0296dd3a663de65d30ba497bd46c696cc1e248c72b13d6d567138a4fc7
-  languageName: node
-  linkType: hard
-
 "grapheme-splitter@npm:^1.0.4":
   version: 1.0.4
   resolution: "grapheme-splitter@npm:1.0.4"
   checksum: 0c22ec54dee1b05cd480f78cf14f732cb5b108edc073572c4ec205df4cd63f30f8db8025afc5debc8835a8ddeacf648a1c7992fe3dcd6ad38f9a476d84906620
   languageName: node
   linkType: hard
 
@@ -7732,15 +7768,15 @@
     semver: ^7.3.5
     validate-npm-package-license: ^3.0.4
     validate-npm-package-name: ^4.0.0
   checksum: e027f60e4a1564809eee790d5a842341c784888fd7c7ace5f9a34ea76224c0adb6f3ab3bf205cf1c9c877a6e1a76c68b00847a984139f60813125d7b42a23a13
   languageName: node
   linkType: hard
 
-"inquirer@npm:8.2.4":
+"inquirer@npm:8.2.4, inquirer@npm:^8.2.4":
   version: 8.2.4
   resolution: "inquirer@npm:8.2.4"
   dependencies:
     ansi-escapes: ^4.2.1
     chalk: ^4.1.1
     cli-cursor: ^3.1.0
     cli-width: ^3.0.0
@@ -7755,37 +7791,14 @@
     strip-ansi: ^6.0.0
     through: ^2.3.6
     wrap-ansi: ^7.0.0
   checksum: dfcb6529d3af443dfea2241cb471508091b51f5121a088fdb8728b23ec9b349ef0a5e13a0ef2c8e19457b0bed22f7cbbcd561f7a4529d084c562a58c605e2655
   languageName: node
   linkType: hard
 
-"inquirer@npm:^8.2.4":
-  version: 8.2.5
-  resolution: "inquirer@npm:8.2.5"
-  dependencies:
-    ansi-escapes: ^4.2.1
-    chalk: ^4.1.1
-    cli-cursor: ^3.1.0
-    cli-width: ^3.0.0
-    external-editor: ^3.0.3
-    figures: ^3.0.0
-    lodash: ^4.17.21
-    mute-stream: 0.0.8
-    ora: ^5.4.1
-    run-async: ^2.4.0
-    rxjs: ^7.5.5
-    string-width: ^4.1.0
-    strip-ansi: ^6.0.0
-    through: ^2.3.6
-    wrap-ansi: ^7.0.0
-  checksum: f13ee4c444187786fb393609dedf6b30870115a57b603f2e6424f29a99abc13446fd45ee22461c33c9c40a92a60a8df62d0d6b25d74fc6676fa4cb211de55b55
-  languageName: node
-  linkType: hard
-
 "internal-slot@npm:^1.0.3, internal-slot@npm:^1.0.5":
   version: 1.0.5
   resolution: "internal-slot@npm:1.0.5"
   dependencies:
     get-intrinsic: ^1.2.0
     has: ^1.0.3
     side-channel: ^1.0.4
@@ -7858,20 +7871,20 @@
     ci-info: ^2.0.0
   bin:
     is-ci: bin.js
   checksum: 77b869057510f3efa439bbb36e9be429d53b3f51abd4776eeea79ab3b221337fe1753d1e50058a9e2c650d38246108beffb15ccfd443929d77748d8c0cc90144
   languageName: node
   linkType: hard
 
-"is-core-module@npm:^2.5.0, is-core-module@npm:^2.8.1, is-core-module@npm:^2.9.0":
-  version: 2.11.0
-  resolution: "is-core-module@npm:2.11.0"
+"is-core-module@npm:^2.12.0, is-core-module@npm:^2.5.0, is-core-module@npm:^2.8.1, is-core-module@npm:^2.9.0":
+  version: 2.12.0
+  resolution: "is-core-module@npm:2.12.0"
   dependencies:
     has: ^1.0.3
-  checksum: f96fd490c6b48eb4f6d10ba815c6ef13f410b0ba6f7eb8577af51697de523e5f2cd9de1c441b51d27251bf0e4aebc936545e33a5d26d5d51f28d25698d4a8bab
+  checksum: f7f7eb2ab71fd769ee9fb2385c095d503aa4b5ce0028c04557de03f1e67a87c85e5bac1f215945fc3c955867a139a415a3ec4c4234a0bffdf715232660f440a6
   languageName: node
   linkType: hard
 
 "is-date-object@npm:^1.0.1":
   version: 1.0.5
   resolution: "is-date-object@npm:1.0.5"
   dependencies:
@@ -8031,28 +8044,21 @@
   resolution: "is-ssh@npm:1.4.0"
   dependencies:
     protocols: ^2.0.1
   checksum: 75eaa17b538bee24b661fbeb0f140226ac77e904a6039f787bea418431e2162f1f9c4c4ccad3bd169e036cd701cc631406e8c505d9fa7e20164e74b47f86f40f
   languageName: node
   linkType: hard
 
-"is-stream@npm:2.0.0":
+"is-stream@npm:2.0.0, is-stream@npm:^2.0.0":
   version: 2.0.0
   resolution: "is-stream@npm:2.0.0"
   checksum: 4dc47738e26bc4f1b3be9070b6b9e39631144f204fc6f87db56961220add87c10a999ba26cf81699f9ef9610426f69cb08a4713feff8deb7d8cadac907826935
   languageName: node
   linkType: hard
 
-"is-stream@npm:^2.0.0":
-  version: 2.0.1
-  resolution: "is-stream@npm:2.0.1"
-  checksum: b8e05ccdf96ac330ea83c12450304d4a591f9958c11fd17bed240af8d5ffe08aedafa4c0f4cfccd4d28dc9d4d129daca1023633d5c11601a6cbc77521f6fae66
-  languageName: node
-  linkType: hard
-
 "is-string@npm:^1.0.5, is-string@npm:^1.0.7":
   version: 1.0.7
   resolution: "is-string@npm:1.0.7"
   dependencies:
     has-tostringtag: ^1.0.0
   checksum: 323b3d04622f78d45077cf89aab783b2f49d24dc641aa89b5ad1a72114cfeff2585efc8c12ef42466dff32bde93d839ad321b26884cf75e5a7892a938b089989
   languageName: node
@@ -8671,15 +8677,15 @@
     jest-util: ^29.5.0
     merge-stream: ^2.0.0
     supports-color: ^8.0.0
   checksum: 1151a1ae3602b1ea7c42a8f1efe2b5a7bf927039deaa0827bf978880169899b705744e288f80a63603fb3fc2985e0071234986af7dc2c21c7a64333d8777c7c9
   languageName: node
   linkType: hard
 
-"jest@npm:^29.2.0":
+"jest@npm:^29.2.0, jest@npm:^29.5.0":
   version: 29.5.0
   resolution: "jest@npm:29.5.0"
   dependencies:
     "@jest/core": ^29.5.0
     "@jest/types": ^29.5.0
     import-local: ^3.0.2
     jest-cli: ^29.5.0
@@ -9164,23 +9170,23 @@
   dependencies:
     prelude-ls: ~1.1.2
     type-check: ~0.3.2
   checksum: 0d084a524231a8246bb10fec48cdbb35282099f6954838604f3c7fc66f2e16fa66fd9cc2f3f20a541a113c4dafdf181e822c887c8a319c9195444e6c64ac395e
   languageName: node
   linkType: hard
 
-"lib0@npm:^0.2.31, lib0@npm:^0.2.42, lib0@npm:^0.2.52, lib0@npm:^0.2.72":
-  version: 0.2.73
-  resolution: "lib0@npm:0.2.73"
+"lib0@npm:^0.2.31, lib0@npm:^0.2.42, lib0@npm:^0.2.52, lib0@npm:^0.2.74":
+  version: 0.2.74
+  resolution: "lib0@npm:0.2.74"
   dependencies:
     isomorphic.js: ^0.2.4
   bin:
     0gentesthtml: bin/gentesthtml.js
     0serve: bin/0serve.js
-  checksum: a9a73513ef6e91a47602ae650483eed7a8f803c512dbea3e08ef1162bd63b463230c6cdcac4ca40d01925b24218398aa3fc3c16692227384eaa326968a220815
+  checksum: a468fc2f8d231bdcb305f04706d0e568ad53a0aa968aaf3d1769fcfbf326a5b158e98d86c0aa8edf26b3223cb60687480f15cfc0d07c681333f9d9d55dd7c802
   languageName: node
   linkType: hard
 
 "libnpmaccess@npm:6.0.3":
   version: 6.0.3
   resolution: "libnpmaccess@npm:6.0.3"
   dependencies:
@@ -9298,15 +9304,15 @@
   resolution: "locate-path@npm:6.0.0"
   dependencies:
     p-locate: ^5.0.0
   checksum: 72eb661788a0368c099a184c59d2fee760b3831c9c1c33955e8a19ae4a21b4116e53fa736dc086cdeb9fce9f7cc508f2f92d2d3aae516f133e16a2bb59a39f5a
   languageName: node
   linkType: hard
 
-"lodash-es@npm:^4.17.15":
+"lodash-es@npm:^4.17.21":
   version: 4.17.21
   resolution: "lodash-es@npm:4.17.21"
   checksum: 05cbffad6e2adbb331a4e16fbd826e7faee403a1a04873b82b42c0f22090f280839f85b95393f487c1303c8a3d2a010048bf06151a6cbe03eee4d388fb0a12d2
   languageName: node
   linkType: hard
 
 "lodash.debounce@npm:^4.0.8":
@@ -9340,14 +9346,21 @@
 "lodash.merge@npm:^4.6.2":
   version: 4.6.2
   resolution: "lodash.merge@npm:4.6.2"
   checksum: ad580b4bdbb7ca1f7abf7e1bce63a9a0b98e370cf40194b03380a46b4ed799c9573029599caebc1b14e3f24b111aef72b96674a56cfa105e0f5ac70546cdc005
   languageName: node
   linkType: hard
 
+"lodash.mergewith@npm:^4.6.1":
+  version: 4.6.2
+  resolution: "lodash.mergewith@npm:4.6.2"
+  checksum: a6db2a9339752411f21b956908c404ec1e088e783a65c8b29e30ae5b3b6384f82517662d6f425cc97c2070b546cc2c7daaa8d33f78db7b6e9be06cd834abdeb8
+  languageName: node
+  linkType: hard
+
 "lodash.truncate@npm:^4.4.2":
   version: 4.4.2
   resolution: "lodash.truncate@npm:4.4.2"
   checksum: b463d8a382cfb5f0e71c504dcb6f807a7bd379ff1ea216669aa42c52fc28c54e404bfbd96791aa09e6df0de2c1d7b8f1b7f4b1a61f324d38fe98bc535aeee4f5
   languageName: node
   linkType: hard
 
@@ -9671,15 +9684,15 @@
   resolution: "minimatch@npm:3.0.5"
   dependencies:
     brace-expansion: ^1.1.7
   checksum: a3b84b426eafca947741b864502cee02860c4e7b145de11ad98775cfcf3066fef422583bc0ffce0952ddf4750c1ccf4220b1556430d4ce10139f66247d87d69e
   languageName: node
   linkType: hard
 
-"minimatch@npm:^3.0.4, minimatch@npm:^3.0.5, minimatch@npm:^3.1.1, minimatch@npm:^3.1.2":
+"minimatch@npm:^3.0.4, minimatch@npm:^3.0.5, minimatch@npm:^3.1.2":
   version: 3.1.2
   resolution: "minimatch@npm:3.1.2"
   dependencies:
     brace-expansion: ^1.1.7
   checksum: c154e566406683e7bcb746e000b84d74465b3a832c45d59912b9b55cd50dee66e5c4b1e5566dba26154040e51672f9aa450a9aef0c97cfc7336b78b7afb9540a
   languageName: node
   linkType: hard
@@ -9854,28 +9867,21 @@
 "modify-values@npm:^1.0.0":
   version: 1.0.1
   resolution: "modify-values@npm:1.0.1"
   checksum: 8296610c608bc97b03c2cf889c6cdf4517e32fa2d836440096374c2209f6b7b3e256c209493a0b32584b9cb32d528e99d0dd19dcd9a14d2d915a312d391cc7e9
   languageName: node
   linkType: hard
 
-"ms@npm:2.1.2":
+"ms@npm:2.1.2, ms@npm:^2.0.0":
   version: 2.1.2
   resolution: "ms@npm:2.1.2"
   checksum: 673cdb2c3133eb050c745908d8ce632ed2c02d85640e2edb3ace856a2266a813b30c613569bf3354fdf4ea7d1a1494add3bfa95e2713baa27d0c2c71fc44f58f
   languageName: node
   linkType: hard
 
-"ms@npm:^2.0.0":
-  version: 2.1.3
-  resolution: "ms@npm:2.1.3"
-  checksum: aa92de608021b242401676e35cfa5aa42dd70cbdc082b916da7fb925c542173e36bce97ea3e804923fe92c0ad991434e4a38327e15a1b5b5f945d66df615ae6d
-  languageName: node
-  linkType: hard
-
 "multimatch@npm:5.0.0":
   version: 5.0.0
   resolution: "multimatch@npm:5.0.0"
   dependencies:
     "@types/minimatch": ^3.0.3
     array-differ: ^3.0.0
     array-union: ^2.1.0
@@ -9888,15 +9894,15 @@
 "mute-stream@npm:0.0.8, mute-stream@npm:~0.0.4":
   version: 0.0.8
   resolution: "mute-stream@npm:0.0.8"
   checksum: ff48d251fc3f827e5b1206cda0ffdaec885e56057ee86a3155e1951bc940fd5f33531774b1cc8414d7668c10a8907f863f6561875ee6e8768931a62121a531a1
   languageName: node
   linkType: hard
 
-"nanoid@npm:^3.3.4":
+"nanoid@npm:^3.3.6":
   version: 3.3.6
   resolution: "nanoid@npm:3.3.6"
   bin:
     nanoid: bin/nanoid.cjs
   checksum: 7d0eda657002738aa5206107bd0580aead6c95c460ef1bdd0b1a87a9c7ae6277ac2e9b945306aaa5b32c6dcb7feaf462d0f552e7f8b5718abfc6ead5c94a71b3
   languageName: node
   linkType: hard
@@ -9948,42 +9954,28 @@
   resolution: "node-addon-api@npm:3.2.1"
   dependencies:
     node-gyp: latest
   checksum: 2369986bb0881ccd9ef6bacdf39550e07e089a9c8ede1cbc5fc7712d8e2faa4d50da0e487e333d4125f8c7a616c730131d1091676c9d499af1d74560756b4a18
   languageName: node
   linkType: hard
 
-"node-fetch@npm:2.6.7":
+"node-fetch@npm:2.6.7, node-fetch@npm:^2.6.0, node-fetch@npm:^2.6.7":
   version: 2.6.7
   resolution: "node-fetch@npm:2.6.7"
   dependencies:
     whatwg-url: ^5.0.0
   peerDependencies:
     encoding: ^0.1.0
   peerDependenciesMeta:
     encoding:
       optional: true
   checksum: 8d816ffd1ee22cab8301c7756ef04f3437f18dace86a1dae22cf81db8ef29c0bf6655f3215cb0cdb22b420b6fe141e64b26905e7f33f9377a7fa59135ea3e10b
   languageName: node
   linkType: hard
 
-"node-fetch@npm:^2.6.0, node-fetch@npm:^2.6.7":
-  version: 2.6.9
-  resolution: "node-fetch@npm:2.6.9"
-  dependencies:
-    whatwg-url: ^5.0.0
-  peerDependencies:
-    encoding: ^0.1.0
-  peerDependenciesMeta:
-    encoding:
-      optional: true
-  checksum: acb04f9ce7224965b2b59e71b33c639794d8991efd73855b0b250921382b38331ffc9d61bce502571f6cc6e11a8905ca9b1b6d4aeb586ab093e2756a1fd190d0
-  languageName: node
-  linkType: hard
-
 "node-gyp-build@npm:^4.3.0":
   version: 4.6.0
   resolution: "node-gyp-build@npm:4.6.0"
   bin:
     node-gyp-build: bin.js
     node-gyp-build-optional: optional.js
     node-gyp-build-test: build-test.js
@@ -10118,23 +10110,14 @@
   resolution: "npm-bundled@npm:1.1.2"
   dependencies:
     npm-normalize-package-bin: ^1.0.1
   checksum: 6e599155ef28d0b498622f47f1ba189dfbae05095a1ed17cb3a5babf961e965dd5eab621f0ec6f0a98de774e5836b8f5a5ee639010d64f42850a74acec3d4d09
   languageName: node
   linkType: hard
 
-"npm-bundled@npm:^2.0.0":
-  version: 2.0.1
-  resolution: "npm-bundled@npm:2.0.1"
-  dependencies:
-    npm-normalize-package-bin: ^2.0.0
-  checksum: 7747293985c48c5268871efe691545b03731cb80029692000cbdb0b3344b9617be5187aa36281cabbe6b938e3651b4e87236d1c31f9e645eef391a1a779413e6
-  languageName: node
-  linkType: hard
-
 "npm-bundled@npm:^3.0.0":
   version: 3.0.0
   resolution: "npm-bundled@npm:3.0.0"
   dependencies:
     npm-normalize-package-bin: ^3.0.0
   checksum: 110859c2d6dcd7941dac0932a29171cbde123060486a4b6e897aaf5e025abeb3d9ffcdfe9e9271992e6396b2986c2c534f1029a45a7c196f1257fa244305dbf8
   languageName: node
@@ -10210,42 +10193,28 @@
     proc-log: ^2.0.1
     semver: ^7.3.5
     validate-npm-package-name: ^4.0.0
   checksum: 3793488843985ed71deb14fcba7c068d8ed03a18fd8f6b235c6a64465c9a25f60261598106d5cc8677c0bee9548e405c34c2e3c7a822e3113d3389351c745dfa
   languageName: node
   linkType: hard
 
-"npm-packlist@npm:5.1.1":
+"npm-packlist@npm:5.1.1, npm-packlist@npm:^5.1.0":
   version: 5.1.1
   resolution: "npm-packlist@npm:5.1.1"
   dependencies:
     glob: ^8.0.1
     ignore-walk: ^5.0.1
     npm-bundled: ^1.1.2
     npm-normalize-package-bin: ^1.0.1
   bin:
     npm-packlist: bin/index.js
   checksum: 28dab153744ceb4695b82a9032d14aa2bfb855d38344a09052673d07860a4d8725f808ed23996e6f2792c48e11f5d147632c159f798d2c24dac92b51a884f0c6
   languageName: node
   linkType: hard
 
-"npm-packlist@npm:^5.1.0":
-  version: 5.1.3
-  resolution: "npm-packlist@npm:5.1.3"
-  dependencies:
-    glob: ^8.0.1
-    ignore-walk: ^5.0.1
-    npm-bundled: ^2.0.0
-    npm-normalize-package-bin: ^2.0.0
-  bin:
-    npm-packlist: bin/index.js
-  checksum: 94cc9c66740e8f80243301de85eb0a2cec5bbd570c3f26b6ad7af1a3eca155f7e810580dc7ea4448f12a8fd82f6db307e7132a5fe69e157eb45b325acadeb22a
-  languageName: node
-  linkType: hard
-
 "npm-packlist@npm:^7.0.0":
   version: 7.0.4
   resolution: "npm-packlist@npm:7.0.4"
   dependencies:
     ignore-walk: ^6.0.0
   checksum: 5ffa1f8f0b32141a60a66713fa3ed03b8ee4800b1ed6b59194d03c3c85da88f3fc21e1de29b665f322678bae85198732b16aa76c0a7cb0e283f9e0db50752233
   languageName: node
@@ -11095,21 +11064,21 @@
   version: 4.2.0
   resolution: "postcss-value-parser@npm:4.2.0"
   checksum: 819ffab0c9d51cf0acbabf8996dffbfafbafa57afc0e4c98db88b67f2094cb44488758f06e5da95d7036f19556a4a732525e84289a425f4f6fd8e412a9d7442f
   languageName: node
   linkType: hard
 
 "postcss@npm:^8.3.11, postcss@npm:^8.4.19, postcss@npm:^8.4.21":
-  version: 8.4.21
-  resolution: "postcss@npm:8.4.21"
+  version: 8.4.23
+  resolution: "postcss@npm:8.4.23"
   dependencies:
-    nanoid: ^3.3.4
+    nanoid: ^3.3.6
     picocolors: ^1.0.0
     source-map-js: ^1.0.2
-  checksum: e39ac60ccd1542d4f9d93d894048aac0d686b3bb38e927d8386005718e6793dbbb46930f0a523fe382f1bbd843c6d980aaea791252bf5e176180e5a4336d9679
+  checksum: 8bb9d1b2ea6e694f8987d4f18c94617971b2b8d141602725fedcc2222fdc413b776a6e1b969a25d627d7b2681ca5aabb56f59e727ef94072e1b6ac8412105a2f
   languageName: node
   linkType: hard
 
 "prelude-ls@npm:^1.2.1":
   version: 1.2.1
   resolution: "prelude-ls@npm:1.2.1"
   checksum: cd192ec0d0a8e4c6da3bb80e4f62afe336df3f76271ac6deb0e6a36187133b6073a19e9727a1ff108cd8b9982e4768850d413baa71214dd80c7979617dca827a
@@ -11237,15 +11206,15 @@
   resolution: "promzard@npm:0.3.0"
   dependencies:
     read: 1
   checksum: 443a3b39ac916099988ee0161ab4e22edd1fa27e3d39a38d60e48c11ca6df3f5a90bfe44d95af06ed8659c4050b789ffe64c3f9f8e49a4bea1ea19105c98445a
   languageName: node
   linkType: hard
 
-"prop-types@npm:^15.7.2, prop-types@npm:^15.8.1":
+"prop-types@npm:^15.8.1":
   version: 15.8.1
   resolution: "prop-types@npm:15.8.1"
   dependencies:
     loose-envify: ^1.4.0
     object-assign: ^4.1.1
     react-is: ^16.13.1
   checksum: c056d3f1c057cb7ff8344c645450e14f088a915d078dcda795041765047fa080d38e5d626560ccaac94a4e16e3aa15f3557c1a9a8d1174530955e992c675e459
@@ -11403,38 +11372,26 @@
   dependencies:
     json-parse-even-better-errors: ^3.0.0
     npm-normalize-package-bin: ^3.0.0
   checksum: 8d406869f045f1d76e2a99865a8fd1c1af9c1dc06200b94d2b07eef87ed734b22703a8d72e1cd36ea36cc48e22020bdd187f88243c7dd0563f72114d38c17072
   languageName: node
   linkType: hard
 
-"read-package-json@npm:5.0.1":
+"read-package-json@npm:5.0.1, read-package-json@npm:^5.0.0":
   version: 5.0.1
   resolution: "read-package-json@npm:5.0.1"
   dependencies:
     glob: ^8.0.1
     json-parse-even-better-errors: ^2.3.1
     normalize-package-data: ^4.0.0
     npm-normalize-package-bin: ^1.0.1
   checksum: e8c2ad72df1f17e71268feabdb9bb0153ed2c7d38a05b759c5c49cf368a754bdd3c0e8a279fbc8d707802ff91d2cf144a995e6ebd5534de2848d52ab2c14034d
   languageName: node
   linkType: hard
 
-"read-package-json@npm:^5.0.0":
-  version: 5.0.2
-  resolution: "read-package-json@npm:5.0.2"
-  dependencies:
-    glob: ^8.0.1
-    json-parse-even-better-errors: ^2.3.1
-    normalize-package-data: ^4.0.0
-    npm-normalize-package-bin: ^2.0.0
-  checksum: 0882ac9cec1bc92fb5515e9727611fb2909351e1e5c840dce3503cbb25b4cd48eb44b61071986e0fc51043208161f07d364a7336206c8609770186818753b51a
-  languageName: node
-  linkType: hard
-
 "read-package-json@npm:^6.0.0":
   version: 6.0.1
   resolution: "read-package-json@npm:6.0.1"
   dependencies:
     glob: ^9.3.0
     json-parse-even-better-errors: ^3.0.0
     normalize-package-data: ^5.0.0
@@ -11581,22 +11538,40 @@
   resolution: "regenerator-transform@npm:0.15.1"
   dependencies:
     "@babel/runtime": ^7.8.4
   checksum: 2d15bdeadbbfb1d12c93f5775493d85874dbe1d405bec323da5c61ec6e701bc9eea36167483e1a5e752de9b2df59ab9a2dfff6bf3784f2b28af2279a673d29a4
   languageName: node
   linkType: hard
 
+"regexp-match-indices@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "regexp-match-indices@npm:1.0.2"
+  dependencies:
+    regexp-tree: ^0.1.11
+  checksum: 8cc779f6cf8f404ead828d09970a7d4bd66bd78d43ab9eb2b5e65f2ef2ba1ed53536f5b5fa839fb90b350365fb44b6a851c7f16289afc3f37789c113ab2a7916
+  languageName: node
+  linkType: hard
+
+"regexp-tree@npm:^0.1.11":
+  version: 0.1.27
+  resolution: "regexp-tree@npm:0.1.27"
+  bin:
+    regexp-tree: bin/regexp-tree
+  checksum: 129aebb34dae22d6694ab2ac328be3f99105143737528ab072ef624d599afecbcfae1f5c96a166fa9e5f64fa1ecf30b411c4691e7924c3e11bbaf1712c260c54
+  languageName: node
+  linkType: hard
+
 "regexp.prototype.flags@npm:^1.4.3":
-  version: 1.4.3
-  resolution: "regexp.prototype.flags@npm:1.4.3"
+  version: 1.5.0
+  resolution: "regexp.prototype.flags@npm:1.5.0"
   dependencies:
     call-bind: ^1.0.2
-    define-properties: ^1.1.3
-    functions-have-names: ^1.2.2
-  checksum: 51228bae732592adb3ededd5e15426be25f289e9c4ef15212f4da73f4ec3919b6140806374b8894036a86020d054a8d2657d3fee6bb9b4d35d8939c20030b7a6
+    define-properties: ^1.2.0
+    functions-have-names: ^1.2.3
+  checksum: c541687cdbdfff1b9a07f6e44879f82c66bbf07665f9a7544c5fd16acdb3ec8d1436caab01662d2fbcad403f3499d49ab0b77fbc7ef29ef961d98cc4bc9755b4
   languageName: node
   linkType: hard
 
 "regexpu-core@npm:^5.3.1":
   version: 5.3.2
   resolution: "regexpu-core@npm:5.3.2"
   dependencies:
@@ -11669,23 +11644,23 @@
   version: 2.0.2
   resolution: "resolve.exports@npm:2.0.2"
   checksum: 1c7778ca1b86a94f8ab4055d196c7d87d1874b96df4d7c3e67bbf793140f0717fd506dcafd62785b079cd6086b9264424ad634fb904409764c3509c3df1653f2
   languageName: node
   linkType: hard
 
 "resolve@npm:^1.10.0, resolve@npm:^1.14.2, resolve@npm:^1.20.0":
-  version: 1.22.1
-  resolution: "resolve@npm:1.22.1"
+  version: 1.22.3
+  resolution: "resolve@npm:1.22.3"
   dependencies:
-    is-core-module: ^2.9.0
+    is-core-module: ^2.12.0
     path-parse: ^1.0.7
     supports-preserve-symlinks-flag: ^1.0.0
   bin:
     resolve: bin/resolve
-  checksum: 07af5fc1e81aa1d866cbc9e9460fbb67318a10fa3c4deadc35c3ad8a898ee9a71a86a65e4755ac3195e0ea0cfbe201eb323ebe655ce90526fd61917313a34e4e
+  checksum: fb834b81348428cb545ff1b828a72ea28feb5a97c026a1cf40aa1008352c72811ff4d4e71f2035273dc536dcfcae20c13604ba6283c612d70fa0b6e44519c374
   languageName: node
   linkType: hard
 
 "resolve@npm:^2.0.0-next.4":
   version: 2.0.0-next.4
   resolution: "resolve@npm:2.0.0-next.4"
   dependencies:
@@ -11695,23 +11670,23 @@
   bin:
     resolve: bin/resolve
   checksum: c438ac9a650f2030fd074219d7f12ceb983b475da2d89ad3d6dd05fbf6b7a0a8cd37d4d10b43cb1f632bc19f22246ab7f36ebda54d84a29bfb2910a0680906d3
   languageName: node
   linkType: hard
 
 "resolve@patch:resolve@^1.10.0#~builtin<compat/resolve>, resolve@patch:resolve@^1.14.2#~builtin<compat/resolve>, resolve@patch:resolve@^1.20.0#~builtin<compat/resolve>":
-  version: 1.22.1
-  resolution: "resolve@patch:resolve@npm%3A1.22.1#~builtin<compat/resolve>::version=1.22.1&hash=c3c19d"
+  version: 1.22.3
+  resolution: "resolve@patch:resolve@npm%3A1.22.3#~builtin<compat/resolve>::version=1.22.3&hash=c3c19d"
   dependencies:
-    is-core-module: ^2.9.0
+    is-core-module: ^2.12.0
     path-parse: ^1.0.7
     supports-preserve-symlinks-flag: ^1.0.0
   bin:
     resolve: bin/resolve
-  checksum: 5656f4d0bedcf8eb52685c1abdf8fbe73a1603bb1160a24d716e27a57f6cecbe2432ff9c89c2bd57542c3a7b9d14b1882b73bfe2e9d7849c9a4c0b8b39f02b8b
+  checksum: ad59734723b596d0891321c951592ed9015a77ce84907f89c9d9307dd0c06e11a67906a3e628c4cae143d3e44898603478af0ddeb2bba3f229a9373efe342665
   languageName: node
   linkType: hard
 
 "resolve@patch:resolve@^2.0.0-next.4#~builtin<compat/resolve>":
   version: 2.0.0-next.4
   resolution: "resolve@patch:resolve@npm%3A2.0.0-next.4#~builtin<compat/resolve>::version=2.0.0-next.4&hash=c3c19d"
   dependencies:
@@ -11791,22 +11766,15 @@
   resolution: "rxjs@npm:7.8.0"
   dependencies:
     tslib: ^2.1.0
   checksum: 61b4d4fd323c1043d8d6ceb91f24183b28bcf5def4f01ca111511d5c6b66755bc5578587fe714ef5d67cf4c9f2e26f4490d4e1d8cabf9bd5967687835e9866a2
   languageName: node
   linkType: hard
 
-"safe-buffer@npm:^5.1.0, safe-buffer@npm:~5.2.0":
-  version: 5.2.1
-  resolution: "safe-buffer@npm:5.2.1"
-  checksum: b99c4b41fdd67a6aaf280fcd05e9ffb0813654894223afb78a31f14a19ad220bba8aba1cb14eddce1fcfb037155fe6de4e861784eb434f7d11ed58d1e70dd491
-  languageName: node
-  linkType: hard
-
-"safe-buffer@npm:~5.1.0, safe-buffer@npm:~5.1.1":
+"safe-buffer@npm:^5.1.0, safe-buffer@npm:~5.1.0, safe-buffer@npm:~5.1.1":
   version: 5.1.2
   resolution: "safe-buffer@npm:5.1.2"
   checksum: f2f1f7943ca44a594893a852894055cf619c1fbcb611237fc39e461ae751187e7baf4dc391a72125e0ac4fb2d8c5c0b3c71529622e6a58f46b960211e704903c
   languageName: node
   linkType: hard
 
 "safe-regex-test@npm:^1.0.0":
@@ -11866,34 +11834,34 @@
     "@types/json-schema": ^7.0.5
     ajv: ^6.12.4
     ajv-keywords: ^3.5.2
   checksum: 32c62fc9e28edd101e1bd83453a4216eb9bd875cc4d3775e4452b541908fa8f61a7bbac8ffde57484f01d7096279d3ba0337078e85a918ecbeb72872fb09fb2b
   languageName: node
   linkType: hard
 
-"schema-utils@npm:^3.0.0, schema-utils@npm:^3.1.0, schema-utils@npm:^3.1.1":
-  version: 3.1.1
-  resolution: "schema-utils@npm:3.1.1"
+"schema-utils@npm:^3.0.0, schema-utils@npm:^3.1.1, schema-utils@npm:^3.1.2":
+  version: 3.1.2
+  resolution: "schema-utils@npm:3.1.2"
   dependencies:
     "@types/json-schema": ^7.0.8
     ajv: ^6.12.5
     ajv-keywords: ^3.5.2
-  checksum: fb73f3d759d43ba033c877628fe9751620a26879f6301d3dbeeb48cf2a65baec5cdf99da65d1bf3b4ff5444b2e59cbe4f81c2456b5e0d2ba7d7fd4aed5da29ce
+  checksum: 39683edfe3beff018cdb1ae4fa296fc55cea13a080aa2b4d9351895cd64b22ba4d87e2e548c2a2ac1bc76e60980670adb0f413a58104479f1a0c12e5663cb8ca
   languageName: node
   linkType: hard
 
 "schema-utils@npm:^4.0.0":
-  version: 4.0.0
-  resolution: "schema-utils@npm:4.0.0"
+  version: 4.0.1
+  resolution: "schema-utils@npm:4.0.1"
   dependencies:
     "@types/json-schema": ^7.0.9
-    ajv: ^8.8.0
+    ajv: ^8.9.0
     ajv-formats: ^2.1.1
-    ajv-keywords: ^5.0.0
-  checksum: c843e92fdd1a5c145dbb6ffdae33e501867f9703afac67bdf35a685e49f85b1dcc10ea250033175a64bd9d31f0555bc6785b8359da0c90bcea30cf6dfbb55a8f
+    ajv-keywords: ^5.1.0
+  checksum: 745e7293c6b6c84940de16753c207311da821aa9911b9e2d158cfd9ffc5bf1f880147abbbe775b96cb8cd3c7f48890950fe0164f54eed9a8aabb948ebf8a3fdd
   languageName: node
   linkType: hard
 
 "semver@npm:2 || 3 || 4 || 5, semver@npm:^5.4.1, semver@npm:^5.5.0, semver@npm:^5.6.0":
   version: 5.7.1
   resolution: "semver@npm:5.7.1"
   bin:
@@ -12330,24 +12298,15 @@
     call-bind: ^1.0.2
     define-properties: ^1.1.4
     es-abstract: ^1.20.4
   checksum: 89080feef416621e6ef1279588994305477a7a91648d9436490d56010a1f7adc39167cddac7ce0b9884b8cdbef086987c4dcb2960209f2af8bac0d23ceff4f41
   languageName: node
   linkType: hard
 
-"string_decoder@npm:^1.1.1":
-  version: 1.3.0
-  resolution: "string_decoder@npm:1.3.0"
-  dependencies:
-    safe-buffer: ~5.2.0
-  checksum: 8417646695a66e73aefc4420eb3b84cc9ffd89572861fe004e6aeb13c7bc00e2f616247505d2dbbef24247c372f70268f594af7126f43548565c68c117bdeb56
-  languageName: node
-  linkType: hard
-
-"string_decoder@npm:~1.1.1":
+"string_decoder@npm:^1.1.1, string_decoder@npm:~1.1.1":
   version: 1.1.1
   resolution: "string_decoder@npm:1.1.1"
   dependencies:
     safe-buffer: ~5.1.0
   checksum: 9ab7e56f9d60a28f2be697419917c50cac19f3e8e6c28ef26ed5f4852289fe0de5d6997d29becf59028556f2c62983790c1d9ba1e2a3cc401768ca12d5183a5b
   languageName: node
   linkType: hard
@@ -12605,42 +12564,28 @@
     fs-constants: ^1.0.0
     inherits: ^2.0.3
     readable-stream: ^3.1.1
   checksum: 699831a8b97666ef50021c767f84924cfee21c142c2eb0e79c63254e140e6408d6d55a065a2992548e72b06de39237ef2b802b99e3ece93ca3904a37622a66f3
   languageName: node
   linkType: hard
 
-"tar@npm:6.1.11":
+"tar@npm:6.1.11, tar@npm:^6.1.11, tar@npm:^6.1.2":
   version: 6.1.11
   resolution: "tar@npm:6.1.11"
   dependencies:
     chownr: ^2.0.0
     fs-minipass: ^2.0.0
     minipass: ^3.0.0
     minizlib: ^2.1.1
     mkdirp: ^1.0.3
     yallist: ^4.0.0
   checksum: a04c07bb9e2d8f46776517d4618f2406fb977a74d914ad98b264fc3db0fe8224da5bec11e5f8902c5b9bcb8ace22d95fbe3c7b36b8593b7dfc8391a25898f32f
   languageName: node
   linkType: hard
 
-"tar@npm:^6.1.11, tar@npm:^6.1.2":
-  version: 6.1.13
-  resolution: "tar@npm:6.1.13"
-  dependencies:
-    chownr: ^2.0.0
-    fs-minipass: ^2.0.0
-    minipass: ^4.0.0
-    minizlib: ^2.1.1
-    mkdirp: ^1.0.3
-    yallist: ^4.0.0
-  checksum: 8a278bed123aa9f53549b256a36b719e317c8b96fe86a63406f3c62887f78267cea9b22dc6f7007009738509800d4a4dccc444abd71d762287c90f35b002eb1c
-  languageName: node
-  linkType: hard
-
 "temp-dir@npm:1.0.0":
   version: 1.0.0
   resolution: "temp-dir@npm:1.0.0"
   checksum: cb2b58ddfb12efa83e939091386ad73b425c9a8487ea0095fe4653192a40d49184a771a1beba99045fbd011e389fd563122d79f54f82be86a55620667e08a6b2
   languageName: node
   linkType: hard
 
@@ -12660,15 +12605,15 @@
     temp-dir: ^2.0.0
     type-fest: ^0.16.0
     unique-string: ^2.0.0
   checksum: 11541b9d4c5b6b6e4912ded3058cfb5a1294dcc0519b73fc1fc74f950f9a68cd380f78cbefe38514ac9233f749efc6486ac14592dcb29ad35a9b3807328cba1b
   languageName: node
   linkType: hard
 
-"terser-webpack-plugin@npm:^5.1.3, terser-webpack-plugin@npm:^5.3.7":
+"terser-webpack-plugin@npm:^5.3.7":
   version: 5.3.7
   resolution: "terser-webpack-plugin@npm:5.3.7"
   dependencies:
     "@jridgewell/trace-mapping": ^0.3.17
     jest-worker: ^27.4.5
     schema-utils: ^3.1.1
     serialize-javascript: ^6.0.1
@@ -12683,24 +12628,24 @@
     uglify-js:
       optional: true
   checksum: 095e699fdeeb553cdf2c6f75f983949271b396d9c201d7ae9fc633c45c1c1ad14c7257ef9d51ccc62213dd3e97f875870ba31550f6d4f1b6674f2615562da7f7
   languageName: node
   linkType: hard
 
 "terser@npm:^5.16.5":
-  version: 5.16.8
-  resolution: "terser@npm:5.16.8"
+  version: 5.17.3
+  resolution: "terser@npm:5.17.3"
   dependencies:
     "@jridgewell/source-map": ^0.3.2
     acorn: ^8.5.0
     commander: ^2.20.0
     source-map-support: ~0.5.20
   bin:
     terser: bin/terser
-  checksum: f4a3ef4848a71f74f637c009395cf5a28660b56237fb8f13532cecfb24d6263e2dfbc1a511a11a94568988898f79cdcbecb9a4d8e104db35a0bea9639b70a325
+  checksum: 6b5a859bf9707f34be6e4c567437bc4e47e9364eec37a48b0ae3bff46bb510ef43caf543a23a89b8f43eca47c90a6759105add171fdb0d768dd639deb4545ac9
   languageName: node
   linkType: hard
 
 "test-exclude@npm:^6.0.0":
   version: 6.0.0
   resolution: "test-exclude@npm:6.0.0"
   dependencies:
@@ -12839,44 +12784,44 @@
 "trim-newlines@npm:^3.0.0":
   version: 3.0.1
   resolution: "trim-newlines@npm:3.0.1"
   checksum: b530f3fadf78e570cf3c761fb74fef655beff6b0f84b29209bac6c9622db75ad1417f4a7b5d54c96605dcd72734ad44526fef9f396807b90839449eb543c6206
   languageName: node
   linkType: hard
 
-"ts-jest@npm:^29.0.0":
-  version: 29.0.5
-  resolution: "ts-jest@npm:29.0.5"
+"ts-jest@npm:^29.1.0":
+  version: 29.1.0
+  resolution: "ts-jest@npm:29.1.0"
   dependencies:
     bs-logger: 0.x
     fast-json-stable-stringify: 2.x
     jest-util: ^29.0.0
     json5: ^2.2.3
     lodash.memoize: 4.x
     make-error: 1.x
     semver: 7.x
     yargs-parser: ^21.0.1
   peerDependencies:
     "@babel/core": ">=7.0.0-beta.0 <8"
     "@jest/types": ^29.0.0
     babel-jest: ^29.0.0
     jest: ^29.0.0
-    typescript: ">=4.3"
+    typescript: ">=4.3 <6"
   peerDependenciesMeta:
     "@babel/core":
       optional: true
     "@jest/types":
       optional: true
     babel-jest:
       optional: true
     esbuild:
       optional: true
   bin:
     ts-jest: cli.js
-  checksum: f60f129c2287f4c963d9ee2677132496c5c5a5d39c27ad234199a1140c26318a7d5bda34890ab0e30636ec42a8de28f84487c09e9dcec639c9c67812b3a38373
+  checksum: 535dc42ad523cbe1e387701fb2e448518419b515c082f09b25411f0b3dd0b854cf3e8141c316d6f4b99883aeb4a4f94159cbb1edfb06d7f77ea6229fadb2e1bf
   languageName: node
   linkType: hard
 
 "tsconfig-paths@npm:^4.1.2":
   version: 4.2.0
   resolution: "tsconfig-paths@npm:4.2.0"
   dependencies:
@@ -13036,41 +12981,41 @@
   bin:
     tsc: bin/tsc
     tsserver: bin/tsserver
   checksum: ee000bc26848147ad423b581bd250075662a354d84f0e06eb76d3b892328d8d4440b7487b5a83e851b12b255f55d71835b008a66cbf8f255a11e4400159237db
   languageName: node
   linkType: hard
 
-"typescript@npm:~5.0.2":
-  version: 5.0.2
-  resolution: "typescript@npm:5.0.2"
+"typescript@npm:~5.0.4":
+  version: 5.0.4
+  resolution: "typescript@npm:5.0.4"
   bin:
     tsc: bin/tsc
     tsserver: bin/tsserver
-  checksum: bef1dcd166acfc6934b2ec4d72f93edb8961a5fab36b8dd2aaf6f4f4cd5c0210f2e0850aef4724f3b4913d5aef203a94a28ded731b370880c8bcff7e4ff91fc1
+  checksum: 82b94da3f4604a8946da585f7d6c3025fff8410779e5bde2855ab130d05e4fd08938b9e593b6ebed165bda6ad9292b230984f10952cf82f0a0ca07bbeaa08172
   languageName: node
   linkType: hard
 
 "typescript@patch:typescript@^3 || ^4#~builtin<compat/typescript>":
   version: 4.9.5
   resolution: "typescript@patch:typescript@npm%3A4.9.5#~builtin<compat/typescript>::version=4.9.5&hash=23ec76"
   bin:
     tsc: bin/tsc
     tsserver: bin/tsserver
   checksum: ab417a2f398380c90a6cf5a5f74badd17866adf57f1165617d6a551f059c3ba0a3e4da0d147b3ac5681db9ac76a303c5876394b13b3de75fdd5b1eaa06181c9d
   languageName: node
   linkType: hard
 
-"typescript@patch:typescript@~5.0.2#~builtin<compat/typescript>":
-  version: 5.0.2
-  resolution: "typescript@patch:typescript@npm%3A5.0.2#~builtin<compat/typescript>::version=5.0.2&hash=1f5320"
+"typescript@patch:typescript@~5.0.4#~builtin<compat/typescript>":
+  version: 5.0.4
+  resolution: "typescript@patch:typescript@npm%3A5.0.4#~builtin<compat/typescript>::version=5.0.4&hash=85af82"
   bin:
     tsc: bin/tsc
     tsserver: bin/tsserver
-  checksum: bdbf3d0aac0d6cf010fbe0536753dc19f278eb4aba88140dcd25487dfe1c56ca8b33abc0dcd42078790a939b08ebc4046f3e9bb961d77d3d2c3cfa9829da4d53
+  checksum: bb309d320c59a26565fb3793dba550576ab861018ff3fd1b7fccabbe46ae4a35546bc45f342c0a0b6f265c801ccdf64ffd68f548f117ceb7f0eac4b805cd52a9
   languageName: node
   linkType: hard
 
 "typestyle@npm:^2.0.4":
   version: 2.4.0
   resolution: "typestyle@npm:2.4.0"
   dependencies:
@@ -13345,28 +13290,68 @@
 "validate.io-number@npm:^1.0.3":
   version: 1.0.3
   resolution: "validate.io-number@npm:1.0.3"
   checksum: 42418aeb6c969efa745475154fe576809b02eccd0961aad0421b090d6e7a12d23a3e28b0d5dddd2c6347c1a6bdccb82bba5048c716131cd20207244d50e07282
   languageName: node
   linkType: hard
 
+"vscode-jsonrpc@npm:8.1.0, vscode-jsonrpc@npm:^8.0.2":
+  version: 8.1.0
+  resolution: "vscode-jsonrpc@npm:8.1.0"
+  checksum: 8980037cc0014802e6ac1e5dfcff9a65e8292727096dfd23c92d2039c0c45de74a00d6ee06938cf1a671286dd8258a5f418cf048c26ad0fcb0c44f96c9e0f278
+  languageName: node
+  linkType: hard
+
+"vscode-jsonrpc@npm:^6.0.0":
+  version: 6.0.0
+  resolution: "vscode-jsonrpc@npm:6.0.0"
+  checksum: 3a67a56f287e8c449f2d9752eedf91e704dc7b9a326f47fb56ac07667631deb45ca52192e9bccb2ab108764e48409d70fa64b930d46fc3822f75270b111c5f53
+  languageName: node
+  linkType: hard
+
+"vscode-languageserver-protocol@npm:^3.17.0":
+  version: 3.17.3
+  resolution: "vscode-languageserver-protocol@npm:3.17.3"
+  dependencies:
+    vscode-jsonrpc: 8.1.0
+    vscode-languageserver-types: 3.17.3
+  checksum: ffea508b2efd7f4853f1cef5e5eac58672f0ae71a9ec275ad37a4a2a24cdc3ff023f941e759951aee01c79da3f3279f10e034f19d875f081eb387181241bd836
+  languageName: node
+  linkType: hard
+
+"vscode-languageserver-types@npm:3.17.3":
+  version: 3.17.3
+  resolution: "vscode-languageserver-types@npm:3.17.3"
+  checksum: fbc8221297261f659a6482875ff2a419dc9d55965dc53745797da569ff9f819cd832e6f2699017baadd946548bbfe212e3f6971f3d960f12dc0ee9c629dacc07
+  languageName: node
+  linkType: hard
+
 "vscode-oniguruma@npm:^1.7.0":
   version: 1.7.0
   resolution: "vscode-oniguruma@npm:1.7.0"
   checksum: 53519d91d90593e6fb080260892e87d447e9b200c4964d766772b5053f5699066539d92100f77f1302c91e8fc5d9c772fbe40fe4c90f3d411a96d5a9b1e63f42
   languageName: node
   linkType: hard
 
 "vscode-textmate@npm:^8.0.0":
   version: 8.0.0
   resolution: "vscode-textmate@npm:8.0.0"
   checksum: 127780dfea89559d70b8326df6ec344cfd701312dd7f3f591a718693812b7852c30b6715e3cfc8b3200a4e2515b4c96f0843c0eacc0a3020969b5de262c2a4bb
   languageName: node
   linkType: hard
 
+"vscode-ws-jsonrpc@npm:~1.0.2":
+  version: 1.0.2
+  resolution: "vscode-ws-jsonrpc@npm:1.0.2"
+  dependencies:
+    vscode-jsonrpc: ^8.0.2
+  checksum: eb2fdb5c96f124326505f06564dfc6584318b748fd6e39b4c0ba16a0d383d13ba0e9433596abdb841428dfc2a5501994c3206723d1cb38c6af5fcac1faf4be26
+  languageName: node
+  linkType: hard
+
 "w3c-keyname@npm:^2.2.4":
   version: 2.2.6
   resolution: "w3c-keyname@npm:2.2.6"
   checksum: 59a31d23ca9953c01c99ed6695fee5b6ea36eb2412d76a21fe4302ab33a3f5cd96c006a763940b6115c3d042c16d3564eeee1156832217d028af0518098b3a42
   languageName: node
   linkType: hard
 
@@ -13432,23 +13417,23 @@
   version: 7.0.0
   resolution: "webidl-conversions@npm:7.0.0"
   checksum: f05588567a2a76428515333eff87200fae6c83c3948a7482ebb109562971e77ef6dc49749afa58abb993391227c5697b3ecca52018793e0cb4620a48f10bd21b
   languageName: node
   linkType: hard
 
 "webpack-cli@npm:^5.0.1":
-  version: 5.0.1
-  resolution: "webpack-cli@npm:5.0.1"
+  version: 5.1.1
+  resolution: "webpack-cli@npm:5.1.1"
   dependencies:
     "@discoveryjs/json-ext": ^0.5.0
-    "@webpack-cli/configtest": ^2.0.1
+    "@webpack-cli/configtest": ^2.1.0
     "@webpack-cli/info": ^2.0.1
-    "@webpack-cli/serve": ^2.0.1
+    "@webpack-cli/serve": ^2.0.4
     colorette: ^2.0.14
-    commander: ^9.4.1
+    commander: ^10.0.1
     cross-spawn: ^7.0.3
     envinfo: ^7.7.3
     fastest-levenshtein: ^1.0.12
     import-local: ^3.0.2
     interpret: ^3.1.1
     rechoir: ^0.8.0
     webpack-merge: ^5.7.3
@@ -13459,15 +13444,15 @@
       optional: true
     webpack-bundle-analyzer:
       optional: true
     webpack-dev-server:
       optional: true
   bin:
     webpack-cli: bin/cli.js
-  checksum: b1544eea669442e78c3dba9f79c0f8d0136759b8b2fe9cd32c0d410250fd719988ae037778ba88993215d44971169f2c268c0c934068be561711615f1951bd53
+  checksum: 7738e6a84a0098886e1e0c0fd0dab44b7dedfbb0580afbb5ef734c5109dcaee80140bebb5d9f4b40f425029563bb09bcbda8b08d904fa14e60ff632e6dcc8a17
   languageName: node
   linkType: hard
 
 "webpack-merge@npm:^5.7.3, webpack-merge@npm:^5.8.0":
   version: 5.8.0
   resolution: "webpack-merge@npm:5.8.0"
   dependencies:
@@ -13491,47 +13476,47 @@
   version: 3.2.3
   resolution: "webpack-sources@npm:3.2.3"
   checksum: 989e401b9fe3536529e2a99dac8c1bdc50e3a0a2c8669cbafad31271eadd994bc9405f88a3039cd2e29db5e6d9d0926ceb7a1a4e7409ece021fe79c37d9c4607
   languageName: node
   linkType: hard
 
 "webpack@npm:^5.76.1":
-  version: 5.77.0
-  resolution: "webpack@npm:5.77.0"
+  version: 5.82.1
+  resolution: "webpack@npm:5.82.1"
   dependencies:
     "@types/eslint-scope": ^3.7.3
-    "@types/estree": ^0.0.51
-    "@webassemblyjs/ast": 1.11.1
-    "@webassemblyjs/wasm-edit": 1.11.1
-    "@webassemblyjs/wasm-parser": 1.11.1
+    "@types/estree": ^1.0.0
+    "@webassemblyjs/ast": ^1.11.5
+    "@webassemblyjs/wasm-edit": ^1.11.5
+    "@webassemblyjs/wasm-parser": ^1.11.5
     acorn: ^8.7.1
     acorn-import-assertions: ^1.7.6
     browserslist: ^4.14.5
     chrome-trace-event: ^1.0.2
-    enhanced-resolve: ^5.10.0
-    es-module-lexer: ^0.9.0
+    enhanced-resolve: ^5.14.0
+    es-module-lexer: ^1.2.1
     eslint-scope: 5.1.1
     events: ^3.2.0
     glob-to-regexp: ^0.4.1
     graceful-fs: ^4.2.9
     json-parse-even-better-errors: ^2.3.1
     loader-runner: ^4.2.0
     mime-types: ^2.1.27
     neo-async: ^2.6.2
-    schema-utils: ^3.1.0
+    schema-utils: ^3.1.2
     tapable: ^2.1.1
-    terser-webpack-plugin: ^5.1.3
+    terser-webpack-plugin: ^5.3.7
     watchpack: ^2.4.0
     webpack-sources: ^3.2.3
   peerDependenciesMeta:
     webpack-cli:
       optional: true
   bin:
     webpack: bin/webpack.js
-  checksum: 21341bb72cbbf61dfb3af91eabe9290a6c05139f268eff3c419e5339deb6c79f2f36de55d9abf017d3ccbad290a535c02325001b2816acc393f3c022e67ac17c
+  checksum: 747ee7ebd238c15249c2652060e3c6ca6d62cc66dcf7e4e2824ecd4875b7ea5e01fce8f4179080a3e84dfdb3c8d0992700444c7c5a05ef47b38c0623d3ac76de
   languageName: node
   linkType: hard
 
 "whatwg-encoding@npm:^2.0.0":
   version: 2.0.0
   resolution: "whatwg-encoding@npm:2.0.0"
   dependencies:
@@ -13891,35 +13876,28 @@
 "yaml@npm:^1.10.0":
   version: 1.10.2
   resolution: "yaml@npm:1.10.2"
   checksum: ce4ada136e8a78a0b08dc10b4b900936912d15de59905b2bf415b4d33c63df1d555d23acb2a41b23cf9fb5da41c256441afca3d6509de7247daa062fd2c5ea5f
   languageName: node
   linkType: hard
 
-"yargs-parser@npm:20.2.4":
+"yargs-parser@npm:20.2.4, yargs-parser@npm:^20.2.2, yargs-parser@npm:^20.2.3":
   version: 20.2.4
   resolution: "yargs-parser@npm:20.2.4"
   checksum: d251998a374b2743a20271c2fd752b9fbef24eb881d53a3b99a7caa5e8227fcafd9abf1f345ac5de46435821be25ec12189a11030c12ee6481fef6863ed8b924
   languageName: node
   linkType: hard
 
 "yargs-parser@npm:21.1.1, yargs-parser@npm:^21.0.1, yargs-parser@npm:^21.1.1":
   version: 21.1.1
   resolution: "yargs-parser@npm:21.1.1"
   checksum: ed2d96a616a9e3e1cc7d204c62ecc61f7aaab633dcbfab2c6df50f7f87b393993fe6640d017759fe112d0cb1e0119f2b4150a87305cc873fd90831c6a58ccf1c
   languageName: node
   linkType: hard
 
-"yargs-parser@npm:^20.2.2, yargs-parser@npm:^20.2.3":
-  version: 20.2.9
-  resolution: "yargs-parser@npm:20.2.9"
-  checksum: 8bb69015f2b0ff9e17b2c8e6bfe224ab463dd00ca211eece72a4cd8a906224d2703fb8a326d36fdd0e68701e201b2a60ed7cf81ce0fd9b3799f9fe7745977ae3
-  languageName: node
-  linkType: hard
-
 "yargs@npm:16.2.0, yargs@npm:^16.2.0":
   version: 16.2.0
   resolution: "yargs@npm:16.2.0"
   dependencies:
     cliui: ^7.0.2
     escalade: ^3.1.1
     get-caller-file: ^2.0.5
@@ -13943,19 +13921,19 @@
     y18n: ^5.0.5
     yargs-parser: ^21.1.1
   checksum: 3d8a43c336a4942bc68080768664aca85c7bd406f018bad362fd255c41c8f4e650277f42fd65d543fce99e084124ddafee7bbfc1a5c6a8fda4cec78609dcf8d4
   languageName: node
   linkType: hard
 
 "yjs@npm:^13.5.40":
-  version: 13.5.51
-  resolution: "yjs@npm:13.5.51"
+  version: 13.6.0
+  resolution: "yjs@npm:13.6.0"
   dependencies:
-    lib0: ^0.2.72
-  checksum: 4dea7a4c71163fd64f24cc153c25af641cefed7c7aadbc7e0973e2f35398635a58b5da4a45f8e10e0fc4331cde517869ac626e6b449d66766fc61d12e81b06f7
+    lib0: ^0.2.74
+  checksum: 54bd3b0c8a8dc5724044356c8015210f9840b7ac46c8d87d66a0cc5f5bf669298d45324942681ad01ea22c7a4de6a29aa22180d63596e18734bc90335ced982f
   languageName: node
   linkType: hard
 
 "yocto-queue@npm:^0.1.0":
   version: 0.1.0
   resolution: "yocto-queue@npm:0.1.0"
   checksum: f77b3d8d00310def622123df93d4ee654fc6a0096182af8bd60679ddcdfb3474c56c6c7190817c84a2785648cdee9d721c0154eb45698c62176c322fb46fc700
```

### Comparing `jupyter_collaboration-1.0.0a8/docs/Makefile` & `jupyter_collaboration-1.0.0a9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/docs/make.bat` & `jupyter_collaboration-1.0.0a9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/docs/source/conf.py` & `jupyter_collaboration-1.0.0a9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/docs/source/configuration.md` & `jupyter_collaboration-1.0.0a9/docs/source/configuration.md`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/docs/source/index.md` & `jupyter_collaboration-1.0.0a9/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/docs/source/_static/jupyter_logo.svg` & `jupyter_collaboration-1.0.0a9/docs/source/_static/jupyter_logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/docs/source/_static/logo-icon.png` & `jupyter_collaboration-1.0.0a9/docs/source/_static/logo-icon.png`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/docs/source/developer/contributing.rst` & `jupyter_collaboration-1.0.0a9/docs/source/developer/contributing.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+.. Copyright (c) Jupyter Development Team.
+.. Distributed under the terms of the Modified BSD License.
+
 Developer documentation
 =======================
 
 If you're reading this section, you're probably interested in contributing to
 Jupyter.  Welcome and thanks for your interest in contributing!
 
 Please take a look at the Contributor documentation, familiarize yourself with
@@ -25,20 +28,24 @@
 
 Installing JupyterLab Real-Time Collaboration
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The development version of the server requires `node <https://nodejs.org/en/download/>`_ and `pip <https://pip.pypa.io/en/stable/installing/>`_.
 
 Once you have installed the dependencies mentioned above, use the following
-steps::
+steps:
+
+.. code-block:: shell
 
     pip install --upgrade pip
     git clone https://github.com/jupyterlab/jupyter_collaboration
     cd jupyter_collaboration
-    pip install -e .
+    pip install -e ".[dev,test]"
+    jupyter labextension develop --overwrite .
+
 
 If you are using a system-wide Python installation and you only want to install the server for you,
 you can add ``--user`` to the install commands.
 
 Once you have done this, you can launch the main branch of Jupyter server
 from any directory in your system with::
 
@@ -90,15 +97,15 @@
 4. Verify the installation with the steps in the previous section.
 
 Running Tests
 -------------
 
 Install dependencies::
 
-    pip install -e .[test]
+    pip install -e .[dev,test]
     pip install -e examples/simple  # to test the examples
 
 To run the Python tests, use::
 
     pytest jupyter_collaboration
```

### Comparing `jupyter_collaboration-1.0.0a8/docs/source/images/rtc_shared_cursors.png` & `jupyter_collaboration-1.0.0a9/docs/source/images/rtc_shared_cursors.png`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/jupyter_collaboration/handlers.py` & `jupyter_collaboration-1.0.0a9/jupyter_collaboration/handlers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,110 +1,37 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
+from __future__ import annotations
+
 import asyncio
 import json
 import uuid
-from logging import getLogger
 from pathlib import Path
-from typing import Any, Dict, Optional, Set
+from typing import Any
 
 from jupyter_server.auth import authorized
 from jupyter_server.base.handlers import APIHandler, JupyterHandler
-from jupyter_server.serverapp import ServerWebApplication
 from jupyter_ydoc import ydocs as YDOCS
 from tornado import web
-from tornado.httputil import HTTPServerRequest
 from tornado.websocket import WebSocketHandler
-from ypy_websocket.websocket_server import WebsocketServer, YRoom
+from ypy_websocket.websocket_server import YRoom
+from ypy_websocket.ystore import BaseYStore
 from ypy_websocket.yutils import YMessageType
 
-from .loaders import FileLoader
+from .loaders import FileLoaderMapping
 from .rooms import DocumentRoom, TransientRoom
-from .utils import decode_file_path
+from .utils import JUPYTER_COLLABORATION_EVENTS_URI, LogLevel, decode_file_path
+from .websocketserver import JupyterWebsocketServer
 
 YFILE = YDOCS["file"]
 
 SERVER_SESSION = str(uuid.uuid4())
 
 
-class RoomNotFound(Exception):
-    pass
-
-
-class JupyterWebsocketServer(WebsocketServer):
-    rooms: Dict[str, YRoom]
-    ypatch_nb: int
-    connected_user: Dict[int, str]
-    background_tasks: Set[asyncio.Task[Any]]
-
-    def __init__(self, *args, **kwargs):
-        self.ystore_class = kwargs.pop("ystore_class")
-        self.log = kwargs["log"]
-        super().__init__(*args, **kwargs)
-        self.ypatch_nb = 0
-        self.connected_users = {}
-        self.background_tasks = set()
-        self.monitor_task = asyncio.create_task(self._monitor())
-
-    def room_exists(self, path: str) -> bool:
-        """
-        Returns true is the room exist or false otherwise.
-
-            Parameters:
-                path (str): Room ID.
-
-            Returns:
-                exists (bool): Whether the room exists or not.
-        """
-        return path in self.rooms
-
-    def add_room(self, path: str, room: YRoom) -> None:
-        """
-        Adds a new room.
-
-            Parameters:
-                path (str): Room ID.
-                room (YRoom): A room.
-        """
-        self.rooms[path] = room
-
-    def get_room(self, path: str) -> YRoom:
-        """
-        Returns the room for the specified room ID or raises a RoomNotFound
-        error if the room doesn't exist.
-
-            Parameters:
-                path (str): Room ID.
-
-            Returns:
-                room (YRoom): The room.
-        """
-        if path not in self.rooms:
-            # Document rooms need a file
-            raise RoomNotFound
-
-        return self.rooms[path]
-
-    async def _monitor(self):
-        """
-        An infinite loop with a 60 seconds delay for counting the number
-        of patches processed in a minute and how many clients are connected.
-
-        #### Note:
-            This method runs in a coroutine for debugging purposes.
-        """
-        while True:
-            await asyncio.sleep(60)
-            clients_nb = sum(len(room.clients) for room in self.rooms.values())
-            self.log.info("Processed %s Y patches in one minute", self.ypatch_nb)
-            self.log.info("Connected Y users: %s", clients_nb)
-            self.ypatch_nb = 0
-
-
 class YDocWebSocketHandler(WebSocketHandler, JupyterHandler):
     """`YDocWebSocketHandler` uses the singleton pattern for ``WebsocketServer``,
     which is a subclass of ypy-websocket's ``WebsocketServer``.
 
     In ``WebsocketServer``, we expect to use a WebSocket object as follows:
 
     - receive messages until the connection is closed with
@@ -117,92 +44,71 @@
        Messages received in Tornado's `on_message(message)` are put in an async
        ``_message_queue``, from which we get them asynchronously.
     - The ``send(message)`` method is async and calls Tornado's ``write_message(message)``.
     - Although it's currently not used in ypy-websocket, ``recv()`` is an async method for
        receiving a message.
     """
 
-    files: Dict[str, FileLoader] = {}
-    websocket_server: Optional[JupyterWebsocketServer] = None
-    _message_queue: "asyncio.Queue[Any]"
-
-    def __init__(
-        self, app: ServerWebApplication, request: HTTPServerRequest, **kwargs: Dict[str, Any]
-    ):
-        super().__init__(app, request, **kwargs)
-
-        # CONFIG
-        file_id_manager = self.settings["file_id_manager"]
-        ystore_class = self.settings["collaborative_ystore_class"]
-        self._cleanup_delay = self.settings["collaborative_document_cleanup_delay"]
-        # self.settings["collaborative_file_poll_interval"]
-        # self.settings["collaborative_document_save_delay"]
-
-        # Instantiate the JupyterWebsocketServer as a Class property
-        # if it doesn't exist yet
-        if self.websocket_server is None:
-            for k, v in self.config.get(ystore_class.__name__, {}).items():
-                setattr(ystore_class, k, v)
-
-            YDocWebSocketHandler.websocket_server = JupyterWebsocketServer(
-                rooms_ready=False,
-                auto_clean_rooms=False,
-                ystore_class=ystore_class,
-                log=self.log,
-            )
+    _message_queue: asyncio.Queue[Any]
+
+    def initialize(
+        self,
+        ywebsocket_server: JupyterWebsocketServer,
+        file_loaders: FileLoaderMapping,
+        ystore_class: type[BaseYStore],
+        document_cleanup_delay: float | None = 60.0,
+        document_save_delay: float | None = 1.0,
+    ) -> None:
+        # File ID manager cannot be passed as argument as the extension may load after this one
+        self._file_id_manager = self.settings["file_id_manager"]
+        self._file_loaders = file_loaders
+        self._cleanup_delay = document_cleanup_delay
+        self._websocket_server = ywebsocket_server
 
-        assert self.websocket_server is not None
         self._message_queue = asyncio.Queue()
 
         # Get room
-        self._room_id: str = request.path.split("/")[-1]
+        self._room_id: str = self.request.path.split("/")[-1]
 
-        if self.websocket_server.room_exists(self._room_id):
-            self.room: YRoom = self.websocket_server.get_room(self._room_id)
+        if self._websocket_server.room_exists(self._room_id):
+            self.room: YRoom = self._websocket_server.get_room(self._room_id)
 
         else:
             if self._room_id.count(":") >= 2:
                 # DocumentRoom
                 file_format, file_type, file_id = decode_file_path(self._room_id)
-                path = file_id_manager.get_path(file_id)
-
-                # Instantiate the FileLoader if it doesn't exist yet
-                file = YDocWebSocketHandler.files.get(file_id)
-                if file is None:
-                    self.log.info("Creating FileLoader for: %s", path)
-                    file = FileLoader(
-                        file_id,
-                        file_format,
-                        file_type,
-                        file_id_manager,
-                        self.contents_manager,
-                        self.log,
-                        self.settings["collaborative_file_poll_interval"],
+                if file_id in self._file_loaders:
+                    self._emit(
+                        LogLevel.WARNING,
+                        None,
+                        "There is another collaborative session accessing the same file.\nThe synchronization between rooms is not supported and you might lose some of your changes.",
                     )
-                    self.files[file_id] = file
 
+                file = self._file_loaders[file_id]
+                path = self._file_id_manager.get_path(file_id)
                 path = Path(path)
                 updates_file_path = str(path.parent / f".{file_type}:{path.name}.y")
                 ystore = ystore_class(path=updates_file_path, log=self.log)
                 self.room = DocumentRoom(
                     self._room_id,
                     file_format,
                     file_type,
                     file,
+                    self.event_logger,
                     ystore,
                     self.log,
-                    self.settings["collaborative_document_save_delay"],
+                    document_save_delay,
                 )
 
             else:
                 # TransientRoom
                 # it is a transient document (e.g. awareness)
                 self.room = TransientRoom(self._room_id, self.log)
 
-            self.websocket_server.add_room(self._room_id, self.room)
+            self._websocket_server.add_room(self._room_id, self.room)
 
     @property
     def path(self):
         """
         Returns the room id. It needs to be called 'path' for compatibility with
         the WebsocketServer (websocket.path).
         """
@@ -235,32 +141,43 @@
             raise web.HTTPError(403)
         return await super().get(*args, **kwargs)
 
     async def open(self, room_id):
         """
         On connection open.
         """
-        assert self.websocket_server is not None
-
-        task = asyncio.create_task(self.websocket_server.serve(self))
-        self.websocket_server.background_tasks.add(task)
-        task.add_done_callback(self.websocket_server.background_tasks.discard)
+        task = asyncio.create_task(self._websocket_server.serve(self))
+        self._websocket_server.background_tasks.add(task)
+        task.add_done_callback(self._websocket_server.background_tasks.discard)
 
         if isinstance(self.room, DocumentRoom):
             # Close the connection if the document session expired
             session_id = self.get_query_argument("sessionId", "")
             if SERVER_SESSION != session_id:
-                self.close(1003, f"Document session {session_id} expired")
+                self.close(
+                    1003,
+                    f"Document session {session_id} expired. You need to reload this browser tab.",
+                )
 
             # cancel the deletion of the room if it was scheduled
             if self.room.cleaner is not None:
                 self.room.cleaner.cancel()
 
-            # Initialize the room
-            await self.room.initialize()
+            try:
+                # Initialize the room
+                await self.room.initialize()
+            except Exception as e:
+                _, _, file_id = decode_file_path(self._room_id)
+                file = self._file_loaders[file_id]
+                self.log.error(f"Error initializing: {file.path}\n{e!r}", exc_info=e)
+                self.close(
+                    1003, f"Error initializing: {file.path}. You need to close the document."
+                )
+
+            self._emit(LogLevel.INFO, "initialize", "New client connected.")
 
     async def send(self, message):
         """
         Send a message to the client.
         """
         # needed to be compatible with WebsocketServer (websocket.send)
         try:
@@ -275,56 +192,67 @@
         message = await self._message_queue.get()
         return message
 
     def on_message(self, message):
         """
         On message receive.
         """
-        assert self.websocket_server is not None
         message_type = message[0]
         if message_type == YMessageType.AWARENESS:
             # awareness
             skip = False
             changes = self.room.awareness.get_changes(message[1:])
             added_users = changes["added"]
             removed_users = changes["removed"]
             for i, user in enumerate(added_users):
                 u = changes["states"][i]
                 if "user" in u:
                     name = u["user"]["name"]
-                    self.websocket_server.connected_users[user] = name
+                    self._websocket_server.connected_users[user] = name
                     self.log.debug("Y user joined: %s", name)
             for user in removed_users:
-                if user in self.websocket_server.connected_users:
-                    name = self.websocket_server.connected_users[user]
-                    del self.websocket_server.connected_users[user]
+                if user in self._websocket_server.connected_users:
+                    name = self._websocket_server.connected_users[user]
+                    del self._websocket_server.connected_users[user]
                     self.log.debug("Y user left: %s", name)
             # filter out message depending on changes
             if skip:
                 self.log.debug(
                     "Filtered out Y message of type: %s",
                     YMessageType(message_type).name,
                 )
                 return skip
 
         self._message_queue.put_nowait(message)
-        self.websocket_server.ypatch_nb += 1
+        self._websocket_server.ypatch_nb += 1
 
     def on_close(self) -> None:
         """
         On connection close.
         """
         # stop serving this client
         self._message_queue.put_nowait(b"")
         if isinstance(self.room, DocumentRoom) and self.room.clients == [self]:
             # no client in this room after we disconnect
             # keep the document for a while in case someone reconnects
             self.log.info("Cleaning room: %s", self._room_id)
             self.room.cleaner = asyncio.create_task(self._clean_room())
 
+    def _emit(self, level: LogLevel, action: str | None = None, msg: str | None = None) -> None:
+        _, _, file_id = decode_file_path(self._room_id)
+        path = self._file_id_manager.get_path(file_id)
+
+        data = {"level": level.value, "room": self._room_id, "path": path}
+        if action:
+            data["action"] = action
+        if msg:
+            data["msg"] = msg
+
+        self.event_logger.emit(schema_id=JUPYTER_COLLABORATION_EVENTS_URI, data=data)
+
     async def _clean_room(self) -> None:
         """
         Async task for cleaning up the resources.
 
         When all the clients of a room leave, we setup a task to clean up the resources
         after a certain amount of time. We need to wait a few seconds to clean up the room
         because sometimes websockets unintentionally disconnect.
@@ -337,59 +265,36 @@
 
         if self._cleanup_delay is None:
             return
 
         await asyncio.sleep(self._cleanup_delay)
 
         # Remove the room from the websocket server
-        assert self.websocket_server is not None
         self.log.info("Deleting Y document from memory: %s", self.room.room_id)
-        self.websocket_server.delete_room(room=self.room)
+        self._websocket_server.delete_room(room=self.room)
 
         # Clean room
         del self.room
         self.log.info("Room %s deleted", self._room_id)
+        self._emit(LogLevel.INFO, "clean", "Room deleted.")
 
         # Clean the file loader if there are not rooms using it
         _, _, file_id = decode_file_path(self._room_id)
-        file = self.files[file_id]
+        file = self._file_loaders[file_id]
         if file.number_of_subscriptions == 0:
             self.log.info("Deleting file %s", file.path)
-            file.clean()
-            del self.files[file_id]
+            del self._file_loaders[file_id]
+            self._emit(LogLevel.INFO, "clean", "Loader deleted.")
 
     def check_origin(self, origin):
         """
         Check origin
         """
         return True
 
-    @classmethod
-    def clean_up(cls):
-        """
-        Class method to stop every coroutine.
-
-        Useful to clean up tasks on server shut down.
-        """
-        log = getLogger(__name__)
-        log.info("Cleaning up resources before server shut down.")
-        if cls.websocket_server is not None:
-            # Cancel tasks and clean up
-            # TODO: should we wait for any save task?
-            rooms = list(cls.websocket_server.rooms.values())
-            log.info("Deleting rooms.")
-            for room in rooms:
-                cls.websocket_server.delete_room(room=room)
-
-        for file in cls.files.values():
-            file.clean()
-
-        log.info("Deleting files.")
-        cls.files.clear()
-
 
 class DocSessionHandler(APIHandler):
     """
     Jupyter Server's handler to retrieve the document's session.
     """
 
     auth_resource = "contents"
```

### Comparing `jupyter_collaboration-1.0.0a8/jupyter_collaboration/rooms.py` & `jupyter_collaboration-1.0.0a9/jupyter_collaboration/rooms.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,51 @@
+# Copyright (c) Jupyter Development Team.
+# Distributed under the terms of the Modified BSD License.
+
 from __future__ import annotations
 
 import asyncio
 from logging import Logger
 from typing import Any
 
+from jupyter_events import EventLogger
 from jupyter_ydoc import ydocs as YDOCS
 from ypy_websocket.websocket_server import YRoom
 from ypy_websocket.ystore import BaseYStore, YDocNotFound
 
-from .loaders import FileLoader, OutOfBandChanges
+from .loaders import FileLoader
+from .utils import JUPYTER_COLLABORATION_EVENTS_URI, LogLevel, OutOfBandChanges
 
 YFILE = YDOCS["file"]
 
 
 class DocumentRoom(YRoom):
     """A Y room for a possibly stored document (e.g. a notebook)."""
 
     def __init__(
         self,
         room_id: str,
         file_format: str,
         file_type: str,
         file: FileLoader,
+        logger: EventLogger,
         ystore: BaseYStore | None,
         log: Logger | None,
-        save_delay: int | None = None,
+        save_delay: float | None = None,
     ):
         super().__init__(ready=False, ystore=ystore, log=log)
 
         self._room_id: str = room_id
         self._file_format: str = file_format
         self._file_type: str = file_type
         self._last_modified: Any = None
         self._file: FileLoader = file
         self._document = YDOCS.get(self._file_type, YFILE)(self.ydoc)
 
+        self._logger = logger
         self._save_delay = save_delay
 
         self._update_lock = asyncio.Lock()
         self._initialization_lock = asyncio.Lock()
         self._cleaner: asyncio.Task | None = None
         self._saving_document: asyncio.Task | None = None
 
@@ -83,55 +90,77 @@
             this setter will subscribe for updates on the shared document.
         """
         async with self._initialization_lock:
             if self.ready:  # type: ignore[has-type]
                 return
 
             self.log.info("Initializing room %s", self._room_id)
+
             model = await self._file.load_content(self._file_format, self._file_type, True)
 
             async with self._update_lock:
                 # try to apply Y updates from the YStore for this document
                 read_from_source = True
                 if self.ystore is not None:
                     try:
                         await self.ystore.apply_updates(self.ydoc)
+                        self._emit(
+                            LogLevel.INFO,
+                            "load",
+                            "Content loaded from the store {}".format(
+                                self.ystore.__class__.__qualname__
+                            ),
+                        )
                         self.log.info(
                             "Content in room %s loaded from the ystore %s",
                             self._room_id,
                             self.ystore.__class__.__name__,
                         )
                         read_from_source = False
                     except YDocNotFound:
                         # YDoc not found in the YStore, create the document from the source file (no change history)
                         pass
 
                 if not read_from_source:
                     # if YStore updates and source file are out-of-sync, resync updates with source
                     if self._document.source != model["content"]:
                         # TODO: Delete document from the store.
+                        self._emit(
+                            LogLevel.INFO, "initialize", "The file is out-of-sync with the ystore."
+                        )
                         self.log.info(
                             "Content in file %s is out-of-sync with the ystore %s",
                             self._file.path,
                             self.ystore.__class__.__name__,
                         )
                         read_from_source = True
 
                 if read_from_source:
+                    self._emit(LogLevel.INFO, "load", "Content loaded from disk.")
                     self.log.info(
                         "Content in room %s loaded from file %s", self._room_id, self._file.path
                     )
                     self._document.source = model["content"]
 
                     if self.ystore:
                         await self.ystore.encode_state_as_update(self.ydoc)
 
                 self._last_modified = model["last_modified"]
                 self._document.dirty = False
                 self.ready = True
+                self._emit(LogLevel.INFO, "initialize", "Room initialized")
+
+    def _emit(self, level: LogLevel, action: str | None = None, msg: str | None = None) -> None:
+        data = {"level": level.value, "room": self._room_id, "path": self._file.path}
+        if action:
+            data["action"] = action
+        if msg:
+            data["msg"] = msg
+
+        self._logger.emit(schema_id=JUPYTER_COLLABORATION_EVENTS_URI, data=data)
 
     def _clean(self) -> None:
         """
         Cleans the rooms.
 
         Cancels the save task and unsubscribes from the file.
         """
@@ -139,26 +168,40 @@
         # TODO: Should we cancel or wait ?
         if self._saving_document:
             self._saving_document.cancel()
 
         self._document.unobserve()
         self._file.unobserve(self.room_id)
 
+    async def _broadcast_updates(self):
+        # FIXME should be upstreamed
+        try:
+            await super()._broadcast_updates()
+        except asyncio.CancelledError:
+            pass
+
     async def _on_content_change(self, event: str, args: dict[str, Any]) -> None:
         """
         Called when the file changes.
 
             Parameters:
                 event (str): Type of change.
                 args (dict): A dictionary with format, type, last_modified.
         """
         if event == "metadata" and self._last_modified < args["last_modified"]:
-            model = await self._file.load_content(self._file_format, self._file_type, True)
-
             self.log.info("Out-of-band changes. Overwriting the content in room %s", self._room_id)
+            self._emit(LogLevel.INFO, "overwrite", "Out-of-band changes. Overwriting the room.")
+
+            try:
+                model = await self._file.load_content(self._file_format, self._file_type, True)
+            except Exception as e:
+                msg = f"Error loading content from file: {self._file.path}\n{e!r}"
+                self.log.error(msg, exc_info=e)
+                self._emit(LogLevel.ERROR, None, msg)
+                return None
 
             async with self._update_lock:
                 self._document.source = model["content"]
                 self._last_modified = model["last_modified"]
                 self._document.dirty = False
 
     def _on_document_change(self, target: str, event: Any) -> None:
@@ -211,22 +254,38 @@
                     "content": self._document.source,
                 }
             )
             self._last_modified = model["last_modified"]
             async with self._update_lock:
                 self._document.dirty = False
 
+            self._emit(LogLevel.INFO, "save", "Content saved.")
+
         except OutOfBandChanges:
             self.log.info("Out-of-band changes. Overwriting the content in room %s", self._room_id)
-            model = await self._file.load_content(self._file_format, self._file_type, True)
+            try:
+                model = await self._file.load_content(self._file_format, self._file_type, True)
+            except Exception as e:
+                msg = f"Error loading content from file: {self._file.path}\n{e!r}"
+                self.log.error(msg, exc_info=e)
+                self._emit(LogLevel.ERROR, None, msg)
+                return None
+
             async with self._update_lock:
                 self._document.source = model["content"]
                 self._last_modified = model["last_modified"]
                 self._document.dirty = False
 
+            self._emit(LogLevel.INFO, "overwrite", "Out-of-band changes while saving.")
+
+        except Exception as e:
+            msg = f"Error saving file: {self._file.path}\n{e!r}"
+            self.log.error(msg, exc_info=e)
+            self._emit(LogLevel.ERROR, None, msg)
+
 
 class TransientRoom(YRoom):
     """A Y room for sharing state (e.g. awareness)."""
 
     def __init__(self, room_id: str, log: Logger | None):
         super().__init__(log=log)
 
@@ -234,7 +293,14 @@
 
     @property
     def room_id(self) -> str:
         """
         The room ID.
         """
         return self._room_id
+
+    async def _broadcast_updates(self):
+        # FIXME should be upstreamed
+        try:
+            await super()._broadcast_updates()
+        except asyncio.CancelledError:
+            pass
```

### Comparing `jupyter_collaboration-1.0.0a8/jupyter_collaboration/stores.py` & `jupyter_collaboration-1.0.0a9/jupyter_collaboration/stores.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/package.json` & `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9582341269841271%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^1.0.0-alpha.9', '@jupyter/docprovider': "*

 * *                   "'^1.0.0-alpha.9', '@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': "*

 * *                   "'^4.0.0', '@jupyterlab/codemirror': '^4.0.0', '@jupyterlab/coreutils': "*

 * *                   "'^6.0.0', '@jupyterlab/filebrowser': '^4.0.0', '@jupyterlab/services': "*

 * *                   "'^7.0.0', '@jupyterlab/settingregistry': '^4.0.0', '@jupyterlab/statedb': "*

 * *                   "'^4.0.0', '@jupyte […]*

```diff
@@ -1,38 +1,42 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^1.0.0-alpha.8",
-        "@jupyter/docprovider": "^1.0.0-alpha.8",
-        "@jupyterlab/application": "^4.0.0-beta.0",
-        "@jupyterlab/apputils": "^4.0.0-beta.0",
-        "@jupyterlab/codemirror": "^4.0.0-beta.0",
-        "@jupyterlab/coreutils": "^6.0.0-beta.0",
-        "@jupyterlab/filebrowser": "^4.0.0-beta.0",
-        "@jupyterlab/services": "^7.0.0-beta.0",
-        "@jupyterlab/settingregistry": "^4.0.0-beta.0",
-        "@jupyterlab/statedb": "^4.0.0-beta.0",
-        "@jupyterlab/translation": "^4.0.0-beta.0",
-        "@jupyterlab/ui-components": "^4.0.0-beta.0",
-        "@lumino/commands": "^2.0.0",
-        "@lumino/widgets": "^2.0.0",
+        "@jupyter/collaboration": "^1.0.0-alpha.9",
+        "@jupyter/docprovider": "^1.0.0-alpha.9",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/codemirror": "^4.0.0",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/docregistry": "^4.0.0",
+        "@jupyterlab/filebrowser": "^4.0.0",
+        "@jupyterlab/fileeditor": "^4.0.0",
+        "@jupyterlab/logconsole": "^4.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0",
+        "@jupyterlab/statedb": "^4.0.0",
+        "@jupyterlab/translation": "^4.0.0",
+        "@jupyterlab/ui-components": "^4.0.0",
+        "@lumino/commands": "^2.1.0",
+        "@lumino/widgets": "^2.1.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
         "yjs": "^13.5.40"
     },
     "description": "JupyterLab - Real-Time Collaboration Extension",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.0.0-beta.0",
-        "@types/react": "^18.0.27",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/react": "~18.0.26",
         "npm-run-all": "^4.1.5",
         "rimraf": "^4.1.2",
-        "typescript": "~5.0.2"
+        "typescript": "~5.0.4"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
         "lib/*.d.ts",
         "lib/*.js.map",
@@ -41,15 +45,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter_collaboration",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c7ae49e75d2022d8409a.js",
+            "load": "static/remoteEntry.f78dd7195bd101ba931a.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/filebrowser-extension:defaultFileBrowser"
         ],
         "extension": true,
         "outputDir": "../../jupyter_collaboration/labextension",
@@ -125,9 +129,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.8"
+    "version": "1.0.0-alpha.9"
 }
```

### Comparing `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig` & `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9585497835497836%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^1.0.0-alpha.9', '@jupyter/docprovider': "*

 * *                   "'^1.0.0-alpha.9', '@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': "*

 * *                   "'^4.0.0', '@jupyterlab/codemirror': '^4.0.0', '@jupyterlab/coreutils': "*

 * *                   "'^6.0.0', '@jupyterlab/filebrowser': '^4.0.0', '@jupyterlab/services': "*

 * *                   "'^7.0.0', '@jupyterlab/settingregistry': '^4.0.0', '@jupyterlab/statedb': "*

 * *                   "'^4.0.0', '@jupyte […]*

```diff
@@ -1,38 +1,42 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^1.0.0-alpha.8",
-        "@jupyter/docprovider": "^1.0.0-alpha.8",
-        "@jupyterlab/application": "^4.0.0-beta.0",
-        "@jupyterlab/apputils": "^4.0.0-beta.0",
-        "@jupyterlab/codemirror": "^4.0.0-beta.0",
-        "@jupyterlab/coreutils": "^6.0.0-beta.0",
-        "@jupyterlab/filebrowser": "^4.0.0-beta.0",
-        "@jupyterlab/services": "^7.0.0-beta.0",
-        "@jupyterlab/settingregistry": "^4.0.0-beta.0",
-        "@jupyterlab/statedb": "^4.0.0-beta.0",
-        "@jupyterlab/translation": "^4.0.0-beta.0",
-        "@jupyterlab/ui-components": "^4.0.0-beta.0",
-        "@lumino/commands": "^2.0.0",
-        "@lumino/widgets": "^2.0.0",
+        "@jupyter/collaboration": "^1.0.0-alpha.9",
+        "@jupyter/docprovider": "^1.0.0-alpha.9",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/codemirror": "^4.0.0",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/docregistry": "^4.0.0",
+        "@jupyterlab/filebrowser": "^4.0.0",
+        "@jupyterlab/fileeditor": "^4.0.0",
+        "@jupyterlab/logconsole": "^4.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0",
+        "@jupyterlab/statedb": "^4.0.0",
+        "@jupyterlab/translation": "^4.0.0",
+        "@jupyterlab/ui-components": "^4.0.0",
+        "@lumino/commands": "^2.1.0",
+        "@lumino/widgets": "^2.1.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
         "yjs": "^13.5.40"
     },
     "description": "JupyterLab - Real-Time Collaboration Extension",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.0.0-beta.0",
-        "@types/react": "^18.0.27",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/react": "~18.0.26",
         "npm-run-all": "^4.1.5",
         "rimraf": "^4.1.2",
-        "typescript": "~5.0.2"
+        "typescript": "~5.0.4"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
         "lib/*.d.ts",
         "lib/*.js.map",
@@ -120,9 +124,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.8"
+    "version": "1.0.0-alpha.9"
 }
```

### Comparing `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/413.cf154c48ecaa08648e56.js` & `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/413.cf154c48ecaa08648e56.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/493.0975334cbddac1bcf819.js` & `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/493.efdf15c07c2318ee4cd7.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                 Te: () => y,
                 Gh: () => v,
                 s3: () => b
             });
             var r = n(5931),
                 s = n(3205);
             var o = n(5852),
-                c = n(1985),
+                c = n(1872),
                 a = n(4406);
             const i = void 0 !== a && a.release && /node|io\.js/.test(a.release.name),
                 l = "undefined" != typeof window && "undefined" != typeof document && !i;
             let u;
             "undefined" != typeof navigator && /Mac/.test(navigator.platform);
             const h = [],
                 f = t => (() => {
@@ -194,15 +194,15 @@
                             o = s.VV(n - r, e.length),
                             c = e.length - o;
                         t.cbuf.set(e.subarray(0, o), r), t.cpos += o, c > 0 && (t.bufs.push(t.cbuf), t.cbuf = new Uint8Array(s.Fp(2 * n, c)), t.cbuf.set(e.subarray(o)), t.cpos = c)
                     })(t, e)
                 };
             new DataView(new ArrayBuffer(4))
         },
-        1985: (t, e, n) => {
+        1872: (t, e, n) => {
             "use strict";
             n.d(e, {
                 Hi: () => s,
                 gB: () => o
             });
             var r = n(9600);
             const s = (t, e) => {
@@ -488,15 +488,15 @@
                 xq: () => h
             });
             var r = n(9476),
                 s = n(2256),
                 o = n(870),
                 c = n(1332),
                 a = n(2019),
-                i = n(1985);
+                i = n(1872);
             n(981);
             class l extends a.y {
                 constructor(t) {
                     super(), this.doc = t, this.clientID = t.clientID, this.states = new Map, this.meta = new Map, this._checkInterval = setInterval((() => {
                         const t = o.ZG();
                         null !== this.getLocalState() && 15e3 <= t - this.meta.get(this.clientID).lastUpdated && this.setLocalState(this.getLocalState());
                         const e = [];
```

### Comparing `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/497.ab1a0ee570b8e4f31289.js` & `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/87.c69c6c0210f40538f288.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,213 +1,288 @@
 "use strict";
 (self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || []).push([
-    [497], {
-        9497: (e, t, r) => {
-            r.r(t), r.d(t, {
-                default: () => S
+    [87], {
+        5087: (e, o, t) => {
+            t.r(o), t.d(o, {
+                default: () => B
             });
-            var o, n = r(2281),
-                a = r(1371),
-                i = r(726),
-                s = r(5581),
-                l = r(3e3),
-                c = r(5996);
+            var r, a = t(2177),
+                n = t(9324),
+                s = t(5355),
+                i = t(2497),
+                l = t(5116),
+                c = t(899),
+                d = t(94),
+                u = t(7387),
+                p = t(2293),
+                v = t(1039);
             ! function(e) {
                 e.openPath = "filebrowser:open-path"
-            }(o || (o = {}));
-            const d = {
+            }(r || (r = {}));
+            const m = {
                     id: "@jupyter/collaboration-extension:drive",
                     description: "The default collaborative drive provider",
-                    provides: c.ICollaborativeDrive,
-                    requires: [i.ITranslator],
+                    provides: v.ICollaborativeDrive,
+                    requires: [u.ITranslator],
                     optional: [],
-                    activate: (e, t) => {
-                        const r = t.load("jupyter_collaboration"),
-                            o = new c.YDrive(e.serviceManager.user, r);
-                        return e.serviceManager.contents.addDrive(o), o
+                    activate: (e, o) => {
+                        const t = o.load("jupyter_collaboration"),
+                            r = new v.YDrive(e.serviceManager.user, t);
+                        return e.serviceManager.contents.addDrive(r), r
                     }
                 },
-                u = {
+                g = {
                     id: "@jupyter/collaboration-extension:yfile",
                     description: "Plugin to register the shared model factory for the content type 'file'",
                     autoStart: !0,
-                    requires: [c.ICollaborativeDrive],
+                    requires: [v.ICollaborativeDrive],
                     optional: [],
-                    activate: (e, t) => {
-                        t.sharedModelFactory.registerDocumentFactory("file", (() => new l.YFile))
+                    activate: (e, o) => {
+                        o.sharedModelFactory.registerDocumentFactory("file", (() => new p.YFile))
                     }
                 },
-                p = {
+                y = {
                     id: "@jupyter/collaboration-extension:ynotebook",
                     description: "Plugin to register the shared model factory for the content type 'notebook'",
                     autoStart: !0,
-                    requires: [c.ICollaborativeDrive],
-                    optional: [s.ISettingRegistry],
-                    activate: (e, t, r) => {
-                        let o = !0;
-                        r && r.load("@jupyterlab/notebook-extension:tracker").then((e => {
-                            const t = e => {
-                                var t;
-                                const r = null == e ? void 0 : e.get("experimentalEnableDocumentWideUndoRedo").composite;
-                                o = null === (t = !r) || void 0 === t || t
+                    requires: [v.ICollaborativeDrive],
+                    optional: [d.ISettingRegistry],
+                    activate: (e, o, t) => {
+                        let r = !0;
+                        t && t.load("@jupyterlab/notebook-extension:tracker").then((e => {
+                            const o = e => {
+                                var o;
+                                const t = null == e ? void 0 : e.get("experimentalEnableDocumentWideUndoRedo").composite;
+                                r = null === (o = !t) || void 0 === o || o
                             };
-                            t(e), e.changed.connect((e => t(e)))
-                        })), t.sharedModelFactory.registerDocumentFactory("notebook", (() => new l.YNotebook({
-                            disableDocumentWideUndoRedo: o
+                            o(e), e.changed.connect((e => o(e)))
+                        })), o.sharedModelFactory.registerDocumentFactory("notebook", (() => new p.YNotebook({
+                            disableDocumentWideUndoRedo: r
                         })))
                     }
                 },
-                v = {
+                b = {
                     id: "@jupyter/collaboration-extension:defaultFileBrowser",
                     description: "The default file browser factory provider",
-                    provides: a.IDefaultFileBrowser,
-                    requires: [c.ICollaborativeDrive, a.IFileBrowserFactory],
-                    optional: [n.IRouter, n.JupyterFrontEnd.ITreeResolver, n.ILabShell, s.ISettingRegistry],
-                    activate: async (e, t, r, o, n, a) => {
+                    provides: s.IDefaultFileBrowser,
+                    requires: [v.ICollaborativeDrive, s.IFileBrowserFactory],
+                    optional: [a.IRouter, a.JupyterFrontEnd.ITreeResolver, a.ILabShell, d.ISettingRegistry],
+                    activate: async (e, o, t, r, a, n) => {
                         const {
-                            commands: i
+                            commands: s
                         } = e;
-                        e.serviceManager.contents.addDrive(t);
-                        const s = r.createFileBrowser("filebrowser", {
+                        e.serviceManager.contents.addDrive(o);
+                        const i = t.createFileBrowser("filebrowser", {
                             auto: !1,
                             restore: !1,
-                            driveName: t.name
+                            driveName: o.name
                         });
-                        return b.restoreBrowser(s, i, o, n, a), s
+                        return w.restoreBrowser(i, s, r, a, n), i
+                    }
+                },
+                h = {
+                    id: "@jupyter/collaboration-extension:logger",
+                    description: "A logging plugin for debugging purposes.",
+                    autoStart: !0,
+                    optional: [l.ILoggerRegistry, i.IEditorTracker, c.INotebookTracker, u.ITranslator],
+                    activate: (e, o, t, r, a) => {
+                        const s = (null != a ? a : u.nullTranslator).load("jupyter_collaboration"),
+                            i = "https://schema.jupyter.org/jupyter_collaboration/session/v1";
+                        if (!o) return void e.serviceManager.events.stream.connect(((e, o) => {
+                            var t, r;
+                            o.schema_id === i && (console.debug(`[${o.room}(${o.path})] ${null!==(t=o.action)&&void 0!==t?t:""}: ${null!==(r=o.msg)&&void 0!==r?r:""}`), "WARNING" === o.level && (0, n.showDialog)({
+                                title: s.__("Warning"),
+                                body: s.__(`Two collaborative sessions are accessing the file ${o.path} simultaneously.\n                \nOpening the same file using different views simultaneously is not supported. Please, close one view; otherwise, you might lose some of your progress.`),
+                                buttons: [n.Dialog.okButton()]
+                            }))
+                        }));
+                        const l = new Map,
+                            c = (e, t) => {
+                                const r = o.getLogger(t.context.path);
+                                l.set(t.context.localPath, r), t.disposed.connect((e => {
+                                    l.delete(e.context.localPath)
+                                }))
+                            };
+                        t && t.widgetAdded.connect(c), r && r.widgetAdded.connect(c), (async () => {
+                            var o, t;
+                            const {
+                                events: r
+                            } = e.serviceManager;
+                            for await (const e of r.stream) if (e.schema_id === i) {
+                                const r = l.get(e.path);
+                                null == r || r.log({
+                                    type: "text",
+                                    level: e.level.toLowerCase(),
+                                    data: `[${e.room}] ${null!==(o=e.action)&&void 0!==o?o:""}: ${null!==(t=e.msg)&&void 0!==t?t:""}`
+                                }), "WARNING" === e.level && (0, n.showDialog)({
+                                    title: s.__("Warning"),
+                                    body: s.__("Two collaborative sessions are accessing the file %1 simultaneously.\n                \n'Opening a document with multiple views simultaneously is not supported. Please close one view; otherwise, you might lose some of your progress.", e.path),
+                                    buttons: [n.Dialog.warnButton({
+                                        label: s.__("Ok")
+                                    })]
+                                })
+                            }
+                        })()
                     }
                 };
-            var b;
+            var w;
             ! function(e) {
-                e.restoreBrowser = async function(e, t, r, n, a) {
-                    const i = "jp-mod-restoring";
-                    if (e.addClass(i), !r) return await e.model.restore(e.id), await e.model.refresh(), void e.removeClass(i);
-                    const s = async () => {
-                        r.routed.disconnect(s);
-                        const l = await (null == n ? void 0 : n.paths);
-                        (null == l ? void 0 : l.file) || (null == l ? void 0 : l.browser) ? (await e.model.restore(e.id, !1), l.file && await t.execute(o.openPath, {
+                e.restoreBrowser = async function(e, o, t, a, n) {
+                    const s = "jp-mod-restoring";
+                    if (e.addClass(s), !t) return await e.model.restore(e.id), await e.model.refresh(), void e.removeClass(s);
+                    const i = async () => {
+                        t.routed.disconnect(i);
+                        const l = await (null == a ? void 0 : a.paths);
+                        (null == l ? void 0 : l.file) || (null == l ? void 0 : l.browser) ? (await e.model.restore(e.id, !1), l.file && await o.execute(r.openPath, {
                             path: l.file,
                             dontShowBrowser: !0
-                        }), l.browser && await t.execute(o.openPath, {
+                        }), l.browser && await o.execute(r.openPath, {
                             path: l.browser,
                             dontShowBrowser: !0
-                        })) : (await e.model.restore(e.id), await e.model.refresh()), e.removeClass(i), (null == a ? void 0 : a.isEmpty("main")) && t.execute("launcher:create")
+                        })) : (await e.model.restore(e.id), await e.model.refresh()), e.removeClass(s), (null == n ? void 0 : n.isEmpty("main")) && o.execute("launcher:create")
                     };
-                    r.routed.connect(s)
+                    t.routed.connect(i)
                 }
-            }(b || (b = {}));
-            var w = r(60),
-                y = r(7478),
-                m = r(9041),
-                h = r(9190),
-                f = r(8778),
-                g = r(4989),
-                x = r(8256),
-                I = r(1682),
-                M = r(981),
-                C = r(6493),
-                j = r(7099);
-            const S = [d, u, p, v, {
-                id: "@jupyter/collaboration-extension:userMenu",
-                description: "Provide connected user menu.",
-                requires: [],
-                provides: m.IUserMenu,
-                activate: e => {
-                    const {
-                        commands: t
-                    } = e, {
-                        user: r
-                    } = e.serviceManager;
-                    return new m.UserMenu({
-                        commands: t,
-                        user: r
-                    })
-                }
-            }, {
-                id: "@jupyter/collaboration-extension:userMenuBar",
-                description: "Add user menu to the interface.",
-                autoStart: !0,
-                requires: [m.IUserMenu],
-                activate: async (e, t) => {
-                    const {
-                        shell: r
-                    } = e, {
-                        user: o
-                    } = e.serviceManager, n = new f.MenuBar({
-                        forceItemsPosition: {
-                            forceX: !1,
-                            forceY: !1
-                        },
-                        renderer: new m.RendererUserMenu(o)
-                    });
-                    n.id = "jp-UserMenu", o.userChanged.connect((() => n.update())), n.addMenu(t), r.add(n, "top", {
-                        rank: 1e3
-                    })
-                }
-            }, {
-                id: "@jupyter/collaboration-extension:rtcGlobalAwareness",
-                description: "Add global awareness to share working document of users.",
-                requires: [I.IStateDB],
-                provides: m.IGlobalAwareness,
-                activate: (e, t) => {
-                    const {
-                        user: r
-                    } = e.serviceManager, o = new M.Doc, n = new C.GL(o), a = x.ServerConnection.makeSettings(), i = g.URLExt.join(a.wsUrl, "api/collaboration/room");
-                    new j.WebsocketProvider(i, "JupyterLab:globalAwareness", o, {
-                        awareness: n
-                    });
-                    const s = () => {
-                        n.setLocalStateField("user", r.identity)
-                    };
-                    return r.isReady && s(), r.ready.then(s).catch((e => console.error(e))), r.userChanged.connect(s), t.changed.connect((async () => {
-                        var e, r;
-                        const o = (null === (r = null === (e = (await t.toJSON())["layout-restorer:data"]) || void 0 === e ? void 0 : e.main) || void 0 === r ? void 0 : r.current) || "";
-                        o.startsWith("editor") || o.startsWith("notebook") ? n.setLocalStateField("current", o) : n.setLocalStateField("current", null)
-                    })), n
-                }
-            }, {
-                id: "@jupyter/collaboration-extension:rtcPanel",
-                description: "Add side panel to display all currently connected users.",
-                autoStart: !0,
-                requires: [m.IGlobalAwareness],
-                optional: [i.ITranslator],
-                activate: (e, t, r) => {
-                    const {
-                        user: o
-                    } = e.serviceManager, n = (null != r ? r : i.nullTranslator).load("jupyter_collaboration"), a = new h.SidePanel({
-                        alignment: "justify"
-                    });
-                    a.id = w.DOMUtils.createDomID(), a.title.icon = h.usersIcon, a.title.caption = n.__("Collaboration"), a.addClass("jp-RTCPanel"), e.shell.add(a, "left", {
-                        rank: 300
-                    });
-                    const s = new m.UserInfoPanel(o);
-                    s.title.label = n.__("User info"), s.title.caption = n.__("User information"), a.addWidget(s);
-                    const l = new m.CollaboratorsPanel(o, t, (t => {
-                        e.commands.execute("docmanager:open", {
-                            path: t
+            }(w || (w = {}));
+            var f = t(674),
+                I = t(6903),
+                _ = t(3897),
+                x = t(8778),
+                j = t(9474),
+                k = t(3020),
+                C = t(1802),
+                S = t(981),
+                M = t(6493),
+                D = t(7099);
+            const P = {
+                    id: "@jupyter/collaboration-extension:userMenu",
+                    description: "Provide connected user menu.",
+                    requires: [],
+                    provides: I.IUserMenu,
+                    activate: e => {
+                        const {
+                            commands: o
+                        } = e, {
+                            user: t
+                        } = e.serviceManager;
+                        return new I.UserMenu({
+                            commands: o,
+                            user: t
                         })
-                    }));
-                    l.title.label = n.__("Online Collaborators"), a.addWidget(l)
-                }
-            }, {
-                id: "@jupyter/collaboration-extension:userEditorCursors",
-                description: "Add CodeMirror extension to display remote user cursors and selections.",
+                    }
+                },
+                T = {
+                    id: "@jupyter/collaboration-extension:user-menu-bar",
+                    description: "Add user menu to the interface.",
+                    autoStart: !0,
+                    requires: [I.IUserMenu, n.IToolbarWidgetRegistry],
+                    activate: async (e, o, t) => {
+                        const {
+                            user: r
+                        } = e.serviceManager, a = new x.MenuBar({
+                            forceItemsPosition: {
+                                forceX: !1,
+                                forceY: !1
+                            },
+                            renderer: new I.RendererUserMenu(r)
+                        });
+                        a.id = "jp-UserMenu", r.userChanged.connect((() => a.update())), a.addMenu(o), t.addFactory("TopBar", "user-menu", (() => a))
+                    }
+                },
+                R = {
+                    id: "@jupyter/collaboration-extension:rtcGlobalAwareness",
+                    description: "Add global awareness to share working document of users.",
+                    requires: [C.IStateDB],
+                    provides: I.IGlobalAwareness,
+                    activate: (e, o) => {
+                        const {
+                            user: t
+                        } = e.serviceManager, r = new S.Doc, a = new M.GL(r), n = k.ServerConnection.makeSettings(), s = j.URLExt.join(n.wsUrl, "api/collaboration/room");
+                        new D.WebsocketProvider(s, "JupyterLab:globalAwareness", r, {
+                            awareness: a
+                        });
+                        const i = () => {
+                            a.setLocalStateField("user", t.identity)
+                        };
+                        return t.isReady && i(), t.ready.then(i).catch((e => console.error(e))), t.userChanged.connect(i), o.changed.connect((async () => {
+                            var e, t;
+                            const r = (null === (t = null === (e = (await o.toJSON())["layout-restorer:data"]) || void 0 === e ? void 0 : e.main) || void 0 === t ? void 0 : t.current) || "";
+                            r.startsWith("editor") || r.startsWith("notebook") ? a.setLocalStateField("current", r) : a.setLocalStateField("current", null)
+                        })), a
+                    }
+                },
+                F = {
+                    id: "@jupyter/collaboration-extension:rtcPanel",
+                    description: "Add side panel to display all currently connected users.",
+                    autoStart: !0,
+                    requires: [I.IGlobalAwareness],
+                    optional: [u.ITranslator],
+                    activate: (e, o, t) => {
+                        const {
+                            user: r
+                        } = e.serviceManager, a = (null != t ? t : u.nullTranslator).load("jupyter_collaboration"), s = new _.SidePanel({
+                            alignment: "justify"
+                        });
+                        s.id = n.DOMUtils.createDomID(), s.title.icon = _.usersIcon, s.title.caption = a.__("Collaboration"), s.addClass("jp-RTCPanel"), e.shell.add(s, "left", {
+                            rank: 300
+                        });
+                        const i = new I.UserInfoPanel(r);
+                        i.title.label = a.__("User info"), i.title.caption = a.__("User information"), s.addWidget(i);
+                        const l = new I.CollaboratorsPanel(r, o, (o => {
+                            e.commands.execute("docmanager:open", {
+                                path: o
+                            })
+                        }));
+                        l.title.label = a.__("Online Collaborators"), s.addWidget(l)
+                    }
+                },
+                U = {
+                    id: "@jupyter/collaboration-extension:userEditorCursors",
+                    description: "Add CodeMirror extension to display remote user cursors and selections.",
+                    autoStart: !0,
+                    requires: [f.IEditorExtensionRegistry],
+                    activate: (e, o) => {
+                        o.addExtension({
+                            name: "remote-user-cursors",
+                            factory(e) {
+                                const {
+                                    awareness: o,
+                                    ysource: t
+                                } = e.model.sharedModel;
+                                return f.EditorExtensionRegistry.createImmutableExtension((0, I.remoteUserCursors)({
+                                    awareness: o,
+                                    ytext: t
+                                }))
+                            }
+                        })
+                    }
+                };
+            var A;
+            ! function(e) {
+                e.share = "collaboration:shared-link"
+            }(A || (A = {}));
+            const B = [m, g, y, b, h, P, T, R, F, {
+                id: "@jupyter/collaboration-extension:shared-link",
                 autoStart: !0,
-                requires: [y.IEditorExtensionRegistry],
-                activate: (e, t) => {
-                    t.addExtension({
-                        name: "remote-user-cursors",
-                        factory(e) {
-                            const {
-                                awareness: t,
-                                ysource: r
-                            } = e.model.sharedModel;
-                            return y.EditorExtensionRegistry.createImmutableExtension((0, m.remoteUserCursors)({
-                                awareness: t,
-                                ytext: r
-                            }))
+                optional: [n.ICommandPalette, u.ITranslator],
+                activate: async (e, o, t) => {
+                    const {
+                        commands: r
+                    } = e, a = (null != t ? t : u.nullTranslator).load("collaboration");
+                    r.addCommand(A.share, {
+                        label: a.__("Generate a Shared Link"),
+                        icon: _.shareIcon,
+                        execute: async () => {
+                            const e = await (0, I.showSharedLinkDialog)({
+                                translator: t
+                            });
+                            e.button.accept && e.value && n.Clipboard.copyToSystem(e.value)
                         }
+                    }), o && o.addItem({
+                        command: A.share,
+                        category: a.__("Server")
                     })
                 }
-            }]
+            }, U]
         }
     }
 ]);
```

### Comparing `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/8.6b2a09634af3599cbddb.js` & `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/8.883cdb5327aeb22e2587.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,104 +1,103 @@
 "use strict";
 (self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || []).push([
     [8, 933], {
         2008: (e, t, s) => {
             s.r(t), s.d(t, {
-                ICollaborativeDrive: () => p,
+                ICollaborativeDrive: () => _,
                 WebSocketProvider: () => h,
                 YDrive: () => d
             });
-            var o = s(60),
-                r = s(4989),
-                n = s(8256),
+            var o = s(9474),
+                r = s(3020),
+                n = s(9324),
                 i = s(7930),
                 a = s(4901),
                 c = s(7099);
             class h {
                 constructor(e) {
                     this._onConnectionClosed = e => {
-                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, o.showErrorMessage)(this._trans.__("Session expired"), this._trans.__("The document session expired. You need to reload this browser tab."), [o.Dialog.okButton({
-                            label: this._trans.__("Reload")
-                        })]).then((e => {
-                            e.button.accept && window.location.reload()
-                        })).catch((e => window.location.reload())), this._sharedModel.dispose())
+                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, n.showErrorMessage)(this._trans.__("Document session error"), e.reason, [n.Dialog.okButton()]), this._sharedModel.dispose())
+                    }, this._onSync = e => {
+                        var t;
+                        e && (this._ready.resolve(), null === (t = this._yWebsocketProvider) || void 0 === t || t.off("sync", this._onSync))
                     }, this._ready = new i.PromiseDelegate, this._isDisposed = !1, this._path = e.path, this._contentType = e.contentType, this._format = e.format, this._serverUrl = e.url, this._sharedModel = e.model, this._awareness = e.model.awareness, this._yWebsocketProvider = null, this._trans = e.translator;
                     const t = e.user;
                     t.ready.then((() => {
                         this._onUserChanged(t)
-                    })).catch((e => console.error(e))), t.userChanged.connect(this._onUserChanged, this), this._connect()
+                    })).catch((e => console.error(e))), t.userChanged.connect(this._onUserChanged, this), this._connect().catch((e => console.warn(e)))
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 get ready() {
                     return this._ready.promise
                 }
                 dispose() {
-                    var e, t;
-                    this.isDisposed || (this._isDisposed = !0, null === (e = this._yWebsocketProvider) || void 0 === e || e.off("connection-close", this._onConnectionClosed), null === (t = this._yWebsocketProvider) || void 0 === t || t.destroy(), a.Signal.clearData(this))
+                    var e, t, s;
+                    this.isDisposed || (this._isDisposed = !0, null === (e = this._yWebsocketProvider) || void 0 === e || e.off("connection-close", this._onConnectionClosed), null === (t = this._yWebsocketProvider) || void 0 === t || t.off("sync", this._onSync), null === (s = this._yWebsocketProvider) || void 0 === s || s.destroy(), a.Signal.clearData(this))
                 }
-                _connect() {
-                    (async function(e, t, s) {
-                        const {
-                            makeSettings: o,
-                            makeRequest: i,
-                            ResponseError: a
-                        } = n.ServerConnection, c = o(), h = r.URLExt.join(c.baseUrl, "api/collaboration/session", encodeURIComponent(s)), d = {
-                            method: "PUT",
-                            body: JSON.stringify({
-                                format: e,
-                                type: t
-                            })
-                        }, l = await i(h, d, c);
-                        if (200 !== l.status && 201 !== l.status) throw new a(l);
-                        return l.json()
-                    })(this._format, this._contentType, this._path).then((e => {
-                        this._yWebsocketProvider = new c.WebsocketProvider(this._serverUrl, `${e.format}:${e.type}:${e.fileId}`, this._sharedModel.ydoc, {
-                            disableBc: !0,
-                            params: {
-                                sessionId: e.sessionId
-                            },
-                            awareness: this._awareness
-                        }), this._yWebsocketProvider.on("connection-close", this._onConnectionClosed)
-                    })).then((e => this._ready.resolve())).catch((e => console.warn(e)))
+                async _connect() {
+                    const e = await async function(e, t, s) {
+                        const n = r.ServerConnection.makeSettings(),
+                            i = o.URLExt.join(n.baseUrl, "api/collaboration/session", encodeURIComponent(s)),
+                            a = {
+                                method: "PUT",
+                                body: JSON.stringify({
+                                    format: e,
+                                    type: t
+                                })
+                            };
+                        let c;
+                        try {
+                            c = await r.ServerConnection.makeRequest(i, a, n)
+                        } catch (e) {
+                            throw new r.ServerConnection.NetworkError(e)
+                        }
+                        let h = await c.text();
+                        if (h.length > 0) try {
+                            h = JSON.parse(h)
+                        } catch (e) {
+                            console.log("Not a JSON response body.", c)
+                        }
+                        if (!c.ok) throw new r.ServerConnection.ResponseError(c, h.message || h);
+                        return h
+                    }(this._format, this._contentType, this._path);
+                    this._yWebsocketProvider = new c.WebsocketProvider(this._serverUrl, `${e.format}:${e.type}:${e.fileId}`, this._sharedModel.ydoc, {
+                        disableBc: !0,
+                        params: {
+                            sessionId: e.sessionId
+                        },
+                        awareness: this._awareness
+                    }), this._yWebsocketProvider.on("sync", this._onSync), this._yWebsocketProvider.on("connection-close", this._onConnectionClosed)
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            class d extends n.Drive {
+            class d extends r.Drive {
                 constructor(e, t) {
                     super({
                         name: "RTC"
                     }), this._onCreate = (e, t) => {
                         if ("string" == typeof e.format) try {
                             const s = new h({
-                                    url: r.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
+                                    url: o.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
                                     path: e.path,
                                     format: e.format,
                                     contentType: e.contentType,
                                     model: t,
                                     user: this._user,
                                     translator: this._trans
                                 }),
-                                n = `${e.format}:${e.contentType}:${e.path}`;
-                            this._providers.set(n, s), t.disposed.connect((() => {
-                                const e = this._providers.get(n);
-                                e && (e.dispose(), this._providers.delete(n))
-                            }));
-                            for (const t of this._providers.keys()) {
-                                if (t === n) continue;
-                                const s = t.split(":")[2];
-                                e.path === s && (0, o.showDialog)({
-                                    title: this._trans.__("Warning"),
-                                    body: this._trans.__("Opening a document with multiple views simultaneously is not supported.Please, close one view otherwise, you might lose some of your changes."),
-                                    buttons: [o.Dialog.okButton()]
-                                })
-                            }
+                                r = `${e.format}:${e.contentType}:${e.path}`;
+                            this._providers.set(r, s), t.disposed.connect((() => {
+                                const e = this._providers.get(r);
+                                e && (e.dispose(), this._providers.delete(r))
+                            }))
                         } catch (t) {
                             console.error(`Failed to open websocket connection for ${e.path}.\n:${t}`)
                         }
                     }, this._user = e, this._trans = t, this._providers = new Map, this.sharedModelFactory = new l(this._onCreate)
                 }
                 dispose() {
                     this.isDisposed || (this._providers.forEach((e => e.dispose())), this._providers.clear(), super.dispose())
@@ -141,11 +140,11 @@
                         if (e.collaborative && this._documentFactories.has(e.contentType)) {
                             const t = this._documentFactories.get(e.contentType)(e);
                             return this._onCreate(e, t), t
                         }
                     } else console.warn(`Only defined format are supported; got ${e.format}.`)
                 }
             }
-            const p = new i.Token("@jupyter/collaboration-extension:ICollaborativeDrive")
+            const _ = new i.Token("@jupyter/collaboration-extension:ICollaborativeDrive")
         }
     }
 ]);
```

### Comparing `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/839.2efa17f8ec8b5c6c87a6.js` & `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/839.14d748171b9c87a422f9.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
             var r = o(9601),
                 t = o.n(r),
                 i = o(2609),
                 a = o.n(i),
                 l = o(6435),
                 c = o(8974),
                 p = a()(t());
-            p.i(l.Z), p.i(c.Z), p.push([n.id, "/* -----------------------------------------------------------------------------\n| Copyright (c) Jupyter Development Team.\n| Distributed under the terms of the Modified BSD License.\n|---------------------------------------------------------------------------- */\n", ""]);
+            p.i(l.Z), p.i(c.Z), p.push([n.id, "/* -----------------------------------------------------------------------------\n| Copyright (c) Jupyter Development Team.\n| Distributed under the terms of the Modified BSD License.\n|---------------------------------------------------------------------------- */\n\n.jp-shared-link-body {\n    user-select: none;\n}\n", ""]);
             const s = p
         },
         6435: (n, e, o) => {
             o.d(e, {
                 Z: () => l
             });
             var r = o(9601),
```

### Comparing `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/933.f161fc3dcf0d2c141b27.js` & `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/933.737bcc7ac7d9a6826f35.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,104 +1,103 @@
 "use strict";
 (self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || []).push([
     [933, 8], {
         2008: (e, t, s) => {
             s.r(t), s.d(t, {
-                ICollaborativeDrive: () => p,
+                ICollaborativeDrive: () => _,
                 WebSocketProvider: () => h,
                 YDrive: () => d
             });
-            var o = s(60),
-                r = s(4989),
-                n = s(8256),
+            var o = s(9474),
+                r = s(3020),
+                n = s(9324),
                 i = s(7930),
                 a = s(4901),
                 c = s(7099);
             class h {
                 constructor(e) {
                     this._onConnectionClosed = e => {
-                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, o.showErrorMessage)(this._trans.__("Session expired"), this._trans.__("The document session expired. You need to reload this browser tab."), [o.Dialog.okButton({
-                            label: this._trans.__("Reload")
-                        })]).then((e => {
-                            e.button.accept && window.location.reload()
-                        })).catch((e => window.location.reload())), this._sharedModel.dispose())
+                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, n.showErrorMessage)(this._trans.__("Document session error"), e.reason, [n.Dialog.okButton()]), this._sharedModel.dispose())
+                    }, this._onSync = e => {
+                        var t;
+                        e && (this._ready.resolve(), null === (t = this._yWebsocketProvider) || void 0 === t || t.off("sync", this._onSync))
                     }, this._ready = new i.PromiseDelegate, this._isDisposed = !1, this._path = e.path, this._contentType = e.contentType, this._format = e.format, this._serverUrl = e.url, this._sharedModel = e.model, this._awareness = e.model.awareness, this._yWebsocketProvider = null, this._trans = e.translator;
                     const t = e.user;
                     t.ready.then((() => {
                         this._onUserChanged(t)
-                    })).catch((e => console.error(e))), t.userChanged.connect(this._onUserChanged, this), this._connect()
+                    })).catch((e => console.error(e))), t.userChanged.connect(this._onUserChanged, this), this._connect().catch((e => console.warn(e)))
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 get ready() {
                     return this._ready.promise
                 }
                 dispose() {
-                    var e, t;
-                    this.isDisposed || (this._isDisposed = !0, null === (e = this._yWebsocketProvider) || void 0 === e || e.off("connection-close", this._onConnectionClosed), null === (t = this._yWebsocketProvider) || void 0 === t || t.destroy(), a.Signal.clearData(this))
+                    var e, t, s;
+                    this.isDisposed || (this._isDisposed = !0, null === (e = this._yWebsocketProvider) || void 0 === e || e.off("connection-close", this._onConnectionClosed), null === (t = this._yWebsocketProvider) || void 0 === t || t.off("sync", this._onSync), null === (s = this._yWebsocketProvider) || void 0 === s || s.destroy(), a.Signal.clearData(this))
                 }
-                _connect() {
-                    (async function(e, t, s) {
-                        const {
-                            makeSettings: o,
-                            makeRequest: i,
-                            ResponseError: a
-                        } = n.ServerConnection, c = o(), h = r.URLExt.join(c.baseUrl, "api/collaboration/session", encodeURIComponent(s)), d = {
-                            method: "PUT",
-                            body: JSON.stringify({
-                                format: e,
-                                type: t
-                            })
-                        }, l = await i(h, d, c);
-                        if (200 !== l.status && 201 !== l.status) throw new a(l);
-                        return l.json()
-                    })(this._format, this._contentType, this._path).then((e => {
-                        this._yWebsocketProvider = new c.WebsocketProvider(this._serverUrl, `${e.format}:${e.type}:${e.fileId}`, this._sharedModel.ydoc, {
-                            disableBc: !0,
-                            params: {
-                                sessionId: e.sessionId
-                            },
-                            awareness: this._awareness
-                        }), this._yWebsocketProvider.on("connection-close", this._onConnectionClosed)
-                    })).then((e => this._ready.resolve())).catch((e => console.warn(e)))
+                async _connect() {
+                    const e = await async function(e, t, s) {
+                        const n = r.ServerConnection.makeSettings(),
+                            i = o.URLExt.join(n.baseUrl, "api/collaboration/session", encodeURIComponent(s)),
+                            a = {
+                                method: "PUT",
+                                body: JSON.stringify({
+                                    format: e,
+                                    type: t
+                                })
+                            };
+                        let c;
+                        try {
+                            c = await r.ServerConnection.makeRequest(i, a, n)
+                        } catch (e) {
+                            throw new r.ServerConnection.NetworkError(e)
+                        }
+                        let h = await c.text();
+                        if (h.length > 0) try {
+                            h = JSON.parse(h)
+                        } catch (e) {
+                            console.log("Not a JSON response body.", c)
+                        }
+                        if (!c.ok) throw new r.ServerConnection.ResponseError(c, h.message || h);
+                        return h
+                    }(this._format, this._contentType, this._path);
+                    this._yWebsocketProvider = new c.WebsocketProvider(this._serverUrl, `${e.format}:${e.type}:${e.fileId}`, this._sharedModel.ydoc, {
+                        disableBc: !0,
+                        params: {
+                            sessionId: e.sessionId
+                        },
+                        awareness: this._awareness
+                    }), this._yWebsocketProvider.on("sync", this._onSync), this._yWebsocketProvider.on("connection-close", this._onConnectionClosed)
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            class d extends n.Drive {
+            class d extends r.Drive {
                 constructor(e, t) {
                     super({
                         name: "RTC"
                     }), this._onCreate = (e, t) => {
                         if ("string" == typeof e.format) try {
                             const s = new h({
-                                    url: r.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
+                                    url: o.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
                                     path: e.path,
                                     format: e.format,
                                     contentType: e.contentType,
                                     model: t,
                                     user: this._user,
                                     translator: this._trans
                                 }),
-                                n = `${e.format}:${e.contentType}:${e.path}`;
-                            this._providers.set(n, s), t.disposed.connect((() => {
-                                const e = this._providers.get(n);
-                                e && (e.dispose(), this._providers.delete(n))
-                            }));
-                            for (const t of this._providers.keys()) {
-                                if (t === n) continue;
-                                const s = t.split(":")[2];
-                                e.path === s && (0, o.showDialog)({
-                                    title: this._trans.__("Warning"),
-                                    body: this._trans.__("Opening a document with multiple views simultaneously is not supported.Please, close one view otherwise, you might lose some of your changes."),
-                                    buttons: [o.Dialog.okButton()]
-                                })
-                            }
+                                r = `${e.format}:${e.contentType}:${e.path}`;
+                            this._providers.set(r, s), t.disposed.connect((() => {
+                                const e = this._providers.get(r);
+                                e && (e.dispose(), this._providers.delete(r))
+                            }))
                         } catch (t) {
                             console.error(`Failed to open websocket connection for ${e.path}.\n:${t}`)
                         }
                     }, this._user = e, this._trans = t, this._providers = new Map, this.sharedModelFactory = new l(this._onCreate)
                 }
                 dispose() {
                     this.isDisposed || (this._providers.forEach((e => e.dispose())), this._providers.clear(), super.dispose())
@@ -141,11 +140,11 @@
                         if (e.collaborative && this._documentFactories.has(e.contentType)) {
                             const t = this._documentFactories.get(e.contentType)(e);
                             return this._onCreate(e, t), t
                         }
                     } else console.warn(`Only defined format are supported; got ${e.format}.`)
                 }
             }
-            const p = new i.Token("@jupyter/collaboration-extension:ICollaborativeDrive")
+            const _ = new i.Token("@jupyter/collaboration-extension:ICollaborativeDrive")
         }
     }
 ]);
```

### Comparing `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/remoteEntry.c7ae49e75d2022d8409a.js` & `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/remoteEntry.f78dd7195bd101ba931a.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, l, u, d, f, s, c, p, b, h, v, y, m, g = {
-            9704: (e, r, t) => {
+    var e, r, t, a, o, n, l, i, u, d, f, s, c, p, b, h, v, y, m, g, j = {
+            6746: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(493), t.e(726), t.e(981), t.e(260), t.e(801), t.e(497)]).then((() => () => t(9497))),
-                        "./extension": () => Promise.all([t.e(493), t.e(726), t.e(981), t.e(260), t.e(801), t.e(497)]).then((() => () => t(9497))),
+                        "./index": () => Promise.all([t.e(493), t.e(619), t.e(981), t.e(296), t.e(744), t.e(87)]).then((() => () => t(5087))),
+                        "./extension": () => Promise.all([t.e(493), t.e(619), t.e(981), t.e(296), t.e(744), t.e(87)]).then((() => () => t(5087))),
                         "./style": () => t.e(839).then((() => () => t(8839)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
@@ -21,309 +21,315 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => n
                 })
             }
         },
-        j = {};
+        w = {};
 
-    function w(e) {
-        var r = j[e];
+    function P(e) {
+        var r = w[e];
         if (void 0 !== r) return r.exports;
-        var t = j[e] = {
+        var t = w[e] = {
             id: e,
             exports: {}
         };
-        return g[e](t, t.exports, w), t.exports
+        return j[e](t, t.exports, P), t.exports
     }
-    w.m = g, w.c = j, w.n = e => {
+    P.m = j, P.c = w, P.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return w.d(r, {
+        return P.d(r, {
             a: r
         }), r
-    }, w.d = (e, r) => {
-        for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
+    }, P.d = (e, r) => {
+        for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        8: "6b2a09634af3599cbddb",
-        9: "f46ff2dd7fa86c1246e8",
-        260: "55fece40a4703413e008",
+    }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
+        8: "883cdb5327aeb22e2587",
+        87: "c69c6c0210f40538f288",
+        296: "66b569f73a5e447ea765",
         413: "cf154c48ecaa08648e56",
-        493: "0975334cbddac1bcf819",
-        497: "ab1a0ee570b8e4f31289",
-        726: "dcde0771b563d36178d7",
-        801: "1ce5dfec9291e64bf68b",
-        839: "2efa17f8ec8b5c6c87a6",
-        901: "f3045e1e297ffd031efd",
-        930: "0236d410b0d873232513",
-        933: "f161fc3dcf0d2c141b27",
-        981: "9470c3f446e34a475ff7"
+        493: "efdf15c07c2318ee4cd7",
+        619: "3ea832ff8016a41a4d10",
+        744: "8d88ecfc016bf00dba1c",
+        760: "c3c71c52d5e0ace455c5",
+        839: "14d748171b9c87a422f9",
+        901: "a771e814402df392d806",
+        930: "50b2067c71cf2a3ca014",
+        933: "737bcc7ac7d9a6826f35",
+        981: "9b18765371d0668dbc59"
     } [e] + ".js?v=" + {
-        8: "6b2a09634af3599cbddb",
-        9: "f46ff2dd7fa86c1246e8",
-        260: "55fece40a4703413e008",
+        8: "883cdb5327aeb22e2587",
+        87: "c69c6c0210f40538f288",
+        296: "66b569f73a5e447ea765",
         413: "cf154c48ecaa08648e56",
-        493: "0975334cbddac1bcf819",
-        497: "ab1a0ee570b8e4f31289",
-        726: "dcde0771b563d36178d7",
-        801: "1ce5dfec9291e64bf68b",
-        839: "2efa17f8ec8b5c6c87a6",
-        901: "f3045e1e297ffd031efd",
-        930: "0236d410b0d873232513",
-        933: "f161fc3dcf0d2c141b27",
-        981: "9470c3f446e34a475ff7"
-    } [e], w.g = function() {
+        493: "efdf15c07c2318ee4cd7",
+        619: "3ea832ff8016a41a4d10",
+        744: "8d88ecfc016bf00dba1c",
+        760: "c3c71c52d5e0ace455c5",
+        839: "14d748171b9c87a422f9",
+        901: "a771e814402df392d806",
+        930: "50b2067c71cf2a3ca014",
+        933: "737bcc7ac7d9a6826f35",
+        981: "9b18765371d0668dbc59"
+    } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter/collaboration-extension:", w.l = (t, a, o, n) => {
+    }(), P.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter/collaboration-extension:", P.l = (t, a, o, n) => {
         if (e[t]) e[t].push(a);
         else {
-            var i, l;
+            var l, i;
             if (void 0 !== o)
                 for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
                     var f = u[d];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                        l = f;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [a];
+            l || (i = !0, (l = document.createElement("script")).charset = "utf-8", l.timeout = 120, P.nc && l.setAttribute("nonce", P.nc), l.setAttribute("data-webpack", r + o), l.src = t), e[t] = [a];
             var s = (r, a) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+                    l.onerror = l.onload = null, clearTimeout(c);
                     var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
+                    if (delete e[t], l.parentNode && l.parentNode.removeChild(l), o && o.forEach((e => e(a))), r) return r(a)
                 },
                 c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
-                    target: i
+                    target: l
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
+            l.onerror = s.bind(null, l.onerror), l.onload = s.bind(null, l.onload), i && document.head.appendChild(l)
         }
-    }, w.r = e => {
+    }, P.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        w.S = {};
+        P.S = {};
         var e = {},
             r = {};
-        w.I = (t, a) => {
+        P.I = (t, a) => {
             a || (a = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(a.indexOf(o) >= 0)) {
                 if (a.push(o), e[t]) return e[t];
-                w.o(w.S, t) || (w.S[t] = {});
-                var n = w.S[t],
-                    i = "@jupyter/collaboration-extension",
-                    l = (e, r, t, a) => {
+                P.o(P.S, t) || (P.S[t] = {});
+                var n = P.S[t],
+                    l = "@jupyter/collaboration-extension",
+                    i = (e, r, t, a) => {
                         var o = n[e] = n[e] || {},
-                            l = o[r];
-                        (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
+                            i = o[r];
+                        (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (o[r] = {
                             get: t,
-                            from: i,
+                            from: l,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyter/collaboration-extension", "1.0.0-alpha.8", (() => Promise.all([w.e(493), w.e(726), w.e(981), w.e(260), w.e(801), w.e(497)]).then((() => () => w(9497))))), l("@jupyter/collaboration", "1.0.0-alpha.8", (() => Promise.all([w.e(930), w.e(726), w.e(981), w.e(9), w.e(260)]).then((() => () => w(6009))))), l("@jupyter/docprovider", "1.0.0-alpha.8", (() => Promise.all([w.e(930), w.e(726), w.e(801), w.e(901), w.e(8)]).then((() => () => w(2008))))), l("y-websocket", "1.5.0", (() => Promise.all([w.e(493), w.e(413), w.e(981)]).then((() => () => w(413)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@jupyter/collaboration-extension", "1.0.0-alpha.9", (() => Promise.all([P.e(493), P.e(619), P.e(981), P.e(296), P.e(744), P.e(87)]).then((() => () => P(5087))))), i("@jupyter/collaboration", "1.0.0-alpha.9", (() => Promise.all([P.e(930), P.e(619), P.e(981), P.e(760), P.e(296)]).then((() => () => P(4760))))), i("@jupyter/docprovider", "1.0.0-alpha.9", (() => Promise.all([P.e(930), P.e(619), P.e(744), P.e(901), P.e(8)]).then((() => () => P(2008))))), i("y-websocket", "1.5.0", (() => Promise.all([P.e(493), P.e(413), P.e(981)]).then((() => () => P(413)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        w.g.importScripts && (e = w.g.location + "");
-        var r = w.g.document;
+        P.g.importScripts && (e = P.g.location + "");
+        var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var a = t.length - 1; a > -1 && !e;) e = t[a--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), w.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), P.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             a = t[1] ? r(t[1]) : [];
         return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
     }, a = (e, r) => {
         e = t(e), r = t(r);
         for (var a = 0;;) {
             if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
             var o = e[a],
                 n = (typeof o)[0];
             if (a >= r.length) return "u" == n;
-            var i = r[a],
-                l = (typeof i)[0];
-            if (n != l) return "o" == n && "n" == l || "s" == l || "u" == n;
-            if ("o" != n && "u" != n && o != i) return o < i;
+            var l = r[a],
+                i = (typeof l)[0];
+            if (n != i) return "o" == n && "n" == i || "s" == i || "u" == n;
+            if ("o" != n && "u" != n && o != l) return o < l;
             a++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(l = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
+            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(i = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, i);
             return t
         }
-        var i = [];
+        var l = [];
         for (n = 1; n < e.length; n++) {
-            var l = e[n];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
+            var i = e[n];
+            l.push(0 === i ? "not(" + u() + ")" : 1 === i ? "(" + u() + " || " + u() + ")" : 2 === i ? l.pop() + " " + l.pop() : o(i))
         }
         return u();
 
         function u() {
-            return i.pop().replace(/^\((.+)\)$/, "$1")
+            return l.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 o = a < 0;
             o && (a = -a - 1);
-            for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var d, f, s = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !u || ("u" == s ? l > a && !o : "" == s != o);
+            for (var l = 0, i = 1, u = !0;; i++, l++) {
+                var d, f, s = i < e.length ? (typeof e[i])[0] : "";
+                if (l >= r.length || "o" == (f = (typeof(d = r[l]))[0])) return !u || ("u" == s ? i > a && !o : "" == s != o);
                 if ("u" == f) {
                     if (!u || "u" != s) return !1
                 } else if (u)
                     if (s == f)
-                        if (l <= a) {
-                            if (d != e[l]) return !1
+                        if (i <= a) {
+                            if (d != e[i]) return !1
                         } else {
-                            if (o ? d > e[l] : d < e[l]) return !1;
-                            d != e[l] && (u = !1)
+                            if (o ? d > e[i] : d < e[i]) return !1;
+                            d != e[i] && (u = !1)
                         }
                 else if ("s" != s && "n" != s) {
-                    if (o || l <= a) return !1;
-                    u = !1, l--
+                    if (o || i <= a) return !1;
+                    u = !1, i--
                 } else {
-                    if (l <= a || f < s != o) return !1;
+                    if (i <= a || f < s != o) return !1;
                     u = !1
-                } else "s" != s && "n" != s && (u = !1, l--)
+                } else "s" != s && "n" != s && (u = !1, i--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
-        for (i = 1; i < e.length; i++) {
-            var b = e[i];
+        for (l = 1; l < e.length; l++) {
+            var b = e[l];
             c.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? n(b, r) : !p())
         }
         return !!p()
-    }, i = (e, r) => {
-        var t = w.S[e];
-        if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
-        return t
     }, l = (e, r) => {
+        var t = P.S[e];
+        if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        return t
+    }, i = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", d = (e, r, t, a) => {
-        var o = l(e, t);
-        return n(a, o) || "undefined" != typeof console && console.warn && console.warn(u(e, t, o, a)), s(e[t][o])
+        var o = i(e, t);
+        return n(a, o) || s(u(e, t, o, a)), c(e[t][o])
     }, f = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !n(t, r) || e && !a(e, r) ? e : r), 0)) && o[r]
-    }, s = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, a, o) {
-        var n = w.I(r);
-        return n && n.then ? n.then(e.bind(e, r, w.S[r], t, a, o)) : e(r, w.S[r], t, a, o)
-    })(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), b = c(((e, r, t, a, o) => r && w.o(r, t) ? d(r, 0, t, a) : o())), h = c(((e, r, t, a, o) => {
-        var n = r && w.o(r, t) && f(r, t, a);
-        return n ? s(n) : o()
-    })), v = {}, y = {
-        60: () => p("default", "@jupyterlab/apputils", [1, 4, 0, 0, , "beta", 1]),
-        4989: () => p("default", "@jupyterlab/coreutils", [1, 6, 0, 0, , "beta", 1]),
-        981: () => p("default", "yjs", [1, 13, 5, 40]),
-        8778: () => p("default", "@lumino/widgets", [1, 2, 0, 1]),
-        9190: () => p("default", "@jupyterlab/ui-components", [1, 4, 0, 0, , "beta", 1]),
-        7099: () => h("default", "y-websocket", [1, 1, 3, 15], (() => Promise.all([w.e(493), w.e(413), w.e(981)]).then((() => () => w(413))))),
-        8256: () => p("default", "@jupyterlab/services", [1, 7, 0, 0, , "beta", 1]),
-        726: () => p("default", "@jupyterlab/translation", [1, 4, 0, 0, , "beta", 1]),
-        1371: () => p("default", "@jupyterlab/filebrowser", [1, 4, 0, 0, , "beta", 1]),
-        1682: () => p("default", "@jupyterlab/statedb", [1, 4, 0, 0, , "beta", 1]),
-        2281: () => p("default", "@jupyterlab/application", [1, 4, 0, 0, , "beta", 1]),
-        3e3: () => p("default", "@jupyter/ydoc", [2, 0, 3, 4]),
-        5581: () => p("default", "@jupyterlab/settingregistry", [1, 4, 0, 0, , "beta", 1]),
-        5996: () => b("default", "@jupyter/docprovider", [1, 1, 0, 0, , "alpha", 8], (() => Promise.all([w.e(930), w.e(901), w.e(933)]).then((() => () => w(2008))))),
-        7478: () => p("default", "@jupyterlab/codemirror", [1, 4, 0, 0, , "beta", 1]),
-        9041: () => b("default", "@jupyter/collaboration", [1, 1, 0, 0, , "alpha", 8], (() => Promise.all([w.e(930), w.e(9)]).then((() => () => w(6009))))),
-        7930: () => p("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        4059: () => p("default", "@lumino/virtualdom", [1, 2, 0, 0]),
-        6029: () => p("default", "react", [1, 18, 2, 0]),
-        8204: () => p("default", "@codemirror/state", [1, 6, 2, 0]),
-        9502: () => p("default", "@codemirror/view", [1, 6, 7, 0]),
-        4901: () => p("default", "@lumino/signaling", [1, 2, 0, 0])
-    }, m = {
-        9: [4059, 6029, 8204, 9502],
-        260: [8778, 9190],
-        497: [726, 1371, 1682, 2281, 3e3, 5581, 5996, 7478, 9041],
-        726: [60, 4989],
-        801: [7099, 8256],
+    }, s = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, c = e => (e.loaded = 1, e.get()), b = (p = e => function(r, t, a, o) {
+        var n = P.I(r);
+        return n && n.then ? n.then(e.bind(e, r, P.S[r], t, a, o)) : e(r, P.S[r], t, a, o)
+    })(((e, r, t, a) => (l(e, t), d(r, 0, t, a)))), h = p(((e, r, t, a, o) => r && P.o(r, t) ? d(r, 0, t, a) : o())), v = p(((e, r, t, a, o) => {
+        var n = r && P.o(r, t) && f(r, t, a);
+        return n ? c(n) : o()
+    })), y = {}, m = {
+        9324: () => b("default", "@jupyterlab/apputils", [1, 4, 1, 1]),
+        9474: () => b("default", "@jupyterlab/coreutils", [1, 6, 0, 1]),
+        981: () => b("default", "yjs", [1, 13, 5, 40]),
+        3897: () => b("default", "@jupyterlab/ui-components", [1, 4, 0, 1]),
+        7387: () => b("default", "@jupyterlab/translation", [1, 4, 0, 1]),
+        8778: () => b("default", "@lumino/widgets", [1, 2, 0, 1]),
+        3020: () => b("default", "@jupyterlab/services", [1, 7, 0, 1]),
+        7099: () => v("default", "y-websocket", [1, 1, 3, 15], (() => Promise.all([P.e(493), P.e(413), P.e(981)]).then((() => () => P(413))))),
+        94: () => b("default", "@jupyterlab/settingregistry", [1, 4, 0, 1]),
+        674: () => b("default", "@jupyterlab/codemirror", [1, 4, 0, 1]),
+        899: () => b("default", "@jupyterlab/notebook", [1, 4, 0, 1]),
+        1039: () => h("default", "@jupyter/docprovider", [1, 1, 0, 0, , "alpha", 9], (() => Promise.all([P.e(930), P.e(901), P.e(933)]).then((() => () => P(2008))))),
+        1802: () => b("default", "@jupyterlab/statedb", [1, 4, 0, 1]),
+        2177: () => b("default", "@jupyterlab/application", [1, 4, 0, 1]),
+        2293: () => b("default", "@jupyter/ydoc", [1, 1, 0, 2]),
+        2497: () => b("default", "@jupyterlab/fileeditor", [1, 4, 0, 1]),
+        5116: () => b("default", "@jupyterlab/logconsole", [1, 4, 0, 1]),
+        5355: () => b("default", "@jupyterlab/filebrowser", [1, 4, 0, 1]),
+        6903: () => h("default", "@jupyter/collaboration", [1, 1, 0, 0, , "alpha", 9], (() => Promise.all([P.e(930), P.e(760)]).then((() => () => P(4760))))),
+        7930: () => b("default", "@lumino/coreutils", [1, 2, 0, 0]),
+        4059: () => b("default", "@lumino/virtualdom", [1, 2, 0, 0]),
+        6029: () => b("default", "react", [1, 18, 2, 0]),
+        6211: () => b("default", "@codemirror/view", [1, 6, 9, 6]),
+        8204: () => b("default", "@codemirror/state", [1, 6, 2, 0]),
+        4901: () => b("default", "@lumino/signaling", [1, 2, 0, 0])
+    }, g = {
+        87: [94, 674, 899, 1039, 1802, 2177, 2293, 2497, 5116, 5355, 6903],
+        296: [3897, 7387, 8778],
+        619: [9324, 9474],
+        744: [3020, 7099],
+        760: [4059, 6029, 6211, 8204],
         901: [4901],
         930: [7930],
         981: [981]
-    }, w.f.consumes = (e, r) => {
-        w.o(m, e) && m[e].forEach((e => {
-            if (w.o(v, e)) return r.push(v[e]);
+    }, P.f.consumes = (e, r) => {
+        P.o(g, e) && g[e].forEach((e => {
+            if (P.o(y, e)) return r.push(y[e]);
             var t = r => {
-                    v[e] = 0, w.m[e] = t => {
-                        delete w.c[e], t.exports = r()
+                    y[e] = 0, P.m[e] = t => {
+                        delete P.c[e], t.exports = r()
                     }
                 },
                 a = r => {
-                    delete v[e], w.m[e] = t => {
-                        throw delete w.c[e], r
+                    delete y[e], P.m[e] = t => {
+                        throw delete P.c[e], r
                     }
                 };
             try {
-                var o = y[e]();
-                o.then ? r.push(v[e] = o.then(t).catch(a)) : t(o)
+                var o = m[e]();
+                o.then ? r.push(y[e] = o.then(t).catch(a)) : t(o)
             } catch (e) {
                 a(e)
             }
         }))
     }, (() => {
         var e = {
             510: 0
         };
-        w.f.j = (r, t) => {
-            var a = w.o(e, r) ? e[r] : void 0;
+        P.f.j = (r, t) => {
+            var a = P.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(9(01|30|81)|260|726|801)$/.test(r)) e[r] = 0;
+                else if (/^(9(01|30|81)|296|619|744)$/.test(r)) e[r] = 0;
             else {
                 var o = new Promise(((t, o) => a = e[r] = [t, o]));
                 t.push(a[2] = o);
-                var n = w.p + w.u(r),
-                    i = new Error;
-                w.l(n, (t => {
-                    if (w.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
+                var n = P.p + P.u(r),
+                    l = new Error;
+                P.l(n, (t => {
+                    if (P.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
                         var o = t && ("load" === t.type ? "missing" : t.type),
                             n = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", i.name = "ChunkLoadError", i.type = o, i.request = n, a[1](i)
+                        l.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", l.name = "ChunkLoadError", l.type = o, l.request = n, a[1](l)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var a, o, [n, i, l] = t,
+                var a, o, [n, l, i] = t,
                     u = 0;
                 if (n.some((r => 0 !== e[r]))) {
-                    for (a in i) w.o(i, a) && (w.m[a] = i[a]);
-                    l && l(w)
+                    for (a in l) P.o(l, a) && (P.m[a] = l[a]);
+                    i && i(P)
                 }
-                for (r && r(t); u < n.length; u++) o = n[u], w.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); u < n.length; u++) o = n[u], P.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), w.nc = void 0;
-    var P = w(9704);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter/collaboration-extension"] = P
+    })(), P.nc = void 0;
+    var S = P(6746);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter/collaboration-extension"] = S
 })();
```

### Comparing `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/third-party-licenses.json` & `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9765625%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '1.0.0-alpha.9'}, 1: {'versionInfo': '1.0.0-alpha.9'}, 3: "*

 * *               "{'versionInfo': '0.2.74'}}"}*

```diff
@@ -1,32 +1,32 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/collaboration",
-            "versionInfo": "1.0.0-alpha.8"
+            "versionInfo": "1.0.0-alpha.9"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/docprovider",
-            "versionInfo": "1.0.0-alpha.8"
+            "versionInfo": "1.0.0-alpha.9"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "6.7.3"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2019 Kevin Jahns <kevin.jahns@protonmail.com>.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "lib0",
-            "versionInfo": "0.2.73"
+            "versionInfo": "0.2.74"
         },
         {
             "extractedText": "(The MIT License)\n\nCopyright (c) 2013 Roman Shtylman <shtylman@gmail.com>\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "process",
             "versionInfo": "0.11.10"
         },
```

### Comparing `jupyter_collaboration-1.0.0a8/scripts/bump_version.py` & `jupyter_collaboration-1.0.0a9/scripts/bump_version.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/packages/collaboration/package.json` & `jupyter_collaboration-1.0.0a9/packages/collaboration/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9645833333333333%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/apputils': '^4.0.0', '@jupyterlab/coreutils': '^6.0.0', "*

 * *                   "'@jupyterlab/services': '^7.0.0', '@jupyterlab/ui-components': '^4.0.0', "*

 * *                   "'@lumino/coreutils': '^2.1.0', '@lumino/widgets': '^2.1.0'}",*

 * * "'devDependencies'": "{'typescript': '~5.0.4'}",*

 * * "'version'": "'1.0.0-alpha.9'"}*

```diff
@@ -2,30 +2,30 @@
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
         "@codemirror/state": "^6.2.0",
         "@codemirror/view": "^6.7.0",
-        "@jupyterlab/apputils": "^4.0.0-beta.0",
-        "@jupyterlab/coreutils": "^6.0.0-beta.0",
-        "@jupyterlab/services": "^7.0.0-beta.0",
-        "@jupyterlab/ui-components": "^4.0.0-beta.0",
-        "@lumino/coreutils": "^2.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/ui-components": "^4.0.0",
+        "@lumino/coreutils": "^2.1.0",
         "@lumino/virtualdom": "^2.0.0",
-        "@lumino/widgets": "^2.0.0",
+        "@lumino/widgets": "^2.1.0",
         "react": "^18.2.0",
         "y-protocols": "^1.0.5",
         "yjs": "^13.5.40"
     },
     "description": "JupyterLab - Real-Time Collaboration Widgets",
     "devDependencies": {
         "@types/react": "^18.0.27",
         "rimraf": "^4.1.2",
-        "typescript": "~5.0.2"
+        "typescript": "~5.0.4"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
         "lib/*.d.ts",
         "lib/*.js.map",
@@ -62,9 +62,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.8"
+    "version": "1.0.0-alpha.9"
 }
```

### Comparing `jupyter_collaboration-1.0.0a8/packages/collaboration/src/collaboratorspanel.tsx` & `jupyter_collaboration-1.0.0a9/packages/collaboration/src/collaboratorspanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/packages/collaboration/src/components.tsx` & `jupyter_collaboration-1.0.0a9/packages/collaboration/src/components.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/packages/collaboration/src/cursors.ts` & `jupyter_collaboration-1.0.0a9/packages/collaboration/src/cursors.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/packages/collaboration/src/menu.ts` & `jupyter_collaboration-1.0.0a9/packages/collaboration/src/menu.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/packages/collaboration/src/tokens.ts` & `jupyter_collaboration-1.0.0a9/packages/collaboration/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/packages/collaboration/src/userinfopanel.tsx` & `jupyter_collaboration-1.0.0a9/packages/collaboration/src/userinfopanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/packages/collaboration/style/menu.css` & `jupyter_collaboration-1.0.0a9/packages/collaboration/style/menu.css`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/packages/collaboration/style/sidepanel.css` & `jupyter_collaboration-1.0.0a9/packages/collaboration/style/sidepanel.css`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/packages/collaboration-extension/package.json` & `jupyter_collaboration-1.0.0a9/packages/collaboration-extension/package.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9585497835497836%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^1.0.0-alpha.9', '@jupyter/docprovider': "*

 * *                   "'^1.0.0-alpha.9', '@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': "*

 * *                   "'^4.0.0', '@jupyterlab/codemirror': '^4.0.0', '@jupyterlab/coreutils': "*

 * *                   "'^6.0.0', '@jupyterlab/filebrowser': '^4.0.0', '@jupyterlab/services': "*

 * *                   "'^7.0.0', '@jupyterlab/settingregistry': '^4.0.0', '@jupyterlab/statedb': "*

 * *                   "'^4.0.0', '@jupyte […]*

```diff
@@ -1,38 +1,42 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^1.0.0-alpha.8",
-        "@jupyter/docprovider": "^1.0.0-alpha.8",
-        "@jupyterlab/application": "^4.0.0-beta.0",
-        "@jupyterlab/apputils": "^4.0.0-beta.0",
-        "@jupyterlab/codemirror": "^4.0.0-beta.0",
-        "@jupyterlab/coreutils": "^6.0.0-beta.0",
-        "@jupyterlab/filebrowser": "^4.0.0-beta.0",
-        "@jupyterlab/services": "^7.0.0-beta.0",
-        "@jupyterlab/settingregistry": "^4.0.0-beta.0",
-        "@jupyterlab/statedb": "^4.0.0-beta.0",
-        "@jupyterlab/translation": "^4.0.0-beta.0",
-        "@jupyterlab/ui-components": "^4.0.0-beta.0",
-        "@lumino/commands": "^2.0.0",
-        "@lumino/widgets": "^2.0.0",
+        "@jupyter/collaboration": "^1.0.0-alpha.9",
+        "@jupyter/docprovider": "^1.0.0-alpha.9",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/codemirror": "^4.0.0",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/docregistry": "^4.0.0",
+        "@jupyterlab/filebrowser": "^4.0.0",
+        "@jupyterlab/fileeditor": "^4.0.0",
+        "@jupyterlab/logconsole": "^4.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0",
+        "@jupyterlab/statedb": "^4.0.0",
+        "@jupyterlab/translation": "^4.0.0",
+        "@jupyterlab/ui-components": "^4.0.0",
+        "@lumino/commands": "^2.1.0",
+        "@lumino/widgets": "^2.1.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
         "yjs": "^13.5.40"
     },
     "description": "JupyterLab - Real-Time Collaboration Extension",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.0.0-beta.0",
-        "@types/react": "^18.0.27",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/react": "~18.0.26",
         "npm-run-all": "^4.1.5",
         "rimraf": "^4.1.2",
-        "typescript": "~5.0.2"
+        "typescript": "~5.0.4"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
         "lib/*.d.ts",
         "lib/*.js.map",
@@ -120,9 +124,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.8"
+    "version": "1.0.0-alpha.9"
 }
```

### Comparing `jupyter_collaboration-1.0.0a8/packages/collaboration-extension/src/collaboration.ts` & `jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/collaboration.ts`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
  * @module collaboration-extension
  */
 
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
-import { DOMUtils } from '@jupyterlab/apputils';
+import { DOMUtils, IToolbarWidgetRegistry } from '@jupyterlab/apputils';
 import {
   EditorExtensionRegistry,
   IEditorExtensionRegistry
 } from '@jupyterlab/codemirror';
 import {
   CollaboratorsPanel,
   IAwareness,
@@ -50,33 +50,37 @@
   }
 };
 
 /**
  * Jupyter plugin adding the IUserMenu to the menu bar if collaborative flag enabled.
  */
 export const menuBarPlugin: JupyterFrontEndPlugin<void> = {
-  id: '@jupyter/collaboration-extension:userMenuBar',
+  id: '@jupyter/collaboration-extension:user-menu-bar',
   description: 'Add user menu to the interface.',
   autoStart: true,
-  requires: [IUserMenu],
-  activate: async (app: JupyterFrontEnd, menu: IUserMenu): Promise<void> => {
-    const { shell } = app;
+  requires: [IUserMenu, IToolbarWidgetRegistry],
+  activate: async (
+    app: JupyterFrontEnd,
+    menu: IUserMenu,
+    toolbarRegistry: IToolbarWidgetRegistry
+  ): Promise<void> => {
     const { user } = app.serviceManager;
 
     const menuBar = new MenuBar({
       forceItemsPosition: {
         forceX: false,
         forceY: false
       },
       renderer: new RendererUserMenu(user)
     });
     menuBar.id = 'jp-UserMenu';
     user.userChanged.connect(() => menuBar.update());
     menuBar.addMenu(menu as Menu);
-    shell.add(menuBar, 'top', { rank: 1000 });
+
+    toolbarRegistry.addFactory('TopBar', 'user-menu', () => menuBar);
   }
 };
 
 /**
  * Jupyter plugin creating a global awareness for RTC.
  */
 export const rtcGlobalAwarenessPlugin: JupyterFrontEndPlugin<IAwareness> = {
```

### Comparing `jupyter_collaboration-1.0.0a8/packages/collaboration-extension/src/index.ts` & `jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/index.ts`

 * *Files 18% similar despite different names*

```diff
@@ -3,32 +3,41 @@
 /**
  * @packageDocumentation
  * @module collaboration-extension
  */
 
 import { JupyterFrontEndPlugin } from '@jupyterlab/application';
 
-import { drive, yfile, ynotebook, defaultFileBrowser } from './filebrowser';
+import {
+  drive,
+  yfile,
+  ynotebook,
+  defaultFileBrowser,
+  logger
+} from './filebrowser';
 import {
   userMenuPlugin,
   menuBarPlugin,
   rtcGlobalAwarenessPlugin,
   rtcPanelPlugin,
   userEditorCursors
 } from './collaboration';
+import { sharedLink } from './sharedlink';
 
 /**
  * Export the plugins as default.
  */
 const plugins: JupyterFrontEndPlugin<any>[] = [
   drive,
   yfile,
   ynotebook,
   defaultFileBrowser,
+  logger,
   userMenuPlugin,
   menuBarPlugin,
   rtcGlobalAwarenessPlugin,
   rtcPanelPlugin,
+  sharedLink,
   userEditorCursors
 ];
 
 export default plugins;
```

### Comparing `jupyter_collaboration-1.0.0a8/packages/docprovider/package.json` & `jupyter_collaboration-1.0.0a9/packages/docprovider/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9518518518518518%*

 * *Differences: {"'dependencies'": "{'@jupyter/ydoc': '^1.0.2', '@jupyterlab/coreutils': '^6.0.0', "*

 * *                   "'@jupyterlab/services': '^7.0.0', '@lumino/coreutils': '^2.1.0', "*

 * *                   "'@lumino/disposable': '^2.1.0', '@lumino/signaling': '^2.1.0'}",*

 * * "'devDependencies'": "{'@jupyterlab/testing': '^4.0.0', 'typescript': '~5.0.4', 'jest': "*

 * *                      "'^29.5.0'}",*

 * * "'version'": "'1.0.0-alpha.9'"}*

```diff
@@ -1,29 +1,30 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/ydoc": "^1.0.0",
-        "@jupyterlab/coreutils": "^6.0.0-beta.0",
-        "@jupyterlab/services": "^7.0.0-beta.0",
-        "@lumino/coreutils": "^2.0.0",
-        "@lumino/disposable": "^2.0.0",
-        "@lumino/signaling": "^2.0.0",
+        "@jupyter/ydoc": "^1.0.2",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@lumino/coreutils": "^2.1.0",
+        "@lumino/disposable": "^2.1.0",
+        "@lumino/signaling": "^2.1.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
         "yjs": "^13.5.40"
     },
     "description": "JupyterLab - Document Provider",
     "devDependencies": {
-        "@jupyterlab/testing": "^4.0.0-beta.0",
+        "@jupyterlab/testing": "^4.0.0",
         "@types/jest": "^29.2.0",
+        "jest": "^29.5.0",
         "rimraf": "^4.1.2",
-        "typescript": "~5.0.2"
+        "typescript": "~5.0.4"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "schema/*.json",
@@ -60,9 +61,9 @@
     ],
     "typedoc": {
         "displayName": "@jupyter/docprovider",
         "entryPoint": "./src/index.ts",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.8"
+    "version": "1.0.0-alpha.9"
 }
```

### Comparing `jupyter_collaboration-1.0.0a8/packages/docprovider/src/requests.ts` & `jupyter_collaboration-1.0.0a9/packages/docprovider/src/requests.ts`

 * *Files 24% similar despite different names*

```diff
@@ -8,40 +8,68 @@
 
 /**
  * Document session endpoint provided by `jupyter_collaboration`
  * See https://github.com/jupyterlab/jupyter_collaboration
  */
 const DOC_SESSION_URL = 'api/collaboration/session';
 
+/**
+ * Document session model
+ */
 export interface ISessionModel {
+  /**
+   * Document format; 'text', 'base64',...
+   */
   format: Contents.FileFormat;
+  /**
+   * Document type
+   */
   type: Contents.ContentType;
+  /**
+   * File unique identifier
+   */
   fileId: string;
+  /**
+   * Server session identifier
+   */
   sessionId: string;
 }
 
 export async function requestDocSession(
   format: string,
   type: string,
   path: string
 ): Promise<ISessionModel> {
-  const { makeSettings, makeRequest, ResponseError } = ServerConnection;
-
-  const settings = makeSettings();
+  const settings = ServerConnection.makeSettings();
   const url = URLExt.join(
     settings.baseUrl,
     DOC_SESSION_URL,
     encodeURIComponent(path)
   );
-  const data = {
+  const body = {
     method: 'PUT',
     body: JSON.stringify({ format, type })
   };
 
-  const response = await makeRequest(url, data, settings);
+  let response: Response;
+  try {
+    response = await ServerConnection.makeRequest(url, body, settings);
+  } catch (error) {
+    throw new ServerConnection.NetworkError(error as Error);
+  }
+
+  let data: any = await response.text();
+
+  if (data.length > 0) {
+    try {
+      data = JSON.parse(data);
+    } catch (error) {
+      console.log('Not a JSON response body.', response);
+    }
+  }
 
-  if (response.status !== 200 && response.status !== 201) {
-    throw new ResponseError(response);
+  if (!response.ok) {
+    throw new ServerConnection.ResponseError(response, data.message || data);
   }
 
-  return response.json();
+  return data;
 }
```

### Comparing `jupyter_collaboration-1.0.0a8/packages/docprovider/src/tokens.ts` & `jupyter_collaboration-1.0.0a9/packages/docprovider/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/packages/docprovider/src/ydrive.ts` & `jupyter_collaboration-1.0.0a9/packages/docprovider/src/ydrive.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 // Copyright (c) Jupyter Development Team.
 // Distributed under the terms of the Modified BSD License.
 
-import { showDialog, Dialog } from '@jupyterlab/apputils';
 import { URLExt } from '@jupyterlab/coreutils';
 import { TranslationBundle } from '@jupyterlab/translation';
 import { Contents, Drive, User } from '@jupyterlab/services';
 
 import { DocumentChange, ISharedDocument, YDocument } from '@jupyter/ydoc';
 
 import { WebSocketProvider } from './yprovider';
@@ -137,31 +136,14 @@
       sharedModel.disposed.connect(() => {
         const provider = this._providers.get(key);
         if (provider) {
           provider.dispose();
           this._providers.delete(key);
         }
       });
-
-      for (const provider of this._providers.keys()) {
-        if (provider === key) {
-          continue;
-        }
-        const path = provider.split(':')[2];
-
-        if (options.path === path) {
-          showDialog({
-            title: this._trans.__('Warning'),
-            body: this._trans.__(
-              'Opening a document with multiple views simultaneously is not supported.Please, close one view otherwise, you might lose some of your changes.'
-            ),
-            buttons: [Dialog.okButton()]
-          });
-        }
-      }
     } catch (error) {
       // Falling back to the contents API if opening the websocket failed
       //  This may happen if the shared document is not a YDocument.
       console.error(
         `Failed to open websocket connection for ${options.path}.\n:${error}`
       );
     }
```

### Comparing `jupyter_collaboration-1.0.0a8/packages/docprovider/src/yprovider.ts` & `jupyter_collaboration-1.0.0a9/packages/docprovider/src/yprovider.ts`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import { Signal } from '@lumino/signaling';
 
 import { DocumentChange, YDocument } from '@jupyter/ydoc';
 
 import { Awareness } from 'y-protocols/awareness';
 import { WebsocketProvider as YWebsocketProvider } from 'y-websocket';
 
-import { ISessionModel, requestDocSession } from './requests';
+import { requestDocSession } from './requests';
 
 /**
  * An interface for a document provider.
  */
 export interface IDocumentProvider extends IDisposable {
   /**
    * Returns a Promise that resolves when the document provider is ready.
@@ -56,15 +56,15 @@
     user.ready
       .then(() => {
         this._onUserChanged(user);
       })
       .catch(e => console.error(e));
     user.userChanged.connect(this._onUserChanged, this);
 
-    this._connect();
+    this._connect().catch(e => console.warn(e));
   }
 
   /**
    * Test whether the object has been disposed.
    */
   get isDisposed(): boolean {
     return this._isDisposed;
@@ -82,69 +82,66 @@
    */
   dispose(): void {
     if (this.isDisposed) {
       return;
     }
     this._isDisposed = true;
     this._yWebsocketProvider?.off('connection-close', this._onConnectionClosed);
+    this._yWebsocketProvider?.off('sync', this._onSync);
     this._yWebsocketProvider?.destroy();
     Signal.clearData(this);
   }
 
-  private _connect(): void {
-    requestDocSession(this._format, this._contentType, this._path)
-      .then((session: ISessionModel) => {
-        this._yWebsocketProvider = new YWebsocketProvider(
-          this._serverUrl,
-          `${session.format}:${session.type}:${session.fileId}`,
-          this._sharedModel.ydoc,
-          {
-            disableBc: true,
-            params: { sessionId: session.sessionId },
-            awareness: this._awareness
-          }
-        );
-
-        this._yWebsocketProvider.on(
-          'connection-close',
-          this._onConnectionClosed
-        );
-      })
-      .then(r => this._ready.resolve())
-      .catch(e => console.warn(e));
+  private async _connect(): Promise<void> {
+    const session = await requestDocSession(
+      this._format,
+      this._contentType,
+      this._path
+    );
+
+    this._yWebsocketProvider = new YWebsocketProvider(
+      this._serverUrl,
+      `${session.format}:${session.type}:${session.fileId}`,
+      this._sharedModel.ydoc,
+      {
+        disableBc: true,
+        params: { sessionId: session.sessionId },
+        awareness: this._awareness
+      }
+    );
+
+    this._yWebsocketProvider.on('sync', this._onSync);
+    this._yWebsocketProvider.on('connection-close', this._onConnectionClosed);
   }
 
   private _onUserChanged(user: User.IManager): void {
     this._awareness.setLocalStateField('user', user.identity);
   }
 
   private _onConnectionClosed = (event: any): void => {
     if (event.code === 1003) {
       console.error('Document provider closed:', event.reason);
 
-      showErrorMessage(
-        this._trans.__('Session expired'),
-        this._trans.__(
-          'The document session expired. You need to reload this browser tab.'
-        ),
-        [Dialog.okButton({ label: this._trans.__('Reload') })]
-      )
-        .then((r: any) => {
-          if (r.button.accept) {
-            window.location.reload();
-          }
-        })
-        .catch(e => window.location.reload());
+      showErrorMessage(this._trans.__('Document session error'), event.reason, [
+        Dialog.okButton()
+      ]);
 
       // Dispose shared model immediately. Better break the document model,
       // than overriding data on disk.
       this._sharedModel.dispose();
     }
   };
 
+  private _onSync = (isSynced: boolean) => {
+    if (isSynced) {
+      this._ready.resolve();
+      this._yWebsocketProvider?.off('sync', this._onSync);
+    }
+  };
+
   private _awareness: Awareness;
   private _contentType: string;
   private _format: string;
   private _isDisposed: boolean;
   private _path: string;
   private _ready = new PromiseDelegate<void>();
   private _serverUrl: string;
```

### Comparing `jupyter_collaboration-1.0.0a8/.gitignore` & `jupyter_collaboration-1.0.0a9/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -128,7 +128,9 @@
 .pnp.*
 .yarn/*
 !.yarn/patches
 !.yarn/plugins
 !.yarn/releases
 !.yarn/sdks
 !.yarn/versions
+packages/docprovider/junit.xml
+.jupyter_ystore.db
```

### Comparing `jupyter_collaboration-1.0.0a8/LICENSE` & `jupyter_collaboration-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/README.md` & `jupyter_collaboration-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a8/pyproject.toml` & `jupyter_collaboration-1.0.0a9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+# Copyright (c) Jupyter Development Team.
+# Distributed under the terms of the Modified BSD License.
+
 [build-system]
 build-backend = "hatchling.build"
-requires = ["hatchling>=1.4.0", "hatch-nodejs-version", "jupyterlab>=4.0.0a32"]
+requires = ["hatchling>=1.4.0", "hatch-nodejs-version", "jupyterlab>=4.0.0"]
 
 [project]
 name = "jupyter_collaboration"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
@@ -23,14 +26,15 @@
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
 ]
 dependencies = [
     "jupyter_server>=2.0.0,<3.0.0",
     "jupyter_ydoc>=1.0.1,<2.0.0",
     "ypy-websocket>=0.8.3,<0.9.0",
+    "jupyter_events",
     "jupyter_server_fileid>=0.6.0,<1"
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
 dev = [
     "click",
@@ -38,17 +42,18 @@
     "jupyter_releaser"
 ]
 test = [
     "coverage",
     "jupyter_server[test]>=2.0.0",
     "pytest>=7.0",
     "pytest-cov",
+    "pytest-asyncio"
 ]
 docs = [
-    "jupyterlab>=4.0.0a32",
+    "jupyterlab>=4.0.0",
     "sphinx",
     "myst-parser",
     "pydata-sphinx-theme"
 ]
 
 [tool.black]
 line-length = 100
@@ -106,15 +111,15 @@
     "jlpm clean:all",
     # Build the assets
     "jlpm build:prod",
     # Clean the build artifacts to not include them in sdist
     "jlpm clean:lib"
 ]
 before-bump-version = [
-    "python -m pip install --pre -U jupyterlab",
+    "python -m pip install -U jupyterlab",
     "jlpm"
 ]
 
 [tool.check-wheel-contents]
 ignore = ["W002"]
 
 [tool.pytest.ini_options]
```

### Comparing `jupyter_collaboration-1.0.0a8/PKG-INFO` & `jupyter_collaboration-1.0.0a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_collaboration
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: JupyterLab Extension enabling Real-Time Collaboration
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter_collaboration
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter_collaboration/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter_collaboration.git
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: # Licensing terms
         
@@ -77,30 +77,32 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Requires-Dist: jupyter-events
 Requires-Dist: jupyter-server-fileid<1,>=0.6.0
 Requires-Dist: jupyter-server<3.0.0,>=2.0.0
 Requires-Dist: jupyter-ydoc<2.0.0,>=1.0.1
 Requires-Dist: ypy-websocket<0.9.0,>=0.8.3
 Provides-Extra: dev
 Requires-Dist: click; extra == 'dev'
 Requires-Dist: jupyter-releaser; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: jupyterlab>=4.0.0a32; extra == 'docs'
+Requires-Dist: jupyterlab>=4.0.0; extra == 'docs'
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: jupyter-server[test]>=2.0.0; extra == 'test'
+Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=7.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Jupyter Real-Time Collaboration
 
 [![Build Status](https://github.com/jupyterlab/jupyter_collaboration/actions/workflows/test.yml/badge.svg?query=branch%3Amain++)](https://github.com/jupyterlab/jupyter_collaboration/actions?query=branch%3Amain++)[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyterlab/jupyter_collaboration/main)[![PyPI](https://img.shields.io/pypi/v/jupyter-collaboration)](https://pypi.org/project/jupyter-collaboration)[![npm](https://img.shields.io/npm/v/@jupyter/collaboration-extension)](https://www.npmjs.com/package/@jupyter/collaboration-extension)
```

