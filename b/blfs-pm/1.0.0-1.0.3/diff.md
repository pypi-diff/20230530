# Comparing `tmp/blfs-pm-1.0.0.tar.gz` & `tmp/blfs-pm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blfs-pm-1.0.0.tar", last modified: Wed Apr 19 06:36:40 2023, max compression
+gzip compressed data, was "blfs-pm-1.0.3.tar", last modified: Tue May 30 21:14:32 2023, max compression
```

## Comparing `blfs-pm-1.0.0.tar` & `blfs-pm-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:36:40.480466 blfs-pm-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-19 06:36:23.000000 blfs-pm-1.0.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-19 06:36:23.000000 blfs-pm-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-19 06:36:23.000000 blfs-pm-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-19 06:36:40.480466 blfs-pm-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-19 06:36:23.000000 blfs-pm-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:36:40.480466 blfs-pm-1.0.0/blfs_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 06:36:23.000000 blfs-pm-1.0.0/blfs_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-19 06:36:23.000000 blfs-pm-1.0.0/blfs_manager/blfspm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-19 06:36:23.000000 blfs-pm-1.0.0/blfs_manager/bootstrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-04-19 06:36:23.000000 blfs-pm-1.0.0/blfs_manager/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-19 06:36:23.000000 blfs-pm-1.0.0/blfs_manager/define.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-19 06:36:23.000000 blfs-pm-1.0.0/blfs_manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:36:40.480466 blfs-pm-1.0.0/blfs_pm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-19 06:36:40.000000 blfs-pm-1.0.0/blfs_pm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-19 06:36:40.000000 blfs-pm-1.0.0/blfs_pm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 06:36:40.000000 blfs-pm-1.0.0/blfs_pm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 06:36:40.000000 blfs-pm-1.0.0/blfs_pm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 06:36:40.000000 blfs-pm-1.0.0/blfs_pm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 06:36:40.000000 blfs-pm-1.0.0/blfs_pm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-19 06:36:23.000000 blfs-pm-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 06:36:40.480466 blfs-pm-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-19 06:36:23.000000 blfs-pm-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:14:32.338383 blfs-pm-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-30 21:14:20.000000 blfs-pm-1.0.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-30 21:14:20.000000 blfs-pm-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-30 21:14:20.000000 blfs-pm-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-30 21:14:32.338383 blfs-pm-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-30 21:14:20.000000 blfs-pm-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:14:32.338383 blfs-pm-1.0.3/blfs_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 21:14:20.000000 blfs-pm-1.0.3/blfs_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-30 21:14:20.000000 blfs-pm-1.0.3/blfs_manager/blfspm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-30 21:14:20.000000 blfs-pm-1.0.3/blfs_manager/bootstrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-30 21:14:20.000000 blfs-pm-1.0.3/blfs_manager/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-30 21:14:20.000000 blfs-pm-1.0.3/blfs_manager/define.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-30 21:14:20.000000 blfs-pm-1.0.3/blfs_manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:14:32.338383 blfs-pm-1.0.3/blfs_pm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-30 21:14:32.000000 blfs-pm-1.0.3/blfs_pm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-30 21:14:32.000000 blfs-pm-1.0.3/blfs_pm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:14:32.000000 blfs-pm-1.0.3/blfs_pm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 21:14:32.000000 blfs-pm-1.0.3/blfs_pm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-30 21:14:32.000000 blfs-pm-1.0.3/blfs_pm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 21:14:32.000000 blfs-pm-1.0.3/blfs_pm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-30 21:14:20.000000 blfs-pm-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:14:32.338383 blfs-pm-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-30 21:14:20.000000 blfs-pm-1.0.3/setup.py
```

### Comparing `blfs-pm-1.0.0/AUTHORS.md` & `blfs-pm-1.0.3/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `blfs-pm-1.0.0/LICENSE` & `blfs-pm-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blfs-pm-1.0.0/PKG-INFO` & `blfs-pm-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blfs-pm
-Version: 1.0.0
+Version: 1.0.3
 Summary: Package manager for Beyond Linux from Scratch (BLFS) system
 Home-page: https://github.com/ahron-maslin/BLFS-automation
 Maintainer: Aharon Maslin
 Maintainer-email: aronmas613@gmail.com
 License: LGPL
 Keywords: BLFS,LFS,Package Manager,automation
 Platform: Linux
@@ -40,35 +40,29 @@
     <li>A working internet connection - you may need to install a couple of BLFS packages like NetworkManager, DHCPClient, and WPA-supplicant.</li>
     <li>A working Python environment</li>
     <li>Python3 package manager (Pip)</li>
     <li>Git (https://www.linuxfromscratch.org/blfs/view/svn/general/git.html)</li>
 </ul>
 
 ### Installation:
-1. Clone this repository:
-```
-git clone https://github.com/ahron-maslin/BLFS-automation.git 
-```
 
-2. Install the requirements:
 ```
-sudo pip install -r requirements.txt
+pip install blfs-pm
 ```
-Note: Installing the requirements, must be done as root - this fixes a bug where the ```wget``` module does not get imported.
 
 ## Usage:
 It is recommended that the package should always be run as root, in order to prevent errors when installing packages to the system.
 
 
 This package has many options to list, download, list commands, or install a given package.
 Note: once again it is *highly* recommended that you always run this as ```root```!
 
-Main usage: ```blfs-pm [-h] [-a] [-b PACKAGE] [-c PACKAGE] [-d PACKAGE] [-f] [-l PACKAGE] [-o] [-r] [-s PACKAGE] [--systemd]```
+Usage: ```blfs-pm [-h] [-a] [-b PACKAGE] [-c PACKAGE] [-d PACKAGE] [-f] [-l PACKAGE] [-o] [-r] [-s PACKAGE] [--systemd]```
 
-Note: It is recommended to follow along the installation process in the BLFS book. ```blfs-m``` is not perfect and I have not tested every BLFS package. There are still some issues with circular dependencies, and at the moment it is best to monitor everything to prevent problems. Additionally, the ```-b (build)``` option will prompt the user to run EVERY command provided for the specific package. Some commands can only be run if optional dependencies are installed (like Texlive, Docbook, etc.). Furthermore, some packages require further kernel configuration (and recompilation) as a prerequisite for installation.
+Note: It is recommended to follow along the installation process in the BLFS book. ```blfs-pm``` is not perfect and I have not tested every BLFS package. There are still some issues with circular dependencies, and at the moment it is best to monitor everything to prevent problems. Additionally, the ```-b (build)``` option will prompt the user to run EVERY command provided for the specific package. Some commands can only be run if optional dependencies are installed (like Texlive, Docbook, etc.). Furthermore, some packages require further kernel configuration (and recompilation) as a prerequisite for installation.
 
 ```
   -h, --help                        show this help message and exit
 
   -a, --all                         Downloads ALL BLFS packages - uses a lot of time and space.
 
   -b PACKAGE, --build PACKAGE       Install a given Package on the system.
```

### Comparing `blfs-pm-1.0.0/README.rst` & `blfs-pm-1.0.3/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 BLFS-automation:
 ================
 
-A simple python script to ease your BLFS project in many ways…
+“A simple Python package that simplifies your BLFS project in many
+ways…”
 
 About this project:
 -------------------
 
 This project is designed for people who have built their own
 LinuxFromScratch (LFS) system, and are now working on the next stage -
 BeyondLinuxFromScratch (BLFS). BLFS packages often require many other
 dependencies to work, and sometimes it is a bit cumbersome to install
-all of those.
+all of those. ``blfs-pm`` aims to make it easier to install these
+packages without the stress of downloading everything and calculating,
+while simultaneously allowing you to still get the full build
+experience.
 
 Download and installation:
 --------------------------
 
 To get a local copy up and running follow these steps.
 
 Prerequisites:
@@ -79,47 +83,35 @@
 .. raw:: html
 
    </ul>
 
 Installation:
 ~~~~~~~~~~~~~
 
-1. Clone this repository:
-
-::
-
-   git clone https://github.com/ahron-maslin/BLFS-automation.git 
-
-2. Install the requirements:
-
 ::
 
-   sudo pip install -r requirements.txt
-
-Note: Installing the requirements, must be done as root - this fixes a
-bug where the ``wget`` module does not get imported.
+   pip install blfs-pm
 
 Usage:
 ------
 
-It is recommended that the main script ``deps.py`` should always be run
-as root, in order to prevent errors when installing packages to the
-system.
+It is recommended that the package should always be run as root, in
+order to prevent errors when installing packages to the system.
 
 This package has many options to list, download, list commands, or
 install a given package. Note: once again it is *highly* recommended
 that you always run this as ``root``!
 
-Main usage:
-``blfs-pm [-h] [-a] [-b PACKAGE] [-c PACKAGE] [-d PACKAGE] [-e PACKAGE] [-f] [-l PACKAGE] [-o] [-r] [-s PACKAGE]``
+Usage:
+``blfs-pm [-h] [-a] [-b PACKAGE] [-c PACKAGE] [-d PACKAGE] [-f] [-l PACKAGE] [-o] [-r] [-s PACKAGE] [--systemd]``
 
 Note: It is recommended to follow along the installation process in the
-BLFS book. This tool is not perfect and I have not tested every BLFS
+BLFS book. ``blfs-pm`` is not perfect and I have not tested every BLFS
 package. There are still some issues with circular dependencies, and at
-the moment it is best to moniter everything to prevent problems.
+the moment it is best to monitor everything to prevent problems.
 Additionally, the ``-b (build)`` option will prompt the user to run
 EVERY command provided for the specific package. Some commands can only
 be run if optional dependencies are installed (like Texlive, Docbook,
 etc.). Furthermore, some packages require further kernel configuration
 (and recompilation) as a prerequisite for installation.
 
 ::
@@ -130,32 +122,33 @@
 
      -b PACKAGE, --build PACKAGE       Install a given Package on the system.
 
      -c PACKAGE, --commands PACKAGE    List installation (without installing) commands for a given package.
      
      -d PACKAGE, --download PACKAGE    Downloads a given BLFS package along with all of its dependencies.
 
-     -e PACKAGE, --everything PACKAGE  Downloads and installs the given package with all of it's dependencies.
-
      -f, --force                       Force package installation even though it is already installed
 
      -l PACKAGE, --list PACKAGE        Lists all of the dependencies for a given BLFS package in order of installation.
 
      -o, --optional                    List/download optional packages.
 
      -r, --recommended                 List/download recommended packages.
 
      -s PACKAGE, --search PACKAGE      Search for a given package.
+     --systemd                         Pass this flag if you built LFS with Systemd
 
 Additional options:
 -------------------
 
 Contributers:
 -------------
 
 Ahron Maslin (creator, maintainer, and designer), Josh W. (moral
 support), Dan the Man (Chief Psychologist)
 
 Todo
 ----
 
--  implement different db’s for different LFS versions
+-  [ ] implement different db’s for different LFS versions
+-  [ ] add ``--info`` flag to display information about a package
+-  [ ] query to install a package if only one search result was found
```

### Comparing `blfs-pm-1.0.0/blfs_manager/blfspm.py` & `blfs-pm-1.0.3/blfs_manager/blfspm.py`

 * *Files identical despite different names*

### Comparing `blfs-pm-1.0.0/blfs_manager/bootstrapper.py` & `blfs-pm-1.0.3/blfs_manager/bootstrapper.py`

 * *Files identical despite different names*

### Comparing `blfs-pm-1.0.0/blfs_manager/commands.py` & `blfs-pm-1.0.3/blfs_manager/commands.py`

 * *Files identical despite different names*

### Comparing `blfs-pm-1.0.0/blfs_manager/define.py` & `blfs-pm-1.0.3/blfs_manager/define.py`

 * *Files identical despite different names*

### Comparing `blfs-pm-1.0.0/blfs_manager/utils.py` & `blfs-pm-1.0.3/blfs_manager/utils.py`

 * *Files identical despite different names*

### Comparing `blfs-pm-1.0.0/blfs_pm.egg-info/PKG-INFO` & `blfs-pm-1.0.3/blfs_pm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blfs-pm
-Version: 1.0.0
+Version: 1.0.3
 Summary: Package manager for Beyond Linux from Scratch (BLFS) system
 Home-page: https://github.com/ahron-maslin/BLFS-automation
 Maintainer: Aharon Maslin
 Maintainer-email: aronmas613@gmail.com
 License: LGPL
 Keywords: BLFS,LFS,Package Manager,automation
 Platform: Linux
@@ -40,35 +40,29 @@
     <li>A working internet connection - you may need to install a couple of BLFS packages like NetworkManager, DHCPClient, and WPA-supplicant.</li>
     <li>A working Python environment</li>
     <li>Python3 package manager (Pip)</li>
     <li>Git (https://www.linuxfromscratch.org/blfs/view/svn/general/git.html)</li>
 </ul>
 
 ### Installation:
-1. Clone this repository:
-```
-git clone https://github.com/ahron-maslin/BLFS-automation.git 
-```
 
-2. Install the requirements:
 ```
-sudo pip install -r requirements.txt
+pip install blfs-pm
 ```
-Note: Installing the requirements, must be done as root - this fixes a bug where the ```wget``` module does not get imported.
 
 ## Usage:
 It is recommended that the package should always be run as root, in order to prevent errors when installing packages to the system.
 
 
 This package has many options to list, download, list commands, or install a given package.
 Note: once again it is *highly* recommended that you always run this as ```root```!
 
-Main usage: ```blfs-pm [-h] [-a] [-b PACKAGE] [-c PACKAGE] [-d PACKAGE] [-f] [-l PACKAGE] [-o] [-r] [-s PACKAGE] [--systemd]```
+Usage: ```blfs-pm [-h] [-a] [-b PACKAGE] [-c PACKAGE] [-d PACKAGE] [-f] [-l PACKAGE] [-o] [-r] [-s PACKAGE] [--systemd]```
 
-Note: It is recommended to follow along the installation process in the BLFS book. ```blfs-m``` is not perfect and I have not tested every BLFS package. There are still some issues with circular dependencies, and at the moment it is best to monitor everything to prevent problems. Additionally, the ```-b (build)``` option will prompt the user to run EVERY command provided for the specific package. Some commands can only be run if optional dependencies are installed (like Texlive, Docbook, etc.). Furthermore, some packages require further kernel configuration (and recompilation) as a prerequisite for installation.
+Note: It is recommended to follow along the installation process in the BLFS book. ```blfs-pm``` is not perfect and I have not tested every BLFS package. There are still some issues with circular dependencies, and at the moment it is best to monitor everything to prevent problems. Additionally, the ```-b (build)``` option will prompt the user to run EVERY command provided for the specific package. Some commands can only be run if optional dependencies are installed (like Texlive, Docbook, etc.). Furthermore, some packages require further kernel configuration (and recompilation) as a prerequisite for installation.
 
 ```
   -h, --help                        show this help message and exit
 
   -a, --all                         Downloads ALL BLFS packages - uses a lot of time and space.
 
   -b PACKAGE, --build PACKAGE       Install a given Package on the system.
```

### Comparing `blfs-pm-1.0.0/setup.py` & `blfs-pm-1.0.3/setup.py`

 * *Files identical despite different names*

