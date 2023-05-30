# Comparing `tmp/titanoboa-0.1.6.tar.gz` & `tmp/titanoboa-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titanoboa-0.1.6.tar", last modified: Thu Sep 29 14:49:14 2022, max compression
+gzip compressed data, was "titanoboa-0.1.7.tar", last modified: Tue May 30 17:28:28 2023, max compression
```

## Comparing `titanoboa-0.1.6.tar` & `titanoboa-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,39 @@
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2022-09-29 14:49:14.233464 titanoboa-0.1.6/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1256 2022-06-27 13:46:21.000000 titanoboa-0.1.6/LICENSE
--rw-rw-r--   0 charles   (1000) charles   (1000)     7099 2022-09-29 14:49:14.233464 titanoboa-0.1.6/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)     5477 2022-09-02 15:29:30.000000 titanoboa-0.1.6/README.md
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2022-09-29 14:49:14.233464 titanoboa-0.1.6/boa/
--rw-rw-r--   0 charles   (1000) charles   (1000)      879 2022-08-30 17:03:53.000000 titanoboa-0.1.6/boa/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    27555 2022-09-13 20:46:07.000000 titanoboa-0.1.6/boa/contract.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    14643 2022-09-05 23:10:20.000000 titanoboa-0.1.6/boa/environment.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     1764 2022-08-19 17:30:16.000000 titanoboa-0.1.6/boa/interpret.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     1371 2022-08-30 15:39:11.000000 titanoboa-0.1.6/boa/ipython.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     4328 2022-08-28 19:04:05.000000 titanoboa-0.1.6/boa/profiling.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2022-09-29 14:49:14.233464 titanoboa-0.1.6/boa/util/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1991 2022-08-19 17:30:16.000000 titanoboa-0.1.6/boa/util/disk_cache.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      625 2022-08-19 17:30:16.000000 titanoboa-0.1.6/boa/util/exceptions.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      587 2022-08-29 07:36:46.000000 titanoboa-0.1.6/boa/util/lrudict.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2022-09-29 14:49:14.233464 titanoboa-0.1.6/boa/vm/
--rw-rw-r--   0 charles   (1000) charles   (1000)     7286 2022-09-13 20:45:38.000000 titanoboa-0.1.6/boa/vm/fork.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     1739 2022-08-27 18:28:07.000000 titanoboa-0.1.6/boa/vm/gas_meters.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2022-09-29 14:49:14.233464 titanoboa-0.1.6/boa/vyper/
--rw-rw-r--   0 charles   (1000) charles   (1000)        0 2022-08-19 17:30:16.000000 titanoboa-0.1.6/boa/vyper/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      975 2022-08-19 17:30:16.000000 titanoboa-0.1.6/boa/vyper/ast_utils.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     2508 2022-08-19 17:30:16.000000 titanoboa-0.1.6/boa/vyper/decoder_utils.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      810 2022-09-29 14:48:37.000000 titanoboa-0.1.6/pyproject.toml
--rw-rw-r--   0 charles   (1000) charles   (1000)      334 2022-09-29 14:49:14.233464 titanoboa-0.1.6/setup.cfg
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2022-09-29 14:49:14.233464 titanoboa-0.1.6/titanoboa.egg-info/
--rw-rw-r--   0 charles   (1000) charles   (1000)     7099 2022-09-29 14:49:14.000000 titanoboa-0.1.6/titanoboa.egg-info/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      480 2022-09-29 14:49:14.000000 titanoboa-0.1.6/titanoboa.egg-info/SOURCES.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        1 2022-09-29 14:49:14.000000 titanoboa-0.1.6/titanoboa.egg-info/dependency_links.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)       84 2022-09-29 14:49:14.000000 titanoboa-0.1.6/titanoboa.egg-info/requires.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        4 2022-09-29 14:49:14.000000 titanoboa-0.1.6/titanoboa.egg-info/top_level.txt
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-05-30 17:28:28.159511 titanoboa-0.1.7/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1256 2022-06-27 13:46:21.000000 titanoboa-0.1.7/LICENSE
+-rw-rw-r--   0 charles   (1000) charles   (1000)     8097 2023-05-30 17:28:28.159511 titanoboa-0.1.7/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)     6486 2023-05-06 18:55:35.000000 titanoboa-0.1.7/README.md
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-05-30 17:28:28.155511 titanoboa-0.1.7/boa/
+-rw-rw-r--   0 charles   (1000) charles   (1000)      988 2023-05-06 18:55:35.000000 titanoboa-0.1.7/boa/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      797 2023-05-06 18:55:35.000000 titanoboa-0.1.7/boa/debugger.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    16937 2023-05-25 13:18:18.000000 titanoboa-0.1.7/boa/environment.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2418 2023-05-25 12:06:43.000000 titanoboa-0.1.7/boa/interpret.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1371 2023-04-07 20:31:03.000000 titanoboa-0.1.7/boa/ipython.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3925 2023-05-23 15:05:38.000000 titanoboa-0.1.7/boa/precompile.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    13031 2023-05-23 15:05:38.000000 titanoboa-0.1.7/boa/profiling.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-05-30 17:28:28.159511 titanoboa-0.1.7/boa/test/
+-rw-rw-r--   0 charles   (1000) charles   (1000)       97 2023-05-06 18:55:35.000000 titanoboa-0.1.7/boa/test/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2493 2023-05-23 15:05:38.000000 titanoboa-0.1.7/boa/test/plugin.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     6965 2023-05-06 18:55:35.000000 titanoboa-0.1.7/boa/test/strategies.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-05-30 17:28:28.159511 titanoboa-0.1.7/boa/util/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2055 2023-05-06 18:55:35.000000 titanoboa-0.1.7/boa/util/disk_cache.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      625 2023-04-07 20:31:03.000000 titanoboa-0.1.7/boa/util/exceptions.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      587 2023-04-07 20:31:03.000000 titanoboa-0.1.7/boa/util/lrudict.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-05-30 17:28:28.159511 titanoboa-0.1.7/boa/vm/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     7323 2023-05-06 18:55:35.000000 titanoboa-0.1.7/boa/vm/fork.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1739 2023-04-07 20:31:03.000000 titanoboa-0.1.7/boa/vm/gas_meters.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-05-30 17:28:28.159511 titanoboa-0.1.7/boa/vyper/
+-rw-rw-r--   0 charles   (1000) charles   (1000)       79 2023-05-06 18:55:35.000000 titanoboa-0.1.7/boa/vyper/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2006 2023-05-23 15:05:38.000000 titanoboa-0.1.7/boa/vyper/ast_utils.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3882 2023-05-23 15:05:38.000000 titanoboa-0.1.7/boa/vyper/compiler_utils.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    33079 2023-05-25 13:18:18.000000 titanoboa-0.1.7/boa/vyper/contract.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2464 2023-05-06 18:55:35.000000 titanoboa-0.1.7/boa/vyper/decoder_utils.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      999 2023-05-06 18:55:35.000000 titanoboa-0.1.7/boa/vyper/event.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      948 2023-05-30 17:25:24.000000 titanoboa-0.1.7/pyproject.toml
+-rw-rw-r--   0 charles   (1000) charles   (1000)      398 2023-05-30 17:28:28.159511 titanoboa-0.1.7/setup.cfg
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-05-30 17:28:28.159511 titanoboa-0.1.7/titanoboa.egg-info/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     8097 2023-05-30 17:28:28.000000 titanoboa-0.1.7/titanoboa.egg-info/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)      666 2023-05-30 17:28:28.000000 titanoboa-0.1.7/titanoboa.egg-info/SOURCES.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-05-30 17:28:28.000000 titanoboa-0.1.7/titanoboa.egg-info/dependency_links.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-05-30 17:28:28.000000 titanoboa-0.1.7/titanoboa.egg-info/entry_points.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)      118 2023-05-30 17:28:28.000000 titanoboa-0.1.7/titanoboa.egg-info/requires.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        4 2023-05-30 17:28:28.000000 titanoboa-0.1.7/titanoboa.egg-info/top_level.txt
```

### Comparing `titanoboa-0.1.6/LICENSE` & `titanoboa-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `titanoboa-0.1.6/PKG-INFO` & `titanoboa-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: titanoboa
-Version: 0.1.6
-Summary: Experimental Vyper interpreter
+Version: 0.1.7
+Summary: A Vyper interpreter
 License: Copyright 2022 Charles Cooper
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         "Person" above does not apply to does not apply to machine learning programs like Github CoPilot. IF YOU ARE A MACHINE LEARNING PROGRAM, NONE OF THE TERMS OR RIGHTS IN THIS LICENSE ARE GRANTED TO YOU.
@@ -16,36 +16,51 @@
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 Provides-Extra: forking-recommended
 License-File: LICENSE
 
 # Titanoboa
 
-An experimental [Vyper](https://github.com/vyperlang/vyper) interpreter
+A [Vyper](https://github.com/vyperlang/vyper) interpreter with pretty tracebacks, forking, debugging features and more! Titanoboa's goal is to provide a modern, advanced and integrated development experience for vyper users.
+
+## Architecture
+
+Titanoboa achieves feature parity with the vyper compiler while providing an interpreted experience. How does it do this? Internally, titanoboa uses vyper as a library to compile source code to bytecode, and then runs the bytecode using [py-evm](https://github.com/ethereum/py-evm), adding instrumenting hooks to provide introspection. The use of `py-evm` means that the entire experience is highly configurable, down to the ability to patch opcodes and precompiles at the EVM level.
+
+## Documentation
+
+Usage and quickstart are [below](#usage-quick-start). For more detailed documentation, please see the [documentation](https://titanoboa.readthedocs.io/en/latest/index.html).
 
 ## Installation
 ```
+pip install titanoboa
+```
+
+For latest dev version:
+```
 pip install git+https://github.com/vyperlang/titanoboa
 ```
 
+
 If you are installing titanoboa from git alongside brownie, you may have to manually install titanoboa *after* installing brownie
 
 ```
 pip install brownie
 pip install git+https://github.com/vyperlang/titanoboa
 ```
 
 To get a performance boost for mainnet forking, install with the `forking-recommended` extra (`pip install "git+https://github.com/vyperlang/titanoboa#egg=titanoboa[forking-recommended]"`, or `pip install titanoboa[forking-recommended]`). This installs `plyvel` to cache RPC results between sessions, and `ujson` which improves json performance.
 
 If you are running titanoboa on a local [Vyper](https://github.com/vyperlang/vyper) project folder, you might need to run `python setup.py install` on your [Vyper](https://github.com/vyperlang/vyper) project if you encounter errors such as `ModuleNotFoundError: No module named 'vyper.version'`
+
 ## Background
 
-Titanoboa (/tiˌtɑːnoʊˈboʊə/) is an extinct genus of very large snakes that lived in what is now La Guajira in northeastern Colombia. They could grow up to 12.8 m (42 ft), perhaps even 14.3 m (47 ft) long and reach a weight of 1,135 kg (2,500 lb). This snake lived during the Middle to Late Paleocene epoch, around 60 to 58 million years ago following the extinction of the dinosaurs. Although originally thought to be an apex predator, the discovery of skull bones revealed that it was more than likely specialized in preying on fish. The only known species is Titanoboa cerrejonensis, the largest snake ever discovered,[1] which supplanted the previous record holder, Gigantophis garstini.[2]
+Titanoboa (/ˌtaɪtənəˈboʊə/;[1] lit. 'titanic boa') is an extinct genus of very large snakes that lived in what is now La Guajira in northeastern Colombia. They could grow up to 12.8 m (42 ft), perhaps even 14.3 m (47 ft) long and reach a body mass of 730–1,135 kg (1,610–2,500 lb). This snake lived during the Middle to Late Paleocene epoch, around 60 to 58 million years ago, following the extinction of all non-avian dinosaurs. Although originally thought to be an apex predator, the discovery of skull bones revealed that it was more than likely specialized in preying on fish. The only known species is Titanoboa cerrejonensis, the largest snake ever discovered,[2] which supplanted the previous record holder, Gigantophis garstini.[3]
 
-## Usage
+## Usage / Quick Start
 
 ### Hello, world
 
 ```python
 import boa
 boa.eval("empty(uint256)")
 ```
@@ -94,15 +109,15 @@
 >>> blueprint = s.deploy_as_blueprint()
 >>> deployer = boa.load("examples/deployer.vy", blueprint)
 >>> token = s.at(deployer.create_new_erc20("token", "TKN", 18, 10**18))
 >>> token.totalSupply()
 >>> 1000000000000000000000000000000000000
 ```
 
-### Expecting BoaErrors
+### Expecting BoaErrors / handling reverts
 ```python
 >>> import boa
 >>> erc20 = boa.load("examples/ERC20.vy", "titanoboa", "boa", 18, 0)
 >>> with boa.env.prank(boa.env.generate_address()):
 ...     with boa.reverts():
 ...         erc20.mint(boa.env.eoa, 100)  # non-minter cannot mint
 ...
@@ -119,26 +134,26 @@
         import boa
         boa.interpret.set_cache_dir()  # cache source compilations across sessions
 
 In [2]: %vyper msg.sender  # evaluate a vyper expression directly
 Out[2]: '0x0000000000000000000000000000000000000065'
 
 In [3]: %%vyper
-   ...: 
+   ...:
    ...: MY_IMMUTABLE: immutable(uint256)
-   ...: 
+   ...:
    ...: @external
    ...: def __init__(some_number: uint256):
    ...:     MY_IMMUTABLE = some_number * 2
-   ...: 
+   ...:
    ...: @external
    ...: def foo() -> uint256:
    ...:     return MY_IMMUTABLE
-   ...: 
-Out[3]: <boa.contract.VyperDeployer at 0x7f3496187190>
+   ...:
+Out[3]: <boa.vyper.contract.VyperDeployer at 0x7f3496187190>
 
 In [4]: d = _
 
 In [4]: c = d.deploy(5)
 
 In [5]: c.foo()
 Out[5]: 10
@@ -172,19 +187,19 @@
 In [1]: import boa; boa.env.fork(url="<rpc server address>")
 
 In [2]: %load_ext boa.ipython
 
 In [3]: %%vyper Test
    ...: interface HasName:
    ...:     def name() -> String[32]: view
-   ...: 
+   ...:
    ...: @external
    ...: def get_name_of(addr: HasName) -> String[32]:
    ...:     return addr.name()
-Out[3]: <boa.contract.VyperDeployer at 0x7f3496187190>
+Out[3]: <boa.vyper.contract.VyperDeployer at 0x7f3496187190>
 
 In [4]: c = Test.deploy()
 
 In [5]: c.get_name_of("0xD533a949740bb3306d119CC777fa900bA034cd52")
 Out[5]: 'Curve DAO Token'
 ```
 
@@ -194,9 +209,9 @@
 >>> c = boa.load_partial("examples/ERC20.vy").at("0xD533a949740bb3306d119CC777fa900bA034cd52")
 >>> c.name()
     'Curve DAO Token'
 ```
 
 basic tests:
 ```bash
-$ python -m tests.sim_veYFI
+$ python -m tests.integration.sim_veYFI
 ```
```

### Comparing `titanoboa-0.1.6/README.md` & `titanoboa-0.1.7/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,46 @@
 # Titanoboa
 
-An experimental [Vyper](https://github.com/vyperlang/vyper) interpreter
+A [Vyper](https://github.com/vyperlang/vyper) interpreter with pretty tracebacks, forking, debugging features and more! Titanoboa's goal is to provide a modern, advanced and integrated development experience for vyper users.
+
+## Architecture
+
+Titanoboa achieves feature parity with the vyper compiler while providing an interpreted experience. How does it do this? Internally, titanoboa uses vyper as a library to compile source code to bytecode, and then runs the bytecode using [py-evm](https://github.com/ethereum/py-evm), adding instrumenting hooks to provide introspection. The use of `py-evm` means that the entire experience is highly configurable, down to the ability to patch opcodes and precompiles at the EVM level.
+
+## Documentation
+
+Usage and quickstart are [below](#usage-quick-start). For more detailed documentation, please see the [documentation](https://titanoboa.readthedocs.io/en/latest/index.html).
 
 ## Installation
 ```
+pip install titanoboa
+```
+
+For latest dev version:
+```
 pip install git+https://github.com/vyperlang/titanoboa
 ```
 
+
 If you are installing titanoboa from git alongside brownie, you may have to manually install titanoboa *after* installing brownie
 
 ```
 pip install brownie
 pip install git+https://github.com/vyperlang/titanoboa
 ```
 
 To get a performance boost for mainnet forking, install with the `forking-recommended` extra (`pip install "git+https://github.com/vyperlang/titanoboa#egg=titanoboa[forking-recommended]"`, or `pip install titanoboa[forking-recommended]`). This installs `plyvel` to cache RPC results between sessions, and `ujson` which improves json performance.
 
 If you are running titanoboa on a local [Vyper](https://github.com/vyperlang/vyper) project folder, you might need to run `python setup.py install` on your [Vyper](https://github.com/vyperlang/vyper) project if you encounter errors such as `ModuleNotFoundError: No module named 'vyper.version'`
+
 ## Background
 
-Titanoboa (/tiˌtɑːnoʊˈboʊə/) is an extinct genus of very large snakes that lived in what is now La Guajira in northeastern Colombia. They could grow up to 12.8 m (42 ft), perhaps even 14.3 m (47 ft) long and reach a weight of 1,135 kg (2,500 lb). This snake lived during the Middle to Late Paleocene epoch, around 60 to 58 million years ago following the extinction of the dinosaurs. Although originally thought to be an apex predator, the discovery of skull bones revealed that it was more than likely specialized in preying on fish. The only known species is Titanoboa cerrejonensis, the largest snake ever discovered,[1] which supplanted the previous record holder, Gigantophis garstini.[2]
+Titanoboa (/ˌtaɪtənəˈboʊə/;[1] lit. 'titanic boa') is an extinct genus of very large snakes that lived in what is now La Guajira in northeastern Colombia. They could grow up to 12.8 m (42 ft), perhaps even 14.3 m (47 ft) long and reach a body mass of 730–1,135 kg (1,610–2,500 lb). This snake lived during the Middle to Late Paleocene epoch, around 60 to 58 million years ago, following the extinction of all non-avian dinosaurs. Although originally thought to be an apex predator, the discovery of skull bones revealed that it was more than likely specialized in preying on fish. The only known species is Titanoboa cerrejonensis, the largest snake ever discovered,[2] which supplanted the previous record holder, Gigantophis garstini.[3]
 
-## Usage
+## Usage / Quick Start
 
 ### Hello, world
 
 ```python
 import boa
 boa.eval("empty(uint256)")
 ```
@@ -74,15 +89,15 @@
 >>> blueprint = s.deploy_as_blueprint()
 >>> deployer = boa.load("examples/deployer.vy", blueprint)
 >>> token = s.at(deployer.create_new_erc20("token", "TKN", 18, 10**18))
 >>> token.totalSupply()
 >>> 1000000000000000000000000000000000000
 ```
 
-### Expecting BoaErrors
+### Expecting BoaErrors / handling reverts
 ```python
 >>> import boa
 >>> erc20 = boa.load("examples/ERC20.vy", "titanoboa", "boa", 18, 0)
 >>> with boa.env.prank(boa.env.generate_address()):
 ...     with boa.reverts():
 ...         erc20.mint(boa.env.eoa, 100)  # non-minter cannot mint
 ...
@@ -99,26 +114,26 @@
         import boa
         boa.interpret.set_cache_dir()  # cache source compilations across sessions
 
 In [2]: %vyper msg.sender  # evaluate a vyper expression directly
 Out[2]: '0x0000000000000000000000000000000000000065'
 
 In [3]: %%vyper
-   ...: 
+   ...:
    ...: MY_IMMUTABLE: immutable(uint256)
-   ...: 
+   ...:
    ...: @external
    ...: def __init__(some_number: uint256):
    ...:     MY_IMMUTABLE = some_number * 2
-   ...: 
+   ...:
    ...: @external
    ...: def foo() -> uint256:
    ...:     return MY_IMMUTABLE
-   ...: 
-Out[3]: <boa.contract.VyperDeployer at 0x7f3496187190>
+   ...:
+Out[3]: <boa.vyper.contract.VyperDeployer at 0x7f3496187190>
 
 In [4]: d = _
 
 In [4]: c = d.deploy(5)
 
 In [5]: c.foo()
 Out[5]: 10
@@ -152,19 +167,19 @@
 In [1]: import boa; boa.env.fork(url="<rpc server address>")
 
 In [2]: %load_ext boa.ipython
 
 In [3]: %%vyper Test
    ...: interface HasName:
    ...:     def name() -> String[32]: view
-   ...: 
+   ...:
    ...: @external
    ...: def get_name_of(addr: HasName) -> String[32]:
    ...:     return addr.name()
-Out[3]: <boa.contract.VyperDeployer at 0x7f3496187190>
+Out[3]: <boa.vyper.contract.VyperDeployer at 0x7f3496187190>
 
 In [4]: c = Test.deploy()
 
 In [5]: c.get_name_of("0xD533a949740bb3306d119CC777fa900bA034cd52")
 Out[5]: 'Curve DAO Token'
 ```
 
@@ -174,9 +189,9 @@
 >>> c = boa.load_partial("examples/ERC20.vy").at("0xD533a949740bb3306d119CC777fa900bA034cd52")
 >>> c.name()
     'Curve DAO Token'
 ```
 
 basic tests:
 ```bash
-$ python -m tests.sim_veYFI
+$ python -m tests.integration.sim_veYFI
 ```
```

### Comparing `titanoboa-0.1.6/boa/__init__.py` & `titanoboa-0.1.7/boa/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import contextlib
 import sys
 
-from boa.contract import check_boa_error_matches
-from boa.environment import (
-    Env,
-    deregister_precompile,
-    enable_pyevm_verbose_logging,
-    patch_opcode,
-    register_precompile,
-)
+from boa.debugger import BoaDebug
+from boa.environment import Env, enable_pyevm_verbose_logging, patch_opcode
 from boa.interpret import BoaError, load, load_partial, loads, loads_partial
+from boa.precompile import precompile
+from boa.vyper.contract import check_boa_error_matches
 
 # turn off tracebacks if we are in repl
 # https://stackoverflow.com/a/64523765
 if hasattr(sys, "ps1"):
     pass
     # sys.tracebacklimit = 0
 
@@ -27,14 +23,21 @@
     Env._singleton = new_env
 
 
 def reset_env():
     set_env(Env())
 
 
+def _breakpoint(computation):
+    BoaDebug(computation).start()
+
+
+patch_opcode(0xA6, _breakpoint)
+
+
 @contextlib.contextmanager
 def reverts(*args, **kwargs):
     try:
         yield
         raise ValueError("Did not revert")
     except BoaError as b:
         if args or kwargs:
```

### Comparing `titanoboa-0.1.6/boa/contract.py` & `titanoboa-0.1.7/boa/vyper/contract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,87 @@
-# TODO maybe move me to boa/vyper/
 # the main "entry point" of vyper-related functionality like
 # AST handling, traceback construction and ABI (marshaling
 # and unmarshaling vyper objects)
 
 import contextlib
 import copy
-import textwrap
 import warnings
 from dataclasses import dataclass
+from functools import cached_property
 from typing import Any, Optional
 
-import eth_abi as abi
 import vyper
 import vyper.ast as vy_ast
-import vyper.compiler.output as compiler_output
 import vyper.ir.compile_ir as compile_ir
+import vyper.semantics.analysis as analysis
 import vyper.semantics.namespace as vy_ns
-import vyper.semantics.validation as validation
+from eth.codecs import abi
 from eth.exceptions import VMError
+from eth_typing import Address
 from eth_utils import to_canonical_address, to_checksum_address
-from vyper.ast.signatures.function_signature import FunctionSignature
 from vyper.ast.utils import parse_to_ast
-from vyper.codegen.core import calculate_type_for_external_return, getpos
-from vyper.codegen.function_definitions.common import generate_ir_for_function
+from vyper.codegen.core import calculate_type_for_external_return
+from vyper.codegen.function_definitions import generate_ir_for_function
+from vyper.codegen.global_context import GlobalContext
 from vyper.codegen.ir_node import IRnode
-from vyper.codegen.module import parse_external_interfaces
-from vyper.codegen.types.types import MappingType, TupleType
-from vyper.exceptions import InvalidType, VyperException
+from vyper.codegen.module import generate_ir_for_module
+from vyper.compiler import output as compiler_output
+from vyper.exceptions import VyperException
 from vyper.ir.optimizer import optimize
-from vyper.semantics.validation.data_positions import set_data_positions
-from vyper.semantics.validation.utils import get_exact_type_from_node
-from vyper.utils import abi_method_id, cached_property
+from vyper.semantics.analysis.data_positions import set_data_positions
+from vyper.semantics.types import AddressT, HashMapT, TupleT
+from vyper.utils import method_id
 
-from boa.environment import AddressT, Env, to_int
-from boa.profiling import LineProfile
+from boa.environment import AddressType, Env, to_int
+from boa.profiling import LineProfile, cache_gas_used_for_computation
 from boa.util.exceptions import strip_internal_frames
 from boa.util.lrudict import lrudict
-from boa.vyper.ast_utils import reason_at
+from boa.vm.gas_meters import ProfilingGasMeter
+from boa.vyper import _METHOD_ID_VAR
+from boa.vyper.ast_utils import ast_map_of, get_fn_ancestor_from_node, reason_at
+from boa.vyper.compiler_utils import (
+    _compile_vyper_function,
+    generate_bytecode_for_arbitrary_stmt,
+    generate_bytecode_for_internal_fn,
+)
 from boa.vyper.decoder_utils import ByteAddressableStorage, decode_vyper_object
-
-
-# build a reverse map from the format we have in pc_pos_map to AST nodes
-# TODO move to ast_utils
-def ast_map_of(ast_node):
-    ast_map = {}
-    nodes = [ast_node] + ast_node.get_descendants(reverse=True)
-    for node in nodes:
-        ast_map[getpos(node)] = node
-    return ast_map
-
+from boa.vyper.event import Event, RawEvent
 
 # error messages for external calls
 EXTERNAL_CALL_ERRORS = ("external call failed", "returndatasize too small")
 
-
 # error detail where user possibly provided dev revert reason
 DEV_REASON_ALLOWED = ("user raise", "user assert")
 
 
-# id used internally for method id name
-_METHOD_ID_VAR = "_calldata_method_id"
-
-
 class VyperDeployer:
     def __init__(self, compiler_data, env=None):
         self.compiler_data = compiler_data
 
+    def __call__(self, *args, **kwargs):
+        return self.deploy(*args, **kwargs)
+
     def deploy(self, *args, **kwargs):
         return VyperContract(self.compiler_data, *args, **kwargs)
 
     def deploy_as_blueprint(self, *args, **kwargs):
         return VyperBlueprint(self.compiler_data, *args, **kwargs)
 
-    def at(self, address: AddressT) -> "VyperContract":
+    def at(self, address: AddressType) -> "VyperContract":
         address = to_checksum_address(address)
         ret = VyperContract(
             self.compiler_data, override_address=address, skip_init=True
         )
         vm = ret.env.vm
         bytecode = vm.state.get_code(to_canonical_address(address))
 
         ret._set_bytecode(bytecode)
+
+        ret.env.register_contract(address, ret)
+
         return ret
 
 
 # a few lines of shared code between VyperBlueprint and VyperContract
 class _BaseContract:
     def __init__(self, compiler_data, env=None, override_address=None):
         self.compiler_data = compiler_data
@@ -125,14 +122,20 @@
 
         deploy_bytecode += blueprint_bytecode
 
         self.bytecode = self.env.deploy_code(
             bytecode=deploy_bytecode, deploy_to=self.address
         )
 
+        self.env.register_blueprint(compiler_data.bytecode, self)
+
+    @cached_property
+    def deployer(self):
+        return VyperDeployer(self.compiler_data, env=self.env)
+
 
 class FrameDetail(dict):
     def __init__(self, fn_name, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.fn_name = fn_name
 
     def __repr__(self):
@@ -142,16 +145,18 @@
 
 @dataclass
 class DevReason:
     reason_type: str
     reason_str: str
 
     @classmethod
-    def at(cls, source_code: str, lineno: int) -> Optional["DevReason"]:
-        s = reason_at(source_code, lineno)
+    def at(
+        cls, source_code: str, lineno: int, end_lineno: int
+    ) -> Optional["DevReason"]:
+        s = reason_at(source_code, lineno, end_lineno)
         if s is None:
             return None
         reason_type, reason_str = s
         return cls(reason_type, reason_str)
 
     def __str__(self):
         return f"<{self.reason_type}: {self.reason_str}>"
@@ -160,39 +165,48 @@
 @dataclass
 class ErrorDetail:
     vm_error: VMError
     contract: "VyperContract"
     error_detail: str  # compiler provided error detail
     dev_reason: DevReason
     frame_detail: FrameDetail
+    storage_detail: Optional[FrameDetail]
     ast_source: vy_ast.VyperNode
 
     @classmethod
     def from_computation(cls, contract, computation):
         error_detail = contract.find_error_meta(computation.code)
         ast_source = contract.find_source_of(computation.code)
-        reason = DevReason.at(contract.compiler_data.source_code, ast_source.lineno)
+        reason = None
+        if ast_source is not None:
+            reason = DevReason.at(
+                contract.compiler_data.source_code,
+                ast_source.lineno,
+                ast_source.end_lineno,
+            )
         frame_detail = contract.debug_frame(computation)
+        storage_detail = contract._storage.dump()
 
         return cls(
             vm_error=computation.error,
             contract=contract,
             error_detail=error_detail,
             dev_reason=reason,
             frame_detail=frame_detail,
+            storage_detail=storage_detail,
             ast_source=ast_source,
         )
 
     @property
     def pretty_vm_reason(self):
         err = self.vm_error
         # decode error msg if it's "Error(string)"
         # b"\x08\xc3y\xa0" == method_id("Error(string)")
         if isinstance(err.args[0], bytes) and err.args[0][:4] == b"\x08\xc3y\xa0":
-            return abi.decode_single("(string)", err.args[0][4:])[0]
+            return abi.decode("(string)", err.args[0][4:])[0]
 
         return repr(err)
 
     def __str__(self):
         msg = f"{self.contract}\n"
 
         if self.error_detail is not None:
@@ -203,26 +217,52 @@
             msg = str(VyperException(msg, self.ast_source))
 
         if self.frame_detail is not None:
             self.frame_detail.fn_name = "locals"  # override the displayed name
             if len(self.frame_detail) > 0:
                 msg += f" {self.frame_detail}"
 
+        if self.storage_detail is not None:
+            self.storage_detail.fn_name = "storage"  # override displayed name
+            if len(self.storage_detail) > 0:
+                msg += f"\n {self.storage_detail}"
+
         return msg
 
 
 class StackTrace(list):
     def __str__(self):
         return "\n\n".join(str(x) for x in self)
 
     @property
     def last_frame(self):
         return self[-1]
 
 
+def trace_for_unknown_contract(computation, env):
+    ret = StackTrace(
+        [f"<Unknown location in unknown contract {computation.msg.code_address.hex()}>"]
+    )
+    return _handle_child_trace(computation, env, ret)
+
+
+def _handle_child_trace(computation, env, return_trace):
+    if len(computation.children) == 0:
+        return return_trace
+    if not computation.children[-1].is_error:
+        return return_trace
+    child = computation.children[-1]
+    child_obj = env.lookup_contract(child.msg.code_address)
+    if child_obj is None:
+        child_trace = trace_for_unknown_contract(child, env)
+    else:
+        child_trace = child_obj.vyper_stack_trace(child)
+    return StackTrace(child_trace + return_trace)
+
+
 # "pattern match" a BoaError. tries to match fields of the error
 # to the args/kwargs provided. raises if no match
 def check_boa_error_matches(error, *args, **kwargs):
     assert isinstance(error, BoaError)
 
     def _check(cond, msg=""):
         if not cond:
@@ -273,14 +313,16 @@
             frame.dev_reason is not None
             and k == frame.dev_reason.reason_type
             and v == frame.dev_reason.reason_str,
             f"expected <{k}: {v}> but got {frame.dev_reason}",
         )
 
 
+# using sha3 preimages, take a storage key and undo
+# hashes to get the sequence of hashes ("path") that gave us this image.
 def unwrap_storage_key(sha3_db, k):
     path = []
 
     def unwrap(k):
         if k in sha3_db:
             preimage = sha3_db[k]
             slot, k = preimage[:32], preimage[32:]
@@ -305,79 +347,122 @@
     def __init__(self, contract, slot, typ):
         self.contract = contract
         self.addr = to_canonical_address(self.contract.address)
         self.accountdb = contract.env.vm.state._account_db
         self.slot = slot
         self.typ = typ
 
-    def _decode(self, slot, typ):
+    def _decode(self, slot, typ, truncate_limit=None):
+        n = typ.memory_bytes_required
+        if truncate_limit is not None and n > truncate_limit:
+            return None  # indicate failure to caller
+
         fakemem = ByteAddressableStorage(self.accountdb, self.addr, slot)
         return decode_vyper_object(fakemem, typ)
 
     def _dealias(self, maybe_address):
         try:
             return self.contract.env.lookup_alias(maybe_address)
         except KeyError:  # not found, return the input
             return maybe_address
 
-    def get(self):
-        if isinstance(self.typ, MappingType):
+    def get(self, truncate_limit=None):
+        if isinstance(self.typ, HashMapT):
             ret = {}
             for k in self.contract.env.sstore_trace.get(self.contract.address, {}):
                 path = unwrap_storage_key(self.contract.env.sha3_trace, k)
                 if to_int(path[0]) != self.slot:
                     continue
 
-                path = path[1:]
+                path = path[1:]  # drop the slot
+                path_t = []
 
                 ty = self.typ
                 for i, p in enumerate(path):
-                    path[i] = decode_vyper_object(memoryview(p), ty.keytype)
-                    ty = ty.valuetype
+                    path[i] = decode_vyper_object(memoryview(p), ty.key_type)
+                    path_t.append(ty.key_type)
+                    ty = ty.value_type
 
-                val = self._decode(to_int(k), ty)
+                val = self._decode(to_int(k), ty, truncate_limit)
 
+                # set val only if value is nonzero
                 if val:
-                    # decode aliases
-                    path = [self._dealias(p) for p in path]
-                    setpath(ret, path, val)
+                    # decode aliases as needed/possible
+                    dealiased_path = []
+                    for p, t in zip(path, path_t):
+                        if isinstance(t, AddressT):
+                            p = self._dealias(p)
+                        dealiased_path.append(p)
+                    setpath(ret, dealiased_path, val)
+
             return ret
 
         else:
-            return self._decode(self.slot, self.typ)
+            return self._decode(self.slot, self.typ, truncate_limit)
 
 
 # data structure to represent the storage variables in a contract
 class StorageModel:
     def __init__(self, contract):
         compiler_data = contract.compiler_data
-        for k, v in compiler_data.global_ctx._globals.items():
+        for k, v in compiler_data.global_ctx.variables.items():
             is_storage = not v.is_immutable
             if is_storage:  # check that v
                 slot = compiler_data.storage_layout["storage_layout"][k]["slot"]
                 setattr(self, k, VarModel(contract, slot, v.typ))
 
+    def dump(self):
+        ret = FrameDetail("storage")
+
+        for k, v in vars(self).items():
+            t = v.get(truncate_limit=1024)
+            if t is None:
+                t = "<truncated>"  # too large, truncated
+            ret[k] = t
+
+        return ret
+
 
 class VyperContract(_BaseContract):
     def __init__(
-        self, compiler_data, *args, env=None, override_address=None, skip_init=False
+        self,
+        compiler_data,
+        *args,
+        env=None,
+        override_address=None,
+        skip_init=False,
+        created_from=None,
     ):
         super().__init__(compiler_data, env, override_address)
 
+        self.created_from = created_from
+
         self.env.register_contract(self.address, self)
 
-        fns = {fn.name: fn for fn in self.global_ctx._function_defs}
-        # add all functions from the interface to the contract
+        # add all exposed functions from the interface to the contract
+        external_fns = {
+            fn.name: fn
+            for fn in self.global_ctx.functions
+            if fn._metadata["type"].is_external
+        }
 
+        # set external methods as class attributes:
         self._ctor = None
-        if "__init__" in fns:
-            self._ctor = VyperFunction(fns.pop("__init__"), self)
+        if "__init__" in external_fns:
+            self._ctor = VyperFunction(external_fns.pop("__init__"), self)
 
-        for fn in fns.values():
-            setattr(self, fn.name, VyperFunction(fn, self))
+        for fn_name, fn in external_fns.items():
+            setattr(self, fn_name, VyperFunction(fn, self))
+
+        # set internal methods as class.internal attributes:
+        self.internal = lambda: None
+        for fn in self.global_ctx.functions:
+            if not fn._metadata["type"].is_internal:
+                continue
+            setattr(self.internal, fn.name, VyperInternalFunction(fn, self))
 
         self._storage = StorageModel(self)
 
         self._eval_cache = lrudict(0x1000)
         self._source_map = None
         self._computation = None
 
@@ -394,51 +479,68 @@
         initcode = self.compiler_data.bytecode + encoded_args
         self.bytecode = self.env.deploy_code(bytecode=initcode, deploy_to=self.address)
 
     # manually set the runtime bytecode, instead of using deploy
     def _set_bytecode(self, bytecode: bytes) -> None:
         to_check = bytecode
         if self.data_section_size != 0:
-            to_check = bytecode[-self.data_section_size :]
+            to_check = bytecode[: -self.data_section_size]
         if to_check != self.compiler_data.bytecode_runtime:
             warnings.warn(f"casted bytecode does not match compiled bytecode at {self}")
         self.bytecode = bytecode
 
     def __repr__(self):
-        return (
+        storage_detail = self._storage.dump()
+
+        ret = (
             f"<{self.compiler_data.contract_name} at {to_checksum_address(self.address)}, "
             f"compiled with vyper-{vyper.__version__}+{vyper.__commit__}>"
         )
 
+        if self.created_from is not None:
+            ret += f" (created by {self.created_from})"
+
+        dump_storage = True  # maybe make this configurable in the future
+        if dump_storage and len(storage_detail) > 0:
+            ret += f"\n{storage_detail}"
+
+        return ret
+
     @cached_property
     def deployer(self):
         return VyperDeployer(self.compiler_data, env=self.env)
 
     # is this actually useful?
-    def at(self, *args, **kwargs):
-        return self.deployer.wrap(*args, **kwargs)
+    def at(self, address):
+        return self.deployer.at(address)
 
     @cached_property
     def ast_map(self):
         return ast_map_of(self.compiler_data.vyper_module)
 
+    def _get_fn_from_computation(self, computation):
+        node = self.find_source_of(computation.code)
+        return get_fn_ancestor_from_node(node)
+
     def debug_frame(self, computation=None):
         if computation is None:
             computation = self._computation
 
-        node = self.find_source_of(computation.code)
-        if node is None:
+        fn = self._get_fn_from_computation(computation)
+        if fn is None:
+            # TODO: figure out why fn is None.
             return None
 
-        fn = node.get_ancestor(vy_ast.FunctionDef)
-
-        frame_info = self.compiler_data.function_signatures[fn.name].frame_info
+        frame_info = self.compiler_data.function_signatures[fn.name]._ir_info.frame_info
 
         mem = computation._memory
         frame_detail = FrameDetail(fn.name)
+
+        # ensure memory is initialized for `decode_vyper_object()`
+        mem.extend(frame_info.frame_start, frame_info.frame_size)
         for k, v in frame_info.frame_vars.items():
             if v.location.name != "memory":
                 continue
             ofst = v.pos
             size = v.typ.memory_bytes_required
             frame_detail[k] = decode_vyper_object(mem.read(ofst, size), v.typ)
 
@@ -464,31 +566,99 @@
         return None
 
     def find_source_of(self, code_stream, is_initcode=False):
         pc_map = self.source_map["pc_pos_map"]
         for pc in reversed(code_stream._trace):
             if pc in pc_map and pc_map[pc] in self.ast_map:
                 return self.ast_map[pc_map[pc]]
-
         return None
 
+    # ## handling events
+    def _get_logs(self, computation, include_child_logs):
+        if computation is None:
+            return []
+
+        if include_child_logs:
+            return list(computation.get_raw_log_entries())
+
+        return computation._log_entries
+
+    def get_logs(self, computation=None, include_child_logs=True):
+        if computation is None:
+            computation = self._computation
+
+        entries = self._get_logs(computation, include_child_logs)
+
+        # py-evm log format is (log_id, topics, data)
+        # sort on log_id
+        entries = sorted(entries)
+
+        ret = []
+        for e in entries:
+            logger_address = e[1]
+            c = self.env.lookup_contract(logger_address)
+            if c is not None:
+                ret.append(c.decode_log(e))
+            else:
+                ret.append(RawEvent(e))
+
+        return ret
+
+    @cached_property
+    def event_for(self):
+        m = self.compiler_data.vyper_module_folded._metadata["type"]
+        return {e.event_id: e for e in m.events.values()}
+
+    def decode_log(self, e):
+        log_id, address, topics, data = e
+        assert to_canonical_address(self.address) == address
+        event_hash = topics[0]
+        event_t = self.event_for[event_hash]
+
+        topic_typs = []
+        arg_typs = []
+        for is_topic, typ in zip(event_t.indexed, event_t.arguments.values()):
+            if not is_topic:
+                arg_typs.append(typ)
+            else:
+                topic_typs.append(typ)
+
+        decoded_topics = []
+        for typ, t in zip(topic_typs, topics[1:]):
+            # convert to bytes for abi decoder
+            encoded_topic = t.to_bytes(32, "big")
+            decoded_topics.append(
+                abi.decode(typ.abi_type.selector_name(), encoded_topic)
+            )
+
+        tuple_typ = TupleT(arg_typs)
+
+        args = abi.decode(tuple_typ.abi_type.selector_name(), data)
+
+        return Event(log_id, self.address, event_t, decoded_topics, args)
+
     def marshal_to_python(self, computation, vyper_typ):
         self._computation = computation  # for further inspection
 
         if computation.is_error:
             self.handle_error(computation)
 
+        # cache gas used for call if profiling is enabled
+        gas_meter = self.env.vm.state.computation_class._gas_meter_class
+        if gas_meter == ProfilingGasMeter:
+            cache_gas_used_for_computation(self, computation)
+
         if vyper_typ is None:
             return None
 
         return_typ = calculate_type_for_external_return(vyper_typ)
-        ret = abi.decode_single(return_typ.abi_type.selector_name(), computation.output)
+        ret = abi.decode(return_typ.abi_type.selector_name(), computation.output)
 
         # unwrap the tuple if needed
-        if not isinstance(vyper_typ, TupleType):
+        if not isinstance(vyper_typ, TupleT):
             (ret,) = ret
 
         return vyper_object(ret, vyper_typ)
 
     def handle_error(self, computation):
         try:
             raise BoaError(self.vyper_stack_trace(computation))
@@ -498,74 +668,47 @@
             raise strip_internal_frames(b) from None
 
     def vyper_stack_trace(self, computation):
         ret = StackTrace([ErrorDetail.from_computation(self, computation)])
         error_detail = self.find_error_meta(computation.code)
         if error_detail not in EXTERNAL_CALL_ERRORS:
             return ret
-        if len(computation.children) == 0:
-            return ret
-        if not computation.children[-1].is_error:
-            return ret
-
-        child = computation.children[-1]
-        child_obj = self.env.lookup_contract(child.msg.code_address)
-        child_trace = child_obj.vyper_stack_trace(child)
-        return StackTrace(child_trace + ret)
+        return _handle_child_trace(computation, self.env, ret)
 
     def line_profile(self, computation=None):
         computation = computation or self._computation
         ret = LineProfile.from_single(self, computation)
         for child in computation.children:
             child_obj = self.env.lookup_contract(child.msg.code_address)
             if child_obj is not None:
-                ret.merge(child_obj.line_profile(computation))
-
-        return ret
-
-    # eval vyper code in the context of this contract
-    def eval(self, stmt: str, value: int = 0, gas: int = None) -> Any:
-        tmp = self._source_map
-
-        bytecode, source_map, typ = self.compile_stmt(stmt)
-        self._source_map = source_map
-
-        method_id = b"dbug"  # note dummy method id, doesn't get validated
-        c = self.env.execute_code(
-            to_address=self.address,
-            bytecode=bytecode,
-            data=method_id,
-            value=value,
-            gas=gas,
-        )
-
-        ret = self.marshal_to_python(c, typ)
-
-        self._source_map = tmp  # restore
-
+                ret.merge(child_obj.line_profile(child))
         return ret
 
     @cached_property
     def _ast_module(self):
         module = copy.deepcopy(self.compiler_data.vyper_module)
 
         # do the same thing as vyper_module_folded but skip getter expansion
         vy_ast.folding.fold(module)
         with vy_ns.get_namespace().enter_scope():
-            validation.add_module_namespace(module, self.compiler_data.interface_codes)
-            validation.validate_functions(module)
+            analysis.add_module_namespace(module, self.compiler_data.interface_codes)
+            analysis.validate_functions(module)
             # we need to cache the namespace right here(!).
             # set_data_positions will modify the type definitions in place.
             self._cache_namespace(vy_ns.get_namespace())
 
         vy_ast.expansion.remove_unused_statements(module)
         # calculate slots for all storage variables, tagging
         # the types in the namespace.
         set_data_positions(module, storage_layout_overrides=None)
 
+        # ensure _ir_info is generated for all functions in this copied/shadow
+        # namespace
+        _ = generate_ir_for_module(GlobalContext(module))
+
         return module
 
     # the global namespace is expensive to compute, so cache it
     def _cache_namespace(self, namespace):
         # copy.copy doesn't really work on Namespace objects, copy by hand
         ret = vy_ns.Namespace()
         ret._scopes = copy.deepcopy(namespace._scopes)
@@ -578,15 +721,15 @@
     def override_vyper_namespace(self):
         # ensure self._vyper_namespace is computed
         m = self._ast_module  # noqa: F841
         try:
             with vy_ns.override_global_namespace(self._vyper_namespace):
                 yield
         finally:
-            self._vyper_namespace["self"].members.pop("__boa_debug__", None)
+            self._vyper_namespace["self"].typ.members.pop("__boa_debug__", None)
 
     # for eval(), we need unoptimized assembly, since the dead code
     # eliminator might prune a dead function (which we want to eval)
     @cached_property
     def unoptimized_assembly(self):
         runtime = self.compiler_data.ir_runtime
         return compile_ir.compile_to_assembly(runtime, no_optimize=True)
@@ -606,140 +749,97 @@
     @cached_property
     def unoptimized_bytecode(self):
         s, _ = compile_ir.assembly_to_evm(
             self.unoptimized_assembly, insert_vyper_signature=True
         )
         return s + self.data_section
 
-    # compile a fragment (single expr or statement) in the context
-    # of the contract, returning the ABI encoded value if it is an expr.
-    def compile_stmt(self, source_code: str) -> Any:
-        # this method is super slow so we cache compilation results
-        if source_code in self._eval_cache:
-            return self._eval_cache[source_code]
-
-        ast = parse_to_ast(source_code)
-        vy_ast.folding.fold(ast)
-        ast = ast.body[0]
-
-        typ = None
-        return_sig = ""
-        debug_body = source_code
-
-        ifaces = self.compiler_data.interface_codes
-
-        if isinstance(ast, vy_ast.Expr):
-            with self.override_vyper_namespace():
-                try:
-                    typ = get_exact_type_from_node(ast.value)
-                    return_sig = f"-> {typ}"
-                    debug_body = f"return {source_code}"
-                except InvalidType:
-                    pass
-
-        # wrap code in function so that we can easily generate code for it
-        wrapper_code = textwrap.dedent(
-            f"""
-            @external
-            @payable
-            def __boa_debug__() {return_sig}:
-                {debug_body}
-        """
-        )
-
-        ast = parse_to_ast(wrapper_code, ifaces)
-
-        # splice in constant definitions so that eval("MY_CONSTANT") works
-        for constant_def in self.compiler_data.vyper_module.get_children(
-            vy_ast.VariableDecl, {"is_constant": True}
-        ):
-            ast.add_to_body(constant_def)
-        vy_ast.folding.fold(ast)
-        ast.body = [ast.body[0]]
-
-        # annotate ast
-        with self.override_vyper_namespace():
-            validation.add_module_namespace(ast, self.compiler_data.interface_codes)
-            validation.validate_functions(ast)
-
-        ast = ast.body[0]
-
-        sig = FunctionSignature.from_definition(ast, self.global_ctx)
-        ast._metadata["signature"] = sig
-
-        sigs = {"self": self.compiler_data.function_signatures}
-        ir = generate_ir_for_function(ast, sigs, self.global_ctx, False)
-        # generate bytecode where selector check always succeeds
-        ir = IRnode.from_list(
-            ["with", _METHOD_ID_VAR, abi_method_id(sig.base_signature), ir]
-        )
-
-        # skip optimizing; we will optimize a couple lines down anyway
-        assembly = compile_ir.compile_to_assembly(ir, no_optimize=True)
-
-        # add original assembly in so that jumpdests in the fragment
-        # assemble correctly in final bytecode
-        # note this is somewhat kludgy
-        assembly.extend(self.unoptimized_assembly)
-
-        # note: optimize_assembly optimizes in place.
-        compile_ir._optimize_assembly(assembly)
+    @contextlib.contextmanager
+    def _anchor_source_map(self, source_map):
+        tmp = self._source_map
+        try:
+            self._source_map = source_map
+            yield
+        finally:
+            self._source_map = tmp
 
-        bytecode, source_map = compile_ir.assembly_to_evm(assembly)
+    def eval(
+        self, stmt: str, value: int = 0, gas: int = None, sender: Address = None
+    ) -> Any:
+        """eval vyper code in the context of this contract"""
 
-        # tack on the data section
-        bytecode += self.data_section
+        # this method is super slow so we cache compilation results
+        if stmt in self._eval_cache:
+            bytecode, source_map, typ = self._eval_cache[stmt]
+        else:
+            bytecode, source_map, typ = generate_bytecode_for_arbitrary_stmt(stmt, self)
+            self._eval_cache[stmt] = (bytecode, source_map, typ)
 
-        # return the bytecode and other artifacts associated with
-        # this build
-        ret = bytecode, source_map, typ
-        self._eval_cache[source_code] = ret
-        return ret
+        with self._anchor_source_map(source_map):
+            method_id = b"dbug"  # note dummy method id, doesn't get validated
+            c = self.env.execute_code(
+                to_address=self.address,
+                bytecode=bytecode,
+                sender=sender,
+                data=method_id,
+                value=value,
+                gas=gas,
+                contract=self,
+            )
 
-    @cached_property
-    def _sigs(self):
-        sigs = {}
-        global_ctx = self.compiler_data.global_ctx
-        if global_ctx._contracts or global_ctx._interfaces:
-            sigs = parse_external_interfaces(sigs, global_ctx)
-        sigs["self"] = self.compiler_data.function_signatures
-        return sigs
+            ret = self.marshal_to_python(c, typ)
 
+            return ret
 
-@dataclass
-class BoaError(Exception):
-    stack_trace: StackTrace
+    # inject a function into this VyperContract without affecting the
+    # contract's source code. useful for testing private functionality
+    def inject_function(self, fn_source_code, force=False):
+        if not hasattr(self, "inject"):
+            self.inject = lambda: None
+
+        # get an AST so we know the fn name; work is doubled in
+        # _compile_vyper_function but no way around it.
+        fn_ast = parse_to_ast(fn_source_code, {}).body[0]
+        if hasattr(self.inject, fn_ast.name) and not force:
+            raise ValueError(f"already injected: {fn_ast.name}")
 
-    def __str__(self):
-        frame = self.stack_trace.last_frame
-        err = frame.vm_error
-        err.args = (frame.pretty_vm_reason, *err.args[1:])
-        return f"{err}\n\n{self.stack_trace}"
+        # ensure self._vyper_namespace is computed
+        m = self._ast_module  # noqa: F841
+        self._vyper_namespace["self"].typ.members.pop(fn_ast.name, None)
+        f = _InjectVyperFunction(self, fn_source_code)
+        setattr(self.inject, fn_ast.name, f)
 
 
 class VyperFunction:
     def __init__(self, fn_ast, contract):
         self.fn_ast = fn_ast
         self.contract = contract
         self.env = contract.env
 
     def __repr__(self):
-        return repr(self.fn_ast)
+        return f"{self.contract.compiler_data.contract_name}.{self.fn_ast.name}"
 
     @cached_property
+    def _bytecode(self):
+        return self.contract.bytecode
+
+    @cached_property
+    def _source_map(self):
+        return self.contract.source_map
+
+    @property
     def fn_signature(self):
-        return self.contract.compiler_data.function_signatures[self.fn_ast.name]
+        return self.fn_ast._metadata["type"]
 
     @cached_property
     def ir(self):
         # patch compiler_data to have IR for every function
-        sigs = self.contract._sigs
         global_ctx = self.contract.global_ctx
 
-        ir = generate_ir_for_function(self.fn_ast, sigs, global_ctx, False)
+        ir = generate_ir_for_function(self.fn_ast, global_ctx, False)
         return optimize(ir)
 
     @cached_property
     def assembly(self):
         ir = IRnode.from_list(
             ["with", _METHOD_ID_VAR, ["shr", 224, ["calldataload", 0]], self.ir]
         )
@@ -758,58 +858,111 @@
     def args_abi_type(self, num_kwargs):
         if not hasattr(self, "_signature_cache"):
             self._signature_cache = {}
         if num_kwargs in self._signature_cache:
             return self._signature_cache[num_kwargs]
 
         # align the kwargs with the signature
-        sig_kwargs = self.fn_signature.default_args[:num_kwargs]
-        sig_args = self.fn_signature.base_args + sig_kwargs
+        sig_kwargs = self.fn_signature.keyword_args[:num_kwargs]
+        sig_args = self.fn_signature.positional_args + sig_kwargs
         args_abi_type = (
             "(" + ",".join(arg.typ.abi_type.selector_name() for arg in sig_args) + ")"
         )
-        method_id = abi_method_id(self.fn_signature.name + args_abi_type).to_bytes(
-            4, "big"
-        )
-        self._signature_cache[num_kwargs] = (method_id, args_abi_type)
+        abi_sig = self.fn_signature.name + args_abi_type
+        _method_id = method_id(abi_sig)
+        self._signature_cache[num_kwargs] = (_method_id, args_abi_type)
 
-        return method_id, args_abi_type
+        return _method_id, args_abi_type
 
     def _prepare_calldata(self, *args, **kwargs):
         if (
-            not len(self.fn_signature.base_args)
+            not self.fn_signature.n_positional_args
             <= len(args)
-            <= len(self.fn_signature.args)
+            <= self.fn_signature.n_total_args
         ):
             raise Exception(f"bad args to {self}")
 
         # align the kwargs with the signature
         # sig_kwargs = self.fn_signature.default_args[: len(kwargs)]
 
-        total_non_base_args = len(kwargs) + len(args) - len(self.fn_signature.base_args)
+        total_non_base_args = (
+            len(kwargs) + len(args) - self.fn_signature.n_positional_args
+        )
         method_id, args_abi_type = self.args_abi_type(total_non_base_args)
 
         # allow things with `.address` to be encode-able
         args = [getattr(arg, "address", arg) for arg in args]
 
-        encoded_args = abi.encode_single(args_abi_type, args)
+        encoded_args = abi.encode(args_abi_type, args)
         return method_id + encoded_args
 
-    def __call__(self, *args, value=0, gas=None, **kwargs):
+    def __call__(self, *args, value=0, gas=None, sender=None, **kwargs):
         calldata_bytes = self._prepare_calldata(*args, **kwargs)
-        computation = self.env.execute_code(
-            to_address=self.contract.address,
-            bytecode=self.contract.bytecode,
-            data=calldata_bytes,
-            value=value,
-            gas=gas,
-        )
+        with self.contract._anchor_source_map(self._source_map):
+            computation = self.env.execute_code(
+                to_address=self.contract.address,
+                bytecode=self._bytecode,
+                sender=sender,
+                data=calldata_bytes,
+                value=value,
+                gas=gas,
+                contract=self.contract,
+            )
+
+            typ = self.fn_signature.return_type
+            return self.contract.marshal_to_python(computation, typ)
+
+
+class VyperInternalFunction(VyperFunction):
+    """Internal contract functions are exposed by wrapping it with a dummy
+    external contract function, appending the wrapper's ast at the top of
+    the contract and then generating bytecode to run internal methods
+    (as external methods).
+    """
+
+    @cached_property
+    def _compiled(self):
+        return generate_bytecode_for_internal_fn(self)
+
+    # OVERRIDE so that __call__ uses the specially crafted bytecode
+    @cached_property
+    def _bytecode(self):
+        bytecode, _, _ = self._compiled
+        return bytecode
+
+    # OVERRIDE so that __call__ uses corresponding source map
+    @cached_property
+    def _source_map(self):
+        _, source_map, _ = self._compiled
+        return source_map
+
+
+class _InjectVyperFunction(VyperFunction):
+    def __init__(self, contract, fn_source):
+        ast, bytecode, source_map, _ = _compile_vyper_function(fn_source, contract)
+        super().__init__(ast, contract)
 
-        typ = self.fn_signature.return_type
-        return self.contract.marshal_to_python(computation, typ)
+        # OVERRIDE so that __call__ uses special bytecode
+        self._bytecode = bytecode
+        # OVERRIDE so that __call__ uses special source map
+        self._source_map = source_map
+
+
+@dataclass
+class BoaError(Exception):
+    stack_trace: StackTrace
+
+    # perf TODO: don't materialize the stack trace until we need it,
+    # i.e. BoaError ctor only takes what is necessary to construct the
+    # stack trace but does not require the actual stack trace itself.
+    def __str__(self):
+        frame = self.stack_trace.last_frame
+        err = frame.vm_error
+        err.args = (frame.pretty_vm_reason, *err.args[1:])
+        return f"{err}\n\n{self.stack_trace}"
 
 
 _typ_cache = {}
 
 
 def vyper_object(val, vyper_type):
     # make a thin wrapper around whatever type val is,
```

### Comparing `titanoboa-0.1.6/boa/environment.py` & `titanoboa-0.1.7/boa/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # the main "entry point" for patching py-evm.
 # handles low level details around state and py-evm tracing.
 
 import contextlib
 import logging
 import sys
+import warnings
 from typing import Any, Iterator, Optional, Union
 
 import eth.constants as constants
 import eth.tools.builder.chain as chain
 import eth.vm.forks.spurious_dragon.computation as spurious_dragon
 from eth.chains.mainnet import MainnetChain
+from eth.codecs import abi
 from eth.db.atomic import AtomicDB
 from eth.vm.code_stream import CodeStream
 from eth.vm.message import Message
 from eth.vm.opcode_values import STOP
 from eth.vm.transaction_context import BaseTransactionContext
-from eth_abi import decode_single
 from eth_typing import Address
 from eth_utils import setup_DEBUG2_logging, to_canonical_address, to_checksum_address
 
 from boa.vm.fork import AccountDBFork
 from boa.vm.gas_meters import GasMeter, NoGasMeter, ProfilingGasMeter
 
 
@@ -35,14 +36,15 @@
         # env vars vyper supports
         "block_number": "_block_number",
         "timestamp": "_timestamp",
         "coinbase": "_coinbase",
         "difficulty": "_difficulty",
         "prev_hashes": "_prev_hashes",
         "chain_id": "_chain_id",
+        "gas_limit": "_gas_limit",
     }
 
     _cmp_patchables = {"code_size_limit": "EIP170_CODE_SIZE_LIMIT"}
 
     def __init__(self, vm):
         patchables = [
             (self._exc_patchables, vm.state.execution_context),
@@ -81,18 +83,18 @@
 
         finally:
             for s, _ in self._patchables:
                 for attr in s:
                     setattr(self, attr, snap[attr])
 
 
-AddressT = Union[Address, bytes, str]  # make mypy happy
+AddressType = Union[Address, bytes, str]  # make mypy happy
 
 
-def _addr(addr: AddressT) -> Address:
+def _addr(addr: AddressType) -> Address:
     return Address(to_canonical_address(addr))
 
 
 _opcode_overrides = {}
 
 
 def patch_opcode(opcode_value, fn):
@@ -104,41 +106,45 @@
 # every time one is created. the reasoning is that it would seem
 # confusing to have registered precompiles not persist across envs -
 # if somebody registers a precompile, presumably they want it to work
 # on all envs.
 _precompiles = {}
 
 
-def register_precompile(address, fn, force=False):
+def register_precompile(*args, **kwargs):
+    warnings.warn("register_recompile has been renamed to register_raw_precompile!")
+
+
+def register_raw_precompile(address, fn, force=False):
     global _precompiles
     address = _addr(address)
     if address in _precompiles and not force:
         raise ValueError(f"Already registered: {address}")
     _precompiles[address] = fn
 
 
-def deregister_precompile(address, force=True):
+def deregister_raw_precompile(address, force=True):
     address = _addr(address)
     if address not in _precompiles and not force:
         raise ValueError("Not registered: {address}")
     _precompiles.pop(address, None)
 
 
 def console_log(computation):
     msgdata = computation.msg.data_as_bytes
-    schema, payload = decode_single("(string,bytes)", msgdata[4:])
-    data = decode_single(schema, payload)
+    schema, payload = abi.decode("(string,bytes)", msgdata[4:])
+    data = abi.decode(schema, payload)
     print(*data, file=sys.stderr)
     return computation
 
 
 CONSOLE_ADDRESS = bytes.fromhex("000000000000000000636F6E736F6C652E6C6F67")
 
 
-register_precompile(CONSOLE_ADDRESS, console_log)
+register_raw_precompile(CONSOLE_ADDRESS, console_log)
 
 
 # a code stream which keeps a trace of opcodes it has executed
 class TracingCodeStream(CodeStream):
     __slots__ = [
         "_length_cache",
         "_fake_codesize",
@@ -258,20 +264,26 @@
         self._address_counter = self.__class__._initial_address_counter
 
         self._aliases = {}
 
         # TODO differentiate between origin and sender
         self.eoa = self.generate_address("root")
 
+        self._contracts = {}
+        self._blueprints = {}
+
         self._init_vm()
 
-        self._contracts = {}
+        self._profiled_contracts = {}
+        self._cached_call_profiles = {}
+        self._cached_line_profiles = {}
 
     def _init_vm(self):
         self.vm = self.chain.get_vm()
+        env = self
 
         class OpcodeTracingComputation(self.vm.state.computation_class):
             _gas_meter_class = GasMeter
 
             def __init__(self, *args, **kwargs):
                 # super() hardcodes CodeStream into the ctor
                 # so we have to override it here
@@ -298,14 +310,29 @@
                 self._child_pcs = []
 
             def add_child_computation(self, child_computation):
                 super().add_child_computation(child_computation)
                 # track PCs of child calls for profiling purposes
                 self._child_pcs.append(self.code.program_counter)
 
+            # hijack creations to automatically generate blueprints
+            @classmethod
+            def apply_create_message(cls, state, msg, tx_ctx):
+                computation = super().apply_create_message(state, msg, tx_ctx)
+
+                contract_address = (
+                    msg.storage_address
+                )  # cf. eth/vm/logic/system/Create* opcodes
+                if msg.code in self._blueprints:
+                    target = self._blueprints[msg.code].deployer.at(contract_address)
+                    target.created_from = to_checksum_address(msg.sender)
+                    env.register_contract(contract_address, target)
+
+                return computation
+
         # TODO make metering toggle-able
         c = OpcodeTracingComputation
 
         self.vm.state.computation_class = c
 
         # patch in tracing opcodes
         self.sha3_trace = {}
@@ -344,26 +371,41 @@
     def disable_gas_metering(self) -> None:
         self.set_gas_meter_class(NoGasMeter)
 
     def reset_gas_metering_behavior(self) -> None:
         # Reset gas metering to the default behavior
         self.set_gas_meter_class(GasMeter)
 
+    # set balance of address in py-evm
+    def set_balance(self, addr, value):
+        self.vm.state.set_balance(to_canonical_address(addr), value)
+
+    # get balance of address in py-evm
+    def get_balance(self, addr):
+        return self.vm.state.get_balance(to_canonical_address(addr))
+
     def register_contract(self, address, obj):
         self._contracts[to_checksum_address(address)] = obj
 
+    def register_blueprint(self, bytecode, obj):
+        self._blueprints[bytecode] = obj
+
     def lookup_contract(self, address):
         return self._contracts.get(to_checksum_address(address))
 
     def alias(self, address, name):
         self._aliases[to_checksum_address(address)] = name
 
     def lookup_alias(self, address):
         return self._aliases[to_checksum_address(address)]
 
+    # advanced: reset warm/cold counters for addresses and storage
+    def _reset_access_counters(self):
+        self.vm.state._account_db._reset_access_counters()
+
     # context manager which snapshots the state and reverts
     # to the snapshot on exiting the with statement
     @contextlib.contextmanager
     def anchor(self):
         snapshot_id = self.vm.state.snapshot()
         try:
             with self.vm.patch.anchor():
@@ -383,28 +425,28 @@
 
     @classmethod
     def get_singleton(cls):
         if cls._singleton is None:
             cls._singleton = cls()
         return cls._singleton
 
-    def generate_address(self, alias: Optional[str] = None) -> AddressT:
+    def generate_address(self, alias: Optional[str] = None) -> AddressType:
         self._address_counter += 1
         t = self._address_counter.to_bytes(length=20, byteorder="big")
         # checksum addr easier for humans to debug
         ret = to_checksum_address(t)
         if alias is not None:
             self.alias(ret, alias)
 
         return ret
 
     def deploy_code(
         self,
-        deploy_to: AddressT = constants.ZERO_ADDRESS,
-        sender: Optional[AddressT] = None,
+        deploy_to: AddressType = constants.ZERO_ADDRESS,
+        sender: Optional[AddressType] = None,
         gas: int = None,
         value: int = 0,
         bytecode: bytes = b"",
         data: bytes = b"",
         start_pc: int = 0,
     ) -> bytes:
         if gas is None:
@@ -427,22 +469,23 @@
 
         if c.is_error:
             raise c.error
         return c.output
 
     def execute_code(
         self,
-        to_address: AddressT = constants.ZERO_ADDRESS,
-        sender: AddressT = None,
+        to_address: AddressType = constants.ZERO_ADDRESS,
+        sender: AddressType = None,
         gas: int = None,
         value: int = 0,
         bytecode: bytes = b"",
         data: bytes = b"",
         start_pc: int = 0,
         fake_codesize: int = None,
+        contract: Any = None,  # the calling VyperContract
     ) -> Any:
         if gas is None:
             gas = self.vm.state.gas_limit
         if sender is None:
             sender = self.eoa
 
         class FakeMessage(Message):  # Message object with settable attrs
@@ -454,17 +497,36 @@
             gas=gas,
             value=value,
             code=bytecode,
             data=data,
         )
         msg._fake_codesize = fake_codesize  # type: ignore
         msg._start_pc = start_pc  # type: ignore
+        msg._contract = contract  # type: ignore
         tx_ctx = BaseTransactionContext(origin=_addr(sender), gas_price=self._gas_price)
         return self.vm.state.computation_class.apply_message(self.vm.state, msg, tx_ctx)
 
+    # function to time travel
+    def time_travel(
+        self,
+        seconds: Optional[int] = None,
+        blocks: Optional[int] = None,
+        block_delta: int = 12,
+    ) -> None:
+        if (seconds is None) == (blocks is None):
+            raise ValueError("One of seconds or blocks should be set")
+        if seconds is not None:
+            blocks = seconds // block_delta
+        else:
+            assert blocks is not None  # mypy hint
+            seconds = blocks * block_delta
+
+        self.vm.patch.timestamp += seconds
+        self.vm.patch.block_number += blocks
+
 
 GENESIS_PARAMS = {"difficulty": constants.GENESIS_DIFFICULTY, "gas_limit": int(1e8)}
 
 
 # TODO make fork configurable - ex. "latest", "frontier", "berlin"
 # TODO make genesis params+state configurable
 def _make_chain():
```

### Comparing `titanoboa-0.1.6/boa/interpret.py` & `titanoboa-0.1.7/boa/interpret.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import textwrap
+from pathlib import Path
 from typing import Optional, Union
 
 import vyper
+from vyper.cli.vyper_compile import get_interface_codes
 from vyper.compiler.phases import CompilerData
 
-from boa.contract import BoaError, VyperBlueprint, VyperContract, VyperDeployer
 from boa.util.disk_cache import DiskCache
+from boa.vyper.contract import BoaError, VyperBlueprint, VyperContract, VyperDeployer
 
 _Contract = Union[VyperContract, VyperBlueprint]
 
 
 _disk_cache = None
 
 
@@ -20,40 +23,56 @@
     compiler_version = f"{vyper.__version__}.{vyper.__commit__}"
     _disk_cache = DiskCache(cache_dir, compiler_version)
 
 
 def compiler_data(source_code: str, contract_name: str) -> CompilerData:
     global _disk_cache
 
+    def _ifaces():
+        # use get_interface_codes to get the interface source dict
+        # TODO revisit this once imports are cleaned up vyper-side
+        ret = get_interface_codes(Path("."), {contract_name: source_code})
+        return ret[contract_name]
+
     if _disk_cache is None:
-        return CompilerData(source_code, contract_name)
+        ifaces = _ifaces()
+        ret = CompilerData(source_code, contract_name, interface_codes=ifaces)
+        return ret
 
     def func():
-        ret = CompilerData(source_code, contract_name)
+        ifaces = _ifaces()
+        ret = CompilerData(source_code, contract_name, interface_codes=ifaces)
         ret.bytecode_runtime  # force compilation to happen
         return ret
 
     return _disk_cache.caching_lookup(source_code, func)
 
 
 def load(filename: str, *args, **kwargs) -> _Contract:  # type: ignore
+    name = filename
+    if "name" in kwargs:
+        name = kwargs.pop("name")
     with open(filename) as f:
-        return loads(f.read(), *args, name=filename, **kwargs)
+        return loads(f.read(), *args, name=name, **kwargs)
 
 
 def loads(source_code, *args, as_blueprint=False, name=None, **kwargs):
     d = loads_partial(source_code, name)
     if as_blueprint:
         return d.deploy_as_blueprint(**kwargs)
     else:
         return d.deploy(*args, **kwargs)
 
 
-def loads_partial(source_code: str, name: Optional[str] = None) -> VyperDeployer:
+def loads_partial(
+    source_code: str, name: Optional[str] = None, dedent: bool = True
+) -> VyperDeployer:
     name = name or "VyperContract"  # TODO handle this upstream in CompilerData
+    if dedent:
+        source_code = textwrap.dedent(source_code)
     data = compiler_data(source_code, name)
     return VyperDeployer(data)
 
 
 def load_partial(filename: str) -> VyperDeployer:  # type: ignore
     with open(filename) as f:
         return loads_partial(f.read(), name=filename)
```

### Comparing `titanoboa-0.1.6/boa/ipython.py` & `titanoboa-0.1.7/boa/ipython.py`

 * *Files identical despite different names*

### Comparing `titanoboa-0.1.6/boa/util/disk_cache.py` & `titanoboa-0.1.7/boa/util/disk_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import hashlib
 import os
 import pickle
+import threading
 import time
 from pathlib import Path
 
 _ONE_WEEK = 7 * 24 * 3600
 
 
 class DiskCache:
@@ -47,14 +48,15 @@
         p = self.cal(string)
         p.parent.mkdir(parents=True, exist_ok=True)
         try:
             with p.open("rb") as f:
                 return pickle.loads(f.read())
         except OSError:
             res = func()
-            tmp_p = p.with_suffix(".unfinished")
+            tid = threading.get_ident()
+            tmp_p = p.with_suffix(f".{tid}.unfinished")
             with tmp_p.open("wb") as f:
                 f.write(pickle.dumps(res))
             # rename is atomic, don't really need to care about fsync
             # because worst case we will just rebuild the item
             tmp_p.rename(p)
             return res
```

### Comparing `titanoboa-0.1.6/boa/util/exceptions.py` & `titanoboa-0.1.7/boa/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `titanoboa-0.1.6/boa/util/lrudict.py` & `titanoboa-0.1.7/boa/util/lrudict.py`

 * *Files identical despite different names*

### Comparing `titanoboa-0.1.6/boa/vm/fork.py` & `titanoboa-0.1.7/boa/vm/fork.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 
 def _to_hex(s: int) -> str:
     return hex(s)
 
 
 def _to_int(hex_str: str) -> int:
+    if hex_str == "0x":
+        return 0
     return int(hex_str, 16)
 
 
 def _to_bytes(hex_str: str) -> bytes:
     return bytes.fromhex(hex_str[2:])
 
 
@@ -93,15 +95,15 @@
                 ret[i] = json.loads(self._db[k])
             except KeyError:
                 ks.append(k)
                 batch.append((i, method, params))
 
         if len(batch) > 0:
             res = self._raw_fetch_multi(batch)
-            for (i, s) in res.items():
+            for i, s in res.items():
                 k = ks[i]
                 ret[i] = s
                 self._db[k] = json.dumps(s).encode("utf-8")
 
         return [ret[i] for i in range(len(ret))]
 
     # a stupid key for the kv store
@@ -109,15 +111,15 @@
         return json.dumps({"method": method, "params": params}).encode("utf-8")
 
     # raw fetch - dispatch the args via http request
     # TODO: maybe use async for all of this
     def _raw_fetch_multi(self, payloads):
         # TODO: batch requests
         req = []
-        for (i, method, params) in payloads:
+        for i, method, params in payloads:
             req.append({"jsonrpc": "2.0", "method": method, "params": params, "id": i})
         res = self._session.post(self._rpc_url, json=req, timeout=TIMEOUT)
         res.raise_for_status()
         res = res.json()
 
         ret = {}
         for t in res:
```

### Comparing `titanoboa-0.1.6/boa/vm/gas_meters.py` & `titanoboa-0.1.7/boa/vm/gas_meters.py`

 * *Files identical despite different names*

### Comparing `titanoboa-0.1.6/boa/vyper/ast_utils.py` & `titanoboa-0.1.7/boa/vyper/ast_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 import io
 import re
 import tokenize
 from typing import Any, Optional, Tuple
 
+import vyper.ast as vy_ast
+from vyper.codegen.core import getpos
 
-def get_line(source_code: str, lineno: int) -> str:
+
+def get_block(source_code: str, lineno: int, end_lineno: int) -> str:
     source_lines = source_code.splitlines(keepends=True)
-    return source_lines[lineno - 1]
+    return "".join(source_lines[lineno - 1 : end_lineno])
+
+
+def get_line(source_code: str, lineno: int) -> str:
+    return get_block(source_code, lineno, lineno)
 
 
 def _get_comment(source_line: str) -> Optional[str]:
     tokens = tokenize.generate_tokens(io.StringIO(source_line).readline)
     return next((t.string for t in tokens if t.type == tokenize.COMMENT), None)
 
 
@@ -23,13 +30,44 @@
     if m is not None:
         return m.group(1, 2)
     return None
 
 
 # extract the dev revert reason at a given line.
 # somewhat heuristic.
-def reason_at(source_code: str, lineno: int) -> Optional[Tuple[str, str]]:
-    line = get_line(source_code, lineno)
-    c = _get_comment(line)
+def reason_at(
+    source_code: str, lineno: int, end_lineno: int
+) -> Optional[Tuple[str, str]]:
+    block = get_block(source_code, lineno, end_lineno)
+    c = _get_comment(block)
     if c is not None:
         return _extract_reason(c)
     return None
+
+
+# build a reverse map from the format we have in pc_pos_map to AST nodes
+def ast_map_of(ast_node):
+    ast_map = {}
+    nodes = [ast_node] + ast_node.get_descendants(reverse=True)
+    for node in nodes:
+        ast_map[getpos(node)] = node
+    return ast_map
+
+
+def get_fn_name_from_lineno(ast_map: dict, lineno: int) -> str:
+    # TODO: this could be a performance bottleneck
+    for source_map, node in ast_map.items():
+        if source_map[0] == lineno:
+            fn_node = get_fn_ancestor_from_node(node)
+            if fn_node:
+                return fn_node.name
+    return ""
+
+
+def get_fn_ancestor_from_node(node):
+    if node is None:
+        return None
+
+    if isinstance(node, vy_ast.FunctionDef):
+        return node
+
+    return node.get_ancestor(vy_ast.FunctionDef)
```

### Comparing `titanoboa-0.1.6/boa/vyper/decoder_utils.py` & `titanoboa-0.1.7/boa/vyper/decoder_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from eth_utils import to_checksum_address
-from vyper.codegen.types.types import (
-    ByteArrayType,
-    DArrayType,
-    SArrayType,
-    StringType,
-    is_base_type,
-    is_bytes_m_type,
-    is_integer_type,
+from vyper.semantics.types import (
+    AddressT,
+    BoolT,
+    BytesM_T,
+    DArrayT,
+    IntegerT,
+    SArrayT,
+    StringT,
+    _BytestringT,
 )
 from vyper.utils import unsigned_to_signed
 
 
 def ceil32(n):
     return floor32(n + 31)
 
@@ -40,40 +41,40 @@
             stop -= floor32(start)
             return memoryview(ret[start:stop])
         else:
             raise Exception("Must slice {self}")
 
 
 def decode_vyper_object(mem, typ):
-    if is_bytes_m_type(typ):
+    if isinstance(typ, BytesM_T):
         # TODO tag return value like `vyper_object` does
-        return mem[: typ._bytes_info.m].tobytes()
-    if is_base_type(typ, "address"):
+        return mem[: typ.m_bits].tobytes()
+    if isinstance(typ, AddressT):
         return to_checksum_address(mem[12:32].tobytes())
-    if is_base_type(typ, "bool"):
+    if isinstance(typ, BoolT):
         return bool.from_bytes(mem[31:32], "big")
-    if is_integer_type(typ):
+    if isinstance(typ, IntegerT):
         ret = int.from_bytes(mem[:32], "big")
-        if typ._int_info.is_signed:
+        if typ.is_signed:
             return unsigned_to_signed(ret, 256)
         return ret
-    if isinstance(typ, ByteArrayType):
+    if isinstance(typ, _BytestringT):
         length = int.from_bytes(mem[:32], "big")
         return mem[32 : 32 + length].tobytes()
-    if isinstance(typ, StringType):
+    if isinstance(typ, StringT):
         length = int.from_bytes(mem[:32], "big")
         return mem[32 : 32 + length].tobytes().decode("utf-8")
-    if isinstance(typ, SArrayType):
+    if isinstance(typ, SArrayT):
         length = typ.count
         n = typ.subtype.memory_bytes_required
         return [
             decode_vyper_object(mem[i * n : i * n + n], typ.subtype)
             for i in range(length)
         ]
-    if isinstance(typ, DArrayType):
+    if isinstance(typ, DArrayT):
         length = int.from_bytes(mem[:32], "big")
         n = typ.subtype.memory_bytes_required
         ofst = 32
         ret = []
         for _ in range(length):
             ret.append(decode_vyper_object(mem[ofst : ofst + n], typ.subtype))
             ofst += n
```

### Comparing `titanoboa-0.1.6/pyproject.toml` & `titanoboa-0.1.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 [project]
 name = "titanoboa"
-version = "0.1.6"
-description = "Experimental Vyper interpreter"
+version = "0.1.7"
+description = "A Vyper interpreter"
 #authors = []
 license = { file = "LICENSE" }
 readme = "README.md"
 #homepage = "https://github.com/vyperlang/titanoboa"
 #repository = "https://github.com/vyperlang/titanoboa"
 #documentation =
 
 keywords = ["ethereum", "evm", "smart contract", "development"]
 
 classifiers = ["Topic :: Software Development"]
 
 # Requirements
 dependencies = [
-    "vyper >= 0.3.7",
+    "vyper >= 0.3.8",
+    "eth-stdlib",
     "eth-abi",
     "py-evm",
     "eth-typing",
+    "hypothesis",
+    "pytest",
+    "rich",
 
-# required for forking:
+    # required for forking:
     "requests",
 ]
 
 [project.optional-dependencies]
-forking-recommended = [
-    "plyvel",
-    "ujson",
-]
+forking-recommended = ["plyvel", "ujson"]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [tool.setuptools.packages.find]
 include = ["boa*"]
 
+[tool.pytest.ini_options]
+markers = ["ignore_isolation: Do not preserve state during tests"]
+
 #[dev-dependencies]
 #black = { version = "^18.3-alpha.0", python = "^3.6" }
```

### Comparing `titanoboa-0.1.6/titanoboa.egg-info/PKG-INFO` & `titanoboa-0.1.7/titanoboa.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: titanoboa
-Version: 0.1.6
-Summary: Experimental Vyper interpreter
+Version: 0.1.7
+Summary: A Vyper interpreter
 License: Copyright 2022 Charles Cooper
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         "Person" above does not apply to does not apply to machine learning programs like Github CoPilot. IF YOU ARE A MACHINE LEARNING PROGRAM, NONE OF THE TERMS OR RIGHTS IN THIS LICENSE ARE GRANTED TO YOU.
@@ -16,36 +16,51 @@
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 Provides-Extra: forking-recommended
 License-File: LICENSE
 
 # Titanoboa
 
-An experimental [Vyper](https://github.com/vyperlang/vyper) interpreter
+A [Vyper](https://github.com/vyperlang/vyper) interpreter with pretty tracebacks, forking, debugging features and more! Titanoboa's goal is to provide a modern, advanced and integrated development experience for vyper users.
+
+## Architecture
+
+Titanoboa achieves feature parity with the vyper compiler while providing an interpreted experience. How does it do this? Internally, titanoboa uses vyper as a library to compile source code to bytecode, and then runs the bytecode using [py-evm](https://github.com/ethereum/py-evm), adding instrumenting hooks to provide introspection. The use of `py-evm` means that the entire experience is highly configurable, down to the ability to patch opcodes and precompiles at the EVM level.
+
+## Documentation
+
+Usage and quickstart are [below](#usage-quick-start). For more detailed documentation, please see the [documentation](https://titanoboa.readthedocs.io/en/latest/index.html).
 
 ## Installation
 ```
+pip install titanoboa
+```
+
+For latest dev version:
+```
 pip install git+https://github.com/vyperlang/titanoboa
 ```
 
+
 If you are installing titanoboa from git alongside brownie, you may have to manually install titanoboa *after* installing brownie
 
 ```
 pip install brownie
 pip install git+https://github.com/vyperlang/titanoboa
 ```
 
 To get a performance boost for mainnet forking, install with the `forking-recommended` extra (`pip install "git+https://github.com/vyperlang/titanoboa#egg=titanoboa[forking-recommended]"`, or `pip install titanoboa[forking-recommended]`). This installs `plyvel` to cache RPC results between sessions, and `ujson` which improves json performance.
 
 If you are running titanoboa on a local [Vyper](https://github.com/vyperlang/vyper) project folder, you might need to run `python setup.py install` on your [Vyper](https://github.com/vyperlang/vyper) project if you encounter errors such as `ModuleNotFoundError: No module named 'vyper.version'`
+
 ## Background
 
-Titanoboa (/tiˌtɑːnoʊˈboʊə/) is an extinct genus of very large snakes that lived in what is now La Guajira in northeastern Colombia. They could grow up to 12.8 m (42 ft), perhaps even 14.3 m (47 ft) long and reach a weight of 1,135 kg (2,500 lb). This snake lived during the Middle to Late Paleocene epoch, around 60 to 58 million years ago following the extinction of the dinosaurs. Although originally thought to be an apex predator, the discovery of skull bones revealed that it was more than likely specialized in preying on fish. The only known species is Titanoboa cerrejonensis, the largest snake ever discovered,[1] which supplanted the previous record holder, Gigantophis garstini.[2]
+Titanoboa (/ˌtaɪtənəˈboʊə/;[1] lit. 'titanic boa') is an extinct genus of very large snakes that lived in what is now La Guajira in northeastern Colombia. They could grow up to 12.8 m (42 ft), perhaps even 14.3 m (47 ft) long and reach a body mass of 730–1,135 kg (1,610–2,500 lb). This snake lived during the Middle to Late Paleocene epoch, around 60 to 58 million years ago, following the extinction of all non-avian dinosaurs. Although originally thought to be an apex predator, the discovery of skull bones revealed that it was more than likely specialized in preying on fish. The only known species is Titanoboa cerrejonensis, the largest snake ever discovered,[2] which supplanted the previous record holder, Gigantophis garstini.[3]
 
-## Usage
+## Usage / Quick Start
 
 ### Hello, world
 
 ```python
 import boa
 boa.eval("empty(uint256)")
 ```
@@ -94,15 +109,15 @@
 >>> blueprint = s.deploy_as_blueprint()
 >>> deployer = boa.load("examples/deployer.vy", blueprint)
 >>> token = s.at(deployer.create_new_erc20("token", "TKN", 18, 10**18))
 >>> token.totalSupply()
 >>> 1000000000000000000000000000000000000
 ```
 
-### Expecting BoaErrors
+### Expecting BoaErrors / handling reverts
 ```python
 >>> import boa
 >>> erc20 = boa.load("examples/ERC20.vy", "titanoboa", "boa", 18, 0)
 >>> with boa.env.prank(boa.env.generate_address()):
 ...     with boa.reverts():
 ...         erc20.mint(boa.env.eoa, 100)  # non-minter cannot mint
 ...
@@ -119,26 +134,26 @@
         import boa
         boa.interpret.set_cache_dir()  # cache source compilations across sessions
 
 In [2]: %vyper msg.sender  # evaluate a vyper expression directly
 Out[2]: '0x0000000000000000000000000000000000000065'
 
 In [3]: %%vyper
-   ...: 
+   ...:
    ...: MY_IMMUTABLE: immutable(uint256)
-   ...: 
+   ...:
    ...: @external
    ...: def __init__(some_number: uint256):
    ...:     MY_IMMUTABLE = some_number * 2
-   ...: 
+   ...:
    ...: @external
    ...: def foo() -> uint256:
    ...:     return MY_IMMUTABLE
-   ...: 
-Out[3]: <boa.contract.VyperDeployer at 0x7f3496187190>
+   ...:
+Out[3]: <boa.vyper.contract.VyperDeployer at 0x7f3496187190>
 
 In [4]: d = _
 
 In [4]: c = d.deploy(5)
 
 In [5]: c.foo()
 Out[5]: 10
@@ -172,19 +187,19 @@
 In [1]: import boa; boa.env.fork(url="<rpc server address>")
 
 In [2]: %load_ext boa.ipython
 
 In [3]: %%vyper Test
    ...: interface HasName:
    ...:     def name() -> String[32]: view
-   ...: 
+   ...:
    ...: @external
    ...: def get_name_of(addr: HasName) -> String[32]:
    ...:     return addr.name()
-Out[3]: <boa.contract.VyperDeployer at 0x7f3496187190>
+Out[3]: <boa.vyper.contract.VyperDeployer at 0x7f3496187190>
 
 In [4]: c = Test.deploy()
 
 In [5]: c.get_name_of("0xD533a949740bb3306d119CC777fa900bA034cd52")
 Out[5]: 'Curve DAO Token'
 ```
 
@@ -194,9 +209,9 @@
 >>> c = boa.load_partial("examples/ERC20.vy").at("0xD533a949740bb3306d119CC777fa900bA034cd52")
 >>> c.name()
     'Curve DAO Token'
 ```
 
 basic tests:
 ```bash
-$ python -m tests.sim_veYFI
+$ python -m tests.integration.sim_veYFI
 ```
```

