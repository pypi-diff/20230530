# Comparing `tmp/gitautobackup-1.0.1.1.tar.gz` & `tmp/gitautobackup-1.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Soft(withgit)\~Legacy\gitautobackup\dist\.tmp-euypp9z1\gitautobackup-1.0.1.1.tar", last modified: Tue May 30 17:47:48 2023, max compression
+gzip compressed data, was "D:\Soft(withgit)\~Legacy\gitautobackup\dist\.tmp-6mf82_fp\gitautobackup-1.0.1.2.tar", last modified: Tue May 30 18:29:25 2023, max compression
```

## Comparing `gitautobackup-1.0.1.1.tar` & `gitautobackup-1.0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 17:47:48.000000 gitautobackup-1.0.1.1/
--rw-rw-rw-   0        0        0    17098 2022-07-31 18:44:36.000000 gitautobackup-1.0.1.1/LICENSE
--rw-rw-rw-   0        0        0    27624 2023-05-30 17:47:48.000000 gitautobackup-1.0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5971 2023-05-30 16:22:48.000000 gitautobackup-1.0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 17:47:48.000000 gitautobackup-1.0.1.1/gitautobackup.egg-info/
--rw-rw-rw-   0        0        0    27624 2023-05-30 17:47:48.000000 gitautobackup-1.0.1.1/gitautobackup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-05-30 17:47:48.000000 gitautobackup-1.0.1.1/gitautobackup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 17:47:48.000000 gitautobackup-1.0.1.1/gitautobackup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-30 17:47:48.000000 gitautobackup-1.0.1.1/gitautobackup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2023-05-30 17:47:48.000000 gitautobackup-1.0.1.1/gitautobackup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-30 17:47:48.000000 gitautobackup-1.0.1.1/gitautobackup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-30 17:45:53.000000 gitautobackup-1.0.1.1/gitautobackup.egg-info/zip-safe
--rw-rw-rw-   0        0        0    15740 2023-05-30 16:31:44.000000 gitautobackup-1.0.1.1/gitautobackup.py
--rw-rw-rw-   0        0        0     2568 2023-05-30 17:47:37.000000 gitautobackup-1.0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 17:47:48.000000 gitautobackup-1.0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 18:29:25.000000 gitautobackup-1.0.1.2/
+-rw-rw-rw-   0        0        0    17098 2023-05-30 17:53:38.000000 gitautobackup-1.0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    27921 2023-05-30 18:29:25.000000 gitautobackup-1.0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6268 2023-05-30 18:15:21.000000 gitautobackup-1.0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 18:29:25.000000 gitautobackup-1.0.1.2/gitautobackup.egg-info/
+-rw-rw-rw-   0        0        0    27921 2023-05-30 18:29:25.000000 gitautobackup-1.0.1.2/gitautobackup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-05-30 18:29:25.000000 gitautobackup-1.0.1.2/gitautobackup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 18:29:25.000000 gitautobackup-1.0.1.2/gitautobackup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-30 18:29:25.000000 gitautobackup-1.0.1.2/gitautobackup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2023-05-30 18:29:25.000000 gitautobackup-1.0.1.2/gitautobackup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-30 18:29:25.000000 gitautobackup-1.0.1.2/gitautobackup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-30 17:45:53.000000 gitautobackup-1.0.1.2/gitautobackup.egg-info/zip-safe
+-rw-rw-rw-   0        0        0    16051 2023-05-30 18:27:59.000000 gitautobackup-1.0.1.2/gitautobackup.py
+-rw-rw-rw-   0        0        0     2558 2023-05-30 18:21:14.000000 gitautobackup-1.0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 18:29:25.000000 gitautobackup-1.0.1.2/setup.cfg
```

### Comparing `gitautobackup-1.0.1.1/LICENSE` & `gitautobackup-1.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gitautobackup-1.0.1.1/PKG-INFO` & `gitautobackup-1.0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitautobackup
-Version: 1.0.1.1
+Version: 1.0.1.2
 Summary: A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools
 Author-email: Markus Hammer <107761433+MarkusHammer@users.noreply.github.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -405,31 +405,31 @@
 
 # Git Auto Backup Tool
 
 A basic CLI program and python module that allows for quickly making and comming changes to a git repository, along with a few other tools. Use it from the command line or import it as a module, it works both ways!
 
 ## Setup
 
+First off, this script uses the ``GitPython`` module, so ensure that you have a compatable version of git installed on you system so that ``GitPython`` can interface with it properly. For more info look [here](https://github.com/gitpython-developers/GitPython).
+
 If not installed via pip, than the requirements for this script must be installed in the python environment. This script requires the ``git`` python module be available in you python environment in order to run. This can also use the ``argparse`` module optionally to help greatly increase the usability on the command line (and is highly suggested). These can be installed using:
 
-``pip install git argparse[cli]``
+``pip install gitautobackup[cli]``
 
 or if you just want the module without the extra cli overhead:
 
-``pip install git argparse``
+``pip install gitautobackup``
 
-If you prefer to have this a s a standalone file and are **sure** that you have all dependences satisfied in some way you can also simply clone this repo into your project and import the ``gitautobackup.py`` file locally.
+If you prefer to have this as a standalone file and are **sure** that you have all dependences satisfied in some way you can also simply clone this repo into your project and import the ``gitautobackup.py`` file locally.
 
 ## Command Line Interface
 
-depending on how you set up this file on you system you can run this module using ``python -m gitautobackup`` if you set it up using pip or ``python ./gitautobackup.py`` or ``py ./gitautobackup.py`` if you have the gitautobackup file locally.
-
-While this module does not explicitly require the ``argparse`` module, it is **highly** suggested as it help greatly improve the usability and allows acess to more options.
+Depending on how you set up this file on your system, you can run this module using ``python -m gitautobackup`` if you set it up using pip, or ``python ./gitautobackup.py`` or ``py ./gitautobackup.py`` if you have the gitautobackup file locally.
 
-If in doubt just install ``argparse``.
+While this module does not explicitly require the ``argparse`` module, it is **highly** suggested as it help greatly improve the usability and allows acess to more options. If in doubt just install ``argparse`` if you can.
 
 ### With ``argparse``
 
 This module does not have any required arguments, as everything does have a default behaviour. The most importnant thing to note is that when not supplied with the path of the git repository, it attempts to deduce the location of a git repository (by testing if the directory is able to be loaded as a git repository) from (in this specific order):
 
 1. The console's current working direcory
 2. The directory given in the 0th arg of the command line (aka ``sys.argv[0]``'s lowest directory)
@@ -448,31 +448,31 @@
 
 - ``--ver`` or ``--version`` prints the program version and then exits. You don't need a input file if you run this command.
 - ``-h`` or ``--help`` prints some details about the programs arguments and then exits. You don't need a input file if you run this command.
 - ``--git`` or ``--github`` prints a like to the github repository and then exits. You don't need a input file if you run this command.
 
 ### Without ``argparse``
 
-While using this on the command line without argparse is not suggested, you may still access a diminished selection of features:
+While using this on the command line without ``argparse`` is not suggested, you may still access a diminished selection of features:
 
 - The ``-m`` or ``--message`` flag still works
 - The path of the git repository does not require a flag and can simply have it path stated. If multiple paths are given, the first one thats a valid repository will be chosen. The program will explicitly fail if none where given.
 - The ``--help`` and ``-h`` args also work as expected.
 
 ### Command Line Interface Example
 
-If argparse is available:
+If ``argparse`` is available:
 
-```cmd:
+```bash:
 python -m gitautobackup -p "./repo" -m "automatic backup after big change" -f -fc -v
 ```
 
-If argparse is not available:
+If ``argparse`` is not available:
 
-```cmd:
+```bash:
 python -m gitautobackup "./repo" -m "automatic backup after big change"
 ```
 
 ## Module Interface
 
 This module can also be interfaced with as a normal module. The points of intreast include the ``main`` function for interfacing with this just like it was the command line (this means **parsing the arguments**, meaning that the features outlined in the Command Line Interface section above), and the ``auto_git_backup`` command for a more direct ussage of the command.
 While both can manage to acheave the same result its suggested to use ``auto_git_backup`` unless there is a specific reason to use ``main``.
@@ -494,12 +494,12 @@
 
 ## Licence
 
 This is licenced under the Mozilla Public License 2.0 (MPL 2.0) Licence. See the ``Licence`` file in this repository for more information.
 
 ## Credits
 
-This project uses the ``pathlib``, ``git`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
+This project uses the ``pathlib``, ``GitPython`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
 
 While not required, feel free to credit "*Markus Hammer*" (or just "*Markus*") if you find this code or script usefull for whatever you may be doing with it.
 
 **Thanks!**
```

### Comparing `gitautobackup-1.0.1.1/README.md` & `gitautobackup-1.0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # Git Auto Backup Tool
 
 A basic CLI program and python module that allows for quickly making and comming changes to a git repository, along with a few other tools. Use it from the command line or import it as a module, it works both ways!
 
 ## Setup
 
+First off, this script uses the ``GitPython`` module, so ensure that you have a compatable version of git installed on you system so that ``GitPython`` can interface with it properly. For more info look [here](https://github.com/gitpython-developers/GitPython).
+
 If not installed via pip, than the requirements for this script must be installed in the python environment. This script requires the ``git`` python module be available in you python environment in order to run. This can also use the ``argparse`` module optionally to help greatly increase the usability on the command line (and is highly suggested). These can be installed using:
 
-``pip install git argparse[cli]``
+``pip install gitautobackup[cli]``
 
 or if you just want the module without the extra cli overhead:
 
-``pip install git argparse``
+``pip install gitautobackup``
 
-If you prefer to have this a s a standalone file and are **sure** that you have all dependences satisfied in some way you can also simply clone this repo into your project and import the ``gitautobackup.py`` file locally.
+If you prefer to have this as a standalone file and are **sure** that you have all dependences satisfied in some way you can also simply clone this repo into your project and import the ``gitautobackup.py`` file locally.
 
 ## Command Line Interface
 
-depending on how you set up this file on you system you can run this module using ``python -m gitautobackup`` if you set it up using pip or ``python ./gitautobackup.py`` or ``py ./gitautobackup.py`` if you have the gitautobackup file locally.
-
-While this module does not explicitly require the ``argparse`` module, it is **highly** suggested as it help greatly improve the usability and allows acess to more options.
+Depending on how you set up this file on your system, you can run this module using ``python -m gitautobackup`` if you set it up using pip, or ``python ./gitautobackup.py`` or ``py ./gitautobackup.py`` if you have the gitautobackup file locally.
 
-If in doubt just install ``argparse``.
+While this module does not explicitly require the ``argparse`` module, it is **highly** suggested as it help greatly improve the usability and allows acess to more options. If in doubt just install ``argparse`` if you can.
 
 ### With ``argparse``
 
 This module does not have any required arguments, as everything does have a default behaviour. The most importnant thing to note is that when not supplied with the path of the git repository, it attempts to deduce the location of a git repository (by testing if the directory is able to be loaded as a git repository) from (in this specific order):
 
 1. The console's current working direcory
 2. The directory given in the 0th arg of the command line (aka ``sys.argv[0]``'s lowest directory)
@@ -43,31 +43,31 @@
 
 - ``--ver`` or ``--version`` prints the program version and then exits. You don't need a input file if you run this command.
 - ``-h`` or ``--help`` prints some details about the programs arguments and then exits. You don't need a input file if you run this command.
 - ``--git`` or ``--github`` prints a like to the github repository and then exits. You don't need a input file if you run this command.
 
 ### Without ``argparse``
 
-While using this on the command line without argparse is not suggested, you may still access a diminished selection of features:
+While using this on the command line without ``argparse`` is not suggested, you may still access a diminished selection of features:
 
 - The ``-m`` or ``--message`` flag still works
 - The path of the git repository does not require a flag and can simply have it path stated. If multiple paths are given, the first one thats a valid repository will be chosen. The program will explicitly fail if none where given.
 - The ``--help`` and ``-h`` args also work as expected.
 
 ### Command Line Interface Example
 
-If argparse is available:
+If ``argparse`` is available:
 
-```cmd:
+```bash:
 python -m gitautobackup -p "./repo" -m "automatic backup after big change" -f -fc -v
 ```
 
-If argparse is not available:
+If ``argparse`` is not available:
 
-```cmd:
+```bash:
 python -m gitautobackup "./repo" -m "automatic backup after big change"
 ```
 
 ## Module Interface
 
 This module can also be interfaced with as a normal module. The points of intreast include the ``main`` function for interfacing with this just like it was the command line (this means **parsing the arguments**, meaning that the features outlined in the Command Line Interface section above), and the ``auto_git_backup`` command for a more direct ussage of the command.
 While both can manage to acheave the same result its suggested to use ``auto_git_backup`` unless there is a specific reason to use ``main``.
@@ -89,12 +89,12 @@
 
 ## Licence
 
 This is licenced under the Mozilla Public License 2.0 (MPL 2.0) Licence. See the ``Licence`` file in this repository for more information.
 
 ## Credits
 
-This project uses the ``pathlib``, ``git`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
+This project uses the ``pathlib``, ``GitPython`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
 
 While not required, feel free to credit "*Markus Hammer*" (or just "*Markus*") if you find this code or script usefull for whatever you may be doing with it.
 
 **Thanks!**
```

### Comparing `gitautobackup-1.0.1.1/gitautobackup.egg-info/PKG-INFO` & `gitautobackup-1.0.1.2/gitautobackup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitautobackup
-Version: 1.0.1.1
+Version: 1.0.1.2
 Summary: A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools
 Author-email: Markus Hammer <107761433+MarkusHammer@users.noreply.github.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -405,31 +405,31 @@
 
 # Git Auto Backup Tool
 
 A basic CLI program and python module that allows for quickly making and comming changes to a git repository, along with a few other tools. Use it from the command line or import it as a module, it works both ways!
 
 ## Setup
 
+First off, this script uses the ``GitPython`` module, so ensure that you have a compatable version of git installed on you system so that ``GitPython`` can interface with it properly. For more info look [here](https://github.com/gitpython-developers/GitPython).
+
 If not installed via pip, than the requirements for this script must be installed in the python environment. This script requires the ``git`` python module be available in you python environment in order to run. This can also use the ``argparse`` module optionally to help greatly increase the usability on the command line (and is highly suggested). These can be installed using:
 
-``pip install git argparse[cli]``
+``pip install gitautobackup[cli]``
 
 or if you just want the module without the extra cli overhead:
 
-``pip install git argparse``
+``pip install gitautobackup``
 
-If you prefer to have this a s a standalone file and are **sure** that you have all dependences satisfied in some way you can also simply clone this repo into your project and import the ``gitautobackup.py`` file locally.
+If you prefer to have this as a standalone file and are **sure** that you have all dependences satisfied in some way you can also simply clone this repo into your project and import the ``gitautobackup.py`` file locally.
 
 ## Command Line Interface
 
-depending on how you set up this file on you system you can run this module using ``python -m gitautobackup`` if you set it up using pip or ``python ./gitautobackup.py`` or ``py ./gitautobackup.py`` if you have the gitautobackup file locally.
-
-While this module does not explicitly require the ``argparse`` module, it is **highly** suggested as it help greatly improve the usability and allows acess to more options.
+Depending on how you set up this file on your system, you can run this module using ``python -m gitautobackup`` if you set it up using pip, or ``python ./gitautobackup.py`` or ``py ./gitautobackup.py`` if you have the gitautobackup file locally.
 
-If in doubt just install ``argparse``.
+While this module does not explicitly require the ``argparse`` module, it is **highly** suggested as it help greatly improve the usability and allows acess to more options. If in doubt just install ``argparse`` if you can.
 
 ### With ``argparse``
 
 This module does not have any required arguments, as everything does have a default behaviour. The most importnant thing to note is that when not supplied with the path of the git repository, it attempts to deduce the location of a git repository (by testing if the directory is able to be loaded as a git repository) from (in this specific order):
 
 1. The console's current working direcory
 2. The directory given in the 0th arg of the command line (aka ``sys.argv[0]``'s lowest directory)
@@ -448,31 +448,31 @@
 
 - ``--ver`` or ``--version`` prints the program version and then exits. You don't need a input file if you run this command.
 - ``-h`` or ``--help`` prints some details about the programs arguments and then exits. You don't need a input file if you run this command.
 - ``--git`` or ``--github`` prints a like to the github repository and then exits. You don't need a input file if you run this command.
 
 ### Without ``argparse``
 
-While using this on the command line without argparse is not suggested, you may still access a diminished selection of features:
+While using this on the command line without ``argparse`` is not suggested, you may still access a diminished selection of features:
 
 - The ``-m`` or ``--message`` flag still works
 - The path of the git repository does not require a flag and can simply have it path stated. If multiple paths are given, the first one thats a valid repository will be chosen. The program will explicitly fail if none where given.
 - The ``--help`` and ``-h`` args also work as expected.
 
 ### Command Line Interface Example
 
-If argparse is available:
+If ``argparse`` is available:
 
-```cmd:
+```bash:
 python -m gitautobackup -p "./repo" -m "automatic backup after big change" -f -fc -v
 ```
 
-If argparse is not available:
+If ``argparse`` is not available:
 
-```cmd:
+```bash:
 python -m gitautobackup "./repo" -m "automatic backup after big change"
 ```
 
 ## Module Interface
 
 This module can also be interfaced with as a normal module. The points of intreast include the ``main`` function for interfacing with this just like it was the command line (this means **parsing the arguments**, meaning that the features outlined in the Command Line Interface section above), and the ``auto_git_backup`` command for a more direct ussage of the command.
 While both can manage to acheave the same result its suggested to use ``auto_git_backup`` unless there is a specific reason to use ``main``.
@@ -494,12 +494,12 @@
 
 ## Licence
 
 This is licenced under the Mozilla Public License 2.0 (MPL 2.0) Licence. See the ``Licence`` file in this repository for more information.
 
 ## Credits
 
-This project uses the ``pathlib``, ``git`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
+This project uses the ``pathlib``, ``GitPython`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
 
 While not required, feel free to credit "*Markus Hammer*" (or just "*Markus*") if you find this code or script usefull for whatever you may be doing with it.
 
 **Thanks!**
```

### Comparing `gitautobackup-1.0.1.1/gitautobackup.py` & `gitautobackup-1.0.1.2/gitautobackup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 '''
     autoback: A simple python script and module to make a automatic backup of a git repository.
     Includes both a CLI interface as well as a module interface for individual functions as well as
         a function that accepts arguments like the CLI interface.
+    
+    By Markus Hammer 2023
+
+    Licenced under the Mozilla Public License 2.0 (MPL 2.0)
+    Read the included 'LICENCE' file for more information.
+
+    See the github repo for more info!
+    
+    This project is on github here:
+    https://github.com/MarkusHammer/gitautobackup
 '''
 
 # I mean I know its good pratice but I do not care for reformating all
 #  my docstrings and making the file less readable just so it fits on smaller screens.
 # No its not a run on sentince problem I can stop anytime I want damn it!
 # pylint: disable=C0301
 
@@ -19,15 +29,15 @@
 from git import Repo, InvalidGitRepositoryError
 
 try:
     from typing import Union
 except ImportError:
     from typing_extensions import Union
 
-__version__ = "1.0.1.1"
+__version__ = "1.0.1.2"
 
 def path_hunt_dir(path: Union[Path, str, None]) -> Union['Path', None]:
     """_summary_
 
     Args:
         path (Union[Path,str,None]): The path to search for the parent directory of. If this is set to None the return value will always also be None
 
@@ -135,15 +145,15 @@
         return possiblepath
 
     try:
         from sys import (argv as cliargv)
     except ImportError:
         pass
     else:
-        if len(argv) > 0 and isinstance(cliargv[0], str):
+        if len(cliargv) > 0 and isinstance(cliargv[0], str):
             possiblepath = path_hunt_dir(cliargv[0])
             if possiblepath is not None and possiblepath.exists():
                 return possiblepath
 
     # this only really helps if this file is run as the main script.
     # Unlikely that it will be needed however because argv is almost always guaranteed
     #   to work on any system that is able to suport the mandatory requirements of this script anyway.
@@ -344,12 +354,13 @@
 
     if args.verbose:
         print("Making auto backup")
 
     return auto_git_backup(path, commit_message=message, further_guess_paths=further_guess_paths, verbose=verbose, force_commit=force_commit, force_compress=force_compress)
 
 
-__main__ = main
-
-if __name__ == "__main__":
+def __main__():
     from sys import (exit as end, argv)
     end(main(argv[1:], prog_arg=argv[0]))
+
+if __name__ == "__main__":
+    __main__()
```

### Comparing `gitautobackup-1.0.1.1/pyproject.toml` & `gitautobackup-1.0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -63,12 +63,12 @@
 Homepage = "https://github.com/MarkusHammer/gitautobackup"
 Github  = "https://github.com/MarkusHammer/gitautobackup"
 Issues = "https://github.com/MarkusHammer/gitautobackup/issues"
 "Pull Requests" = "https://github.com/MarkusHammer/gitautobackup/pulls"
 Git = "https://github.com/MarkusHammer/gitautobackup.git"
 
 [project.scripts]
-gitautobackup = "gitautobackup.__main__:main"
-#autobackup = "gitautobackup.__main__:main"
+gitautobackup = "gitautobackup:__main__"
+#autobackup = "gitautobackup:__main__"
 
 [tool.setuptools]
 zip-safe = true
```

